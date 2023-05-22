# Comparing `tmp/PyCQuery-1.0.6.tar.gz` & `tmp/PyCQuery-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCQuery-1.0.6.tar", last modified: Thu May 18 06:24:00 2023, max compression
+gzip compressed data, was "PyCQuery-1.0.7.tar", last modified: Mon May 22 01:43:37 2023, max compression
```

## Comparing `PyCQuery-1.0.6.tar` & `PyCQuery-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-18 06:24:00.138237 PyCQuery-1.0.6/
--rw-r--r--   0 user       (501) staff       (20)    11348 2022-08-11 00:11:52.000000 PyCQuery-1.0.6/LICENSE
--rw-r--r--   0 user       (501) staff       (20)       56 2022-08-11 00:11:52.000000 PyCQuery-1.0.6/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     7210 2022-08-11 00:11:52.000000 PyCQuery-1.0.6/NOTICE
--rw-r--r--   0 user       (501) staff       (20)      564 2023-05-18 06:24:00.138380 PyCQuery-1.0.6/PKG-INFO
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-18 06:24:00.137961 PyCQuery-1.0.6/PyCQuery.egg-info/
--rw-r--r--   0 user       (501) staff       (20)      564 2023-05-18 06:24:00.000000 PyCQuery-1.0.6/PyCQuery.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     4346 2023-05-18 06:24:00.000000 PyCQuery-1.0.6/PyCQuery.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-18 06:24:00.000000 PyCQuery-1.0.6/PyCQuery.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2022-10-21 12:36:09.000000 PyCQuery-1.0.6/PyCQuery.egg-info/not-zip-safe
--rw-r--r--   0 user       (501) staff       (20)      150 2023-05-18 06:24:00.000000 PyCQuery-1.0.6/PyCQuery.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)      236 2023-05-18 06:24:00.000000 PyCQuery-1.0.6/PyCQuery.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     5162 2022-08-11 00:11:52.000000 PyCQuery-1.0.6/README.md
--rw-r--r--   0 user       (501) staff       (20)      282 2022-08-11 00:11:52.000000 PyCQuery-1.0.6/requirements.txt
--rw-r--r--   0 user       (501) staff       (20)      151 2023-05-18 06:24:00.138710 PyCQuery-1.0.6/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)     3416 2022-08-11 00:11:52.000000 PyCQuery-1.0.6/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-22 01:43:37.335530 PyCQuery-1.0.7/
+-rw-r--r--   0 user       (501) staff       (20)    11348 2022-08-11 00:11:52.000000 PyCQuery-1.0.7/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)       56 2022-08-11 00:11:52.000000 PyCQuery-1.0.7/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     7210 2022-08-11 00:11:52.000000 PyCQuery-1.0.7/NOTICE
+-rw-r--r--   0 user       (501) staff       (20)      564 2023-05-22 01:43:37.335606 PyCQuery-1.0.7/PKG-INFO
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-22 01:43:37.335379 PyCQuery-1.0.7/PyCQuery.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)      564 2023-05-22 01:43:37.000000 PyCQuery-1.0.7/PyCQuery.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     4346 2023-05-22 01:43:37.000000 PyCQuery-1.0.7/PyCQuery.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-22 01:43:37.000000 PyCQuery-1.0.7/PyCQuery.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2022-10-21 12:36:09.000000 PyCQuery-1.0.7/PyCQuery.egg-info/not-zip-safe
+-rw-r--r--   0 user       (501) staff       (20)      150 2023-05-22 01:43:37.000000 PyCQuery-1.0.7/PyCQuery.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)      236 2023-05-22 01:43:37.000000 PyCQuery-1.0.7/PyCQuery.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     5162 2022-08-11 00:11:52.000000 PyCQuery-1.0.7/README.md
+-rw-r--r--   0 user       (501) staff       (20)      330 2023-05-22 01:37:04.000000 PyCQuery-1.0.7/requirements.txt
+-rw-r--r--   0 user       (501) staff       (20)      151 2023-05-22 01:43:37.335855 PyCQuery-1.0.7/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)     3416 2022-08-11 00:11:52.000000 PyCQuery-1.0.7/setup.py
```

### Comparing `PyCQuery-1.0.6/LICENSE` & `PyCQuery-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCQuery-1.0.6/NOTICE` & `PyCQuery-1.0.7/NOTICE`

 * *Files identical despite different names*

### Comparing `PyCQuery-1.0.6/PKG-INFO` & `PyCQuery-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCQuery
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python interface to Hive with pure-python Kerberos support
 Home-page: https://github.com/naver/PyCQuery
 Author: NAVER Corp.
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `PyCQuery-1.0.6/PyCQuery.egg-info/PKG-INFO` & `PyCQuery-1.0.7/PyCQuery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCQuery
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python interface to Hive with pure-python Kerberos support
 Home-page: https://github.com/naver/PyCQuery
 Author: NAVER Corp.
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `PyCQuery-1.0.6/PyCQuery.egg-info/SOURCES.txt` & `PyCQuery-1.0.7/PyCQuery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyCQuery-1.0.6/README.md` & `PyCQuery-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `PyCQuery-1.0.6/setup.py` & `PyCQuery-1.0.7/setup.py`

 * *Files identical despite different names*

