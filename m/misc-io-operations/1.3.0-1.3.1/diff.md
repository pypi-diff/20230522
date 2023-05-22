# Comparing `tmp/misc_io_operations-1.3.0.tar.gz` & `tmp/misc_io_operations-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misc_io_operations-1.3.0.tar", last modified: Mon May 22 03:05:01 2023, max compression
+gzip compressed data, was "misc_io_operations-1.3.1.tar", last modified: Mon May 22 19:42:25 2023, max compression
```

## Comparing `misc_io_operations-1.3.0.tar` & `misc_io_operations-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 03:05:01.289760 misc_io_operations-1.3.0/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1194 2023-05-22 03:05:01.289760 misc_io_operations-1.3.0/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      319 2023-05-22 03:04:42.000000 misc_io_operations-1.3.0/README.md
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 03:05:01.289760 misc_io_operations-1.3.0/miops/
--rw-r--r--   0 codsp     (1000) codsp     (1000)       88 2023-05-22 02:23:07.000000 misc_io_operations-1.3.0/miops/__init__.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      452 2023-05-22 02:22:33.000000 misc_io_operations-1.3.0/miops/file_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      182 2023-05-22 02:22:23.000000 misc_io_operations-1.3.0/miops/io_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      309 2023-05-22 02:21:31.000000 misc_io_operations-1.3.0/miops/rand_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      246 2023-05-22 02:22:14.000000 misc_io_operations-1.3.0/miops/url_ops.py
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 03:05:01.289760 misc_io_operations-1.3.0/misc_io_operations.egg-info/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1194 2023-05-22 03:05:01.000000 misc_io_operations-1.3.0/misc_io_operations.egg-info/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      314 2023-05-22 03:05:01.000000 misc_io_operations-1.3.0/misc_io_operations.egg-info/SOURCES.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 03:05:01.000000 misc_io_operations-1.3.0/misc_io_operations.egg-info/dependency_links.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 03:05:01.000000 misc_io_operations-1.3.0/misc_io_operations.egg-info/requires.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        6 2023-05-22 03:05:01.000000 misc_io_operations-1.3.0/misc_io_operations.egg-info/top_level.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 03:05:01.289760 misc_io_operations-1.3.0/setup.cfg
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1065 2023-05-22 03:04:45.000000 misc_io_operations-1.3.0/setup.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 19:42:25.569049 misc_io_operations-1.3.1/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1194 2023-05-22 19:42:25.569049 misc_io_operations-1.3.1/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      319 2023-05-22 03:04:42.000000 misc_io_operations-1.3.1/README.md
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 19:42:25.569049 misc_io_operations-1.3.1/misc_io_operations/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       32 2023-05-22 19:41:23.000000 misc_io_operations-1.3.1/misc_io_operations/__init__.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1192 2023-05-22 19:41:04.000000 misc_io_operations-1.3.1/misc_io_operations/misc_io_operations.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 19:42:25.569049 misc_io_operations-1.3.1/misc_io_operations.egg-info/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1194 2023-05-22 19:42:25.000000 misc_io_operations-1.3.1/misc_io_operations.egg-info/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      299 2023-05-22 19:42:25.000000 misc_io_operations-1.3.1/misc_io_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 19:42:25.000000 misc_io_operations-1.3.1/misc_io_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 19:42:25.000000 misc_io_operations-1.3.1/misc_io_operations.egg-info/requires.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       19 2023-05-22 19:42:25.000000 misc_io_operations-1.3.1/misc_io_operations.egg-info/top_level.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 19:42:25.569049 misc_io_operations-1.3.1/setup.cfg
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1078 2023-05-22 19:42:22.000000 misc_io_operations-1.3.1/setup.py
```

### Comparing `misc_io_operations-1.3.0/PKG-INFO` & `misc_io_operations-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misc_io_operations
-Version: 1.3.0
+Version: 1.3.1
 Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: MIT
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
```

### Comparing `misc_io_operations-1.3.0/misc_io_operations.egg-info/PKG-INFO` & `misc_io_operations-1.3.1/misc_io_operations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misc-io-operations
-Version: 1.3.0
+Version: 1.3.1
 Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: MIT
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
```

### Comparing `misc_io_operations-1.3.0/setup.py` & `misc_io_operations-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 setup(
     name='misc_io_operations',
-    packages=['miops'],
-    version="1.3.0",
+    packages=['misc_io_operations'],
+    version="1.3.1",
     license="MIT",
     description="Simplification of daily input/output operations",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="GamerXZEN",
     author_email="codspecialops@gmail.com",
     url="https://github.com/GamerXZEN/misc_io_operations",
```

