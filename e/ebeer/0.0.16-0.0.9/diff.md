# Comparing `tmp/ebeer-0.0.16.tar.gz` & `tmp/ebeer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebeer-0.0.16.tar", last modified: Mon May 22 18:22:36 2023, max compression
+gzip compressed data, was "ebeer-0.0.9.tar", last modified: Fri May 19 18:26:10 2023, max compression
```

## Comparing `ebeer-0.0.16.tar` & `ebeer-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:22:36.280148 ebeer-0.0.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-22 18:21:30.000000 ebeer-0.0.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 18:21:30.000000 ebeer-0.0.16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 18:22:36.280148 ebeer-0.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 18:21:30.000000 ebeer-0.0.16/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-22 18:21:30.000000 ebeer-0.0.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 18:22:36.280148 ebeer-0.0.16/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:22:36.268148 ebeer-0.0.16/src/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 18:21:30.000000 ebeer-0.0.16/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:22:36.272148 ebeer-0.0.16/src/ebeer/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-22 18:21:30.000000 ebeer-0.0.16/src/ebeer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-22 18:21:30.000000 ebeer-0.0.16/src/ebeer/beer_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-22 18:21:30.000000 ebeer-0.0.16/src/ebeer/label_index.py
--rw-r--r--   0 runner    (1001) docker     (123)  6684424 2023-05-22 18:21:30.000000 ebeer-0.0.16/src/ebeer/trained_model.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:22:36.276148 ebeer-0.0.16/src/ebeer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 18:22:36.000000 ebeer-0.0.16/src/ebeer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-22 18:22:36.000000 ebeer-0.0.16/src/ebeer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:22:36.000000 ebeer-0.0.16/src/ebeer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 18:22:36.000000 ebeer-0.0.16/src/ebeer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 18:22:36.000000 ebeer-0.0.16/src/ebeer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:22:36.276148 ebeer-0.0.16/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-22 18:21:30.000000 ebeer-0.0.16/tests/test_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:10.477319 ebeer-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 18:26:10.477319 ebeer-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 18:25:05.000000 ebeer-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-19 18:25:05.000000 ebeer-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:26:10.477319 ebeer-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:10.477319 ebeer-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 18:25:05.000000 ebeer-0.0.9/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 18:25:05.000000 ebeer-0.0.9/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:10.477319 ebeer-0.0.9/src/ebeer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 18:25:05.000000 ebeer-0.0.9/src/ebeer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-19 18:25:05.000000 ebeer-0.0.9/src/ebeer/beer_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-19 18:25:05.000000 ebeer-0.0.9/src/ebeer/label_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:10.477319 ebeer-0.0.9/src/ebeer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 18:26:10.000000 ebeer-0.0.9/src/ebeer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-19 18:26:10.000000 ebeer-0.0.9/src/ebeer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:26:10.000000 ebeer-0.0.9/src/ebeer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 18:26:10.000000 ebeer-0.0.9/src/ebeer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-19 18:25:05.000000 ebeer-0.0.9/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:10.477319 ebeer-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-19 18:25:05.000000 ebeer-0.0.9/tests/test_classify.py
```

### Comparing `ebeer-0.0.16/src/ebeer/beer_classifier.py` & `ebeer-0.0.9/src/ebeer/beer_classifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import tensorflow as tf
 
+# from label_index import labels_index
 from tensorflow import keras
 from tensorflow.keras.optimizers import Adam
 from tensorflow.keras.models import Sequential
 from tensorflow.keras.layers import (Dense, Flatten, Conv2D, MaxPooling2D)
 
 
 class BeerClassifier:
@@ -51,18 +52,15 @@
             metrics=[
                 'accuracy',
                 tf.keras.metrics.Precision(),
                 tf.keras.metrics.Recall()
             ]
         )
 
-        import importlib_resources
-        resource_path = importlib_resources.files('ebeer').joinpath(
-            'trained_model.h5')
-        model = keras.models.load_model(resource_path)
+        model = keras.models.load_model("src/trained_model/trained_model.h5")
 
         image_original = tf.keras.utils.load_img(
             path_img,
             grayscale=False,
             color_mode="rgb",
             target_size=None,
             interpolation="nearest"
```

### Comparing `ebeer-0.0.16/src/ebeer/label_index.py` & `ebeer-0.0.9/src/ebeer/label_index.py`

 * *Files identical despite different names*

