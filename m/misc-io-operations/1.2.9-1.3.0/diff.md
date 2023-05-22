# Comparing `tmp/misc_io_operations-1.2.9.tar.gz` & `tmp/misc_io_operations-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misc_io_operations-1.2.9.tar", last modified: Mon May 22 03:04:03 2023, max compression
+gzip compressed data, was "misc_io_operations-1.3.0.tar", last modified: Mon May 22 03:05:01 2023, max compression
```

## Comparing `misc_io_operations-1.2.9.tar` & `misc_io_operations-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 03:04:03.499469 misc_io_operations-1.2.9/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1188 2023-05-22 03:04:03.499469 misc_io_operations-1.2.9/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      313 2023-05-22 03:03:15.000000 misc_io_operations-1.2.9/README.md
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 03:04:03.499469 misc_io_operations-1.2.9/miops/
--rw-r--r--   0 codsp     (1000) codsp     (1000)       88 2023-05-22 02:23:07.000000 misc_io_operations-1.2.9/miops/__init__.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      452 2023-05-22 02:22:33.000000 misc_io_operations-1.2.9/miops/file_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      182 2023-05-22 02:22:23.000000 misc_io_operations-1.2.9/miops/io_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      309 2023-05-22 02:21:31.000000 misc_io_operations-1.2.9/miops/rand_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      246 2023-05-22 02:22:14.000000 misc_io_operations-1.2.9/miops/url_ops.py
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 03:04:03.499469 misc_io_operations-1.2.9/misc_io_operations.egg-info/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1188 2023-05-22 03:04:03.000000 misc_io_operations-1.2.9/misc_io_operations.egg-info/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      314 2023-05-22 03:04:03.000000 misc_io_operations-1.2.9/misc_io_operations.egg-info/SOURCES.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 03:04:03.000000 misc_io_operations-1.2.9/misc_io_operations.egg-info/dependency_links.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 03:04:03.000000 misc_io_operations-1.2.9/misc_io_operations.egg-info/requires.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        6 2023-05-22 03:04:03.000000 misc_io_operations-1.2.9/misc_io_operations.egg-info/top_level.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 03:04:03.499469 misc_io_operations-1.2.9/setup.cfg
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1065 2023-05-22 03:03:54.000000 misc_io_operations-1.2.9/setup.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 03:05:01.289760 misc_io_operations-1.3.0/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1194 2023-05-22 03:05:01.289760 misc_io_operations-1.3.0/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      319 2023-05-22 03:04:42.000000 misc_io_operations-1.3.0/README.md
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 03:05:01.289760 misc_io_operations-1.3.0/miops/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       88 2023-05-22 02:23:07.000000 misc_io_operations-1.3.0/miops/__init__.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      452 2023-05-22 02:22:33.000000 misc_io_operations-1.3.0/miops/file_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      182 2023-05-22 02:22:23.000000 misc_io_operations-1.3.0/miops/io_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      309 2023-05-22 02:21:31.000000 misc_io_operations-1.3.0/miops/rand_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      246 2023-05-22 02:22:14.000000 misc_io_operations-1.3.0/miops/url_ops.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 03:05:01.289760 misc_io_operations-1.3.0/misc_io_operations.egg-info/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1194 2023-05-22 03:05:01.000000 misc_io_operations-1.3.0/misc_io_operations.egg-info/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      314 2023-05-22 03:05:01.000000 misc_io_operations-1.3.0/misc_io_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 03:05:01.000000 misc_io_operations-1.3.0/misc_io_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 03:05:01.000000 misc_io_operations-1.3.0/misc_io_operations.egg-info/requires.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        6 2023-05-22 03:05:01.000000 misc_io_operations-1.3.0/misc_io_operations.egg-info/top_level.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 03:05:01.289760 misc_io_operations-1.3.0/setup.cfg
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1065 2023-05-22 03:04:45.000000 misc_io_operations-1.3.0/setup.py
```

### Comparing `misc_io_operations-1.2.9/PKG-INFO` & `misc_io_operations-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misc_io_operations
-Version: 1.2.9
+Version: 1.3.0
 Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: MIT
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
@@ -30,10 +30,10 @@
 
 ## Documentation
 
 The import statment:
 
 ```>>> import miops as mps```
 
-c (in function name) - Console-Based Input/Output Operations
+```c``` (in function name) - Console-Based Input/Output Operations
```

### Comparing `misc_io_operations-1.2.9/misc_io_operations.egg-info/PKG-INFO` & `misc_io_operations-1.3.0/misc_io_operations.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misc-io-operations
-Version: 1.2.9
+Version: 1.3.0
 Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: MIT
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
@@ -30,10 +30,10 @@
 
 ## Documentation
 
 The import statment:
 
 ```>>> import miops as mps```
 
-c (in function name) - Console-Based Input/Output Operations
+```c``` (in function name) - Console-Based Input/Output Operations
```

### Comparing `misc_io_operations-1.2.9/setup.py` & `misc_io_operations-1.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 setup(
     name='misc_io_operations',
     packages=['miops'],
-    version="1.2.9",
+    version="1.3.0",
     license="MIT",
     description="Simplification of daily input/output operations",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="GamerXZEN",
     author_email="codspecialops@gmail.com",
     url="https://github.com/GamerXZEN/misc_io_operations",
```

