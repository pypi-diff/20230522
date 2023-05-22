# Comparing `tmp/usdanuts-0.0.3.tar.gz` & `tmp/usdanuts-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usdanuts-0.0.3.tar", last modified: Mon May 22 01:52:17 2023, max compression
+gzip compressed data, was "usdanuts-0.0.4.tar", last modified: Mon May 22 02:36:17 2023, max compression
```

## Comparing `usdanuts-0.0.3.tar` & `usdanuts-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 ew        (1000) ew        (1000)        0 2023-05-22 01:52:17.671724 usdanuts-0.0.3/
--rwxrwxrwx   0 ew        (1000) ew        (1000)      660 2023-05-22 01:52:17.671724 usdanuts-0.0.3/PKG-INFO
--rwxrwxrwx   0 ew        (1000) ew        (1000)     1601 2023-05-22 00:29:37.000000 usdanuts-0.0.3/README.md
--rwxrwxrwx   0 ew        (1000) ew        (1000)       38 2023-05-22 01:52:17.671724 usdanuts-0.0.3/setup.cfg
--rwxrwxrwx   0 ew        (1000) ew        (1000)      847 2023-05-22 01:51:48.000000 usdanuts-0.0.3/setup.py
-drwxrwxrwx   0 ew        (1000) ew        (1000)        0 2023-05-22 01:52:17.607945 usdanuts-0.0.3/usdanuts/
--rwxrwxrwx   0 ew        (1000) ew        (1000)       89 2023-05-22 01:52:00.000000 usdanuts-0.0.3/usdanuts/__init__.py
--rwxrwxrwx   0 ew        (1000) ew        (1000)     3444 2023-05-22 00:30:19.000000 usdanuts-0.0.3/usdanuts/usdanuts.py
-drwxrwxrwx   0 ew        (1000) ew        (1000)        0 2023-05-22 01:52:17.663551 usdanuts-0.0.3/usdanuts.egg-info/
--rwxrwxrwx   0 ew        (1000) ew        (1000)      660 2023-05-22 01:52:17.000000 usdanuts-0.0.3/usdanuts.egg-info/PKG-INFO
--rwxrwxrwx   0 ew        (1000) ew        (1000)      188 2023-05-22 01:52:17.000000 usdanuts-0.0.3/usdanuts.egg-info/SOURCES.txt
--rwxrwxrwx   0 ew        (1000) ew        (1000)        1 2023-05-22 01:52:17.000000 usdanuts-0.0.3/usdanuts.egg-info/dependency_links.txt
--rwxrwxrwx   0 ew        (1000) ew        (1000)        9 2023-05-22 01:52:17.000000 usdanuts-0.0.3/usdanuts.egg-info/top_level.txt
+drwxrwxrwx   0 ew        (1000) ew        (1000)        0 2023-05-22 02:36:17.895702 usdanuts-0.0.4/
+-rwxrwxrwx   0 ew        (1000) ew        (1000)      660 2023-05-22 02:36:17.892675 usdanuts-0.0.4/PKG-INFO
+-rwxrwxrwx   0 ew        (1000) ew        (1000)     1605 2023-05-22 02:03:48.000000 usdanuts-0.0.4/README.md
+-rwxrwxrwx   0 ew        (1000) ew        (1000)       38 2023-05-22 02:36:17.897857 usdanuts-0.0.4/setup.cfg
+-rwxrwxrwx   0 ew        (1000) ew        (1000)      847 2023-05-22 02:25:40.000000 usdanuts-0.0.4/setup.py
+drwxrwxrwx   0 ew        (1000) ew        (1000)        0 2023-05-22 02:36:17.816369 usdanuts-0.0.4/usdanuts/
+-rwxrwxrwx   0 ew        (1000) ew        (1000)       89 2023-05-22 01:52:00.000000 usdanuts-0.0.4/usdanuts/__init__.py
+-rwxrwxrwx   0 ew        (1000) ew        (1000)     3490 2023-05-22 02:35:44.000000 usdanuts-0.0.4/usdanuts/usdanuts.py
+drwxrwxrwx   0 ew        (1000) ew        (1000)        0 2023-05-22 02:36:17.866135 usdanuts-0.0.4/usdanuts.egg-info/
+-rwxrwxrwx   0 ew        (1000) ew        (1000)      660 2023-05-22 02:36:17.000000 usdanuts-0.0.4/usdanuts.egg-info/PKG-INFO
+-rwxrwxrwx   0 ew        (1000) ew        (1000)      188 2023-05-22 02:36:17.000000 usdanuts-0.0.4/usdanuts.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ew        (1000) ew        (1000)        1 2023-05-22 02:36:17.000000 usdanuts-0.0.4/usdanuts.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ew        (1000) ew        (1000)        9 2023-05-22 02:36:17.000000 usdanuts-0.0.4/usdanuts.egg-info/top_level.txt
```

### Comparing `usdanuts-0.0.3/PKG-INFO` & `usdanuts-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: usdanuts
-Version: 0.0.3
+Version: 0.0.4
 Summary: Calls USDA FoodData Central API for food nutrient data and parses responses.
 Home-page: UNKNOWN
 Author: eliwagnercode (Eli Wagner)
 Author-email: <eliwagnercode@gmail.com>
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: nutrition,nutritional,nutrient,food,foods,pantry,diet,diets,dietary,eat,eats,eating
```

### Comparing `usdanuts-0.0.3/README.md` & `usdanuts-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# nuts
+# usdanuts
 Nutrient Upgraded Tally System
 
 This Python project was inspired in part by the Nutrient Object Management System (noms) package, created by Noah Tren (https://github.com/noahtren/noms). 
 The noms package utilizes the USDA Standard Reference Food Composition Database, which is now decommissioned; the nuts package calls the currently active USDA FoodData Central API.
 
 The nuts package is designed to: 
 - Take a food query from the user.
```

### Comparing `usdanuts-0.0.3/setup.py` & `usdanuts-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Calls USDA FoodData Central API for food nutrient data and parses responses.'
 
 # Setting up
 setup(
     name="usdanuts",
     version=VERSION,
     author="eliwagnercode (Eli Wagner)",
```

### Comparing `usdanuts-0.0.3/usdanuts/usdanuts.py` & `usdanuts-0.0.4/usdanuts/usdanuts.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Accepts query, data types, and API key
 # Returns url to call API
 def get_url(query, 
               dataType = "Foundation,Branded,SRLegacy,Survey(FNDDS)", 
               API_KEY="DEMO_KEY", 
               pageNumber=1):
   query, dataType, API_KEY, pageNumber = \
-  str(query), str(dataType), str(API_KEY), str(pageNumber)
+  str(query), str(dataType).replace(" ",""), str(API_KEY), str(pageNumber)
   url = f"https://api.nal.usda.gov/fdc/v1/foods/search?api_key={API_KEY}"\
         f"&sortBy=publishedDate&sortOrder=desc&pageSize=100"\
         f"&dataType={dataType}&pageNumber={pageNumber}&query={query}"
   return url
 
 # Makes API call for each results page
 # Accepts query, data types, and API key
@@ -75,9 +75,9 @@
   search_list = get_search_list(search_pages)
   df = pd.DataFrame(data=search_list, index = range(len(search_list)))
   return df
 
 # Accepts Pandas DataFrame and optional filename prefix
 # Exports Pandas DataFrame as CSV
 def get_csv(df,prefix=""):
-  prefix = str(prefix)
-  df.to_csv(f"FDC_Search_{datetime.datetime.now()}.csv",index=False)
+  prefix = str(prefix) + "_" if prefix != ""
+  df.to_csv(f"{prefix}FDC_Search_{datetime.datetime.now()}.csv",index=False)
```

### Comparing `usdanuts-0.0.3/usdanuts.egg-info/PKG-INFO` & `usdanuts-0.0.4/usdanuts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: usdanuts
-Version: 0.0.3
+Version: 0.0.4
 Summary: Calls USDA FoodData Central API for food nutrient data and parses responses.
 Home-page: UNKNOWN
 Author: eliwagnercode (Eli Wagner)
 Author-email: <eliwagnercode@gmail.com>
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: nutrition,nutritional,nutrient,food,foods,pantry,diet,diets,dietary,eat,eats,eating
```

