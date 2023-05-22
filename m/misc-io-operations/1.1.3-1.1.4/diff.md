# Comparing `tmp/misc_io_operations-1.1.3.tar.gz` & `tmp/misc_io_operations-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misc_io_operations-1.1.3.tar", last modified: Mon May 22 02:24:30 2023, max compression
+gzip compressed data, was "misc_io_operations-1.1.4.tar", last modified: Mon May 22 02:26:50 2023, max compression
```

## Comparing `misc_io_operations-1.1.3.tar` & `misc_io_operations-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:24:30.085569 misc_io_operations-1.1.3/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1139 2023-05-22 02:24:30.085569 misc_io_operations-1.1.3/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      260 2023-05-22 02:09:13.000000 misc_io_operations-1.1.3/README.md
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:24:30.085569 misc_io_operations-1.1.3/miops/
--rw-r--r--   0 codsp     (1000) codsp     (1000)       88 2023-05-22 02:23:07.000000 misc_io_operations-1.1.3/miops/__init__.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      452 2023-05-22 02:22:33.000000 misc_io_operations-1.1.3/miops/file_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      182 2023-05-22 02:22:23.000000 misc_io_operations-1.1.3/miops/io_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      309 2023-05-22 02:21:31.000000 misc_io_operations-1.1.3/miops/rand_ops.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)      246 2023-05-22 02:22:14.000000 misc_io_operations-1.1.3/miops/url_ops.py
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:24:30.085569 misc_io_operations-1.1.3/misc_io_operations.egg-info/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1139 2023-05-22 02:24:30.000000 misc_io_operations-1.1.3/misc_io_operations.egg-info/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      314 2023-05-22 02:24:30.000000 misc_io_operations-1.1.3/misc_io_operations.egg-info/SOURCES.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 02:24:30.000000 misc_io_operations-1.1.3/misc_io_operations.egg-info/dependency_links.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 02:24:30.000000 misc_io_operations-1.1.3/misc_io_operations.egg-info/requires.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        6 2023-05-22 02:24:30.000000 misc_io_operations-1.1.3/misc_io_operations.egg-info/top_level.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 02:24:30.085569 misc_io_operations-1.1.3/setup.cfg
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1066 2023-05-22 02:23:44.000000 misc_io_operations-1.1.3/setup.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:26:50.766478 misc_io_operations-1.1.4/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1185 2023-05-22 02:26:50.766478 misc_io_operations-1.1.4/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      260 2023-05-22 02:09:13.000000 misc_io_operations-1.1.4/README.md
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:26:50.766478 misc_io_operations-1.1.4/miops/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       88 2023-05-22 02:23:07.000000 misc_io_operations-1.1.4/miops/__init__.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      452 2023-05-22 02:22:33.000000 misc_io_operations-1.1.4/miops/file_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      182 2023-05-22 02:22:23.000000 misc_io_operations-1.1.4/miops/io_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      309 2023-05-22 02:21:31.000000 misc_io_operations-1.1.4/miops/rand_ops.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      246 2023-05-22 02:22:14.000000 misc_io_operations-1.1.4/miops/url_ops.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:26:50.766478 misc_io_operations-1.1.4/misc_io_operations.egg-info/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1185 2023-05-22 02:26:50.000000 misc_io_operations-1.1.4/misc_io_operations.egg-info/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      314 2023-05-22 02:26:50.000000 misc_io_operations-1.1.4/misc_io_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 02:26:50.000000 misc_io_operations-1.1.4/misc_io_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 02:26:50.000000 misc_io_operations-1.1.4/misc_io_operations.egg-info/requires.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        6 2023-05-22 02:26:50.000000 misc_io_operations-1.1.4/misc_io_operations.egg-info/top_level.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 02:26:50.766478 misc_io_operations-1.1.4/setup.cfg
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1118 2023-05-22 02:26:48.000000 misc_io_operations-1.1.4/setup.py
```

### Comparing `misc_io_operations-1.1.3/PKG-INFO` & `misc_io_operations-1.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: misc_io_operations
-Version: 1.1.3
+Version: 1.1.4
 Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: UNKNOWN
+Download-URL: https://pypi.org/project/miops/
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `misc_io_operations-1.1.3/misc_io_operations.egg-info/PKG-INFO` & `misc_io_operations-1.1.4/misc_io_operations.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: misc-io-operations
-Version: 1.1.3
+Version: 1.1.4
 Summary: Simplification of daily input/output operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: UNKNOWN
+Download-URL: https://pypi.org/project/miops/
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `misc_io_operations-1.1.3/setup.py` & `misc_io_operations-1.1.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup
 setup(
     name='misc_io_operations',
     packages=['miops'],
-    version="1.1.3",
+    download_url="https://pypi.org/project/miops/",
+    version="1.1.4",
     liscense="MIT",
     description="Simplification of daily input/output operations",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="GamerXZEN",
     author_email="codspecialops@gmail.com",
     url="https://github.com/GamerXZEN/misc_io_operations",
```

