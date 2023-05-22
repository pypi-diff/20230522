# Comparing `tmp/GrappyLfjv-0.0.17.tar.gz` & `tmp/GrappyLfjv-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GrappyLfjv-0.0.17.tar", last modified: Mon May 22 00:37:41 2023, max compression
+gzip compressed data, was "GrappyLfjv-0.0.18.tar", last modified: Mon May 22 07:17:23 2023, max compression
```

## Comparing `GrappyLfjv-0.0.17.tar` & `GrappyLfjv-0.0.18.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 00:37:41.211758 GrappyLfjv-0.0.17/
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     1060 2023-05-16 15:35:17.000000 GrappyLfjv-0.0.17/LICENSE
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     1395 2023-05-22 00:37:41.211352 GrappyLfjv-0.0.17/PKG-INFO
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     1139 2023-05-22 00:26:49.000000 GrappyLfjv-0.0.17/README.md
--rw-r--r--   0 benjamintrevian   (501) staff       (20)       38 2023-05-22 00:37:41.211916 GrappyLfjv-0.0.17/setup.cfg
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      606 2023-05-22 00:37:35.000000 GrappyLfjv-0.0.17/setup.py
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 00:37:41.207998 GrappyLfjv-0.0.17/src/
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 00:37:41.210615 GrappyLfjv-0.0.17/src/GrappyLfjv.egg-info/
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     1395 2023-05-22 00:37:41.000000 GrappyLfjv-0.0.17/src/GrappyLfjv.egg-info/PKG-INFO
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      229 2023-05-22 00:37:41.000000 GrappyLfjv-0.0.17/src/GrappyLfjv.egg-info/SOURCES.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)        1 2023-05-22 00:37:41.000000 GrappyLfjv-0.0.17/src/GrappyLfjv.egg-info/dependency_links.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)       15 2023-05-22 00:37:41.000000 GrappyLfjv-0.0.17/src/GrappyLfjv.egg-info/requires.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)        7 2023-05-22 00:37:41.000000 GrappyLfjv-0.0.17/src/GrappyLfjv.egg-info/top_level.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     4085 2023-05-22 00:19:27.000000 GrappyLfjv-0.0.17/src/grappy.py
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:17:23.174525 GrappyLfjv-0.0.18/
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     1060 2023-05-16 15:35:17.000000 GrappyLfjv-0.0.18/LICENSE
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     3207 2023-05-22 07:17:23.174063 GrappyLfjv-0.0.18/PKG-INFO
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     3030 2023-05-22 07:17:05.000000 GrappyLfjv-0.0.18/README.md
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)       38 2023-05-22 07:17:23.174775 GrappyLfjv-0.0.18/setup.cfg
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)      606 2023-05-22 07:17:19.000000 GrappyLfjv-0.0.18/setup.py
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:17:23.170511 GrappyLfjv-0.0.18/src/
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:17:23.173375 GrappyLfjv-0.0.18/src/GrappyLfjv.egg-info/
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     3207 2023-05-22 07:17:23.000000 GrappyLfjv-0.0.18/src/GrappyLfjv.egg-info/PKG-INFO
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)      229 2023-05-22 07:17:23.000000 GrappyLfjv-0.0.18/src/GrappyLfjv.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)        1 2023-05-22 07:17:23.000000 GrappyLfjv-0.0.18/src/GrappyLfjv.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)       15 2023-05-22 07:17:23.000000 GrappyLfjv-0.0.18/src/GrappyLfjv.egg-info/requires.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)        7 2023-05-22 07:17:23.000000 GrappyLfjv-0.0.18/src/GrappyLfjv.egg-info/top_level.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     4085 2023-05-22 06:03:40.000000 GrappyLfjv-0.0.18/src/grappy.py
```

### Comparing `GrappyLfjv-0.0.17/LICENSE` & `GrappyLfjv-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `GrappyLfjv-0.0.17/setup.py` & `GrappyLfjv-0.0.18/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name= "GrappyLfjv",
-    version= "0.0.17",
+    version= "0.0.18",
     description= "Simplification de la création de graphiques avec matplotlib",
     long_description=read("README.md"),
     long_description_content_type='text/markdown',
     py_modules=["grappy"],
     package_dir={"": "src"},
     install_requires = [
         "matplotlib > 3.0"
```

### Comparing `GrappyLfjv-0.0.17/src/grappy.py` & `GrappyLfjv-0.0.18/src/grappy.py`

 * *Files identical despite different names*

