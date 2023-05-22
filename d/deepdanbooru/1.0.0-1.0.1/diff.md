# Comparing `tmp/deepdanbooru-1.0.0.tar.gz` & `tmp/deepdanbooru-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdanbooru-1.0.0.tar", last modified: Mon May 22 17:26:11 2023, max compression
+gzip compressed data, was "deepdanbooru-1.0.1.tar", last modified: Mon May 22 17:33:49 2023, max compression
```

## Comparing `deepdanbooru-1.0.0.tar` & `deepdanbooru-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,20 @@
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.934501 deepdanbooru-1.0.0/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     1068 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/LICENSE
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     5039 2023-05-22 17:26:11.934501 deepdanbooru-1.0.0/PKG-INFO
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     4459 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/README.md
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.927834 deepdanbooru-1.0.0/deepdanbooru/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)      312 2023-05-22 17:23:26.000000 deepdanbooru-1.0.0/deepdanbooru/__init__.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     7997 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/__main__.py
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.931167 deepdanbooru-1.0.0/deepdanbooru/commands/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)      390 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/commands/__init__.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     1237 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/commands/convert_to_tflite.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)      422 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/commands/create_project.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     5123 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/commands/download_tags.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     3255 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/commands/evaluate.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     1439 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/commands/evaluate_project.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     3992 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/commands/grad_cam.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     4392 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/commands/make_training_database.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)    12774 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/commands/train_project.py
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.931167 deepdanbooru-1.0.0/deepdanbooru/data/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     1047 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/data/__init__.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     1192 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/data/dataset.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     3699 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/data/dataset_wrapper.py
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.931167 deepdanbooru-1.0.0/deepdanbooru/extra/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)      434 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/extra/__init__.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     1440 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/gradcam.py
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.931167 deepdanbooru-1.0.0/deepdanbooru/image/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     1761 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/image/__init__.py
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.931167 deepdanbooru-1.0.0/deepdanbooru/io/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)      867 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/io/__init__.py
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.931167 deepdanbooru-1.0.0/deepdanbooru/model/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)      289 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/model/__init__.py
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.931167 deepdanbooru-1.0.0/deepdanbooru/model/layers/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     2147 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/model/layers/__init__.py
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.931167 deepdanbooru-1.0.0/deepdanbooru/model/losses/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)      861 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/model/losses/__init__.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     6102 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/model/resnet.py
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.934501 deepdanbooru-1.0.0/deepdanbooru/project/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)      172 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/project/__init__.py
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     1650 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/project/project.py
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.934501 deepdanbooru-1.0.0/deepdanbooru/train/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/deepdanbooru/train/__init__.py
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.931167 deepdanbooru-1.0.0/deepdanbooru.egg-info/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     5039 2023-05-22 17:26:11.000000 deepdanbooru-1.0.0/deepdanbooru.egg-info/PKG-INFO
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     1159 2023-05-22 17:26:11.000000 deepdanbooru-1.0.0/deepdanbooru.egg-info/SOURCES.txt
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)        1 2023-05-22 17:26:11.000000 deepdanbooru-1.0.0/deepdanbooru.egg-info/dependency_links.txt
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)       60 2023-05-22 17:26:11.000000 deepdanbooru-1.0.0/deepdanbooru.egg-info/entry_points.txt
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)        1 2023-05-22 17:21:20.000000 deepdanbooru-1.0.0/deepdanbooru.egg-info/not-zip-safe
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)      156 2023-05-22 17:26:11.000000 deepdanbooru-1.0.0/deepdanbooru.egg-info/requires.txt
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)       13 2023-05-22 17:26:11.000000 deepdanbooru-1.0.0/deepdanbooru.egg-info/top_level.txt
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)       80 2023-05-22 17:12:57.000000 deepdanbooru-1.0.0/pyproject.toml
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     1114 2023-05-22 17:26:11.934501 deepdanbooru-1.0.0/setup.cfg
-drwxr-xr-x   0 kamuri    (1000) kamuri    (1000)        0 2023-05-22 17:26:11.934501 deepdanbooru-1.0.0/tests/
--rw-r--r--   0 kamuri    (1000) kamuri    (1000)     2379 2023-05-22 13:41:43.000000 deepdanbooru-1.0.0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:49.265826 deepdanbooru-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-22 17:33:40.000000 deepdanbooru-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-22 17:33:49.265826 deepdanbooru-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-22 17:33:40.000000 deepdanbooru-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:49.265826 deepdanbooru-1.0.1/deepdanbooru/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-22 17:33:40.000000 deepdanbooru-1.0.1/deepdanbooru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-05-22 17:33:40.000000 deepdanbooru-1.0.1/deepdanbooru/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-22 17:33:40.000000 deepdanbooru-1.0.1/deepdanbooru/gradcam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:49.265826 deepdanbooru-1.0.1/deepdanbooru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-22 17:33:49.000000 deepdanbooru-1.0.1/deepdanbooru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-22 17:33:49.000000 deepdanbooru-1.0.1/deepdanbooru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:33:49.000000 deepdanbooru-1.0.1/deepdanbooru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-22 17:33:49.000000 deepdanbooru-1.0.1/deepdanbooru.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:33:49.000000 deepdanbooru-1.0.1/deepdanbooru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-22 17:33:49.000000 deepdanbooru-1.0.1/deepdanbooru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 17:33:49.000000 deepdanbooru-1.0.1/deepdanbooru.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 17:33:40.000000 deepdanbooru-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-22 17:33:49.265826 deepdanbooru-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:49.265826 deepdanbooru-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-22 17:33:40.000000 deepdanbooru-1.0.1/tests/test_main.py
```

### Comparing `deepdanbooru-1.0.0/LICENSE` & `deepdanbooru-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepdanbooru-1.0.0/PKG-INFO` & `deepdanbooru-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: deepdanbooru
-Version: 1.0.0
-Summary: "DeepDanbooru is AI based multi-label girl image classification system, "
+Version: 1.0.1
+Summary: DeepDanbooru is AI based multi-label girl image classification system, implemented by using TensorFlow.
 Home-page: https://github.com/KichangKim/DeepDanbooru
 Author: Kichang Kim
 Author-email: admin@kanotype.net
 License: MIT
 Keywords: icq bot framework async python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `deepdanbooru-1.0.0/README.md` & `deepdanbooru-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `deepdanbooru-1.0.0/deepdanbooru/__main__.py` & `deepdanbooru-1.0.1/deepdanbooru/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import click
 import warnings
 import os
 import deepdanbooru as dd
 import tensorflow.lite as tflite
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 
 @click.version_option(prog_name="DeepDanbooru", version=__version__)
 @click.group()
 def main():
     """
     AI based multi-label girl image classification system, implemented by using TensorFlow.
```

### Comparing `deepdanbooru-1.0.0/deepdanbooru/gradcam.py` & `deepdanbooru-1.0.1/deepdanbooru/gradcam.py`

 * *Files identical despite different names*

### Comparing `deepdanbooru-1.0.0/deepdanbooru.egg-info/PKG-INFO` & `deepdanbooru-1.0.1/deepdanbooru.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: deepdanbooru
-Version: 1.0.0
-Summary: "DeepDanbooru is AI based multi-label girl image classification system, "
+Version: 1.0.1
+Summary: DeepDanbooru is AI based multi-label girl image classification system, implemented by using TensorFlow.
 Home-page: https://github.com/KichangKim/DeepDanbooru
 Author: Kichang Kim
 Author-email: admin@kanotype.net
 License: MIT
 Keywords: icq bot framework async python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `deepdanbooru-1.0.0/setup.cfg` & `deepdanbooru-1.0.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [metadata]
 name = deepdanbooru
 version = attr: deepdanbooru.__main__.__version__
-description = "DeepDanbooru is AI based multi-label girl image classification system, "
-	"implemented by using TensorFlow."
+description = DeepDanbooru is AI based multi-label girl image classification system, implemented by using TensorFlow.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Kichang Kim
 author_email = admin@kanotype.net
 url = https://github.com/KichangKim/DeepDanbooru
 keywords = icq bot framework async python
 license = MIT
```

### Comparing `deepdanbooru-1.0.0/tests/test_main.py` & `deepdanbooru-1.0.1/tests/test_main.py`

 * *Files identical despite different names*

