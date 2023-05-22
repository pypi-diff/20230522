# Comparing `tmp/AutoCarver-4.3.0.tar.gz` & `tmp/AutoCarver-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AutoCarver-4.3.0.tar", last modified: Mon May 22 07:25:36 2023, max compression
+gzip compressed data, was "dist\AutoCarver-4.3.1.tar", last modified: Mon May 22 07:50:03 2023, max compression
```

## Comparing `AutoCarver-4.3.0.tar` & `AutoCarver-4.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 07:25:36.000000 AutoCarver-4.3.0/
-drwxrwxrwx   0        0        0        0 2023-05-22 07:25:36.000000 AutoCarver-4.3.0/AutoCarver/
--rw-rw-rw-   0        0        0    23961 2023-05-22 07:18:16.000000 AutoCarver-4.3.0/AutoCarver/AutoCarver.py
--rw-rw-rw-   0        0        0     8599 2023-05-22 07:18:35.000000 AutoCarver-4.3.0/AutoCarver/Converters.py
--rw-rw-rw-   0        0        0    52539 2023-05-22 07:18:23.000000 AutoCarver-4.3.0/AutoCarver/Discretizers.py
--rw-rw-rw-   0        0        0    28038 2023-05-22 07:18:44.000000 AutoCarver-4.3.0/AutoCarver/FeatureSelector.py
--rw-rw-rw-   0        0        0        0 2023-01-10 08:49:10.000000 AutoCarver-4.3.0/AutoCarver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 07:25:36.000000 AutoCarver-4.3.0/AutoCarver.egg-info/
--rw-rw-rw-   0        0        0     7119 2023-05-22 07:25:27.000000 AutoCarver-4.3.0/AutoCarver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-22 07:25:34.000000 AutoCarver-4.3.0/AutoCarver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 07:25:27.000000 AutoCarver-4.3.0/AutoCarver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 07:25:27.000000 AutoCarver-4.3.0/AutoCarver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2023-01-05 13:13:13.000000 AutoCarver-4.3.0/LICENSE
--rw-rw-rw-   0        0        0     7119 2023-05-22 07:25:36.000000 AutoCarver-4.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6346 2023-05-14 13:54:01.000000 AutoCarver-4.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 07:25:36.000000 AutoCarver-4.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-05-22 07:19:00.000000 AutoCarver-4.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:50:03.000000 AutoCarver-4.3.1/
+drwxrwxrwx   0        0        0        0 2023-05-22 07:50:03.000000 AutoCarver-4.3.1/AutoCarver/
+-rw-rw-rw-   0        0        0    23989 2023-05-22 07:48:34.000000 AutoCarver-4.3.1/AutoCarver/AutoCarver.py
+-rw-rw-rw-   0        0        0     8599 2023-05-22 07:18:35.000000 AutoCarver-4.3.1/AutoCarver/Converters.py
+-rw-rw-rw-   0        0        0    52539 2023-05-22 07:18:23.000000 AutoCarver-4.3.1/AutoCarver/Discretizers.py
+-rw-rw-rw-   0        0        0    28038 2023-05-22 07:18:44.000000 AutoCarver-4.3.1/AutoCarver/FeatureSelector.py
+-rw-rw-rw-   0        0        0        0 2023-01-10 08:49:10.000000 AutoCarver-4.3.1/AutoCarver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:50:03.000000 AutoCarver-4.3.1/AutoCarver.egg-info/
+-rw-rw-rw-   0        0        0     7119 2023-05-22 07:49:56.000000 AutoCarver-4.3.1/AutoCarver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-22 07:50:01.000000 AutoCarver-4.3.1/AutoCarver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 07:49:56.000000 AutoCarver-4.3.1/AutoCarver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 07:49:56.000000 AutoCarver-4.3.1/AutoCarver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2023-01-05 13:13:13.000000 AutoCarver-4.3.1/LICENSE
+-rw-rw-rw-   0        0        0     7119 2023-05-22 07:50:03.000000 AutoCarver-4.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6346 2023-05-14 13:54:01.000000 AutoCarver-4.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 07:50:03.000000 AutoCarver-4.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-05-22 07:48:47.000000 AutoCarver-4.3.1/setup.py
```

### Comparing `AutoCarver-4.3.0/AutoCarver/AutoCarver.py` & `AutoCarver-4.3.1/AutoCarver/AutoCarver.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,15 +382,15 @@
         # getting all possible combinations for the feature without NaNS
         combinations = get_all_combinations(order, max_n_mod, raw=False)
     
     # keeping nans as a modality
     else:
     
         # getting all possible combinations for the feature with NaNS
-        combinations = get_all_nan_combinations(order, str_nan)
+        combinations = get_all_nan_combinations(order, str_nan, max_n_mod)
 
     # computing association measure per combination 
     associations = [apply_combination(xtab, combi) for combi in combinations]
 
     # sort according to association measure
     if len(combinations) > 0:
         associations = DataFrame(associations)
@@ -450,21 +450,21 @@
     
     # converting back to GroupedList
     if not raw:
         combinations = [groupedlist_combination(combination, values) for combination in combinations]
 
     return combinations
 
-def get_all_nan_combinations(order: GroupedList, str_nan: str) -> List[GroupedList]:
+def get_all_nan_combinations(order: GroupedList, str_nan: str, max_n_mod: int) -> List[GroupedList]:
     """ all possible combinations of modalities with numpy.nan"""
 
     # computing all non-NaN combinations
     # case 0: several modalities -> several combinations
     if len(order) > 1:
-        combinations = get_all_combinations(order, len(order), raw=True)
+        combinations = get_all_combinations(order, max_n_mod-1, raw=True)
     # case 1: unique or no modality -> two combinations
     else:
         combinations = []
 
     # iterating over each combinations of non-NaNs
     new_combinations = []
     for combi in combinations:
```

### Comparing `AutoCarver-4.3.0/AutoCarver/Converters.py` & `AutoCarver-4.3.1/AutoCarver/Converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.3.0/AutoCarver/Discretizers.py` & `AutoCarver-4.3.1/AutoCarver/Discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.3.0/AutoCarver/FeatureSelector.py` & `AutoCarver-4.3.1/AutoCarver/FeatureSelector.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.3.0/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-4.3.1/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.3.0
+Version: 4.3.1
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `AutoCarver-4.3.0/LICENSE` & `AutoCarver-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.3.0/PKG-INFO` & `AutoCarver-4.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.3.0
+Version: 4.3.1
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `AutoCarver-4.3.0/README.md` & `AutoCarver-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.3.0/setup.py` & `AutoCarver-4.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='AutoCarver',
-    version='4.3.0',
+    version='4.3.1',
     author='Mario DEFRANCE',
     author_email='defrancemario@gmail.com',
     description='Automatic Bucketizing of Features with Optimal Association',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mdefrance/AutoCarver',
     project_urls = {
```

