# Comparing `tmp/smartlogger-0.0.1.dev6.tar.gz` & `tmp/smartlogger-0.0.1.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartlogger-0.0.1.dev6.tar", last modified: Thu May 18 13:23:29 2023, max compression
+gzip compressed data, was "smartlogger-0.0.1.dev7.tar", last modified: Mon May 22 10:19:59 2023, max compression
```

## Comparing `smartlogger-0.0.1.dev6.tar` & `smartlogger-0.0.1.dev7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:29.283345 smartlogger-0.0.1.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-18 13:23:29.283345 smartlogger-0.0.1.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-18 13:23:19.000000 smartlogger-0.0.1.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 13:23:29.283345 smartlogger-0.0.1.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-18 13:23:19.000000 smartlogger-0.0.1.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:29.283345 smartlogger-0.0.1.dev6/smartlogger/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-18 13:23:19.000000 smartlogger-0.0.1.dev6/smartlogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-18 13:23:19.000000 smartlogger-0.0.1.dev6/smartlogger/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-18 13:23:19.000000 smartlogger-0.0.1.dev6/smartlogger/smartlogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:29.283345 smartlogger-0.0.1.dev6/smartlogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-18 13:23:29.000000 smartlogger-0.0.1.dev6/smartlogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-18 13:23:29.000000 smartlogger-0.0.1.dev6/smartlogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:23:29.000000 smartlogger-0.0.1.dev6/smartlogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-18 13:23:29.000000 smartlogger-0.0.1.dev6/smartlogger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 13:23:29.000000 smartlogger-0.0.1.dev6/smartlogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 13:23:29.000000 smartlogger-0.0.1.dev6/smartlogger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:19:59.699528 smartlogger-0.0.1.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-22 10:19:59.699528 smartlogger-0.0.1.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-22 10:19:46.000000 smartlogger-0.0.1.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 10:19:59.699528 smartlogger-0.0.1.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-22 10:19:46.000000 smartlogger-0.0.1.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:19:59.695528 smartlogger-0.0.1.dev7/smartlogger/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-22 10:19:46.000000 smartlogger-0.0.1.dev7/smartlogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-22 10:19:46.000000 smartlogger-0.0.1.dev7/smartlogger/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-22 10:19:46.000000 smartlogger-0.0.1.dev7/smartlogger/smartlogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:19:59.699528 smartlogger-0.0.1.dev7/smartlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-22 10:19:59.000000 smartlogger-0.0.1.dev7/smartlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-22 10:19:59.000000 smartlogger-0.0.1.dev7/smartlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:19:59.000000 smartlogger-0.0.1.dev7/smartlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 10:19:59.000000 smartlogger-0.0.1.dev7/smartlogger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-22 10:19:59.000000 smartlogger-0.0.1.dev7/smartlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 10:19:59.000000 smartlogger-0.0.1.dev7/smartlogger.egg-info/top_level.txt
```

### Comparing `smartlogger-0.0.1.dev6/setup.py` & `smartlogger-0.0.1.dev7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,21 +14,18 @@
 # Package meta-data.
 NAME = "smartlogger"
 DESCRIPTION = "python logging client for SmartDash"
 URL = "https://github.com/notAI-tech/smartdash"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev6"
+VERSION = "0.0.1.dev7"
 
 # What packages are required for this module to be executed?
-REQUIRED = [
-    "requests",
-    "liteindex"
-]
+REQUIRED = ["requests", "liteindex"]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `smartlogger-0.0.1.dev6/smartlogger/smartlogger.py` & `smartlogger-0.0.1.dev7/smartlogger/smartlogger.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,34 +3,31 @@
 import time
 import uuid
 import logging
 from liteindex import DefinedIndex
 
 
 def upload_to_smartdash():
-    try:
-        import argparse
+    import argparse
 
-        parser = argparse.ArgumentParser(description="Smartlogger sync service")
-        parser.add_argument(
-            "--name",
-            type=str,
-            help="name, given at log or timer initialization time.",
-            required=True,
-        )
-        parser.add_argument(
-            "--save_dir", type=str, help="Directory to save logs", required=True
-        )
-        parser.add_argument(
-            "--smartdash_url", type=str, help="Smartdash server URL", required=True
-        )
-        args = parser.parse_args()
-        _upload_to_smartdash(args.name, args.save_dir, args.smartdash_url)
-    except:
-        pass
+    parser = argparse.ArgumentParser(description="Smartlogger sync service")
+    parser.add_argument(
+        "--name",
+        type=str,
+        help="name, given at log or timer initialization time.",
+        required=True,
+    )
+    parser.add_argument(
+        "--save_dir", type=str, help="Directory to save logs", required=True
+    )
+    parser.add_argument(
+        "--smartdash_url", type=str, help="Smartdash server URL", required=True
+    )
+    args = parser.parse_args()
+    _upload_to_smartdash(args.name, args.save_dir, args.smartdash_url)
 
 
 def _upload_to_smartdash(name, log_dir, url, batch_size=100):
     import requests
 
     def upload_data(name, index_type, db_prefix):
         try:
@@ -75,133 +72,152 @@
 
 class SmartTimer:
     def __init__(self, name, save_to_dir="./"):
         self.name = name
         os.makedirs(save_to_dir, exist_ok=True)
         self.timers_index = DefinedIndex(
             f"{self.name}_timers",
-            schema={"u_id": "", "stage": "", "timestamp": 0, "failed": False},
+            schema={
+                "u_id": "",
+                "stage": "",
+                "timestamp": 0,
+                "failed": False,
+                "start": False,
+            },
             db_path=os.path.join(save_to_dir, f"{self.name}_timers.db"),
             auto_key=True,
         )
 
-    def start(self, id):
+    def start(self, id, stage="begin"):
         self.timers_index.add(
             {
                 "u_id": str(id),
-                "stage": "start",
+                "stage": stage,
                 "timestamp": time.time(),
                 "failed": False,
+                "start": True,
             }
         )
 
-    def stage_success(self, id, name):
+    def finished(self, id, stage="end"):
         self.timers_index.add(
-            {"u_id": str(id), "stage": name, "timestamp": time.time(), "failed": False}
-        )
-
-    def stage_failed(self, id, name):
-        self.timers_index.add(
-            {"u_id": str(id), "stage": name, "timestamp": time.time(), "failed": True}
+            {
+                "u_id": str(id),
+                "stage": stage,
+                "timestamp": time.time(),
+                "failed": False,
+                "start": False,
+            }
         )
 
-    def finished(self, id):
+    def failed(self, id, stage="end"):
         self.timers_index.add(
             {
                 "u_id": str(id),
-                "stage": "finished",
+                "stage": stage,
                 "timestamp": time.time(),
-                "failed": False,
+                "failed": True,
+                "start": False,
             }
         )
 
 
 class SmartLogger:
     def __init__(self, name, save_to_dir="./"):
         self.name = name
         self.logs_index = DefinedIndex(
             f"{self.name}_logs",
-            schema={"u_id": "", "level": "", "messages": [], "timestamp": 0},
+            schema={
+                "u_id": "",
+                "level": "",
+                "messages": [],
+                "timestamp": 0,
+                "stage": "",
+            },
             db_path=os.path.join(save_to_dir, f"{self.name}_logs.db"),
             auto_key=True,
         )
         self.ml_inputs_outputs_index = DefinedIndex(
             f"{self.name}_ml_inputs_outputs",
             schema={
                 "u_id": "",
                 "inputs": [],
                 "outputs": [],
                 "model_type": "",
                 "timestamp": 0,
+                "stage": "",
             },
             db_path=os.path.join(save_to_dir, f"{self.name}_logs.db"),
             auto_key=True,
         )
 
-    def _log(self, id, level, *messages):
+    def _log(self, id, level, *messages, stage=None):
         timestamp = time.time()
         self.logs_index.add(
             {
                 "u_id": str(id),
                 "level": level,
                 "messages": [str(_) for _ in messages],
                 "timestamp": timestamp,
+                "stage": stage,
             }
         )
 
-    def debug(self, id, *messages):
-        self._log(id, "DEBUG", *messages)
+    def debug(self, id, *messages, stage=None):
+        self._log(id, "DEBUG", *messages, stage=stage)
 
-    def info(self, id, *messages):
-        self._log(id, "INFO", *messages)
+    def info(self, id, *messages, stage=None):
+        self._log(id, "INFO", *messages, stage=stage)
 
-    def warning(self, id, *messages):
-        self._log(id, "WARNING", *messages)
+    def warning(self, id, *messages, stage=None):
+        self._log(id, "WARNING", *messages, stage=stage)
 
-    def exception(self, id, *messages):
-        self._log(id, "EXCEPTION", *messages)
+    def exception(self, id, *messages, stage=None):
+        self._log(id, "EXCEPTION", *messages, stage=stage)
 
-    def ml_inputs_outputs(self, id, inputs, outputs, model_type):
+    def ml_inputs_outputs(self, id, inputs, outputs, model_type, stage=None):
         if not isinstance(inputs, (list, tuple)):
             raise ValueError("inputs must be a list or tuple")
         if not isinstance(outputs, (list, tuple)):
             raise ValueError("outputs must be a list or tuple")
         if len(inputs) != len(outputs):
             raise ValueError("inputs and outputs must be the same length")
 
         self.ml_inputs_outputs_index.add(
             {
                 "u_id": str(id),
                 "inputs": inputs,
                 "outputs": outputs,
                 "model_type": model_type,
                 "timestamp": time.time(),
+                "stage": stage,
             }
         )
 
 
 if __name__ == "__main__":
     import sys
     import uuid
     import time
     import random
 
     if sys.argv[1] == "dummy":
 
         def create_some_log(pipeline_timer):
             u_id = str(uuid.uuid4())
-            pipeline_timer.start(id=u_id)
+
+            pipeline_timer.start(id=u_id, stage="begin")
             time.sleep(random.randint(100, 600) / 1000)
-            pipeline_timer.stage_success(id=u_id, name="pre_processing")
+            pipeline_timer.start(id=u_id, stage="feature_extraction")
             time.sleep(random.randint(100, 600) / 1000)
 
             if random.choice([0, 1, 2, 3, 4]) == 3:
-                pipeline_timer.stage_failed(id=u_id, name="feature_extraction")
+                pipeline_timer.failed(id=u_id, name="feature_extraction")
             else:
-                pipeline_timer.stage_success(id=u_id, name="feature_extraction")
+                pipeline_timer.finished(id=u_id, name="feature_extraction")
 
             time.sleep(random.randint(100, 600) / 1000)
             pipeline_timer.finished(id=u_id)
 
             pipeline_logger.debug(u_id, "message_1", "message_2", "message_3")
             pipeline_logger.info(u_id, "message_5", "message_6")
             pipeline_logger.warning(u_id, "message_7", "message_8")
```

