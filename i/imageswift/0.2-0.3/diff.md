# Comparing `tmp/imageswift-0.2.tar.gz` & `tmp/imageswift-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\imageswift-0.2.tar", last modified: Mon May 22 21:03:44 2023, max compression
+gzip compressed data, was "dist\imageswift-0.3.tar", last modified: Mon May 22 21:20:26 2023, max compression
```

## Comparing `imageswift-0.2.tar` & `imageswift-0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 21:03:44.278009 imageswift-0.2/
--rw-rw-rw-   0        0        0      673 2023-05-22 21:03:44.278009 imageswift-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 21:03:44.278009 imageswift-0.2/imageswift/
--rw-rw-rw-   0        0        0       90 2023-05-22 20:36:49.313731 imageswift-0.2/imageswift/__init__.py
--rw-rw-rw-   0        0        0     3347 2023-05-22 20:06:39.463755 imageswift-0.2/imageswift/predicting.py
--rw-rw-rw-   0        0        0     5805 2023-05-22 20:06:46.957769 imageswift-0.2/imageswift/training.py
--rw-rw-rw-   0        0        0       40 2023-05-22 19:49:02.487025 imageswift-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1015 2023-05-22 21:03:41.465918 imageswift-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 21:20:26.842824 imageswift-0.3/
+-rw-rw-rw-   0        0        0      673 2023-05-22 21:20:26.842824 imageswift-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 21:20:26.842824 imageswift-0.3/imageswift/
+-rw-rw-rw-   0        0        0       90 2023-05-22 20:36:49.313731 imageswift-0.3/imageswift/__init__.py
+-rw-rw-rw-   0        0        0     3222 2023-05-22 21:19:19.571918 imageswift-0.3/imageswift/predicting.py
+-rw-rw-rw-   0        0        0     5805 2023-05-22 20:06:46.957769 imageswift-0.3/imageswift/training.py
+-rw-rw-rw-   0        0        0       40 2023-05-22 19:49:02.487025 imageswift-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-05-22 21:20:21.522833 imageswift-0.3/setup.py
```

### Comparing `imageswift-0.2/PKG-INFO` & `imageswift-0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: imageswift
-Version: 0.2
+Version: 0.3
 Summary: Easily train an image recognition model on your own images.
 Home-page: https://github.com/Suchisrit/ImageSwift
 Author: Suchisrit Gangopadhyay
 Author-email: suchisrit@gmail.com
 License: MIT
-Download-URL: https://github.com/Suchisrit/ImageSwift/archive/refs/tags/v0.2.tar.gz
+Download-URL: https://github.com/Suchisrit/ImageSwift/archive/refs/tags/v0.3.tar.gz
 Description: UNKNOWN
 Keywords: CV,Image Recognition,AI,ML
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `imageswift-0.2/imageswift/predicting.py` & `imageswift-0.3/imageswift/predicting.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 import tensorflow as tf
-from tensorflow import keras
-from tensorflow.keras import layers
-from keras.models import Sequential
-from keras.layers import Dense
-from keras.models import model_from_json
+from tensorflow.keras.models import model_from_json
 import os
 
 class TrainedModel():
     def __init__(self, strModelPath, strWeightsPath, strDatasetPath, image_size=(150, 150)):
         self.image_size = image_size
         self.strModelPath = strModelPath
         self.strWeightsPath = strWeightsPath
```

### Comparing `imageswift-0.2/imageswift/training.py` & `imageswift-0.3/imageswift/training.py`

 * *Files identical despite different names*

### Comparing `imageswift-0.2/setup.py` & `imageswift-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'imageswift',         
   packages = ['imageswift'],   
-  version = '0.2',      
+  version = '0.3',      
   license='MIT',        
   description = 'Easily train an image recognition model on your own images.',   
   author = 'Suchisrit Gangopadhyay',                  
   author_email = 'suchisrit@gmail.com',      
   url = 'https://github.com/Suchisrit/ImageSwift',   
-  download_url = 'https://github.com/Suchisrit/ImageSwift/archive/refs/tags/v0.2.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/Suchisrit/ImageSwift/archive/refs/tags/v0.3.tar.gz',    # I explain this later on
   keywords = ['CV', 'Image Recognition', 'AI', 'ML'],   
   install_requires=[            
           'tensorflow==2.3.0',
           'seaborn==0.11.2',
           'pandas==1.2.0',
           'matplotlib==3.3.0'
       ],
```

