# Comparing `tmp/taskproc-0.11.1.tar.gz` & `tmp/taskproc-0.11.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskproc-0.11.1.tar", max compression
+gzip compressed data, was "taskproc-0.11.2.tar", max compression
```

## Comparing `taskproc-0.11.1.tar` & `taskproc-0.11.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7867 2023-05-20 10:00:14.638602 taskproc-0.11.1/README.md
--rw-r--r--   0        0        0      681 2023-05-20 09:59:50.498225 taskproc-0.11.1/pyproject.toml
--rw-r--r--   0        0        0      624 2023-05-19 04:18:19.730222 taskproc-0.11.1/taskproc/__init__.py
--rw-r--r--   0        0        0     2891 2023-05-19 07:13:23.867522 taskproc-0.11.1/taskproc/app.py
--rw-r--r--   0        0        0     4865 2023-05-20 10:01:15.924401 taskproc-0.11.1/taskproc/database.py
--rw-r--r--   0        0        0     7621 2023-05-19 07:06:46.262957 taskproc-0.11.1/taskproc/graph.py
--rw-r--r--   0        0        0    15872 2023-05-19 16:35:18.369038 taskproc-0.11.1/taskproc/task.py
--rw-r--r--   0        0        0     1391 2023-05-18 04:14:19.815251 taskproc-0.11.1/taskproc/types.py
--rw-r--r--   0        0        0     8699 1970-01-01 00:00:00.000000 taskproc-0.11.1/PKG-INFO
+-rw-r--r--   0        0        0     8111 2023-05-21 01:40:12.885265 taskproc-0.11.2/README.md
+-rw-r--r--   0        0        0      681 2023-05-22 07:28:08.234873 taskproc-0.11.2/pyproject.toml
+-rw-r--r--   0        0        0      624 2023-05-19 04:18:19.730222 taskproc-0.11.2/taskproc/__init__.py
+-rw-r--r--   0        0        0     2891 2023-05-19 07:13:23.867522 taskproc-0.11.2/taskproc/app.py
+-rw-r--r--   0        0        0     4865 2023-05-21 01:39:23.593621 taskproc-0.11.2/taskproc/database.py
+-rw-r--r--   0        0        0     7621 2023-05-19 07:06:46.262957 taskproc-0.11.2/taskproc/graph.py
+-rw-r--r--   0        0        0    15554 2023-05-22 07:25:31.589696 taskproc-0.11.2/taskproc/task.py
+-rw-r--r--   0        0        0     1391 2023-05-18 04:14:19.815251 taskproc-0.11.2/taskproc/types.py
+-rw-r--r--   0        0        0     8943 1970-01-01 00:00:00.000000 taskproc-0.11.2/PKG-INFO
```

### Comparing `taskproc-0.11.1/README.md` & `taskproc-0.11.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,22 @@
-# Checkpoint-tool
+# taskproc
 
 A lightweight workflow building/execution/management tool written in pure Python.
-
 Internally, it depends on `DiskCache`, `cloudpickle` `networkx` and `concurrent.futures`.
 
+#### Features
+* Decomposing long and complex computation into tasks, i.e., smaller units of work.
+* Executing them in a distributed way, supporting multithreading, multiprocessing, local clusters/containers.
+* Creating/discarding caches per task and reusing them whenever possible. 
+
+#### Nonfeatures
+* Automatic retry
+* External service integration with remote clusters/containers or cloud platforms (GCP, AWS, ...)
+* Periodic scheduling
+* GUI dashboard
 
 ## Installation
 
 ```
 pip install taskproc
 ```
 
@@ -25,17 +34,16 @@
 # `infer_task_type` decorator helps the type checker to infer the types of the task class. (optional)
 @infer_task_type
 class Choose(TaskBase):
     """ Compute the binomial coefficient. """
     # Inside a task, we first declare the values that must be computed upstream with the descriptor `Req`.
     # In this example, `Choose(n, k)` depends on `Choose(n - 1, k - 1)` and `Choose(n - 1, k)`,
     # so it requires two `int` values.
-    # Either the type annotation `Requires[...]` or the assignment `= Req()` may be omitted.
-    prev1: Requires[int] = Req()
-    prev2: Requires[int] = Req()
+    prev1: Requires[int]
+    prev2: Requires[int]
 
     def build_task(self, n: int, k: int):
         # The prerequisite tasks and the other instance attributes are prepared here.
         # It thus recursively defines all the tasks we need to run this task,
         # i.e., the entire upstream workflow.
 
         if 0 < k < n:
@@ -57,15 +65,15 @@
 
 # To run the task as well as upstream workflow, use the `run_graph()` method.
 ans = Choose(6, 3).run_graph()  # `ans` should be 6 Choose 3, which is 20.
 
 # It greedily executes all the necessary tasks as parallel as possible
 # and then spits out the return value of the task on which we call `run_graph()`.
 # The return values of the intermediate tasks are cached at
-# `{$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/...`
+# `{$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/results/...`
 # and reused on the fly whenever possible.
 ```
 
 ### Deleting cache
 
 It is possible to selectively discard cache: 
 ```python
@@ -79,40 +87,31 @@
 # Delete all the cache associated with `Choose`,
 # equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.Choose`.
 Choose.clear_all_tasks()            
 ```
 
 ### Task IO
 
-The arguments of the `init` method can be anything JSON serializable:
+The arguments of the `build_task` method can be anything JSON serializable including `Task`s:
 ```python
-class T1(TaskBase):
-    def build_task(self, **param1):
-        ...
-    ...
-
-class T2(TaskBase):
-    def build_task(self, **param2):
+class MyTask(TaskBase):
+    def build_task(self, param1, param2):
         ...
-    ...
-
-class T3(TaskBase):
-    x1 = Req()
-    x2 = Req()
-
-    def build_task(self, json_params):
-        self.x1 = T1(**json_params['param1'])
-        self.x2 = T2(**json_params['param2'])
 
-    def run_task(self):
+MyTask(
+    param1={
+        'upstream_task0': UpstreamTask(),
+        'other_params': [1, 2],
         ...
-
-result = T3({'param1': { ... }, 'param2': { ... }}).run_graph()
+    },
+    param2={ ... }
+}).run_graph()
 ```
 
+<!--
 Otherwise they can be passed via `Task` and `Req`:
 ```python
 from taskproc import Task
 Dataset = ...  # Some complex data structure
 Model = ...    # Some complex data structure
 
 class LoadDataset(TaskBase):
@@ -159,56 +158,54 @@
 
     def build_task(self, task_dict: dict[str, Task[float]]):
         self.scores = task_dict
 
     def run_task(self) -> float:
         return sum(self.scores.values()) / len(self.scores)  # We have access to the dict of the results.
 ```
+-->
 
-One can also directly access the items of dictionary-valued upstream tasks.
+The output of the `run_task` method should be serializable with `cloudpickle`,
+which is then compressed with `gzip`.
+The compression level can be changed as follows (defaults to 9).
 ```python
-class MultiOutputTask(TaskBase):
+class NoCompressionTask(TaskBase, compress_level=0):
     ...
+```
 
+If the output is a dictionary, one can directly access its element:
+```python
+class MultiOutputTask(TaskBase):
     def run_task(self) -> dict[str, int]:
         return {'foo': 42, ...}
 
 class DownstreamTask(TaskBase):
     dep: Requires[int]
 
     def build_task(self):
         self.dep = MultiOutputTask()['foo']
 ```
 
-The output of the `run_task` method should be serializable with `cloudpickle`,
-which is then compressed with `gzip`.
-The compression level can be changed as follows (defaults to 9).
-```python
-class NoCompressionTask(TaskBase, compress_level=0):
-    ...
-```
 
 ### Job scheduling and prefixes
 To run task on job schedulers, one can add prefix to the call of task.
 ```python
 
-class TaskWithJobScheduler(TaskBase, job_prefix=['jbsub', '-tty', '-queue x86_1h', '-cores 16+1', '-mem 64g', '-require a100_80gb']):
+class TaskWithJobScheduler(TaskBase, job_prefix=['jbsub', '-interactive', '-tty', '-queue x86_1h', '-cores 16+1', '-mem 64g']):
     ...
 ```
 
 ### Data directories
 
 Use `task.task_directory` to get a fresh path dedicated to each task.
 The directory is automatically created at
 `{$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/data/{task_id}`
 and the contents of the directory are cleared at each task call and persist until the task is cleared.
 ```python
 class TrainModel(TaskBase):
-    ...
-
     def run_task(self) -> str:
         ...
         model_path = self.task_directory / 'model.bin'
         model.save(model_path)
         return model_path
 ```
 
@@ -253,16 +250,14 @@
 class Main(TaskBase):
     ...
 ```
 The command runs the `Main()` task and stores the cache right next to `taskfile.py` as `.cache/taskproc/...`.
 Please refer to `python -m taskproc.app --help` for more info.
 
 ### Other useful properties
-* `TaskBase.task_id`
-* `TaskBase.task_args`
-* `TaskBase.task_stdout`
-* `TaskBase.task_stderr`
-
-
+* `TaskBase.task_id`: An integer id for each task
+* `TaskBase.task_args`: The argument of the task
+* `TaskBase.task_stdout`: path to the task's stdout
+* `TaskBase.task_stderr`: Path to the task's stderr
 
 ## TODO
 - [ ] Task graph visualizer
```

### Comparing `taskproc-0.11.1/pyproject.toml` & `taskproc-0.11.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskproc"
-version = "0.11.1"
+version = "0.11.2"
 description = "A lightweight task processing library written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/taskproc"
 repository = "https://github.com/koheimiya/taskproc"
 readme = "README.md"
 packages = [{include = "taskproc"}]
```

### Comparing `taskproc-0.11.1/taskproc/__init__.py` & `taskproc-0.11.2/taskproc/__init__.py`

 * *Files identical despite different names*

### Comparing `taskproc-0.11.1/taskproc/app.py` & `taskproc-0.11.2/taskproc/app.py`

 * *Files identical despite different names*

### Comparing `taskproc-0.11.1/taskproc/database.py` & `taskproc-0.11.2/taskproc/database.py`

 * *Files identical despite different names*

### Comparing `taskproc-0.11.1/taskproc/graph.py` & `taskproc-0.11.2/taskproc/graph.py`

 * *Files identical despite different names*

### Comparing `taskproc-0.11.1/taskproc/task.py` & `taskproc-0.11.2/taskproc/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
-from collections.abc import Iterable, Iterator
-from contextlib import contextmanager, redirect_stderr, redirect_stdout
+from collections.abc import Iterable
+from contextlib import redirect_stderr, redirect_stdout
 from typing import Callable, Generic, Mapping, Protocol, Sequence, Type, TypeVar, Any, cast
 from typing_extensions import ParamSpec, Self, get_origin, overload
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from concurrent.futures import Executor
 import ast
@@ -14,15 +14,14 @@
 import json
 import shutil
 import subprocess
 import tempfile
 import cloudpickle
 import gzip
 import sys
-import io
 
 
 from .types import Json, TaskKey, Context
 from .database import Database
 from .graph import TaskGraph, run_task_graph
 
 
@@ -41,23 +40,23 @@
     """ Information specific to a task class (not instance) """
     def __init__(
             self,
             task_class: Type[TaskType[P, R]],
             channels: tuple[str, ...],
             compress_level: int,
             job_prefix: list[str] | None,
-            capture_output: bool,
+            detach_output: bool,
             ) -> None:
 
         self.task_class = task_class
         self.name = _serialize_function(task_class)
         self.db = Database.make(name=self.name, compress_level=compress_level)
         self.channels = (self.name,) + channels
         self.job_prefix = job_prefix
-        self.capture_output = capture_output
+        self.detach_output = detach_output
         self.worker_registry: dict[Json, TaskWorker[R]] = {}
 
         source = inspect.getsource(task_class)
         formatted_source = ast.unparse(ast.parse(source))
         self.source_timestamp = self.db.update_source_if_necessary(formatted_source)
 
     def clear_all(self) -> None:
@@ -128,56 +127,45 @@
                     worker = cloudpickle.load(gzip.open("{worker_path}", "rb"))
                     res = worker._run_task_with_captured_output()
                     cloudpickle.dump(res, gzip.open("{result_path}", "wb"))
                 """.replace('\n', ';')
                 with gzip.open(worker_path, 'wb') as worker_ref:
                     cloudpickle.dump(self, worker_ref)
                 res = subprocess.run(
-                        [*job_prefix, sys.executable, '-c', pycmd],
-                        capture_output=True,
+                        ' '.join([*job_prefix, sys.executable, '-c', repr(pycmd)]),
+                        capture_output=True, check=True, shell=True,
                         )
                 print(res.stdout.decode(), end='')
                 print(res.stderr.decode(), end='', file=sys.stderr)
                 res.check_returncode()
                 with gzip.open(result_path, 'rb') as result_ref:
                     return cloudpickle.load(result_ref)
 
     def _run_task_with_captured_output(self) -> R:
-        if not self.config.capture_output:
+        if not self.config.detach_output:
             return self.instance.run_task()
 
-        stdout = io.TextIOWrapper(io.BytesIO())
-        stderr = io.TextIOWrapper(io.BytesIO())
-        out, err = b'', b''
         try:
-            try:
-                with redirect_stdout(stdout):
-                    with redirect_stderr(stderr):
-                        return self.instance.run_task()
-            finally:
-                stdout.seek(0)
-                out = stdout.read()
-                stderr.seek(0)
-                err = stderr.read()
-                with open(self.stdout_path, 'w') as ref:
-                    ref.write(out)
-                with open(self.stderr_path, 'w') as ref:
-                    ref.write(err)
+            with open(self.stdout_path, 'w+') as stdout:
+                with open(self.stderr_path, 'w+') as stderr:
+                    with redirect_stdout(stdout):
+                        with redirect_stderr(stderr):
+                            return self.instance.run_task()
         except:
             task_info = {
                     'name': self.config.name,
                     'id': self.task_id,
                     'args': self.task_args,
                     }
             LOGGER.error(f'Error occurred while running task {task_info}')
             LOGGER.error(f'Here is the stdout ({self.stdout_path}):')
-            for line in out.splitlines():
+            for line in open(self.stdout_path).readlines():
                 LOGGER.error(line)
             LOGGER.error(f'Here is the stderr ({self.stderr_path}):')
-            for line in err.splitlines():
+            for line in open(self.stderr_path).readlines():
                 LOGGER.error(line)
             raise
 
     @property
     def task_id(self) -> int:
         return self.config.db.id_table.get(self.arg_key)
 
@@ -240,25 +228,25 @@
         elif _channel is None:
             channels = tuple()
         else:
             raise ValueError('Invalid channel value:', _channel)
 
         compress_level = kwargs.pop('compress_level', 9)
         job_prefix = kwargs.pop('job_prefix', None)
-        capture_output = kwargs.pop('capture_output', True)
+        detach_output = kwargs.pop('detach_output', True)
 
         # Fill missing requirement
         ann = inspect.get_annotations(cls, eval_str=True)
         for k, v in ann.items():
             if get_origin(v) is Req and getattr(cls, k, None) is None:
                 req = Req()
                 req.__set_name__(None, k)
                 setattr(cls, k, req)
 
-        cls._task_config = TaskConfig(task_class=cls, channels=channels, compress_level=compress_level, job_prefix=job_prefix, capture_output=capture_output)
+        cls._task_config = TaskConfig(task_class=cls, channels=channels, compress_level=compress_level, job_prefix=job_prefix, detach_output=detach_output)
         super().__init_subclass__(**kwargs)
 
     def __init__(self, *args: P.args, **kwargs: P.kwargs) -> None:
         self._task_worker: TaskWorker[R] = TaskWorker.make(
                 self._task_config, self, *args, **kwargs
                 )
```

### Comparing `taskproc-0.11.1/taskproc/types.py` & `taskproc-0.11.2/taskproc/types.py`

 * *Files identical despite different names*

### Comparing `taskproc-0.11.1/PKG-INFO` & `taskproc-0.11.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskproc
-Version: 0.11.1
+Version: 0.11.2
 Summary: A lightweight task processing library written in pure Python
 Home-page: https://github.com/koheimiya/taskproc
 License: MIT
 Author: Kohei Miyaguchi
 Author-email: koheimiyaguchi@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,20 +16,29 @@
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/koheimiya/taskproc
 Description-Content-Type: text/markdown
 
-# Checkpoint-tool
+# taskproc
 
 A lightweight workflow building/execution/management tool written in pure Python.
-
 Internally, it depends on `DiskCache`, `cloudpickle` `networkx` and `concurrent.futures`.
 
+#### Features
+* Decomposing long and complex computation into tasks, i.e., smaller units of work.
+* Executing them in a distributed way, supporting multithreading, multiprocessing, local clusters/containers.
+* Creating/discarding caches per task and reusing them whenever possible. 
+
+#### Nonfeatures
+* Automatic retry
+* External service integration with remote clusters/containers or cloud platforms (GCP, AWS, ...)
+* Periodic scheduling
+* GUI dashboard
 
 ## Installation
 
 ```
 pip install taskproc
 ```
 
@@ -47,17 +56,16 @@
 # `infer_task_type` decorator helps the type checker to infer the types of the task class. (optional)
 @infer_task_type
 class Choose(TaskBase):
     """ Compute the binomial coefficient. """
     # Inside a task, we first declare the values that must be computed upstream with the descriptor `Req`.
     # In this example, `Choose(n, k)` depends on `Choose(n - 1, k - 1)` and `Choose(n - 1, k)`,
     # so it requires two `int` values.
-    # Either the type annotation `Requires[...]` or the assignment `= Req()` may be omitted.
-    prev1: Requires[int] = Req()
-    prev2: Requires[int] = Req()
+    prev1: Requires[int]
+    prev2: Requires[int]
 
     def build_task(self, n: int, k: int):
         # The prerequisite tasks and the other instance attributes are prepared here.
         # It thus recursively defines all the tasks we need to run this task,
         # i.e., the entire upstream workflow.
 
         if 0 < k < n:
@@ -79,15 +87,15 @@
 
 # To run the task as well as upstream workflow, use the `run_graph()` method.
 ans = Choose(6, 3).run_graph()  # `ans` should be 6 Choose 3, which is 20.
 
 # It greedily executes all the necessary tasks as parallel as possible
 # and then spits out the return value of the task on which we call `run_graph()`.
 # The return values of the intermediate tasks are cached at
-# `{$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/...`
+# `{$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/results/...`
 # and reused on the fly whenever possible.
 ```
 
 ### Deleting cache
 
 It is possible to selectively discard cache: 
 ```python
@@ -101,40 +109,31 @@
 # Delete all the cache associated with `Choose`,
 # equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.Choose`.
 Choose.clear_all_tasks()            
 ```
 
 ### Task IO
 
-The arguments of the `init` method can be anything JSON serializable:
+The arguments of the `build_task` method can be anything JSON serializable including `Task`s:
 ```python
-class T1(TaskBase):
-    def build_task(self, **param1):
-        ...
-    ...
-
-class T2(TaskBase):
-    def build_task(self, **param2):
+class MyTask(TaskBase):
+    def build_task(self, param1, param2):
         ...
-    ...
-
-class T3(TaskBase):
-    x1 = Req()
-    x2 = Req()
-
-    def build_task(self, json_params):
-        self.x1 = T1(**json_params['param1'])
-        self.x2 = T2(**json_params['param2'])
 
-    def run_task(self):
+MyTask(
+    param1={
+        'upstream_task0': UpstreamTask(),
+        'other_params': [1, 2],
         ...
-
-result = T3({'param1': { ... }, 'param2': { ... }}).run_graph()
+    },
+    param2={ ... }
+}).run_graph()
 ```
 
+<!--
 Otherwise they can be passed via `Task` and `Req`:
 ```python
 from taskproc import Task
 Dataset = ...  # Some complex data structure
 Model = ...    # Some complex data structure
 
 class LoadDataset(TaskBase):
@@ -181,56 +180,54 @@
 
     def build_task(self, task_dict: dict[str, Task[float]]):
         self.scores = task_dict
 
     def run_task(self) -> float:
         return sum(self.scores.values()) / len(self.scores)  # We have access to the dict of the results.
 ```
+-->
 
-One can also directly access the items of dictionary-valued upstream tasks.
+The output of the `run_task` method should be serializable with `cloudpickle`,
+which is then compressed with `gzip`.
+The compression level can be changed as follows (defaults to 9).
 ```python
-class MultiOutputTask(TaskBase):
+class NoCompressionTask(TaskBase, compress_level=0):
     ...
+```
 
+If the output is a dictionary, one can directly access its element:
+```python
+class MultiOutputTask(TaskBase):
     def run_task(self) -> dict[str, int]:
         return {'foo': 42, ...}
 
 class DownstreamTask(TaskBase):
     dep: Requires[int]
 
     def build_task(self):
         self.dep = MultiOutputTask()['foo']
 ```
 
-The output of the `run_task` method should be serializable with `cloudpickle`,
-which is then compressed with `gzip`.
-The compression level can be changed as follows (defaults to 9).
-```python
-class NoCompressionTask(TaskBase, compress_level=0):
-    ...
-```
 
 ### Job scheduling and prefixes
 To run task on job schedulers, one can add prefix to the call of task.
 ```python
 
-class TaskWithJobScheduler(TaskBase, job_prefix=['jbsub', '-tty', '-queue x86_1h', '-cores 16+1', '-mem 64g', '-require a100_80gb']):
+class TaskWithJobScheduler(TaskBase, job_prefix=['jbsub', '-interactive', '-tty', '-queue x86_1h', '-cores 16+1', '-mem 64g']):
     ...
 ```
 
 ### Data directories
 
 Use `task.task_directory` to get a fresh path dedicated to each task.
 The directory is automatically created at
 `{$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/data/{task_id}`
 and the contents of the directory are cleared at each task call and persist until the task is cleared.
 ```python
 class TrainModel(TaskBase):
-    ...
-
     def run_task(self) -> str:
         ...
         model_path = self.task_directory / 'model.bin'
         model.save(model_path)
         return model_path
 ```
 
@@ -275,17 +272,15 @@
 class Main(TaskBase):
     ...
 ```
 The command runs the `Main()` task and stores the cache right next to `taskfile.py` as `.cache/taskproc/...`.
 Please refer to `python -m taskproc.app --help` for more info.
 
 ### Other useful properties
-* `TaskBase.task_id`
-* `TaskBase.task_args`
-* `TaskBase.task_stdout`
-* `TaskBase.task_stderr`
-
-
+* `TaskBase.task_id`: An integer id for each task
+* `TaskBase.task_args`: The argument of the task
+* `TaskBase.task_stdout`: path to the task's stdout
+* `TaskBase.task_stderr`: Path to the task's stderr
 
 ## TODO
 - [ ] Task graph visualizer
```

