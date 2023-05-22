# Comparing `tmp/plone.batching-2.0.4.tar.gz` & `tmp/plone.batching-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.batching-2.0.4.tar", last modified: Tue Mar 14 16:34:00 2023, max compression
+gzip compressed data, was "plone.batching-2.0.5.tar", last modified: Mon May 22 18:04:04 2023, max compression
```

## Comparing `plone.batching-2.0.4.tar` & `plone.batching-2.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:34:00.089463 plone.batching-2.0.4/
--rw-r--r--   0 maurits    (501) staff       (20)     4696 2023-03-14 16:33:59.000000 plone.batching-2.0.4/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-14 16:33:59.000000 plone.batching-2.0.4/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      154 2023-03-14 16:33:59.000000 plone.batching-2.0.4/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     9838 2023-03-14 16:34:00.089582 plone.batching-2.0.4/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      274 2023-03-14 16:33:59.000000 plone.batching-2.0.4/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:34:00.083560 plone.batching-2.0.4/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     2179 2023-03-14 16:33:59.000000 plone.batching-2.0.4/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      127 2023-03-14 16:33:59.000000 plone.batching-2.0.4/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3950 2023-03-14 16:33:59.000000 plone.batching-2.0.4/docs/usage.rst
--rw-r--r--   0 maurits    (501) staff       (20)      123 2023-03-14 16:33:59.000000 plone.batching-2.0.4/lint-requirements.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:34:00.083799 plone.batching-2.0.4/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:34:00.088714 plone.batching-2.0.4/plone/batching/
--rw-r--r--   0 maurits    (501) staff       (20)      168 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone/batching/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     8368 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone/batching/batch.py
--rw-r--r--   0 maurits    (501) staff       (20)      719 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone/batching/batch_macros.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4936 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone/batching/batching.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4188 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone/batching/batchnavigation.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3629 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone/batching/batchnavigation_bootstrap.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1969 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone/batching/browser.py
--rw-r--r--   0 maurits    (501) staff       (20)      586 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone/batching/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1927 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone/batching/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:34:00.089261 plone.batching-2.0.4/plone/batching/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone/batching/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    10824 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone/batching/tests/test_batching.py
--rw-r--r--   0 maurits    (501) staff       (20)     3578 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone/batching/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:34:00.085969 plone.batching-2.0.4/plone.batching.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     9838 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone.batching.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      854 2023-03-14 16:34:00.000000 plone.batching-2.0.4/plone.batching.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone.batching.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone.batching.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone.batching.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone.batching.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       95 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone.batching.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-14 16:33:59.000000 plone.batching-2.0.4/plone.batching.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      869 2023-03-14 16:33:59.000000 plone.batching-2.0.4/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      249 2023-03-14 16:34:00.090058 plone.batching-2.0.4/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1665 2023-03-14 16:33:59.000000 plone.batching-2.0.4/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:04:04.233055 plone.batching-2.0.5/
+-rw-r--r--   0 maurits    (501) staff       (20)     4815 2023-05-22 18:04:03.000000 plone.batching-2.0.5/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-22 18:04:03.000000 plone.batching-2.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      154 2023-05-22 18:04:03.000000 plone.batching-2.0.5/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     9957 2023-05-22 18:04:04.233233 plone.batching-2.0.5/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      274 2023-05-22 18:04:03.000000 plone.batching-2.0.5/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:04:04.226866 plone.batching-2.0.5/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     2179 2023-05-22 18:04:03.000000 plone.batching-2.0.5/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-05-22 18:04:03.000000 plone.batching-2.0.5/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3950 2023-05-22 18:04:03.000000 plone.batching-2.0.5/docs/usage.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      123 2023-05-22 18:04:03.000000 plone.batching-2.0.5/lint-requirements.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:04:04.227111 plone.batching-2.0.5/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 18:04:03.000000 plone.batching-2.0.5/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:04:04.232283 plone.batching-2.0.5/plone/batching/
+-rw-r--r--   0 maurits    (501) staff       (20)      168 2023-05-22 18:04:03.000000 plone.batching-2.0.5/plone/batching/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8368 2023-05-22 18:04:03.000000 plone.batching-2.0.5/plone/batching/batch.py
+-rw-r--r--   0 maurits    (501) staff       (20)      719 2023-05-22 18:04:03.000000 plone.batching-2.0.5/plone/batching/batch_macros.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4936 2023-05-22 18:04:03.000000 plone.batching-2.0.5/plone/batching/batching.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4188 2023-05-22 18:04:03.000000 plone.batching-2.0.5/plone/batching/batchnavigation.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3629 2023-05-22 18:04:03.000000 plone.batching-2.0.5/plone/batching/batchnavigation_bootstrap.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1969 2023-05-22 18:04:03.000000 plone.batching-2.0.5/plone/batching/browser.py
+-rw-r--r--   0 maurits    (501) staff       (20)      586 2023-05-22 18:04:03.000000 plone.batching-2.0.5/plone/batching/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1927 2023-05-22 18:04:03.000000 plone.batching-2.0.5/plone/batching/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:04:04.232762 plone.batching-2.0.5/plone/batching/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 18:04:03.000000 plone.batching-2.0.5/plone/batching/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10824 2023-05-22 18:04:03.000000 plone.batching-2.0.5/plone/batching/tests/test_batching.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3578 2023-05-22 18:04:03.000000 plone.batching-2.0.5/plone/batching/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 18:04:04.229487 plone.batching-2.0.5/plone.batching.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     9957 2023-05-22 18:04:04.000000 plone.batching-2.0.5/plone.batching.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      854 2023-05-22 18:04:04.000000 plone.batching-2.0.5/plone.batching.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 18:04:04.000000 plone.batching-2.0.5/plone.batching.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-05-22 18:04:04.000000 plone.batching-2.0.5/plone.batching.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 18:04:04.000000 plone.batching-2.0.5/plone.batching.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 18:04:04.000000 plone.batching-2.0.5/plone.batching.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       95 2023-05-22 18:04:04.000000 plone.batching-2.0.5/plone.batching.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 18:04:04.000000 plone.batching-2.0.5/plone.batching.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2858 2023-05-22 18:04:03.000000 plone.batching-2.0.5/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      226 2023-05-22 18:04:04.233692 plone.batching-2.0.5/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1665 2023-05-22 18:04:03.000000 plone.batching-2.0.5/setup.py
```

### Comparing `plone.batching-2.0.4/CHANGES.rst` & `plone.batching-2.0.5/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.5 (2023-05-22)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (12f48b08, 50c0e759)
+
+
 2.0.4 (2023-03-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.batching-2.0.4/PKG-INFO` & `plone.batching-2.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.batching
-Version: 2.0.4
+Version: 2.0.5
 Summary: Batching facilities used in Plone.
 Home-page: https://pypi.org/project/plone.batching
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -37,14 +37,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.5 (2023-05-22)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (12f48b08, 50c0e759)
+
+
 2.0.4 (2023-03-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.batching-2.0.4/docs/LICENSE.txt` & `plone.batching-2.0.5/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.batching-2.0.4/docs/usage.rst` & `plone.batching-2.0.5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `plone.batching-2.0.4/plone/batching/batch.py` & `plone.batching-2.0.5/plone/batching/batch.py`

 * *Files identical despite different names*

### Comparing `plone.batching-2.0.4/plone/batching/batch_macros.pt` & `plone.batching-2.0.5/plone/batching/batch_macros.pt`

 * *Files identical despite different names*

### Comparing `plone.batching-2.0.4/plone/batching/batching.rst` & `plone.batching-2.0.5/plone/batching/batching.rst`

 * *Files identical despite different names*

### Comparing `plone.batching-2.0.4/plone/batching/batchnavigation.pt` & `plone.batching-2.0.5/plone/batching/batchnavigation.pt`

 * *Files identical despite different names*

### Comparing `plone.batching-2.0.4/plone/batching/batchnavigation_bootstrap.pt` & `plone.batching-2.0.5/plone/batching/batchnavigation_bootstrap.pt`

 * *Files identical despite different names*

### Comparing `plone.batching-2.0.4/plone/batching/browser.py` & `plone.batching-2.0.5/plone/batching/browser.py`

 * *Files identical despite different names*

### Comparing `plone.batching-2.0.4/plone/batching/configure.zcml` & `plone.batching-2.0.5/plone/batching/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.batching-2.0.4/plone/batching/interfaces.py` & `plone.batching-2.0.5/plone/batching/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.batching-2.0.4/plone/batching/tests/test_batching.py` & `plone.batching-2.0.5/plone/batching/tests/test_batching.py`

 * *Files identical despite different names*

### Comparing `plone.batching-2.0.4/plone/batching/utils.py` & `plone.batching-2.0.5/plone/batching/utils.py`

 * *Files identical despite different names*

### Comparing `plone.batching-2.0.4/plone.batching.egg-info/PKG-INFO` & `plone.batching-2.0.5/plone.batching.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.batching
-Version: 2.0.4
+Version: 2.0.5
 Summary: Batching facilities used in Plone.
 Home-page: https://pypi.org/project/plone.batching
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -37,14 +37,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.5 (2023-05-22)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (12f48b08, 50c0e759)
+
+
 2.0.4 (2023-03-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.batching-2.0.4/plone.batching.egg-info/SOURCES.txt` & `plone.batching-2.0.5/plone.batching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.batching-2.0.4/setup.py` & `plone.batching-2.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.0.4"
+version = "2.0.5"
 
 setup(
     name="plone.batching",
     version=version,
     description="Batching facilities used in Plone.",
     long_description="\n".join(
         [
```

