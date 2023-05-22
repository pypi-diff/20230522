# Comparing `tmp/gpswe-0.0.1.tar.gz` & `tmp/gpswe-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpswe-0.0.1.tar", last modified: Mon May 22 01:04:50 2023, max compression
+gzip compressed data, was "gpswe-0.0.2.tar", last modified: Mon May 22 01:08:17 2023, max compression
```

## Comparing `gpswe-0.0.1.tar` & `gpswe-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:04:50.513631 gpswe-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1079 2023-05-18 21:02:07.000000 gpswe-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1140 2023-05-22 01:04:50.513631 gpswe-0.0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2589 2023-05-22 00:58:45.000000 gpswe-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:04:50.513631 gpswe-0.0.1/gpswe/
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-21 17:59:42.000000 gpswe-0.0.1/gpswe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2179 2023-05-21 17:59:42.000000 gpswe-0.0.1/gpswe/connections.py
--rw-r--r--   0 root         (0) root         (0)     3300 2023-05-21 17:59:42.000000 gpswe-0.0.1/gpswe/gps_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:04:50.513631 gpswe-0.0.1/gpswe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1140 2023-05-22 01:04:50.000000 gpswe-0.0.1/gpswe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-22 01:04:50.000000 gpswe-0.0.1/gpswe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 01:04:50.000000 gpswe-0.0.1/gpswe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 01:04:50.000000 gpswe-0.0.1/gpswe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-22 01:04:50.000000 gpswe-0.0.1/gpswe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 01:04:50.513631 gpswe-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1643 2023-05-22 01:03:38.000000 gpswe-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:08:17.967426 gpswe-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-05-18 21:02:07.000000 gpswe-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3532 2023-05-22 01:08:17.967426 gpswe-0.0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2581 2023-05-22 01:07:50.000000 gpswe-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:08:17.967426 gpswe-0.0.2/gpswe/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-21 17:59:42.000000 gpswe-0.0.2/gpswe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-05-21 17:59:42.000000 gpswe-0.0.2/gpswe/connections.py
+-rw-r--r--   0 root         (0) root         (0)     3300 2023-05-21 17:59:42.000000 gpswe-0.0.2/gpswe/gps_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 01:08:17.967426 gpswe-0.0.2/gpswe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3532 2023-05-22 01:08:17.000000 gpswe-0.0.2/gpswe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-22 01:08:17.000000 gpswe-0.0.2/gpswe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 01:08:17.000000 gpswe-0.0.2/gpswe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 01:08:17.000000 gpswe-0.0.2/gpswe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-22 01:08:17.000000 gpswe-0.0.2/gpswe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 01:08:17.967426 gpswe-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-05-22 01:07:16.000000 gpswe-0.0.2/setup.py
```

### Comparing `gpswe-0.0.1/LICENSE` & `gpswe-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpswe-0.0.1/README.md` & `gpswe-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # gpswe
 
 **gpswe** - this module is a Python client library for work with GPS Trackers (Wialon IPS, EGTS)
 
 
 ## Installation
 
-Install the current version with [PyPI](https://pypi.org/project/clubhouse-api/):
+Install the current version with [PyPI](https://pypi.org/project/gpswe/):
 
 ```bash
 pip install gpswe
 ```
 
 ## Usage
```

### Comparing `gpswe-0.0.1/gpswe/connections.py` & `gpswe-0.0.2/gpswe/connections.py`

 * *Files identical despite different names*

### Comparing `gpswe-0.0.1/gpswe/gps_server.py` & `gpswe-0.0.2/gpswe/gps_server.py`

 * *Files identical despite different names*

### Comparing `gpswe-0.0.1/setup.py` & `gpswe-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 """
 :authors: Ivan Kudinov
 :license: The MIT License (MIT) see LICENSE file
 :copyright: (c) 2023 Ivan Kudinov
 """
 
-version = "0.0.1"
+version = "0.0.2"
 
-long_description = '''Python library for parse, save and work 
-                    with Wialon and EGTS data'''
+with open('README.md', encoding='utf-8') as f:
+    long_description = f.read()
 
 setup(
     name="gpswe",
     version=version,
 
     author="Ivan Kudinov",
     author_email="marvel.2012@mail.ru",
```

