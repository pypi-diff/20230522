# Comparing `tmp/LasBuildSeg-0.1.14.tar.gz` & `tmp/LasBuildSeg-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LasBuildSeg-0.1.14.tar", last modified: Thu May 18 08:16:04 2023, max compression
+gzip compressed data, was "LasBuildSeg-0.1.15.tar", last modified: Mon May 22 16:01:24 2023, max compression
```

## Comparing `LasBuildSeg-0.1.14.tar` & `LasBuildSeg-0.1.15.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 08:16:04.062588 LasBuildSeg-0.1.14/
--rw-rw-rw-   0        0        0      107 2023-05-18 08:14:14.000000 LasBuildSeg-0.1.14/CHANGELOG.txt
--rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.14/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 08:16:04.004055 LasBuildSeg-0.1.14/LasBuildSeg/
-drwxrwxrwx   0        0        0        0 2023-05-18 08:16:04.058646 LasBuildSeg-0.1.14/LasBuildSeg/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.14/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
--rw-rw-rw-   0        0        0    14829 2023-05-18 08:14:10.000000 LasBuildSeg-0.1.14/LasBuildSeg/LasBuildSeg.py
--rw-rw-rw-   0        0        0      518 2023-05-17 08:50:32.000000 LasBuildSeg-0.1.14/LasBuildSeg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:16:04.042851 LasBuildSeg-0.1.14/LasBuildSeg.egg-info/
--rw-rw-rw-   0        0        0     2448 2023-05-18 08:16:03.000000 LasBuildSeg-0.1.14/LasBuildSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-05-18 08:16:03.000000 LasBuildSeg-0.1.14/LasBuildSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 08:16:03.000000 LasBuildSeg-0.1.14/LasBuildSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-05-18 08:16:03.000000 LasBuildSeg-0.1.14/LasBuildSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-18 08:16:03.000000 LasBuildSeg-0.1.14/LasBuildSeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.14/MANIFEST.in
--rw-rw-rw-   0        0        0     2448 2023-05-18 08:16:04.060593 LasBuildSeg-0.1.14/PKG-INFO
--rw-rw-rw-   0        0        0     1516 2023-05-17 20:10:13.000000 LasBuildSeg-0.1.14/README.md
--rw-rw-rw-   0        0        0     1496 2023-05-18 08:15:18.000000 LasBuildSeg-0.1.14/Setup.py
--rw-rw-rw-   0        0        0      123 2023-05-17 11:16:46.000000 LasBuildSeg-0.1.14/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 08:16:04.062588 LasBuildSeg-0.1.14/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 16:01:24.215221 LasBuildSeg-0.1.15/
+-rw-rw-rw-   0        0        0      149 2023-05-22 15:47:35.000000 LasBuildSeg-0.1.15/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.15/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 16:01:24.106583 LasBuildSeg-0.1.15/LasBuildSeg/
+drwxrwxrwx   0        0        0        0 2023-05-22 16:01:24.209277 LasBuildSeg-0.1.15/LasBuildSeg/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.15/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
+-rw-rw-rw-   0        0        0    15758 2023-05-22 15:46:19.000000 LasBuildSeg-0.1.15/LasBuildSeg/LasBuildSeg.py
+-rw-rw-rw-   0        0        0      518 2023-05-17 08:50:32.000000 LasBuildSeg-0.1.15/LasBuildSeg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:01:24.182343 LasBuildSeg-0.1.15/LasBuildSeg.egg-info/
+-rw-rw-rw-   0        0        0     3062 2023-05-22 16:01:22.000000 LasBuildSeg-0.1.15/LasBuildSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-22 16:01:23.000000 LasBuildSeg-0.1.15/LasBuildSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:01:22.000000 LasBuildSeg-0.1.15/LasBuildSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-05-22 16:01:22.000000 LasBuildSeg-0.1.15/LasBuildSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-22 16:01:22.000000 LasBuildSeg-0.1.15/LasBuildSeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.15/MANIFEST.in
+-rw-rw-rw-   0        0        0     3062 2023-05-22 16:01:24.213228 LasBuildSeg-0.1.15/PKG-INFO
+-rw-rw-rw-   0        0        0     2132 2023-05-22 16:00:07.000000 LasBuildSeg-0.1.15/README.md
+-rw-rw-rw-   0        0        0     1496 2023-05-22 15:47:40.000000 LasBuildSeg-0.1.15/Setup.py
+-rw-rw-rw-   0        0        0      123 2023-05-17 11:16:46.000000 LasBuildSeg-0.1.15/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 16:01:24.216218 LasBuildSeg-0.1.15/setup.cfg
```

### Comparing `LasBuildSeg-0.1.14/LICENSE.txt` & `LasBuildSeg-0.1.15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.14/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py` & `LasBuildSeg-0.1.15/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.14/LasBuildSeg/LasBuildSeg.py` & `LasBuildSeg-0.1.15/LasBuildSeg/LasBuildSeg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,112 +1,101 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Sun May 7 10:46:30 2023
-
-
-@author: Mertcan
-"""
-
 import laspy
 import numpy as np
-from scipy.interpolate import griddata
 import rasterio
 import pyproj
 import cv2
-from rasterio.transform import from_origin
 import scipy
+from scipy.interpolate import griddata
+from rasterio.transform import from_origin
+import scipy.spatial
 from rasterio.warp import calculate_default_transform, reproject, Resampling
-from rasterio.plot import show
 from rasterio.mask import mask
 import rasterio.features
 from shapely.geometry import shape, mapping
 import json
-from shapely.geometry import Polygon, MultiPolygon
-
 
-def generate_dsm(las_file_name: str, input_epsg: int, resolution, intermethod: str, scale):
+def generate_dsm(las_file_path: str, input_epsg: int, interpolation_method: str):
+    """
+    Generate a Digital Surface Model (DSM) from a LAS file.
+
+    Args:
+        las_file_path (str): Path to the LAS file.
+        input_epsg (int): EPSG code of the input coordinate reference system (CRS).
+        interpolation_method (str): Interpolation method to use.
+
+    Outputs:
+        dsm.tif the output DSM file.
+    """
     # Read the LAS file
-    las_file = laspy.read(las_file_name)
-
-    # Set the CRS information to projection
-    las_file.header.scale[0] = scale
-    las_file.header.scale[1] = scale
-    las_file.header.scale[2] = scale
-
-    # Write the updated LAS file
-    las_file.write("updated_file.las")
-
-    # Read the updated LAS file
-    las_file = laspy.read('updated_file.las')
+    las_file = laspy.read(las_file_path)
+    resolution = 1
 
     # Create a Pyproj CRS object for the input EPSG code
     input_crs = pyproj.CRS.from_epsg(input_epsg)
-    
+
     # Extract the x, y, and z coordinates from the LAS file
     x = las_file.x
     y = las_file.y
     z = las_file.z
 
     # Calculate the grid bounds based on the x and y coordinates
     x_min = np.floor(min(x))
     x_max = np.ceil(max(x))
     y_min = np.floor(min(y))
     y_max = np.ceil(max(y))
 
     # Generate the grid of points for the DSM
-    grid_x, grid_y = np.meshgrid(np.arange(x_min, x_max , resolution), np.arange(y_min, y_max , resolution))
+    grid_x, grid_y = np.meshgrid(np.arange(x_min, x_max, resolution), np.arange(y_min, y_max, resolution))
 
-    # Generate the DSM using Nearest Neighbor interpolation of the point cloud
-    dsm = griddata((x, y), z, (grid_x, grid_y), method=intermethod)
+    # Generate the DSM using the specified interpolation method
+    dsm = griddata((x, y), z, (grid_x, grid_y), method=interpolation_method)
 
     # Save the DSM to a GeoTIFF file using rasterio
     with rasterio.open("dsm.tif", 'w', driver='GTiff', height=dsm.shape[0], width=dsm.shape[1], count=1, 
                        dtype=dsm.dtype, crs=input_crs, transform=rasterio.transform.Affine(resolution, 0, x_min, 0, resolution, y_min)) as dst:
         dst.write(dsm, 1)
     
     print('Success in Creating DSM')
-#generate_dsm('Yourdata.laz', 8734, 1)
 
 
 
-def generate_dtm(las_file_path, input_epsg, resolution, intermethod,scale):
-    # Load LiDAR data
-    las_file_dtm = laspy.read(las_file_path)
-     # Set the CRS information to projection
-    las_file_dtm.header.scale[0] = scale
-    las_file_dtm.header.scale[1] = scale
-    las_file_dtm.header.scale[2] = scale
 
-    # Write the updated LAS file
-    las_file_dtm.write("updated_file.las")
+def generate_dtm(las_file_path, input_epsg, interpolation_method, ground_multiplier):
+    """
+    Generate a Digital Terrain Model (DTM) from LiDAR data (This is not a %100 accurate DSM but it enchances
+                                                            the resualts of the building extraction.)
+
+    Args:
+        las_file_path (str): Path to the LAS file.
+        input_epsg (int): EPSG code of the input coordinate reference system.
+        interpolation_method (str): Interpolation method for non-ground points.
+        ground_multiplier (float): Multiplier for ground values in the DTM for contrast ecnheament.
+
+    Returns:
+        dtm.tif the output DSM file
+    """
 
-    # Read the updated LAS file
-    las_file_dtm = laspy.read('updated_file.las')
+    # Load LiDAR data
+    las_data = laspy.read(las_file_path)
+
+    # Set the desired resolution
+    resolution = 1
 
     # Create a Pyproj CRS object for the input EPSG code
     input_crs = pyproj.CRS.from_epsg(input_epsg) 
 
-    points = np.vstack((las_file_dtm.x, las_file_dtm.y, las_file_dtm.z)).T
-    
-    # Extract the x, y, and z coordinates from the LAS file
-    # xdtm = las_file_dtm.x
-    # ydtm = las_file_dtm.y
-     
-    # # Calculate the grid bounds based on the x and y coordinates
-    # min_x = np.floor(min(xdtm))
-    # max_x = np.ceil(max(xdtm))
-    # min_y = np.floor(min(ydtm))
-    # max_y = np.ceil(max(ydtm))
-    
+    # Extract x, y, and z coordinates from the LiDAR data
+    points = np.vstack((las_data.x, las_data.y, las_data.z)).T
     
     # Determine the bounds of the point cloud
-    min_x, max_x = np.min(points[:,0]), np.max(points[:,0])
-    min_y, max_y = np.min(points[:,1]), np.max(points[:,1])
-    # Classify ground points in lidar data class 2
-    ground_points = points[las_file_dtm.classification == 2]
+    min_x, max_x = np.min(points[:, 0]), np.max(points[:, 0])
+    min_y, max_y = np.min(points[:, 1]), np.max(points[:, 1])
+
+    # Classify ground points in the LiDAR data (class 2)
+    ground_points = points[las_data.classification == 2]
 
     # Calculate the size of the output raster
     width = int(np.ceil((max_x - min_x) / resolution))
     height = int(np.ceil((max_y - min_y) / resolution))
 
     # Create the output raster profile
     profile = {
@@ -119,68 +108,71 @@
         'transform': from_origin(min_x, min_y, resolution, -resolution)
     }
 
     # Create an empty numpy array for the output DTM
     dtm = np.zeros((height, width), dtype=np.float32)
 
     # Create a KDTree from the x, y coordinates of the ground points
-    tree = scipy.spatial.cKDTree(ground_points[:, :2])
+    ground_tree = scipy.spatial.cKDTree(ground_points[:, :2])
 
     # Create a mesh grid for the output raster
     mesh_x, mesh_y = np.meshgrid(np.arange(min_x, max_x, resolution), np.arange(min_y, max_y, resolution))
 
     # Interpolate the z values of the ground points onto the mesh grid
-    values = tree.query(np.vstack((mesh_x.ravel(), mesh_y.ravel())).T)[0]
-    mesh_z = values.reshape(mesh_x.shape)
-
+    ground_values = ground_tree.query(np.vstack((mesh_x.ravel(), mesh_y.ravel())).T)[0]
+    mesh_z = ground_values.reshape(mesh_x.shape)
 
     # Load the point cloud
-    dsm_file = laspy.read('updated_file.las')
-    dsm_points = np.vstack((dsm_file.x, dsm_file.y, dsm_file.z)).T
+    dsm_data = laspy.read('updated_file.las')
+    dsm_points = np.vstack((dsm_data.x, dsm_data.y, dsm_data.z)).T
 
-    # Classify points as aboveground features (non-ground points)
-    non_ground_points = dsm_points[dsm_file.classification != 2]
+    # Classify points as non-ground (not class 2)
+    non_ground_points = dsm_points[dsm_data.classification != 2]
 
     # Interpolate the non-ground points onto the mesh grid
-    non_ground_z = griddata(non_ground_points[:, :2], non_ground_points[:, 2], (mesh_x, mesh_y), method=intermethod)
+    non_ground_z = griddata(non_ground_points[:, :2], non_ground_points[:, 2], (mesh_x, mesh_y), method=interpolation_method)
 
-    # Subtract the interpolated non-ground values from the interpolated ground values
-    dtm = 10*mesh_z - non_ground_z
+    # Subtract the interpolated non-ground values from the interpolated ground values also enhancge the contrast by using ground_multiplier
+    dtm = ground_multiplier * mesh_z - non_ground_z
 
     # Write the output raster to a file
     with rasterio.open('dtm.tif', 'w', **profile) as dst:
         dst.write(dtm, 1)
-#generate_dtm('Yourdata.laz', EPSG, Resulation)
-
+    print('Success in Creating DTM')
 
 
 
+def generate_ndhm(dtm_file, dsm_file):
+    """
+    Generate the Normalized Digital Height Model (NDHM) by subtracting the Digital Terrain Model (DTM) from the Digital Surface Model (DSM).
 
-#DTM and DSM need to be in same resulation
-import rasterio
-from rasterio.warp import calculate_default_transform, reproject, Resampling
+    Args:
+        dtm_file (str): Path to the DTM file.
+        dsm_file (str): Path to the DSM file.
+
+    Returns:
+       ndhm.tiff output NDHM file
+    """
 
-#DTM and DSM need to be in same resulation
-def generate_ndhm(dtm_file, dsm_file):
     # Load DSM and DTM
-    with rasterio.open(dsm_file) as src:
-        dsm = src.read(1)
-        dsm_meta = src.profile
+    with rasterio.open(dsm_file) as dsm_src:
+        dsm = dsm_src.read(1)
+        dsm_meta = dsm_src.profile
 
-    with rasterio.open(dtm_file) as src:
-        dtm = src.read(1)
+    with rasterio.open(dtm_file) as dtm_src:
+        dtm = dtm_src.read(1)
 
     # Compute NDHM
     ndhm = dsm - dtm
 
     # Write NDHM to file
     ndhm_meta = dsm_meta.copy()
     ndhm_meta['dtype'] = 'float32'
-    with rasterio.open('ndhmtemp.tif', 'w', **ndhm_meta) as dst:
-        dst.write(ndhm.astype(np.float32), 1)
+    with rasterio.open('ndhmtemp.tif', 'w', **ndhm_meta) as ndhm_dst:
+        ndhm_dst.write(ndhm.astype(np.float32), 1)
 
     # Define the target CRS as EPSG:3857
     target_crs = 'EPSG:3857'
 
     # Open the input file
     with rasterio.open('ndhmtemp.tif') as src:
         # Get the metadata of the input file
@@ -207,190 +199,243 @@
                 src_transform=src.transform,
                 src_crs=src.crs,
                 dst_transform=dst_transform,
                 dst_crs=target_crs,
                 resampling=Resampling.nearest,
                 dst_nodata=0)
 
+        print('Success in Creating NDHM')
 
-#Our algorithms
 
 
 def read_geotiff(filename):
+    """
+    Read a geotiff file and return the image data and profile.
+
+    Args:
+        filename (str): Path to the geotiff file.
+
+    Returns:
+        tuple: A tuple with two values - the image data and a dictionary with metadata about the image.
+    """
     with rasterio.open(filename) as src:
         img = src.read(1)
         profile = src.profile.copy()
-        profile.update({
-            'crs': 'EPSG:3857'})
+        profile.update({'crs': 'EPSG:3857'})
     return img, profile
 
-# This function reads a geotiff file and returns the image and profile data.
-# filename: the path to the geotiff file
-# Returns a tuple with two values: the image data and a dictionary with metadata about the image.
-def DSM_Transform(DSM):
+
+def dsm_transform(dsm_file):
+    """
+    Transform the DSM to the target CRS (EPSG:3857).
+
+    Args:
+        dsm_file (str): Path to the DSM file.
+
+    Returns:
+        dsm3857.tiff: This image is a corrdinate trasnformed DSM file
+    """
     target_crs = 'EPSG:3857'
 
-    with rasterio.open(DSM) as src:
-        # Get the metadata of the input file
+    with rasterio.open(dsm_file) as src:
         src_profile = src.profile.copy()
-
-        # Calculate the transform to the target CRS
         dst_transform, dst_width, dst_height = calculate_default_transform(
             src.crs, target_crs, src.width, src.height, *src.bounds)
 
-        # Update the metadata of the output file with the target CRS and nodata value
         src_profile.update({
             'crs': target_crs,
             'transform': dst_transform,
             'width': dst_width,
             'height': dst_height,
             'nodata': 0})
 
-        # Create the output file
         with rasterio.open('dsm3857.tif', 'w', **src_profile) as dst:
-            # Reproject the input file to the target CRS
             reproject(
                 source=rasterio.band(src, 1),
                 destination=rasterio.band(dst, 1),
                 src_transform=src.transform,
                 src_crs=src.crs,
                 dst_transform=dst_transform,
                 dst_crs=target_crs,
                 resampling=Resampling.nearest,
                 dst_nodata=0)
 
-# This function converts an image to 8-bit color depth.
-# img: the image data
-# Returns the image data converted to 8-bit color depth.    
-def to_8bit(img):
-    img_8bit = cv2.normalize(img, None, 0, 255, cv2.NORM_MINMAX, cv2.CV_8UC1)
-    return img_8bit
-
-
-# This function applies an adaptive threshold to an image to separate objects from the background.
-# img_8bit: the 8-bit image data
-# block_size: the size of the neighborhood used to calculate the threshold value
-# constant: a value subtracted from the calculated threshold value
-# Returns a binary image where objects are white and the background is black.
-def threshold(img_8bit, block_size=51, constant=4.6):
-    img_thresh = cv2.adaptiveThreshold(img_8bit, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, block_size, constant)
-    return img_thresh
-
-
-# This function applies a morphological opening to an image to remove small objects.
-# img_thresh: the binary image data
-# kernel_size: the size of the kernel used for the morphological operation
-# Returns the image data with small objects removed.
-def morphopen(img_thresh, kernel_size=3):
-    kernel = np.ones((kernel_size, kernel_size), np.uint8)
-    img_open = cv2.morphologyEx(img_thresh, cv2.MORPH_OPEN, kernel)
-    return img_open
-
-
 
+def to_8bit(image):
+    """
+    Convert an image to 8-bit color depth.
+
+    Args:
+        image: The image data.
+
+    Returns:
+        numpy.ndarray: The image data converted to 8-bit color depth.
+    """
+    image_8bit = cv2.normalize(image, None, 0, 255, cv2.NORM_MINMAX, cv2.CV_8UC1)
+    return image_8bit
+
+
+def threshold(image, block_size=51, constant=4.6):
+    """
+    Apply an adaptive threshold to an image to separate objects from the background.
+
+    Args:
+        image: The 8-bit image data.
+        block_size (int): The size of the neighborhood used to calculate the threshold value.
+        constant (float): A value subtracted from the calculated threshold value.
+
+    Returns:
+        numpy.ndarray: A binary image where objects are white and the background is black.
+    """
+    image_thresh = cv2.adaptiveThreshold(image, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, block_size, constant)
+    return image_thresh
+
+
+def morph_open(image, kernel_size=3):
+    """
+    Apply a morphological opening to an image to remove small objects.
+
+    Args:
+        image: The binary image data.
+        kernel_size (int): The size of the kernel used for the morphological operation.
+
+    Returns:
+        numpy.ndarray: The image data with small objects removed.
+    """
+    kernel = np.ones((kernel_size, kernel_size), np.uint8)
+    image_open = cv2.morphologyEx(image, cv2.MORPH_OPEN, kernel)
+    return image_open
 
-#No tri only for testing purposes
 def filter_contoursntri(img_open, profile, min_size=35, max_size=5000, squareness_threshold=0.3, width_threshold=3, height_threshold=3):
-    
+    """
+    This section is only used for testing purposes so we can see the change between using the method of TRI and no TRI
+
+    """
     contours, _ = cv2.findContours(img_open.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
     pixel_size = abs(profile['transform'][0])
     building_mask = np.zeros_like(img_open, dtype=np.uint8)
 
 
     for contour in contours:
         rect = cv2.minAreaRect(contour)
         w, h = rect[1]
         if w < h:
             w, h = h, w
         squareness = w / h if h != 0 else 0
         size = w * h * pixel_size ** 2
 
         # Compute the average TRI within the building contour
-        mask = np.zeros_like(img_open, dtype=np.uint8)
         cv2.drawContours(mask, [contour], -1, 1, -1)
 
         if squareness >= squareness_threshold and min_size <= size <= max_size and w >= width_threshold and h >= height_threshold:
             cv2.drawContours(building_mask, [contour], -1, 255, -1)
-
-    return building_mask
-
-
-
-# This function filters out contours that do not meet certain criteria (size, shape, etc.) and creates a binary mask of the remaining objects.
-# img_open: the image data with small objects removed
-# profile: a dictionary with metadata about the image
-# min_size: the minimum size of objects to keep
-# max_size: the maximum size of objects to keep
-# squareness_threshold: the minimum squareness of objects to keep (ratio of width to height)
-# width_threshold: the minimum width of objects to keep
-# height_threshold: the minimum height of objects to keep
-# Returns a binary mask where the objects to keep are white and the rest is black.
-def filter_contours(img_open, dem, profile, min_size=35, max_size=5000, squareness_threshold=0.3, width_threshold=3, height_threshold=3, tri_threshold=3):
-    
-    contours, _ = cv2.findContours(img_open.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+            
+            
+def filter_contours(image, dem, profile, min_size=35, max_size=5000, squareness_threshold=0.3, width_threshold=3, height_threshold=3, tri_threshold=3):
+    """
+    Filter out contours that do not meet certain criteria and create a binary mask of the remaining objects.
+
+    Args:
+        image: The image data with small objects removed.
+        dem: The Digital Elevation Model data.
+        profile: A dictionary with metadata about the image.
+        min_size (int): The minimum size of objects to keep.
+        max_size (int): The maximum size of objects to keep.
+        squareness_threshold (float): The minimum squareness of objects to keep (ratio of width to height).
+        width_threshold (int): The minimum width of objects to keep.
+        height_threshold (int): The minimum height of objects to keep.
+        tri_threshold (float): The maximum Terrain Ruggedness Index (TRI) value to keep.
+
+    Returns:
+        numpy.ndarray: A binary mask where the objects to keep are white and the rest is black.
+    """
+    contours, _ = cv2.findContours(image.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
     pixel_size = abs(profile['transform'][0])
-    building_mask = np.zeros_like(img_open, dtype=np.uint8)
-
-    # Compute the Terrain Ruggedness Index (TRI) from the DEM
+    building_mask = np.zeros_like(image, dtype=np.uint8)
     dx, dy = np.gradient(dem)
     tri = np.sqrt(dx**2 + dy**2)
     tri /= pixel_size
 
     for contour in contours:
         rect = cv2.minAreaRect(contour)
         w, h = rect[1]
         if w < h:
             w, h = h, w
         squareness = w / h if h != 0 else 0
         size = w * h * pixel_size ** 2
 
-        # Compute the average TRI within the building contour
-        mask = np.zeros_like(img_open, dtype=np.uint8)
+        mask = np.zeros_like(image, dtype=np.uint8)
         cv2.drawContours(mask, [contour], -1, 1, -1)
         tri_values = tri[mask == 1]
         tri_mean = np.mean(tri_values)
 
         if squareness >= squareness_threshold and min_size <= size <= max_size and w >= width_threshold and h >= height_threshold and tri_mean <= tri_threshold:
             cv2.drawContours(building_mask, [contour], -1, 255, -1)
 
     return building_mask
 
 
+def close(image, kernel_size):
+    """
+    Apply a morphological closing to an image.
+
+    Args:
+        image: The image data.
+        kernel_size (int): The size of the kernel used for the morphological operation.
+
+    Returns:
+        numpy.ndarray: The image data after morphological closing.
+    """
+    kernel = np.ones((kernel_size, kernel_size), np.uint8)
+    image_closed = cv2.morphologyEx(image, cv2.MORPH_CLOSE, kernel)
+    return image_closed
 
 
-def close(building_mask, CloseKernel_size):
-    kernel = np.ones((CloseKernel_size, CloseKernel_size), np.uint8)
-    building_mask_closed = cv2.morphologyEx(building_mask, cv2.MORPH_CLOSE, kernel)
-    return building_mask_closed
-
 def write_geotiff(filename, data, profile):
+    """
+    Write image data and profile to a geotiff file.
+
+    Args:
+        filename (str): Path to the output geotiff file.
+        data: The image data.
+        profile: A dictionary with metadata about the image.
+
+    Returns:
+        output image
+    """
     profile.update(count=1, dtype=rasterio.uint8, crs=rasterio.crs.CRS.from_epsg(3857))
     with rasterio.open(filename, 'w', **profile) as dst:
-        dst.crs = profile['crs']  # Add CRS information
+        dst.crs = profile['crs']
         dst.write(data.astype(rasterio.uint8), 1)
 
 
 def building_footprints_to_geojson(tiff_file, geojson_file):
-    # Load the building mask
+    """
+    Convert building footprints to GeoJSON format.
+
+    Args:
+        tiff_file (str): Path to the input tiff file.
+        geojson_file (str): Path to the output GeoJSON file.
+
+    Returns:
+        geojson_file: Output GeoJSON file.
+    """
     with rasterio.open(tiff_file) as src:
         building_mask = src.read(1)
 
-    # Create a mask that is True for building pixels and False for all other pixels
     building_only_mask = (building_mask == 0).astype('uint8')
 
-    # Polygonize the building pixels to get the building footprints as polygons
     building_polygons = list(rasterio.features.shapes(building_only_mask, transform=src.transform))
 
-    # Convert the building polygons to a GeoJSON FeatureCollection
     features = []
     for polygon, value in building_polygons:
         if value == 0:
             feature = {'type': 'Feature',
                        'geometry': mapping(shape(polygon)),
                        'properties': {'value': int(value)}}
             features.append(feature)
 
     geojson_dict = {'type': 'FeatureCollection', 'features': features, 'crs': {'type': 'name', 'properties': {'name': 'EPSG:3857'}}}
 
-    # Write the GeoJSON file to disk
     with open(geojson_file, 'w') as f:
         json.dump(geojson_dict, f)
+    print('Output GeoJSON is ready')
```

### Comparing `LasBuildSeg-0.1.14/LasBuildSeg/__init__.py` & `LasBuildSeg-0.1.15/LasBuildSeg/__init__.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.14/LasBuildSeg.egg-info/PKG-INFO` & `LasBuildSeg-0.1.15/LasBuildSeg.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.14
+Version: 0.1.15
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,43 +24,66 @@
 
 This of example of an how you can run your code
 
 ```python
 import LasBuildSeg as lasb
 import numpy as np
 
-input_laz = '<input>.laz'
-epsg_code = <epsg_code>
-dsm_resolution = <resolution>
-scale=<lazfilescale>
-method=<interpoaltion method>
+# Define input parameters
+input_laz = '<input>.laz'  # Path to the input laz/las data file
+epsg_code = <epsg_code>  # EPSG code of the input laz data
+multy = <DTM non-ground multipalction number>  # Multiplication factor for DSM height enhancement
+intermethod = '<interpolation method>'  # Interpolation method ('cubic', 'nearest', or 'linear')
+
+# Define default parameter values
+constant = 3.6  # Adaptive threshold constant
+block_size = 51  # Adaptive threshold block size
+kernel_size = 3  # Morphological open kernel size
+tri_threshold = 3  # Terrain Ruggedness Index threshold
 
-Lasb.generate_dsm(input_laz, epsg_code, dsm_resolution,intermethod)
-Lasb.generate_dtm(input_laz, epsg_code, dsm_resolution,intermethod)
+# Define contour filtering parameters
+min_size = 35
+max_size = 5000
+squareness_threshold = 0.3
+width_threshold = 3
+height_threshold = 3
+CloseKernel_size = 15
+
+# Generate DSM and DTM
+lasb.generate_dsm(input_laz, epsg_code, intermethod)
+lasb.generate_dtm(input_laz, epsg_code, intermethod, multy)
+
+# Generate NDHM
 lasb.generate_ndhm('dtm.tif', 'dsm.tif')
 
+# Read NDHM image and profile
 img, profile = lasb.read_geotiff('ndhm.tif')
+
+# Transform DSM
 lasb.DSM_Transform('dsm.tif')
 
+# Read transformed DSM and profile
 dem, _ = lasb.read_geotiff('dsm3857.tif')
+
+# Convert image to 8-bit
 img_8bit = lasb.to_8bit(img)
-constant = 3.6
-block_size = 51
+
+# Apply adaptive thresholding
 img_thresh = lasb.threshold(img_8bit, block_size, constant)
-kernel_size = 3
+
+# Apply morphological opening
 img_open = lasb.morphopen(img_thresh, kernel_size)
 
-min_size = 35
-max_size = 5000
-squareness_threshold=0.3 
-width_threshold=3 
-height_threshold=3 
-tri_threshold=3
-building_mask = Lasb.filter_contoursntri(img_open, profile, min_size, max_size, squareness_threshold, width_threshold, height_threshold)
-kernel_size = 3
-CloseKernel_size=15
+# Filter contours without TRI
+building_mask = lasb.filter_contoursntri(img_open, profile, min_size, max_size, squareness_threshold, width_threshold, height_threshold)
+
+# Apply morphological closing
 building_mask_closed = lasb.close(building_mask, CloseKernel_size)
-# Invert the building mask to make buildings appear as white ground pixels
-inverted_building_mask = np.ones_like(building_mask, dtype=np.uint8) - building_mask_closed
+
+# Write building mask to GeoTIFF
 lasb.write_geotiff('buildings.tif', building_mask_closed, profile)
+
+# Convert building mask to GeoJSON
 lasb.building_footprints_to_geojson('buildings.tif', 'building.geojson')
-print('All of our steps are done.')
+
+# Print completion message
+print('All steps are complete.')
```

### Comparing `LasBuildSeg-0.1.14/PKG-INFO` & `LasBuildSeg-0.1.15/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.14
+Version: 0.1.15
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,43 +24,66 @@
 
 This of example of an how you can run your code
 
 ```python
 import LasBuildSeg as lasb
 import numpy as np
 
-input_laz = '<input>.laz'
-epsg_code = <epsg_code>
-dsm_resolution = <resolution>
-scale=<lazfilescale>
-method=<interpoaltion method>
+# Define input parameters
+input_laz = '<input>.laz'  # Path to the input laz/las data file
+epsg_code = <epsg_code>  # EPSG code of the input laz data
+multy = <DTM non-ground multipalction number>  # Multiplication factor for DSM height enhancement
+intermethod = '<interpolation method>'  # Interpolation method ('cubic', 'nearest', or 'linear')
+
+# Define default parameter values
+constant = 3.6  # Adaptive threshold constant
+block_size = 51  # Adaptive threshold block size
+kernel_size = 3  # Morphological open kernel size
+tri_threshold = 3  # Terrain Ruggedness Index threshold
 
-Lasb.generate_dsm(input_laz, epsg_code, dsm_resolution,intermethod)
-Lasb.generate_dtm(input_laz, epsg_code, dsm_resolution,intermethod)
+# Define contour filtering parameters
+min_size = 35
+max_size = 5000
+squareness_threshold = 0.3
+width_threshold = 3
+height_threshold = 3
+CloseKernel_size = 15
+
+# Generate DSM and DTM
+lasb.generate_dsm(input_laz, epsg_code, intermethod)
+lasb.generate_dtm(input_laz, epsg_code, intermethod, multy)
+
+# Generate NDHM
 lasb.generate_ndhm('dtm.tif', 'dsm.tif')
 
+# Read NDHM image and profile
 img, profile = lasb.read_geotiff('ndhm.tif')
+
+# Transform DSM
 lasb.DSM_Transform('dsm.tif')
 
+# Read transformed DSM and profile
 dem, _ = lasb.read_geotiff('dsm3857.tif')
+
+# Convert image to 8-bit
 img_8bit = lasb.to_8bit(img)
-constant = 3.6
-block_size = 51
+
+# Apply adaptive thresholding
 img_thresh = lasb.threshold(img_8bit, block_size, constant)
-kernel_size = 3
+
+# Apply morphological opening
 img_open = lasb.morphopen(img_thresh, kernel_size)
 
-min_size = 35
-max_size = 5000
-squareness_threshold=0.3 
-width_threshold=3 
-height_threshold=3 
-tri_threshold=3
-building_mask = Lasb.filter_contoursntri(img_open, profile, min_size, max_size, squareness_threshold, width_threshold, height_threshold)
-kernel_size = 3
-CloseKernel_size=15
+# Filter contours without TRI
+building_mask = lasb.filter_contoursntri(img_open, profile, min_size, max_size, squareness_threshold, width_threshold, height_threshold)
+
+# Apply morphological closing
 building_mask_closed = lasb.close(building_mask, CloseKernel_size)
-# Invert the building mask to make buildings appear as white ground pixels
-inverted_building_mask = np.ones_like(building_mask, dtype=np.uint8) - building_mask_closed
+
+# Write building mask to GeoTIFF
 lasb.write_geotiff('buildings.tif', building_mask_closed, profile)
+
+# Convert building mask to GeoJSON
 lasb.building_footprints_to_geojson('buildings.tif', 'building.geojson')
-print('All of our steps are done.')
+
+# Print completion message
+print('All steps are complete.')
```

### Comparing `LasBuildSeg-0.1.14/Setup.py` & `LasBuildSeg-0.1.15/Setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     INSTALL_REQUIRES = []
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
         
 setup(
   name='LasBuildSeg',
-  version='0.1.14',
+  version='0.1.15',
   description='Building Footrprint Extraction from Aerial LiDAR data',
   long_description=long_description,
   long_description_content_type='text/markdown',  
   url='',  
   author='MertcanErdem',
   author_email='merak908@gmail.com',
   license='GNU General Public License v2.0',
```

