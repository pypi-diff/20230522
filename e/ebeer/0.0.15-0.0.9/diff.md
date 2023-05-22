# Comparing `tmp/ebeer-0.0.15.tar.gz` & `tmp/ebeer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebeer-0.0.15.tar", last modified: Mon May 22 17:57:28 2023, max compression
+gzip compressed data, was "ebeer-0.0.9.tar", last modified: Fri May 19 18:26:10 2023, max compression
```

## Comparing `ebeer-0.0.15.tar` & `ebeer-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:57:28.320551 ebeer-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-22 17:56:17.000000 ebeer-0.0.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 17:56:17.000000 ebeer-0.0.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 17:57:28.320551 ebeer-0.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 17:56:17.000000 ebeer-0.0.15/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-22 17:56:17.000000 ebeer-0.0.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:57:28.320551 ebeer-0.0.15/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:57:28.312550 ebeer-0.0.15/src/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 17:56:17.000000 ebeer-0.0.15/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:57:28.312550 ebeer-0.0.15/src/ebeer/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-22 17:56:17.000000 ebeer-0.0.15/src/ebeer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-22 17:56:17.000000 ebeer-0.0.15/src/ebeer/beer_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-22 17:56:17.000000 ebeer-0.0.15/src/ebeer/label_index.py
--rw-r--r--   0 runner    (1001) docker     (123)  6684424 2023-05-22 17:56:18.000000 ebeer-0.0.15/src/ebeer/trained_model.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:57:28.320551 ebeer-0.0.15/src/ebeer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 17:57:28.000000 ebeer-0.0.15/src/ebeer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-22 17:57:28.000000 ebeer-0.0.15/src/ebeer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:57:28.000000 ebeer-0.0.15/src/ebeer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 17:57:28.000000 ebeer-0.0.15/src/ebeer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 17:57:28.000000 ebeer-0.0.15/src/ebeer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:57:28.320551 ebeer-0.0.15/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-22 17:56:18.000000 ebeer-0.0.15/tests/test_classify.py
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

### Comparing `ebeer-0.0.15/src/ebeer/beer_classifier.py` & `ebeer-0.0.9/src/ebeer/beer_classifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import numpy as np
 import tensorflow as tf
 
+# from label_index import labels_index
 from tensorflow import keras
 from tensorflow.keras.optimizers import Adam
 from tensorflow.keras.models import Sequential
 from tensorflow.keras.layers import (Dense, Flatten, Conv2D, MaxPooling2D)
 
 
 class BeerClassifier:
 
     def __init__(self) -> None:
-        pass 
+        pass
 
-    def predict(self, path_cnn_weights, path_img):
+    def predict(self, path_img):
 
         width = 128
         height = 128
         size = (width, height)
         channels = 3
         n_neuronios_saida = 20
         learning_rate = 1e-4
@@ -51,15 +52,15 @@
             metrics=[
                 'accuracy',
                 tf.keras.metrics.Precision(),
                 tf.keras.metrics.Recall()
             ]
         )
 
-        model = keras.models.load_model(path_cnn_weights)
+        model = keras.models.load_model("src/trained_model/trained_model.h5")
 
         image_original = tf.keras.utils.load_img(
             path_img,
             grayscale=False,
             color_mode="rgb",
             target_size=None,
             interpolation="nearest"
```

### Comparing `ebeer-0.0.15/src/ebeer/label_index.py` & `ebeer-0.0.9/src/ebeer/label_index.py`

 * *Files identical despite different names*

