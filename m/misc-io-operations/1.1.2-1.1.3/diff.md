# Comparing `tmp/misc_io_operations-1.1.2.tar.gz` & `tmp/misc_io_operations-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misc_io_operations-1.1.2.tar", last modified: Mon May 22 02:10:19 2023, max compression
+gzip compressed data, was "misc_io_operations-1.1.3.tar", last modified: Mon May 22 02:24:30 2023, max compression
```

## Comparing `misc_io_operations-1.1.2.tar` & `misc_io_operations-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:10:19.799358 misc_io_operations-1.1.2/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1129 2023-05-22 02:10:19.799358 misc_io_operations-1.1.2/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      260 2023-05-22 02:09:13.000000 misc_io_operations-1.1.2/README.md
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:10:19.799358 misc_io_operations-1.1.2/misc_io_operations/
--rw-r--r--   0 codsp     (1000) codsp     (1000)      187 2023-05-20 04:22:31.000000 misc_io_operations-1.1.2/misc_io_operations/__init__.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1250 2023-05-20 15:45:22.000000 misc_io_operations-1.1.2/misc_io_operations/misc_io_operations.py
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:10:19.799358 misc_io_operations-1.1.2/misc_io_operations.egg-info/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1129 2023-05-22 02:10:19.000000 misc_io_operations-1.1.2/misc_io_operations.egg-info/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      299 2023-05-22 02:10:19.000000 misc_io_operations-1.1.2/misc_io_operations.egg-info/SOURCES.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 02:10:19.000000 misc_io_operations-1.1.2/misc_io_operations.egg-info/dependency_links.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 02:10:19.000000 misc_io_operations-1.1.2/misc_io_operations.egg-info/requires.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)       19 2023-05-22 02:10:19.000000 misc_io_operations-1.1.2/misc_io_operations.egg-info/top_level.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 02:10:19.799358 misc_io_operations-1.1.2/setup.cfg
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1069 2023-05-22 02:09:31.000000 misc_io_operations-1.1.2/setup.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:24:30.085569 misc_io_operations-1.1.3/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1139 2023-05-22 02:24:30.085569 misc_io_operations-1.1.3/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      260 2023-05-22 02:09:13.000000 misc_io_operations-1.1.3/README.md
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:24:30.085569 misc_io_operations-1.1.3/miops/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       88 2023-05-22 02:23:07.000000 misc_io_operations-1.1.3/miops/__init__.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      452 2023-05-22 02:22:33.000000 misc_io_operations-1.1.3/miops/file_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      182 2023-05-22 02:22:23.000000 misc_io_operations-1.1.3/miops/io_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      309 2023-05-22 02:21:31.000000 misc_io_operations-1.1.3/miops/rand_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      246 2023-05-22 02:22:14.000000 misc_io_operations-1.1.3/miops/url_ops.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:24:30.085569 misc_io_operations-1.1.3/misc_io_operations.egg-info/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1139 2023-05-22 02:24:30.000000 misc_io_operations-1.1.3/misc_io_operations.egg-info/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      314 2023-05-22 02:24:30.000000 misc_io_operations-1.1.3/misc_io_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 02:24:30.000000 misc_io_operations-1.1.3/misc_io_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 02:24:30.000000 misc_io_operations-1.1.3/misc_io_operations.egg-info/requires.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        6 2023-05-22 02:24:30.000000 misc_io_operations-1.1.3/misc_io_operations.egg-info/top_level.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 02:24:30.085569 misc_io_operations-1.1.3/setup.cfg
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1066 2023-05-22 02:23:44.000000 misc_io_operations-1.1.3/setup.py
```

### Comparing `misc_io_operations-1.1.2/PKG-INFO` & `misc_io_operations-1.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: misc_io_operations
-Version: 1.1.2
-Summary: Simplification of daily IO operations
+Version: 1.1.3
+Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: UNKNOWN
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `misc_io_operations-1.1.2/misc_io_operations.egg-info/PKG-INFO` & `misc_io_operations-1.1.3/misc_io_operations.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: misc-io-operations
-Version: 1.1.2
-Summary: Simplification of daily IO operations
+Version: 1.1.3
+Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: UNKNOWN
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `misc_io_operations-1.1.2/setup.py` & `misc_io_operations-1.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 setup(
     name='misc_io_operations',
-    packages=['misc_io_operations'],
-    version="1.1.2",
+    packages=['miops'],
+    version="1.1.3",
     liscense="MIT",
-    description="Simplification of daily IO operations",
+    description="Simplification of daily input/output operations",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="GamerXZEN",
     author_email="codspecialops@gmail.com",
     url="https://github.com/GamerXZEN/misc_io_operations",
     keywords=["operations", "input", "output", "input/output", "miscellaneous", "python",],
     install_requires=["requests"],
```

