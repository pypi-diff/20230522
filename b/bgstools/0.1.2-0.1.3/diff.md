# Comparing `tmp/bgstools-0.1.2.tar.gz` & `tmp/bgstools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgstools-0.1.2.tar", max compression
+gzip compressed data, was "bgstools-0.1.3.tar", max compression
```

## Comparing `bgstools-0.1.2.tar` & `bgstools-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0       72 2023-05-22 09:38:31.760561 bgstools-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-03 11:32:59.064694 bgstools-0.1.2/bgstools/__init__.py
--rw-r--r--   0        0        0      339 2023-05-22 15:45:26.380252 bgstools-0.1.2/bgstools/bgstools.py
--rw-r--r--   0        0        0        0 2023-05-19 11:22:49.081592 bgstools-0.1.2/bgstools/datastorage/__init__.py
--rw-r--r--   0        0        0     4950 2023-05-19 11:22:49.081592 bgstools-0.1.2/bgstools/datastorage/datastorage.py
--rw-r--r--   0        0        0        0 2023-05-03 11:53:10.602842 bgstools-0.1.2/bgstools/io/__init__.py
--rw-r--r--   0        0        0     2112 2023-05-22 15:44:57.697847 bgstools-0.1.2/bgstools/io/io.py
--rw-r--r--   0        0        0        0 2023-05-03 11:53:10.542842 bgstools-0.1.2/bgstools/spatial/__init__.py
--rw-r--r--   0        0        0     2654 2023-05-03 11:53:10.542842 bgstools-0.1.2/bgstools/spatial/spatial.py
--rw-r--r--   0        0        0        0 2023-05-22 15:59:56.616803 bgstools-0.1.2/bgstools/stt/__init__.py
--rw-r--r--   0        0        0     2180 2023-05-22 16:11:53.523910 bgstools-0.1.2/bgstools/stt/stt.py
--rw-r--r--   0        0        0        0 2023-05-03 11:53:10.492843 bgstools-0.1.2/bgstools/utils/__init__.py
--rw-r--r--   0        0        0      972 2023-05-03 11:53:10.492843 bgstools-0.1.2/bgstools/utils/utils.py
--rw-r--r--   0        0        0      373 2023-05-22 16:23:18.612932 bgstools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 bgstools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-05-22 09:38:31.760561 bgstools-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 11:32:59.064694 bgstools-0.1.3/bgstools/__init__.py
+-rw-r--r--   0        0        0       64 2023-05-22 20:01:20.000000 bgstools-0.1.3/bgstools/datastorage/__init__.py
+-rw-r--r--   0        0        0     5014 2023-05-22 20:29:18.000000 bgstools-0.1.3/bgstools/datastorage/datastorage.py
+-rw-r--r--   0        0        0       50 2023-05-22 20:28:44.000000 bgstools-0.1.3/bgstools/io/__init__.py
+-rw-r--r--   0        0        0     2112 2023-05-22 17:37:56.000000 bgstools-0.1.3/bgstools/io/io.py
+-rw-r--r--   0        0        0      122 2023-05-22 20:28:18.000000 bgstools-0.1.3/bgstools/spatial/__init__.py
+-rw-r--r--   0        0        0     2654 2023-05-22 17:37:56.000000 bgstools-0.1.3/bgstools/spatial/spatial.py
+-rw-r--r--   0        0        0       39 2023-05-22 20:27:28.000000 bgstools-0.1.3/bgstools/stt/__init__.py
+-rw-r--r--   0        0        0     2176 2023-05-22 20:27:34.000000 bgstools-0.1.3/bgstools/stt/stt.py
+-rw-r--r--   0        0        0       99 2023-05-22 20:25:04.000000 bgstools-0.1.3/bgstools/utils/__init__.py
+-rw-r--r--   0        0        0     2971 2023-05-22 20:24:36.000000 bgstools-0.1.3/bgstools/utils/utils.py
+-rw-r--r--   0        0        0      373 2023-05-22 20:50:44.761986 bgstools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 bgstools-0.1.3/PKG-INFO
```

### Comparing `bgstools-0.1.2/bgstools/datastorage/datastorage.py` & `bgstools-0.1.3/bgstools/datastorage/datastorage.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,7 +150,8 @@
         """
         self.storage_strategy.update_data(update_func)
 
     def delete_data(self):
         """Deletes the data stored by the current storage strategy."""
         self.storage_strategy.delete_data() 
 
+from .datastorage import DataStore, StorageStrategy, YamlStorage
```

### Comparing `bgstools-0.1.2/bgstools/io/io.py` & `bgstools-0.1.3/bgstools/io/io.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.2/bgstools/spatial/spatial.py` & `bgstools-0.1.3/bgstools/spatial/spatial.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.2/bgstools/stt/stt.py` & `bgstools-0.1.3/bgstools/stt/stt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # streamlit tools (stt)
 from collections import OrderedDict
 from typing import Optional, Tuple, Any
-from bgstools.io import script_as_module
+from ..utils import script_as_module
 import streamlit as st
 
 
 def build_activities_menu(
     activities_dict: OrderedDict[str, dict], 
     label: str, 
     key: str,
```

### Comparing `bgstools-0.1.2/PKG-INFO` & `bgstools-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgstools
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: José Beltrán
 Author-email: 102664984+jose-begeospatial@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

