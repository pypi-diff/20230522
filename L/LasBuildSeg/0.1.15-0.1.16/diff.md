# Comparing `tmp/LasBuildSeg-0.1.15.tar.gz` & `tmp/LasBuildSeg-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LasBuildSeg-0.1.15.tar", last modified: Mon May 22 16:01:24 2023, max compression
+gzip compressed data, was "LasBuildSeg-0.1.16.tar", last modified: Mon May 22 16:05:27 2023, max compression
```

## Comparing `LasBuildSeg-0.1.15.tar` & `LasBuildSeg-0.1.16.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:01:24.215221 LasBuildSeg-0.1.15/
--rw-rw-rw-   0        0        0      149 2023-05-22 15:47:35.000000 LasBuildSeg-0.1.15/CHANGELOG.txt
--rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.15/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 16:01:24.106583 LasBuildSeg-0.1.15/LasBuildSeg/
-drwxrwxrwx   0        0        0        0 2023-05-22 16:01:24.209277 LasBuildSeg-0.1.15/LasBuildSeg/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.15/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
--rw-rw-rw-   0        0        0    15758 2023-05-22 15:46:19.000000 LasBuildSeg-0.1.15/LasBuildSeg/LasBuildSeg.py
--rw-rw-rw-   0        0        0      518 2023-05-17 08:50:32.000000 LasBuildSeg-0.1.15/LasBuildSeg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:01:24.182343 LasBuildSeg-0.1.15/LasBuildSeg.egg-info/
--rw-rw-rw-   0        0        0     3062 2023-05-22 16:01:22.000000 LasBuildSeg-0.1.15/LasBuildSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-05-22 16:01:23.000000 LasBuildSeg-0.1.15/LasBuildSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:01:22.000000 LasBuildSeg-0.1.15/LasBuildSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-05-22 16:01:22.000000 LasBuildSeg-0.1.15/LasBuildSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-22 16:01:22.000000 LasBuildSeg-0.1.15/LasBuildSeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.15/MANIFEST.in
--rw-rw-rw-   0        0        0     3062 2023-05-22 16:01:24.213228 LasBuildSeg-0.1.15/PKG-INFO
--rw-rw-rw-   0        0        0     2132 2023-05-22 16:00:07.000000 LasBuildSeg-0.1.15/README.md
--rw-rw-rw-   0        0        0     1496 2023-05-22 15:47:40.000000 LasBuildSeg-0.1.15/Setup.py
--rw-rw-rw-   0        0        0      123 2023-05-17 11:16:46.000000 LasBuildSeg-0.1.15/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 16:01:24.216218 LasBuildSeg-0.1.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 16:05:27.601095 LasBuildSeg-0.1.16/
+-rw-rw-rw-   0        0        0      149 2023-05-22 16:03:38.000000 LasBuildSeg-0.1.16/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.16/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 16:05:27.541293 LasBuildSeg-0.1.16/LasBuildSeg/
+drwxrwxrwx   0        0        0        0 2023-05-22 16:05:27.592125 LasBuildSeg-0.1.16/LasBuildSeg/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.16/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
+-rw-rw-rw-   0        0        0    15758 2023-05-22 16:04:22.000000 LasBuildSeg-0.1.16/LasBuildSeg/LasBuildSeg.py
+-rw-rw-rw-   0        0        0      519 2023-05-22 16:05:05.000000 LasBuildSeg-0.1.16/LasBuildSeg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:05:27.588142 LasBuildSeg-0.1.16/LasBuildSeg.egg-info/
+-rw-rw-rw-   0        0        0     3062 2023-05-22 16:05:26.000000 LasBuildSeg-0.1.16/LasBuildSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-22 16:05:27.000000 LasBuildSeg-0.1.16/LasBuildSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:05:26.000000 LasBuildSeg-0.1.16/LasBuildSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-05-22 16:05:26.000000 LasBuildSeg-0.1.16/LasBuildSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-22 16:05:26.000000 LasBuildSeg-0.1.16/LasBuildSeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.16/MANIFEST.in
+-rw-rw-rw-   0        0        0     3062 2023-05-22 16:05:27.598108 LasBuildSeg-0.1.16/PKG-INFO
+-rw-rw-rw-   0        0        0     2132 2023-05-22 16:00:07.000000 LasBuildSeg-0.1.16/README.md
+-rw-rw-rw-   0        0        0     1496 2023-05-22 16:03:41.000000 LasBuildSeg-0.1.16/Setup.py
+-rw-rw-rw-   0        0        0      123 2023-05-17 11:16:46.000000 LasBuildSeg-0.1.16/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 16:05:27.601095 LasBuildSeg-0.1.16/setup.cfg
```

### Comparing `LasBuildSeg-0.1.15/LICENSE.txt` & `LasBuildSeg-0.1.16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.15/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py` & `LasBuildSeg-0.1.16/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.15/LasBuildSeg/LasBuildSeg.py` & `LasBuildSeg-0.1.16/LasBuildSeg/LasBuildSeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     with rasterio.open(filename) as src:
         img = src.read(1)
         profile = src.profile.copy()
         profile.update({'crs': 'EPSG:3857'})
     return img, profile
 
 
-def dsm_transform(dsm_file):
+def DSM_transform(dsm_file):
     """
     Transform the DSM to the target CRS (EPSG:3857).
 
     Args:
         dsm_file (str): Path to the DSM file.
 
     Returns:
```

### Comparing `LasBuildSeg-0.1.15/LasBuildSeg/__init__.py` & `LasBuildSeg-0.1.16/LasBuildSeg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .LasBuildSeg import generate_dsm
 from .LasBuildSeg import generate_dtm
 from .LasBuildSeg import generate_ndhm
 from .LasBuildSeg import read_geotiff
 from .LasBuildSeg import to_8bit
 from .LasBuildSeg import threshold
-from .LasBuildSeg import morphopen
+from .LasBuildSeg import morph_open
 from .LasBuildSeg import filter_contours
 from .LasBuildSeg import close
 from .LasBuildSeg import write_geotiff
 from .LasBuildSeg import DSM_Transform
 from .LasBuildSeg import building_footprints_to_geojson
 from .LasBuildSeg import filter_contoursntri
```

### Comparing `LasBuildSeg-0.1.15/LasBuildSeg.egg-info/PKG-INFO` & `LasBuildSeg-0.1.16/LasBuildSeg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.15
+Version: 0.1.16
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.1.15/PKG-INFO` & `LasBuildSeg-0.1.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.15
+Version: 0.1.16
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.1.15/README.md` & `LasBuildSeg-0.1.16/README.md`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.15/Setup.py` & `LasBuildSeg-0.1.16/Setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     INSTALL_REQUIRES = []
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
         
 setup(
   name='LasBuildSeg',
-  version='0.1.15',
+  version='0.1.16',
   description='Building Footrprint Extraction from Aerial LiDAR data',
   long_description=long_description,
   long_description_content_type='text/markdown',  
   url='',  
   author='MertcanErdem',
   author_email='merak908@gmail.com',
   license='GNU General Public License v2.0',
```

