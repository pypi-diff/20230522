# Comparing `tmp/json_log_viewer-0.1.1.tar.gz` & `tmp/json_log_viewer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_log_viewer-0.1.1.tar", max compression
+gzip compressed data, was "json_log_viewer-0.1.2.tar", max compression
```

## Comparing `json_log_viewer-0.1.1.tar` & `json_log_viewer-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      575 2023-05-22 19:56:11.806875 json_log_viewer-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-21 16:09:41.838934 json_log_viewer-0.1.1/json_log_viewer/__init__.py
--rw-r--r--   0        0        0      776 2023-05-22 19:56:11.817367 json_log_viewer-0.1.1/json_log_viewer/__main__.py
--rw-r--r--   0        0        0        0 2023-05-21 10:24:56.000000 json_log_viewer-0.1.1/json_log_viewer/extractor/__init__.py
--rw-r--r--   0        0        0     1368 2023-05-21 17:16:59.595845 json_log_viewer-0.1.1/json_log_viewer/extractor/extract.py
--rw-r--r--   0        0        0     1085 2023-05-22 09:54:50.981130 json_log_viewer-0.1.1/json_log_viewer/extractor/test_extract.py
--rw-r--r--   0        0        0        0 2023-05-21 10:25:02.000000 json_log_viewer-0.1.1/json_log_viewer/logs/__init__.py
--rw-r--r--   0        0        0     1086 2023-05-21 17:06:18.621369 json_log_viewer-0.1.1/json_log_viewer/logs/log.py
--rw-r--r--   0        0        0      627 2023-05-22 09:54:50.987903 json_log_viewer-0.1.1/json_log_viewer/logs/test_log.py
--rw-r--r--   0        0        0     1005 2023-05-22 09:54:50.996869 json_log_viewer-0.1.1/json_log_viewer/logs/tree.py
--rw-r--r--   0        0        0      317 2023-05-22 09:54:51.002158 json_log_viewer-0.1.1/json_log_viewer/test_version.py
--rw-r--r--   0        0        0      544 2023-05-22 19:56:11.779132 json_log_viewer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 json_log_viewer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      575 2023-05-22 19:56:11.806875 json_log_viewer-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 16:09:41.838934 json_log_viewer-0.1.2/json_log_viewer/__init__.py
+-rw-r--r--   0        0        0      776 2023-05-22 20:00:16.638176 json_log_viewer-0.1.2/json_log_viewer/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:24:56.000000 json_log_viewer-0.1.2/json_log_viewer/extractor/__init__.py
+-rw-r--r--   0        0        0     1368 2023-05-21 17:16:59.595845 json_log_viewer-0.1.2/json_log_viewer/extractor/extract.py
+-rw-r--r--   0        0        0     1085 2023-05-22 09:54:50.981130 json_log_viewer-0.1.2/json_log_viewer/extractor/test_extract.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:25:02.000000 json_log_viewer-0.1.2/json_log_viewer/logs/__init__.py
+-rw-r--r--   0        0        0     1086 2023-05-21 17:06:18.621369 json_log_viewer-0.1.2/json_log_viewer/logs/log.py
+-rw-r--r--   0        0        0      627 2023-05-22 09:54:50.987903 json_log_viewer-0.1.2/json_log_viewer/logs/test_log.py
+-rw-r--r--   0        0        0     1005 2023-05-22 09:54:50.996869 json_log_viewer-0.1.2/json_log_viewer/logs/tree.py
+-rw-r--r--   0        0        0      317 2023-05-22 09:54:51.002158 json_log_viewer-0.1.2/json_log_viewer/test_version.py
+-rw-r--r--   0        0        0      556 2023-05-22 20:00:16.630123 json_log_viewer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 json_log_viewer-0.1.2/PKG-INFO
```

### Comparing `json_log_viewer-0.1.1/README.md` & `json_log_viewer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `json_log_viewer-0.1.1/json_log_viewer/__main__.py` & `json_log_viewer-0.1.2/json_log_viewer/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from docopt import docopt
 
 from json_log_viewer.extractor.extract import extract_from_file
 from json_log_viewer.logs.log import JsonLog
 from json_log_viewer.logs.tree import TreeApp
 
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 
 
 def main(files: list[str]):
     json_logs: list[JsonLog] = []
     for f in files:
         path = Path(f)
         raw_logs = extract_from_file(path)
```

### Comparing `json_log_viewer-0.1.1/json_log_viewer/extractor/extract.py` & `json_log_viewer-0.1.2/json_log_viewer/extractor/extract.py`

 * *Files identical despite different names*

### Comparing `json_log_viewer-0.1.1/json_log_viewer/extractor/test_extract.py` & `json_log_viewer-0.1.2/json_log_viewer/extractor/test_extract.py`

 * *Files identical despite different names*

### Comparing `json_log_viewer-0.1.1/json_log_viewer/logs/log.py` & `json_log_viewer-0.1.2/json_log_viewer/logs/log.py`

 * *Files identical despite different names*

### Comparing `json_log_viewer-0.1.1/json_log_viewer/logs/test_log.py` & `json_log_viewer-0.1.2/json_log_viewer/logs/test_log.py`

 * *Files identical despite different names*

### Comparing `json_log_viewer-0.1.1/json_log_viewer/logs/tree.py` & `json_log_viewer-0.1.2/json_log_viewer/logs/tree.py`

 * *Files identical despite different names*

### Comparing `json_log_viewer-0.1.1/pyproject.toml` & `json_log_viewer-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "json_log_viewer"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Samuel Broster <sam@broster.dev>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 textual = "^0.26.0"
@@ -20,8 +20,8 @@
 pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-jlv = "jlv.__main__:run"
+jlv = "json_log_viewer.__main__:run"
```

### Comparing `json_log_viewer-0.1.1/PKG-INFO` & `json_log_viewer-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-log-viewer
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Samuel Broster
 Author-email: sam@broster.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
```

