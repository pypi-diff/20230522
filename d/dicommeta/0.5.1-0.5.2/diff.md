# Comparing `tmp/dicommeta-0.5.1.tar.gz` & `tmp/dicommeta-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicommeta-0.5.1.tar", max compression
+gzip compressed data, was "dicommeta-0.5.2.tar", max compression
```

## Comparing `dicommeta-0.5.1.tar` & `dicommeta-0.5.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.5.1/LICENSE
--rw-r--r--   0        0        0     1874 2023-05-22 13:47:11.148987 dicommeta-0.5.1/README.md
--rw-r--r--   0        0        0      510 2023-05-22 15:48:47.006095 dicommeta-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4017 2023-05-22 15:48:22.477834 dicommeta-0.5.1/src/dicommeta.py
--rw-r--r--   0        0        0     2327 1970-01-01 00:00:00.000000 dicommeta-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1874 2023-05-22 13:47:11.148987 dicommeta-0.5.2/README.md
+-rw-r--r--   0        0        0      530 2023-05-22 17:29:47.177098 dicommeta-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4017 2023-05-22 15:48:22.477834 dicommeta-0.5.2/src/dicommeta.py
+-rw-r--r--   0        0        0     2368 1970-01-01 00:00:00.000000 dicommeta-0.5.2/PKG-INFO
```

### Comparing `dicommeta-0.5.1/LICENSE` & `dicommeta-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.1/README.md` & `dicommeta-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.1/src/dicommeta.py` & `dicommeta-0.5.2/src/dicommeta.py`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.1/PKG-INFO` & `dicommeta-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: dicommeta
-Version: 0.5.1
+Version: 0.5.2
 Summary: Dicom Metadata structures
 Author: Kevin Long
 Author-email: longke@pennmedicine.upenn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
+Requires-Dist: enums-py (>=0.6.0,<0.7.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # DicomMeta
 
 dicommeta is a Python library for efficiently storing large amounts of Dicom Metadata
```

