# Comparing `tmp/cpdb-api-1.0.4.tar.gz` & `tmp/cpdb_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpdb-api-1.0.4.tar", last modified: Mon May 22 14:03:16 2023, max compression
+gzip compressed data, was "cpdb_api-1.0.5.tar", last modified: Mon May 22 14:11:27 2023, max compression
```

## Comparing `cpdb-api-1.0.4.tar` & `cpdb_api-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:03:16.755518 cpdb-api-1.0.4/
--rw-r--r--   0 kevindackow   (501) staff       (20)    11357 2023-02-03 18:07:36.000000 cpdb-api-1.0.4/LICENSE
--rw-r--r--   0 kevindackow   (501) staff       (20)     1711 2023-05-22 14:03:16.755312 cpdb-api-1.0.4/PKG-INFO
--rw-r--r--   0 kevindackow   (501) staff       (20)     1097 2023-05-22 14:01:24.000000 cpdb-api-1.0.4/README.md
--rw-r--r--   0 kevindackow   (501) staff       (20)      758 2023-05-22 13:59:36.000000 cpdb-api-1.0.4/pyproject.toml
--rw-r--r--   0 kevindackow   (501) staff       (20)       38 2023-05-22 14:03:16.755590 cpdb-api-1.0.4/setup.cfg
-drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:03:16.752229 cpdb-api-1.0.4/src/
-drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:03:16.753537 cpdb-api-1.0.4/src/cpdb-api/
--rw-r--r--   0 kevindackow   (501) staff       (20)        0 2023-02-24 17:37:12.000000 cpdb-api-1.0.4/src/cpdb-api/__init__.py
--rw-r--r--   0 kevindackow   (501) staff       (20)     6871 2023-05-02 22:34:56.000000 cpdb-api-1.0.4/src/cpdb-api/request.py
-drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:03:16.754936 cpdb-api-1.0.4/src/cpdb_api.egg-info/
--rw-r--r--   0 kevindackow   (501) staff       (20)     1711 2023-05-22 14:03:16.000000 cpdb-api-1.0.4/src/cpdb_api.egg-info/PKG-INFO
--rw-r--r--   0 kevindackow   (501) staff       (20)      260 2023-05-22 14:03:16.000000 cpdb-api-1.0.4/src/cpdb_api.egg-info/SOURCES.txt
--rw-r--r--   0 kevindackow   (501) staff       (20)        1 2023-05-22 14:03:16.000000 cpdb-api-1.0.4/src/cpdb_api.egg-info/dependency_links.txt
--rw-r--r--   0 kevindackow   (501) staff       (20)       16 2023-05-22 14:03:16.000000 cpdb-api-1.0.4/src/cpdb_api.egg-info/requires.txt
--rw-r--r--   0 kevindackow   (501) staff       (20)        9 2023-05-22 14:03:16.000000 cpdb-api-1.0.4/src/cpdb_api.egg-info/top_level.txt
+drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:11:27.813760 cpdb_api-1.0.5/
+-rw-r--r--   0 kevindackow   (501) staff       (20)    11357 2023-02-03 18:07:36.000000 cpdb_api-1.0.5/LICENSE
+-rw-r--r--   0 kevindackow   (501) staff       (20)     1711 2023-05-22 14:11:27.813468 cpdb_api-1.0.5/PKG-INFO
+-rw-r--r--   0 kevindackow   (501) staff       (20)     1097 2023-05-22 14:10:41.000000 cpdb_api-1.0.5/README.md
+-rw-r--r--   0 kevindackow   (501) staff       (20)      758 2023-05-22 14:11:11.000000 cpdb_api-1.0.5/pyproject.toml
+-rw-r--r--   0 kevindackow   (501) staff       (20)       38 2023-05-22 14:11:27.813838 cpdb_api-1.0.5/setup.cfg
+drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:11:27.809961 cpdb_api-1.0.5/src/
+drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:11:27.811342 cpdb_api-1.0.5/src/cpdb_api/
+-rw-r--r--   0 kevindackow   (501) staff       (20)        0 2023-02-24 17:37:12.000000 cpdb_api-1.0.5/src/cpdb_api/__init__.py
+-rw-r--r--   0 kevindackow   (501) staff       (20)     6871 2023-05-02 22:34:56.000000 cpdb_api-1.0.5/src/cpdb_api/request.py
+drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:11:27.813006 cpdb_api-1.0.5/src/cpdb_api.egg-info/
+-rw-r--r--   0 kevindackow   (501) staff       (20)     1711 2023-05-22 14:11:27.000000 cpdb_api-1.0.5/src/cpdb_api.egg-info/PKG-INFO
+-rw-r--r--   0 kevindackow   (501) staff       (20)      260 2023-05-22 14:11:27.000000 cpdb_api-1.0.5/src/cpdb_api.egg-info/SOURCES.txt
+-rw-r--r--   0 kevindackow   (501) staff       (20)        1 2023-05-22 14:11:27.000000 cpdb_api-1.0.5/src/cpdb_api.egg-info/dependency_links.txt
+-rw-r--r--   0 kevindackow   (501) staff       (20)       16 2023-05-22 14:11:27.000000 cpdb_api-1.0.5/src/cpdb_api.egg-info/requires.txt
+-rw-r--r--   0 kevindackow   (501) staff       (20)        9 2023-05-22 14:11:27.000000 cpdb_api-1.0.5/src/cpdb_api.egg-info/top_level.txt
```

### Comparing `cpdb-api-1.0.4/LICENSE` & `cpdb_api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cpdb-api-1.0.4/PKG-INFO` & `cpdb_api-1.0.5/src/cpdb_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpdb-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: An API to access the NewClimate Institute's Climate Policy Database
 Author-email: NewClimate Institute <info@newclimate.org>
 Project-URL: Homepage, https://climatepolicydatabase.org
 Project-URL: Source Code, https://github.com/KevinDackow/CPDB-API
 Keywords: nci,cpdb,climatepolicydatabase,newclimateinstitute
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,21 +21,21 @@
 
 ```
 pip install cpdb-api
 ```
 
 If you *need* to specify a version, please do this (we strongly recommend against this unless you know what you're doing):
 ```
-pip install cpdb_api==<version e.g. 1.0.5>
+pip install cpdb-api==<version e.g. 1.0.5>
 ```
 
 # Usage
 
 ```
-from cpdb-api import request 
+from cpdb_api import request 
 
 r = request.Request()
 
 # set filters
 r.set_country("IND")
 r.set_decision_date(2010)
 r.set_policy_status("Planned")
```

### Comparing `cpdb-api-1.0.4/README.md` & `cpdb_api-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 ```
 pip install cpdb-api
 ```
 
 If you *need* to specify a version, please do this (we strongly recommend against this unless you know what you're doing):
 ```
-pip install cpdb_api==<version e.g. 1.0.5>
+pip install cpdb-api==<version e.g. 1.0.5>
 ```
 
 # Usage
 
 ```
-from cpdb-api import request 
+from cpdb_api import request 
 
 r = request.Request()
 
 # set filters
 r.set_country("IND")
 r.set_decision_date(2010)
 r.set_policy_status("Planned")
```

### Comparing `cpdb-api-1.0.4/src/cpdb-api/request.py` & `cpdb_api-1.0.5/src/cpdb_api/request.py`

 * *Files identical despite different names*

### Comparing `cpdb-api-1.0.4/src/cpdb_api.egg-info/PKG-INFO` & `cpdb_api-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cpdb-api
-Version: 1.0.4
+Name: cpdb_api
+Version: 1.0.5
 Summary: An API to access the NewClimate Institute's Climate Policy Database
 Author-email: NewClimate Institute <info@newclimate.org>
 Project-URL: Homepage, https://climatepolicydatabase.org
 Project-URL: Source Code, https://github.com/KevinDackow/CPDB-API
 Keywords: nci,cpdb,climatepolicydatabase,newclimateinstitute
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,21 +21,21 @@
 
 ```
 pip install cpdb-api
 ```
 
 If you *need* to specify a version, please do this (we strongly recommend against this unless you know what you're doing):
 ```
-pip install cpdb_api==<version e.g. 1.0.5>
+pip install cpdb-api==<version e.g. 1.0.5>
 ```
 
 # Usage
 
 ```
-from cpdb-api import request 
+from cpdb_api import request 
 
 r = request.Request()
 
 # set filters
 r.set_country("IND")
 r.set_decision_date(2010)
 r.set_policy_status("Planned")
```

