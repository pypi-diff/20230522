# Comparing `tmp/usdanuts-0.0.4.tar.gz` & `tmp/usdanuts-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usdanuts-0.0.4.tar", last modified: Mon May 22 02:36:17 2023, max compression
+gzip compressed data, was "usdanuts-0.0.5.tar", last modified: Mon May 22 02:40:37 2023, max compression
```

## Comparing `usdanuts-0.0.4.tar` & `usdanuts-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 ew        (1000) ew        (1000)        0 2023-05-22 02:36:17.895702 usdanuts-0.0.4/
--rwxrwxrwx   0 ew        (1000) ew        (1000)      660 2023-05-22 02:36:17.892675 usdanuts-0.0.4/PKG-INFO
--rwxrwxrwx   0 ew        (1000) ew        (1000)     1605 2023-05-22 02:03:48.000000 usdanuts-0.0.4/README.md
--rwxrwxrwx   0 ew        (1000) ew        (1000)       38 2023-05-22 02:36:17.897857 usdanuts-0.0.4/setup.cfg
--rwxrwxrwx   0 ew        (1000) ew        (1000)      847 2023-05-22 02:25:40.000000 usdanuts-0.0.4/setup.py
-drwxrwxrwx   0 ew        (1000) ew        (1000)        0 2023-05-22 02:36:17.816369 usdanuts-0.0.4/usdanuts/
--rwxrwxrwx   0 ew        (1000) ew        (1000)       89 2023-05-22 01:52:00.000000 usdanuts-0.0.4/usdanuts/__init__.py
--rwxrwxrwx   0 ew        (1000) ew        (1000)     3490 2023-05-22 02:35:44.000000 usdanuts-0.0.4/usdanuts/usdanuts.py
-drwxrwxrwx   0 ew        (1000) ew        (1000)        0 2023-05-22 02:36:17.866135 usdanuts-0.0.4/usdanuts.egg-info/
--rwxrwxrwx   0 ew        (1000) ew        (1000)      660 2023-05-22 02:36:17.000000 usdanuts-0.0.4/usdanuts.egg-info/PKG-INFO
--rwxrwxrwx   0 ew        (1000) ew        (1000)      188 2023-05-22 02:36:17.000000 usdanuts-0.0.4/usdanuts.egg-info/SOURCES.txt
--rwxrwxrwx   0 ew        (1000) ew        (1000)        1 2023-05-22 02:36:17.000000 usdanuts-0.0.4/usdanuts.egg-info/dependency_links.txt
--rwxrwxrwx   0 ew        (1000) ew        (1000)        9 2023-05-22 02:36:17.000000 usdanuts-0.0.4/usdanuts.egg-info/top_level.txt
+drwxrwxrwx   0 ew        (1000) ew        (1000)        0 2023-05-22 02:40:37.532697 usdanuts-0.0.5/
+-rwxrwxrwx   0 ew        (1000) ew        (1000)      660 2023-05-22 02:40:37.532697 usdanuts-0.0.5/PKG-INFO
+-rwxrwxrwx   0 ew        (1000) ew        (1000)     1605 2023-05-22 02:03:48.000000 usdanuts-0.0.5/README.md
+-rwxrwxrwx   0 ew        (1000) ew        (1000)       38 2023-05-22 02:40:37.532697 usdanuts-0.0.5/setup.cfg
+-rwxrwxrwx   0 ew        (1000) ew        (1000)      847 2023-05-22 02:38:10.000000 usdanuts-0.0.5/setup.py
+drwxrwxrwx   0 ew        (1000) ew        (1000)        0 2023-05-22 02:40:37.469639 usdanuts-0.0.5/usdanuts/
+-rwxrwxrwx   0 ew        (1000) ew        (1000)       89 2023-05-22 01:52:00.000000 usdanuts-0.0.5/usdanuts/__init__.py
+-rwxrwxrwx   0 ew        (1000) ew        (1000)     3498 2023-05-22 02:37:39.000000 usdanuts-0.0.5/usdanuts/usdanuts.py
+drwxrwxrwx   0 ew        (1000) ew        (1000)        0 2023-05-22 02:40:37.516651 usdanuts-0.0.5/usdanuts.egg-info/
+-rwxrwxrwx   0 ew        (1000) ew        (1000)      660 2023-05-22 02:40:37.000000 usdanuts-0.0.5/usdanuts.egg-info/PKG-INFO
+-rwxrwxrwx   0 ew        (1000) ew        (1000)      188 2023-05-22 02:40:37.000000 usdanuts-0.0.5/usdanuts.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ew        (1000) ew        (1000)        1 2023-05-22 02:40:37.000000 usdanuts-0.0.5/usdanuts.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ew        (1000) ew        (1000)        9 2023-05-22 02:40:37.000000 usdanuts-0.0.5/usdanuts.egg-info/top_level.txt
```

### Comparing `usdanuts-0.0.4/PKG-INFO` & `usdanuts-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: usdanuts
-Version: 0.0.4
+Version: 0.0.5
 Summary: Calls USDA FoodData Central API for food nutrient data and parses responses.
 Home-page: UNKNOWN
 Author: eliwagnercode (Eli Wagner)
 Author-email: <eliwagnercode@gmail.com>
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: nutrition,nutritional,nutrient,food,foods,pantry,diet,diets,dietary,eat,eats,eating
```

### Comparing `usdanuts-0.0.4/README.md` & `usdanuts-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `usdanuts-0.0.4/setup.py` & `usdanuts-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Calls USDA FoodData Central API for food nutrient data and parses responses.'
 
 # Setting up
 setup(
     name="usdanuts",
     version=VERSION,
     author="eliwagnercode (Eli Wagner)",
```

### Comparing `usdanuts-0.0.4/usdanuts/usdanuts.py` & `usdanuts-0.0.5/usdanuts/usdanuts.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,9 +75,9 @@
   search_list = get_search_list(search_pages)
   df = pd.DataFrame(data=search_list, index = range(len(search_list)))
   return df
 
 # Accepts Pandas DataFrame and optional filename prefix
 # Exports Pandas DataFrame as CSV
 def get_csv(df,prefix=""):
-  prefix = str(prefix) + "_" if prefix != ""
+  prefix = str(prefix) + "_" if prefix != "" else ""
   df.to_csv(f"{prefix}FDC_Search_{datetime.datetime.now()}.csv",index=False)
```

### Comparing `usdanuts-0.0.4/usdanuts.egg-info/PKG-INFO` & `usdanuts-0.0.5/usdanuts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: usdanuts
-Version: 0.0.4
+Version: 0.0.5
 Summary: Calls USDA FoodData Central API for food nutrient data and parses responses.
 Home-page: UNKNOWN
 Author: eliwagnercode (Eli Wagner)
 Author-email: <eliwagnercode@gmail.com>
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: nutrition,nutritional,nutrient,food,foods,pantry,diet,diets,dietary,eat,eats,eating
```

