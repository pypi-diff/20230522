# Comparing `tmp/pitop.processing-0.30.0.post1.tar.gz` & `tmp/pitop.processing-0.31.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.processing-0.30.0.post1.tar", last modified: Fri Dec 16 14:08:40 2022, max compression
+gzip compressed data, was "dist/pitop.processing-0.31.0.post2.tar", last modified: Mon May 22 19:13:13 2023, max compression
```

## Comparing `pitop.processing-0.30.0.post1.tar` & `pitop.processing-0.31.0.post2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      991 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      153 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/pitop/processing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/pitop/processing/algorithms/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10933 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/algorithms/ball_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/
--rw-r--r--   0 runner    (1001) docker     (122)       90 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      737 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/core/emotion.py
--rw-r--r--   0 runner    (1001) docker     (122)     3361 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/core/face.py
--rw-r--r--   0 runner    (1001) docker     (122)     7135 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/core/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8779 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/emotion_classifier.py
--rw-r--r--   0 runner    (1001) docker     (122)    10660 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/face_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     3250 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/algorithms/line_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/pitop/processing/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/core/load_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/core/math_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5439 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/pitop/processing/core/vision_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/pitop.processing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      991 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/pitop.processing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      892 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/pitop.processing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/pitop.processing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      218 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/pitop.processing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/pitop.processing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-16 14:08:40.000000 pitop.processing-0.30.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2313 2022-12-16 14:07:48.000000 pitop.processing-0.30.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/pitop/processing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/pitop/processing/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10933 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/algorithms/ball_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      737 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/core/emotion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/core/face.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7135 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/core/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8777 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/emotion_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10660 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3250 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/algorithms/line_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/pitop/processing/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/core/load_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/core/math_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5439 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/pitop/processing/core/vision_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/pitop.processing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/pitop.processing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/pitop.processing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/pitop.processing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/pitop.processing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/pitop.processing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:13:13.000000 pitop.processing-0.31.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2313 2023-05-22 19:12:55.000000 pitop.processing-0.31.0.post2/setup.py
```

### Comparing `pitop.processing-0.30.0.post1/PKG-INFO` & `pitop.processing-0.31.0.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.processing
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Processing
```

### Comparing `pitop.processing-0.30.0.post1/pitop/processing/algorithms/ball_detect.py` & `pitop.processing-0.31.0.post2/pitop/processing/algorithms/ball_detect.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/core/emotion.py` & `pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/core/emotion.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/core/face.py` & `pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/core/face.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/core/face_utils.py` & `pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/core/face_utils.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/emotion_classifier.py` & `pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/emotion_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
             (text_x, text_y),
             self.font,
             self.font_scale,
             text_colour,
             thickness=self.font_thickness,
         )
 
-        for (x, y) in face.features:
+        for x, y in face.features:
             cv2.circle(
                 frame,
                 (int(x), int(y)),
                 2,
                 tuple_for_color_by_name("magenta", bgr=True),
                 -1,
             )
```

### Comparing `pitop.processing-0.30.0.post1/pitop/processing/algorithms/faces/face_detector.py` & `pitop.processing-0.31.0.post2/pitop/processing/algorithms/faces/face_detector.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.30.0.post1/pitop/processing/algorithms/line_detect.py` & `pitop.processing-0.31.0.post2/pitop/processing/algorithms/line_detect.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.30.0.post1/pitop/processing/core/load_models.py` & `pitop.processing-0.31.0.post2/pitop/processing/core/load_models.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.30.0.post1/pitop/processing/core/math_functions.py` & `pitop.processing-0.31.0.post2/pitop/processing/core/math_functions.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.30.0.post1/pitop/processing/core/vision_functions.py` & `pitop.processing-0.31.0.post2/pitop/processing/core/vision_functions.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.30.0.post1/pitop.processing.egg-info/PKG-INFO` & `pitop.processing-0.31.0.post2/pitop.processing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.processing
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Processing
```

### Comparing `pitop.processing-0.30.0.post1/pitop.processing.egg-info/SOURCES.txt` & `pitop.processing-0.31.0.post2/pitop.processing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.30.0.post1/setup.py` & `pitop.processing-0.31.0.post2/setup.py`

 * *Files identical despite different names*

