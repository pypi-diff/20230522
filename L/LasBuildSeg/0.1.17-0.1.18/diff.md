# Comparing `tmp/LasBuildSeg-0.1.17.tar.gz` & `tmp/LasBuildSeg-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LasBuildSeg-0.1.17.tar", last modified: Mon May 22 16:09:25 2023, max compression
+gzip compressed data, was "LasBuildSeg-0.1.18.tar", last modified: Mon May 22 16:18:50 2023, max compression
```

## Comparing `LasBuildSeg-0.1.17.tar` & `LasBuildSeg-0.1.18.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:25.258629 LasBuildSeg-0.1.17/
--rw-rw-rw-   0        0        0      149 2023-05-22 16:07:49.000000 LasBuildSeg-0.1.17/CHANGELOG.txt
--rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.17/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:25.194850 LasBuildSeg-0.1.17/LasBuildSeg/
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:25.250656 LasBuildSeg-0.1.17/LasBuildSeg/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.17/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
--rw-rw-rw-   0        0        0    15758 2023-05-22 16:04:22.000000 LasBuildSeg-0.1.17/LasBuildSeg/LasBuildSeg.py
--rw-rw-rw-   0        0        0      519 2023-05-22 16:07:43.000000 LasBuildSeg-0.1.17/LasBuildSeg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:09:25.245674 LasBuildSeg-0.1.17/LasBuildSeg.egg-info/
--rw-rw-rw-   0        0        0     3062 2023-05-22 16:09:23.000000 LasBuildSeg-0.1.17/LasBuildSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-05-22 16:09:24.000000 LasBuildSeg-0.1.17/LasBuildSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:09:23.000000 LasBuildSeg-0.1.17/LasBuildSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-05-22 16:09:23.000000 LasBuildSeg-0.1.17/LasBuildSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-22 16:09:23.000000 LasBuildSeg-0.1.17/LasBuildSeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.17/MANIFEST.in
--rw-rw-rw-   0        0        0     3062 2023-05-22 16:09:25.256640 LasBuildSeg-0.1.17/PKG-INFO
--rw-rw-rw-   0        0        0     2132 2023-05-22 16:00:07.000000 LasBuildSeg-0.1.17/README.md
--rw-rw-rw-   0        0        0     1496 2023-05-22 16:07:53.000000 LasBuildSeg-0.1.17/Setup.py
--rw-rw-rw-   0        0        0      123 2023-05-17 11:16:46.000000 LasBuildSeg-0.1.17/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 16:09:25.259626 LasBuildSeg-0.1.17/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 16:18:50.019945 LasBuildSeg-0.1.18/
+-rw-rw-rw-   0        0        0      149 2023-05-22 16:18:25.000000 LasBuildSeg-0.1.18/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.18/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 16:18:49.960150 LasBuildSeg-0.1.18/LasBuildSeg/
+drwxrwxrwx   0        0        0        0 2023-05-22 16:18:50.012969 LasBuildSeg-0.1.18/LasBuildSeg/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.18/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
+-rw-rw-rw-   0        0        0    15751 2023-05-22 16:18:14.000000 LasBuildSeg-0.1.18/LasBuildSeg/LasBuildSeg.py
+-rw-rw-rw-   0        0        0      519 2023-05-22 16:07:43.000000 LasBuildSeg-0.1.18/LasBuildSeg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:18:50.007995 LasBuildSeg-0.1.18/LasBuildSeg.egg-info/
+-rw-rw-rw-   0        0        0     3062 2023-05-22 16:18:48.000000 LasBuildSeg-0.1.18/LasBuildSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-22 16:18:49.000000 LasBuildSeg-0.1.18/LasBuildSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:18:48.000000 LasBuildSeg-0.1.18/LasBuildSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-05-22 16:18:48.000000 LasBuildSeg-0.1.18/LasBuildSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-22 16:18:48.000000 LasBuildSeg-0.1.18/LasBuildSeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.18/MANIFEST.in
+-rw-rw-rw-   0        0        0     3062 2023-05-22 16:18:50.017952 LasBuildSeg-0.1.18/PKG-INFO
+-rw-rw-rw-   0        0        0     2132 2023-05-22 16:00:07.000000 LasBuildSeg-0.1.18/README.md
+-rw-rw-rw-   0        0        0     1496 2023-05-22 16:18:28.000000 LasBuildSeg-0.1.18/Setup.py
+-rw-rw-rw-   0        0        0      123 2023-05-17 11:16:46.000000 LasBuildSeg-0.1.18/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 16:18:50.020942 LasBuildSeg-0.1.18/setup.cfg
```

### Comparing `LasBuildSeg-0.1.17/LICENSE.txt` & `LasBuildSeg-0.1.18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.17/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py` & `LasBuildSeg-0.1.18/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.17/LasBuildSeg/LasBuildSeg.py` & `LasBuildSeg-0.1.18/LasBuildSeg/LasBuildSeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,15 @@
         rect = cv2.minAreaRect(contour)
         w, h = rect[1]
         if w < h:
             w, h = h, w
         squareness = w / h if h != 0 else 0
         size = w * h * pixel_size ** 2
 
-        # Compute the average TRI within the building contour
+        mask = np.zeros_like(img_open, dtype=np.uint8)
         cv2.drawContours(mask, [contour], -1, 1, -1)
 
         if squareness >= squareness_threshold and min_size <= size <= max_size and w >= width_threshold and h >= height_threshold:
             cv2.drawContours(building_mask, [contour], -1, 255, -1)
             
             
 def filter_contours(image, dem, profile, min_size=35, max_size=5000, squareness_threshold=0.3, width_threshold=3, height_threshold=3, tri_threshold=3):
```

### Comparing `LasBuildSeg-0.1.17/LasBuildSeg/__init__.py` & `LasBuildSeg-0.1.18/LasBuildSeg/__init__.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.17/LasBuildSeg.egg-info/PKG-INFO` & `LasBuildSeg-0.1.18/LasBuildSeg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.17
+Version: 0.1.18
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.1.17/PKG-INFO` & `LasBuildSeg-0.1.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.17
+Version: 0.1.18
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.1.17/README.md` & `LasBuildSeg-0.1.18/README.md`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.17/Setup.py` & `LasBuildSeg-0.1.18/Setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     INSTALL_REQUIRES = []
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
         
 setup(
   name='LasBuildSeg',
-  version='0.1.17',
+  version='0.1.18',
   description='Building Footrprint Extraction from Aerial LiDAR data',
   long_description=long_description,
   long_description_content_type='text/markdown',  
   url='',  
   author='MertcanErdem',
   author_email='merak908@gmail.com',
   license='GNU General Public License v2.0',
```

