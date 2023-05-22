# Comparing `tmp/pysparse-array-1.0.3.tar.gz` & `tmp/pysparse-array-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparse-array-1.0.3.tar", last modified: Sun May 21 09:35:58 2023, max compression
+gzip compressed data, was "pysparse-array-1.0.4.tar", last modified: Mon May 22 10:24:59 2023, max compression
```

## Comparing `pysparse-array-1.0.3.tar` & `pysparse-array-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-21 09:35:58.849029 pysparse-array-1.0.3/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     2860 2023-05-21 09:35:11.000000 pysparse-array-1.0.3/HISTORY.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-1.0.3/LICENSE.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-1.0.3/MANIFEST.in
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-21 09:35:58.845931 pysparse-array-1.0.3/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)     4694 2023-05-20 21:17:03.000000 pysparse-array-1.0.3/README.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)      763 2023-05-21 09:35:18.000000 pysparse-array-1.0.3/pyproject.toml
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-21 09:35:58.799236 pysparse-array-1.0.3/pysparse_array.egg-info/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-21 09:35:58.000000 pysparse-array-1.0.3/pysparse_array.egg-info/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-21 09:35:58.000000 pysparse-array-1.0.3/pysparse_array.egg-info/SOURCES.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-21 09:35:58.000000 pysparse-array-1.0.3/pysparse_array.egg-info/dependency_links.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       34 2023-05-21 09:35:58.000000 pysparse-array-1.0.3/pysparse_array.egg-info/requires.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-21 09:35:58.000000 pysparse-array-1.0.3/pysparse_array.egg-info/top_level.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-21 09:35:58.849331 pysparse-array-1.0.3/setup.cfg
--rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-21 09:35:24.000000 pysparse-array-1.0.3/setup.py
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-21 09:35:58.823658 pysparse-array-1.0.3/sparse/
--rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-1.0.3/sparse/__init__.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     8750 2023-05-21 08:43:09.000000 pysparse-array-1.0.3/sparse/array_api.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     7483 2023-05-21 09:30:56.000000 pysparse-array-1.0.3/sparse/core.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-22 10:24:59.722361 pysparse-array-1.0.4/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     2910 2023-05-22 10:24:01.000000 pysparse-array-1.0.4/HISTORY.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-1.0.4/LICENSE.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-1.0.4/MANIFEST.in
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-22 10:24:59.697316 pysparse-array-1.0.4/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     4694 2023-05-20 21:17:03.000000 pysparse-array-1.0.4/README.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      763 2023-05-22 10:24:09.000000 pysparse-array-1.0.4/pyproject.toml
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-22 10:24:59.591321 pysparse-array-1.0.4/pysparse_array.egg-info/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-22 10:24:59.000000 pysparse-array-1.0.4/pysparse_array.egg-info/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-22 10:24:59.000000 pysparse-array-1.0.4/pysparse_array.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-22 10:24:59.000000 pysparse-array-1.0.4/pysparse_array.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       34 2023-05-22 10:24:59.000000 pysparse-array-1.0.4/pysparse_array.egg-info/requires.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-22 10:24:59.000000 pysparse-array-1.0.4/pysparse_array.egg-info/top_level.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-22 10:24:59.723110 pysparse-array-1.0.4/setup.cfg
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-22 10:24:14.000000 pysparse-array-1.0.4/setup.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-22 10:24:59.693788 pysparse-array-1.0.4/sparse/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-1.0.4/sparse/__init__.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     8845 2023-05-22 10:23:21.000000 pysparse-array-1.0.4/sparse/array_api.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     7483 2023-05-21 09:30:56.000000 pysparse-array-1.0.4/sparse/core.py
```

### Comparing `pysparse-array-1.0.3/HISTORY.md` & `pysparse-array-1.0.4/HISTORY.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 #Changelog
 
 All notable changes to the `PySparse` package will be documented in this file.
 
 ## [Unreleased]
 
+## [1.0.4]
+
+### Fixed
+- Fixed multi-indexing bug
+
 ## [1.0.3]
 
 ### Fixed
 - Fixed further bug around multi-index slicing, and in doing so, tidied up some unnecessary Class code
 - Fixed bug whereby the first value was being lost when converting to_sparse
 - Fixed bug whereby certain values were being lost in to_sparse due to a dictionary error
```

### Comparing `pysparse-array-1.0.3/LICENSE.txt` & `pysparse-array-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.3/PKG-INFO` & `pysparse-array-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-1.0.3/README.md` & `pysparse-array-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.3/pyproject.toml` & `pysparse-array-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pysparse-array"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
 	{ name="Thomas Frost", email="tdgfrost@gmail.com" },
 ]
 description = "A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries."
 readme = "README.md"
 requires-python = ">=3.8.0"
 classifiers = [
```

### Comparing `pysparse-array-1.0.3/pysparse_array.egg-info/PKG-INFO` & `pysparse-array-1.0.4/pysparse_array.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-1.0.3/setup.py` & `pysparse-array-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='pysparse-array',
-    version='1.0.3',
+    version='1.0.4',
     description='Package to encode and decode large OOM numpy arrays as Sparse binaries',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     packages=find_packages(),
     author='Thomas Frost',
     author_email='tdgfrost@gmail.com',
     url='https://github.com/tdgfrost/PySparse',
```

### Comparing `pysparse-array-1.0.3/sparse/array_api.py` & `pysparse-array-1.0.4/sparse/array_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,18 @@
         elif isinstance(items, tuple):
             for idx, item in enumerate(items):
                 if not isinstance(item, (int, slice, np.ndarray, type(Ellipsis), type(None))):
                     raise TypeError(
                         'indices must be integers, slices, np.ndarray, Ellipsis, or NoneType - not {}'.format(
                             type(item)))
 
-            return self.__getitem__(items[0])[items[1:]]
+            new_items = list(items)
+            new_items[0] = slice(None, None, None)
+
+            return self.__getitem__(items[0])[tuple(new_items)]
 
         else:
             raise TypeError(
                 'indices must be integers, slices, np.ndarray, Ellipsis, or NoneType - not {}'.format(type(items)))
 
     def __get_row(self, row_idx) -> np.ndarray:
         """
```

### Comparing `pysparse-array-1.0.3/sparse/core.py` & `pysparse-array-1.0.4/sparse/core.py`

 * *Files identical despite different names*

