# Comparing `tmp/misc_io_operations-1.1.1.tar.gz` & `tmp/misc_io_operations-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misc_io_operations-1.1.1.tar", last modified: Sat May 20 22:08:41 2023, max compression
+gzip compressed data, was "misc_io_operations-1.1.2.tar", last modified: Mon May 22 02:10:19 2023, max compression
```

## Comparing `misc_io_operations-1.1.1.tar` & `misc_io_operations-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-20 22:08:41.844440 misc_io_operations-1.1.1/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1125 2023-05-20 22:08:41.844440 misc_io_operations-1.1.1/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      296 2023-05-20 15:43:55.000000 misc_io_operations-1.1.1/README.md
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-20 22:08:41.844440 misc_io_operations-1.1.1/misc_io_operations/
--rw-r--r--   0 codsp     (1000) codsp     (1000)      187 2023-05-20 04:22:31.000000 misc_io_operations-1.1.1/misc_io_operations/__init__.py
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1250 2023-05-20 15:45:22.000000 misc_io_operations-1.1.1/misc_io_operations/misc_io_operations.py
-drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-20 22:08:41.844440 misc_io_operations-1.1.1/misc_io_operations.egg-info/
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1125 2023-05-20 22:08:41.000000 misc_io_operations-1.1.1/misc_io_operations.egg-info/PKG-INFO
--rw-r--r--   0 codsp     (1000) codsp     (1000)      299 2023-05-20 22:08:41.000000 misc_io_operations-1.1.1/misc_io_operations.egg-info/SOURCES.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-20 22:08:41.000000 misc_io_operations-1.1.1/misc_io_operations.egg-info/dependency_links.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-20 22:08:41.000000 misc_io_operations-1.1.1/misc_io_operations.egg-info/requires.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)       19 2023-05-20 22:08:41.000000 misc_io_operations-1.1.1/misc_io_operations.egg-info/top_level.txt
--rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-20 22:08:41.844440 misc_io_operations-1.1.1/setup.cfg
--rw-r--r--   0 codsp     (1000) codsp     (1000)     1018 2023-05-20 22:05:27.000000 misc_io_operations-1.1.1/setup.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:10:19.799358 misc_io_operations-1.1.2/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1129 2023-05-22 02:10:19.799358 misc_io_operations-1.1.2/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      260 2023-05-22 02:09:13.000000 misc_io_operations-1.1.2/README.md
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:10:19.799358 misc_io_operations-1.1.2/misc_io_operations/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      187 2023-05-20 04:22:31.000000 misc_io_operations-1.1.2/misc_io_operations/__init__.py
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1250 2023-05-20 15:45:22.000000 misc_io_operations-1.1.2/misc_io_operations/misc_io_operations.py
+drwxr-xr-x   0 codsp     (1000) codsp     (1000)        0 2023-05-22 02:10:19.799358 misc_io_operations-1.1.2/misc_io_operations.egg-info/
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1129 2023-05-22 02:10:19.000000 misc_io_operations-1.1.2/misc_io_operations.egg-info/PKG-INFO
+-rw-r--r--   0 codsp     (1000) codsp     (1000)      299 2023-05-22 02:10:19.000000 misc_io_operations-1.1.2/misc_io_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        1 2023-05-22 02:10:19.000000 misc_io_operations-1.1.2/misc_io_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)        9 2023-05-22 02:10:19.000000 misc_io_operations-1.1.2/misc_io_operations.egg-info/requires.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       19 2023-05-22 02:10:19.000000 misc_io_operations-1.1.2/misc_io_operations.egg-info/top_level.txt
+-rw-r--r--   0 codsp     (1000) codsp     (1000)       38 2023-05-22 02:10:19.799358 misc_io_operations-1.1.2/setup.cfg
+-rw-r--r--   0 codsp     (1000) codsp     (1000)     1069 2023-05-22 02:09:31.000000 misc_io_operations-1.1.2/setup.py
```

### Comparing `misc_io_operations-1.1.1/PKG-INFO` & `misc_io_operations-1.1.2/misc_io_operations.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: misc_io_operations
-Version: 1.1.1
+Name: misc-io-operations
+Version: 1.1.2
 Summary: Simplification of daily IO operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: UNKNOWN
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
@@ -14,22 +14,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
 
-# Miscellaneous IO Operations Package
+# Miscellaneous I/O Operations Package
 
 ## About
 
 This is a collection of miscellaneous Python functions
 that can be used to simplify daily and
 lengthy coding processes and tasks.
 
 ## Documentation
 
-@ - Sign for a special keyphrase in a name in the docs
-@c - Console-Based Input/Output Operations
+c (in function name) - Console-Based Input/Output Operations
```

### Comparing `misc_io_operations-1.1.1/misc_io_operations/misc_io_operations.py` & `misc_io_operations-1.1.2/misc_io_operations/misc_io_operations.py`

 * *Files identical despite different names*

### Comparing `misc_io_operations-1.1.1/misc_io_operations.egg-info/PKG-INFO` & `misc_io_operations-1.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: misc-io-operations
-Version: 1.1.1
+Name: misc_io_operations
+Version: 1.1.2
 Summary: Simplification of daily IO operations
 Home-page: https://github.com/GamerXZEN/misc_io_operations
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 License: UNKNOWN
 Keywords: operations,input,output,input/output,miscellaneous,python
 Platform: UNKNOWN
@@ -14,22 +14,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
 
-# Miscellaneous IO Operations Package
+# Miscellaneous I/O Operations Package
 
 ## About
 
 This is a collection of miscellaneous Python functions
 that can be used to simplify daily and
 lengthy coding processes and tasks.
 
 ## Documentation
 
-@ - Sign for a special keyphrase in a name in the docs
-@c - Console-Based Input/Output Operations
+c (in function name) - Console-Based Input/Output Operations
```

### Comparing `misc_io_operations-1.1.1/setup.py` & `misc_io_operations-1.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup
 setup(
     name='misc_io_operations',
     packages=['misc_io_operations'],
-    version="1.1.1",
+    version="1.1.2",
     liscense="MIT",
     description="Simplification of daily IO operations",
     long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
     author="GamerXZEN",
     author_email="codspecialops@gmail.com",
     url="https://github.com/GamerXZEN/misc_io_operations",
     keywords=["operations", "input", "output", "input/output", "miscellaneous", "python",],
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 3 - Alpha",
```

