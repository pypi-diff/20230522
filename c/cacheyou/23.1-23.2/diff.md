# Comparing `tmp/cacheyou-23.1.tar.gz` & `tmp/cacheyou-23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacheyou-23.1.tar", last modified: Fri May 19 10:41:10 2023, max compression
+gzip compressed data, was "cacheyou-23.2.tar", last modified: Mon May 22 08:29:46 2023, max compression
```

## Comparing `cacheyou-23.1.tar` & `cacheyou-23.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      575 2023-05-19 10:40:54.836398 cacheyou-23.1/LICENSE.txt
--rw-r--r--   0        0        0      830 2023-05-19 10:40:54.836398 cacheyou-23.1/README.md
--rw-r--r--   0        0        0      516 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/_cmd.py
--rw-r--r--   0        0        0     5832 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/adapter.py
--rw-r--r--   0        0        0     1895 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/cache.py
--rw-r--r--   0        0        0      288 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/caches/__init__.py
--rw-r--r--   0        0        0     5347 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/caches/file_cache.py
--rw-r--r--   0        0        0     1709 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/caches/redis_cache.py
--rw-r--r--   0        0        0    17699 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/controller.py
--rw-r--r--   0        0        0     4208 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/filewrapper.py
--rw-r--r--   0        0        0     4808 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/heuristics.py
--rw-r--r--   0        0        0        0 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/py.typed
--rw-r--r--   0        0        0     7348 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/serialize.py
--rw-r--r--   0        0        0     1284 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/wrapper.py
--rw-r--r--   0        0        0     5673 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/Makefile
--rw-r--r--   0        0        0     8119 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/conf.py
--rw-r--r--   0        0        0     5478 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/custom_heuristics.rst
--rw-r--r--   0        0        0     5209 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/etags.rst
--rw-r--r--   0        0        0     2289 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/index.rst
--rw-r--r--   0        0        0     4085 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/release_notes.rst
--rw-r--r--   0        0        0      643 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/requirements.txt
--rw-r--r--   0        0        0     4297 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/storage.rst
--rw-r--r--   0        0        0     2372 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/tips.rst
--rw-r--r--   0        0        0     1792 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/usage.rst
--rw-r--r--   0        0        0     2626 2023-05-19 10:41:10.088362 cacheyou-23.1/pyproject.toml
--rw-r--r--   0        0        0       30 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/__init__.py
--rw-r--r--   0        0        0     4750 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/conftest.py
--rw-r--r--   0        0        0     1114 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/issue_263.py
--rw-r--r--   0        0        0     1682 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_adapter.py
--rw-r--r--   0        0        0    10845 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_cache_control.py
--rw-r--r--   0        0        0     1470 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_chunked_response.py
--rw-r--r--   0        0        0     5110 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_etag.py
--rw-r--r--   0        0        0     6679 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_expires_heuristics.py
--rw-r--r--   0        0        0     1747 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_max_age.py
--rw-r--r--   0        0        0     1597 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_redirects.py
--rw-r--r--   0        0        0      941 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_regressions.py
--rw-r--r--   0        0        0     5484 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_serialization.py
--rw-r--r--   0        0        0      259 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_server_http_version.py
--rw-r--r--   0        0        0     5689 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_storage_filecache.py
--rw-r--r--   0        0        0      789 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_storage_redis.py
--rw-r--r--   0        0        0     2957 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_vary.py
--rw-r--r--   0        0        0      792 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/utils.py
--rw-r--r--   0        0        0      484 2023-05-19 10:40:54.840398 cacheyou-23.1/tox.ini
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 cacheyou-23.1/PKG-INFO
+-rw-r--r--   0        0        0      575 2023-05-22 08:29:27.176707 cacheyou-23.2/LICENSE.txt
+-rw-r--r--   0        0        0      830 2023-05-22 08:29:27.176707 cacheyou-23.2/README.md
+-rw-r--r--   0        0        0      516 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/_cmd.py
+-rw-r--r--   0        0        0     5832 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/adapter.py
+-rw-r--r--   0        0        0     1895 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/cache.py
+-rw-r--r--   0        0        0      288 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/caches/__init__.py
+-rw-r--r--   0        0        0     5347 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/caches/file_cache.py
+-rw-r--r--   0        0        0     1709 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/caches/redis_cache.py
+-rw-r--r--   0        0        0    17699 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/controller.py
+-rw-r--r--   0        0        0     4208 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/filewrapper.py
+-rw-r--r--   0        0        0     4808 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/heuristics.py
+-rw-r--r--   0        0        0        0 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/py.typed
+-rw-r--r--   0        0        0     7612 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/serialize.py
+-rw-r--r--   0        0        0     1284 2023-05-22 08:29:27.176707 cacheyou-23.2/cacheyou/wrapper.py
+-rw-r--r--   0        0        0     5673 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/Makefile
+-rw-r--r--   0        0        0     8119 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/conf.py
+-rw-r--r--   0        0        0     5478 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/custom_heuristics.rst
+-rw-r--r--   0        0        0     5209 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/etags.rst
+-rw-r--r--   0        0        0     2289 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/index.rst
+-rw-r--r--   0        0        0     4161 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/release_notes.rst
+-rw-r--r--   0        0        0      643 2023-05-22 08:29:27.176707 cacheyou-23.2/docs/requirements.txt
+-rw-r--r--   0        0        0     4297 2023-05-22 08:29:27.180707 cacheyou-23.2/docs/storage.rst
+-rw-r--r--   0        0        0     2372 2023-05-22 08:29:27.180707 cacheyou-23.2/docs/tips.rst
+-rw-r--r--   0        0        0     1792 2023-05-22 08:29:27.180707 cacheyou-23.2/docs/usage.rst
+-rw-r--r--   0        0        0     2626 2023-05-22 08:29:46.849022 cacheyou-23.2/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/__init__.py
+-rw-r--r--   0        0        0     4750 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/conftest.py
+-rw-r--r--   0        0        0     1114 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/issue_263.py
+-rw-r--r--   0        0        0     1682 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_adapter.py
+-rw-r--r--   0        0        0    10845 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_cache_control.py
+-rw-r--r--   0        0        0     1470 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_chunked_response.py
+-rw-r--r--   0        0        0     5110 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_etag.py
+-rw-r--r--   0        0        0     6679 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_expires_heuristics.py
+-rw-r--r--   0        0        0     1747 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_max_age.py
+-rw-r--r--   0        0        0     1597 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_redirects.py
+-rw-r--r--   0        0        0      941 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_regressions.py
+-rw-r--r--   0        0        0     5484 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_serialization.py
+-rw-r--r--   0        0        0      259 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_server_http_version.py
+-rw-r--r--   0        0        0     5689 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_storage_filecache.py
+-rw-r--r--   0        0        0      789 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_storage_redis.py
+-rw-r--r--   0        0        0     2957 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/test_vary.py
+-rw-r--r--   0        0        0      792 2023-05-22 08:29:27.180707 cacheyou-23.2/tests/utils.py
+-rw-r--r--   0        0        0      484 2023-05-22 08:29:27.180707 cacheyou-23.2/tox.ini
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 cacheyou-23.2/PKG-INFO
```

### Comparing `cacheyou-23.1/LICENSE.txt` & `cacheyou-23.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/README.md` & `cacheyou-23.2/README.md`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/cacheyou/__init__.py` & `cacheyou-23.2/cacheyou/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 """
 import logging
 
 from cacheyou.adapter import CacheControlAdapter
 from cacheyou.controller import CacheController
 from cacheyou.wrapper import CacheControl
 
-__version__ = "23.1"
+__version__ = "23.2"
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __all__ = ("CacheControl", "CacheControlAdapter", "CacheController")
```

### Comparing `cacheyou-23.1/cacheyou/_cmd.py` & `cacheyou-23.2/cacheyou/_cmd.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/cacheyou/adapter.py` & `cacheyou-23.2/cacheyou/adapter.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/cacheyou/cache.py` & `cacheyou-23.2/cacheyou/cache.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/cacheyou/caches/file_cache.py` & `cacheyou-23.2/cacheyou/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/cacheyou/caches/redis_cache.py` & `cacheyou-23.2/cacheyou/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/cacheyou/controller.py` & `cacheyou-23.2/cacheyou/controller.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/cacheyou/filewrapper.py` & `cacheyou-23.2/cacheyou/filewrapper.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/cacheyou/heuristics.py` & `cacheyou-23.2/cacheyou/heuristics.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/cacheyou/serialize.py` & `cacheyou-23.2/cacheyou/serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import base64
+import inspect
 import io
 import json
 import pickle
 import typing as t
 import zlib
 
 import msgpack
@@ -50,14 +51,16 @@
                 "headers": {str(k): str(v) for k, v in response.headers.items()},
                 "status": response.status,
                 "version": response.version,
                 "reason": str(response.reason),
                 "decode_content": response.decode_content,
             }
         }
+        if hasattr(response, "strict"):
+            data["response"]["strict"] = response.strict  # type: ignore[attr-defined]
 
         # Construct our vary headers
         data["vary"] = {}
         if "vary" in response_headers:
             varied_headers = response_headers["vary"].split(",")
             for header in varied_headers:
                 header = str(header).strip()
@@ -123,28 +126,30 @@
 
         headers: t.MutableMapping[str, str] = CaseInsensitiveDict(
             data=cached["response"]["headers"]
         )
         if headers.get("transfer-encoding", "") == "chunked":
             headers.pop("transfer-encoding")
 
-        cached["response"]["headers"] = headers
-
         try:
             if body_file is None:
                 body_file = io.BytesIO(body_raw)
         except TypeError:
             # This can happen if cachecontrol serialized to v1 format (pickle)
             # using Python 2. A Python 2 str(byte string) will be unpickled as
             # a Python 3 str (unicode string), which will cause the above to
             # fail with:
             #
             #     TypeError: 'str' does not support the buffer interface
             body_file = io.BytesIO(body_raw.encode("utf8"))
 
+        cached["response"]["headers"] = headers
+        if "strict" not in inspect.signature(HTTPResponse).parameters:
+            cached["response"].pop("strict", None)
+
         return HTTPResponse(body=body_file, preload_content=False, **cached["response"])
 
     def _loads_v0(
         self, request: PreparedRequest, data: bytes, body_file: t.IO[bytes] | None = None
     ) -> HTTPResponse | None:
         # The original legacy cache data. This doesn't contain enough
         # information to construct everything we need, so we'll treat this as
```

### Comparing `cacheyou-23.1/cacheyou/wrapper.py` & `cacheyou-23.2/cacheyou/wrapper.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/docs/Makefile` & `cacheyou-23.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/docs/conf.py` & `cacheyou-23.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 copyright = "2013, Eric Larson, 2023 Frost Ming"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = "23.1"
+release = "23.2"
 # The short X.Y version.
 version = release
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
```

### Comparing `cacheyou-23.1/docs/custom_heuristics.rst` & `cacheyou-23.2/docs/custom_heuristics.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/docs/etags.rst` & `cacheyou-23.2/docs/etags.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/docs/index.rst` & `cacheyou-23.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/docs/release_notes.rst` & `cacheyou-23.2/docs/release_notes.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
   SPDX-License-Identifier: Apache-2.0
 
 ===============
  Release Notes
 ===============
 
+23.2
+====
+
+* Handle ``strict`` parameter for both ``urllib3`` 1.x and 2.x.
+
 23.1
 ====
 
 * Add type hints to the code base.
 
 23.0
 ====
```

### Comparing `cacheyou-23.1/docs/requirements.txt` & `cacheyou-23.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/docs/storage.rst` & `cacheyou-23.2/docs/storage.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/docs/tips.rst` & `cacheyou-23.2/docs/tips.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/docs/usage.rst` & `cacheyou-23.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/pyproject.toml` & `cacheyou-23.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "CacheYou"
-version = "23.1"
+version = "23.2"
 description = "httplib2 caching for requests"
 keywords = [
     "requests",
     "http",
     "caching",
     "web",
 ]
@@ -123,15 +123,15 @@
 
 [tool.ruff.isort]
 known-first-party = [
     "cacheyou",
 ]
 
 [tool.bumpver]
-current_version = "23.1"
+current_version = "23.2"
 version_pattern = "YY.INC0[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `cacheyou-23.1/tests/conftest.py` & `cacheyou-23.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/issue_263.py` & `cacheyou-23.2/tests/issue_263.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/test_adapter.py` & `cacheyou-23.2/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/test_cache_control.py` & `cacheyou-23.2/tests/test_cache_control.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/test_chunked_response.py` & `cacheyou-23.2/tests/test_chunked_response.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/test_etag.py` & `cacheyou-23.2/tests/test_etag.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/test_expires_heuristics.py` & `cacheyou-23.2/tests/test_expires_heuristics.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/test_max_age.py` & `cacheyou-23.2/tests/test_max_age.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/test_redirects.py` & `cacheyou-23.2/tests/test_redirects.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/test_regressions.py` & `cacheyou-23.2/tests/test_regressions.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/test_serialization.py` & `cacheyou-23.2/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/test_storage_filecache.py` & `cacheyou-23.2/tests/test_storage_filecache.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/test_storage_redis.py` & `cacheyou-23.2/tests/test_storage_redis.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/test_vary.py` & `cacheyou-23.2/tests/test_vary.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/tests/utils.py` & `cacheyou-23.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.1/PKG-INFO` & `cacheyou-23.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacheyou
-Version: 23.1
+Version: 23.2
 Summary: httplib2 caching for requests
 Keywords: requests http caching web
 Author-Email: Frost Ming <me@frostming.com>, Eric Larson <eric@ionrock.org>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

