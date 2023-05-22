# Comparing `tmp/SFTB-1.0.tar.gz` & `tmp/SFTB-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SFTB-1.0.tar", last modified: Thu May 18 08:36:23 2023, max compression
+gzip compressed data, was "SFTB-1.1.tar", last modified: Mon May 22 01:42:18 2023, max compression
```

## Comparing `SFTB-1.0.tar` & `SFTB-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 08:36:23.877644 SFTB-1.0/
--rw-rw-rw-   0        0        0     1084 2023-05-18 07:11:00.000000 SFTB-1.0/LICENSE
--rw-rw-rw-   0        0        0    15272 2023-05-18 08:36:23.877644 SFTB-1.0/PKG-INFO
--rw-rw-rw-   0        0        0    14131 2023-05-18 08:35:29.000000 SFTB-1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-18 08:36:23.842869 SFTB-1.0/SFTB/
--rw-rw-rw-   0        0        0    19553 2023-05-18 06:44:07.000000 SFTB-1.0/SFTB/SFTB.py
--rw-rw-rw-   0        0        0        0 2023-05-18 06:45:09.000000 SFTB-1.0/SFTB/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:36:23.875902 SFTB-1.0/SFTB.egg-info/
--rw-rw-rw-   0        0        0    15272 2023-05-18 08:36:23.000000 SFTB-1.0/SFTB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-05-18 08:36:23.000000 SFTB-1.0/SFTB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 08:36:23.000000 SFTB-1.0/SFTB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-18 08:36:23.000000 SFTB-1.0/SFTB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-18 08:36:23.000000 SFTB-1.0/SFTB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 08:36:23.877644 SFTB-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1249 2023-05-18 07:29:09.000000 SFTB-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 01:42:18.926511 SFTB-1.1/
+-rw-rw-rw-   0        0        0     1084 2023-05-18 07:11:00.000000 SFTB-1.1/LICENSE
+-rw-rw-rw-   0        0        0    15272 2023-05-22 01:42:18.910885 SFTB-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14131 2023-05-18 08:35:29.000000 SFTB-1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-22 01:42:18.895258 SFTB-1.1/SFTB/
+-rw-rw-rw-   0        0        0    19553 2023-05-18 06:44:07.000000 SFTB-1.1/SFTB/SFTB.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:45:09.000000 SFTB-1.1/SFTB/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 01:42:18.910885 SFTB-1.1/SFTB.egg-info/
+-rw-rw-rw-   0        0        0    15272 2023-05-22 01:42:18.000000 SFTB-1.1/SFTB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-05-22 01:42:18.000000 SFTB-1.1/SFTB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 01:42:18.000000 SFTB-1.1/SFTB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-22 01:42:18.000000 SFTB-1.1/SFTB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-22 01:42:18.000000 SFTB-1.1/SFTB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 01:42:18.926511 SFTB-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1240 2023-05-22 01:41:10.000000 SFTB-1.1/setup.py
```

### Comparing `SFTB-1.0/LICENSE` & `SFTB-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SFTB-1.0/PKG-INFO` & `SFTB-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SFTB
-Version: 1.0
+Version: 1.1
 Summary: SFTB: A New Algorithm for Pairwise Comparison Data-based Ranking Solutions.
 Author: Y.C.Huang
 Author-email: 1950003@tongji.edu.cn
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `SFTB-1.0/README.rst` & `SFTB-1.1/README.rst`

 * *Files identical despite different names*

### Comparing `SFTB-1.0/SFTB/SFTB.py` & `SFTB-1.1/SFTB/SFTB.py`

 * *Files identical despite different names*

### Comparing `SFTB-1.0/SFTB.egg-info/PKG-INFO` & `SFTB-1.1/SFTB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SFTB
-Version: 1.0
+Version: 1.1
 Summary: SFTB: A New Algorithm for Pairwise Comparison Data-based Ranking Solutions.
 Author: Y.C.Huang
 Author-email: 1950003@tongji.edu.cn
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `SFTB-1.0/setup.py` & `SFTB-1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding='UTF-8') as f:
   long_description = f.read()
 
 setup(name='SFTB',  # 包名
-      version='1.0',  # 版本号
+      version='1.1',  # 版本号
       description='SFTB: A New Algorithm for Pairwise Comparison Data-based Ranking Solutions.',
       long_description=long_description,
       author='Y.C.Huang',
       author_email='1950003@tongji.edu.cn',
-      install_requires=['numpy','pandas','matplotlib','random','scipy'],
+      install_requires=['numpy','pandas','matplotlib','scipy'],
       license='MIT License',
       packages=find_packages(),
       platforms=["all"],
       classifiers=[
           'Intended Audience :: Developers',
           'Operating System :: OS Independent',
           'Natural Language :: Chinese (Simplified)',
```

