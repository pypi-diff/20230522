# Comparing `tmp/misc_io_operations-1.2.6.tar.gz` & `tmp/misc_io_operations-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misc_io_operations-1.2.6.tar", last modified: Mon May 22 02:38:49 2023, max compression
+gzip compressed data, was "misc_io_operations-1.2.7.tar", last modified: Mon May 22 02:45:42 2023, max compression
```

## Comparing `misc_io_operations-1.2.6.tar` & `misc_io_operations-1.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:38:49.721020 misc_io_operations-1.2.6/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1139 2023-05-22 02:38:49.721020 misc_io_operations-1.2.6/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      260 2023-05-22 02:09:13.000000 misc_io_operations-1.2.6/README.md
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:38:49.721020 misc_io_operations-1.2.6/miops/
--rw-r--r--   0 codsp     (1000) codsp     (1000)       88 2023-05-22 02:23:07.000000 misc_io_operations-1.2.6/miops/__init__.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      452 2023-05-22 02:22:33.000000 misc_io_operations-1.2.6/miops/file_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      182 2023-05-22 02:22:23.000000 misc_io_operations-1.2.6/miops/io_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      309 2023-05-22 02:21:31.000000 misc_io_operations-1.2.6/miops/rand_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      246 2023-05-22 02:22:14.000000 misc_io_operations-1.2.6/miops/url_ops.py
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:38:49.721020 misc_io_operations-1.2.6/misc_io_operations.egg-info/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1139 2023-05-22 02:38:49.000000 misc_io_operations-1.2.6/misc_io_operations.egg-info/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      314 2023-05-22 02:38:49.000000 misc_io_operations-1.2.6/misc_io_operations.egg-info/SOURCES.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 02:38:49.000000 misc_io_operations-1.2.6/misc_io_operations.egg-info/dependency_links.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 02:38:49.000000 misc_io_operations-1.2.6/misc_io_operations.egg-info/requires.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        6 2023-05-22 02:38:49.000000 misc_io_operations-1.2.6/misc_io_operations.egg-info/top_level.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 02:38:49.721020 misc_io_operations-1.2.6/setup.cfg
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1066 2023-05-22 02:38:38.000000 misc_io_operations-1.2.6/setup.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:45:42.633478 misc_io_operations-1.2.7/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1135 2023-05-22 02:45:42.633478 misc_io_operations-1.2.7/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      260 2023-05-22 02:09:13.000000 misc_io_operations-1.2.7/README.md
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:45:42.633478 misc_io_operations-1.2.7/miops/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       88 2023-05-22 02:23:07.000000 misc_io_operations-1.2.7/miops/__init__.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      452 2023-05-22 02:22:33.000000 misc_io_operations-1.2.7/miops/file_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      182 2023-05-22 02:22:23.000000 misc_io_operations-1.2.7/miops/io_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      309 2023-05-22 02:21:31.000000 misc_io_operations-1.2.7/miops/rand_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      246 2023-05-22 02:22:14.000000 misc_io_operations-1.2.7/miops/url_ops.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:45:42.633478 misc_io_operations-1.2.7/misc_io_operations.egg-info/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1135 2023-05-22 02:45:42.000000 misc_io_operations-1.2.7/misc_io_operations.egg-info/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      314 2023-05-22 02:45:42.000000 misc_io_operations-1.2.7/misc_io_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 02:45:42.000000 misc_io_operations-1.2.7/misc_io_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 02:45:42.000000 misc_io_operations-1.2.7/misc_io_operations.egg-info/requires.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        6 2023-05-22 02:45:42.000000 misc_io_operations-1.2.7/misc_io_operations.egg-info/top_level.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 02:45:42.633478 misc_io_operations-1.2.7/setup.cfg
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1065 2023-05-22 02:45:15.000000 misc_io_operations-1.2.7/setup.py
```

### Comparing `misc_io_operations-1.2.6/PKG-INFO` & `misc_io_operations-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: misc_io_operations
-Version: 1.2.6
+Version: 1.2.7
 Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
-License: UNKNOWN
+License: MIT
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `misc_io_operations-1.2.6/misc_io_operations.egg-info/PKG-INFO` & `misc_io_operations-1.2.7/misc_io_operations.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: misc-io-operations
-Version: 1.2.6
+Version: 1.2.7
 Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
-License: UNKNOWN
+License: MIT
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `misc_io_operations-1.2.6/setup.py` & `misc_io_operations-1.2.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 setup(
     name='misc_io_operations',
     packages=['miops'],
-    version="1.2.6",
-    liscense="MIT",
+    version="1.2.7",
+    license="MIT",
     description="Simplification of daily input/output operations",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="GamerXZEN",
     author_email="codspecialops@gmail.com",
     url="https://github.com/GamerXZEN/misc_io_operations",
     keywords=["operations", "input", "output", "input/output", "miscellaneous", "python",],
```

