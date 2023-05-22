# Comparing `tmp/cuke-0.1.3.tar.gz` & `tmp/cuke-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuke-0.1.3.tar", max compression
+gzip compressed data, was "cuke-0.1.4.tar", max compression
```

## Comparing `cuke-0.1.3.tar` & `cuke-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      405 2023-05-21 00:39:44.202192 cuke-0.1.3/README.md
--rw-r--r--   0        0        0    12966 2023-05-21 00:39:44.202192 cuke-0.1.3/cuke/__init__.py
--rw-r--r--   0        0        0      655 2023-05-21 00:39:44.202192 cuke-0.1.3/cuke/errors.py
--rw-r--r--   0        0        0     1702 2023-05-21 00:39:44.202192 cuke-0.1.3/cuke/util.py
--rw-r--r--   0        0        0      775 2023-05-21 00:39:44.202192 cuke-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 cuke-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      405 2023-05-22 01:12:36.747300 cuke-0.1.4/README.md
+-rw-r--r--   0        0        0    13069 2023-05-22 01:12:36.747300 cuke-0.1.4/cuke/__init__.py
+-rw-r--r--   0        0        0      655 2023-05-22 01:12:36.747300 cuke-0.1.4/cuke/errors.py
+-rw-r--r--   0        0        0     1702 2023-05-22 01:12:36.747300 cuke-0.1.4/cuke/util.py
+-rw-r--r--   0        0        0      775 2023-05-22 01:12:36.747300 cuke-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 cuke-0.1.4/PKG-INFO
```

### Comparing `cuke-0.1.3/cuke/__init__.py` & `cuke-0.1.4/cuke/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 import requests
 from requests.exceptions import HTTPError
 
 from cuke.errors import NoApiKey, NoPageYet, SetPageIdOnInitialization
 from cuke.util import add_header_to_function, get_function_body, make_request_in_api_key_order
 
 KEYS_TO_NOT_UPDATE = {"_dirty_set", "_instant_updates", "_vars", "_vars_lock", "_daemon",
-                      "_contributor_key", "_editor_key", "_page_id", "_page_subslug", "_page_slug"}
+                      "_contributor_key", "_editor_key", "_page_id", "_page_subslug", "_page_slug",
+                      "_views"}
 
 class Cuke:
     def __init__(self, url="https://cuke.cool", api_key=None, instant_updates=False,
                  page_slug=None, page_subslug=None, page_id=None, contributor_key=None,
                  editor_key=None, private=False, **kwargs):
         self._dirty_set = set()
         self._instant_updates = instant_updates
@@ -50,14 +51,15 @@
         self._event = None
         self._frame_time = None
         self._packages = []
         self._template = None
         self._basic_auth = {}
         self._code = None
         self._title = None
+        self._views = None
 
         self._private = private
 
         if self._page_id:
             self._initialize_vars()
         self._dirty_set = set()
 
@@ -135,14 +137,15 @@
         resp = resp.json()
         
         self._template = resp.pop("__template__")
         self._basic_auth = resp.pop("__basic_auth__")
         self._code = resp.pop("__code__")
         self._private = resp.pop("__private__")
         self._title = resp.pop("__title__")
+        self._views = resp.pop("__views__")
         self._frame_time = self._code.get("frame_time")
         self._packages = self._code.get("packages")
         self._ui_thread_js_for_loop_output = self._code.get("ui_thread_js_for_loop_output")
         self._ui_thread_js_for_loop_input = self._code.get("ui_thread_js_for_loop_input")
         self._webworker = self._code.get("webworker")
 
         for k in resp:
```

### Comparing `cuke-0.1.3/cuke/errors.py` & `cuke-0.1.4/cuke/errors.py`

 * *Files identical despite different names*

### Comparing `cuke-0.1.3/cuke/util.py` & `cuke-0.1.4/cuke/util.py`

 * *Files identical despite different names*

### Comparing `cuke-0.1.3/pyproject.toml` & `cuke-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cuke"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python client for cuke.cool"
 authors = ["tomgrek <tom.grek@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cuke"}]
 homepage = "https://cuke.cool"
 repository = "https://github.com/tomgrek/cuke.cool"
 documentation = "https://docs.cuke.cool"
```

### Comparing `cuke-0.1.3/PKG-INFO` & `cuke-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuke
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python client for cuke.cool
 Home-page: https://cuke.cool
 Keywords: publishing,faas,serverless,webpage,python
 Author: tomgrek
 Author-email: tom.grek@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

