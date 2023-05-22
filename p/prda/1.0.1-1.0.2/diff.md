# Comparing `tmp/prda-1.0.1.tar.gz` & `tmp/prda-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prda-1.0.1.tar", last modified: Fri May  5 07:38:19 2023, max compression
+gzip compressed data, was "prda-1.0.2.tar", last modified: Mon May 22 08:06:29 2023, max compression
```

## Comparing `prda-1.0.1.tar` & `prda-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,19 @@
-drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-05-05 07:38:19.204540 prda-1.0.1/
--rw-r--r--   0 minshaojie   (501) staff       (20)     1068 2023-05-05 06:38:57.000000 prda-1.0.1/LICENSE
--rw-r--r--   0 minshaojie   (501) staff       (20)     1818 2023-05-05 07:38:19.204240 prda-1.0.1/PKG-INFO
-drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-05-05 07:38:19.204060 prda-1.0.1/prda.egg-info/
--rw-r--r--   0 minshaojie   (501) staff       (20)     1818 2023-05-05 07:38:19.000000 prda-1.0.1/prda.egg-info/PKG-INFO
--rw-r--r--   0 minshaojie   (501) staff       (20)      155 2023-05-05 07:38:19.000000 prda-1.0.1/prda.egg-info/SOURCES.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)        1 2023-05-05 07:38:19.000000 prda-1.0.1/prda.egg-info/dependency_links.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)       68 2023-05-05 07:38:19.000000 prda-1.0.1/prda.egg-info/requires.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)        1 2023-05-05 07:38:19.000000 prda-1.0.1/prda.egg-info/top_level.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)       38 2023-05-05 07:38:19.204585 prda-1.0.1/setup.cfg
--rw-r--r--   0 minshaojie   (501) staff       (20)      901 2023-05-05 07:38:11.000000 prda-1.0.1/setup.py
+drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-05-22 08:06:29.237162 prda-1.0.2/
+-rw-r--r--   0 minshaojie   (501) staff       (20)     1068 2023-05-05 06:38:57.000000 prda-1.0.2/LICENSE
+-rw-r--r--   0 minshaojie   (501) staff       (20)     1818 2023-05-22 08:06:29.236989 prda-1.0.2/PKG-INFO
+-rw-r--r--   0 minshaojie   (501) staff       (20)     2769 2023-05-07 14:06:10.000000 prda-1.0.2/README.md
+drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-05-22 08:06:29.235759 prda-1.0.2/prda/
+-rw-r--r--   0 minshaojie   (501) staff       (20)      108 2022-12-18 07:50:04.000000 prda-1.0.2/prda/__init__.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)    12932 2023-05-16 06:36:16.000000 prda-1.0.2/prda/graphic.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)      856 2023-05-05 07:16:05.000000 prda-1.0.2/prda/iostream.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)     7314 2023-05-03 13:03:18.000000 prda-1.0.2/prda/ml.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)     8779 2023-05-03 07:16:35.000000 prda-1.0.2/prda/prep.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)     3389 2022-12-03 12:39:17.000000 prda-1.0.2/prda/utility.py
+drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-05-22 08:06:29.236718 prda-1.0.2/prda.egg-info/
+-rw-r--r--   0 minshaojie   (501) staff       (20)     1818 2023-05-22 08:06:29.000000 prda-1.0.2/prda.egg-info/PKG-INFO
+-rw-r--r--   0 minshaojie   (501) staff       (20)      255 2023-05-22 08:06:29.000000 prda-1.0.2/prda.egg-info/SOURCES.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)        1 2023-05-22 08:06:29.000000 prda-1.0.2/prda.egg-info/dependency_links.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)       68 2023-05-22 08:06:29.000000 prda-1.0.2/prda.egg-info/requires.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)        5 2023-05-22 08:06:29.000000 prda-1.0.2/prda.egg-info/top_level.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)       38 2023-05-22 08:06:29.237210 prda-1.0.2/setup.cfg
+-rw-r--r--   0 minshaojie   (501) staff       (20)      901 2023-05-22 07:56:02.000000 prda-1.0.2/setup.py
```

### Comparing `prda-1.0.1/LICENSE` & `prda-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prda-1.0.1/PKG-INFO` & `prda-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prda
-Version: 1.0.1
+Version: 1.0.2
 Summary: Prda contains packages for data processing, analysis and visualization. The ultimate goal is to fill the “last mile” between analysts and packages.
 Home-page: https://github.com/4AlexMin/prda
 Author: Shaojie Min
 Author-email: alexmin@cqu.edu.cn
 License: MIT License
         
         Copyright (c) 2021 Shaojie Min
```

### Comparing `prda-1.0.1/prda.egg-info/PKG-INFO` & `prda-1.0.2/prda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prda
-Version: 1.0.1
+Version: 1.0.2
 Summary: Prda contains packages for data processing, analysis and visualization. The ultimate goal is to fill the “last mile” between analysts and packages.
 Home-page: https://github.com/4AlexMin/prda
 Author: Shaojie Min
 Author-email: alexmin@cqu.edu.cn
 License: MIT License
         
         Copyright (c) 2021 Shaojie Min
```

### Comparing `prda-1.0.1/setup.py` & `prda-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('LICENSE', 'r') as f:
     license = f.read()
 
 
 setup(
     name='prda',
-    version='1.0.1',
+    version='1.0.2',
     author='Shaojie Min',
     author_email='alexmin@cqu.edu.cn',
     description='Prda contains packages for data processing, analysis and visualization. The ultimate goal is to fill the “last mile” between analysts and packages.',
     url='https://github.com/4AlexMin/prda',
     license=license,
     packages=find_packages(),
     install_requires=[
```

