# Comparing `tmp/flirimageextractor-1.5.1.tar.gz` & `tmp/flirimageextractor-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flirimageextractor-1.5.1.tar", max compression
+gzip compressed data, was "flirimageextractor-1.5.2.tar", max compression
```

## Comparing `flirimageextractor-1.5.1.tar` & `flirimageextractor-1.5.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-04-28 00:51:49.787215 flirimageextractor-1.5.1/LICENSE
--rw-r--r--   0        0        0     3520 2023-04-28 00:51:49.787215 flirimageextractor-1.5.1/README.md
--rw-r--r--   0        0        0      114 2023-04-28 00:51:49.807215 flirimageextractor-1.5.1/flirimageextractor/__init__.py
--rw-r--r--   0        0        0     3604 2023-04-28 00:51:49.807215 flirimageextractor-1.5.1/flirimageextractor/__main__.py
--rw-r--r--   0        0        0     2135 2023-04-28 00:51:49.807215 flirimageextractor-1.5.1/flirimageextractor/dialogs.py
--rw-r--r--   0        0        0    16918 2023-04-28 00:51:49.807215 flirimageextractor-1.5.1/flirimageextractor/flir_image_extractor.py
--rw-r--r--   0        0        0     9492 2023-04-28 00:51:49.807215 flirimageextractor-1.5.1/flirimageextractor/flyr_unpack.py
--rw-r--r--   0        0        0     4140 2023-04-28 00:51:49.807215 flirimageextractor-1.5.1/flirimageextractor/processing.py
--rw-r--r--   0        0        0    42181 2023-04-28 00:51:49.807215 flirimageextractor-1.5.1/flirimageextractor/thermal_base.py
--rw-r--r--   0        0        0     9341 2023-04-28 00:51:49.807215 flirimageextractor-1.5.1/flirimageextractor/utils.py
--rw-r--r--   0        0        0     1568 2023-04-28 00:51:49.807215 flirimageextractor-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     5079 1970-01-01 00:00:00.000000 flirimageextractor-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-22 00:44:41.960662 flirimageextractor-1.5.2/LICENSE
+-rw-r--r--   0        0        0     3520 2023-05-22 00:44:41.960662 flirimageextractor-1.5.2/README.md
+-rw-r--r--   0        0        0      114 2023-05-22 00:44:41.984663 flirimageextractor-1.5.2/flirimageextractor/__init__.py
+-rw-r--r--   0        0        0     3604 2023-05-22 00:44:41.984663 flirimageextractor-1.5.2/flirimageextractor/__main__.py
+-rw-r--r--   0        0        0     2135 2023-05-22 00:44:41.984663 flirimageextractor-1.5.2/flirimageextractor/dialogs.py
+-rw-r--r--   0        0        0    16918 2023-05-22 00:44:41.984663 flirimageextractor-1.5.2/flirimageextractor/flir_image_extractor.py
+-rw-r--r--   0        0        0     9492 2023-05-22 00:44:41.984663 flirimageextractor-1.5.2/flirimageextractor/flyr_unpack.py
+-rw-r--r--   0        0        0     4140 2023-05-22 00:44:41.984663 flirimageextractor-1.5.2/flirimageextractor/processing.py
+-rw-r--r--   0        0        0    42181 2023-05-22 00:44:41.988663 flirimageextractor-1.5.2/flirimageextractor/thermal_base.py
+-rw-r--r--   0        0        0     9341 2023-05-22 00:44:41.988663 flirimageextractor-1.5.2/flirimageextractor/utils.py
+-rw-r--r--   0        0        0     1568 2023-05-22 00:44:41.988663 flirimageextractor-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 flirimageextractor-1.5.2/PKG-INFO
```

### Comparing `flirimageextractor-1.5.1/LICENSE` & `flirimageextractor-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.1/README.md` & `flirimageextractor-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.1/flirimageextractor/__main__.py` & `flirimageextractor-1.5.2/flirimageextractor/__main__.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.1/flirimageextractor/dialogs.py` & `flirimageextractor-1.5.2/flirimageextractor/dialogs.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.1/flirimageextractor/flir_image_extractor.py` & `flirimageextractor-1.5.2/flirimageextractor/flir_image_extractor.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.1/flirimageextractor/flyr_unpack.py` & `flirimageextractor-1.5.2/flirimageextractor/flyr_unpack.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.1/flirimageextractor/processing.py` & `flirimageextractor-1.5.2/flirimageextractor/processing.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.1/flirimageextractor/thermal_base.py` & `flirimageextractor-1.5.2/flirimageextractor/thermal_base.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.1/flirimageextractor/utils.py` & `flirimageextractor-1.5.2/flirimageextractor/utils.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.1/pyproject.toml` & `flirimageextractor-1.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flirimageextractor"
-version = "1.5.1"
+version = "1.5.2"
 description = "A small tool/lib to read temperatures and original photos from FLIR® thermal camera images."
 authors = [
     "National Drones <development@nationaldrones.com>",
     "olawale williams <olawalewilliams9438@gmail.com>",
 ]
 readme = "README.md"
 maintainers = [
```

### Comparing `flirimageextractor-1.5.1/PKG-INFO` & `flirimageextractor-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flirimageextractor
-Version: 1.5.1
+Version: 1.5.2
 Summary: A small tool/lib to read temperatures and original photos from FLIR® thermal camera images.
 Home-page: https://github.com/nationaldronesau/FlirImageExtractor
 License: MIT
 Keywords: extract-images,flir,thermal,flirtools
 Author: National Drones
 Author-email: development@nationaldrones.com
 Maintainer: olawale williams
@@ -15,15 +15,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Digital Camera
 Requires-Dist: keyring (==23.13.1)
 Requires-Dist: loguru (==0.7.0)
 Requires-Dist: logzero (==1.7.0)
 Requires-Dist: m2r (==0.3.1)
 Requires-Dist: matplotlib (==3.5.3)
 Requires-Dist: numpy (==1.21.1)
```

