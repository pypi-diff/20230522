# Comparing `tmp/pylibrb-0.0.2.tar.gz` & `tmp/pylibrb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibrb-0.0.2.tar", last modified: Mon May 22 10:38:03 2023, max compression
+gzip compressed data, was "pylibrb-0.0.3.tar", last modified: Mon May 22 14:28:52 2023, max compression
```

## Comparing `pylibrb-0.0.2.tar` & `pylibrb-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:38:03.837435 pylibrb-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-05-22 10:37:50.000000 pylibrb-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 10:37:50.000000 pylibrb-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-22 10:38:03.837435 pylibrb-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-22 10:37:50.000000 pylibrb-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 10:37:50.000000 pylibrb-0.0.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-22 10:37:50.000000 pylibrb-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-22 10:38:03.837435 pylibrb-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-22 10:37:50.000000 pylibrb-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:38:03.833435 pylibrb-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:38:03.833435 pylibrb-0.0.2/src/pylibrb/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-22 10:37:50.000000 pylibrb-0.0.2/src/pylibrb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36255 2023-05-22 10:37:50.000000 pylibrb-0.0.2/src/pylibrb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:37:50.000000 pylibrb-0.0.2/src/pylibrb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:38:03.837435 pylibrb-0.0.2/src/pylibrb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-22 10:38:03.000000 pylibrb-0.0.2/src/pylibrb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-22 10:38:03.000000 pylibrb-0.0.2/src/pylibrb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:38:03.000000 pylibrb-0.0.2/src/pylibrb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 10:38:03.000000 pylibrb-0.0.2/src/pylibrb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 10:38:03.000000 pylibrb-0.0.2/src/pylibrb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:38:03.837435 pylibrb-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-22 10:37:50.000000 pylibrb-0.0.2/tests/test_stretcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:52.854421 pylibrb-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-05-22 14:28:36.000000 pylibrb-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-22 14:28:36.000000 pylibrb-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-22 14:28:52.854421 pylibrb-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-22 14:28:36.000000 pylibrb-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 14:28:36.000000 pylibrb-0.0.3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-22 14:28:36.000000 pylibrb-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-22 14:28:52.854421 pylibrb-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-22 14:28:36.000000 pylibrb-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:52.850421 pylibrb-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:52.854421 pylibrb-0.0.3/src/pylibrb/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-22 14:28:36.000000 pylibrb-0.0.3/src/pylibrb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36255 2023-05-22 14:28:36.000000 pylibrb-0.0.3/src/pylibrb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:36.000000 pylibrb-0.0.3/src/pylibrb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:52.854421 pylibrb-0.0.3/src/pylibrb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-22 14:28:52.000000 pylibrb-0.0.3/src/pylibrb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-22 14:28:52.000000 pylibrb-0.0.3/src/pylibrb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:28:52.000000 pylibrb-0.0.3/src/pylibrb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 14:28:52.000000 pylibrb-0.0.3/src/pylibrb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 14:28:52.000000 pylibrb-0.0.3/src/pylibrb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:52.854421 pylibrb-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-22 14:28:36.000000 pylibrb-0.0.3/tests/test_stretcher.py
```

### Comparing `pylibrb-0.0.2/LICENSE` & `pylibrb-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.2/PKG-INFO` & `pylibrb-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibrb
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python bindings for the RubberBand library
 Home-page: https://github.com/pawel-glomski/pylibrb
 Author: Paweł Głomski
 Author-email: pglomski.dev@gmail.com
 License: 'GPLv2'
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
```

### Comparing `pylibrb-0.0.2/README.md` & `pylibrb-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.2/setup.cfg` & `pylibrb-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.2/src/pylibrb/__init__.pyi` & `pylibrb-0.0.3/src/pylibrb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.2/src/pylibrb.egg-info/PKG-INFO` & `pylibrb-0.0.3/src/pylibrb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibrb
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python bindings for the RubberBand library
 Home-page: https://github.com/pawel-glomski/pylibrb
 Author: Paweł Głomski
 Author-email: pglomski.dev@gmail.com
 License: 'GPLv2'
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
```

### Comparing `pylibrb-0.0.2/tests/test_stretcher.py` & `pylibrb-0.0.3/tests/test_stretcher.py`

 * *Files identical despite different names*

