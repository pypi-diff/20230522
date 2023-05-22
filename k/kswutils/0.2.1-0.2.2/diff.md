# Comparing `tmp/kswutils-0.2.1.tar.gz` & `tmp/kswutils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kswutils-0.2.1.tar", last modified: Fri Mar 10 03:30:25 2023, max compression
+gzip compressed data, was "kswutils-0.2.2.tar", last modified: Mon May 22 05:11:51 2023, max compression
```

## Comparing `kswutils-0.2.1.tar` & `kswutils-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-03-10 03:30:25.867996 kswutils-0.2.1/
--rw-r--r--   0 justin     (501) staff       (20)      160 2023-03-10 03:30:25.868050 kswutils-0.2.1/PKG-INFO
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-03-10 03:30:25.866351 kswutils-0.2.1/kswutils/
--rw-rw-r--   0 justin     (501) staff       (20)        4 2023-01-12 05:41:01.000000 kswutils-0.2.1/kswutils/__init__.py
--rw-r--r--   0 justin     (501) staff       (20)     1489 2023-01-12 09:14:40.000000 kswutils-0.2.1/kswutils/accelerometer.py
--rw-r--r--   0 justin     (501) staff       (20)     2152 2023-03-10 03:26:57.000000 kswutils-0.2.1/kswutils/accelerometer2.py
--rwxrwxrwx   0 justin     (501) staff       (20)     2154 2023-02-27 06:09:06.000000 kswutils-0.2.1/kswutils/calculator.py
--rw-r--r--   0 justin     (501) staff       (20)     7716 2023-02-27 06:08:20.000000 kswutils-0.2.1/kswutils/drawio.py
--rwxrwxrwx   0 justin     (501) staff       (20)     2136 2023-02-27 05:50:32.000000 kswutils-0.2.1/kswutils/fileio.py
--rw-r--r--   0 justin     (501) staff       (20)     2335 2023-02-27 06:06:50.000000 kswutils-0.2.1/kswutils/signalprocessing.py
--rwxrwxrwx   0 justin     (501) staff       (20)     4674 2023-01-12 09:14:50.000000 kswutils-0.2.1/kswutils/smartsensor.py
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-03-10 03:30:25.867865 kswutils-0.2.1/kswutils.egg-info/
--rw-r--r--   0 justin     (501) staff       (20)      160 2023-03-10 03:30:25.000000 kswutils-0.2.1/kswutils.egg-info/PKG-INFO
--rw-r--r--   0 justin     (501) staff       (20)      365 2023-03-10 03:30:25.000000 kswutils-0.2.1/kswutils.egg-info/SOURCES.txt
--rw-r--r--   0 justin     (501) staff       (20)        1 2023-03-10 03:30:25.000000 kswutils-0.2.1/kswutils.egg-info/dependency_links.txt
--rw-r--r--   0 justin     (501) staff       (20)        1 2023-01-10 08:17:46.000000 kswutils-0.2.1/kswutils.egg-info/not-zip-safe
--rw-r--r--   0 justin     (501) staff       (20)        9 2023-03-10 03:30:25.000000 kswutils-0.2.1/kswutils.egg-info/top_level.txt
--rw-rw-r--   0 justin     (501) staff       (20)       38 2023-03-10 03:30:25.868383 kswutils-0.2.1/setup.cfg
--rw-rw-r--   0 justin     (501) staff       (20)      206 2023-03-10 03:29:59.000000 kswutils-0.2.1/setup.py
+drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-05-22 05:11:51.515421 kswutils-0.2.2/
+-rw-r--r--   0 justin     (501) staff       (20)      160 2023-05-22 05:11:51.515503 kswutils-0.2.2/PKG-INFO
+drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-05-22 05:11:51.513863 kswutils-0.2.2/kswutils/
+-rw-rw-r--   0 justin     (501) staff       (20)        4 2023-01-12 05:41:01.000000 kswutils-0.2.2/kswutils/__init__.py
+-rw-r--r--   0 justin     (501) staff       (20)     1489 2023-01-12 09:14:40.000000 kswutils-0.2.2/kswutils/accelerometer.py
+-rw-r--r--   0 justin     (501) staff       (20)     2152 2023-03-10 03:26:57.000000 kswutils-0.2.2/kswutils/accelerometer2.py
+-rwxrwxrwx   0 justin     (501) staff       (20)     2154 2023-02-27 06:09:06.000000 kswutils-0.2.2/kswutils/calculator.py
+-rw-r--r--   0 justin     (501) staff       (20)     7716 2023-02-27 06:08:20.000000 kswutils-0.2.2/kswutils/drawio.py
+-rwxrwxrwx   0 justin     (501) staff       (20)     3069 2023-05-22 05:09:40.000000 kswutils-0.2.2/kswutils/fileio.py
+-rw-r--r--   0 justin     (501) staff       (20)     2335 2023-02-27 06:06:50.000000 kswutils-0.2.2/kswutils/signalprocessing.py
+-rwxrwxrwx   0 justin     (501) staff       (20)     4674 2023-01-12 09:14:50.000000 kswutils-0.2.2/kswutils/smartsensor.py
+drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-05-22 05:11:51.515245 kswutils-0.2.2/kswutils.egg-info/
+-rw-r--r--   0 justin     (501) staff       (20)      160 2023-05-22 05:11:51.000000 kswutils-0.2.2/kswutils.egg-info/PKG-INFO
+-rw-r--r--   0 justin     (501) staff       (20)      365 2023-05-22 05:11:51.000000 kswutils-0.2.2/kswutils.egg-info/SOURCES.txt
+-rw-r--r--   0 justin     (501) staff       (20)        1 2023-05-22 05:11:51.000000 kswutils-0.2.2/kswutils.egg-info/dependency_links.txt
+-rw-r--r--   0 justin     (501) staff       (20)        1 2023-01-10 08:17:46.000000 kswutils-0.2.2/kswutils.egg-info/not-zip-safe
+-rw-r--r--   0 justin     (501) staff       (20)        9 2023-05-22 05:11:51.000000 kswutils-0.2.2/kswutils.egg-info/top_level.txt
+-rw-rw-r--   0 justin     (501) staff       (20)       38 2023-05-22 05:11:51.515842 kswutils-0.2.2/setup.cfg
+-rw-rw-r--   0 justin     (501) staff       (20)      206 2023-05-22 05:10:48.000000 kswutils-0.2.2/setup.py
```

### Comparing `kswutils-0.2.1/kswutils/accelerometer.py` & `kswutils-0.2.2/kswutils/accelerometer.py`

 * *Files identical despite different names*

### Comparing `kswutils-0.2.1/kswutils/accelerometer2.py` & `kswutils-0.2.2/kswutils/accelerometer2.py`

 * *Files identical despite different names*

### Comparing `kswutils-0.2.1/kswutils/calculator.py` & `kswutils-0.2.2/kswutils/calculator.py`

 * *Files identical despite different names*

### Comparing `kswutils-0.2.1/kswutils/drawio.py` & `kswutils-0.2.2/kswutils/drawio.py`

 * *Files identical despite different names*

### Comparing `kswutils-0.2.1/kswutils/fileio.py` & `kswutils-0.2.2/kswutils/fileio.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,48 @@
 import os
 import pickle
+import logging
+from datetime import datetime
 
 # Path vs Directory
 # Path is the directory to an object (a file)
 # Path: Obj
 # Directory: Folder
 
 
 class FileIO:
     def __init__(self) -> None:
         pass
 
     @staticmethod
+    def create_logger():
+        dir_path = os.path.join(os.getcwd(), 'log')
+        filename = "{:%Y-%m-%d_%H-%M-%S}".format(datetime.now()) + '.log'
+
+        logging.captureWarnings(True)
+        formatter = logging.Formatter(
+            '%(asctime)s %(levelname)s %(message)s')
+        logger = logging.getLogger('py.warnings')
+        logger.setLevel(logging.INFO)
+
+        if not os.path.exists(dir_path):
+            os.makedirs(dir_path)
+
+        fileHandler = logging.FileHandler(dir_path+'/'+filename, 'w', 'utf-8')
+        fileHandler.setFormatter(formatter)
+        logger.addHandler(fileHandler)
+
+        consoleHandler = logging.StreamHandler()
+        consoleHandler.setLevel(logging.DEBUG)
+        consoleHandler.setFormatter(formatter)
+        logger.addHandler(consoleHandler)
+        
+        return logger        
+
+    @staticmethod
     def get_subdirectories(baseDir):
         """ get sub-directories / sub-paths
 
         Args:
             baseDir (string or list): target directory(ies).
 
         Returns:
@@ -80,7 +107,9 @@
     @staticmethod
     def get_name_with_extion(dir):
         return os.path.basename(dir)
 
     @staticmethod
     def get_name_without_extion(dir):
         return os.path.basename(dir).split('.')[0]
+    
+
```

### Comparing `kswutils-0.2.1/kswutils/signalprocessing.py` & `kswutils-0.2.2/kswutils/signalprocessing.py`

 * *Files identical despite different names*

### Comparing `kswutils-0.2.1/kswutils/smartsensor.py` & `kswutils-0.2.2/kswutils/smartsensor.py`

 * *Files identical despite different names*

