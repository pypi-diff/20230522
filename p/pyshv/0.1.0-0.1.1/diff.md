# Comparing `tmp/pyshv-0.1.0.tar.gz` & `tmp/pyshv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyshv-0.1.0.tar", last modified: Thu Apr 20 13:57:53 2023, max compression
+gzip compressed data, was "pyshv-0.1.1.tar", last modified: Mon May 22 19:34:04 2023, max compression
```

## Comparing `pyshv-0.1.0.tar` & `pyshv-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2023-04-20 13:57:53.936587 pyshv-0.1.0/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1071 2022-11-15 13:44:11.000000 pyshv-0.1.0/LICENSE
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1827 2023-04-20 13:57:53.936587 pyshv-0.1.0/PKG-INFO
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1205 2023-04-13 16:55:42.000000 pyshv-0.1.0/README.rst
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2023-04-20 13:57:53.931587 pyshv-0.1.0/docs/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1110 2023-04-13 16:55:42.000000 pyshv-0.1.0/docs/conf.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1612 2023-04-20 13:57:41.000000 pyshv-0.1.0/pyproject.toml
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2023-04-20 13:57:53.932587 pyshv-0.1.0/pyshv.egg-info/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1827 2023-04-20 13:57:53.000000 pyshv-0.1.0/pyshv.egg-info/PKG-INFO
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      576 2023-04-20 13:57:53.000000 pyshv-0.1.0/pyshv.egg-info/SOURCES.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)        1 2023-04-20 13:57:53.000000 pyshv-0.1.0/pyshv.egg-info/dependency_links.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)       52 2023-04-20 13:57:53.000000 pyshv-0.1.0/pyshv.egg-info/entry_points.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      128 2023-04-20 13:57:53.000000 pyshv-0.1.0/pyshv.egg-info/requires.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)       28 2023-04-20 13:57:53.000000 pyshv-0.1.0/pyshv.egg-info/top_level.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)       38 2023-04-20 13:57:53.936587 pyshv-0.1.0/setup.cfg
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2023-04-20 13:57:53.934587 pyshv-0.1.0/shv/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      476 2023-04-20 06:37:14.000000 pyshv-0.1.0/shv/__init__.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    15479 2023-04-20 10:30:04.000000 pyshv-0.1.0/shv/chainpack.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7438 2023-04-13 16:55:42.000000 pyshv-0.1.0/shv/clientconnection.py
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2023-04-20 13:57:53.934587 pyshv-0.1.0/shv/cp2cp/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      135 2023-04-20 12:01:13.000000 pyshv-0.1.0/shv/cp2cp/__init__.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2134 2023-04-20 12:01:13.000000 pyshv-0.1.0/shv/cp2cp/__main__.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1990 2023-04-20 12:01:13.000000 pyshv-0.1.0/shv/cp2cp/cp2cp.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1396 2023-04-20 10:45:03.000000 pyshv-0.1.0/shv/cpcontext.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    23349 2023-04-13 16:55:42.000000 pyshv-0.1.0/shv/cpon.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)        0 2023-04-07 07:26:23.000000 pyshv-0.1.0/shv/py.typed
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     8107 2023-04-20 12:01:13.000000 pyshv-0.1.0/shv/rpcclient.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4610 2023-04-14 16:19:51.000000 pyshv-0.1.0/shv/rpcmessage.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      229 2023-04-13 10:55:09.000000 pyshv-0.1.0/shv/rpcprotocol.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2211 2023-04-14 17:02:30.000000 pyshv-0.1.0/shv/rpcserver.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     6960 2023-04-18 18:19:33.000000 pyshv-0.1.0/shv/rpcvalue.py
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2023-04-20 13:57:53.935587 pyshv-0.1.0/tests/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)        0 2023-04-03 08:25:38.000000 pyshv-0.1.0/tests/__init__.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1607 2023-04-20 12:01:13.000000 pyshv-0.1.0/tests/conftest.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      462 2023-04-20 12:01:13.000000 pyshv-0.1.0/tests/test_client.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2911 2023-04-13 16:55:42.000000 pyshv-0.1.0/tests/test_conversions.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2872 2023-04-20 12:01:13.000000 pyshv-0.1.0/tests/test_example.py
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2023-05-22 19:34:04.731304 pyshv-0.1.1/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1071 2022-11-15 13:44:11.000000 pyshv-0.1.1/LICENSE
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1808 2023-05-22 19:34:04.731304 pyshv-0.1.1/PKG-INFO
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1186 2023-04-20 14:09:00.000000 pyshv-0.1.1/README.rst
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2023-05-22 19:34:04.724304 pyshv-0.1.1/docs/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1110 2023-05-22 19:31:56.000000 pyshv-0.1.1/docs/conf.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1622 2023-05-22 19:33:50.000000 pyshv-0.1.1/pyproject.toml
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2023-05-22 19:34:04.726304 pyshv-0.1.1/pyshv.egg-info/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1808 2023-05-22 19:34:04.000000 pyshv-0.1.1/pyshv.egg-info/PKG-INFO
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      624 2023-05-22 19:34:04.000000 pyshv-0.1.1/pyshv.egg-info/SOURCES.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)        1 2023-05-22 19:34:04.000000 pyshv-0.1.1/pyshv.egg-info/dependency_links.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)       52 2023-05-22 19:34:04.000000 pyshv-0.1.1/pyshv.egg-info/entry_points.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      128 2023-05-22 19:34:04.000000 pyshv-0.1.1/pyshv.egg-info/requires.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)       40 2023-05-22 19:34:04.000000 pyshv-0.1.1/pyshv.egg-info/top_level.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)       38 2023-05-22 19:34:04.731304 pyshv-0.1.1/setup.cfg
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2023-05-22 19:34:04.729304 pyshv-0.1.1/shv/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      476 2023-05-22 19:31:56.000000 pyshv-0.1.1/shv/__init__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    15479 2023-05-22 19:31:56.000000 pyshv-0.1.1/shv/chainpack.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7478 2023-05-22 19:31:56.000000 pyshv-0.1.1/shv/clientconnection.py
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2023-05-22 19:34:04.729304 pyshv-0.1.1/shv/cp2cp/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      135 2023-04-20 12:01:13.000000 pyshv-0.1.1/shv/cp2cp/__init__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2134 2023-04-20 12:01:13.000000 pyshv-0.1.1/shv/cp2cp/__main__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1990 2023-05-22 19:31:56.000000 pyshv-0.1.1/shv/cp2cp/cp2cp.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1396 2023-05-22 19:31:56.000000 pyshv-0.1.1/shv/cpcontext.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    23349 2023-05-22 19:31:56.000000 pyshv-0.1.1/shv/cpon.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)        0 2023-04-07 07:26:23.000000 pyshv-0.1.1/shv/py.typed
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      962 2023-05-18 21:08:02.000000 pyshv-0.1.1/shv/rpcbroker.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     8107 2023-05-22 19:31:56.000000 pyshv-0.1.1/shv/rpcclient.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4610 2023-05-22 19:31:56.000000 pyshv-0.1.1/shv/rpcmessage.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      229 2023-04-13 10:55:09.000000 pyshv-0.1.1/shv/rpcprotocol.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2211 2023-04-14 17:02:30.000000 pyshv-0.1.1/shv/rpcserver.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     6960 2023-05-22 19:31:56.000000 pyshv-0.1.1/shv/rpcvalue.py
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2023-05-22 19:34:04.731304 pyshv-0.1.1/tests/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)        0 2023-04-03 08:25:38.000000 pyshv-0.1.1/tests/__init__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1607 2023-05-22 19:31:56.000000 pyshv-0.1.1/tests/conftest.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      462 2023-05-22 19:31:56.000000 pyshv-0.1.1/tests/test_client.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2199 2023-05-22 19:31:56.000000 pyshv-0.1.1/tests/test_clientconnection.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2911 2023-05-22 19:31:56.000000 pyshv-0.1.1/tests/test_conversions.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2872 2023-05-22 19:31:56.000000 pyshv-0.1.1/tests/test_example.py
```

### Comparing `pyshv-0.1.0/LICENSE` & `pyshv-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyshv-0.1.0/PKG-INFO` & `pyshv-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshv
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pure Python SHV implementation
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.com/elektroline-predator/pyshv
 Project-URL: Bug Tracker, https://gitlab.com/elektroline-predator/pyshv/-/issues
 Project-URL: Github, https://github.com/silicon-heaven/libshv-py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,16 +30,14 @@
 
 
 Installation
 ------------
 
 The installation can be done with package manager `pip`.
 
-    pip install .
-
 
 Running tests
 -------------
 
 This project contains tests in directory tests.
 
 To run tests you have to use **pytest**. To run all tests just run it in the top
```

### Comparing `pyshv-0.1.0/README.rst` & `pyshv-0.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 
 
 Installation
 ------------
 
 The installation can be done with package manager `pip`.
 
-    pip install .
-
 
 Running tests
 -------------
 
 This project contains tests in directory tests.
 
 To run tests you have to use **pytest**. To run all tests just run it in the top
```

### Comparing `pyshv-0.1.0/docs/conf.py` & `pyshv-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.1.0/pyproject.toml` & `pyshv-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [project]
 name = "pyshv"
-version = "0.1.0"
+version = "0.1.1"
 description = "Pure Python SHV implementation"
 readme = "README.rst"
 authors = [
   { name="Elektroline a.s." },
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
-dependencies = []
 
 [project.urls]
 "Homepage" = "https://gitlab.com/elektroline-predator/pyshv"
 "Bug Tracker" = "https://gitlab.com/elektroline-predator/pyshv/-/issues"
 "Github" = "https://github.com/silicon-heaven/libshv-py"
 
 [project.optional-dependencies]
@@ -42,14 +41,15 @@
 pycp2cp = "shv.cp2cp.__main__:main"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
+exclude = ["docs", "tests"]
 [tool.setuptools.package-data]
 "*" = ["py.typed"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.isort]
```

### Comparing `pyshv-0.1.0/pyshv.egg-info/PKG-INFO` & `pyshv-0.1.1/pyshv.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshv
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pure Python SHV implementation
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.com/elektroline-predator/pyshv
 Project-URL: Bug Tracker, https://gitlab.com/elektroline-predator/pyshv/-/issues
 Project-URL: Github, https://github.com/silicon-heaven/libshv-py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,16 +30,14 @@
 
 
 Installation
 ------------
 
 The installation can be done with package manager `pip`.
 
-    pip install .
-
 
 Running tests
 -------------
 
 This project contains tests in directory tests.
 
 To run tests you have to use **pytest**. To run all tests just run it in the top
```

### Comparing `pyshv-0.1.0/pyshv.egg-info/SOURCES.txt` & `pyshv-0.1.1/pyshv.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 pyshv.egg-info/top_level.txt
 shv/__init__.py
 shv/chainpack.py
 shv/clientconnection.py
 shv/cpcontext.py
 shv/cpon.py
 shv/py.typed
+shv/rpcbroker.py
 shv/rpcclient.py
 shv/rpcmessage.py
 shv/rpcprotocol.py
 shv/rpcserver.py
 shv/rpcvalue.py
 shv/cp2cp/__init__.py
 shv/cp2cp/__main__.py
 shv/cp2cp/cp2cp.py
 tests/__init__.py
 tests/conftest.py
 tests/test_client.py
+tests/test_clientconnection.py
 tests/test_conversions.py
 tests/test_example.py
```

### Comparing `pyshv-0.1.0/shv/chainpack.py` & `pyshv-0.1.1/shv/chainpack.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.1.0/shv/clientconnection.py` & `pyshv-0.1.1/shv/clientconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,17 @@
                         asyncio.get_event_loop().call_soon(
                             handler, path, msg.params().value
                         )
 
     def _get_signal_handler(self, shv_path: str) -> None | typing.Callable:
         """Get the handler for the longest path match."""
         split_key = shv_path.split("/")
-        paths = ("/".join(split_key[:i]) for i in range(len(split_key)))
+        paths = (
+            "/".join(split_key[: len(split_key) - i]) for i in range(len(split_key))
+        )
         return next(
             (
                 self._signal_handlers[path]
                 for path in paths
                 if path in self._signal_handlers
             ),
             None,
```

### Comparing `pyshv-0.1.0/shv/cp2cp/__main__.py` & `pyshv-0.1.1/shv/cp2cp/__main__.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.1.0/shv/cp2cp/cp2cp.py` & `pyshv-0.1.1/shv/cp2cp/cp2cp.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.1.0/shv/cpcontext.py` & `pyshv-0.1.1/shv/cpcontext.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.1.0/shv/cpon.py` & `pyshv-0.1.1/shv/cpon.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.1.0/shv/rpcclient.py` & `pyshv-0.1.1/shv/rpcclient.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.1.0/shv/rpcmessage.py` & `pyshv-0.1.1/shv/rpcmessage.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.1.0/shv/rpcserver.py` & `pyshv-0.1.1/shv/rpcserver.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.1.0/shv/rpcvalue.py` & `pyshv-0.1.1/shv/rpcvalue.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.1.0/tests/conftest.py` & `pyshv-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.1.0/tests/test_conversions.py` & `pyshv-0.1.1/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.1.0/tests/test_example.py` & `pyshv-0.1.1/tests/test_example.py`

 * *Files identical despite different names*

