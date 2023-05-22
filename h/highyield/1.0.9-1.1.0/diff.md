# Comparing `tmp/highyield-1.0.9.tar.gz` & `tmp/highyield-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highyield-1.0.9.tar", last modified: Wed May 17 01:26:49 2023, max compression
+gzip compressed data, was "highyield-1.1.0.tar", last modified: Mon May 22 21:03:54 2023, max compression
```

## Comparing `highyield-1.0.9.tar` & `highyield-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-17 01:26:49.197835 highyield-1.0.9/
--rw-r--r--   0 v1         (502) wheel        (0)    35129 2023-01-06 21:21:15.000000 highyield-1.0.9/LICENSE
--rw-r--r--   0 v1         (502) wheel        (0)       29 2023-01-06 21:17:34.000000 highyield-1.0.9/MANIFEST.in
--rw-r--r--   0 v1         (502) wheel        (0)     1980 2023-05-17 01:26:49.197602 highyield-1.0.9/PKG-INFO
--rw-r--r--   0 v1         (502) wheel        (0)     1469 2023-05-17 01:03:18.000000 highyield-1.0.9/README.md
-drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-17 01:26:49.196186 highyield-1.0.9/highyield/
--rw-r--r--   0 v1         (502) wheel        (0)      198 2023-01-06 23:04:04.000000 highyield-1.0.9/highyield/__init__.py
--rw-r--r--   0 v1         (502) wheel        (0)      491 2023-05-17 01:12:26.000000 highyield-1.0.9/highyield/basics.py
--rw-r--r--   0 v1         (502) wheel        (0)     3075 2023-01-02 19:44:42.000000 highyield-1.0.9/highyield/converter.py
--rw-r--r--   0 v1         (502) wheel        (0)     4265 2023-01-04 22:06:46.000000 highyield-1.0.9/highyield/copy.py
--rw-r--r--   0 v1         (502) wheel        (0)     1691 2023-01-18 22:18:24.000000 highyield-1.0.9/highyield/create.py
-drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-17 01:26:49.197045 highyield-1.0.9/highyield/data/
--rw-r--r--   0 v1         (502) wheel        (0)     1906 2023-01-03 23:05:21.000000 highyield-1.0.9/highyield/data/RR.csv
--rw-r--r--   0 v1         (502) wheel        (0)      346 2023-01-07 14:41:36.000000 highyield-1.0.9/highyield/imports.py
--rw-r--r--   0 v1         (502) wheel        (0)     1534 2023-01-06 18:44:52.000000 highyield-1.0.9/highyield/pdf.py
--rw-r--r--   0 v1         (502) wheel        (0)     1330 2023-01-15 13:10:42.000000 highyield-1.0.9/highyield/rename.py
--rw-r--r--   0 v1         (502) wheel        (0)     4878 2023-01-07 14:45:09.000000 highyield-1.0.9/highyield/tts.py
-drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-17 01:26:49.196931 highyield-1.0.9/highyield.egg-info/
--rw-r--r--   0 v1         (502) wheel        (0)     1980 2023-05-17 01:26:49.000000 highyield-1.0.9/highyield.egg-info/PKG-INFO
--rw-r--r--   0 v1         (502) wheel        (0)      449 2023-05-17 01:26:49.000000 highyield-1.0.9/highyield.egg-info/SOURCES.txt
--rw-r--r--   0 v1         (502) wheel        (0)        1 2023-05-17 01:26:49.000000 highyield-1.0.9/highyield.egg-info/dependency_links.txt
--rw-r--r--   0 v1         (502) wheel        (0)        1 2023-01-06 23:47:02.000000 highyield-1.0.9/highyield.egg-info/not-zip-safe
--rw-r--r--   0 v1         (502) wheel        (0)       30 2023-05-17 01:26:49.000000 highyield-1.0.9/highyield.egg-info/requires.txt
--rw-r--r--   0 v1         (502) wheel        (0)       10 2023-05-17 01:26:49.000000 highyield-1.0.9/highyield.egg-info/top_level.txt
--rw-r--r--   0 v1         (502) wheel        (0)      103 2023-01-06 22:57:09.000000 highyield-1.0.9/pyproject.toml
--rw-r--r--   0 v1         (502) wheel        (0)       38 2023-05-17 01:26:49.197891 highyield-1.0.9/setup.cfg
--rw-r--r--   0 v1         (502) wheel        (0)      993 2023-05-17 01:03:39.000000 highyield-1.0.9/setup.py
+drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-22 21:03:54.406242 highyield-1.1.0/
+-rw-r--r--   0 v1         (502) wheel        (0)    35129 2023-01-06 21:21:15.000000 highyield-1.1.0/LICENSE
+-rw-r--r--   0 v1         (502) wheel        (0)       29 2023-01-06 21:17:34.000000 highyield-1.1.0/MANIFEST.in
+-rw-r--r--   0 v1         (502) wheel        (0)     1976 2023-05-22 21:03:54.406113 highyield-1.1.0/PKG-INFO
+-rw-r--r--   0 v1         (502) wheel        (0)     1465 2023-05-22 20:36:54.000000 highyield-1.1.0/README.md
+drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-22 21:03:54.404762 highyield-1.1.0/highyield/
+-rw-r--r--   0 v1         (502) wheel        (0)      198 2023-01-06 23:04:04.000000 highyield-1.1.0/highyield/__init__.py
+-rw-r--r--   0 v1         (502) wheel        (0)     2138 2023-05-22 20:40:49.000000 highyield-1.1.0/highyield/basics.py
+-rw-r--r--   0 v1         (502) wheel        (0)     3057 2023-05-22 20:51:33.000000 highyield-1.1.0/highyield/converter.py
+-rw-r--r--   0 v1         (502) wheel        (0)     4256 2023-05-22 20:28:18.000000 highyield-1.1.0/highyield/copy.py
+-rw-r--r--   0 v1         (502) wheel        (0)     1679 2023-05-22 20:28:31.000000 highyield-1.1.0/highyield/create.py
+drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-22 21:03:54.405820 highyield-1.1.0/highyield/data/
+-rw-r--r--   0 v1         (502) wheel        (0)     1906 2023-01-03 23:05:21.000000 highyield-1.1.0/highyield/data/RR.csv
+-rw-r--r--   0 v1         (502) wheel        (0)      346 2023-01-07 14:41:36.000000 highyield-1.1.0/highyield/imports.py
+-rw-r--r--   0 v1         (502) wheel        (0)     1516 2023-05-22 20:28:53.000000 highyield-1.1.0/highyield/pdf.py
+-rw-r--r--   0 v1         (502) wheel        (0)     1328 2023-05-22 20:29:48.000000 highyield-1.1.0/highyield/rename.py
+-rw-r--r--   0 v1         (502) wheel        (0)     4842 2023-05-22 20:35:23.000000 highyield-1.1.0/highyield/tts.py
+drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-22 21:03:54.405703 highyield-1.1.0/highyield.egg-info/
+-rw-r--r--   0 v1         (502) wheel        (0)     1976 2023-05-22 21:03:54.000000 highyield-1.1.0/highyield.egg-info/PKG-INFO
+-rw-r--r--   0 v1         (502) wheel        (0)      449 2023-05-22 21:03:54.000000 highyield-1.1.0/highyield.egg-info/SOURCES.txt
+-rw-r--r--   0 v1         (502) wheel        (0)        1 2023-05-22 21:03:54.000000 highyield-1.1.0/highyield.egg-info/dependency_links.txt
+-rw-r--r--   0 v1         (502) wheel        (0)        1 2023-01-06 23:47:02.000000 highyield-1.1.0/highyield.egg-info/not-zip-safe
+-rw-r--r--   0 v1         (502) wheel        (0)       39 2023-05-22 21:03:54.000000 highyield-1.1.0/highyield.egg-info/requires.txt
+-rw-r--r--   0 v1         (502) wheel        (0)       10 2023-05-22 21:03:54.000000 highyield-1.1.0/highyield.egg-info/top_level.txt
+-rw-r--r--   0 v1         (502) wheel        (0)      103 2023-01-06 22:57:09.000000 highyield-1.1.0/pyproject.toml
+-rw-r--r--   0 v1         (502) wheel        (0)       38 2023-05-22 21:03:54.406278 highyield-1.1.0/setup.cfg
+-rw-r--r--   0 v1         (502) wheel        (0)     1013 2023-05-22 20:37:41.000000 highyield-1.1.0/setup.py
```

### Comparing `highyield-1.0.9/LICENSE` & `highyield-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `highyield-1.0.9/PKG-INFO` & `highyield-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: highyield
-Version: 1.0.9
+Version: 1.1.0
 Summary: Collection of high-yield functions intended to simplify and automate specific tasks.
 Home-page: https://github.com/kenf1/High-Yield
 Author: KF
 Author-email: kenfv1@outlook.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## highyield `<a href="https://kenf1.github.io/Rendered/highyield%20Documentation/"><img src="https://raw.githubusercontent.com/kenf1/Rendered/main/Hex_Sticker/High-Yield.png" align="right" height="138.5" />``</a>`
+## highyield <a href="https://kenf1.github.io/Rendered/highyield%20Documentation/"><img src="https://raw.githubusercontent.com/kenf1/Rendered/main/Hex_Sticker/High-Yield.png" align="right" height="138.5" /></a>
 
 [![PyPI](https://img.shields.io/pypi/v/highyield.svg)](https://pypi.org/project/highyield) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0) [![](https://img.shields.io/badge/-Documentation-yellow)](https://kenf1.github.io/Rendered/highyield%20Documentation/)
 
 `highyield` is a Python package containing a collection of high-yield functions (grouped by modules) intended to simplify and automate specific tasks.
 
 This package requires Python >= 3.8 due to reliance on [`pandas` package](https://pypi.org/project/pandas/).
 
@@ -39,15 +39,15 @@
 
 ### Dependencies
 
 The table below lists the dependencies for each module within this package:
 
 | Module    | Packages             |
 | --------- | -------------------- |
-| basics    | os                   |
+| basics    | os, requests         |
 | converter | os, pandas, docx2pdf |
 | copy      | os, shutil, pandas   |
 | create    | os, shutil           |
 | imports   | importlib, pandas    |
 | pdf       | os, pypdf            |
 | rename    | os, re               |
 | tts       | pyttsx3, pandas      |
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: highyield Version: 1.0.9 Summary: Collection of
+Metadata-Version: 2.1 Name: highyield Version: 1.1.0 Summary: Collection of
 high-yield functions intended to simplify and automate specific tasks. Home-
 page: https://github.com/kenf1/High-Yield Author: KF Author-email:
 kenfv1@outlook.com License: GPLv3 Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE ## highyield `
+Description-Content-Type: text/markdown License-File: LICENSE ## highyield
 [https://raw.githubusercontent.com/kenf1/Rendered/main/Hex_Sticker/High-
-Yield.png]``` [![PyPI](https://img.shields.io/pypi/v/highyield.svg)](https://
+Yield.png] [![PyPI](https://img.shields.io/pypi/v/highyield.svg)](https://
 pypi.org/project/highyield) [![License: GPL v3](https://img.shields.io/badge/
 License-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0) [![]
 (https://img.shields.io/badge/-Documentation-yellow)](https://kenf1.github.io/
 Rendered/highyield%20Documentation/) `highyield` is a Python package containing
 a collection of high-yield functions (grouped by modules) intended to simplify
 and automate specific tasks. This package requires Python >= 3.8 due to
 reliance on [`pandas` package](https://pypi.org/project/pandas/). ### Install
 To install, open the terminal and type in the following. For Windows and Linux:
 ```{python} pip install highyield ``` For macOS: ```{python} python3 -m pip
 install highyield ``` ### Dependencies The table below lists the dependencies
 for each module within this package: | Module | Packages | | --------- | ------
--------------- | | basics | os | | converter | os, pandas, docx2pdf | | copy |
-os, shutil, pandas | | create | os, shutil | | imports | importlib, pandas | |
-pdf | os, pypdf | | rename | os, re | | tts | pyttsx3, pandas |
+-------------- | | basics | os, requests | | converter | os, pandas, docx2pdf |
+| copy | os, shutil, pandas | | create | os, shutil | | imports | importlib,
+pandas | | pdf | os, pypdf | | rename | os, re | | tts | pyttsx3, pandas |
```

### Comparing `highyield-1.0.9/README.md` & `highyield-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## highyield `<a href="https://kenf1.github.io/Rendered/highyield%20Documentation/"><img src="https://raw.githubusercontent.com/kenf1/Rendered/main/Hex_Sticker/High-Yield.png" align="right" height="138.5" />``</a>`
+## highyield <a href="https://kenf1.github.io/Rendered/highyield%20Documentation/"><img src="https://raw.githubusercontent.com/kenf1/Rendered/main/Hex_Sticker/High-Yield.png" align="right" height="138.5" /></a>
 
 [![PyPI](https://img.shields.io/pypi/v/highyield.svg)](https://pypi.org/project/highyield) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0) [![](https://img.shields.io/badge/-Documentation-yellow)](https://kenf1.github.io/Rendered/highyield%20Documentation/)
 
 `highyield` is a Python package containing a collection of high-yield functions (grouped by modules) intended to simplify and automate specific tasks.
 
 This package requires Python >= 3.8 due to reliance on [`pandas` package](https://pypi.org/project/pandas/).
 
@@ -24,15 +24,15 @@
 
 ### Dependencies
 
 The table below lists the dependencies for each module within this package:
 
 | Module    | Packages             |
 | --------- | -------------------- |
-| basics    | os                   |
+| basics    | os, requests         |
 | converter | os, pandas, docx2pdf |
 | copy      | os, shutil, pandas   |
 | create    | os, shutil           |
 | imports   | importlib, pandas    |
 | pdf       | os, pypdf            |
 | rename    | os, re               |
 | tts       | pyttsx3, pandas      |
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-## highyield `[https://raw.githubusercontent.com/kenf1/Rendered/main/
-Hex_Sticker/High-Yield.png]``` [![PyPI](https://img.shields.io/pypi/v/
+## highyield [https://raw.githubusercontent.com/kenf1/Rendered/main/
+Hex_Sticker/High-Yield.png] [![PyPI](https://img.shields.io/pypi/v/
 highyield.svg)](https://pypi.org/project/highyield) [![License: GPL v3](https:/
 /img.shields.io/badge/License-GPLv3-brightgreen.svg)](https://www.gnu.org/
 licenses/gpl-3.0) [![](https://img.shields.io/badge/-Documentation-yellow)]
 (https://kenf1.github.io/Rendered/highyield%20Documentation/) `highyield` is a
 Python package containing a collection of high-yield functions (grouped by
 modules) intended to simplify and automate specific tasks. This package
 requires Python >= 3.8 due to reliance on [`pandas` package](https://pypi.org/
 project/pandas/). ### Install To install, open the terminal and type in the
 following. For Windows and Linux: ```{python} pip install highyield ``` For
 macOS: ```{python} python3 -m pip install highyield ``` ### Dependencies The
 table below lists the dependencies for each module within this package: |
-Module | Packages | | --------- | -------------------- | | basics | os | |
-converter | os, pandas, docx2pdf | | copy | os, shutil, pandas | | create | os,
-shutil | | imports | importlib, pandas | | pdf | os, pypdf | | rename | os, re
-| | tts | pyttsx3, pandas |
+Module | Packages | | --------- | -------------------- | | basics | os,
+requests | | converter | os, pandas, docx2pdf | | copy | os, shutil, pandas | |
+create | os, shutil | | imports | importlib, pandas | | pdf | os, pypdf | |
+rename | os, re | | tts | pyttsx3, pandas |
```

### Comparing `highyield-1.0.9/highyield/converter.py` & `highyield-1.1.0/highyield/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import docx2pdf
 
 #csv2xlsx
 def csv2xlsx(target_dir,current_name,header="infer"):
     """Function to convert `.csv` files to `.xlsx`. Slightly modified from `xlsx2csv` function.
 
     Args:
-        target_dir (_type_): Directory target file is located in. Will also be where generated `.xlsx` will be saved.
-        current_name (_type_): Name of `.csv` file.
-        header (str, optional): Include header row? Defaults to "infer" (makes best guess).
+        target_dir (str): Directory target file is located in. Will also be where generated `.xlsx` will be saved.
+        current_name (str): Name of `.csv` file.
+        header (bool, optional): Include header row? Defaults to "infer" (makes best guess).
     """
     
     #change directory
     os.chdir(path=target_dir)
 
     #split current_name into name & extension
     file_name, ext = os.path.splitext(current_name)
@@ -33,19 +33,19 @@
     print(f"{current_name} has been converted to {new_file_name} in {target_dir}")
     
 #xlsx2csv
 def xlsx2csv(target_dir,current_name,sheet_name=0,sep=",",index=None,header=True):
     """Function to convert `.xls*` files to `.csv`. Slightly modified from `csv2xlsx` function.
 
     Args:
-        target_dir (_type_): Directory target file is located in. Will also be where generated `.csv` will be saved.
-        current_name (_type_): Name of `.xls*` file.
-        sheet_name (_type_): Name of sheet. Defaults to 0 (1st sheet).
+        target_dir (str): Directory target file is located in. Will also be where generated `.csv` will be saved.
+        current_name (str): Name of `.xls*` file.
+        sheet_name (int, str): Name of sheet. Defaults to 0 (1st sheet).
         sep (str, optional): Separator to use for `.csv`. Defaults to ",".
-        index (_type_, optional): Write row names? Defaults to None.
+        index (str, optional): Write row names? Defaults to None.
         header (bool, optional): Include header row? Defaults to True.
     """
     
     #change directory
     os.chdir(path=target_dir)
 
     #split current_name into name & extension
@@ -65,16 +65,16 @@
     print(f"{current_name} has been converted to {new_file_name} in {target_dir}")
     
 #word2pdf
 def word2pdf(target_dir,current_name):
     """Function to convert `.doc*` files to `.pdf`. Might need to grant access to certain files/folders (dependent on operating system).
 
     Args:
-        target_dir (_type_): Directory target file is located in. Will also be where generated `.pdf` will be saved.
-        current_name (_type_): Name of `.doc*` file.
+        target_dir (str): Directory target file is located in. Will also be where generated `.pdf` will be saved.
+        current_name (str): Name of `.doc*` file.
     """
 
     #change directory
     os.chdir(path=target_dir)
 
     #split current_name into name & extension
     file_name, ext = os.path.splitext(current_name)
```

### Comparing `highyield-1.0.9/highyield/copy.py` & `highyield-1.1.0/highyield/copy.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pandas as pd
 
 #automate_copy
 def automate_copy(ref_file,source_col="source",dest_col="dest"):
     """Use `.csv` or `.xls*` file to automate process of copying files from source path to destination path. Either file must have header. Copies file data and permissions.
 
     Args:
-        ref_file (_type_): Separate `.csv` or `.xls*` file containing full path of source & destination to pass into `shutil.copy` function.
+        ref_file (str): Separate `.csv` or `.xls*` file containing full path of source & destination to pass into `shutil.copy` function.
         source_col (str, optional): Source column. Defaults to "source".
         dest_col (str, optional): Destination column. Defaults to "dest".
     """
     
     #det ext type
     ext = os.path.splitext(ref_file)[1]
     
@@ -39,15 +39,15 @@
     print("Complete. Files have been copied from specified source to specified destination.")
     
 #automate_copy2
 def automate_copy2(ref_file,source_col="source",dest_col="dest"):
     """Use `.csv` or `.xls*` file to automate process of copying files from source path to destination path. Either file must have header. Copies file data, permissions, and metadata.
 
     Args:
-        ref_file (_type_): Separate `.csv` or `.xls*` file containing full path of source & destination to pass into `shutil.copy` function.
+        ref_file (str): Separate `.csv` or `.xls*` file containing full path of source & destination to pass into `shutil.copy` function.
         source_col (str, optional): Source column. Defaults to "source".
         dest_col (str, optional): Destination column. Defaults to "dest".
     """
     
     #det ext type
     ext = os.path.splitext(ref_file)[1]
     
@@ -74,15 +74,15 @@
     print("Complete. Files have been copied from specified source to specified destination.")
     
 #automate_copyfile
 def automate_copyfile(ref_file,source_col="source",dest_col="dest"):
     """Use `.csv` or `.xls*` file to automate process of copying files from source path to destination path. Either file must have header. Files are copied without permissions and metadata.
 
     Args:
-        ref_file (_type_): Separate `.csv` or `.xls*` file containing full path of source & destination to pass into `shutil.copy` function.
+        ref_file (str): Separate `.csv` or `.xls*` file containing full path of source & destination to pass into `shutil.copy` function.
         source_col (str, optional): Source column. Defaults to "source".
         dest_col (str, optional): Destination column. Defaults to "dest".
     """
     
     #det ext type
     ext = os.path.splitext(ref_file)[1]
```

### Comparing `highyield-1.0.9/highyield/create.py` & `highyield-1.1.0/highyield/create.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from highyield import create
 
 #gen_proj_folder
 def gen_proj_folder(full_path,file_location):
     """To simplify the creation of a new repo. It achieves this task by creating a new folder and pastes `.gitignore` file from the specified location inside. However, this function can also be used for other files. Note: If folder already exists, the function will only add the specified file to said folder.
 
     Args:
-        full_path (_type_): Full path to new folder.
-        file_location (_type_): Full path to where `.gitignore` or file to copy from is located.
+        full_path (str): Full path to new folder.
+        file_location (str): Full path to where `.gitignore` or file to copy from is located.
     """
     
     #checks if path already exist (creates folder if not)
     if os.path.exists(full_path) is True:
         print("Folder already exists.")
     else:
         os.mkdir(path=full_path)
@@ -26,16 +26,16 @@
     print(f"The specified file from {file_location} has been copied to {full_path}.")
     
 #proj_multi_file
 def proj_multi_file(full_path,file_list):
     """Wrapper function around `gen_proj_folder` to generated a new folder and paste multiple files designated in list into the newly created folder.
 
     Args:
-        full_path (_type_): Full path to new folder.
-        file_list (_type_): A list of full paths to where files to copy from are located.
+        full_path (str): Full path to new folder.
+        file_list (str): A list of full paths to where files to copy from are located.
     """
     
     #copy each item in file_list
     for item in file_list:
         create.gen_proj_folder(full_path=full_path,file_location=item)
     
     #print completion message
```

### Comparing `highyield-1.0.9/highyield/data/RR.csv` & `highyield-1.1.0/highyield/data/RR.csv`

 * *Files identical despite different names*

### Comparing `highyield-1.0.9/highyield/pdf.py` & `highyield-1.1.0/highyield/pdf.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from pypdf import PdfReader
 
 #extract text from single page of pdf
 def pdf_extract_single(file_path,page_num):
     """Extract text from single page of pdf.
 
     Args:
-        file_path (_type_): Full path to pdf file.
-        page_num (_type_): Page to extract text from. 0 = page 1.
+        file_path (str): Full path to pdf file.
+        page_num (int): Page to extract text from. 0 = page 1.
     """
     
     #import pdf
     reader = PdfReader(file_path)
     
     #save selected pdf page
     pdfpage = reader.pages[page_num]
@@ -21,15 +21,15 @@
     print(pdfpage.extract_text())
 
 #extract text from all pages of pdf
 def pdf_extract_all(file_path):
     """Extract text from all pages of pdf.
 
     Args:
-        file_path (_type_): Full path to pdf file.
+        file_path (str): Full path to pdf file.
     """
     
     #import pdf
     reader = PdfReader(file_path)
 
     #get total num pages 
     num_pages = len(reader.pages)
@@ -40,17 +40,17 @@
         print(pdfpage.extract_text())
         
 #extract text from selected pages of pdf
 def pdf_extract_range(file_path,lower_bound,upper_bound):
     """Extract text from range of pages in pdf.
 
     Args:
-        file_path (_type_): Full path to pdf file.
-        lower_bound (_type_): Page to start extracting from. 0 = page 1.
-        upper_bound (_type_): Page to stop extracting from. Text from this page and afterwards will not be included.
+        file_path (str): Full path to pdf file.
+        lower_bound (int): Page to start extracting from. 0 = page 1.
+        upper_bound (int): Page to stop extracting from. Text from this page and afterwards will not be included.
     """
     
     #import pdf
     reader = PdfReader(file_path)
 
     #extract text
     for i in range(lower_bound,upper_bound):
```

### Comparing `highyield-1.0.9/highyield/rename.py` & `highyield-1.1.0/highyield/rename.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #import modules
 import os
 import re
 
 def bulk_rename(target_path,ext,new_name,search_term="[A-z0-9]*"):
     """Custom function to bulk rename files matching criteria specified by regular expressions. Will automatically sort and exclude `.DS_Store` (a macOS specific file) (if present).
     Args:
-        target_path (path): Full path to target folder.
-        ext (string): File extension (`.` included).
-        new_name (string): New name for all matched files to share.
-        search_term (regex): Name of files to include (can use regex), default is "[A-z0-9]*" to include all files inside target folder.
+        target_path (str): Full path to target folder.
+        ext (str): File extension (`.` included).
+        new_name (str): New name for all matched files to share.
+        search_term (str, regex): Name of files to include (can use regex), default is "[A-z0-9]*" to include all files inside target folder.
     """
     
     #list all files in target_path + sort in ascending order
     all_files = sorted(os.listdir(target_path))
     
     #rm DS_Store
     if all_files[0] == ".DS_Store":
```

### Comparing `highyield-1.0.9/highyield/tts.py` & `highyield-1.1.0/highyield/tts.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import pandas as pd
 
 #spreadsheet_tts    
 def spreadsheet_tts(file_name,lower_bound=0,upper_bound=None,header=None):
     """Text-to-speech from rows in specified spreadsheet (`.csv` or `.xls*`) file. By default, the function will use all rows from the specified spreadsheet.
 
     Args:
-        file_name (_type_): Full path to spreadsheet file. Will see error if file doesn't match either format.
+        file_name (str): Full path to spreadsheet file. Will see error if file doesn't match either format.
         lower_bound (int, optional): Which row should TTS engine start from? Defaults to 0 (first row).
-        upper_bound (_type_, optional): Which row should TTS engine end? Defaults to None (last row).
-        header (_type_, optional): Does header exist in spreadsheet file? Defaults to None.
+        upper_bound (int, optional): Which row should TTS engine end? Defaults to None (last row).
+        header (str, optional): Does header exist in spreadsheet file? Defaults to None.
     """
     
     #will choose whether to use read_csv or read_excel, throws error if either can't read+import
     try:
         raw_text = pd.read_csv(filepath_or_buffer=file_name,header=header)
     except:
         raw_text = pd.read_excel(io=file_name,header=header)
@@ -36,19 +36,19 @@
     engine.runAndWait()
 
 #spreadsheet_tts_save
 def spreadsheet_tts_save(file_name,save_name,lower_bound=0,upper_bound=None,header=None):
     """Saves text-to-speech output from rows in specified spreadsheet (`.csv` or `.xls*`) file. Similar to `spreadsheet_tts` but saves output instead. By default, the function will use all rows from the specified spreadsheet.
 
     Args:
-        file_name (_type_): Full path to spreadsheet file. Will see error if file doesn't match either format.
-        save_name (_type_): Full path and extension for audio file output from this function.
+        file_name (str): Full path to spreadsheet file. Will see error if file doesn't match either format.
+        save_name (str): Full path and extension for audio file output from this function.
         lower_bound (int, optional): Which row should TTS engine start from? Defaults to 0 (first row).
-        upper_bound (_type_, optional): Which row should TTS engine end? Defaults to None (last row).
-        header (_type_, optional): Does header exist in spreadsheet file? Defaults to None.
+        upper_bound (int, optional): Which row should TTS engine end? Defaults to None (last row).
+        header (str, optional): Does header exist in spreadsheet file? Defaults to None.
     """
     
     #will choose whether to use read_csv or read_excel, throws error if either can't read+import
     try:
         raw_text = pd.read_csv(filepath_or_buffer=file_name,header=header)
     except:
         raw_text = pd.read_excel(io=file_name,header=header)
@@ -72,17 +72,17 @@
     engine.runAndWait()
     
 #df_tts
 def df_tts(df_name,lower_bound=0,upper_bound=None):
     """Text to speech from user imported dataframe. By default, the function will use all rows from the specified spreadsheet.
 
     Args:
-        df_name (_type_): Name of dataframe to pass into this function.
+        df_name (str): Name of dataframe to pass into this function.
         lower_bound (int, optional): Which row should TTS engine start from? Defaults to 0 (first row).
-        upper_bound (_type_, optional): Which row should TTS engine end? Defaults to None (last row).
+        upper_bound (int, optional): Which row should TTS engine end? Defaults to None (last row).
     """
     
     #rm NaN rows
     raw_text = df_name.dropna()
     
     #convert df col to list
     if upper_bound is None:
@@ -98,18 +98,18 @@
     engine.runAndWait()
     
 #df_tts_save
 def df_tts_save(df_name,save_name,lower_bound=0,upper_bound=None):
     """Saves text-to speech from user imported dataframe. By default, the function will use all rows from the specified spreadsheet.
 
     Args:
-        df_name (_type_): Name of dataframe to pass into this function.
-        save_name (_type_): Full path and extension for audio file output from this function.
+        df_name (str): Name of dataframe to pass into this function.
+        save_name (str): Full path and extension for audio file output from this function.
         lower_bound (int, optional): Which row should TTS engine start from? Defaults to 0 (first row).
-        upper_bound (_type_, optional): Which row should TTS engine end? Defaults to None (last row).
+        upper_bound (int, optional): Which row should TTS engine end? Defaults to None (last row).
     """
     
     #rm NaN rows
     raw_text = df_name.dropna()
     
     #convert df col to list
     if upper_bound is None:
```

### Comparing `highyield-1.0.9/highyield.egg-info/PKG-INFO` & `highyield-1.1.0/highyield.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: highyield
-Version: 1.0.9
+Version: 1.1.0
 Summary: Collection of high-yield functions intended to simplify and automate specific tasks.
 Home-page: https://github.com/kenf1/High-Yield
 Author: KF
 Author-email: kenfv1@outlook.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## highyield `<a href="https://kenf1.github.io/Rendered/highyield%20Documentation/"><img src="https://raw.githubusercontent.com/kenf1/Rendered/main/Hex_Sticker/High-Yield.png" align="right" height="138.5" />``</a>`
+## highyield <a href="https://kenf1.github.io/Rendered/highyield%20Documentation/"><img src="https://raw.githubusercontent.com/kenf1/Rendered/main/Hex_Sticker/High-Yield.png" align="right" height="138.5" /></a>
 
 [![PyPI](https://img.shields.io/pypi/v/highyield.svg)](https://pypi.org/project/highyield) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0) [![](https://img.shields.io/badge/-Documentation-yellow)](https://kenf1.github.io/Rendered/highyield%20Documentation/)
 
 `highyield` is a Python package containing a collection of high-yield functions (grouped by modules) intended to simplify and automate specific tasks.
 
 This package requires Python >= 3.8 due to reliance on [`pandas` package](https://pypi.org/project/pandas/).
 
@@ -39,15 +39,15 @@
 
 ### Dependencies
 
 The table below lists the dependencies for each module within this package:
 
 | Module    | Packages             |
 | --------- | -------------------- |
-| basics    | os                   |
+| basics    | os, requests         |
 | converter | os, pandas, docx2pdf |
 | copy      | os, shutil, pandas   |
 | create    | os, shutil           |
 | imports   | importlib, pandas    |
 | pdf       | os, pypdf            |
 | rename    | os, re               |
 | tts       | pyttsx3, pandas      |
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: highyield Version: 1.0.9 Summary: Collection of
+Metadata-Version: 2.1 Name: highyield Version: 1.1.0 Summary: Collection of
 high-yield functions intended to simplify and automate specific tasks. Home-
 page: https://github.com/kenf1/High-Yield Author: KF Author-email:
 kenfv1@outlook.com License: GPLv3 Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE ## highyield `
+Description-Content-Type: text/markdown License-File: LICENSE ## highyield
 [https://raw.githubusercontent.com/kenf1/Rendered/main/Hex_Sticker/High-
-Yield.png]``` [![PyPI](https://img.shields.io/pypi/v/highyield.svg)](https://
+Yield.png] [![PyPI](https://img.shields.io/pypi/v/highyield.svg)](https://
 pypi.org/project/highyield) [![License: GPL v3](https://img.shields.io/badge/
 License-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0) [![]
 (https://img.shields.io/badge/-Documentation-yellow)](https://kenf1.github.io/
 Rendered/highyield%20Documentation/) `highyield` is a Python package containing
 a collection of high-yield functions (grouped by modules) intended to simplify
 and automate specific tasks. This package requires Python >= 3.8 due to
 reliance on [`pandas` package](https://pypi.org/project/pandas/). ### Install
 To install, open the terminal and type in the following. For Windows and Linux:
 ```{python} pip install highyield ``` For macOS: ```{python} python3 -m pip
 install highyield ``` ### Dependencies The table below lists the dependencies
 for each module within this package: | Module | Packages | | --------- | ------
--------------- | | basics | os | | converter | os, pandas, docx2pdf | | copy |
-os, shutil, pandas | | create | os, shutil | | imports | importlib, pandas | |
-pdf | os, pypdf | | rename | os, re | | tts | pyttsx3, pandas |
+-------------- | | basics | os, requests | | converter | os, pandas, docx2pdf |
+| copy | os, shutil, pandas | | create | os, shutil | | imports | importlib,
+pandas | | pdf | os, pypdf | | rename | os, re | | tts | pyttsx3, pandas |
```

### Comparing `highyield-1.0.9/setup.py` & `highyield-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory/"README.md").read_text()
 
 setup(name="highyield",
-      version="1.0.9",
+      version="1.1.0",
       description="Collection of high-yield functions intended to simplify and automate specific tasks.",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/kenf1/High-Yield",
       author="KF",
       author_email="kenfv1@outlook.com",
       license="GPLv3",
@@ -21,10 +21,11 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent"
       ],
       install_requires=[
         "pandas",
         "pyttsx3",
         "docx2pdf",
-        "pypdf"
+        "pypdf",
+        "requests"
       ],
       zip_safe=False)
```

