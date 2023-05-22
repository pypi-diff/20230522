# Comparing `tmp/TuXingKeJi-0.0.1.tar.gz` & `tmp/TuXingKeJi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Wenli\Desktop\TuXingKeJi_SDK\dist\.tmp-zh8oyz31\TuXingKeJi-0.0.1.tar", last modified: Mon May 22 20:55:18 2023, max compression
+gzip compressed data, was "C:\Users\Wenli\Desktop\TuXingKeJi_SDK\dist\.tmp-i0lxy5rh\TuXingKeJi-0.0.2.tar", last modified: Mon May 22 21:07:13 2023, max compression
```

## Comparing `TuXingKeJi-0.0.1.tar` & `TuXingKeJi-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 20:55:18.980528 TuXingKeJi-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-05-21 18:28:11.000000 TuXingKeJi-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      884 2023-05-22 20:55:18.978529 TuXingKeJi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       71 2023-05-21 18:17:49.000000 TuXingKeJi-0.0.1/README.md
--rw-rw-rw-   0        0        0      951 2023-05-22 20:54:47.000000 TuXingKeJi-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-22 20:55:18.980528 TuXingKeJi-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-22 20:55:18.906527 TuXingKeJi-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 20:55:18.935527 TuXingKeJi-0.0.1/src/TuXingKeJi/
--rw-rw-rw-   0        0        0    12514 2023-05-22 20:54:47.000000 TuXingKeJi-0.0.1/src/TuXingKeJi/TuXingSDK.py
--rw-rw-rw-   0        0        0        0 2023-05-21 18:10:34.000000 TuXingKeJi-0.0.1/src/TuXingKeJi/__init__.py
--rw-rw-rw-   0        0        0     2856 2023-05-21 12:47:13.000000 TuXingKeJi-0.0.1/src/TuXingKeJi/enumHelper.py
--rw-rw-rw-   0        0        0     4107 2023-05-22 20:47:29.000000 TuXingKeJi-0.0.1/src/TuXingKeJi/peripheral.py
--rw-rw-rw-   0        0        0     1325 2023-05-20 00:11:39.000000 TuXingKeJi-0.0.1/src/TuXingKeJi/serialHelper.py
-drwxrwxrwx   0        0        0        0 2023-05-22 20:55:18.971520 TuXingKeJi-0.0.1/src/TuXingKeJi.egg-info/
--rw-rw-rw-   0        0        0      884 2023-05-22 20:55:18.000000 TuXingKeJi-0.0.1/src/TuXingKeJi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-05-22 20:55:18.000000 TuXingKeJi-0.0.1/src/TuXingKeJi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 20:55:18.000000 TuXingKeJi-0.0.1/src/TuXingKeJi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-05-22 20:55:18.000000 TuXingKeJi-0.0.1/src/TuXingKeJi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 20:55:18.000000 TuXingKeJi-0.0.1/src/TuXingKeJi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 20:55:18.974528 TuXingKeJi-0.0.1/tests/
--rw-rw-rw-   0        0        0      373 2023-05-22 20:54:47.000000 TuXingKeJi-0.0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-22 21:07:13.549273 TuXingKeJi-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-05-21 18:28:11.000000 TuXingKeJi-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      884 2023-05-22 21:07:13.548274 TuXingKeJi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       71 2023-05-21 18:17:49.000000 TuXingKeJi-0.0.2/README.md
+-rw-rw-rw-   0        0        0      951 2023-05-22 21:06:17.000000 TuXingKeJi-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 21:07:13.550278 TuXingKeJi-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 21:07:13.481280 TuXingKeJi-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 21:07:13.511273 TuXingKeJi-0.0.2/src/TuXingKeJi/
+-rw-rw-rw-   0        0        0    12514 2023-05-22 20:54:47.000000 TuXingKeJi-0.0.2/src/TuXingKeJi/TuXingSDK.py
+-rw-rw-rw-   0        0        0        0 2023-05-21 18:10:34.000000 TuXingKeJi-0.0.2/src/TuXingKeJi/__init__.py
+-rw-rw-rw-   0        0        0     2856 2023-05-21 12:47:13.000000 TuXingKeJi-0.0.2/src/TuXingKeJi/enumHelper.py
+-rw-rw-rw-   0        0        0     4107 2023-05-22 20:47:29.000000 TuXingKeJi-0.0.2/src/TuXingKeJi/peripheral.py
+-rw-rw-rw-   0        0        0     1325 2023-05-20 00:11:39.000000 TuXingKeJi-0.0.2/src/TuXingKeJi/serialHelper.py
+drwxrwxrwx   0        0        0        0 2023-05-22 21:07:13.542276 TuXingKeJi-0.0.2/src/TuXingKeJi.egg-info/
+-rw-rw-rw-   0        0        0      884 2023-05-22 21:07:13.000000 TuXingKeJi-0.0.2/src/TuXingKeJi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-05-22 21:07:13.000000 TuXingKeJi-0.0.2/src/TuXingKeJi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 21:07:13.000000 TuXingKeJi-0.0.2/src/TuXingKeJi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-05-22 21:07:13.000000 TuXingKeJi-0.0.2/src/TuXingKeJi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 21:07:13.000000 TuXingKeJi-0.0.2/src/TuXingKeJi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 21:07:13.545271 TuXingKeJi-0.0.2/tests/
+-rw-rw-rw-   0        0        0      373 2023-05-22 20:54:47.000000 TuXingKeJi-0.0.2/tests/test.py
```

### Comparing `TuXingKeJi-0.0.1/LICENSE` & `TuXingKeJi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.1/PKG-INFO` & `TuXingKeJi-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuXingKeJi
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package for TuXingKeJi UAV control
 Author-email: chenghao <chenghao.wang@uphf.fr>
 Project-URL: Homepage, https://github.com/martinWANG2014/TuXingKeJi_SDK
 Project-URL: Bug Tracker, https://github.com/martinWANG2014/TuXingKeJi_SDK/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `TuXingKeJi-0.0.1/pyproject.toml` & `TuXingKeJi-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "TuXingKeJi"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="chenghao", email="chenghao.wang@uphf.fr" },
 ]
 description = "A python package for TuXingKeJi UAV control"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `TuXingKeJi-0.0.1/src/TuXingKeJi/TuXingSDK.py` & `TuXingKeJi-0.0.2/src/TuXingKeJi/TuXingSDK.py`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.1/src/TuXingKeJi/enumHelper.py` & `TuXingKeJi-0.0.2/src/TuXingKeJi/enumHelper.py`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.1/src/TuXingKeJi/peripheral.py` & `TuXingKeJi-0.0.2/src/TuXingKeJi/peripheral.py`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.1/src/TuXingKeJi/serialHelper.py` & `TuXingKeJi-0.0.2/src/TuXingKeJi/serialHelper.py`

 * *Files identical despite different names*

### Comparing `TuXingKeJi-0.0.1/src/TuXingKeJi.egg-info/PKG-INFO` & `TuXingKeJi-0.0.2/src/TuXingKeJi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuXingKeJi
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package for TuXingKeJi UAV control
 Author-email: chenghao <chenghao.wang@uphf.fr>
 Project-URL: Homepage, https://github.com/martinWANG2014/TuXingKeJi_SDK
 Project-URL: Bug Tracker, https://github.com/martinWANG2014/TuXingKeJi_SDK/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

