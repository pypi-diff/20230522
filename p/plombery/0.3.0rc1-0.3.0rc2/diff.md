# Comparing `tmp/plombery-0.3.0rc1.tar.gz` & `tmp/plombery-0.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plombery-0.3.0rc1.tar", last modified: Mon May 22 15:52:05 2023, max compression
+gzip compressed data, was "plombery-0.3.0rc2.tar", last modified: Mon May 22 17:43:35 2023, max compression
```

## Comparing `plombery-0.3.0rc1.tar` & `plombery-0.3.0rc2.tar`

### file list

```diff
@@ -1,54 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:52:05.542598 plombery-0.3.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-22 15:52:05.542598 plombery-0.3.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 15:52:05.542598 plombery-0.3.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:52:05.534598 plombery-0.3.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:52:05.538598 plombery-0.3.0rc1/src/plombery/
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:52:05.538598 plombery-0.3.0rc1/src/plombery/api/
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/api/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:52:05.538598 plombery-0.3.0rc1/src/plombery/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/database/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/database/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/database/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/database/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:52:05.538598 plombery-0.3.0rc1/src/plombery/logger/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/logger/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/logger/web_socket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:52:05.538598 plombery-0.3.0rc1/src/plombery/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:52:05.538598 plombery-0.3.0rc1/src/plombery/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/orchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/orchestrator/data_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/orchestrator/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:52:05.542598 plombery-0.3.0rc1/src/plombery/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/pipeline/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/pipeline/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/pipeline/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/pipeline/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:52:05.542598 plombery-0.3.0rc1/src/plombery/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:52:05.542598 plombery-0.3.0rc1/src/plombery/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/src/plombery/websocket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:52:05.538598 plombery-0.3.0rc1/src/plombery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-22 15:52:05.000000 plombery-0.3.0rc1/src/plombery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-22 15:52:05.000000 plombery-0.3.0rc1/src/plombery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:52:05.000000 plombery-0.3.0rc1/src/plombery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-22 15:52:05.000000 plombery-0.3.0rc1/src/plombery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 15:52:05.000000 plombery-0.3.0rc1/src/plombery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:52:05.542598 plombery-0.3.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-22 15:51:09.000000 plombery-0.3.0rc1/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.221079 plombery-0.3.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-22 17:43:35.221079 plombery-0.3.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 17:43:35.221079 plombery-0.3.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.213079 plombery-0.3.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.213079 plombery-0.3.0rc2/src/plombery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.213079 plombery-0.3.0rc2/src/plombery/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/api/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.217079 plombery-0.3.0rc2/src/plombery/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/database/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/database/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/database/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/database/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.217079 plombery-0.3.0rc2/src/plombery/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/logger/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/logger/web_socket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.217079 plombery-0.3.0rc2/src/plombery/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.217079 plombery-0.3.0rc2/src/plombery/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/orchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/orchestrator/data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/orchestrator/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.217079 plombery-0.3.0rc2/src/plombery/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/pipeline/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/pipeline/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/pipeline/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/pipeline/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.217079 plombery-0.3.0rc2/src/plombery/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.221079 plombery-0.3.0rc2/src/plombery/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  1395472 2023-05-22 17:43:22.000000 plombery-0.3.0rc2/src/plombery/static/assets/HandsonTable-a6b0964d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    37420 2023-05-22 17:43:22.000000 plombery-0.3.0rc2/src/plombery/static/assets/HandsonTable-a8e02e84.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-05-22 17:43:22.000000 plombery-0.3.0rc2/src/plombery/static/assets/index-6aea2e83.js
+-rw-r--r--   0 runner    (1001) docker     (123)   272858 2023-05-22 17:43:22.000000 plombery-0.3.0rc2/src/plombery/static/assets/index-c8f76152.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1103782 2023-05-22 17:43:22.000000 plombery-0.3.0rc2/src/plombery/static/assets/vendor-ccd85f8c.js
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-22 17:43:22.000000 plombery-0.3.0rc2/src/plombery/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-22 17:43:19.000000 plombery-0.3.0rc2/src/plombery/static/mario-pipe-flower.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.221079 plombery-0.3.0rc2/src/plombery/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/src/plombery/websocket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.213079 plombery-0.3.0rc2/src/plombery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-22 17:43:35.000000 plombery-0.3.0rc2/src/plombery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-22 17:43:35.000000 plombery-0.3.0rc2/src/plombery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:43:35.000000 plombery-0.3.0rc2/src/plombery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-22 17:43:35.000000 plombery-0.3.0rc2/src/plombery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 17:43:35.000000 plombery-0.3.0rc2/src/plombery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:43:35.221079 plombery-0.3.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-22 17:42:26.000000 plombery-0.3.0rc2/tests/test_logging.py
```

### Comparing `plombery-0.3.0rc1/LICENSE` & `plombery-0.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/PKG-INFO` & `plombery-0.3.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plombery
-Version: 0.3.0rc1
+Version: 0.3.0rc2
 Summary: Python task scheduler with a user-friendly web UI
 Author-email: Luca Faggianelli <luca@velvetlab.tech>
 License: MIT
 Keywords: pipeline,task-scheduler,apscheduler,orchestrator,web-ui,fastapi,pydantic
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plombery Version: 0.3.0rc1 Summary: Python task
+Metadata-Version: 2.1 Name: plombery Version: 0.3.0rc2 Summary: Python task
 scheduler with a user-friendly web UI Author-email: Luca Faggianelli
 velvetlab.tech> License: MIT Keywords: pipeline,task-
 scheduler,apscheduler,orchestrator,web-ui,fastapi,pydantic Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown Provides-Extra: dev Provides-Extra: docs License-File:
 LICENSE     [![Contributors][contributors-shield]][contributors-url] [![Forks]
 [forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues]
```

### Comparing `plombery-0.3.0rc1/README.md` & `plombery-0.3.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/pyproject.toml` & `plombery-0.3.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/__init__.py` & `plombery-0.3.0rc2/src/plombery/__init__.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/api/__init__.py` & `plombery-0.3.0rc2/src/plombery/api/__init__.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/api/authentication.py` & `plombery-0.3.0rc2/src/plombery/api/authentication.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/api/middlewares.py` & `plombery-0.3.0rc2/src/plombery/api/middlewares.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/config.py` & `plombery-0.3.0rc2/src/plombery/config.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/database/base.py` & `plombery-0.3.0rc2/src/plombery/database/base.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/database/models.py` & `plombery-0.3.0rc2/src/plombery/database/models.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/database/repository.py` & `plombery-0.3.0rc2/src/plombery/database/repository.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/logger/__init__.py` & `plombery-0.3.0rc2/src/plombery/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/logger/formatter.py` & `plombery-0.3.0rc2/src/plombery/logger/formatter.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/notifications/__init__.py` & `plombery-0.3.0rc2/src/plombery/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/orchestrator/__init__.py` & `plombery-0.3.0rc2/src/plombery/orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/orchestrator/data_storage.py` & `plombery-0.3.0rc2/src/plombery/orchestrator/data_storage.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/orchestrator/executor.py` & `plombery-0.3.0rc2/src/plombery/orchestrator/executor.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/pipeline/__init__.py` & `plombery-0.3.0rc2/src/plombery/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/pipeline/pipeline.py` & `plombery-0.3.0rc2/src/plombery/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/schemas.py` & `plombery-0.3.0rc2/src/plombery/schemas.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery/websocket/__init__.py` & `plombery-0.3.0rc2/src/plombery/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/src/plombery.egg-info/PKG-INFO` & `plombery-0.3.0rc2/src/plombery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plombery
-Version: 0.3.0rc1
+Version: 0.3.0rc2
 Summary: Python task scheduler with a user-friendly web UI
 Author-email: Luca Faggianelli <luca@velvetlab.tech>
 License: MIT
 Keywords: pipeline,task-scheduler,apscheduler,orchestrator,web-ui,fastapi,pydantic
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plombery Version: 0.3.0rc1 Summary: Python task
+Metadata-Version: 2.1 Name: plombery Version: 0.3.0rc2 Summary: Python task
 scheduler with a user-friendly web UI Author-email: Luca Faggianelli
 velvetlab.tech> License: MIT Keywords: pipeline,task-
 scheduler,apscheduler,orchestrator,web-ui,fastapi,pydantic Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown Provides-Extra: dev Provides-Extra: docs License-File:
 LICENSE     [![Contributors][contributors-shield]][contributors-url] [![Forks]
 [forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues]
```

### Comparing `plombery-0.3.0rc1/src/plombery.egg-info/SOURCES.txt` & `plombery-0.3.0rc2/src/plombery.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -30,11 +30,17 @@
 src/plombery/orchestrator/executor.py
 src/plombery/pipeline/__init__.py
 src/plombery/pipeline/_utils.py
 src/plombery/pipeline/context.py
 src/plombery/pipeline/pipeline.py
 src/plombery/pipeline/task.py
 src/plombery/pipeline/trigger.py
-src/plombery/static/.gitkeep
+src/plombery/static/index.html
+src/plombery/static/mario-pipe-flower.png
+src/plombery/static/assets/HandsonTable-a6b0964d.js
+src/plombery/static/assets/HandsonTable-a8e02e84.css
+src/plombery/static/assets/index-6aea2e83.js
+src/plombery/static/assets/index-c8f76152.css
+src/plombery/static/assets/vendor-ccd85f8c.js
 src/plombery/websocket/__init__.py
 tests/test_api.py
 tests/test_logging.py
```

### Comparing `plombery-0.3.0rc1/tests/test_api.py` & `plombery-0.3.0rc2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `plombery-0.3.0rc1/tests/test_logging.py` & `plombery-0.3.0rc2/tests/test_logging.py`

 * *Files identical despite different names*

