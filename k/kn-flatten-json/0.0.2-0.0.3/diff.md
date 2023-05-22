# Comparing `tmp/kn_flatten_json-0.0.2.tar.gz` & `tmp/kn_flatten_json-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kn_flatten_json-0.0.2.tar", last modified: Tue Jan 31 18:07:05 2023, max compression
+gzip compressed data, was "dist\kn_flatten_json-0.0.3.tar", last modified: Mon May 22 07:58:33 2023, max compression
```

## Comparing `kn_flatten_json-0.0.2.tar` & `kn_flatten_json-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 18:07:05.000000 kn_flatten_json-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-01-31 18:07:05.000000 kn_flatten_json-0.0.2/kn_flatten_json/
--rw-rw-rw-   0        0        0     1951 2023-01-24 17:09:20.000000 kn_flatten_json-0.0.2/kn_flatten_json/kn_flatten_json.py
--rw-rw-rw-   0        0        0       44 2023-01-31 18:00:14.000000 kn_flatten_json-0.0.2/kn_flatten_json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-31 18:07:05.000000 kn_flatten_json-0.0.2/kn_flatten_json.egg-info/
--rw-rw-rw-   0        0        0        1 2023-01-31 18:07:05.000000 kn_flatten_json-0.0.2/kn_flatten_json.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2428 2023-01-31 18:07:05.000000 kn_flatten_json-0.0.2/kn_flatten_json.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-01-31 18:07:05.000000 kn_flatten_json-0.0.2/kn_flatten_json.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       16 2023-01-31 18:07:05.000000 kn_flatten_json-0.0.2/kn_flatten_json.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2428 2023-01-31 18:07:05.000000 kn_flatten_json-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1300 2023-01-31 17:56:00.000000 kn_flatten_json-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-01-31 18:07:05.000000 kn_flatten_json-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1007 2023-01-31 18:06:35.000000 kn_flatten_json-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:58:33.000000 kn_flatten_json-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-22 07:58:33.000000 kn_flatten_json-0.0.3/kn_flatten_json/
+-rw-rw-rw-   0        0        0     5066 2023-05-22 07:54:02.000000 kn_flatten_json-0.0.3/kn_flatten_json/kn_flatten_json.py
+-rw-rw-rw-   0        0        0       56 2023-05-22 07:54:41.000000 kn_flatten_json-0.0.3/kn_flatten_json/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:58:33.000000 kn_flatten_json-0.0.3/kn_flatten_json.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-22 07:58:30.000000 kn_flatten_json-0.0.3/kn_flatten_json.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2268 2023-05-22 07:58:30.000000 kn_flatten_json-0.0.3/kn_flatten_json.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-22 07:58:31.000000 kn_flatten_json-0.0.3/kn_flatten_json.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       16 2023-05-22 07:58:30.000000 kn_flatten_json-0.0.3/kn_flatten_json.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2268 2023-05-22 07:58:33.000000 kn_flatten_json-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1266 2023-02-03 07:02:29.000000 kn_flatten_json-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 07:58:33.000000 kn_flatten_json-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1007 2023-05-18 06:26:24.000000 kn_flatten_json-0.0.3/setup.py
```

### Comparing `kn_flatten_json-0.0.2/kn_flatten_json.egg-info/PKG-INFO` & `kn_flatten_json-0.0.3/kn_flatten_json.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,56 @@
 Metadata-Version: 2.1
 Name: kn-flatten-json
-Version: 0.0.2
+Version: 0.0.3
 Summary: kpt_flatten_json
 Home-page: UNKNOWN
 Author: Sukriti
 Author-email: sukriti.saluja@kockpit.in
 License: UNKNOWN
 Description: 
-        # Description
-        
+        # Project description
         Kpt-flatten-json pypi package helps to flatten a dataframe containing complex datatypes like arrays and structures.
         
         
-        ## Install
         
-        $ [sudo] pip install kpt_flatten_json
+        ## Installation
         
+        $ [sudo] pip install kpt_flatten_json
         
-        ## Functions
+        ## Function
         
         kpt_flatten_json: Returns a flattened dataframe
         
-        ## Example
         
+        ## Usage/Examples
+        
+        ```python
         from kpt_flatten_json import *
         
         flatdf= kpt_flatten_json(complexdf)
-        
-         
-        
-        ----------------------complexdf-----------------------
-        
-        |batters|id|name| ppu|topping| type|
-        
-        
-        |{[{1001, Regular}...|0001|Cake|0.55|[{5001, None}, {5...|donut|
-        
-        
-        
-        -------------------------flatdf---------------------------
-        
-        
-        |id|name|ppu|type|topping_id|topping_type|batters_batter_id|batters_batter_type|
-        
-        
-        |0001|Cake|0.55|donut|      5001|                None|             1001|            Regular|
-        
-        |0001|Cake|0.55|donut|      5001|                None|             1002|          Chocolate|
-        
-        |0001|Cake|0.55|donut|      5001|                None|             1003|          Blueberry|
-        
-        |0001|Cake|0.55|donut|      5001|                None|             1004|       Devil's Food|
-        
-        |0001|Cake|0.55|donut|      5002|              Glazed|             1001|            Regular|
-        
-        |0001|Cake|0.55|donut|      5002|              Glazed|             1002|          Chocolate|
-        
-        |0001|Cake|0.55|donut|      5002|              Glazed|             1003|          Blueberry|
+        ```
         
         
+        ## Complex Dataframe
         
         
+        | batters| id| name | ppu | topping| type               |
+        | :-------- | :------- | :------------------------- |:-------- | :------- | :------------------------- |
+        | {[{1001, Regular}... | 0001 | Cake|0.55 | [{5001, None}, {5... | donut|
+        
+        ## Flattened Dataframe
+        | id| name| ppu | type | topping_id | topping_type               | batters_batter_id | batters_batter_type               |
+        | :-------- | :------- | :------------------------- |:-------- | :------- | :------------------------- |:-------- | :------- |
+        |0001|Cake|0.55|donut| 5001| None| 1001| Regular|
+        |0001|Cake|0.55|donut| 5001| None| 1002| Chocolate|
+        |0001|Cake|0.55|donut| 5001| None| 1003| Blueberry|
+        |0001|Cake|0.55|donut| 5001| None| 1004| Devil's Food|
+        |0001|Cake|0.55|donut| 5002| Glazed| 1001| Regular|
+        |0001|Cake|0.55|donut| 5002| Glazed| 1002| Chocolate|
+        |0001|Cake|0.55|donut| 5002| Glazed| 1003| Blueberry|
 Keywords: flatten,json,normalize,normalize pyspark dataframe,complex datatypes,flatten dataframe
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `kn_flatten_json-0.0.2/PKG-INFO` & `kn_flatten_json-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,56 @@
 Metadata-Version: 2.1
 Name: kn_flatten_json
-Version: 0.0.2
+Version: 0.0.3
 Summary: kpt_flatten_json
 Home-page: UNKNOWN
 Author: Sukriti
 Author-email: sukriti.saluja@kockpit.in
 License: UNKNOWN
 Description: 
-        # Description
-        
+        # Project description
         Kpt-flatten-json pypi package helps to flatten a dataframe containing complex datatypes like arrays and structures.
         
         
-        ## Install
         
-        $ [sudo] pip install kpt_flatten_json
+        ## Installation
         
+        $ [sudo] pip install kpt_flatten_json
         
-        ## Functions
+        ## Function
         
         kpt_flatten_json: Returns a flattened dataframe
         
-        ## Example
         
+        ## Usage/Examples
+        
+        ```python
         from kpt_flatten_json import *
         
         flatdf= kpt_flatten_json(complexdf)
-        
-         
-        
-        ----------------------complexdf-----------------------
-        
-        |batters|id|name| ppu|topping| type|
-        
-        
-        |{[{1001, Regular}...|0001|Cake|0.55|[{5001, None}, {5...|donut|
-        
-        
-        
-        -------------------------flatdf---------------------------
-        
-        
-        |id|name|ppu|type|topping_id|topping_type|batters_batter_id|batters_batter_type|
-        
-        
-        |0001|Cake|0.55|donut|      5001|                None|             1001|            Regular|
-        
-        |0001|Cake|0.55|donut|      5001|                None|             1002|          Chocolate|
-        
-        |0001|Cake|0.55|donut|      5001|                None|             1003|          Blueberry|
-        
-        |0001|Cake|0.55|donut|      5001|                None|             1004|       Devil's Food|
-        
-        |0001|Cake|0.55|donut|      5002|              Glazed|             1001|            Regular|
-        
-        |0001|Cake|0.55|donut|      5002|              Glazed|             1002|          Chocolate|
-        
-        |0001|Cake|0.55|donut|      5002|              Glazed|             1003|          Blueberry|
+        ```
         
         
+        ## Complex Dataframe
         
         
+        | batters| id| name | ppu | topping| type               |
+        | :-------- | :------- | :------------------------- |:-------- | :------- | :------------------------- |
+        | {[{1001, Regular}... | 0001 | Cake|0.55 | [{5001, None}, {5... | donut|
+        
+        ## Flattened Dataframe
+        | id| name| ppu | type | topping_id | topping_type               | batters_batter_id | batters_batter_type               |
+        | :-------- | :------- | :------------------------- |:-------- | :------- | :------------------------- |:-------- | :------- |
+        |0001|Cake|0.55|donut| 5001| None| 1001| Regular|
+        |0001|Cake|0.55|donut| 5001| None| 1002| Chocolate|
+        |0001|Cake|0.55|donut| 5001| None| 1003| Blueberry|
+        |0001|Cake|0.55|donut| 5001| None| 1004| Devil's Food|
+        |0001|Cake|0.55|donut| 5002| Glazed| 1001| Regular|
+        |0001|Cake|0.55|donut| 5002| Glazed| 1002| Chocolate|
+        |0001|Cake|0.55|donut| 5002| Glazed| 1003| Blueberry|
 Keywords: flatten,json,normalize,normalize pyspark dataframe,complex datatypes,flatten dataframe
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `kn_flatten_json-0.0.2/setup.py` & `kn_flatten_json-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 from pathlib import Path
 this_directory = Path(__file__).parent
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'kpt_flatten_json'
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 
 # Setting up
 setup(
     name="kn_flatten_json",
```

