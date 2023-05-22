# Comparing `tmp/things.py-0.0.9.tar.gz` & `tmp/things.py-0.0.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "things.py-0.0.9.tar", last modified: Tue Apr 13 16:13:45 2021, max compression
+gzip compressed data, was "things.py-0.0.9.dev0.tar", last modified: Tue Apr 13 16:15:27 2021, max compression
```

## Comparing `things.py-0.0.9.tar` & `things.py-0.0.9.dev0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mike       (501) admin       (80)        0 2021-04-13 16:13:45.905040 things.py-0.0.9/
--rw-r--r--   0 mike       (501) admin       (80)     5887 2021-04-13 16:13:45.905399 things.py-0.0.9/PKG-INFO
--rw-rw-r--   0 mike       (501) admin       (80)     4335 2021-04-01 12:07:55.000000 things.py-0.0.9/README.md
--rw-r--r--   0 mike       (501) admin       (80)      254 2021-04-13 16:13:45.906607 things.py-0.0.9/setup.cfg
--rw-r--r--   0 mike       (501) admin       (80)     1451 2021-04-13 08:47:14.000000 things.py-0.0.9/setup.py
-drwxr-xr-x   0 mike       (501) admin       (80)        0 2021-04-13 16:13:45.895288 things.py-0.0.9/tests/
--rw-rw-r--   0 mike       (501) admin       (80)        0 2021-03-25 11:58:55.000000 things.py-0.0.9/tests/__init__.py
--rw-r--r--   0 mike       (501) admin       (80)     5586 2021-04-13 14:22:39.000000 things.py-0.0.9/tests/test_things.py
-drwxr-xr-x   0 mike       (501) admin       (80)        0 2021-04-13 16:13:45.899035 things.py-0.0.9/things/
--rw-r--r--   0 mike       (501) admin       (80)      747 2021-04-13 16:10:29.000000 things.py-0.0.9/things/__init__.py
--rw-r--r--   0 mike       (501) admin       (80)    18509 2021-04-13 16:01:56.000000 things.py-0.0.9/things/api.py
--rwxr-xr-x   0 mike       (501) admin       (80)    29029 2021-04-13 14:17:50.000000 things.py-0.0.9/things/database.py
-drwxr-xr-x   0 mike       (501) admin       (80)        0 2021-04-13 16:13:45.904290 things.py-0.0.9/things.py.egg-info/
--rw-r--r--   0 mike       (501) admin       (80)     5887 2021-04-13 16:13:45.000000 things.py-0.0.9/things.py.egg-info/PKG-INFO
--rw-r--r--   0 mike       (501) admin       (80)      251 2021-04-13 16:13:45.000000 things.py-0.0.9/things.py.egg-info/SOURCES.txt
--rw-r--r--   0 mike       (501) admin       (80)        1 2021-04-13 16:13:45.000000 things.py-0.0.9/things.py.egg-info/dependency_links.txt
--rw-r--r--   0 mike       (501) admin       (80)       13 2021-04-13 16:13:45.000000 things.py-0.0.9/things.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 16:15:27.041203 things.py-0.0.9.dev0/
+-rw-r--r--   0 runner    (1001) docker     (121)     5892 2021-04-13 16:15:27.041203 things.py-0.0.9.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4335 2021-04-13 16:15:14.000000 things.py-0.0.9.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2021-04-13 16:15:27.041203 things.py-0.0.9.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1451 2021-04-13 16:15:14.000000 things.py-0.0.9.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 16:15:27.041203 things.py-0.0.9.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-13 16:15:14.000000 things.py-0.0.9.dev0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5586 2021-04-13 16:15:14.000000 things.py-0.0.9.dev0/tests/test_things.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 16:15:27.041203 things.py-0.0.9.dev0/things/
+-rw-r--r--   0 runner    (1001) docker     (121)      751 2021-04-13 16:15:14.000000 things.py-0.0.9.dev0/things/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18509 2021-04-13 16:15:14.000000 things.py-0.0.9.dev0/things/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    29029 2021-04-13 16:15:14.000000 things.py-0.0.9.dev0/things/database.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 16:15:27.041203 things.py-0.0.9.dev0/things.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5892 2021-04-13 16:15:26.000000 things.py-0.0.9.dev0/things.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2021-04-13 16:15:26.000000 things.py-0.0.9.dev0/things.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-13 16:15:26.000000 things.py-0.0.9.dev0/things.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-04-13 16:15:26.000000 things.py-0.0.9.dev0/things.py.egg-info/top_level.txt
```

### Comparing `things.py-0.0.9/PKG-INFO` & `things.py-0.0.9.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: things.py
-Version: 0.0.9
+Version: 0.0.9.dev0
 Summary: A simple Python 3 library to read your Things app data.
 Home-page: https://github.com/thingsapi/things.py
 Author: Alexander Willner, Michael B.
 Author-email: alex@willner.ws
 License: UNKNOWN
 Description: # Things Python API
```

### Comparing `things.py-0.0.9/README.md` & `things.py-0.0.9.dev0/README.md`

 * *Files identical despite different names*

### Comparing `things.py-0.0.9/setup.py` & `things.py-0.0.9.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `things.py-0.0.9/tests/test_things.py` & `things.py-0.0.9.dev0/tests/test_things.py`

 * *Files identical despite different names*

### Comparing `things.py-0.0.9/things/__init__.py` & `things.py-0.0.9.dev0/things/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """A simple Python 3 library to read your Things app data."""
 
 __author__ = ["Alexander Willner", "Michael Belfrage"]
 __copyright__ = "2021 Alexander Willner & Michael Belfrage"
 __credits__ = ["Alexander Willner", "Michael Belfrage"]
 __license__ = "Apache License 2.0"
-__version__ = "0.0.9"
+__version__ = "0.0.9.dev"
 __maintainer__ = ["Alexander Willner", "Michael Belfrage"]
 __email__ = "alex@willner.ws"
 __status__ = "Development"
 
 from things.api import (  # noqa
     anytime,
     areas,
```

### Comparing `things.py-0.0.9/things/api.py` & `things.py-0.0.9.dev0/things/api.py`

 * *Files identical despite different names*

### Comparing `things.py-0.0.9/things/database.py` & `things.py-0.0.9.dev0/things/database.py`

 * *Files identical despite different names*

### Comparing `things.py-0.0.9/things.py.egg-info/PKG-INFO` & `things.py-0.0.9.dev0/things.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: things.py
-Version: 0.0.9
+Version: 0.0.9.dev0
 Summary: A simple Python 3 library to read your Things app data.
 Home-page: https://github.com/thingsapi/things.py
 Author: Alexander Willner, Michael B.
 Author-email: alex@willner.ws
 License: UNKNOWN
 Description: # Things Python API
```

