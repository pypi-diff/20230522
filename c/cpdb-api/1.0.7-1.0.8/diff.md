# Comparing `tmp/cpdb_api-1.0.7.tar.gz` & `tmp/cpdb_api-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpdb_api-1.0.7.tar", last modified: Mon May 22 14:33:55 2023, max compression
+gzip compressed data, was "cpdb_api-1.0.8.tar", last modified: Mon May 22 14:37:42 2023, max compression
```

## Comparing `cpdb_api-1.0.7.tar` & `cpdb_api-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:33:55.922770 cpdb_api-1.0.7/
--rw-r--r--   0 kevindackow   (501) staff       (20)    11357 2023-02-03 18:07:36.000000 cpdb_api-1.0.7/LICENSE
--rw-r--r--   0 kevindackow   (501) staff       (20)     1705 2023-05-22 14:33:55.922553 cpdb_api-1.0.7/PKG-INFO
--rw-r--r--   0 kevindackow   (501) staff       (20)     1091 2023-05-22 14:22:29.000000 cpdb_api-1.0.7/README.md
--rw-r--r--   0 kevindackow   (501) staff       (20)      758 2023-05-22 14:33:44.000000 cpdb_api-1.0.7/pyproject.toml
--rw-r--r--   0 kevindackow   (501) staff       (20)       38 2023-05-22 14:33:55.922840 cpdb_api-1.0.7/setup.cfg
-drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:33:55.918711 cpdb_api-1.0.7/src/
-drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:33:55.920837 cpdb_api-1.0.7/src/cpdb_api/
--rw-r--r--   0 kevindackow   (501) staff       (20)        0 2023-02-24 17:37:12.000000 cpdb_api-1.0.7/src/cpdb_api/__init__.py
--rw-r--r--   0 kevindackow   (501) staff       (20)     6616 2023-05-22 14:33:30.000000 cpdb_api-1.0.7/src/cpdb_api/request.py
-drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:33:55.922277 cpdb_api-1.0.7/src/cpdb_api.egg-info/
--rw-r--r--   0 kevindackow   (501) staff       (20)     1705 2023-05-22 14:33:55.000000 cpdb_api-1.0.7/src/cpdb_api.egg-info/PKG-INFO
--rw-r--r--   0 kevindackow   (501) staff       (20)      260 2023-05-22 14:33:55.000000 cpdb_api-1.0.7/src/cpdb_api.egg-info/SOURCES.txt
--rw-r--r--   0 kevindackow   (501) staff       (20)        1 2023-05-22 14:33:55.000000 cpdb_api-1.0.7/src/cpdb_api.egg-info/dependency_links.txt
--rw-r--r--   0 kevindackow   (501) staff       (20)       16 2023-05-22 14:33:55.000000 cpdb_api-1.0.7/src/cpdb_api.egg-info/requires.txt
--rw-r--r--   0 kevindackow   (501) staff       (20)        9 2023-05-22 14:33:55.000000 cpdb_api-1.0.7/src/cpdb_api.egg-info/top_level.txt
+drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:37:42.835364 cpdb_api-1.0.8/
+-rw-r--r--   0 kevindackow   (501) staff       (20)    11357 2023-02-03 18:07:36.000000 cpdb_api-1.0.8/LICENSE
+-rw-r--r--   0 kevindackow   (501) staff       (20)     1705 2023-05-22 14:37:42.834970 cpdb_api-1.0.8/PKG-INFO
+-rw-r--r--   0 kevindackow   (501) staff       (20)     1091 2023-05-22 14:22:29.000000 cpdb_api-1.0.8/README.md
+-rw-r--r--   0 kevindackow   (501) staff       (20)      758 2023-05-22 14:37:15.000000 cpdb_api-1.0.8/pyproject.toml
+-rw-r--r--   0 kevindackow   (501) staff       (20)       38 2023-05-22 14:37:42.835450 cpdb_api-1.0.8/setup.cfg
+drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:37:42.831597 cpdb_api-1.0.8/src/
+drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:37:42.833102 cpdb_api-1.0.8/src/cpdb_api/
+-rw-r--r--   0 kevindackow   (501) staff       (20)        0 2023-02-24 17:37:12.000000 cpdb_api-1.0.8/src/cpdb_api/__init__.py
+-rw-r--r--   0 kevindackow   (501) staff       (20)     6619 2023-05-22 14:36:58.000000 cpdb_api-1.0.8/src/cpdb_api/request.py
+drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:37:42.834486 cpdb_api-1.0.8/src/cpdb_api.egg-info/
+-rw-r--r--   0 kevindackow   (501) staff       (20)     1705 2023-05-22 14:37:42.000000 cpdb_api-1.0.8/src/cpdb_api.egg-info/PKG-INFO
+-rw-r--r--   0 kevindackow   (501) staff       (20)      260 2023-05-22 14:37:42.000000 cpdb_api-1.0.8/src/cpdb_api.egg-info/SOURCES.txt
+-rw-r--r--   0 kevindackow   (501) staff       (20)        1 2023-05-22 14:37:42.000000 cpdb_api-1.0.8/src/cpdb_api.egg-info/dependency_links.txt
+-rw-r--r--   0 kevindackow   (501) staff       (20)       16 2023-05-22 14:37:42.000000 cpdb_api-1.0.8/src/cpdb_api.egg-info/requires.txt
+-rw-r--r--   0 kevindackow   (501) staff       (20)        9 2023-05-22 14:37:42.000000 cpdb_api-1.0.8/src/cpdb_api.egg-info/top_level.txt
```

### Comparing `cpdb_api-1.0.7/LICENSE` & `cpdb_api-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cpdb_api-1.0.7/PKG-INFO` & `cpdb_api-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpdb_api
-Version: 1.0.7
+Version: 1.0.8
 Summary: An API to access the NewClimate Institute's Climate Policy Database
 Author-email: NewClimate Institute <info@newclimate.org>
 Project-URL: Homepage, https://climatepolicydatabase.org
 Project-URL: Source Code, https://github.com/KevinDackow/CPDB-API
 Keywords: nci,cpdb,climatepolicydatabase,newclimateinstitute
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cpdb_api-1.0.7/README.md` & `cpdb_api-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cpdb_api-1.0.7/pyproject.toml` & `cpdb_api-1.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpdb_api"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="NewClimate Institute", email="info@newclimate.org" },
 ]
 description = "An API to access the NewClimate Institute's Climate Policy Database"
 dependencies = [
   "pandas",
   "requests"
```

### Comparing `cpdb_api-1.0.7/src/cpdb_api/request.py` & `cpdb_api-1.0.8/src/cpdb_api/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         Adds sectors to query (Case insensitive). Each provided sector must be one of the sectors from the section of
         the same name on https://climatepolicydatabase.org/policies.
         Some examples: agriculture and forestry or CCS.
 
         :param sector: a list of sectors to add to the query.
         :return: none
         """
-        if self._sector = "":
+        if self._sector == "":
           self._sector = sector
         else:
           self._sector = ",".join([self._sector, sector])
 
     def add_policy_instrument(self, policy_instrument):
         """
         Adds policy instruments to the list of policy instruments to query for. Case insensitive. Each provided policy
@@ -78,29 +78,29 @@
         Some examples: grid access and priority for renewables or
         strategic planning. Note that for policy instruments that are grouped on the website,
         e.g. performance label, the server will treat it as a query for all contained groups.
 
         :param policy_instrument: a list of policy instruments to add to the query.
         :return: none
         """
-        if self._policy_instrument = "":
+        if self._policy_instrument == "":
           self._policy_instrument = policy_instrument
         else:
           self._policy_instrument = ",".join([self._policy_instrument, policy_instrument])
 
     def add_mitigation_area(self, mitigation_area):
         """
         A list of mitigation areas to query. Items must be one of:
         energy efficiency, energy service demand reduction and resource efficiency, 
         non energy use, other low carbon technologies and fuel switch, renewables, unknown
 
         :param mitigation_area: a list of policy types to add to the query.
         :return: none
         """
-        if self._mitigation_area = "":
+        if self._mitigation_area == "":
           self._mitigation_area = mitigation_area
         else:
           self._mitigation_area = ",".join([self._mitigation_area, mitigation_area])
 
     # For request issuing & data retrieval.
     def issue(self):
         """
```

### Comparing `cpdb_api-1.0.7/src/cpdb_api.egg-info/PKG-INFO` & `cpdb_api-1.0.8/src/cpdb_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpdb-api
-Version: 1.0.7
+Version: 1.0.8
 Summary: An API to access the NewClimate Institute's Climate Policy Database
 Author-email: NewClimate Institute <info@newclimate.org>
 Project-URL: Homepage, https://climatepolicydatabase.org
 Project-URL: Source Code, https://github.com/KevinDackow/CPDB-API
 Keywords: nci,cpdb,climatepolicydatabase,newclimateinstitute
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

