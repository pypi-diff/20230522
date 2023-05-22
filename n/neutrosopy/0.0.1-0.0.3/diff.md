# Comparing `tmp/neutrosopy-0.0.1.tar.gz` & `tmp/neutrosopy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutrosopy-0.0.1.tar", last modified: Mon May 22 02:23:42 2023, max compression
+gzip compressed data, was "neutrosopy-0.0.3.tar", last modified: Mon May 22 02:38:04 2023, max compression
```

## Comparing `neutrosopy-0.0.1.tar` & `neutrosopy-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 02:23:42.175332 neutrosopy-0.0.1/
--rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-22 02:18:04.000000 neutrosopy-0.0.1/LICENSE
--rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-22 02:23:42.175332 neutrosopy-0.0.1/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)       67 2023-05-22 02:18:04.000000 neutrosopy-0.0.1/README.md
--rw-rw-r--   0 galen     (1000) galen     (1000)      638 2023-05-22 02:23:11.000000 neutrosopy-0.0.1/pyproject.toml
--rw-rw-r--   0 galen     (1000) galen     (1000)       38 2023-05-22 02:23:42.175332 neutrosopy-0.0.1/setup.cfg
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 02:23:42.171332 neutrosopy-0.0.1/src/
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 02:23:42.171332 neutrosopy-0.0.1/src/neutrosopy/
--rw-rw-r--   0 galen     (1000) galen     (1000)        0 2023-05-22 02:21:31.000000 neutrosopy-0.0.1/src/neutrosopy/__init__.py
--rw-rw-r--   0 galen     (1000) galen     (1000)     6035 2023-05-22 02:18:04.000000 neutrosopy-0.0.1/src/neutrosopy/neutrosophic.py
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 02:23:42.175332 neutrosopy-0.0.1/src/neutrosopy.egg-info/
--rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-22 02:23:42.000000 neutrosopy-0.0.1/src/neutrosopy.egg-info/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)      242 2023-05-22 02:23:42.000000 neutrosopy-0.0.1/src/neutrosopy.egg-info/SOURCES.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-22 02:23:42.000000 neutrosopy-0.0.1/src/neutrosopy.egg-info/dependency_links.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)       11 2023-05-22 02:23:42.000000 neutrosopy-0.0.1/src/neutrosopy.egg-info/top_level.txt
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 02:38:04.011453 neutrosopy-0.0.3/
+-rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-22 02:18:04.000000 neutrosopy-0.0.3/LICENSE
+-rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-22 02:38:04.011453 neutrosopy-0.0.3/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)       67 2023-05-22 02:18:04.000000 neutrosopy-0.0.3/README.md
+-rw-rw-r--   0 galen     (1000) galen     (1000)      638 2023-05-22 02:37:36.000000 neutrosopy-0.0.3/pyproject.toml
+-rw-rw-r--   0 galen     (1000) galen     (1000)       38 2023-05-22 02:38:04.011453 neutrosopy-0.0.3/setup.cfg
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 02:38:04.007453 neutrosopy-0.0.3/src/
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 02:38:04.007453 neutrosopy-0.0.3/src/neutrosopy/
+-rw-rw-r--   0 galen     (1000) galen     (1000)       27 2023-05-22 02:28:34.000000 neutrosopy-0.0.3/src/neutrosopy/__init__.py
+-rw-rw-r--   0 galen     (1000) galen     (1000)     6035 2023-05-22 02:18:04.000000 neutrosopy-0.0.3/src/neutrosopy/neutrosophic.py
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 02:38:04.011453 neutrosopy-0.0.3/src/neutrosopy.egg-info/
+-rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-22 02:38:03.000000 neutrosopy-0.0.3/src/neutrosopy.egg-info/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)      276 2023-05-22 02:38:04.000000 neutrosopy-0.0.3/src/neutrosopy.egg-info/SOURCES.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-22 02:38:03.000000 neutrosopy-0.0.3/src/neutrosopy.egg-info/dependency_links.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)       11 2023-05-22 02:38:03.000000 neutrosopy-0.0.3/src/neutrosopy.egg-info/top_level.txt
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 02:38:04.011453 neutrosopy-0.0.3/tests/
+-rw-rw-r--   0 galen     (1000) galen     (1000)     1589 2023-05-22 02:29:06.000000 neutrosopy-0.0.3/tests/test_neutrosophic_number.py
```

### Comparing `neutrosopy-0.0.1/LICENSE` & `neutrosopy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neutrosopy-0.0.1/PKG-INFO` & `neutrosopy-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutrosopy
-Version: 0.0.1
+Version: 0.0.3
 Summary: Class and utility functions for working with algebraic neutrosophic numbers.
 Author-email: Galen Seilis <galen.seilis@seilis.ca>
 Project-URL: Homepage, https://github.com/galenseilis/neutrosopy
 Project-URL: Bug Tracker, https://github.com/galenseilis/neutrosopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neutrosopy-0.0.1/pyproject.toml` & `neutrosopy-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neutrosopy"
-version = "0.0.1"
+version = "0.0.3"
 authors = [
   { name="Galen Seilis", email="galen.seilis@seilis.ca" },
 ]
 description = "Class and utility functions for working with algebraic neutrosophic numbers."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `neutrosopy-0.0.1/src/neutrosopy/neutrosophic.py` & `neutrosopy-0.0.3/src/neutrosopy/neutrosophic.py`

 * *Files identical despite different names*

### Comparing `neutrosopy-0.0.1/src/neutrosopy.egg-info/PKG-INFO` & `neutrosopy-0.0.3/src/neutrosopy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutrosopy
-Version: 0.0.1
+Version: 0.0.3
 Summary: Class and utility functions for working with algebraic neutrosophic numbers.
 Author-email: Galen Seilis <galen.seilis@seilis.ca>
 Project-URL: Homepage, https://github.com/galenseilis/neutrosopy
 Project-URL: Bug Tracker, https://github.com/galenseilis/neutrosopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

