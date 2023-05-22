# Comparing `tmp/omero-cli-zarr-0.5.2.tar.gz` & `tmp/omero-cli-zarr-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-cli-zarr-0.5.2.tar", last modified: Wed May 17 21:08:21 2023, max compression
+gzip compressed data, was "omero-cli-zarr-0.5.3.tar", last modified: Mon May 22 13:24:48 2023, max compression
```

## Comparing `omero-cli-zarr-0.5.2.tar` & `omero-cli-zarr-0.5.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.591786 omero-cli-zarr-0.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/.github/workflows/precommit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/.github/workflows/publish_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.591786 omero-cli-zarr-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.591786 omero-cli-zarr-0.5.2/src/omero/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/src/omero/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/src/omero/plugins/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-17 21:08:21.000000 omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-17 21:08:21.000000 omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:08:21.000000 omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-17 21:08:21.000000 omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 21:08:21.000000 omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/src/omero_zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/src/omero_zarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 21:08:21.000000 omero-cli-zarr-0.5.2/src/omero_zarr/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/src/omero_zarr/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/src/omero_zarr/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/src/omero_zarr/raw_pixels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/src/omero_zarr/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:24:48.524397 omero-cli-zarr-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:24:48.524397 omero-cli-zarr-0.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:24:48.524397 omero-cli-zarr-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/.github/workflows/precommit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/.github/workflows/publish_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-22 13:24:48.524397 omero-cli-zarr-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 13:24:48.524397 omero-cli-zarr-0.5.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:24:48.524397 omero-cli-zarr-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:24:48.524397 omero-cli-zarr-0.5.3/src/omero/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:24:48.524397 omero-cli-zarr-0.5.3/src/omero/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/src/omero/plugins/zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:24:48.524397 omero-cli-zarr-0.5.3/src/omero_cli_zarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-22 13:24:48.000000 omero-cli-zarr-0.5.3/src/omero_cli_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-22 13:24:48.000000 omero-cli-zarr-0.5.3/src/omero_cli_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:24:48.000000 omero-cli-zarr-0.5.3/src/omero_cli_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 13:24:48.000000 omero-cli-zarr-0.5.3/src/omero_cli_zarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 13:24:48.000000 omero-cli-zarr-0.5.3/src/omero_cli_zarr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:24:48.524397 omero-cli-zarr-0.5.3/src/omero_zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/src/omero_zarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 13:24:48.000000 omero-cli-zarr-0.5.3/src/omero_zarr/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/src/omero_zarr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/src/omero_zarr/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/src/omero_zarr/raw_pixels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-22 13:24:40.000000 omero-cli-zarr-0.5.3/src/omero_zarr/util.py
```

### Comparing `omero-cli-zarr-0.5.2/.github/workflows/publish_pypi.yml` & `omero-cli-zarr-0.5.3/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `omero-cli-zarr-0.5.2/.pre-commit-config.yaml` & `omero-cli-zarr-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `omero-cli-zarr-0.5.2/LICENSE.txt` & `omero-cli-zarr-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omero-cli-zarr-0.5.2/PKG-INFO` & `omero-cli-zarr-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero-cli-zarr
-Version: 0.5.2
+Version: 0.5.3
 Summary: Plugin for exporting images in zarr format.
 Home-page: https://github.com/ome/omero-cli-zarr/
 Author: The Open Microscopy Team
 Author-email: 
 License: UNKNOWN
 Keywords: OMERO.CLI,plugin
 Platform: UNKNOWN
```

### Comparing `omero-cli-zarr-0.5.2/README.rst` & `omero-cli-zarr-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `omero-cli-zarr-0.5.2/setup.py` & `omero-cli-zarr-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     return long_description
 
 
 long_description = get_long_description()
 
 setup(
     name="omero-cli-zarr",
-    version="0.5.2",
+    version="0.5.3",
     packages=["omero_zarr", "omero.plugins"],
     package_dir={"": "src"},
     description="Plugin for exporting images in zarr format.",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Plugins",
         "Intended Audience :: Developers",
```

### Comparing `omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/PKG-INFO` & `omero-cli-zarr-0.5.3/src/omero_cli_zarr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero-cli-zarr
-Version: 0.5.2
+Version: 0.5.3
 Summary: Plugin for exporting images in zarr format.
 Home-page: https://github.com/ome/omero-cli-zarr/
 Author: The Open Microscopy Team
 Author-email: 
 License: UNKNOWN
 Keywords: OMERO.CLI,plugin
 Platform: UNKNOWN
```

### Comparing `omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/SOURCES.txt` & `omero-cli-zarr-0.5.3/src/omero_cli_zarr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omero-cli-zarr-0.5.2/src/omero_zarr/__init__.py` & `omero-cli-zarr-0.5.3/src/omero_zarr/__init__.py`

 * *Files identical despite different names*

### Comparing `omero-cli-zarr-0.5.2/src/omero_zarr/cli.py` & `omero-cli-zarr-0.5.3/src/omero_zarr/cli.py`

 * *Files identical despite different names*

### Comparing `omero-cli-zarr-0.5.2/src/omero_zarr/masks.py` & `omero-cli-zarr-0.5.3/src/omero_zarr/masks.py`

 * *Files identical despite different names*

### Comparing `omero-cli-zarr-0.5.2/src/omero_zarr/raw_pixels.py` & `omero-cli-zarr-0.5.3/src/omero_zarr/raw_pixels.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,20 @@
         dims[-1] = dims[-1] // 2
         dims[-2] = dims[-2] // 2
         output = da_resize(
             dask_image, tuple(dims), preserve_range=True, anti_aliasing=False
         )
 
         # write to disk
-        da.to_zarr(arr=output, url=image_path, component=path)
+        da.to_zarr(
+            arr=output,
+            url=parent.store,
+            component=str(path),
+            dimension_separator=parent._store._dimension_separator,
+        )
 
     return paths
 
 
 def marshal_acquisition(acquisition: omero.gateway._PlateAcquisitionWrapper) -> Dict:
     """Marshal a PlateAcquisitionWrapper to JSON"""
     acq = {
```

### Comparing `omero-cli-zarr-0.5.2/src/omero_zarr/util.py` & `omero-cli-zarr-0.5.3/src/omero_zarr/util.py`

 * *Files identical despite different names*

