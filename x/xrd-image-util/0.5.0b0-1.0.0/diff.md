# Comparing `tmp/xrd-image-util-0.5.0b0.tar.gz` & `tmp/xrd-image-util-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrd-image-util-0.5.0b0.tar", last modified: Fri Feb 17 16:42:42 2023, max compression
+gzip compressed data, was "xrd-image-util-1.0.0.tar", last modified: Mon May 22 15:47:07 2023, max compression
```

## Comparing `xrd-image-util-0.5.0b0.tar` & `xrd-image-util-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 16:42:42.991308 xrd-image-util-0.5.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-02-17 16:42:30.000000 xrd-image-util-0.5.0b0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-02-17 16:42:42.991308 xrd-image-util-0.5.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-17 16:42:30.000000 xrd-image-util-0.5.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-02-17 16:42:31.000000 xrd-image-util-0.5.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 16:42:42.991308 xrd-image-util-0.5.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 16:42:42.991308 xrd-image-util-0.5.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-17 16:42:31.000000 xrd-image-util-0.5.0b0/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-02-17 16:42:31.000000 xrd-image-util-0.5.0b0/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-17 16:42:31.000000 xrd-image-util-0.5.0b0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 16:42:42.991308 xrd-image-util-0.5.0b0/xrd_image_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-02-17 16:42:42.000000 xrd-image-util-0.5.0b0/xrd_image_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-17 16:42:42.000000 xrd-image-util-0.5.0b0/xrd_image_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 16:42:42.000000 xrd-image-util-0.5.0b0/xrd_image_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-17 16:42:42.000000 xrd-image-util-0.5.0b0/xrd_image_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-17 16:42:42.000000 xrd-image-util-0.5.0b0/xrd_image_util.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 16:42:42.991308 xrd-image-util-0.5.0b0/xrdimageutil/
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-02-17 16:42:31.000000 xrd-image-util-0.5.0b0/xrdimageutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-02-17 16:42:31.000000 xrd-image-util-0.5.0b0/xrdimageutil/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:47:07.270236 xrd-image-util-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-22 15:46:54.000000 xrd-image-util-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-22 15:47:07.270236 xrd-image-util-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-22 15:46:54.000000 xrd-image-util-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-22 15:46:55.000000 xrd-image-util-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:47:07.270236 xrd-image-util-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:47:07.266236 xrd-image-util-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-22 15:46:55.000000 xrd-image-util-1.0.0/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-22 15:46:55.000000 xrd-image-util-1.0.0/tests/test_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:47:07.266236 xrd-image-util-1.0.0/xrd_image_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-22 15:47:07.000000 xrd-image-util-1.0.0/xrd_image_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-22 15:47:07.000000 xrd-image-util-1.0.0/xrd_image_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:47:07.000000 xrd-image-util-1.0.0/xrd_image_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 15:47:07.000000 xrd-image-util-1.0.0/xrd_image_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 15:47:07.000000 xrd-image-util-1.0.0/xrd_image_util.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:47:07.266236 xrd-image-util-1.0.0/xrdimageutil/
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-05-22 15:46:55.000000 xrd-image-util-1.0.0/xrdimageutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-22 15:46:55.000000 xrd-image-util-1.0.0/xrdimageutil/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-22 15:46:55.000000 xrd-image-util-1.0.0/xrdimageutil/utils.py
```

### Comparing `xrd-image-util-0.5.0b0/LICENSE.txt` & `xrd-image-util-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xrd-image-util-0.5.0b0/PKG-INFO` & `xrd-image-util-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrd-image-util
-Version: 0.5.0b0
+Version: 1.0.0
 Summary: Utility package for handling XRD image data.
 Author-email: Henry Smith <henryjsmith12@outlook.com>
 License: Copyright (c) UChicago Argonne, LLC. All rights reserved.
         
         Copyright UChicago Argonne, LLC. This software was produced
         under U.S. Government contract DE-AC02-06CH11357 for Argonne National
         Laboratory (ANL), which is operated by UChicago Argonne, LLC for the
@@ -73,16 +73,14 @@
 ```pip install xrd-image-util```
 
 ## Execution
 The package can be imported in-line with the following line of code (the alias of `xiu` is not required):
 
 ```import xrdimageutil as xiu```
 
-See the `demos` subdirectory for basic use cases.
-
 ## License
 See [`LICENSE.txt`](https://github.com/henryjsmith12/xrd-image-util/blob/main/LICENSE) for more information.
 
 ## Author
 [Henry Smith](https://www.linkedin.com/in/henry-smith-5956a0189/) - Co-op Student Technical at Argonne National Laboratory
 
 ## Support
```

### Comparing `xrd-image-util-0.5.0b0/README.md` & `xrd-image-util-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 ```pip install xrd-image-util```
 
 ## Execution
 The package can be imported in-line with the following line of code (the alias of `xiu` is not required):
 
 ```import xrdimageutil as xiu```
 
-See the `demos` subdirectory for basic use cases.
-
 ## License
 See [`LICENSE.txt`](https://github.com/henryjsmith12/xrd-image-util/blob/main/LICENSE) for more information.
 
 ## Author
 [Henry Smith](https://www.linkedin.com/in/henry-smith-5956a0189/) - Co-op Student Technical at Argonne National Laboratory
 
 ## Support
```

### Comparing `xrd-image-util-0.5.0b0/pyproject.toml` & `xrd-image-util-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xrd-image-util"
-version = "0.5.0-beta"
+version = "1.0.0"
 authors = [
     {name = "Henry Smith", email = "henryjsmith12@outlook.com"},
 ]
 description = "Utility package for handling XRD image data."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xrd-image-util-0.5.0b0/xrd_image_util.egg-info/PKG-INFO` & `xrd-image-util-1.0.0/xrd_image_util.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrd-image-util
-Version: 0.5.0b0
+Version: 1.0.0
 Summary: Utility package for handling XRD image data.
 Author-email: Henry Smith <henryjsmith12@outlook.com>
 License: Copyright (c) UChicago Argonne, LLC. All rights reserved.
         
         Copyright UChicago Argonne, LLC. This software was produced
         under U.S. Government contract DE-AC02-06CH11357 for Argonne National
         Laboratory (ANL), which is operated by UChicago Argonne, LLC for the
@@ -73,16 +73,14 @@
 ```pip install xrd-image-util```
 
 ## Execution
 The package can be imported in-line with the following line of code (the alias of `xiu` is not required):
 
 ```import xrdimageutil as xiu```
 
-See the `demos` subdirectory for basic use cases.
-
 ## License
 See [`LICENSE.txt`](https://github.com/henryjsmith12/xrd-image-util/blob/main/LICENSE) for more information.
 
 ## Author
 [Henry Smith](https://www.linkedin.com/in/henry-smith-5956a0189/) - Co-op Student Technical at Argonne National Laboratory
 
 ## Support
```

