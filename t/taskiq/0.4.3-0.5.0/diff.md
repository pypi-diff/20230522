# Comparing `tmp/taskiq-0.4.3.tar.gz` & `tmp/taskiq-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq-0.4.3.tar", max compression
+gzip compressed data, was "taskiq-0.5.0.tar", max compression
```

## Comparing `taskiq-0.4.3.tar` & `taskiq-0.5.0.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0     1075 2023-05-09 14:56:10.515367 taskiq-0.4.3/LICENSE
--rw-r--r--   0        0        0     1875 2023-05-09 14:56:10.515367 taskiq-0.4.3/README.md
--rw-r--r--   0        0        0     2884 2023-05-09 14:56:10.519367 taskiq-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1587 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/__init__.py
--rw-r--r--   0        0        0     2077 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/__main__.py
--rw-r--r--   0        0        0      194 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/abc/__init__.py
--rw-r--r--   0        0        0    12063 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/abc/broker.py
--rw-r--r--   0        0        0      323 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/abc/cmd.py
--rw-r--r--   0        0        0      629 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/abc/formatter.py
--rw-r--r--   0        0        0     2997 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/abc/middleware.py
--rw-r--r--   0        0        0     1375 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/abc/result_backend.py
--rw-r--r--   0        0        0     1084 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/abc/schedule_source.py
--rw-r--r--   0        0        0       34 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/brokers/__init__.py
--rw-r--r--   0        0        0     5566 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/brokers/inmemory_broker.py
--rw-r--r--   0        0        0     2197 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/brokers/shared_broker.py
--rw-r--r--   0        0        0     2514 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/brokers/zmq_broker.py
--rw-r--r--   0        0        0       31 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/__init__.py
--rw-r--r--   0        0        0      197 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/common_args.py
--rw-r--r--   0        0        0       37 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/scheduler/__init__.py
--rw-r--r--   0        0        0     1990 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/scheduler/args.py
--rw-r--r--   0        0        0      651 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/scheduler/cmd.py
--rw-r--r--   0        0        0     3911 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/scheduler/run.py
--rw-r--r--   0        0        0     2550 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/utils.py
--rw-r--r--   0        0        0     1516 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/watcher.py
--rw-r--r--   0        0        0       43 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/worker/__init__.py
--rw-r--r--   0        0        0     5438 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/worker/args.py
--rw-r--r--   0        0        0      628 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/worker/cmd.py
--rw-r--r--   0        0        0     1742 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/worker/log_collector.py
--rw-r--r--   0        0        0     7498 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/worker/process_manager.py
--rw-r--r--   0        0        0     6044 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/cli/worker/run.py
--rw-r--r--   0        0        0      468 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/context.py
--rw-r--r--   0        0        0     2929 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/decor.py
--rw-r--r--   0        0        0      510 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/events.py
--rw-r--r--   0        0        0      778 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/exceptions.py
--rw-r--r--   0        0        0       25 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/formatters/__init__.py
--rw-r--r--   0        0        0      844 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/formatters/json_formatter.py
--rw-r--r--   0        0        0     1887 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/funcs.py
--rw-r--r--   0        0        0     5552 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/kicker.py
--rw-r--r--   0        0        0      507 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/message.py
--rw-r--r--   0        0        0       26 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/middlewares/__init__.py
--rw-r--r--   0        0        0     4315 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/middlewares/prometheus_middleware.py
--rw-r--r--   0        0        0     2039 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/middlewares/retry_middleware.py
--rw-r--r--   0        0        0        0 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/py.typed
--rw-r--r--   0        0        0      113 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/receiver/__init__.py
--rw-r--r--   0        0        0     2795 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/receiver/params_parser.py
--rw-r--r--   0        0        0     9651 2023-05-09 14:56:10.519367 taskiq-0.4.3/taskiq/receiver/receiver.py
--rw-r--r--   0        0        0      483 2023-05-09 14:56:10.523367 taskiq-0.4.3/taskiq/result.py
--rw-r--r--   0        0        0       35 2023-05-09 14:56:10.523367 taskiq-0.4.3/taskiq/result_backends/__init__.py
--rw-r--r--   0        0        0     1268 2023-05-09 14:56:10.523367 taskiq-0.4.3/taskiq/result_backends/dummy.py
--rw-r--r--   0        0        0      146 2023-05-09 14:56:10.523367 taskiq-0.4.3/taskiq/schedule_sources/__init__.py
--rw-r--r--   0        0        0     1519 2023-05-09 14:56:10.523367 taskiq-0.4.3/taskiq/schedule_sources/label_based.py
--rw-r--r--   0        0        0      264 2023-05-09 14:56:10.523367 taskiq-0.4.3/taskiq/scheduler/__init__.py
--rw-r--r--   0        0        0     1056 2023-05-09 14:56:10.523367 taskiq-0.4.3/taskiq/scheduler/merge_functions.py
--rw-r--r--   0        0        0     1717 2023-05-09 14:56:10.523367 taskiq-0.4.3/taskiq/scheduler/scheduler.py
--rw-r--r--   0        0        0     1071 2023-05-09 14:56:10.523367 taskiq-0.4.3/taskiq/state.py
--rw-r--r--   0        0        0     4139 2023-05-09 14:56:10.523367 taskiq-0.4.3/taskiq/task.py
--rw-r--r--   0        0        0      874 2023-05-09 14:56:10.523367 taskiq-0.4.3/taskiq/utils.py
--rw-r--r--   0        0        0      106 2023-05-09 14:56:10.523367 taskiq-0.4.3/taskiq/warnings.py
--rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 taskiq-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-21 22:13:26.880195 taskiq-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1875 2023-05-21 22:13:26.880195 taskiq-0.5.0/README.md
+-rw-r--r--   0        0        0     2880 2023-05-21 22:13:26.884195 taskiq-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1587 2023-05-21 22:13:26.884195 taskiq-0.5.0/taskiq/__init__.py
+-rw-r--r--   0        0        0     2077 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/__main__.py
+-rw-r--r--   0        0        0      194 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/__init__.py
+-rw-r--r--   0        0        0    12064 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/broker.py
+-rw-r--r--   0        0        0      323 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/cmd.py
+-rw-r--r--   0        0        0      629 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/formatter.py
+-rw-r--r--   0        0        0     3002 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/middleware.py
+-rw-r--r--   0        0        0     1376 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/result_backend.py
+-rw-r--r--   0        0        0     1084 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/schedule_source.py
+-rw-r--r--   0        0        0       34 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/brokers/__init__.py
+-rw-r--r--   0        0        0     5679 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/brokers/inmemory_broker.py
+-rw-r--r--   0        0        0     2197 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/brokers/shared_broker.py
+-rw-r--r--   0        0        0     2514 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/brokers/zmq_broker.py
+-rw-r--r--   0        0        0       31 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/common_args.py
+-rw-r--r--   0        0        0       37 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/scheduler/__init__.py
+-rw-r--r--   0        0        0     1990 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/scheduler/args.py
+-rw-r--r--   0        0        0      651 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/scheduler/cmd.py
+-rw-r--r--   0        0        0     3912 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/scheduler/run.py
+-rw-r--r--   0        0        0     2550 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/utils.py
+-rw-r--r--   0        0        0     1517 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/watcher.py
+-rw-r--r--   0        0        0       43 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/worker/__init__.py
+-rw-r--r--   0        0        0     6060 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/worker/args.py
+-rw-r--r--   0        0        0      628 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/worker/cmd.py
+-rw-r--r--   0        0        0     1742 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/worker/log_collector.py
+-rw-r--r--   0        0        0     7497 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/worker/process_manager.py
+-rw-r--r--   0        0        0     6163 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/worker/run.py
+-rw-r--r--   0        0        0      468 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/context.py
+-rw-r--r--   0        0        0     2930 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/decor.py
+-rw-r--r--   0        0        0      511 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/events.py
+-rw-r--r--   0        0        0      941 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/exceptions.py
+-rw-r--r--   0        0        0       25 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/formatters/__init__.py
+-rw-r--r--   0        0        0      844 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1887 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/funcs.py
+-rw-r--r--   0        0        0     5552 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/kicker.py
+-rw-r--r--   0        0        0      507 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/message.py
+-rw-r--r--   0        0        0       26 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/middlewares/__init__.py
+-rw-r--r--   0        0        0     4315 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/middlewares/prometheus_middleware.py
+-rw-r--r--   0        0        0     2043 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/middlewares/retry_middleware.py
+-rw-r--r--   0        0        0        0 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/py.typed
+-rw-r--r--   0        0        0      113 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/receiver/__init__.py
+-rw-r--r--   0        0        0     2795 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/receiver/params_parser.py
+-rw-r--r--   0        0        0    11406 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/receiver/receiver.py
+-rw-r--r--   0        0        0     2020 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/result.py
+-rw-r--r--   0        0        0       35 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/result_backends/__init__.py
+-rw-r--r--   0        0        0     1268 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/result_backends/dummy.py
+-rw-r--r--   0        0        0      146 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/schedule_sources/__init__.py
+-rw-r--r--   0        0        0     1520 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/schedule_sources/label_based.py
+-rw-r--r--   0        0        0      264 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/scheduler/__init__.py
+-rw-r--r--   0        0        0     1056 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/scheduler/merge_functions.py
+-rw-r--r--   0        0        0     1717 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/scheduler/scheduler.py
+-rw-r--r--   0        0        0    11302 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/serialization.py
+-rw-r--r--   0        0        0     1071 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/state.py
+-rw-r--r--   0        0        0     4141 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/task.py
+-rw-r--r--   0        0        0      874 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/utils.py
+-rw-r--r--   0        0        0      106 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/warnings.py
+-rw-r--r--   0        0        0     3654 1970-01-01 00:00:00.000000 taskiq-0.5.0/PKG-INFO
```

### Comparing `taskiq-0.4.3/LICENSE` & `taskiq-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/README.md` & `taskiq-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/pyproject.toml` & `taskiq-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq"
-version = "0.4.3"
+version = "0.5.0"
 description = "Distributed task queue with full async support"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 maintainers = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 repository = "https://github.com/taskiq-python/taskiq"
 homepage = "https://taskiq-python.github.io/"
 documentation = "https://taskiq-python.github.io/"
@@ -28,14 +28,15 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 typing-extensions = ">=3.10.0.0"
 pydantic = "^1.6.2"
 importlib-metadata = "*"
 pycron = "^3.0.0"
 taskiq_dependencies = "^1"
+anyio = "^3"
 # For prometheus metrics
 prometheus_client = { version = "^0", optional = true }
 # For ZMQBroker
 pyzmq = { version = "^23.2.0", optional = true }
 # For speed
 uvloop = { version = ">=0.16.0,<1", optional = true }
 # For hot-reload.
@@ -51,15 +52,14 @@
 pre-commit = "^2.20.0"
 yesqa = "^1.3.0"
 autoflake = "^1.4"
 wemake-python-styleguide = "^0.16.1"
 coverage = "^6.4.2"
 pytest-cov = "^3.0.0"
 mock = "^4.0.3"
-anyio = "^3.6.1"
 pytest-xdist = { version = "^2.5.0", extras = ["psutil"] }
 types-mock = "^4.0.15"
 
 [tool.poetry.extras]
 zmq = ["pyzmq"]
 uv = ["uvloop"]
 metrics = ["prometheus_client"]
```

### Comparing `taskiq-0.4.3/taskiq/__init__.py` & `taskiq-0.5.0/taskiq/__init__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/__main__.py` & `taskiq-0.5.0/taskiq/__main__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/abc/broker.py` & `taskiq-0.5.0/taskiq/abc/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     def add_dependency_context(self, new_ctx: Dict[Any, Any]) -> None:
         """
         Add first-level dependencies.
 
         Provided dict will be used to inject new dependencies
         in all dependency graph contexts.
 
-        :param new_ctx: Additional context values for dependnecy injection.
+        :param new_ctx: Additional context values for dependency injection.
         """
         self.custom_dependency_context.update(new_ctx)
 
     def add_middlewares(self, *middlewares: "TaskiqMiddleware") -> None:
         """
         Add a list of middlewares.
 
@@ -148,15 +148,15 @@
         await self.result_backend.startup()
 
     async def shutdown(self) -> None:
         """
         Close the broker.
 
         This method is called,
-        when broker is closig.
+        when broker is closing.
         """
         event = TaskiqEvents.CLIENT_SHUTDOWN
         if self.is_worker_process:
             event = TaskiqEvents.WORKER_SHUTDOWN
 
         # Call all shutdown events.
         for handler in self.event_handlers[event]:
```

### Comparing `taskiq-0.4.3/taskiq/abc/formatter.py` & `taskiq-0.5.0/taskiq/abc/formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/abc/middleware.py` & `taskiq-0.5.0/taskiq/abc/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     def pre_execute(
         self,
         message: "TaskiqMessage",
     ) -> "Union[TaskiqMessage, Coroutine[Any, Any, TaskiqMessage]]":
         """
         This hook is called before executing task.
 
-        This is a worker-side hook, wich means it
+        This is a worker-side hook, which means it
         executes in the worker process.
 
         :param message: incoming parsed taskiq message.
         :return: modified message.
         """
         return message
 
@@ -93,15 +93,15 @@
         :param result: returned value.
         """
 
     def on_error(
         self,
         message: "TaskiqMessage",
         result: "TaskiqResult[Any]",
-        exception: Exception,
+        exception: BaseException,
     ) -> "Union[None, Coroutine[Any, Any, None]]":
         """
         This function is called when exception is found.
 
         :param message: incoming message.
         :param result: returned value.
         :param exception: found exception.
```

### Comparing `taskiq-0.4.3/taskiq/abc/result_backend.py` & `taskiq-0.5.0/taskiq/abc/result_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         """Do something on shutdown."""
 
     @abstractmethod
     async def set_result(self, task_id: str, result: TaskiqResult[_ReturnType]) -> None:
         """
         Saves result to the result backend.
 
-        Result must be save so it can be accesed later
+        Result must be save so it can be accessed later
         by the calling side of the system.
 
         :param task_id: id of a task to save.
         :param result: result of execution.
         :return: nothing.
         """
```

### Comparing `taskiq-0.4.3/taskiq/abc/schedule_source.py` & `taskiq-0.5.0/taskiq/abc/schedule_source.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/brokers/inmemory_broker.py` & `taskiq-0.5.0/taskiq/brokers/inmemory_broker.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,41 +84,43 @@
 class InMemoryBroker(AsyncBroker):
     """
     This broker is used to execute tasks without sending them elsewhere.
 
     It's useful for local development, if you don't want to setup real broker.
     """
 
-    def __init__(
+    def __init__(  # noqa: WPS211
         self,
         sync_tasks_pool_size: int = 4,
         max_stored_results: int = 100,
         cast_types: bool = True,
         max_async_tasks: int = 30,
+        propagate_exceptions: bool = True,
     ) -> None:
         super().__init__()
         self.result_backend = InmemoryResultBackend(
             max_stored_results=max_stored_results,
         )
         self.executor = ThreadPoolExecutor(sync_tasks_pool_size)
         self.receiver = Receiver(
             broker=self,
             executor=self.executor,
             validate_params=cast_types,
             max_async_tasks=max_async_tasks,
+            propagate_exceptions=propagate_exceptions,
         )
         self._running_tasks: "Set[asyncio.Task[Any]]" = set()
 
     async def kick(self, message: BrokerMessage) -> None:
         """
         Kicking task.
 
         This method just executes given task.
 
-        :param message: incomming message.
+        :param message: incoming message.
 
         :raises TaskiqError: if someone wants to kick unknown task.
         """
         target_task = self.available_tasks.get(message.task_name)
         if target_task is None:
             raise TaskiqError("Unknown task.")
```

### Comparing `taskiq-0.4.3/taskiq/brokers/shared_broker.py` & `taskiq-0.5.0/taskiq/brokers/shared_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/brokers/zmq_broker.py` & `taskiq-0.5.0/taskiq/brokers/zmq_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/cli/scheduler/args.py` & `taskiq-0.5.0/taskiq/cli/scheduler/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         parser.add_argument(
             "--fs-discover",
             "-fsd",
             action="store_true",
             help=(
                 "If this option is on, "
                 "taskiq will try to find tasks modules "
-                "in current directory recursievly. Name of file to search for "
+                "in current directory recursively. Name of file to search for "
                 "can be configured using `--tasks-pattern` option."
             ),
         )
         parser.add_argument(
             "--tasks-pattern",
             "-tp",
             default="tasks.py",
```

### Comparing `taskiq-0.4.3/taskiq/cli/scheduler/cmd.py` & `taskiq-0.5.0/taskiq/cli/scheduler/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/cli/scheduler/run.py` & `taskiq-0.5.0/taskiq/cli/scheduler/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 async def schedules_updater(
     scheduler: TaskiqScheduler,
     current_schedules: List[ScheduledTask],
 ) -> None:
     """
     Periodic update to schedules.
 
-    This task preiodicaly checks for new schedules,
+    This task periodically checks for new schedules,
     assembles the final list and replaces current
     schedule with a new one.
 
     :param scheduler: current scheduler.
     :param current_schedules: list of schedules.
     """
     while True:
```

### Comparing `taskiq-0.4.3/taskiq/cli/utils.py` & `taskiq-0.5.0/taskiq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/cli/watcher.py` & `taskiq-0.5.0/taskiq/cli/watcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from gitignore_parser import parse_gitignore
 from watchdog.events import FileSystemEvent
 
 logger = getLogger("taskiq.worker")
 
 
 class FileWatcher:  # pragma: no cover
-    """Filewatcher that watchs for filesystem changes."""
+    """Filewatcher that watches for filesystem changes."""
 
     def __init__(
         self,
         callback: Callable[..., None],
         use_gitignore: bool = True,
         **callback_kwargs: Any,
     ) -> None:
```

### Comparing `taskiq-0.4.3/taskiq/cli/worker/args.py` & `taskiq-0.5.0/taskiq/cli/worker/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     no_parse: bool = False
     shutdown_timeout: float = 5
     reload: bool = False
     no_gitignore: bool = False
     max_async_tasks: int = 100
     receiver: str = "taskiq.receiver:Receiver"
     receiver_arg: List[Tuple[str, str]] = field(default_factory=list)
+    max_prefetch: int = 0
+    no_propagate_errors: bool = False
 
     @classmethod
     def from_cli(  # noqa: WPS213
         cls,
         args: Optional[Sequence[str]] = None,
     ) -> "WorkerArgs":
         """
@@ -95,15 +97,15 @@
         parser.add_argument(
             "--fs-discover",
             "-fsd",
             action="store_true",
             help=(
                 "If this option is on, "
                 "taskiq will try to find tasks modules "
-                "in current directory recursievly. Name of file to search for "
+                "in current directory recursively. Name of file to search for "
                 "can be configured using `--tasks-pattern` option."
             ),
         )
         parser.add_argument(
             "--log-level",
             default="INFO",
             choices=[level.name for level in LogLevel],
@@ -122,26 +124,36 @@
             type=str,
             default=(
                 "[%(asctime)s]"
                 "[%(levelname)-7s]"
                 "[%(module)s:%(funcName)s:%(lineno)d] "
                 "%(message)s"
             ),
-            help="Format wich is used when collecting logs from function execution",
+            help="Format which is used when collecting logs from function execution",
         )
         parser.add_argument(
             "--no-parse",
             action="store_true",
             help=(
                 "If this parameter is on,"
                 " taskiq doesn't parse incoming parameters "
                 " with pydantic."
             ),
         )
         parser.add_argument(
+            "--no-propagate-errors",
+            action="store_true",
+            dest="no_propagate_errors",
+            help=(
+                "If this parameter is on,"
+                " all errors that happen in tasks "
+                " won't be propagated to generator dependencies."
+            ),
+        )
+        parser.add_argument(
             "--max-threadpool-threads",
             type=int,
             help="Maximum number of threads for executing sync functions.",
         )
         parser.add_argument(
             "--shutdown-timeout",
             type=float,
@@ -164,10 +176,17 @@
         parser.add_argument(
             "--max-async-tasks",
             type=int,
             dest="max_async_tasks",
             default=100,
             help="Maximum simultaneous async tasks per worker process. ",
         )
+        parser.add_argument(
+            "--max-prefetch",
+            type=int,
+            dest="max_prefetch",
+            default=0,
+            help="Maximum prefetched tasks per worker process. ",
+        )
 
         namespace = parser.parse_args(args)
         return WorkerArgs(**namespace.__dict__)
```

### Comparing `taskiq-0.4.3/taskiq/cli/worker/cmd.py` & `taskiq-0.5.0/taskiq/cli/worker/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/cli/worker/log_collector.py` & `taskiq-0.5.0/taskiq/cli/worker/log_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """A class to write to multiple streams."""
 
     def __init__(self, *streams: IO[Any]) -> None:
         self.streams = streams
 
     def write(self, message: Any) -> None:
         """
-        This write request writes to all avaialble streams.
+        This write request writes to all available streams.
 
         :param message: message to write.
         """
         for stream in self.streams:
             stream.write(message)
```

### Comparing `taskiq-0.4.3/taskiq/cli/worker/process_manager.py` & `taskiq-0.5.0/taskiq/cli/worker/process_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     logger.info("Scheduled workers reload.")
 
 
 def get_signal_handler(
     action_queue: "Queue[ProcessActionBase]",
 ) -> Callable[[int, Any], None]:
     """
-    Generate singnal handler for main process.
+    Generate signal handler for main process.
 
     The signal handler will just put the SHUTDOWN event in
     the action queue.
 
     :param action_queue: event queue.
     :returns: actual signal handler.
     """
```

### Comparing `taskiq-0.4.3/taskiq/cli/worker/run.py` & `taskiq-0.5.0/taskiq/cli/worker/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 logger = logging.getLogger("taskiq.worker")
 
 
 async def shutdown_broker(broker: AsyncBroker, timeout: float) -> None:
     """
     This function used to shutdown broker.
 
-    Broker can throw erorrs during shutdown,
+    Broker can throw errors during shutdown,
     or it may return some value.
 
     We need to handle such situations.
 
     :param broker: current broker.
-    :param timeout: maximum amout of time to shutdown the broker.
+    :param timeout: maximum amount of time to shutdown the broker.
     """
     logger.warning("Shutting down the broker.")
     try:
         ret_val = await asyncio.wait_for(broker.shutdown(), timeout)  # type: ignore
         if ret_val is not None:
             logger.info("Broker returned value on shutdown: '%s'", str(ret_val))
     except asyncio.TimeoutError:
@@ -66,15 +66,15 @@
 
 
 def start_listen(args: WorkerArgs) -> None:  # noqa: WPS210, WPS213
     """
     This function starts actual listening process.
 
     It imports broker and all tasks.
-    Since tasks registers themselfs in a global set,
+    Since tasks registers themselves in a global set,
     it's easy to just import module where you have decorated
     function and they will be available in broker's `available_tasks`
     field.
 
     :param args: CLI arguments.
     :raises ValueError: if broker is not an AsyncBroker instance.
     :raises ValueError: if receiver is not a Receiver type.
@@ -106,15 +106,15 @@
         Signal handler.
 
         This handler checks if process is already
         terminating and if it's true, it does nothing.
 
         :param signum: received signal number.
         :param _frame: current execution frame.
-        :raises KeyboardInterrupt: if termiation hasn't begun.
+        :raises KeyboardInterrupt: if termination hasn't begun.
         """
         logger.debug(f"Got signal {signum}.")
         nonlocal shutting_down  # noqa: WPS420
         if shutting_down:
             return
         shutting_down = True  # noqa: WPS442
         raise KeyboardInterrupt
@@ -128,14 +128,16 @@
         logger.debug("Initialize receiver.")
         with ThreadPoolExecutor(args.max_threadpool_threads) as pool:
             receiver = receiver_type(
                 broker=broker,
                 executor=pool,
                 validate_params=not args.no_parse,
                 max_async_tasks=args.max_async_tasks,
+                max_prefetch=args.max_prefetch,
+                propagate_exceptions=not args.no_propagate_errors,
                 **receiver_args,
             )
             loop.run_until_complete(receiver.listen())
     except KeyboardInterrupt:
         logger.warning("Worker process interrupted.")
         loop.run_until_complete(shutdown_broker(broker, args.shutdown_timeout))
 
@@ -164,15 +166,15 @@
         raise ValueError("To use '--reload' flag, please install 'taskiq[reload]'.")
 
     if Observer is not None and args.reload:
         observer = Observer()
         observer.start()
         args.workers = 1
         logging.warning(
-            "Reload on chage enabled. Number of worker processes set to 1.",
+            "Reload on change enabled. Number of worker processes set to 1.",
         )
 
     manager = ProcessManager(args=args, observer=observer, worker_function=start_listen)
 
     manager.start()
 
     if observer is not None and observer.is_alive():
```

### Comparing `taskiq-0.4.3/taskiq/decor.py` & `taskiq-0.5.0/taskiq/decor.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         labels: Dict[str, Any],
     ) -> None:
         self.broker = broker
         self.task_name = task_name
         self.original_func = original_func
         self.labels = labels
 
-    # Docs for this method are ommited in order to help
+    # Docs for this method are omitted in order to help
     # your IDE resolve correct docs for it.
     def __call__(  # noqa: D102
         self,
         *args: _FuncParams.args,
         **kwargs: _FuncParams.kwargs,
     ) -> _ReturnType:
         return self.original_func(*args, **kwargs)
@@ -93,16 +93,16 @@
         """
         return await self.kicker().kiq(*args, **kwargs)
 
     def kicker(self) -> AsyncKicker[_FuncParams, _ReturnType]:
         """
         This function returns kicker object.
 
-        Kicker is a object that can modyfy kiq request
-        before sendig it.
+        Kicker is a object that can modify kiq request
+        before sending it.
 
         :return: AsyncKicker instance.
         """
         return AsyncKicker(
             task_name=self.task_name,
             broker=self.broker,
             labels=self.labels,
```

### Comparing `taskiq-0.4.3/taskiq/exceptions.py` & `taskiq-0.5.0/taskiq/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,7 +24,15 @@
 
 class ResultSetError(ResultBackendError):
     """Error if ResultBackend was unable to set result."""
 
 
 class ResultIsReadyError(ResultBackendError):
     """Error if ResultBackend was unable to find out if the task is ready."""
+
+
+class SecurityError(TaskiqError):
+    """Security related exception."""
+
+
+class NoResultError(TaskiqError):
+    """Error if user does not want to set result."""
```

### Comparing `taskiq-0.4.3/taskiq/formatters/json_formatter.py` & `taskiq-0.5.0/taskiq/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/funcs.py` & `taskiq-0.5.0/taskiq/funcs.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/kicker.py` & `taskiq-0.5.0/taskiq/kicker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/middlewares/prometheus_middleware.py` & `taskiq-0.5.0/taskiq/middlewares/prometheus_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/middlewares/retry_middleware.py` & `taskiq-0.5.0/taskiq/middlewares/retry_middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ) -> None:
         self.default_retry_count = default_retry_count
 
     async def on_error(
         self,
         message: "TaskiqMessage",
         result: "TaskiqResult[Any]",
-        exception: Exception,
+        exception: BaseException,
     ) -> None:
         """
         Retry on error.
 
         This middleware is used to retry
         tasks on errors.
```

### Comparing `taskiq-0.4.3/taskiq/receiver/params_parser.py` & `taskiq-0.5.0/taskiq/receiver/params_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     For example
 
     you have task like this:
 
     >>> def my_task(a: int) -> str
     >>>     ...
 
-    If you will kall my_task.kiq("11")
+    If you will call my_task.kiq("11")
 
     You'll receive parsed 11 (int).
     But, if you call it with mytask.kiq("str"),
     you get the same value.
 
     If you want to skip parsing completely,
     you can pass --no-parse to worker,
```

### Comparing `taskiq-0.4.3/taskiq/receiver/receiver.py` & `taskiq-0.5.0/taskiq/receiver/receiver.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import asyncio
 import inspect
 from concurrent.futures import Executor
 from logging import getLogger
 from time import time
-from typing import Any, Callable, Dict, Optional, get_type_hints
+from typing import Any, Callable, Dict, Optional, Set, get_type_hints
 
+import anyio
 from taskiq_dependencies import DependencyGraph
 
 from taskiq.abc.broker import AsyncBroker
 from taskiq.abc.middleware import TaskiqMiddleware
 from taskiq.context import Context
+from taskiq.exceptions import NoResultError
 from taskiq.message import TaskiqMessage
 from taskiq.receiver.params_parser import parse_params
 from taskiq.result import TaskiqResult
 from taskiq.state import TaskiqState
 from taskiq.utils import maybe_awaitable
 
 logger = getLogger(__name__)
+QUEUE_DONE = b"-1"
 
 
 def _run_sync(target: Callable[..., Any], message: TaskiqMessage) -> Any:
     """
     Runs function synchronously.
 
     We use this function, because
@@ -32,53 +35,57 @@
     """
     return target(*message.args, **message.kwargs)
 
 
 class Receiver:
     """Class that uses as a callback handler."""
 
-    def __init__(
+    def __init__(  # noqa: WPS211
         self,
         broker: AsyncBroker,
         executor: Optional[Executor] = None,
         validate_params: bool = True,
         max_async_tasks: "Optional[int]" = None,
+        max_prefetch: int = 0,
+        propagate_exceptions: bool = True,
     ) -> None:
         self.broker = broker
         self.executor = executor
         self.validate_params = validate_params
         self.task_signatures: Dict[str, inspect.Signature] = {}
         self.task_hints: Dict[str, Dict[str, Any]] = {}
         self.dependency_graphs: Dict[str, DependencyGraph] = {}
+        self.propagate_exceptions = propagate_exceptions
         for task in self.broker.available_tasks.values():
             self.task_signatures[task.task_name] = inspect.signature(task.original_func)
             self.task_hints[task.task_name] = get_type_hints(task.original_func)
             self.dependency_graphs[task.task_name] = DependencyGraph(task.original_func)
         self.sem: "Optional[asyncio.Semaphore]" = None
         if max_async_tasks is not None and max_async_tasks > 0:
             self.sem = asyncio.Semaphore(max_async_tasks)
         else:
             logger.warning(
                 "Setting unlimited number of async tasks "
                 + "can result in undefined behavior",
             )
+        self.sem_prefetch = asyncio.Semaphore(max_prefetch)
 
     async def callback(  # noqa: C901, WPS213
         self,
         message: bytes,
         raise_err: bool = False,
     ) -> None:
         """
         Receive new message and execute tasks.
 
         This method is used to process message,
         that came from brokers.
 
         :raises Exception: if raise_err is true,
-            and excpetion were found while saving result.
+            and exception were found while saving result.
         :param message: received message.
         :param raise_err: raise an error if cannot save result in
             result_backend.
         """
         try:
             taskiq_msg = self.broker.formatter.loads(message=message)
         except Exception as exc:
@@ -117,18 +124,19 @@
             target=self.broker.available_tasks[taskiq_msg.task_name].original_func,
             message=taskiq_msg,
         )
         for middleware in self.broker.middlewares:
             if middleware.__class__.post_execute != TaskiqMiddleware.post_execute:
                 await maybe_awaitable(middleware.post_execute(taskiq_msg, result))
         try:
-            await self.broker.result_backend.set_result(taskiq_msg.task_id, result)
-            for middleware in self.broker.middlewares:
-                if middleware.__class__.post_save != TaskiqMiddleware.post_save:
-                    await maybe_awaitable(middleware.post_save(taskiq_msg, result))
+            if not isinstance(result.error, NoResultError):
+                await self.broker.result_backend.set_result(taskiq_msg.task_id, result)
+                for middleware in self.broker.middlewares:
+                    if middleware.__class__.post_save != TaskiqMiddleware.post_save:
+                        await maybe_awaitable(middleware.post_save(taskiq_msg, result))
         except Exception as exc:
             logger.exception(
                 "Can't set result in result backend. Cause: %s",
                 exc,
                 exc_info=True,
             )
             if raise_err:
@@ -193,32 +201,40 @@
                 # run it in executor.
                 returned = await loop.run_in_executor(
                     self.executor,
                     _run_sync,
                     target,
                     message,
                 )
-        except Exception as exc:
+        except BaseException as exc:  # noqa: WPS424
             found_exception = exc
             logger.error(
                 "Exception found while executing function: %s",
                 exc,
                 exc_info=True,
             )
         # Stop the timer.
         execution_time = time() - start_time
         if dep_ctx:
-            await dep_ctx.close()
+            args = (None, None, None)
+            if found_exception and self.propagate_exceptions:
+                args = (  # type: ignore
+                    type(found_exception),
+                    found_exception,
+                    found_exception.__traceback__,
+                )
+            await dep_ctx.close(*args)
 
         # Assemble result.
         result: "TaskiqResult[Any]" = TaskiqResult(
             is_err=found_exception is not None,
             log=None,
             return_value=returned,
             execution_time=round(execution_time, 2),
+            error=found_exception,
         )
         # If exception is found we execute middlewares.
         if found_exception is not None:
             for middleware in self.broker.middlewares:
                 if middleware.__class__.on_error != TaskiqMiddleware.on_error:
                     await maybe_awaitable(
                         middleware.on_error(
@@ -235,15 +251,46 @@
         This function iterates over tasks asynchronously.
 
         It uses listen() method of an AsyncBroker
         to get new messages from queues.
         """
         await self.broker.startup()
         logger.info("Listening started.")
-        tasks = set()
+        queue: asyncio.Queue[bytes] = asyncio.Queue()
+
+        async with anyio.create_task_group() as gr:
+            gr.start_soon(self.prefetcher, queue)
+            gr.start_soon(self.runner, queue)
+
+    async def prefetcher(self, queue: "asyncio.Queue[Any]") -> None:
+        """
+        Prefetch tasks data.
+
+        :param queue: queue for prefetched data.
+        """
+        iterator = self.broker.listen()
+
+        while True:
+            try:
+                await self.sem_prefetch.acquire()
+                message = await iterator.__anext__()  # noqa: WPS609
+                await queue.put(message)
+
+            except StopAsyncIteration:
+                break
+
+        await queue.put(QUEUE_DONE)
+
+    async def runner(self, queue: "asyncio.Queue[bytes]") -> None:
+        """
+        Run tasks.
+
+        :param queue: queue with prefetched data.
+        """
+        tasks: Set[asyncio.Task[Any]] = set()
 
         def task_cb(task: "asyncio.Task[Any]") -> None:
             """
             Callback for tasks.
 
             This function used to remove task
             from the list of active tasks and release
@@ -251,19 +298,27 @@
 
             :param task: finished task
             """
             tasks.discard(task)
             if self.sem is not None:
                 self.sem.release()
 
-        async for message in self.broker.listen():
+        while True:
             # Waits for semaphore to be released.
             if self.sem is not None:
                 await self.sem.acquire()
-            task = asyncio.create_task(self.callback(message=message, raise_err=False))
+
+            self.sem_prefetch.release()
+            message = await queue.get()
+            if message is QUEUE_DONE:
+                break
+
+            task = asyncio.create_task(
+                self.callback(message=message, raise_err=False),
+            )
             tasks.add(task)
 
             # We want the task to remove itself from the set when it's done.
             #
             # Because python's GC can silently cancel task
             # and it considered to be Hisenbug.
             # https://textual.textualize.io/blog/2023/02/11/the-heisenbug-lurking-in-your-async-code/
```

### Comparing `taskiq-0.4.3/taskiq/result_backends/dummy.py` & `taskiq-0.5.0/taskiq/result_backends/dummy.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/schedule_sources/label_based.py` & `taskiq-0.5.0/taskiq/schedule_sources/label_based.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         """
         Collect schedules for all tasks.
 
         this function checks labels for all
         tasks available to the broker.
 
         If task has a schedule label,
-        it will be parsed and retuned.
+        it will be parsed and returned.
 
         :return: list of schedules.
         """
         schedules = []
         for task_name, task in self.broker.available_tasks.items():
             if task.broker != self.broker:
                 continue
```

### Comparing `taskiq-0.4.3/taskiq/scheduler/merge_functions.py` & `taskiq-0.5.0/taskiq/scheduler/merge_functions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/scheduler/scheduler.py` & `taskiq-0.5.0/taskiq/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/state.py` & `taskiq-0.5.0/taskiq/state.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/taskiq/task.py` & `taskiq-0.5.0/taskiq/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,18 +51,18 @@
     ) -> Union[
         "TaskiqResult[_ReturnType]",
         Coroutine[Any, Any, "TaskiqResult[_ReturnType]"],
     ]:
         """
         Wait for result to become ready and get it.
 
-        This function constantly checks wheter result is ready
+        This function constantly checks whether result is ready
         and fetches it when it becomes available.
 
-        :param check_interval: how ofen availability is checked.
+        :param check_interval: how often availability is checked.
         :param timeout: maximum amount of time it will wait
             before raising TaskiqResultTimeoutError.
         :param with_logs: whether you need to download logs.
         :return: TaskiqResult.
         """
 
 
@@ -77,15 +77,15 @@
         self.task_id = task_id
         self.result_backend = result_backend
 
     async def is_ready(self) -> bool:
         """
         Checks if task is completed.
 
-        :raises ResultIsReadyError: if we can't get info about task readyness.
+        :raises ResultIsReadyError: if we can't get info about task readiness.
 
         :return: True if task is completed.
         """
         try:
             return await self.result_backend.is_result_ready(self.task_id)
         except Exception as exc:
             raise ResultIsReadyError() from exc
```

### Comparing `taskiq-0.4.3/taskiq/utils.py` & `taskiq-0.5.0/taskiq/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.3/PKG-INFO` & `taskiq-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq
-Version: 0.4.3
+Version: 0.5.0
 Summary: Distributed task queue with full async support
 Home-page: https://taskiq-python.github.io/
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Maintainer: Pavel Kirilin
@@ -17,26 +17,22 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Provides-Extra: metrics
 Provides-Extra: reload
 Provides-Extra: uv
 Provides-Extra: zmq
+Requires-Dist: anyio (>=3,<4)
 Requires-Dist: gitignore-parser (>=0,<1) ; extra == "reload"
 Requires-Dist: importlib-metadata
 Requires-Dist: prometheus_client (>=0,<1) ; extra == "metrics"
 Requires-Dist: pycron (>=3.0.0,<4.0.0)
 Requires-Dist: pydantic (>=1.6.2,<2.0.0)
 Requires-Dist: pyzmq (>=23.2.0,<24.0.0) ; extra == "zmq"
 Requires-Dist: taskiq_dependencies (>=1,<2)
```

#### html2text {}

```diff
@@ -1,38 +1,35 @@
-Metadata-Version: 2.1 Name: taskiq Version: 0.4.3 Summary: Distributed task
+Metadata-Version: 2.1 Name: taskiq Version: 0.5.0 Summary: Distributed task
 queue with full async support Home-page: https://taskiq-python.github.io/
 License: LICENSE Keywords: taskiq,tasks,distributed,async Author: Pavel Kirilin
 Author-email: win10@list.ru Maintainer: Pavel Kirilin Maintainer-email:
 win10@list.ru Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: System :: Networking Classifier:
-Typing :: Typed Provides-Extra: metrics Provides-Extra: reload Provides-Extra:
-uv Provides-Extra: zmq Requires-Dist: gitignore-parser (>=0,<1) ; extra ==
-"reload" Requires-Dist: importlib-metadata Requires-Dist: prometheus_client
-(>=0,<1) ; extra == "metrics" Requires-Dist: pycron (>=3.0.0,<4.0.0) Requires-
-Dist: pydantic (>=1.6.2,<2.0.0) Requires-Dist: pyzmq (>=23.2.0,<24.0.0) ; extra
-== "zmq" Requires-Dist: taskiq_dependencies (>=1,<2) Requires-Dist: typing-
-extensions (>=3.10.0.0) Requires-Dist: uvloop (>=0.16.0,<1) ; extra == "uv"
-Requires-Dist: watchdog (>=2.1.9,<3.0.0) ; extra == "reload" Project-URL:
-Documentation, https://taskiq-python.github.io/ Project-URL: Repository, https:
-//github.com/taskiq-python/taskiq Description-Content-Type: text/markdown [!
-[PyPI - Python Version](https://img.shields.io/pypi/pyversions/
-taskiq?style=for-the-badge)](https://pypi.org/project/taskiq/) [![PyPI](https:/
-/img.shields.io/pypi/v/taskiq?style=for-the-badge)](https://pypi.org/project/
-taskiq/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/taskiq?style=for-
-the-badge)](https://pypistats.org/packages/taskiq)
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Topic :: System :: Networking Classifier: Typing :: Typed
+Provides-Extra: metrics Provides-Extra: reload Provides-Extra: uv Provides-
+Extra: zmq Requires-Dist: anyio (>=3,<4) Requires-Dist: gitignore-parser
+(>=0,<1) ; extra == "reload" Requires-Dist: importlib-metadata Requires-Dist:
+prometheus_client (>=0,<1) ; extra == "metrics" Requires-Dist: pycron
+(>=3.0.0,<4.0.0) Requires-Dist: pydantic (>=1.6.2,<2.0.0) Requires-Dist: pyzmq
+(>=23.2.0,<24.0.0) ; extra == "zmq" Requires-Dist: taskiq_dependencies (>=1,<2)
+Requires-Dist: typing-extensions (>=3.10.0.0) Requires-Dist: uvloop
+(>=0.16.0,<1) ; extra == "uv" Requires-Dist: watchdog (>=2.1.9,<3.0.0) ; extra
+== "reload" Project-URL: Documentation, https://taskiq-python.github.io/
+Project-URL: Repository, https://github.com/taskiq-python/taskiq Description-
+Content-Type: text/markdown [![PyPI - Python Version](https://img.shields.io/
+pypi/pyversions/taskiq?style=for-the-badge)](https://pypi.org/project/taskiq/)
+[![PyPI](https://img.shields.io/pypi/v/taskiq?style=for-the-badge)](https://
+pypi.org/project/taskiq/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/
+taskiq?style=for-the-badge)](https://pypistats.org/packages/taskiq)
 [https://raw.githubusercontent.com/taskiq-python/taskiq/master/imgs/logo.svg]
 ===============================================================================
 Taskiq is an asynchronous distributed task queue for python. This project takes
 inspiration from big projects such as [Celery](https://docs.celeryq.dev) and
 [Dramatiq](https://dramatiq.io/). But taskiq can send and run both the sync and
 async functions. Also, we use [PEP-612](https://peps.python.org/pep-0612/) to
 provide the best autosuggestions possible. But since it's a new PEP, I
```

