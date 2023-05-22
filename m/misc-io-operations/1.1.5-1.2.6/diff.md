# Comparing `tmp/misc_io_operations-1.1.5.tar.gz` & `tmp/misc_io_operations-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misc_io_operations-1.1.5.tar", last modified: Mon May 22 02:33:01 2023, max compression
+gzip compressed data, was "misc_io_operations-1.2.6.tar", last modified: Mon May 22 02:38:49 2023, max compression
```

## Comparing `misc_io_operations-1.1.5.tar` & `misc_io_operations-1.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:33:01.808827 misc_io_operations-1.1.5/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1139 2023-05-22 02:33:01.808827 misc_io_operations-1.1.5/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      260 2023-05-22 02:09:13.000000 misc_io_operations-1.1.5/README.md
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:33:01.808827 misc_io_operations-1.1.5/miops/
--rw-r--r--   0 codsp     (1000) codsp     (1000)       88 2023-05-22 02:23:07.000000 misc_io_operations-1.1.5/miops/__init__.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      452 2023-05-22 02:22:33.000000 misc_io_operations-1.1.5/miops/file_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      182 2023-05-22 02:22:23.000000 misc_io_operations-1.1.5/miops/io_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      309 2023-05-22 02:21:31.000000 misc_io_operations-1.1.5/miops/rand_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      246 2023-05-22 02:22:14.000000 misc_io_operations-1.1.5/miops/url_ops.py
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:33:01.808827 misc_io_operations-1.1.5/misc_io_operations.egg-info/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1139 2023-05-22 02:33:01.000000 misc_io_operations-1.1.5/misc_io_operations.egg-info/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      314 2023-05-22 02:33:01.000000 misc_io_operations-1.1.5/misc_io_operations.egg-info/SOURCES.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 02:33:01.000000 misc_io_operations-1.1.5/misc_io_operations.egg-info/dependency_links.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 02:33:01.000000 misc_io_operations-1.1.5/misc_io_operations.egg-info/requires.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        6 2023-05-22 02:33:01.000000 misc_io_operations-1.1.5/misc_io_operations.egg-info/top_level.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 02:33:01.808827 misc_io_operations-1.1.5/setup.cfg
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1066 2023-05-22 02:32:36.000000 misc_io_operations-1.1.5/setup.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:38:49.721020 misc_io_operations-1.2.6/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1139 2023-05-22 02:38:49.721020 misc_io_operations-1.2.6/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      260 2023-05-22 02:09:13.000000 misc_io_operations-1.2.6/README.md
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:38:49.721020 misc_io_operations-1.2.6/miops/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       88 2023-05-22 02:23:07.000000 misc_io_operations-1.2.6/miops/__init__.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      452 2023-05-22 02:22:33.000000 misc_io_operations-1.2.6/miops/file_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      182 2023-05-22 02:22:23.000000 misc_io_operations-1.2.6/miops/io_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      309 2023-05-22 02:21:31.000000 misc_io_operations-1.2.6/miops/rand_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      246 2023-05-22 02:22:14.000000 misc_io_operations-1.2.6/miops/url_ops.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:38:49.721020 misc_io_operations-1.2.6/misc_io_operations.egg-info/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1139 2023-05-22 02:38:49.000000 misc_io_operations-1.2.6/misc_io_operations.egg-info/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      314 2023-05-22 02:38:49.000000 misc_io_operations-1.2.6/misc_io_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 02:38:49.000000 misc_io_operations-1.2.6/misc_io_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 02:38:49.000000 misc_io_operations-1.2.6/misc_io_operations.egg-info/requires.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        6 2023-05-22 02:38:49.000000 misc_io_operations-1.2.6/misc_io_operations.egg-info/top_level.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 02:38:49.721020 misc_io_operations-1.2.6/setup.cfg
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1066 2023-05-22 02:38:38.000000 misc_io_operations-1.2.6/setup.py
```

### Comparing `misc_io_operations-1.1.5/PKG-INFO` & `misc_io_operations-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misc_io_operations
-Version: 1.1.5
+Version: 1.2.6
 Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: UNKNOWN
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
```

### Comparing `misc_io_operations-1.1.5/misc_io_operations.egg-info/PKG-INFO` & `misc_io_operations-1.2.6/misc_io_operations.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misc-io-operations
-Version: 1.1.5
+Version: 1.2.6
 Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: UNKNOWN
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
```

### Comparing `misc_io_operations-1.1.5/setup.py` & `misc_io_operations-1.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 setup(
     name='misc_io_operations',
     packages=['miops'],
-    version="1.1.5",
+    version="1.2.6",
     liscense="MIT",
     description="Simplification of daily input/output operations",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="GamerXZEN",
     author_email="codspecialops@gmail.com",
     url="https://github.com/GamerXZEN/misc_io_operations",
```

