# Comparing `tmp/duckingit-0.0.7.tar.gz` & `tmp/duckingit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckingit-0.0.7.tar", last modified: Thu May 18 09:43:48 2023, max compression
+gzip compressed data, was "duckingit-0.0.8.tar", last modified: Mon May 22 17:27:57 2023, max compression
```

## Comparing `duckingit-0.0.7.tar` & `duckingit-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:43:48.808335 duckingit-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 09:43:34.000000 duckingit-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-18 09:43:48.808335 duckingit-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-18 09:43:34.000000 duckingit-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:43:48.808335 duckingit-0.0.7/duckingit/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-18 09:43:34.000000 duckingit-0.0.7/duckingit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-05-18 09:43:34.000000 duckingit-0.0.7/duckingit/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-18 09:43:34.000000 duckingit-0.0.7/duckingit/_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-18 09:43:34.000000 duckingit-0.0.7/duckingit/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-18 09:43:34.000000 duckingit-0.0.7/duckingit/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-18 09:43:34.000000 duckingit-0.0.7/duckingit/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-05-18 09:43:34.000000 duckingit-0.0.7/duckingit/_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-18 09:43:34.000000 duckingit-0.0.7/duckingit/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-18 09:43:34.000000 duckingit-0.0.7/duckingit/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:43:48.808335 duckingit-0.0.7/duckingit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-18 09:43:48.000000 duckingit-0.0.7/duckingit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-18 09:43:48.000000 duckingit-0.0.7/duckingit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:43:48.000000 duckingit-0.0.7/duckingit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 09:43:48.000000 duckingit-0.0.7/duckingit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 09:43:48.000000 duckingit-0.0.7/duckingit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-18 09:43:34.000000 duckingit-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 09:43:48.808335 duckingit-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.059910 duckingit-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 17:27:37.000000 duckingit-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-22 17:27:57.059910 duckingit-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-22 17:27:37.000000 duckingit-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.059910 duckingit-0.0.8/duckingit/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.059910 duckingit-0.0.8/duckingit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-22 17:27:57.000000 duckingit-0.0.8/duckingit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-22 17:27:57.000000 duckingit-0.0.8/duckingit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:27:57.000000 duckingit-0.0.8/duckingit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-22 17:27:57.000000 duckingit-0.0.8/duckingit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 17:27:57.000000 duckingit-0.0.8/duckingit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-22 17:27:37.000000 duckingit-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:27:57.059910 duckingit-0.0.8/setup.cfg
```

### Comparing `duckingit-0.0.7/LICENSE` & `duckingit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.7/PKG-INFO` & `duckingit-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckingit
-Version: 0.0.7
+Version: 0.0.8
 Summary: A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB
 Author-email: Tobias Egelund <egelundtobias@gmail.com>
 Project-URL: Homepage, https://github.com/tobiasegelund/duckingit
 Project-URL: Bug Tracker, https://github.com/tobiasegelund/duckingit/issues
 Keywords: Serverless,DuckDB,Data Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckingit-0.0.7/README.md` & `duckingit-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.7/duckingit/_config.py` & `duckingit-0.0.8/duckingit/_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,19 +54,19 @@
             raise AttributeError()
 
         super(LambdaConfig, self).__setattr__(name, value)
 
     def update(self):
         config_dict = copy.deepcopy(self.__dict__)
         warm_up = config_dict.pop("WarmUp")
+        provider = Providers.get_or_raise("aws").lambda_
 
-        Providers.AWS.klass.update_lambda_configurations(config_dict)
-
+        provider.update_lambda_configurations(config_dict)
         if warm_up:
-            Providers.AWS.klass.warm_up_lambda_function()
+            provider.lambda_.warm_up_lambda_function()
 
 
 @dataclass
 class SQSConfig(ServiceConfig):
     QueueSuccess: str = "DuckSuccess"
     QueueFailure: str = "DuckFailure"
 
@@ -133,15 +133,17 @@
     def update(self) -> None:
         config_dict = {
             k: str(v)
             for k, v in self.__dict__.items()
             if k in ("DelaySeconds", "MaximumMessageSize", "MessageRetentionPeriod")
         }
         for name in [self.__dict__["QueueSuccess"], self.__dict__["QueueFailure"]]:
-            Providers.AWS.klass.update_sqs_configurations(name=name, configs=config_dict)
+            Providers.get_or_raise("aws").sqs.update_sqs_configurations(
+                name=name, configs=config_dict
+            )
 
 
 @dataclass
 class AWSConfig(ServiceConfig):
     aws_region: str = ""
     aws_access_key_id: str = ""
     aws_secret_access_key: str = ""
```

### Comparing `duckingit-0.0.7/duckingit/_controller.py` & `duckingit-0.0.8/duckingit/_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 import typing as t
 
 from duckingit._exceptions import FailedLambdaFunctions
-from duckingit._planner import Plan, Stage, Stages, Task
+from duckingit._planner import Plan, Stage, Task
 from duckingit._utils import scan_source_for_files
 from duckingit.providers import Providers
 
 if t.TYPE_CHECKING:
     from duckingit._session import DuckSession
 
 
@@ -34,15 +34,15 @@
         self.cache_expiration_time = getattr(session.conf, "session.cache_expiration_time")
 
         self.success_queue = getattr(self.session.conf, "aws_sqs.QueueSuccess")
         self.failure_queue = getattr(self.session.conf, "aws_sqs.QueueFailure")
         self.verbose = getattr(self.session.conf, "session.verbose")
 
     def _set_provider(self):
-        self.provider = Providers.AWS.klass
+        self.provider = Providers.get_or_raise("aws")
 
     def fetch_cache_metadata(self) -> dict[str, datetime.datetime]:
         return self.session.metadata_cached
 
     def update_cache_metadata(
         self, execution_stage: Stage, execution_time: datetime.datetime
     ) -> None:
@@ -111,15 +111,17 @@
             default_prefix = prefix
 
         context[stage.id] = [f"{default_prefix}/{i}.parquet" for i in stage.output]
         # self.evaluate_execution_stage(execution_stage=stage, prefix=default_prefix)
 
         execution_time = datetime.datetime.now()
         if len(stage.tasks) > 0:
-            request_ids = self.provider.invoke(execution_tasks=stage.tasks, prefix=default_prefix)
+            request_ids = self.provider.lambda_.invoke(
+                execution_tasks=stage.tasks, prefix=default_prefix
+            )
 
             self.check_status_of_invokations(request_ids=request_ids)
 
         completed.add(stage)
         self.update_cache_metadata(execution_stage=stage, execution_time=execution_time)
 
     def execute_plan(self, execution_plan: Plan, prefix: str, default_prefix: str):
@@ -144,39 +146,41 @@
         cnt = 0
 
         total_tasks = len(request_ids)
         while len(request_ids) > 0:
             # Logic to speed up fast queries
             if cnt < len(WAIT_TIME_SUCCESS_QUEUE_SECONDS):
                 wait_time = WAIT_TIME_SUCCESS_QUEUE_SECONDS[cnt]
-            messages = self.provider.poll_messages_from_queue(
+            messages = self.provider.sqs.poll_messages_from_queue(
                 name=self.success_queue, wait_time_seconds=wait_time
             )
 
             if len(messages) > 0:
                 for message in messages:
                     try:
                         request_ids.pop(message.request_id)
                     except KeyError:
                         continue
 
                 entries = list(message.create_entry_payload() for message in messages)
-                self.provider.delete_messages_from_queue(name=self.success_queue, entries=entries)
+                self.provider.sqs.delete_messages_from_queue(
+                    name=self.success_queue, entries=entries
+                )
 
             if self.verbose:
                 print(f"\tTASKS COMPLETED: {total_tasks - len(request_ids)}/{total_tasks}")
 
             cnt += 1
 
             if cnt % ITERATIONS_TO_CHECK_FAILED == 0:
-                messages = self.provider.poll_messages_from_queue(
+                messages = self.provider.sqs.poll_messages_from_queue(
                     name=self.failure_queue,
                     wait_time_seconds=WAIT_TIME_FAILURE_QUEUE_SECONDS,
                 )
 
                 if len(messages) > 0:
-                    self.provider.purge_queue(self.failure_queue)  # clean up
+                    self.provider.sqs.purge_queue(self.failure_queue)  # clean up
                     raise FailedLambdaFunctions(f"{messages}")
 
     # def show(self):
     #     # Select only X parquet files?
     #     pass
```

### Comparing `duckingit-0.0.7/duckingit/_dataset.py` & `duckingit-0.0.8/duckingit/_dataset.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.7/duckingit/_parser.py` & `duckingit-0.0.8/duckingit/_parser.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.7/duckingit/_planner.py` & `duckingit-0.0.8/duckingit/_planner.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.7/duckingit/_session.py` & `duckingit-0.0.8/duckingit/_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     def conf(self) -> DuckConfig:
         return DuckConfig()
 
     def _load_httpfs(self) -> None:
         self._conn.execute("INSTALL httpfs; LOAD httpfs;")
 
     def _set_credentials(self) -> None:
-        self._conn.execute(Providers.AWS.credentials)
+        self._conn.execute(Providers.get_or_raise("aws").duckdb_settings())
 
     def sql(self, query: str) -> Dataset:
         """Creates a Dataset to execute against DuckDB instances
 
         The Dataset can also be configured to save to a specific path or temporary table
         using the write method of the Dataset class.
```

### Comparing `duckingit-0.0.7/duckingit/_utils.py` & `duckingit-0.0.8/duckingit/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 def create_conn_with_httpfs_loaded() -> duckdb.DuckDBPyConnection:
     """Returns a in memory DuckDB connection with httpfs loaded"""
     from duckingit.providers import Providers
 
     conn = duckdb.connect(":memory:")
     conn.execute("LOAD httpfs;")
-    conn.execute(Providers.AWS.credentials)
+    conn.execute(Providers.get_or_raise("aws").duckdb_settings())
 
     return conn
 
 
 def scan_source_for_files(source: str) -> list[str]:
     """Scans the source for files using DuckDB
```

### Comparing `duckingit-0.0.7/duckingit.egg-info/PKG-INFO` & `duckingit-0.0.8/duckingit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckingit
-Version: 0.0.7
+Version: 0.0.8
 Summary: A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB
 Author-email: Tobias Egelund <egelundtobias@gmail.com>
 Project-URL: Homepage, https://github.com/tobiasegelund/duckingit
 Project-URL: Bug Tracker, https://github.com/tobiasegelund/duckingit/issues
 Keywords: Serverless,DuckDB,Data Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckingit-0.0.7/pyproject.toml` & `duckingit-0.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "duckingit"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   {name="Tobias Egelund", email="egelundtobias@gmail.com" },
 ]
 description = "A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["Serverless", "DuckDB", "Data Engineering"]
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "boto3",
     "duckdb",
-    'sqlglot',
+    'sqlglot<=12.0',
     'pyarrow',
 ]
 
 [tool.setuptools]
 packages = ["duckingit"]
 
 [project.urls]
```

