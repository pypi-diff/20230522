# Comparing `tmp/FyersTesting-0.0.2.tar.gz` & `tmp/FyersTesting-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FyersTesting-0.0.2.tar", last modified: Mon May 22 11:12:08 2023, max compression
+gzip compressed data, was "FyersTesting-0.0.3.tar", last modified: Mon May 22 11:23:45 2023, max compression
```

## Comparing `FyersTesting-0.0.2.tar` & `FyersTesting-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-22 11:12:08.730283 FyersTesting-0.0.2/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-22 11:12:08.730283 FyersTesting-0.0.2/FyersTesting.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      672 2023-05-22 11:12:08.000000 FyersTesting-0.0.2/FyersTesting.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      209 2023-05-22 11:12:08.000000 FyersTesting-0.0.2/FyersTesting.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-05-22 11:12:08.000000 FyersTesting-0.0.2/FyersTesting.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      107 2023-05-22 11:12:08.000000 FyersTesting-0.0.2/FyersTesting.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-05-22 11:12:08.000000 FyersTesting-0.0.2/FyersTesting.egg-info/top_level.txt
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-05-22 10:22:05.000000 FyersTesting-0.0.2/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      672 2023-05-22 11:12:08.730283 FyersTesting-0.0.2/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)      256 2023-05-22 10:22:09.000000 FyersTesting-0.0.2/README.md
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-05-22 11:12:08.730283 FyersTesting-0.0.2/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)      860 2023-05-22 11:11:59.000000 FyersTesting-0.0.2/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-22 11:23:45.417502 FyersTesting-0.0.3/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-22 11:23:45.417502 FyersTesting-0.0.3/FyersTesting.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      672 2023-05-22 11:23:44.000000 FyersTesting-0.0.3/FyersTesting.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      209 2023-05-22 11:23:45.000000 FyersTesting-0.0.3/FyersTesting.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-05-22 11:23:45.000000 FyersTesting-0.0.3/FyersTesting.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      107 2023-05-22 11:23:45.000000 FyersTesting-0.0.3/FyersTesting.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-05-22 11:23:45.000000 FyersTesting-0.0.3/FyersTesting.egg-info/top_level.txt
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-05-22 10:22:05.000000 FyersTesting-0.0.3/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      672 2023-05-22 11:23:45.417502 FyersTesting-0.0.3/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)      256 2023-05-22 10:22:09.000000 FyersTesting-0.0.3/README.md
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-05-22 11:23:45.417502 FyersTesting-0.0.3/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)      860 2023-05-22 11:23:36.000000 FyersTesting-0.0.3/setup.py
```

### Comparing `FyersTesting-0.0.2/FyersTesting.egg-info/PKG-INFO` & `FyersTesting-0.0.3/FyersTesting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FyersTesting
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fyers trading APIs.
 Home-page: https://github.com/
 Author: Fyers-Tech
 Author-email: support@fyers.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FyersTesting-0.0.2/LICENSE.txt` & `FyersTesting-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FyersTesting-0.0.2/PKG-INFO` & `FyersTesting-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FyersTesting
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fyers trading APIs.
 Home-page: https://github.com/
 Author: Fyers-Tech
 Author-email: support@fyers.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FyersTesting-0.0.2/setup.py` & `FyersTesting-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='FyersTesting',  
-     version='0.0.2',
+     version='0.0.3',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/",
      packages=setuptools.find_packages(),
```

