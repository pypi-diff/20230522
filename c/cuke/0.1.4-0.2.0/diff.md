# Comparing `tmp/cuke-0.1.4.tar.gz` & `tmp/cuke-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuke-0.1.4.tar", max compression
+gzip compressed data, was "cuke-0.2.0.tar", max compression
```

## Comparing `cuke-0.1.4.tar` & `cuke-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      405 2023-05-22 01:12:36.747300 cuke-0.1.4/README.md
--rw-r--r--   0        0        0    13069 2023-05-22 01:12:36.747300 cuke-0.1.4/cuke/__init__.py
--rw-r--r--   0        0        0      655 2023-05-22 01:12:36.747300 cuke-0.1.4/cuke/errors.py
--rw-r--r--   0        0        0     1702 2023-05-22 01:12:36.747300 cuke-0.1.4/cuke/util.py
--rw-r--r--   0        0        0      775 2023-05-22 01:12:36.747300 cuke-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 cuke-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      405 2023-05-22 04:37:24.606623 cuke-0.2.0/README.md
+-rw-r--r--   0        0        0    13286 2023-05-22 04:37:24.606623 cuke-0.2.0/cuke/__init__.py
+-rw-r--r--   0        0        0      655 2023-05-22 04:37:24.606623 cuke-0.2.0/cuke/errors.py
+-rw-r--r--   0        0        0      394 2023-05-22 04:37:24.606623 cuke-0.2.0/cuke/types.py
+-rw-r--r--   0        0        0     1702 2023-05-22 04:37:24.606623 cuke-0.2.0/cuke/util.py
+-rw-r--r--   0        0        0      775 2023-05-22 04:37:24.610623 cuke-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 cuke-0.2.0/PKG-INFO
```

### Comparing `cuke-0.1.4/cuke/__init__.py` & `cuke-0.2.0/cuke/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import time
 import weakref
 
 import requests
 from requests.exceptions import HTTPError
 
 from cuke.errors import NoApiKey, NoPageYet, SetPageIdOnInitialization
+from cuke.types import Image
 from cuke.util import add_header_to_function, get_function_body, make_request_in_api_key_order
 
 KEYS_TO_NOT_UPDATE = {"_dirty_set", "_instant_updates", "_vars", "_vars_lock", "_daemon",
                       "_contributor_key", "_editor_key", "_page_id", "_page_subslug", "_page_slug",
                       "_views"}
 
 class Cuke:
@@ -216,14 +217,16 @@
                     continue
                 elif str(type(self._vars[k])) == "<class 'matplotlib.figure.Figure'>":
                     buf = io.BytesIO()
                     self._vars[k].savefig(buf, format="png")
                     update[k] = {"type": "png_b64", "value": base64.b64encode(buf.getvalue()).decode() }
                 elif str(type(self._vars[k])) == "<class 'function'>":
                     update[k] = {"type": "function", "value": get_function_body(self._vars[k]) }
+                elif str(type(self._vars[k])) == "<class 'cuke.types.Image'>":
+                    update[k] = {"type": "png_b64", "value": base64.b64encode(self._vars[k].data).decode() }
                 else:
                     update[k] = {"type": "error", "value": f"Could not serialize. {e}" }
         # TODO this needs error handling or it kills the thread
         if os.environ.get("CUKE_PIPELINE_STAGE", None):
             headers = {"X-Cuke-Pipeline-Stage": os.environ["CUKE_PIPELINE_STAGE"]}
         else:
             headers = {}
```

### Comparing `cuke-0.1.4/cuke/errors.py` & `cuke-0.2.0/cuke/errors.py`

 * *Files identical despite different names*

### Comparing `cuke-0.1.4/cuke/util.py` & `cuke-0.2.0/cuke/util.py`

 * *Files identical despite different names*

### Comparing `cuke-0.1.4/pyproject.toml` & `cuke-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cuke"
-version = "0.1.4"
+version = "0.2.0"
 description = "Python client for cuke.cool"
 authors = ["tomgrek <tom.grek@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cuke"}]
 homepage = "https://cuke.cool"
 repository = "https://github.com/tomgrek/cuke.cool"
 documentation = "https://docs.cuke.cool"
```

### Comparing `cuke-0.1.4/PKG-INFO` & `cuke-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuke
-Version: 0.1.4
+Version: 0.2.0
 Summary: Python client for cuke.cool
 Home-page: https://cuke.cool
 Keywords: publishing,faas,serverless,webpage,python
 Author: tomgrek
 Author-email: tom.grek@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

