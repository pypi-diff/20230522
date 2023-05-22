# Comparing `tmp/ttcore-0.1.7.tar.gz` & `tmp/ttcore-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttcore-0.1.7.tar", last modified: Wed May 17 12:32:57 2023, max compression
+gzip compressed data, was "ttcore-0.1.8.tar", last modified: Mon May 22 08:33:25 2023, max compression
```

## Comparing `ttcore-0.1.7.tar` & `ttcore-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:32:57.743664 ttcore-0.1.7/
--rw-rw-r--   0 user      (1000) user      (1000)    11358 2023-03-30 08:55:21.000000 ttcore-0.1.7/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)      633 2023-05-17 12:32:57.743664 ttcore-0.1.7/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      112 2023-03-30 08:58:11.000000 ttcore-0.1.7/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      200 2023-05-17 12:32:57.744664 ttcore-0.1.7/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      871 2023-05-17 12:32:25.000000 ttcore-0.1.7/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:32:57.742664 ttcore-0.1.7/ttcore/
--rw-r--r--   0 user      (1000) user      (1000)    11747 2023-05-17 12:32:25.000000 ttcore-0.1.7/ttcore/bottle.py
--rw-r--r--   0 user      (1000) user      (1000)    10600 2023-05-17 12:32:25.000000 ttcore-0.1.7/ttcore/docs.html
--rw-rw-r--   0 user      (1000) user      (1000)      501 2023-03-30 08:55:53.000000 ttcore-0.1.7/ttcore/ip.py
--rw-r--r--   0 user      (1000) user      (1000)     2801 2023-04-03 18:50:11.000000 ttcore-0.1.7/ttcore/mailers.py
--rw-r--r--   0 user      (1000) user      (1000)     1139 2023-04-03 14:30:07.000000 ttcore-0.1.7/ttcore/messages.py
--rw-rw-r--   0 user      (1000) user      (1000)     1029 2023-03-30 08:55:53.000000 ttcore-0.1.7/ttcore/peewee.py
--rw-r--r--   0 user      (1000) user      (1000)     3486 2023-04-03 14:30:07.000000 ttcore-0.1.7/ttcore/utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:32:57.743664 ttcore-0.1.7/ttcore.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      633 2023-05-17 12:32:57.000000 ttcore-0.1.7/ttcore.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      331 2023-05-17 12:32:57.000000 ttcore-0.1.7/ttcore.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:32:57.000000 ttcore-0.1.7/ttcore.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-05-17 12:32:57.000000 ttcore-0.1.7/ttcore.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2023-05-17 12:32:57.000000 ttcore-0.1.7/ttcore.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-03-30 11:51:08.000000 ttcore-0.1.7/ttcore.egg-info/zip-safe
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-22 08:33:25.638784 ttcore-0.1.8/
+-rw-rw-r--   0 user      (1000) user      (1000)    11358 2023-03-30 08:55:21.000000 ttcore-0.1.8/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)      633 2023-05-22 08:33:25.638784 ttcore-0.1.8/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      112 2023-03-30 08:58:11.000000 ttcore-0.1.8/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      200 2023-05-22 08:33:25.639784 ttcore-0.1.8/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      871 2023-05-22 08:33:17.000000 ttcore-0.1.8/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-22 08:33:25.635784 ttcore-0.1.8/ttcore/
+-rw-r--r--   0 user      (1000) user      (1000)    11747 2023-05-22 08:33:17.000000 ttcore-0.1.8/ttcore/bottle.py
+-rw-r--r--   0 user      (1000) user      (1000)    10600 2023-05-17 12:32:25.000000 ttcore-0.1.8/ttcore/docs.html
+-rw-rw-r--   0 user      (1000) user      (1000)      501 2023-03-30 08:55:53.000000 ttcore-0.1.8/ttcore/ip.py
+-rw-r--r--   0 user      (1000) user      (1000)     2801 2023-04-03 18:50:11.000000 ttcore-0.1.8/ttcore/mailers.py
+-rw-r--r--   0 user      (1000) user      (1000)     1139 2023-04-03 14:30:07.000000 ttcore-0.1.8/ttcore/messages.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1029 2023-03-30 08:55:53.000000 ttcore-0.1.8/ttcore/peewee.py
+-rw-r--r--   0 user      (1000) user      (1000)     3486 2023-04-03 14:30:07.000000 ttcore-0.1.8/ttcore/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-22 08:33:25.637784 ttcore-0.1.8/ttcore.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      633 2023-05-22 08:33:25.000000 ttcore-0.1.8/ttcore.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      331 2023-05-22 08:33:25.000000 ttcore-0.1.8/ttcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-22 08:33:25.000000 ttcore-0.1.8/ttcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-05-22 08:33:25.000000 ttcore-0.1.8/ttcore.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2023-05-22 08:33:25.000000 ttcore-0.1.8/ttcore.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-03-30 11:51:08.000000 ttcore-0.1.8/ttcore.egg-info/zip-safe
```

### Comparing `ttcore-0.1.7/LICENSE.txt` & `ttcore-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.7/PKG-INFO` & `ttcore-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttcore
-Version: 0.1.7
+Version: 0.1.8
 Summary: Atomic Batteries Included. Used by https://tigerteamx.com to maximize producitivty.
 Home-page: https://github.com/tigerteamx/ttcore
 Author: Martin F
 Author-email: pypi.org@tigerteamx.com
 Keywords: productivity,bottlepy,peewee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ttcore-0.1.7/setup.py` & `ttcore-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="ttcore",
-    version="0.1.7",
+    version="0.1.8",
     author="Martin F",
     author_email="pypi.org@tigerteamx.com",
     description="Atomic Batteries Included. Used by https://tigerteamx.com to maximize producitivty.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tigerteamx/ttcore",
     packages=['ttcore'],
```

### Comparing `ttcore-0.1.7/ttcore/bottle.py` & `ttcore-0.1.8/ttcore/bottle.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             params=doc_params,
         ))
 
         @wraps(func)
         @post(path)
         def wrapper(*args, **kwargs):
             if roles and not _auth(roles):
-                return HTTPResponse(status=403, body=dict(msg=f"Invalid access. Requires {', '.join(roles)}"))
+                return HTTPResponse(status=401, body=dict(msg=f"Invalid access. Requires {', '.join(roles)}"))
 
             data = _get_request_data() if len(params) > 0 else {}
             data = _filter_data(data, params)
             _validate_data(data, doc_params)
 
             ctx = Context(
                 path=path,
```

### Comparing `ttcore-0.1.7/ttcore/docs.html` & `ttcore-0.1.8/ttcore/docs.html`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.7/ttcore/mailers.py` & `ttcore-0.1.8/ttcore/mailers.py`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.7/ttcore/messages.py` & `ttcore-0.1.8/ttcore/messages.py`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.7/ttcore/peewee.py` & `ttcore-0.1.8/ttcore/peewee.py`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.7/ttcore/utils.py` & `ttcore-0.1.8/ttcore/utils.py`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.7/ttcore.egg-info/PKG-INFO` & `ttcore-0.1.8/ttcore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttcore
-Version: 0.1.7
+Version: 0.1.8
 Summary: Atomic Batteries Included. Used by https://tigerteamx.com to maximize producitivty.
 Home-page: https://github.com/tigerteamx/ttcore
 Author: Martin F
 Author-email: pypi.org@tigerteamx.com
 Keywords: productivity,bottlepy,peewee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

