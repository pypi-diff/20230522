# Comparing `tmp/rio-cogeo-3.5.1.tar.gz` & `tmp/rio_cogeo-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio-cogeo-3.5.1.tar", last modified: Thu Apr  6 15:17:47 2023, max compression
+gzip compressed data, was "rio_cogeo-3.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rio-cogeo-3.5.1.tar` & `rio_cogeo-3.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      213 2023-04-06 15:17:33.591065 rio-cogeo-3.5.1/.bumpversion.cfg
--rw-r--r--   0        0        0     1172 2023-04-06 15:17:33.591065 rio-cogeo-3.5.1/.gitignore
--rw-r--r--   0        0        0      740 2023-04-06 15:17:33.591065 rio-cogeo-3.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1517 2023-04-06 15:17:33.591065 rio-cogeo-3.5.1/LICENSE
--rw-r--r--   0        0        0     3373 2023-04-06 15:17:33.591065 rio-cogeo-3.5.1/README.md
--rw-r--r--   0        0        0     2305 2023-04-06 15:17:33.595065 rio-cogeo-3.5.1/pyproject.toml
--rw-r--r--   0        0        0      218 2023-04-06 15:17:33.595065 rio-cogeo-3.5.1/rio_cogeo/__init__.py
--rw-r--r--   0        0        0    28428 2023-04-06 15:17:33.595065 rio-cogeo-3.5.1/rio_cogeo/cogeo.py
--rw-r--r--   0        0        0      406 2023-04-06 15:17:33.595065 rio-cogeo-3.5.1/rio_cogeo/errors.py
--rw-r--r--   0        0        0     1950 2023-04-06 15:17:33.595065 rio-cogeo-3.5.1/rio_cogeo/models.py
--rw-r--r--   0        0        0     4521 2023-04-06 15:17:33.595065 rio-cogeo-3.5.1/rio_cogeo/profiles.py
--rw-r--r--   0        0        0       21 2023-04-06 15:17:33.595065 rio-cogeo-3.5.1/rio_cogeo/scripts/__init__.py
--rw-r--r--   0        0        0    13693 2023-04-06 15:17:33.595065 rio-cogeo-3.5.1/rio_cogeo/scripts/cli.py
--rw-r--r--   0        0        0     4595 2023-04-06 15:17:33.595065 rio-cogeo-3.5.1/rio_cogeo/utils.py
--rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 rio-cogeo-3.5.1/PKG-INFO
+-rw-r--r--   0        0        0      213 2023-05-22 21:41:00.779658 rio_cogeo-3.5.2/.bumpversion.cfg
+-rw-r--r--   0        0        0     1172 2023-05-22 21:41:00.779658 rio_cogeo-3.5.2/.gitignore
+-rw-r--r--   0        0        0      740 2023-05-22 21:41:00.779658 rio_cogeo-3.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1517 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/LICENSE
+-rw-r--r--   0        0        0     3373 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/README.md
+-rw-r--r--   0        0        0     2305 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/__init__.py
+-rw-r--r--   0        0        0    29058 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/cogeo.py
+-rw-r--r--   0        0        0      406 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/errors.py
+-rw-r--r--   0        0        0     1950 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/models.py
+-rw-r--r--   0        0        0     4521 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/profiles.py
+-rw-r--r--   0        0        0       21 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/scripts/__init__.py
+-rw-r--r--   0        0        0    13693 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/scripts/cli.py
+-rw-r--r--   0        0        0     4595 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/utils.py
+-rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 rio_cogeo-3.5.2/PKG-INFO
```

### Comparing `rio-cogeo-3.5.1/.gitignore` & `rio_cogeo-3.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rio-cogeo-3.5.1/.pre-commit-config.yaml` & `rio_cogeo-3.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rio-cogeo-3.5.1/LICENSE` & `rio_cogeo-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rio-cogeo-3.5.1/README.md` & `rio_cogeo-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `rio-cogeo-3.5.1/pyproject.toml` & `rio_cogeo-3.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rio-cogeo-3.5.1/rio_cogeo/cogeo.py` & `rio_cogeo-3.5.2/rio_cogeo/cogeo.py`

 * *Files 2% similar despite different names*

```diff
@@ -483,14 +483,26 @@
                     f"The offset of the main IFD should be < 300. It is {ifd_offset} instead"
                 )
 
             ifd_offsets = [ifd_offset]
             details["ifd_offsets"] = {}
             details["ifd_offsets"]["main"] = ifd_offset
 
+            # Optimizations are usually invalidated when a COG is modified.
+            # When this happens, GDAL >= 3.1 flags the modifications by updating the ghost headers.
+            gdal_ghost_headers = src.get_tag_item("GDAL_STRUCTURAL_METADATA", "TIFF")
+            if (
+                gdal_ghost_headers is not None
+                and "KNOWN_INCOMPATIBLE_EDITION=YES" in gdal_ghost_headers
+            ):
+                errors.append(
+                    "This file used to have optimizations in its layout, "
+                    "but those have been, at least partly, invalidated by later changes"
+                )
+
             if overviews and overviews != sorted(overviews):
                 errors.append("Overviews should be sorted")
 
             for ix, dec in enumerate(overviews):
 
                 # NOTE: Size check is handled in rasterio `src.overviews` methods
                 # https://github.com/mapbox/rasterio/blob/4ebdaa08cdcc65b141ed3fe95cf8bbdd9117bc0b/rasterio/_base.pyx
```

### Comparing `rio-cogeo-3.5.1/rio_cogeo/models.py` & `rio_cogeo-3.5.2/rio_cogeo/models.py`

 * *Files identical despite different names*

### Comparing `rio-cogeo-3.5.1/rio_cogeo/profiles.py` & `rio_cogeo-3.5.2/rio_cogeo/profiles.py`

 * *Files identical despite different names*

### Comparing `rio-cogeo-3.5.1/rio_cogeo/scripts/cli.py` & `rio_cogeo-3.5.2/rio_cogeo/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `rio-cogeo-3.5.1/rio_cogeo/utils.py` & `rio_cogeo-3.5.2/rio_cogeo/utils.py`

 * *Files identical despite different names*

### Comparing `rio-cogeo-3.5.1/PKG-INFO` & `rio_cogeo-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-cogeo
-Version: 3.5.1
+Version: 3.5.2
 Summary: Cloud Optimized GeoTIFF (COGEO) creation plugin for rasterio
 Keywords: COGEO,CloudOptimized Geotiff,rasterio
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rio-cogeo Version: 3.5.1 Summary: Cloud Optimized
+Metadata-Version: 2.1 Name: rio-cogeo Version: 3.5.2 Summary: Cloud Optimized
 GeoTIFF (COGEO) creation plugin for rasterio Keywords: COGEO,CloudOptimized
 Geotiff,rasterio Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

