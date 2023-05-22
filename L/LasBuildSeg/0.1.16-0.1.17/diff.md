# Comparing `tmp/LasBuildSeg-0.1.16.tar.gz` & `tmp/LasBuildSeg-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LasBuildSeg-0.1.16.tar", last modified: Mon May 22 16:05:27 2023, max compression
+gzip compressed data, was "LasBuildSeg-0.1.17.tar", last modified: Mon May 22 16:09:25 2023, max compression
```

## Comparing `LasBuildSeg-0.1.16.tar` & `LasBuildSeg-0.1.17.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:05:27.601095 LasBuildSeg-0.1.16/
--rw-rw-rw-   0        0        0      149 2023-05-22 16:03:38.000000 LasBuildSeg-0.1.16/CHANGELOG.txt
--rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.16/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 16:05:27.541293 LasBuildSeg-0.1.16/LasBuildSeg/
-drwxrwxrwx   0        0        0        0 2023-05-22 16:05:27.592125 LasBuildSeg-0.1.16/LasBuildSeg/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.16/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
--rw-rw-rw-   0        0        0    15758 2023-05-22 16:04:22.000000 LasBuildSeg-0.1.16/LasBuildSeg/LasBuildSeg.py
--rw-rw-rw-   0        0        0      519 2023-05-22 16:05:05.000000 LasBuildSeg-0.1.16/LasBuildSeg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:05:27.588142 LasBuildSeg-0.1.16/LasBuildSeg.egg-info/
--rw-rw-rw-   0        0        0     3062 2023-05-22 16:05:26.000000 LasBuildSeg-0.1.16/LasBuildSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-05-22 16:05:27.000000 LasBuildSeg-0.1.16/LasBuildSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:05:26.000000 LasBuildSeg-0.1.16/LasBuildSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-05-22 16:05:26.000000 LasBuildSeg-0.1.16/LasBuildSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-22 16:05:26.000000 LasBuildSeg-0.1.16/LasBuildSeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.16/MANIFEST.in
--rw-rw-rw-   0        0        0     3062 2023-05-22 16:05:27.598108 LasBuildSeg-0.1.16/PKG-INFO
--rw-rw-rw-   0        0        0     2132 2023-05-22 16:00:07.000000 LasBuildSeg-0.1.16/README.md
--rw-rw-rw-   0        0        0     1496 2023-05-22 16:03:41.000000 LasBuildSeg-0.1.16/Setup.py
--rw-rw-rw-   0        0        0      123 2023-05-17 11:16:46.000000 LasBuildSeg-0.1.16/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 16:05:27.601095 LasBuildSeg-0.1.16/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:25.258629 LasBuildSeg-0.1.17/
+-rw-rw-rw-   0        0        0      149 2023-05-22 16:07:49.000000 LasBuildSeg-0.1.17/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.17/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:25.194850 LasBuildSeg-0.1.17/LasBuildSeg/
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:25.250656 LasBuildSeg-0.1.17/LasBuildSeg/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.17/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
+-rw-rw-rw-   0        0        0    15758 2023-05-22 16:04:22.000000 LasBuildSeg-0.1.17/LasBuildSeg/LasBuildSeg.py
+-rw-rw-rw-   0        0        0      519 2023-05-22 16:07:43.000000 LasBuildSeg-0.1.17/LasBuildSeg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:09:25.245674 LasBuildSeg-0.1.17/LasBuildSeg.egg-info/
+-rw-rw-rw-   0        0        0     3062 2023-05-22 16:09:23.000000 LasBuildSeg-0.1.17/LasBuildSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-22 16:09:24.000000 LasBuildSeg-0.1.17/LasBuildSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:09:23.000000 LasBuildSeg-0.1.17/LasBuildSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-05-22 16:09:23.000000 LasBuildSeg-0.1.17/LasBuildSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-22 16:09:23.000000 LasBuildSeg-0.1.17/LasBuildSeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.17/MANIFEST.in
+-rw-rw-rw-   0        0        0     3062 2023-05-22 16:09:25.256640 LasBuildSeg-0.1.17/PKG-INFO
+-rw-rw-rw-   0        0        0     2132 2023-05-22 16:00:07.000000 LasBuildSeg-0.1.17/README.md
+-rw-rw-rw-   0        0        0     1496 2023-05-22 16:07:53.000000 LasBuildSeg-0.1.17/Setup.py
+-rw-rw-rw-   0        0        0      123 2023-05-17 11:16:46.000000 LasBuildSeg-0.1.17/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 16:09:25.259626 LasBuildSeg-0.1.17/setup.cfg
```

### Comparing `LasBuildSeg-0.1.16/LICENSE.txt` & `LasBuildSeg-0.1.17/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.16/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py` & `LasBuildSeg-0.1.17/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.16/LasBuildSeg/LasBuildSeg.py` & `LasBuildSeg-0.1.17/LasBuildSeg/LasBuildSeg.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.16/LasBuildSeg/__init__.py` & `LasBuildSeg-0.1.17/LasBuildSeg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,10 +4,10 @@
 from .LasBuildSeg import read_geotiff
 from .LasBuildSeg import to_8bit
 from .LasBuildSeg import threshold
 from .LasBuildSeg import morph_open
 from .LasBuildSeg import filter_contours
 from .LasBuildSeg import close
 from .LasBuildSeg import write_geotiff
-from .LasBuildSeg import DSM_Transform
+from .LasBuildSeg import DSM_transform
 from .LasBuildSeg import building_footprints_to_geojson
 from .LasBuildSeg import filter_contoursntri
```

### Comparing `LasBuildSeg-0.1.16/LasBuildSeg.egg-info/PKG-INFO` & `LasBuildSeg-0.1.17/LasBuildSeg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.16
+Version: 0.1.17
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.1.16/PKG-INFO` & `LasBuildSeg-0.1.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.16
+Version: 0.1.17
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.1.16/README.md` & `LasBuildSeg-0.1.17/README.md`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.16/Setup.py` & `LasBuildSeg-0.1.17/Setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     INSTALL_REQUIRES = []
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
         
 setup(
   name='LasBuildSeg',
-  version='0.1.16',
+  version='0.1.17',
   description='Building Footrprint Extraction from Aerial LiDAR data',
   long_description=long_description,
   long_description_content_type='text/markdown',  
   url='',  
   author='MertcanErdem',
   author_email='merak908@gmail.com',
   license='GNU General Public License v2.0',
```

