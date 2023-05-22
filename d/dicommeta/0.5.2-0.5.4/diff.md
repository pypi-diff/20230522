# Comparing `tmp/dicommeta-0.5.2.tar.gz` & `tmp/dicommeta-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicommeta-0.5.2.tar", max compression
+gzip compressed data, was "dicommeta-0.5.4.tar", max compression
```

## Comparing `dicommeta-0.5.2.tar` & `dicommeta-0.5.4.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.5.2/LICENSE
--rw-r--r--   0        0        0     1874 2023-05-22 13:47:11.148987 dicommeta-0.5.2/README.md
--rw-r--r--   0        0        0      530 2023-05-22 17:29:47.177098 dicommeta-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4017 2023-05-22 15:48:22.477834 dicommeta-0.5.2/src/dicommeta.py
--rw-r--r--   0        0        0     2368 1970-01-01 00:00:00.000000 dicommeta-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.5.4/LICENSE
+-rw-r--r--   0        0        0     1880 2023-05-22 17:47:09.010671 dicommeta-0.5.4/README.md
+-rw-r--r--   0        0        0      507 2023-05-22 19:29:02.986506 dicommeta-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-05-22 17:47:09.015177 dicommeta-0.5.4/src/dicommeta/Instance.py
+-rw-r--r--   0        0        0      721 2023-05-22 17:47:09.004819 dicommeta-0.5.4/src/dicommeta/Series.py
+-rw-r--r--   0        0        0     2608 2023-05-22 17:59:43.981254 dicommeta-0.5.4/src/dicommeta/Study.py
+-rw-r--r--   0        0        0     2096 2023-05-22 17:47:09.016479 dicommeta-0.5.4/src/dicommeta/Utils.py
+-rw-r--r--   0        0        0      139 2023-05-22 19:17:01.141051 dicommeta-0.5.4/src/dicommeta/__init__.py
+-rw-r--r--   0        0        0     2333 1970-01-01 00:00:00.000000 dicommeta-0.5.4/PKG-INFO
```

### Comparing `dicommeta-0.5.2/LICENSE` & `dicommeta-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.2/README.md` & `dicommeta-0.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```
 
 ## Usage
 
 ```python
 from pprint import pprint
 from src.dicommeta import (Series, Study, Instance)
-from src.enums import Mode
+from dicommeta.Utils import Mode
 
 new_dicom_study = Study(
     StudyInstanceUID='1.3.6.1.4.1.14519.5.2.1.4334.1501.757929841898426427124434115918',
     SpecificCharacterSet='ISO_IR 100',
     StudyDate="20190701",
     StudyTime='023750',
     AccessionNumber='sdfk324234',
```

### Comparing `dicommeta-0.5.2/PKG-INFO` & `dicommeta-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: dicommeta
-Version: 0.5.2
+Version: 0.5.4
 Summary: Dicom Metadata structures
 Author: Kevin Long
 Author-email: longke@pennmedicine.upenn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: enums-py (>=0.6.0,<0.7.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # DicomMeta
 
 dicommeta is a Python library for efficiently storing large amounts of Dicom Metadata
 
@@ -26,15 +25,15 @@
 ```
 
 ## Usage
 
 ```python
 from pprint import pprint
 from src.dicommeta import (Series, Study, Instance)
-from src.enums import Mode
+from dicommeta.Utils import Mode
 
 new_dicom_study = Study(
     StudyInstanceUID='1.3.6.1.4.1.14519.5.2.1.4334.1501.757929841898426427124434115918',
     SpecificCharacterSet='ISO_IR 100',
     StudyDate="20190701",
     StudyTime='023750',
     AccessionNumber='sdfk324234',
```

