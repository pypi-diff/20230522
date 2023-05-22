# Comparing `tmp/impick-0.1.0.tar.gz` & `tmp/impick-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impick-0.1.0.tar", last modified: Mon May 22 15:48:01 2023, max compression
+gzip compressed data, was "impick-0.1.1.tar", last modified: Mon May 22 17:47:13 2023, max compression
```

## Comparing `impick-0.1.0.tar` & `impick-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 15:48:01.373058 impick-0.1.0/
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1088 2023-05-22 08:32:04.000000 impick-0.1.0/LICENSE
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      148 2023-05-22 08:28:27.000000 impick-0.1.0/MANIFEST.in
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2927 2023-05-22 15:48:01.373058 impick-0.1.0/PKG-INFO
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2399 2023-05-22 15:47:05.000000 impick-0.1.0/README.md
-drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 15:48:01.373058 impick-0.1.0/impick/
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 08:24:44.000000 impick-0.1.0/impick/__init__.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 15:48:00.000000 impick-0.1.0/impick/__init__.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       22 2023-05-22 15:47:29.000000 impick-0.1.0/impick/__version__.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 15:48:00.000000 impick-0.1.0/impick/__version__.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      225 2023-05-22 08:24:44.000000 impick-0.1.0/impick/py.typed
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     5386 2023-05-22 15:21:34.000000 impick-0.1.0/impick/server.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      639 2023-05-22 15:48:00.000000 impick-0.1.0/impick/server.pyi
-drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 15:48:01.373058 impick-0.1.0/impick.egg-info/
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2927 2023-05-22 15:48:01.000000 impick-0.1.0/impick.egg-info/PKG-INFO
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      401 2023-05-22 15:48:01.000000 impick-0.1.0/impick.egg-info/SOURCES.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        1 2023-05-22 15:48:01.000000 impick-0.1.0/impick.egg-info/dependency_links.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       61 2023-05-22 15:48:01.000000 impick-0.1.0/impick.egg-info/entry_points.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        1 2023-05-22 08:33:58.000000 impick-0.1.0/impick.egg-info/not-zip-safe
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       66 2023-05-22 15:48:01.000000 impick-0.1.0/impick.egg-info/requires.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        7 2023-05-22 15:48:01.000000 impick-0.1.0/impick.egg-info/top_level.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       66 2023-05-22 14:43:47.000000 impick-0.1.0/requirements.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       38 2023-05-22 15:48:01.373058 impick-0.1.0/setup.cfg
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1443 2023-05-22 15:25:51.000000 impick-0.1.0/setup.py
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 17:47:13.360107 impick-0.1.1/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1088 2023-05-22 17:43:14.000000 impick-0.1.1/LICENSE
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      178 2023-05-22 17:46:21.000000 impick-0.1.1/MANIFEST.in
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2927 2023-05-22 17:47:13.360107 impick-0.1.1/PKG-INFO
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2399 2023-05-22 17:43:14.000000 impick-0.1.1/README.md
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 17:47:13.356108 impick-0.1.1/html/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      401 2023-05-22 17:43:14.000000 impick-0.1.1/html/completed.html
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2394 2023-05-22 17:43:14.000000 impick-0.1.1/html/index.html
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 17:47:13.360107 impick-0.1.1/impick/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 17:43:14.000000 impick-0.1.1/impick/__init__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       22 2023-05-22 17:44:55.000000 impick-0.1.1/impick/__version__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      225 2023-05-22 17:43:14.000000 impick-0.1.1/impick/py.typed
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     5386 2023-05-22 17:43:14.000000 impick-0.1.1/impick/server.py
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-22 17:47:13.360107 impick-0.1.1/impick.egg-info/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2927 2023-05-22 17:47:13.000000 impick-0.1.1/impick.egg-info/PKG-INFO
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      376 2023-05-22 17:47:13.000000 impick-0.1.1/impick.egg-info/SOURCES.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        1 2023-05-22 17:47:13.000000 impick-0.1.1/impick.egg-info/dependency_links.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       61 2023-05-22 17:47:13.000000 impick-0.1.1/impick.egg-info/entry_points.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        1 2023-05-22 17:46:24.000000 impick-0.1.1/impick.egg-info/not-zip-safe
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       66 2023-05-22 17:47:13.000000 impick-0.1.1/impick.egg-info/requires.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        7 2023-05-22 17:47:13.000000 impick-0.1.1/impick.egg-info/top_level.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       66 2023-05-22 17:43:14.000000 impick-0.1.1/requirements.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       38 2023-05-22 17:47:13.360107 impick-0.1.1/setup.cfg
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1443 2023-05-22 17:43:14.000000 impick-0.1.1/setup.py
```

### Comparing `impick-0.1.0/LICENSE` & `impick-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `impick-0.1.0/PKG-INFO` & `impick-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impick
-Version: 0.1.0
+Version: 0.1.1
 Summary: ImPick - view and select a single image from a group using the web-GUI
 Home-page: https://github.com/rilshok/impick
 Author: Vladislav A. Proskurov
 Author-email: rilshok@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `impick-0.1.0/README.md` & `impick-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `impick-0.1.0/impick/server.py` & `impick-0.1.1/impick/server.py`

 * *Files identical despite different names*

### Comparing `impick-0.1.0/impick.egg-info/PKG-INFO` & `impick-0.1.1/impick.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impick
-Version: 0.1.0
+Version: 0.1.1
 Summary: ImPick - view and select a single image from a group using the web-GUI
 Home-page: https://github.com/rilshok/impick
 Author: Vladislav A. Proskurov
 Author-email: rilshok@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `impick-0.1.0/setup.py` & `impick-0.1.1/setup.py`

 * *Files identical despite different names*

