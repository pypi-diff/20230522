# Comparing `tmp/spaemis-0.2.0.tar.gz` & `tmp/spaemis-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaemis-0.2.0.tar", max compression
+gzip compressed data, was "spaemis-0.2.0a2.tar", max compression
```

## Comparing `spaemis-0.2.0.tar` & `spaemis-0.2.0a2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1080 2023-05-22 13:38:17.390670 spaemis-0.2.0/LICENSE
--rw-r--r--   0        0        0     1733 2023-05-22 13:38:17.390670 spaemis-0.2.0/README.md
--rw-r--r--   0        0        0     4558 2023-05-22 13:38:18.310678 spaemis-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      196 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/__init__.py
--rw-r--r--   0        0        0      242 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/commands/__init__.py
--rw-r--r--   0        0        0      525 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/commands/base.py
--rw-r--r--   0        0        0     1756 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/commands/generate_command.py
--rw-r--r--   0        0        0      733 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/commands/gse_emis_command.py
--rw-r--r--   0        0        0     1309 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/commands/point_source_command.py
--rw-r--r--   0        0        0     8561 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/config.py
--rw-r--r--   0        0        0      644 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/constants.py
--rwxr-xr-x   0        0        0    25545 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/gse_emis.py
--rw-r--r--   0        0        0     6046 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/input_data.py
--rw-r--r--   0        0        0     9850 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/inventory.py
--rw-r--r--   0        0        0      186 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/main.py
--rw-r--r--   0        0        0     7356 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/project.py
--rw-r--r--   0        0        0        0 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/py.typed
--rw-r--r--   0        0        0     2218 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/scaling/__init__.py
--rw-r--r--   0        0        0     2645 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/scaling/base.py
--rw-r--r--   0        0        0     1323 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/scaling/constant.py
--rw-r--r--   0        0        0     1128 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/scaling/exclude.py
--rw-r--r--   0        0        0     3528 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/scaling/point_source.py
--rw-r--r--   0        0        0     5416 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/scaling/proxy.py
--rw-r--r--   0        0        0     3010 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/scaling/relative_change.py
--rw-r--r--   0        0        0     5846 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/scaling/timeseries.py
--rw-r--r--   0        0        0     2023 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/unit_registry.py
--rw-r--r--   0        0        0     5495 2023-05-22 13:38:18.314678 spaemis-0.2.0/src/spaemis/utils.py
--rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 spaemis-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-22 13:26:05.725376 spaemis-0.2.0a2/LICENSE
+-rw-r--r--   0        0        0     1733 2023-05-22 13:26:05.725376 spaemis-0.2.0a2/README.md
+-rw-r--r--   0        0        0     4596 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/__init__.py
+-rw-r--r--   0        0        0      242 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/commands/__init__.py
+-rw-r--r--   0        0        0      525 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/commands/base.py
+-rw-r--r--   0        0        0     1756 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/commands/generate_command.py
+-rw-r--r--   0        0        0      733 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/commands/gse_emis_command.py
+-rw-r--r--   0        0        0     1309 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/commands/point_source_command.py
+-rw-r--r--   0        0        0     8561 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/config.py
+-rw-r--r--   0        0        0      644 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/constants.py
+-rwxr-xr-x   0        0        0    25545 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/gse_emis.py
+-rw-r--r--   0        0        0     6046 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/input_data.py
+-rw-r--r--   0        0        0     9850 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/inventory.py
+-rw-r--r--   0        0        0      186 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/main.py
+-rw-r--r--   0        0        0     7356 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/project.py
+-rw-r--r--   0        0        0        0 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/py.typed
+-rw-r--r--   0        0        0     2218 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/scaling/__init__.py
+-rw-r--r--   0        0        0     2645 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/scaling/base.py
+-rw-r--r--   0        0        0     1323 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/scaling/constant.py
+-rw-r--r--   0        0        0     1128 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/scaling/exclude.py
+-rw-r--r--   0        0        0     3528 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/scaling/point_source.py
+-rw-r--r--   0        0        0     5416 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/scaling/proxy.py
+-rw-r--r--   0        0        0     3010 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/scaling/relative_change.py
+-rw-r--r--   0        0        0     5846 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/scaling/timeseries.py
+-rw-r--r--   0        0        0     2023 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/unit_registry.py
+-rw-r--r--   0        0        0     5495 2023-05-22 13:26:06.613385 spaemis-0.2.0a2/src/spaemis/utils.py
+-rw-r--r--   0        0        0     3350 1970-01-01 00:00:00.000000 spaemis-0.2.0a2/PKG-INFO
```

### Comparing `spaemis-0.2.0/LICENSE` & `spaemis-0.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/README.md` & `spaemis-0.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/pyproject.toml` & `spaemis-0.2.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.coverage.run]
 source = ["src"]
 
 [tool.poetry]
 name = "spaemis"
-version = "0.2.0"
+version = "0.2.0a2"
 description = "Produce a coherent set of emissions for regional air quality modelling"
 authors = ["Jared Lewis <jared.lewis@climate-resource.com>"]
 readme = "README.md"
 packages = [{include = "spaemis", from = "src"}]
 keywords = ["emissions", "climate", "air quality"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -42,18 +42,19 @@
 netcdf4 = "^1.6.3"
 scipy = "^1.10.1"
 pooch = "^1.7.0"
 typing-extensions = "^4.5.0"
 pyyaml = "^6.0"
 
 [tool.commitizen]
-version = "0.2.0"
+version = "0.2.0a2"
 version_files = ["pyproject.toml:^version"]
 tag_format = "v$version"
 major_version_zero = true
+changelog_merge_prerelease = true
 
 [tool.poetry.extras]
 notebooks = [
     "notebook",
     "matplotlib",
     "seaborn",
     "jupytext" ,
```

### Comparing `spaemis-0.2.0/src/spaemis/commands/base.py` & `spaemis-0.2.0a2/src/spaemis/commands/base.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/commands/generate_command.py` & `spaemis-0.2.0a2/src/spaemis/commands/generate_command.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/commands/gse_emis_command.py` & `spaemis-0.2.0a2/src/spaemis/commands/gse_emis_command.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/commands/point_source_command.py` & `spaemis-0.2.0a2/src/spaemis/commands/point_source_command.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/config.py` & `spaemis-0.2.0a2/src/spaemis/config.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/constants.py` & `spaemis-0.2.0a2/src/spaemis/constants.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/gse_emis.py` & `spaemis-0.2.0a2/src/spaemis/gse_emis.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/input_data.py` & `spaemis-0.2.0a2/src/spaemis/input_data.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/inventory.py` & `spaemis-0.2.0a2/src/spaemis/inventory.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/project.py` & `spaemis-0.2.0a2/src/spaemis/project.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/scaling/__init__.py` & `spaemis-0.2.0a2/src/spaemis/scaling/__init__.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/scaling/base.py` & `spaemis-0.2.0a2/src/spaemis/scaling/base.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/scaling/constant.py` & `spaemis-0.2.0a2/src/spaemis/scaling/constant.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/scaling/exclude.py` & `spaemis-0.2.0a2/src/spaemis/scaling/exclude.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/scaling/point_source.py` & `spaemis-0.2.0a2/src/spaemis/scaling/point_source.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/scaling/proxy.py` & `spaemis-0.2.0a2/src/spaemis/scaling/proxy.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/scaling/relative_change.py` & `spaemis-0.2.0a2/src/spaemis/scaling/relative_change.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/scaling/timeseries.py` & `spaemis-0.2.0a2/src/spaemis/scaling/timeseries.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/unit_registry.py` & `spaemis-0.2.0a2/src/spaemis/unit_registry.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/src/spaemis/utils.py` & `spaemis-0.2.0a2/src/spaemis/utils.py`

 * *Files identical despite different names*

### Comparing `spaemis-0.2.0/PKG-INFO` & `spaemis-0.2.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spaemis
-Version: 0.2.0
+Version: 0.2.0a2
 Summary: Produce a coherent set of emissions for regional air quality modelling
 Home-page: https://github.com/climate-resource/spaemis
 Keywords: emissions,climate,air quality
 Author: Jared Lewis
 Author-email: jared.lewis@climate-resource.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
```

