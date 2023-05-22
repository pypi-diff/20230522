# Comparing `tmp/neutrosopy-0.0.5.tar.gz` & `tmp/neutrosopy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutrosopy-0.0.5.tar", last modified: Mon May 22 03:17:25 2023, max compression
+gzip compressed data, was "neutrosopy-0.0.6.tar", last modified: Mon May 22 03:22:34 2023, max compression
```

## Comparing `neutrosopy-0.0.5.tar` & `neutrosopy-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:17:25.581791 neutrosopy-0.0.5/
--rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-22 02:18:04.000000 neutrosopy-0.0.5/LICENSE
--rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-22 03:17:25.581791 neutrosopy-0.0.5/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)       67 2023-05-22 02:18:04.000000 neutrosopy-0.0.5/README.md
--rw-rw-r--   0 galen     (1000) galen     (1000)      638 2023-05-22 03:16:52.000000 neutrosopy-0.0.5/pyproject.toml
--rw-rw-r--   0 galen     (1000) galen     (1000)       38 2023-05-22 03:17:25.581791 neutrosopy-0.0.5/setup.cfg
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:17:25.577791 neutrosopy-0.0.5/src/
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:17:25.581791 neutrosopy-0.0.5/src/neutrosopy/
--rw-rw-r--   0 galen     (1000) galen     (1000)       28 2023-05-22 03:16:26.000000 neutrosopy-0.0.5/src/neutrosopy/__init__.py
--rw-rw-r--   0 galen     (1000) galen     (1000)    15188 2023-05-22 02:53:44.000000 neutrosopy-0.0.5/src/neutrosopy/neutrosophic.py
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:17:25.581791 neutrosopy-0.0.5/src/neutrosopy.egg-info/
--rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-22 03:17:25.000000 neutrosopy-0.0.5/src/neutrosopy.egg-info/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)      276 2023-05-22 03:17:25.000000 neutrosopy-0.0.5/src/neutrosopy.egg-info/SOURCES.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-22 03:17:25.000000 neutrosopy-0.0.5/src/neutrosopy.egg-info/dependency_links.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)       11 2023-05-22 03:17:25.000000 neutrosopy-0.0.5/src/neutrosopy.egg-info/top_level.txt
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:17:25.581791 neutrosopy-0.0.5/tests/
--rw-rw-r--   0 galen     (1000) galen     (1000)     1589 2023-05-22 02:29:06.000000 neutrosopy-0.0.5/tests/test_neutrosophic_number.py
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:22:34.608807 neutrosopy-0.0.6/
+-rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-22 02:18:04.000000 neutrosopy-0.0.6/LICENSE
+-rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-22 03:22:34.608807 neutrosopy-0.0.6/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)       67 2023-05-22 02:18:04.000000 neutrosopy-0.0.6/README.md
+-rw-rw-r--   0 galen     (1000) galen     (1000)      638 2023-05-22 03:21:47.000000 neutrosopy-0.0.6/pyproject.toml
+-rw-rw-r--   0 galen     (1000) galen     (1000)       38 2023-05-22 03:22:34.608807 neutrosopy-0.0.6/setup.cfg
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:22:34.604807 neutrosopy-0.0.6/src/
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:22:34.604807 neutrosopy-0.0.6/src/neutrosopy/
+-rw-rw-r--   0 galen     (1000) galen     (1000)       28 2023-05-22 03:16:26.000000 neutrosopy-0.0.6/src/neutrosopy/__init__.py
+-rw-rw-r--   0 galen     (1000) galen     (1000)    15188 2023-05-22 02:53:44.000000 neutrosopy-0.0.6/src/neutrosopy/neutrosophic.py
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:22:34.604807 neutrosopy-0.0.6/src/neutrosopy.egg-info/
+-rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-22 03:22:34.000000 neutrosopy-0.0.6/src/neutrosopy.egg-info/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)      276 2023-05-22 03:22:34.000000 neutrosopy-0.0.6/src/neutrosopy.egg-info/SOURCES.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-22 03:22:34.000000 neutrosopy-0.0.6/src/neutrosopy.egg-info/dependency_links.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)       11 2023-05-22 03:22:34.000000 neutrosopy-0.0.6/src/neutrosopy.egg-info/top_level.txt
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:22:34.604807 neutrosopy-0.0.6/tests/
+-rw-rw-r--   0 galen     (1000) galen     (1000)     1589 2023-05-22 02:29:06.000000 neutrosopy-0.0.6/tests/test_neutrosophic_number.py
```

### Comparing `neutrosopy-0.0.5/LICENSE` & `neutrosopy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neutrosopy-0.0.5/PKG-INFO` & `neutrosopy-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutrosopy
-Version: 0.0.5
+Version: 0.0.6
 Summary: Class and utility functions for working with algebraic neutrosophic numbers.
 Author-email: Galen Seilis <galen.seilis@seilis.ca>
 Project-URL: Homepage, https://github.com/galenseilis/neutrosopy
 Project-URL: Bug Tracker, https://github.com/galenseilis/neutrosopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neutrosopy-0.0.5/pyproject.toml` & `neutrosopy-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neutrosopy"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Galen Seilis", email="galen.seilis@seilis.ca" },
 ]
 description = "Class and utility functions for working with algebraic neutrosophic numbers."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `neutrosopy-0.0.5/src/neutrosopy/neutrosophic.py` & `neutrosopy-0.0.6/src/neutrosopy/neutrosophic.py`

 * *Files identical despite different names*

### Comparing `neutrosopy-0.0.5/src/neutrosopy.egg-info/PKG-INFO` & `neutrosopy-0.0.6/src/neutrosopy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutrosopy
-Version: 0.0.5
+Version: 0.0.6
 Summary: Class and utility functions for working with algebraic neutrosophic numbers.
 Author-email: Galen Seilis <galen.seilis@seilis.ca>
 Project-URL: Homepage, https://github.com/galenseilis/neutrosopy
 Project-URL: Bug Tracker, https://github.com/galenseilis/neutrosopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neutrosopy-0.0.5/tests/test_neutrosophic_number.py` & `neutrosopy-0.0.6/tests/test_neutrosophic_number.py`

 * *Files identical despite different names*

