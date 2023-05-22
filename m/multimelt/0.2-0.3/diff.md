# Comparing `tmp/multimelt-0.2.tar.gz` & `tmp/multimelt-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimelt-0.2.tar", last modified: Mon May 22 12:48:48 2023, max compression
+gzip compressed data, was "multimelt-0.3.tar", last modified: Mon May 22 14:02:38 2023, max compression
```

## Comparing `multimelt-0.2.tar` & `multimelt-0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 burgardc (1776895) l-ige    (10377)        0 2023-05-22 12:48:48.787328 multimelt-0.2/
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)    35149 2021-08-22 11:07:21.000000 multimelt-0.2/LICENSE
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)     3362 2023-05-22 12:48:48.000000 multimelt-0.2/PKG-INFO
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)     2558 2023-05-22 10:11:02.000000 multimelt-0.2/README.rst
-drwxr-xr-x   0 burgardc (1776895) l-ige    (10377)        0 2023-05-22 12:48:48.583320 multimelt-0.2/multimelt/
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)    11422 2022-09-07 11:49:58.000000 multimelt-0.2/multimelt/T_S_profile_functions.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)        0 2021-08-22 11:09:31.000000 multimelt-0.2/multimelt/__init__.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)    16843 2023-05-22 10:08:17.000000 multimelt-0.2/multimelt/box_functions.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)     1890 2021-08-22 11:09:51.000000 multimelt-0.2/multimelt/constants.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)    71837 2023-05-22 12:20:40.000000 multimelt-0.2/multimelt/create_isf_mask_functions.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)    93979 2023-05-22 12:19:03.000000 multimelt-0.2/multimelt/melt_functions.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)    30434 2022-09-28 10:11:43.000000 multimelt-0.2/multimelt/plume_functions.py
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)     2302 2023-05-22 10:08:53.000000 multimelt-0.2/multimelt/useful_functions.py
-drwxr-xr-x   0 burgardc (1776895) l-ige    (10377)        0 2023-05-22 12:48:48.771327 multimelt-0.2/multimelt.egg-info/
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)     3362 2023-05-22 12:48:46.000000 multimelt-0.2/multimelt.egg-info/PKG-INFO
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)      424 2023-05-22 12:48:46.000000 multimelt-0.2/multimelt.egg-info/SOURCES.txt
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)        1 2023-05-22 12:48:46.000000 multimelt-0.2/multimelt.egg-info/dependency_links.txt
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)       52 2023-05-22 12:48:46.000000 multimelt-0.2/multimelt.egg-info/requires.txt
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)       10 2023-05-22 12:48:46.000000 multimelt-0.2/multimelt.egg-info/top_level.txt
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)       38 2023-05-22 12:48:48.000000 multimelt-0.2/setup.cfg
--rw-r--r--   0 burgardc (1776895) l-ige    (10377)     2530 2023-05-22 12:23:51.000000 multimelt-0.2/setup.py
+drwxr-xr-x   0 burgardc (1776895) l-ige    (10377)        0 2023-05-22 14:02:38.667634 multimelt-0.3/
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)    35149 2021-08-22 11:07:21.000000 multimelt-0.3/LICENSE
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)     3362 2023-05-22 14:02:38.000000 multimelt-0.3/PKG-INFO
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)     2558 2023-05-22 10:11:02.000000 multimelt-0.3/README.rst
+drwxr-xr-x   0 burgardc (1776895) l-ige    (10377)        0 2023-05-22 14:02:38.587631 multimelt-0.3/multimelt/
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)    11422 2022-09-07 11:49:58.000000 multimelt-0.3/multimelt/T_S_profile_functions.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)        0 2021-08-22 11:09:31.000000 multimelt-0.3/multimelt/__init__.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)    16843 2023-05-22 10:08:17.000000 multimelt-0.3/multimelt/box_functions.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)     1890 2021-08-22 11:09:51.000000 multimelt-0.3/multimelt/constants.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)    71837 2023-05-22 12:20:40.000000 multimelt-0.3/multimelt/create_isf_mask_functions.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)    93979 2023-05-22 12:19:03.000000 multimelt-0.3/multimelt/melt_functions.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)    30434 2022-09-28 10:11:43.000000 multimelt-0.3/multimelt/plume_functions.py
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)     2302 2023-05-22 10:08:53.000000 multimelt-0.3/multimelt/useful_functions.py
+drwxr-xr-x   0 burgardc (1776895) l-ige    (10377)        0 2023-05-22 14:02:38.651634 multimelt-0.3/multimelt.egg-info/
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)     3362 2023-05-22 14:02:38.000000 multimelt-0.3/multimelt.egg-info/PKG-INFO
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)      424 2023-05-22 14:02:38.000000 multimelt-0.3/multimelt.egg-info/SOURCES.txt
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)        1 2023-05-22 14:02:38.000000 multimelt-0.3/multimelt.egg-info/dependency_links.txt
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)       71 2023-05-22 14:02:38.000000 multimelt-0.3/multimelt.egg-info/requires.txt
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)       10 2023-05-22 14:02:38.000000 multimelt-0.3/multimelt.egg-info/top_level.txt
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)       38 2023-05-22 14:02:38.000000 multimelt-0.3/setup.cfg
+-rw-r--r--   0 burgardc (1776895) l-ige    (10377)     2549 2023-05-22 14:01:52.000000 multimelt-0.3/setup.py
```

### Comparing `multimelt-0.2/LICENSE` & `multimelt-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multimelt-0.2/PKG-INFO` & `multimelt-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimelt
-Version: 0.2
+Version: 0.3
 Summary: Regroupment of the main existing ice shelf basal melt parameterisations
 Home-page: https://github.com/ClimateClara/multimelt
 Author: Clara Burgard
 Author-email: clara.burgard@univ-grenoble-alpes.fr
 License: GPL-3.0
 Project-URL: Source, https://github.com/ClimateClara/multimelt
 Project-URL: Tracker, https://github.com/ClimateClara/multimelt/issues
```

### Comparing `multimelt-0.2/README.rst` & `multimelt-0.3/README.rst`

 * *Files identical despite different names*

### Comparing `multimelt-0.2/multimelt/T_S_profile_functions.py` & `multimelt-0.3/multimelt/T_S_profile_functions.py`

 * *Files identical despite different names*

### Comparing `multimelt-0.2/multimelt/box_functions.py` & `multimelt-0.3/multimelt/box_functions.py`

 * *Files identical despite different names*

### Comparing `multimelt-0.2/multimelt/constants.py` & `multimelt-0.3/multimelt/constants.py`

 * *Files identical despite different names*

### Comparing `multimelt-0.2/multimelt/create_isf_mask_functions.py` & `multimelt-0.3/multimelt/create_isf_mask_functions.py`

 * *Files identical despite different names*

### Comparing `multimelt-0.2/multimelt/melt_functions.py` & `multimelt-0.3/multimelt/melt_functions.py`

 * *Files identical despite different names*

### Comparing `multimelt-0.2/multimelt/plume_functions.py` & `multimelt-0.3/multimelt/plume_functions.py`

 * *Files identical despite different names*

### Comparing `multimelt-0.2/multimelt/useful_functions.py` & `multimelt-0.3/multimelt/useful_functions.py`

 * *Files identical despite different names*

### Comparing `multimelt-0.2/multimelt.egg-info/PKG-INFO` & `multimelt-0.3/multimelt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimelt
-Version: 0.2
+Version: 0.3
 Summary: Regroupment of the main existing ice shelf basal melt parameterisations
 Home-page: https://github.com/ClimateClara/multimelt
 Author: Clara Burgard
 Author-email: clara.burgard@univ-grenoble-alpes.fr
 License: GPL-3.0
 Project-URL: Source, https://github.com/ClimateClara/multimelt
 Project-URL: Tracker, https://github.com/ClimateClara/multimelt/issues
```

### Comparing `multimelt-0.2/setup.py` & `multimelt-0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 setuptools.setup(
 	
     #The project's name
     name='multimelt',
     
     #The project's version 
-    version='0.2',
+    version='0.3',
     
     #The project's metadata
     author='Clara Burgard',
     author_email='clara.burgard@univ-grenoble-alpes.fr',
     description='Regroupment of the main existing ice shelf basal melt parameterisations',
     long_description=long_description,
     
@@ -67,14 +67,14 @@
 	
     install_requires=[
           'numpy',
           'xarray',
           'pandas',
           'tqdm',
           'scipy',
-          'cc3d',
+          'connected-components-3d',
           'gsw',
           'pyproj',
           'dask',
       ],
 
 )
```

