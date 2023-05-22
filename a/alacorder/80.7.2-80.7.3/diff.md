# Comparing `tmp/alacorder-80.7.2.tar.gz` & `tmp/alacorder-80.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.7.2.tar", max compression
+gzip compressed data, was "alacorder-80.7.3.tar", max compression
```

## Comparing `alacorder-80.7.2.tar` & `alacorder-80.7.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.2/LICENSE
--rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.7.2/README.md
--rw-r--r--   0        0        0      746 2023-05-21 21:55:38.253512 alacorder-80.7.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-21 21:31:22.687412 alacorder-80.7.2/src/alacorder/.DS_Store
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.2/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.2/src/alacorder/__init__.py
--rw-r--r--   0        0        0   238144 2023-05-21 21:55:17.304226 alacorder-80.7.2/src/alacorder/__main__.py
--rw-r--r--   0        0        0   238144 2023-05-21 21:55:10.650312 alacorder-80.7.2/src/alacorder/alac.py
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.3/LICENSE
+-rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.7.3/README.md
+-rw-r--r--   0        0        0      746 2023-05-21 22:21:11.410329 alacorder-80.7.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-21 21:31:22.687412 alacorder-80.7.3/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.3/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.3/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   238222 2023-05-21 22:20:40.027734 alacorder-80.7.3/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   238222 2023-05-21 22:20:29.780069 alacorder-80.7.3/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.7.3/PKG-INFO
```

### Comparing `alacorder-80.7.2/LICENSE` & `alacorder-80.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.2/README.md` & `alacorder-80.7.3/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.2/pyproject.toml` & `alacorder-80.7.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.7.2"
+version = "80.7.3"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.7.2/src/alacorder/.DS_Store` & `alacorder-80.7.3/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.2/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.7.3/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.2/src/alacorder/__main__.py` & `alacorder-80.7.3/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.7.2"
+version = "80.7.3"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3858,14 +3858,15 @@
                 size=[26, 10],
                 key="SQ-OUTPUTPATH",
             ),
             sg.FolderBrowse(
                 button_text="Select Folder", button_color=("white", "black")
             ),
         ],
+        [sg.Checkbox('Criminal Only', key="SQ-CRIMINALONLY", default=False)],
         [sg.Text("Alacourt.com Credentials", font=BODY_FONT)],
         [
             sg.Text("Customer ID: "),
             sg.Input(key="SQ-CUSTOMERID", size=(16, 1)),
         ],
         [
             sg.Text("User ID:"),
```

### Comparing `alacorder-80.7.2/src/alacorder/alac.py` & `alacorder-80.7.3/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.7.2"
+version = "80.7.3"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3858,14 +3858,15 @@
                 size=[26, 10],
                 key="SQ-OUTPUTPATH",
             ),
             sg.FolderBrowse(
                 button_text="Select Folder", button_color=("white", "black")
             ),
         ],
+        [sg.Checkbox('Criminal Only', key="SQ-CRIMINALONLY", default=False)],
         [sg.Text("Alacourt.com Credentials", font=BODY_FONT)],
         [
             sg.Text("Customer ID: "),
             sg.Input(key="SQ-CUSTOMERID", size=(16, 1)),
         ],
         [
             sg.Text("User ID:"),
```

### Comparing `alacorder-80.7.2/PKG-INFO` & `alacorder-80.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.7.2
+Version: 80.7.3
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

