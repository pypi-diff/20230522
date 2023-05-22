# Comparing `tmp/dicommeta-0.4.0.tar.gz` & `tmp/dicommeta-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicommeta-0.4.0.tar", max compression
+gzip compressed data, was "dicommeta-0.5.0.tar", max compression
```

## Comparing `dicommeta-0.4.0.tar` & `dicommeta-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.4.0/LICENSE
--rw-r--r--   0        0        0     2074 2023-05-22 12:16:24.934516 dicommeta-0.4.0/README.md
--rw-r--r--   0        0        0      450 2023-05-22 12:44:18.347661 dicommeta-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4947 2023-05-21 00:52:55.487404 dicommeta-0.4.0/src/dicommeta.py
--rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 dicommeta-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1874 2023-05-22 13:47:11.148987 dicommeta-0.5.0/README.md
+-rw-r--r--   0        0        0      510 2023-05-22 15:19:09.972700 dicommeta-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3956 2023-05-22 13:54:56.725449 dicommeta-0.5.0/src/dicommeta.py
+-rw-r--r--   0        0        0     2327 1970-01-01 00:00:00.000000 dicommeta-0.5.0/PKG-INFO
```

### Comparing `dicommeta-0.4.0/LICENSE` & `dicommeta-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dicommeta-0.4.0/README.md` & `dicommeta-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 pip install dicommeta
 ```
 
 ## Usage
 
 ```python
 from pprint import pprint
-from src.dicommeta import (Series, Study, Instance, Mode)
+from src.dicommeta import (Series, Study, Instance)
+from src.enums import Mode
 
 new_dicom_study = Study(
-                        StudyInstanceUID='1.3.6.1.4.1.14519.5.2.1.4334.1501.757929841898426427124434115918',
-                        SpecificCharacterSet='ISO_IR 100',
-                        StudyDate="20190701",
-                        StudyTime='023750',
-                        AccessionNumber='sdfk324234',
-                        ReferringPhysicianName='Dr Strange',
-                        PatientName='John Doe', 
-                        PatientID='A123',
-                        StudyUID='study001',
-                        PatientBirthDate='2000-01-01',
-                        mode=Mode.CT)
+    StudyInstanceUID='1.3.6.1.4.1.14519.5.2.1.4334.1501.757929841898426427124434115918',
+    SpecificCharacterSet='ISO_IR 100',
+    StudyDate="20190701",
+    StudyTime='023750',
+    AccessionNumber='sdfk324234',
+    ReferringPhysicianName='Dr Strange',
+    PatientName='John Doe',
+    PatientID='A123',
+    StudyUID='study001',
+    PatientBirthDate='2000-01-01',
+    mode=Mode.CT)
 
 new_series01 = Series(seriesUID='series001')
 new_series01.add_instance(Instance(SOPinstanceUID='Instance001'))
 new_series01.add_instance(Instance(SOPinstanceUID='Instance002'))
 new_series01.add_instance(Instance(SOPinstanceUID='Instance002'))
 new_dicom_study.add_series(new_series01)
 new_series11 = Series(seriesUID='series001')
```

### Comparing `dicommeta-0.4.0/PKG-INFO` & `dicommeta-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicommeta
-Version: 0.4.0
+Version: 0.5.0
 Summary: Dicom Metadata structures
 Author: Kevin Long
 Author-email: longke@pennmedicine.upenn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -24,28 +24,29 @@
 pip install dicommeta
 ```
 
 ## Usage
 
 ```python
 from pprint import pprint
-from src.dicommeta import (Series, Study, Instance, Mode)
+from src.dicommeta import (Series, Study, Instance)
+from src.enums import Mode
 
 new_dicom_study = Study(
-                        StudyInstanceUID='1.3.6.1.4.1.14519.5.2.1.4334.1501.757929841898426427124434115918',
-                        SpecificCharacterSet='ISO_IR 100',
-                        StudyDate="20190701",
-                        StudyTime='023750',
-                        AccessionNumber='sdfk324234',
-                        ReferringPhysicianName='Dr Strange',
-                        PatientName='John Doe', 
-                        PatientID='A123',
-                        StudyUID='study001',
-                        PatientBirthDate='2000-01-01',
-                        mode=Mode.CT)
+    StudyInstanceUID='1.3.6.1.4.1.14519.5.2.1.4334.1501.757929841898426427124434115918',
+    SpecificCharacterSet='ISO_IR 100',
+    StudyDate="20190701",
+    StudyTime='023750',
+    AccessionNumber='sdfk324234',
+    ReferringPhysicianName='Dr Strange',
+    PatientName='John Doe',
+    PatientID='A123',
+    StudyUID='study001',
+    PatientBirthDate='2000-01-01',
+    mode=Mode.CT)
 
 new_series01 = Series(seriesUID='series001')
 new_series01.add_instance(Instance(SOPinstanceUID='Instance001'))
 new_series01.add_instance(Instance(SOPinstanceUID='Instance002'))
 new_series01.add_instance(Instance(SOPinstanceUID='Instance002'))
 new_dicom_study.add_series(new_series01)
 new_series11 = Series(seriesUID='series001')
```

