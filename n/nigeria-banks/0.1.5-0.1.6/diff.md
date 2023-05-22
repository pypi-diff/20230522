# Comparing `tmp/nigeria_banks-0.1.5.tar.gz` & `tmp/nigeria_banks-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nigeria_banks-0.1.5.tar", last modified: Fri May 19 15:34:37 2023, max compression
+gzip compressed data, was "nigeria_banks-0.1.6.tar", last modified: Mon May 22 00:05:30 2023, max compression
```

## Comparing `nigeria_banks-0.1.5.tar` & `nigeria_banks-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:37.821495 nigeria_banks-0.1.5/cbn_banks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/cbn_banks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/cbn_banks/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/cbn_banks/bank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/cbn_banks/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/cbn_banks/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/cbn_banks/database/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/nigeria_banks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/nigeria_banks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/nigeria_banks/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/nigeria_banks/bank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/nigeria_banks/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/nigeria_banks/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62044 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/nigeria_banks/database/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/nigeria_banks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-19 15:34:37.000000 nigeria_banks-0.1.5/nigeria_banks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-19 15:34:37.000000 nigeria_banks-0.1.5/nigeria_banks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:34:37.000000 nigeria_banks-0.1.5/nigeria_banks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 15:34:37.000000 nigeria_banks-0.1.5/nigeria_banks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:05:30.901164 nigeria_banks-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-22 00:05:21.000000 nigeria_banks-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 00:05:21.000000 nigeria_banks-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-22 00:05:30.901164 nigeria_banks-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-22 00:05:21.000000 nigeria_banks-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:05:30.901164 nigeria_banks-0.1.6/nigeria_banks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 00:05:21.000000 nigeria_banks-0.1.6/nigeria_banks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 00:05:21.000000 nigeria_banks-0.1.6/nigeria_banks/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-22 00:05:21.000000 nigeria_banks-0.1.6/nigeria_banks/bank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:05:30.901164 nigeria_banks-0.1.6/nigeria_banks/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 00:05:21.000000 nigeria_banks-0.1.6/nigeria_banks/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62044 2023-05-22 00:05:21.000000 nigeria_banks-0.1.6/nigeria_banks/database/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:05:30.901164 nigeria_banks-0.1.6/nigeria_banks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-22 00:05:30.000000 nigeria_banks-0.1.6/nigeria_banks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-22 00:05:30.000000 nigeria_banks-0.1.6/nigeria_banks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 00:05:30.000000 nigeria_banks-0.1.6/nigeria_banks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 00:05:30.000000 nigeria_banks-0.1.6/nigeria_banks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 00:05:30.901164 nigeria_banks-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-22 00:05:21.000000 nigeria_banks-0.1.6/setup.py
```

### Comparing `nigeria_banks-0.1.5/LICENSE` & `nigeria_banks-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nigeria_banks-0.1.5/PKG-INFO` & `nigeria_banks-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nigeria_banks
-Version: 0.1.5
+Version: 0.1.6
 Summary: Get details of specific bank in Nigeria
 Home-page: https://github.com/Josephchinedu/nigeria_banks
 Author: Devjoseph
 Author-email: joseph4jubilant@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nigeria_banks-0.1.5/README.md` & `nigeria_banks-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nigeria_banks-0.1.5/cbn_banks/bank.py` & `nigeria_banks-0.1.6/nigeria_banks/bank.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from nigeria_banks.database.db import bankdb
 
 
 def getBank(name=None, bank_code=None, cbn_code=None, ussd_code = None):
     data = bankdb()
     if name:
         for bank in data:
-            if (bank["bank_short_name"]).lower() == name.lower():
+            if bank["bank_short_name"] == name:
                 return bank
     elif bank_code:
         for bank in data:
             if bank["bank_code"] == bank_code:
                 return bank
     elif cbn_code:
         for bank in data:
```

### Comparing `nigeria_banks-0.1.5/nigeria_banks/database/db.py` & `nigeria_banks-0.1.6/nigeria_banks/database/db.py`

 * *Files identical despite different names*

### Comparing `nigeria_banks-0.1.5/nigeria_banks.egg-info/PKG-INFO` & `nigeria_banks-0.1.6/nigeria_banks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nigeria-banks
-Version: 0.1.5
+Version: 0.1.6
 Summary: Get details of specific bank in Nigeria
 Home-page: https://github.com/Josephchinedu/nigeria_banks
 Author: Devjoseph
 Author-email: joseph4jubilant@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nigeria_banks-0.1.5/setup.py` & `nigeria_banks-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 NAME = 'nigeria_banks'
 DESCRIPTION = 'Get details of specific bank in Nigeria'
 URL = 'https://github.com/Josephchinedu/nigeria_banks'
 EMAIL = 'joseph4jubilant@gmail.com'
 AUTHOR = 'Devjoseph'
 REQUIRES_PYTHON = '>=3.7.9'
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
 EXTRAS = {
```

