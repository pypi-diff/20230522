# Comparing `tmp/fedops-0.1.0.tar.gz` & `tmp/fedops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedops-0.1.0.tar", last modified: Fri May 19 13:02:48 2023, max compression
+gzip compressed data, was "fedops-0.1.1.tar", last modified: Mon May 22 16:52:57 2023, max compression
```

## Comparing `fedops-0.1.0.tar` & `fedops-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,35 @@
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-19 13:02:48.872477 fedops-0.1.0/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-19 13:02:48.872350 fedops-0.1.0/PKG-INFO
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-19 13:02:48.872184 fedops-0.1.0/fedops.egg-info/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-19 13:02:48.000000 fedops-0.1.0/fedops.egg-info/PKG-INFO
--rw-r--r--   0 yangsemo   (501) staff       (20)      157 2023-05-19 13:02:48.000000 fedops-0.1.0/fedops.egg-info/SOURCES.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-19 13:02:48.000000 fedops-0.1.0/fedops.egg-info/dependency_links.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-19 13:02:48.000000 fedops-0.1.0/fedops.egg-info/requires.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-19 13:02:48.000000 fedops-0.1.0/fedops.egg-info/top_level.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-19 13:02:48.872513 fedops-0.1.0/setup.cfg
--rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-19 12:47:12.000000 fedops-0.1.0/setup.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-22 16:52:57.155953 fedops-0.1.1/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-22 16:52:57.155785 fedops-0.1.1/PKG-INFO
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-22 16:52:57.149075 fedops-0.1.1/fedops/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-22 16:52:45.000000 fedops-0.1.1/fedops/__init__.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-22 16:52:57.153454 fedops-0.1.1/fedops/client/
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1129 2023-05-22 16:03:54.000000 fedops-0.1.1/fedops/client/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     7003 2023-05-22 16:00:57.000000 fedops-0.1.1/fedops/client/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 04:50:21.000000 fedops-0.1.1/fedops/client/app_test.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2809 2023-05-18 10:47:23.000000 fedops-0.1.1/fedops/client/client_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)    12517 2023-05-18 10:32:47.000000 fedops-0.1.1/fedops/client/client_data.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     6073 2023-05-19 05:35:33.000000 fedops-0.1.1/fedops/client/client_fl.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2909 2023-05-18 08:14:34.000000 fedops-0.1.1/fedops/client/client_model.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2059 2023-05-22 15:51:31.000000 fedops-0.1.1/fedops/client/client_task.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1614 2023-05-22 04:50:40.000000 fedops-0.1.1/fedops/client/client_task_copy.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3571 2023-05-22 15:54:13.000000 fedops-0.1.1/fedops/client/client_utils.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2230 2023-05-22 11:55:10.000000 fedops-0.1.1/fedops/client/client_wandb.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 04:17:43.000000 fedops-0.1.1/fedops/client/test.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-22 16:52:57.155115 fedops-0.1.1/fedops/server/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      868 2023-05-22 16:40:03.000000 fedops-0.1.1/fedops/server/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     8967 2023-05-22 16:31:47.000000 fedops-0.1.1/fedops/server/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2909 2023-05-18 12:01:35.000000 fedops-0.1.1/fedops/server/init_gl_model.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-19 06:37:19.000000 fedops-0.1.1/fedops/server/server_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2209 2023-05-22 16:31:47.000000 fedops-0.1.1/fedops/server/server_task.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3715 2023-05-19 07:54:45.000000 fedops-0.1.1/fedops/server/server_utils.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-22 16:52:57.155419 fedops-0.1.1/fedops/utils/
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 03:47:38.000000 fedops-0.1.1/fedops/utils/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 03:48:03.000000 fedops-0.1.1/fedops/utils/version.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-22 16:52:57.149934 fedops-0.1.1/fedops.egg-info/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-22 16:52:57.000000 fedops-0.1.1/fedops.egg-info/PKG-INFO
+-rw-r--r--   0 yangsemo   (501) staff       (20)      722 2023-05-22 16:52:57.000000 fedops-0.1.1/fedops.egg-info/SOURCES.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-22 16:52:57.000000 fedops-0.1.1/fedops.egg-info/dependency_links.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-22 16:52:57.000000 fedops-0.1.1/fedops.egg-info/requires.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-22 16:52:57.000000 fedops-0.1.1/fedops.egg-info/top_level.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-22 16:52:57.155996 fedops-0.1.1/setup.cfg
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-22 16:52:45.000000 fedops-0.1.1/setup.py
```

### Comparing `fedops-0.1.0/PKG-INFO` & `fedops-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.0
+Version: 0.1.1
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.0/fedops.egg-info/PKG-INFO` & `fedops-0.1.1/fedops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.0
+Version: 0.1.1
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.0/setup.py` & `fedops-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fedops',
-    version='0.1.0',
+    version='0.1.1',
     author='Semo Yang',
     author_email='tpah20@gmail.com',
     description='FL Lifecycle Operations Management Platform',
     long_description='Long description of your library',
     url='https://github.com/gachon-CCLab/FedOps.git',
     packages=find_packages(),
     install_requires=[
```

