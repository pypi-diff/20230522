# Comparing `tmp/laff-0.6.0.tar.gz` & `tmp/laff-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laff-0.6.0.tar", max compression
+gzip compressed data, was "laff-0.6.1.tar", max compression
```

## Comparing `laff-0.6.0.tar` & `laff-0.6.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     2642 2023-04-10 13:43:40.172834 laff-0.6.0/README.md
--rw-r--r--   0        0        0       31 2023-05-19 17:34:57.346443 laff-0.6.0/laff/__init__.py
--rw-r--r--   0        0        0     1482 2023-05-19 18:24:22.268766 laff-0.6.0/laff/lcimport.py
--rw-r--r--   0        0        0      410 2023-05-19 18:24:16.448792 laff-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 laff-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2642 2023-04-10 13:43:40.172834 laff-0.6.1/README.md
+-rw-r--r--   0        0        0       31 2023-05-19 17:34:57.346443 laff-0.6.1/laff/__init__.py
+-rw-r--r--   0        0        0      109 2023-05-22 12:37:51.258725 laff-0.6.1/laff/laff.py
+-rw-r--r--   0        0        0     1482 2023-05-19 18:24:22.268766 laff-0.6.1/laff/lcimport.py
+-rw-r--r--   0        0        0      410 2023-05-22 12:38:21.091044 laff-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 laff-0.6.1/PKG-INFO
```

### Comparing `laff-0.6.0/README.md` & `laff-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `laff-0.6.0/laff/lcimport.py` & `laff-0.6.1/laff/lcimport.py`

 * *Files identical despite different names*

### Comparing `laff-0.6.0/PKG-INFO` & `laff-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laff
-Version: 0.6.0
+Version: 0.6.1
 Summary: GRB lightcurve flare and continuum fitter.
 Author: Adam Hennessy
 Author-email: ah724@leicester.ac.uk
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

