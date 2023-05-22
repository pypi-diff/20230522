# Comparing `tmp/misc_io_operations-1.3.1.tar.gz` & `tmp/misc_io_operations-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misc_io_operations-1.3.1.tar", last modified: Mon May 22 19:42:25 2023, max compression
+gzip compressed data, was "misc_io_operations-1.3.2.tar", last modified: Mon May 22 19:49:33 2023, max compression
```

## Comparing `misc_io_operations-1.3.1.tar` & `misc_io_operations-1.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 19:42:25.569049 misc_io_operations-1.3.1/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1194 2023-05-22 19:42:25.569049 misc_io_operations-1.3.1/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      319 2023-05-22 03:04:42.000000 misc_io_operations-1.3.1/README.md
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 19:42:25.569049 misc_io_operations-1.3.1/misc_io_operations/
--rw-r--r--   0 codsp     (1000) codsp     (1000)       32 2023-05-22 19:41:23.000000 misc_io_operations-1.3.1/misc_io_operations/__init__.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1192 2023-05-22 19:41:04.000000 misc_io_operations-1.3.1/misc_io_operations/misc_io_operations.py
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 19:42:25.569049 misc_io_operations-1.3.1/misc_io_operations.egg-info/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1194 2023-05-22 19:42:25.000000 misc_io_operations-1.3.1/misc_io_operations.egg-info/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      299 2023-05-22 19:42:25.000000 misc_io_operations-1.3.1/misc_io_operations.egg-info/SOURCES.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 19:42:25.000000 misc_io_operations-1.3.1/misc_io_operations.egg-info/dependency_links.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 19:42:25.000000 misc_io_operations-1.3.1/misc_io_operations.egg-info/requires.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)       19 2023-05-22 19:42:25.000000 misc_io_operations-1.3.1/misc_io_operations.egg-info/top_level.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 19:42:25.569049 misc_io_operations-1.3.1/setup.cfg
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1078 2023-05-22 19:42:22.000000 misc_io_operations-1.3.1/setup.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 19:49:33.428920 misc_io_operations-1.3.2/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1194 2023-05-22 19:49:33.428920 misc_io_operations-1.3.2/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      319 2023-05-22 03:04:42.000000 misc_io_operations-1.3.2/README.md
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 19:49:33.428920 misc_io_operations-1.3.2/misc_io_operations/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      133 2023-05-22 19:47:39.000000 misc_io_operations-1.3.2/misc_io_operations/__init__.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1192 2023-05-22 19:41:04.000000 misc_io_operations-1.3.2/misc_io_operations/misc_io_operations.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 19:49:33.428920 misc_io_operations-1.3.2/misc_io_operations.egg-info/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1194 2023-05-22 19:49:33.000000 misc_io_operations-1.3.2/misc_io_operations.egg-info/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      299 2023-05-22 19:49:33.000000 misc_io_operations-1.3.2/misc_io_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 19:49:33.000000 misc_io_operations-1.3.2/misc_io_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 19:49:33.000000 misc_io_operations-1.3.2/misc_io_operations.egg-info/requires.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       19 2023-05-22 19:49:33.000000 misc_io_operations-1.3.2/misc_io_operations.egg-info/top_level.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 19:49:33.428920 misc_io_operations-1.3.2/setup.cfg
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1078 2023-05-22 19:49:09.000000 misc_io_operations-1.3.2/setup.py
```

### Comparing `misc_io_operations-1.3.1/PKG-INFO` & `misc_io_operations-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misc_io_operations
-Version: 1.3.1
+Version: 1.3.2
 Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: MIT
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
```

### Comparing `misc_io_operations-1.3.1/misc_io_operations/misc_io_operations.py` & `misc_io_operations-1.3.2/misc_io_operations/misc_io_operations.py`

 * *Files identical despite different names*

### Comparing `misc_io_operations-1.3.1/misc_io_operations.egg-info/PKG-INFO` & `misc_io_operations-1.3.2/misc_io_operations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misc-io-operations
-Version: 1.3.1
+Version: 1.3.2
 Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: MIT
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
```

### Comparing `misc_io_operations-1.3.1/setup.py` & `misc_io_operations-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 setup(
     name='misc_io_operations',
     packages=['misc_io_operations'],
-    version="1.3.1",
+    version="1.3.2",
     license="MIT",
     description="Simplification of daily input/output operations",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="GamerXZEN",
     author_email="codspecialops@gmail.com",
     url="https://github.com/GamerXZEN/misc_io_operations",
```

