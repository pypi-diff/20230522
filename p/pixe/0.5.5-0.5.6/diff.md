# Comparing `tmp/pixe-0.5.5.tar.gz` & `tmp/pixe-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixe-0.5.5.tar", last modified: Mon May 22 02:51:30 2023, max compression
+gzip compressed data, was "pixe-0.5.6.tar", last modified: Mon May 22 03:29:48 2023, max compression
```

## Comparing `pixe-0.5.5.tar` & `pixe-0.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 iroh      (1000) iroh      (1000)        0 2023-05-22 02:51:30.657411 pixe-0.5.5/
--rw-rw-r--   0 iroh      (1000) iroh      (1000)    11357 2023-02-28 15:56:19.000000 pixe-0.5.5/LICENSE
--rw-rw-r--   0 iroh      (1000) iroh      (1000)     4003 2023-05-22 02:51:30.657411 pixe-0.5.5/PKG-INFO
--rw-r--r--   0 iroh      (1000) iroh      (1000)     3382 2023-05-22 00:30:49.000000 pixe-0.5.5/README.md
-drwxrwxr-x   0 iroh      (1000) iroh      (1000)        0 2023-05-22 02:51:30.656411 pixe-0.5.5/pixe.egg-info/
--rw-rw-r--   0 iroh      (1000) iroh      (1000)     4003 2023-05-22 02:51:30.000000 pixe-0.5.5/pixe.egg-info/PKG-INFO
--rw-rw-r--   0 iroh      (1000) iroh      (1000)      255 2023-05-22 02:51:30.000000 pixe-0.5.5/pixe.egg-info/SOURCES.txt
--rw-rw-r--   0 iroh      (1000) iroh      (1000)        1 2023-05-22 02:51:30.000000 pixe-0.5.5/pixe.egg-info/dependency_links.txt
--rw-rw-r--   0 iroh      (1000) iroh      (1000)       34 2023-05-22 02:51:30.000000 pixe-0.5.5/pixe.egg-info/entry_points.txt
--rw-rw-r--   0 iroh      (1000) iroh      (1000)      126 2023-05-22 02:51:30.000000 pixe-0.5.5/pixe.egg-info/requires.txt
--rw-rw-r--   0 iroh      (1000) iroh      (1000)        5 2023-05-22 02:51:30.000000 pixe-0.5.5/pixe.egg-info/top_level.txt
--rw-r--r--   0 iroh      (1000) iroh      (1000)     7194 2023-05-22 02:46:41.000000 pixe-0.5.5/pixe.py
--rw-r--r--   0 iroh      (1000) iroh      (1000)      867 2023-05-22 02:47:46.000000 pixe-0.5.5/pyproject.toml
--rw-rw-r--   0 iroh      (1000) iroh      (1000)       38 2023-05-22 02:51:30.657411 pixe-0.5.5/setup.cfg
-drwxrwxr-x   0 iroh      (1000) iroh      (1000)        0 2023-05-22 02:51:30.656411 pixe-0.5.5/tests/
--rw-rw-r--   0 iroh      (1000) iroh      (1000)     3683 2023-02-28 15:56:19.000000 pixe-0.5.5/tests/test_integration.py
--rw-rw-r--   0 iroh      (1000) iroh      (1000)     1744 2023-02-28 15:56:19.000000 pixe-0.5.5/tests/test_unit.py
+drwxrwxr-x   0 iroh      (1000) iroh      (1000)        0 2023-05-22 03:29:48.591004 pixe-0.5.6/
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)    11357 2023-02-28 15:56:19.000000 pixe-0.5.6/LICENSE
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)     4003 2023-05-22 03:29:48.590004 pixe-0.5.6/PKG-INFO
+-rw-r--r--   0 iroh      (1000) iroh      (1000)     3382 2023-05-22 00:30:49.000000 pixe-0.5.6/README.md
+drwxrwxr-x   0 iroh      (1000) iroh      (1000)        0 2023-05-22 03:29:48.590004 pixe-0.5.6/pixe.egg-info/
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)     4003 2023-05-22 03:29:48.000000 pixe-0.5.6/pixe.egg-info/PKG-INFO
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)      255 2023-05-22 03:29:48.000000 pixe-0.5.6/pixe.egg-info/SOURCES.txt
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)        1 2023-05-22 03:29:48.000000 pixe-0.5.6/pixe.egg-info/dependency_links.txt
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)       34 2023-05-22 03:29:48.000000 pixe-0.5.6/pixe.egg-info/entry_points.txt
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)      126 2023-05-22 03:29:48.000000 pixe-0.5.6/pixe.egg-info/requires.txt
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)        5 2023-05-22 03:29:48.000000 pixe-0.5.6/pixe.egg-info/top_level.txt
+-rw-r--r--   0 iroh      (1000) iroh      (1000)     7358 2023-05-22 03:26:18.000000 pixe-0.5.6/pixe.py
+-rw-r--r--   0 iroh      (1000) iroh      (1000)      867 2023-05-22 03:28:27.000000 pixe-0.5.6/pyproject.toml
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)       38 2023-05-22 03:29:48.591004 pixe-0.5.6/setup.cfg
+drwxrwxr-x   0 iroh      (1000) iroh      (1000)        0 2023-05-22 03:29:48.590004 pixe-0.5.6/tests/
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)     3683 2023-02-28 15:56:19.000000 pixe-0.5.6/tests/test_integration.py
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)     1744 2023-02-28 15:56:19.000000 pixe-0.5.6/tests/test_unit.py
```

### Comparing `pixe-0.5.5/LICENSE` & `pixe-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pixe-0.5.5/PKG-INFO` & `pixe-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixe
-Version: 0.5.5
+Version: 0.5.6
 Summary: A digital helper to keep your files neat and tidy
 Author-email: Chris Wells <chris@ithuna.com>
 License: Apache License, Version 2.0
 Project-URL: homepage, https://github.com/ithuna/pixe.git
 Keywords: archive,photos,organize
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pixe-0.5.5/README.md` & `pixe-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `pixe-0.5.5/pixe.egg-info/PKG-INFO` & `pixe-0.5.6/pixe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixe
-Version: 0.5.5
+Version: 0.5.6
 Summary: A digital helper to keep your files neat and tidy
 Author-email: Chris Wells <chris@ithuna.com>
 License: Apache License, Version 2.0
 Project-URL: homepage, https://github.com/ithuna/pixe.git
 Keywords: archive,photos,organize
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pixe-0.5.5/pixe.py` & `pixe-0.5.6/pixe.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 import datetime
 import pathlib
 import multiprocessing
 import shutil
 import re
 import os
 import fnmatch
+import pkg_resources
 
 import click
 import PIL.Image
 import piexif
 
 # Using a date that shouldn't appear in our collection, but that also isn't a common default.
 # In this case, Ansel Adams birthday.
 ERROR_DATE = datetime.datetime(1902, 2, 20)
 
 # store a datetime of when this run began
 START_TIME = datetime.datetime.now()
 
+# Package introspection
+PKG_RESOURCES = pkg_resources.get_distribution('pixe')
 
 def _calc_checksum(image_path: pathlib.Path, block_size: int = 8192) -> str:
     """
     Create a sha1 checksum of just the image data (no meta/exif).
 
     :param image_path: a path to an image to process
     :param block_size: the block size to use when chunking up the image data
@@ -156,14 +159,15 @@
     """
     for file in file_list:
         print(_process_file(file, dest, move, **kwargs))
 
 
 @click.command()
 @click.argument("src")
+@click.version_option(PKG_RESOURCES.version, '-v', '--version')
 @click.option("--dest", "-d", default=".", help="desired destination")
 @click.option(
     "--recurse",
     "-r",
     is_flag=True,
     default=False,
     help="recurse into sub-directories (default: off)",
```

### Comparing `pixe-0.5.5/pyproject.toml` & `pixe-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixe"
-version = "0.5.5"
+version = "0.5.6"
 description = "A digital helper to keep your files neat and tidy"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "Apache License, Version 2.0"}
 keywords = ["archive", "photos", "organize"]
 authors = [
     {name = "Chris Wells", email = "chris@ithuna.com"},
```

### Comparing `pixe-0.5.5/tests/test_integration.py` & `pixe-0.5.6/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pixe-0.5.5/tests/test_unit.py` & `pixe-0.5.6/tests/test_unit.py`

 * *Files identical despite different names*

