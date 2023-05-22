# Comparing `tmp/pitop.system-0.30.0.post1.tar.gz` & `tmp/pitop.system-0.31.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.system-0.30.0.post1.tar", last modified: Fri Dec 16 14:08:51 2022, max compression
+gzip compressed data, was "dist/pitop.system-0.31.0.post2.tar", last modified: Mon May 22 19:13:14 2023, max compression
```

## Comparing `pitop.system-0.30.0.post1.tar` & `pitop.system-0.31.0.post2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:51.000000 pitop.system-0.30.0.post1/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-16 14:07:48.000000 pitop.system-0.30.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2022-12-16 14:08:51.000000 pitop.system-0.30.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      160 2022-12-16 14:07:48.000000 pitop.system-0.30.0.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:51.000000 pitop.system-0.30.0.post1/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:51.000000 pitop.system-0.30.0.post1/pitop/system/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2022-12-16 14:07:48.000000 pitop.system-0.30.0.post1/pitop/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      276 2022-12-16 14:07:48.000000 pitop.system-0.30.0.post1/pitop/system/daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     1632 2022-12-16 14:07:48.000000 pitop.system-0.30.0.post1/pitop/system/device.py
--rw-r--r--   0 runner    (1001) docker     (122)     3988 2022-12-16 14:07:48.000000 pitop.system-0.30.0.post1/pitop/system/peripherals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1491 2022-12-16 14:07:48.000000 pitop.system-0.30.0.post1/pitop/system/pitop.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:51.000000 pitop.system-0.30.0.post1/pitop.system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2022-12-16 14:08:51.000000 pitop.system-0.30.0.post1/pitop.system.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      331 2022-12-16 14:08:51.000000 pitop.system-0.30.0.post1/pitop.system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-16 14:08:51.000000 pitop.system-0.30.0.post1/pitop.system.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-12-16 14:08:51.000000 pitop.system-0.30.0.post1/pitop.system.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-12-16 14:08:51.000000 pitop.system-0.30.0.post1/pitop.system.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-16 14:08:51.000000 pitop.system-0.30.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1997 2022-12-16 14:07:48.000000 pitop.system-0.30.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.system-0.31.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-22 19:12:56.000000 pitop.system-0.31.0.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-05-22 19:13:14.000000 pitop.system-0.31.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-22 19:12:56.000000 pitop.system-0.31.0.post2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.system-0.31.0.post2/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.system-0.31.0.post2/pitop/system/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-22 19:12:56.000000 pitop.system-0.31.0.post2/pitop/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-22 19:12:56.000000 pitop.system-0.31.0.post2/pitop/system/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1632 2023-05-22 19:12:56.000000 pitop.system-0.31.0.post2/pitop/system/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-05-22 19:12:56.000000 pitop.system-0.31.0.post2/pitop/system/peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-05-22 19:12:56.000000 pitop.system-0.31.0.post2/pitop/system/pitop.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.system-0.31.0.post2/pitop.system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-05-22 19:13:14.000000 pitop.system-0.31.0.post2/pitop.system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      331 2023-05-22 19:13:14.000000 pitop.system-0.31.0.post2/pitop.system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 19:13:14.000000 pitop.system-0.31.0.post2/pitop.system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-22 19:13:14.000000 pitop.system-0.31.0.post2/pitop.system.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 19:13:14.000000 pitop.system-0.31.0.post2/pitop.system.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:13:14.000000 pitop.system-0.31.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1997 2023-05-22 19:12:56.000000 pitop.system-0.31.0.post2/setup.py
```

### Comparing `pitop.system-0.30.0.post1/PKG-INFO` & `pitop.system-0.31.0.post2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.system
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python System
```

### Comparing `pitop.system-0.30.0.post1/pitop/system/device.py` & `pitop.system-0.31.0.post2/pitop/system/device.py`

 * *Files identical despite different names*

### Comparing `pitop.system-0.30.0.post1/pitop/system/peripherals.py` & `pitop.system-0.31.0.post2/pitop/system/peripherals.py`

 * *Files identical despite different names*

### Comparing `pitop.system-0.30.0.post1/pitop/system/pitop.py` & `pitop.system-0.31.0.post2/pitop/system/pitop.py`

 * *Files identical despite different names*

### Comparing `pitop.system-0.30.0.post1/pitop.system.egg-info/PKG-INFO` & `pitop.system-0.31.0.post2/pitop.system.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.system
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python System
```

### Comparing `pitop.system-0.30.0.post1/setup.py` & `pitop.system-0.31.0.post2/setup.py`

 * *Files identical despite different names*

