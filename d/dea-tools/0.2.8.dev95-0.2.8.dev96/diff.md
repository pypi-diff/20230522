# Comparing `tmp/dea-tools-0.2.8.dev95.tar.gz` & `tmp/dea-tools-0.2.8.dev96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dea-tools-0.2.8.dev95.tar", last modified: Thu May 18 10:10:20 2023, max compression
+gzip compressed data, was "dea-tools-0.2.8.dev96.tar", last modified: Mon May 22 00:06:13 2023, max compression
```

## Comparing `dea-tools-0.2.8.dev95.tar` & `dea-tools-0.2.8.dev96.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.353197 dea-tools-0.2.8.dev95/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-18 10:10:20.353197 dea-tools-0.2.8.dev95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.349197 dea-tools-0.2.8.dev95/dea_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.353197 dea-tools-0.2.8.dev95/dea_tools/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32250 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/animations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/changefilmstrips.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/crophealth.py
--rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/deacoastlines.py
--rw-r--r--   0 runner    (1001) docker     (123)    29019 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/imageexport.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/miningrehab.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/widgetconstructors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20197 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/bandindices.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/bom.py
--rw-r--r--   0 runner    (1001) docker     (123)    62213 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)    60087 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/coastal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)    51764 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/datahandling.py
--rw-r--r--   0 runner    (1001) docker     (123)    39758 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/landcover.py
--rw-r--r--   0 runner    (1001) docker     (123)    37726 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/pyfes_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36817 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)    26490 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/waterbodies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.349197 dea-tools-0.2.8.dev95/dea_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-18 10:10:18.000000 dea-tools-0.2.8.dev95/dea_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-18 10:10:20.000000 dea-tools-0.2.8.dev95/dea_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:10:18.000000 dea-tools-0.2.8.dev95/dea_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-18 10:10:18.000000 dea-tools-0.2.8.dev95/dea_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 10:10:18.000000 dea-tools-0.2.8.dev95/dea_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 10:10:20.353197 dea-tools-0.2.8.dev95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:06:13.007174 dea-tools-0.2.8.dev96/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-22 00:06:13.007174 dea-tools-0.2.8.dev96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:06:13.003174 dea-tools-0.2.8.dev96/dea_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:06:13.007174 dea-tools-0.2.8.dev96/dea_tools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32250 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/changefilmstrips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/crophealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/deacoastlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29019 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/imageexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/miningrehab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/widgetconstructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20197 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/bandindices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/bom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62213 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60087 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/coastal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52113 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/datahandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39758 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/landcover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37726 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/pyfes_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36817 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26490 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/waterbodies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:06:13.007174 dea-tools-0.2.8.dev96/dea_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-22 00:06:11.000000 dea-tools-0.2.8.dev96/dea_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-22 00:06:12.000000 dea-tools-0.2.8.dev96/dea_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 00:06:11.000000 dea-tools-0.2.8.dev96/dea_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 00:06:11.000000 dea-tools-0.2.8.dev96/dea_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 00:06:11.000000 dea-tools-0.2.8.dev96/dea_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 00:06:13.007174 dea-tools-0.2.8.dev96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/setup.py
```

### Comparing `dea-tools-0.2.8.dev95/LICENSE` & `dea-tools-0.2.8.dev96/LICENSE`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/PKG-INFO` & `dea-tools-0.2.8.dev96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dea-tools
-Version: 0.2.8.dev95
+Version: 0.2.8.dev96
 Summary: Functions and algorithms for analysing Digital Earth Australia data.
 Home-page: https://github.com/GeoscienceAustralia/dea-notebooks
 Author: Geoscience Australia
 Author-email: earth.observation@ga.gov.au
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dea-tools-0.2.8.dev95/README.rst` & `dea-tools-0.2.8.dev96/README.rst`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/app/animations.py` & `dea-tools-0.2.8.dev96/dea_tools/app/animations.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/app/changefilmstrips.py` & `dea-tools-0.2.8.dev96/dea_tools/app/changefilmstrips.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/app/crophealth.py` & `dea-tools-0.2.8.dev96/dea_tools/app/crophealth.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/app/deacoastlines.py` & `dea-tools-0.2.8.dev96/dea_tools/app/deacoastlines.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/app/imageexport.py` & `dea-tools-0.2.8.dev96/dea_tools/app/imageexport.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/app/miningrehab.py` & `dea-tools-0.2.8.dev96/dea_tools/app/miningrehab.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/app/widgetconstructors.py` & `dea-tools-0.2.8.dev96/dea_tools/app/widgetconstructors.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/bandindices.py` & `dea-tools-0.2.8.dev96/dea_tools/bandindices.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/bom.py` & `dea-tools-0.2.8.dev96/dea_tools/bom.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/classification.py` & `dea-tools-0.2.8.dev96/dea_tools/classification.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/climate.py` & `dea-tools-0.2.8.dev96/dea_tools/climate.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/coastal.py` & `dea-tools-0.2.8.dev96/dea_tools/coastal.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/dask.py` & `dea-tools-0.2.8.dev96/dea_tools/dask.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/datahandling.py` & `dea-tools-0.2.8.dev96/dea_tools/datahandling.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,22 +232,29 @@
         spatiotemporal query and load parameters used to extract data.
         Keyword arguments can either be listed directly in the
         `load_ard` call like any other parameter (e.g.
         `measurements=['nbart_red']`), or by passing in a query kwarg
         dictionary (e.g. `**query`). Keywords can include `measurements`,
         `x`, `y`, `time`, `resolution`, `resampling`, `group_by`, `crs`;
         see the `dc.load` documentation for all possible options:
-        https://datacube-core.readthedocs.io/en/latest/dev/api/generate/datacube.Datacube.load.html
+        https://datacube-core.readthedocs.io/en/latest/api/indexed-data/generate/datacube.Datacube.load.html
 
     Returns
     -------
     combined_ds : xarray.Dataset
         An xarray.Dataset containing only satellite observations with
         a proportion of good quality pixels greater than `min_gooddata`.
 
+    Notes
+    -----
+    The `load_ard` function builds on the Open Data Cube's native `dc.load`
+    function by adding the ability to load multiple satellite data
+    products at once, and automatically apply cloud masking and filtering.
+    For loading non-satellite data products (e.g. DEA Water Observations),
+    use `dc.load` instead.
     """
 
     #########
     # Setup #
     #########
 
     # Verify that products were provided
```

### Comparing `dea-tools-0.2.8.dev95/dea_tools/landcover.py` & `dea-tools-0.2.8.dev96/dea_tools/landcover.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/plotting.py` & `dea-tools-0.2.8.dev96/dea_tools/plotting.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/pyfes_model.py` & `dea-tools-0.2.8.dev96/dea_tools/pyfes_model.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/spatial.py` & `dea-tools-0.2.8.dev96/dea_tools/spatial.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/temporal.py` & `dea-tools-0.2.8.dev96/dea_tools/temporal.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/validation.py` & `dea-tools-0.2.8.dev96/dea_tools/validation.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools/waterbodies.py` & `dea-tools-0.2.8.dev96/dea_tools/waterbodies.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/dea_tools.egg-info/PKG-INFO` & `dea-tools-0.2.8.dev96/dea_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dea-tools
-Version: 0.2.8.dev95
+Version: 0.2.8.dev96
 Summary: Functions and algorithms for analysing Digital Earth Australia data.
 Home-page: https://github.com/GeoscienceAustralia/dea-notebooks
 Author: Geoscience Australia
 Author-email: earth.observation@ga.gov.au
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dea-tools-0.2.8.dev95/dea_tools.egg-info/SOURCES.txt` & `dea-tools-0.2.8.dev96/dea_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/index.rst` & `dea-tools-0.2.8.dev96/index.rst`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev95/setup.py` & `dea-tools-0.2.8.dev96/setup.py`

 * *Files identical despite different names*

