# Comparing `tmp/ezq-3.0.2.tar.gz` & `tmp/ezq-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezq-3.0.2.tar", last modified: Mon May 22 02:34:14 2023, max compression
+gzip compressed data, was "ezq-3.0.3.tar", last modified: Mon May 22 02:34:44 2023, max compression
```

## Comparing `ezq-3.0.2.tar` & `ezq-3.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:14.274775 ezq-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-22 02:33:59.000000 ezq-3.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-22 02:34:14.274775 ezq-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-05-22 02:33:59.000000 ezq-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-22 02:33:59.000000 ezq-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 02:34:14.274775 ezq-3.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:14.270775 ezq-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:14.274775 ezq-3.0.2/src/ezq/
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-05-22 02:33:59.000000 ezq-3.0.2/src/ezq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:14.274775 ezq-3.0.2/src/ezq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-22 02:34:14.000000 ezq-3.0.2/src/ezq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-22 02:34:14.000000 ezq-3.0.2/src/ezq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 02:34:14.000000 ezq-3.0.2/src/ezq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 02:34:14.000000 ezq-3.0.2/src/ezq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 02:34:14.000000 ezq-3.0.2/src/ezq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:14.274775 ezq-3.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-22 02:33:59.000000 ezq-3.0.2/test/test_ezq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-22 02:33:59.000000 ezq-3.0.2/test/test_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:44.530097 ezq-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-22 02:34:26.000000 ezq-3.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-22 02:34:44.530097 ezq-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-05-22 02:34:26.000000 ezq-3.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-22 02:34:26.000000 ezq-3.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 02:34:44.530097 ezq-3.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:44.530097 ezq-3.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:44.530097 ezq-3.0.3/src/ezq/
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-05-22 02:34:26.000000 ezq-3.0.3/src/ezq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:44.530097 ezq-3.0.3/src/ezq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-22 02:34:44.000000 ezq-3.0.3/src/ezq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-22 02:34:44.000000 ezq-3.0.3/src/ezq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 02:34:44.000000 ezq-3.0.3/src/ezq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 02:34:44.000000 ezq-3.0.3/src/ezq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 02:34:44.000000 ezq-3.0.3/src/ezq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:44.530097 ezq-3.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-22 02:34:26.000000 ezq-3.0.3/test/test_ezq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-22 02:34:26.000000 ezq-3.0.3/test/test_iter.py
```

### Comparing `ezq-3.0.2/LICENSE.md` & `ezq-3.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ezq-3.0.2/PKG-INFO` & `ezq-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezq
-Version: 3.0.2
+Version: 3.0.3
 Summary: Simple wrapper for python multiprocessing and threading.
 Author-email: Metaist LLC <metaist@metaist.com>
 License: MIT
 Project-URL: Homepage, https://github.com/metaist/ezq
 Project-URL: Documentation, https://metaist.github.io/ezq/
 Project-URL: Repository, https://github.com/metaist/ezq.git
 Project-URL: Changelog, https://github.com/metaist/ezq/blob/main/CHANGELOG.md
```

### Comparing `ezq-3.0.2/README.md` & `ezq-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ezq-3.0.2/pyproject.toml` & `ezq-3.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "ezq"
-version = "3.0.2"
+version = "3.0.3"
 description = "Simple wrapper for python multiprocessing and threading."
 keywords = ["queue", "worker", "multiprocessing", "threading"]
 requires-python = ">=3.8"
 dependencies = [
   # library dependencies support a range
   "multiprocess~=0.70.14",
 ]
```

### Comparing `ezq-3.0.2/src/ezq/__init__.py` & `ezq-3.0.3/src/ezq/__init__.py`

 * *Files identical despite different names*

### Comparing `ezq-3.0.2/src/ezq.egg-info/PKG-INFO` & `ezq-3.0.3/src/ezq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezq
-Version: 3.0.2
+Version: 3.0.3
 Summary: Simple wrapper for python multiprocessing and threading.
 Author-email: Metaist LLC <metaist@metaist.com>
 License: MIT
 Project-URL: Homepage, https://github.com/metaist/ezq
 Project-URL: Documentation, https://metaist.github.io/ezq/
 Project-URL: Repository, https://github.com/metaist/ezq.git
 Project-URL: Changelog, https://github.com/metaist/ezq/blob/main/CHANGELOG.md
```

### Comparing `ezq-3.0.2/test/test_ezq.py` & `ezq-3.0.3/test/test_ezq.py`

 * *Files identical despite different names*

### Comparing `ezq-3.0.2/test/test_iter.py` & `ezq-3.0.3/test/test_iter.py`

 * *Files identical despite different names*

