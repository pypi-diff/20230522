# Comparing `tmp/pitop.display-0.30.0.post1.tar.gz` & `tmp/pitop.display-0.31.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.display-0.30.0.post1.tar", last modified: Fri Dec 16 14:08:22 2022, max compression
+gzip compressed data, was "dist/pitop.display-0.31.0.post2.tar", last modified: Mon May 22 19:13:11 2023, max compression
```

## Comparing `pitop.display-0.30.0.post1.tar` & `pitop.display-0.31.0.post2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:22.000000 pitop.display-0.30.0.post1/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2022-12-16 14:07:48.000000 pitop.display-0.30.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      971 2022-12-16 14:08:22.000000 pitop.display-0.30.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      136 2022-12-16 14:07:48.000000 pitop.display-0.30.0.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:22.000000 pitop.display-0.30.0.post1/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:22.000000 pitop.display-0.30.0.post1/pitop/display/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2022-12-16 14:07:48.000000 pitop.display-0.30.0.post1/pitop/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5417 2022-12-16 14:07:48.000000 pitop.display-0.30.0.post1/pitop/display/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:22.000000 pitop.display-0.30.0.post1/pitop.display.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      971 2022-12-16 14:08:22.000000 pitop.display-0.30.0.post1/pitop.display.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-12-16 14:08:22.000000 pitop.display-0.30.0.post1/pitop.display.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-16 14:08:22.000000 pitop.display-0.30.0.post1/pitop.display.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2022-12-16 14:08:22.000000 pitop.display-0.30.0.post1/pitop.display.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-12-16 14:08:22.000000 pitop.display-0.30.0.post1/pitop.display.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-16 14:08:22.000000 pitop.display-0.30.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1935 2022-12-16 14:07:48.000000 pitop.display-0.30.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.display-0.31.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-22 19:12:55.000000 pitop.display-0.31.0.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-05-22 19:13:11.000000 pitop.display-0.31.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-05-22 19:12:55.000000 pitop.display-0.31.0.post2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.display-0.31.0.post2/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.display-0.31.0.post2/pitop/display/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-22 19:12:55.000000 pitop.display-0.31.0.post2/pitop/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5417 2023-05-22 19:12:55.000000 pitop.display-0.31.0.post2/pitop/display/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.display-0.31.0.post2/pitop.display.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-05-22 19:13:11.000000 pitop.display-0.31.0.post2/pitop.display.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-05-22 19:13:11.000000 pitop.display-0.31.0.post2/pitop.display.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 19:13:11.000000 pitop.display-0.31.0.post2/pitop.display.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-22 19:13:11.000000 pitop.display-0.31.0.post2/pitop.display.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 19:13:11.000000 pitop.display-0.31.0.post2/pitop.display.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:13:11.000000 pitop.display-0.31.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1935 2023-05-22 19:12:55.000000 pitop.display-0.31.0.post2/setup.py
```

### Comparing `pitop.display-0.30.0.post1/PKG-INFO` & `pitop.display-0.31.0.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.display
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Display
```

### Comparing `pitop.display-0.30.0.post1/pitop/display/display.py` & `pitop.display-0.31.0.post2/pitop/display/display.py`

 * *Files identical despite different names*

### Comparing `pitop.display-0.30.0.post1/pitop.display.egg-info/PKG-INFO` & `pitop.display-0.31.0.post2/pitop.display.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.display
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Display
```

### Comparing `pitop.display-0.30.0.post1/setup.py` & `pitop.display-0.31.0.post2/setup.py`

 * *Files identical despite different names*

