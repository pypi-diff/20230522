# Comparing `tmp/cpdb_api-1.0.5.tar.gz` & `tmp/cpdb_api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpdb_api-1.0.5.tar", last modified: Mon May 22 14:11:27 2023, max compression
+gzip compressed data, was "cpdb_api-1.0.6.tar", last modified: Mon May 22 14:23:03 2023, max compression
```

## Comparing `cpdb_api-1.0.5.tar` & `cpdb_api-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:11:27.813760 cpdb_api-1.0.5/
--rw-r--r--   0 kevindackow   (501) staff       (20)    11357 2023-02-03 18:07:36.000000 cpdb_api-1.0.5/LICENSE
--rw-r--r--   0 kevindackow   (501) staff       (20)     1711 2023-05-22 14:11:27.813468 cpdb_api-1.0.5/PKG-INFO
--rw-r--r--   0 kevindackow   (501) staff       (20)     1097 2023-05-22 14:10:41.000000 cpdb_api-1.0.5/README.md
--rw-r--r--   0 kevindackow   (501) staff       (20)      758 2023-05-22 14:11:11.000000 cpdb_api-1.0.5/pyproject.toml
--rw-r--r--   0 kevindackow   (501) staff       (20)       38 2023-05-22 14:11:27.813838 cpdb_api-1.0.5/setup.cfg
-drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:11:27.809961 cpdb_api-1.0.5/src/
-drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:11:27.811342 cpdb_api-1.0.5/src/cpdb_api/
--rw-r--r--   0 kevindackow   (501) staff       (20)        0 2023-02-24 17:37:12.000000 cpdb_api-1.0.5/src/cpdb_api/__init__.py
--rw-r--r--   0 kevindackow   (501) staff       (20)     6871 2023-05-02 22:34:56.000000 cpdb_api-1.0.5/src/cpdb_api/request.py
-drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:11:27.813006 cpdb_api-1.0.5/src/cpdb_api.egg-info/
--rw-r--r--   0 kevindackow   (501) staff       (20)     1711 2023-05-22 14:11:27.000000 cpdb_api-1.0.5/src/cpdb_api.egg-info/PKG-INFO
--rw-r--r--   0 kevindackow   (501) staff       (20)      260 2023-05-22 14:11:27.000000 cpdb_api-1.0.5/src/cpdb_api.egg-info/SOURCES.txt
--rw-r--r--   0 kevindackow   (501) staff       (20)        1 2023-05-22 14:11:27.000000 cpdb_api-1.0.5/src/cpdb_api.egg-info/dependency_links.txt
--rw-r--r--   0 kevindackow   (501) staff       (20)       16 2023-05-22 14:11:27.000000 cpdb_api-1.0.5/src/cpdb_api.egg-info/requires.txt
--rw-r--r--   0 kevindackow   (501) staff       (20)        9 2023-05-22 14:11:27.000000 cpdb_api-1.0.5/src/cpdb_api.egg-info/top_level.txt
+drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:23:03.110710 cpdb_api-1.0.6/
+-rw-r--r--   0 kevindackow   (501) staff       (20)    11357 2023-02-03 18:07:36.000000 cpdb_api-1.0.6/LICENSE
+-rw-r--r--   0 kevindackow   (501) staff       (20)     1705 2023-05-22 14:23:03.110401 cpdb_api-1.0.6/PKG-INFO
+-rw-r--r--   0 kevindackow   (501) staff       (20)     1091 2023-05-22 14:22:29.000000 cpdb_api-1.0.6/README.md
+-rw-r--r--   0 kevindackow   (501) staff       (20)      758 2023-05-22 14:22:37.000000 cpdb_api-1.0.6/pyproject.toml
+-rw-r--r--   0 kevindackow   (501) staff       (20)       38 2023-05-22 14:23:03.110780 cpdb_api-1.0.6/setup.cfg
+drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:23:03.107541 cpdb_api-1.0.6/src/
+drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:23:03.108835 cpdb_api-1.0.6/src/cpdb_api/
+-rw-r--r--   0 kevindackow   (501) staff       (20)        0 2023-02-24 17:37:12.000000 cpdb_api-1.0.6/src/cpdb_api/__init__.py
+-rw-r--r--   0 kevindackow   (501) staff       (20)     6234 2023-05-22 14:22:11.000000 cpdb_api-1.0.6/src/cpdb_api/request.py
+drwxr-xr-x   0 kevindackow   (501) staff       (20)        0 2023-05-22 14:23:03.110094 cpdb_api-1.0.6/src/cpdb_api.egg-info/
+-rw-r--r--   0 kevindackow   (501) staff       (20)     1705 2023-05-22 14:23:03.000000 cpdb_api-1.0.6/src/cpdb_api.egg-info/PKG-INFO
+-rw-r--r--   0 kevindackow   (501) staff       (20)      260 2023-05-22 14:23:03.000000 cpdb_api-1.0.6/src/cpdb_api.egg-info/SOURCES.txt
+-rw-r--r--   0 kevindackow   (501) staff       (20)        1 2023-05-22 14:23:03.000000 cpdb_api-1.0.6/src/cpdb_api.egg-info/dependency_links.txt
+-rw-r--r--   0 kevindackow   (501) staff       (20)       16 2023-05-22 14:23:03.000000 cpdb_api-1.0.6/src/cpdb_api.egg-info/requires.txt
+-rw-r--r--   0 kevindackow   (501) staff       (20)        9 2023-05-22 14:23:03.000000 cpdb_api-1.0.6/src/cpdb_api.egg-info/top_level.txt
```

### Comparing `cpdb_api-1.0.5/LICENSE` & `cpdb_api-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cpdb_api-1.0.5/PKG-INFO` & `cpdb_api-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpdb_api
-Version: 1.0.5
+Version: 1.0.6
 Summary: An API to access the NewClimate Institute's Climate Policy Database
 Author-email: NewClimate Institute <info@newclimate.org>
 Project-URL: Homepage, https://climatepolicydatabase.org
 Project-URL: Source Code, https://github.com/KevinDackow/CPDB-API
 Keywords: nci,cpdb,climatepolicydatabase,newclimateinstitute
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -34,19 +34,19 @@
 from cpdb_api import request 
 
 r = request.Request()
 
 # set filters
 r.set_country("IND")
 r.set_decision_date(2010)
-r.set_policy_status("Planned")
+r.set_policy_status("In force")
 r.add_sector("Electricity and heat")
-r.add_sector("General")
-r.add_policy_instrument("Direct investment")
-r.add_policy_instrument("Energy efficiency")
+r.add_sector("Coal")
+r.add_policy_instrument("Energy and other taxes")
+r.add_mitigation_area("Renewables")
 
 # Issue the request (this returns a pandas dataframe, if you want to parse it programmatically)
 r.issue()
 
 # save the result to CSV file
 r.save_csv("filtered_cpdb.csv")
 ```
```

### Comparing `cpdb_api-1.0.5/README.md` & `cpdb_api-1.0.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 from cpdb_api import request 
 
 r = request.Request()
 
 # set filters
 r.set_country("IND")
 r.set_decision_date(2010)
-r.set_policy_status("Planned")
+r.set_policy_status("In force")
 r.add_sector("Electricity and heat")
-r.add_sector("General")
-r.add_policy_instrument("Direct investment")
-r.add_policy_instrument("Energy efficiency")
+r.add_sector("Coal")
+r.add_policy_instrument("Energy and other taxes")
+r.add_mitigation_area("Renewables")
 
 # Issue the request (this returns a pandas dataframe, if you want to parse it programmatically)
 r.issue()
 
 # save the result to CSV file
 r.save_csv("filtered_cpdb.csv")
 ```
```

### Comparing `cpdb_api-1.0.5/pyproject.toml` & `cpdb_api-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpdb_api"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="NewClimate Institute", email="info@newclimate.org" },
 ]
 description = "An API to access the NewClimate Institute's Climate Policy Database"
 dependencies = [
   "pandas",
   "requests"
```

### Comparing `cpdb_api-1.0.5/src/cpdb_api/request.py` & `cpdb_api-1.0.6/src/cpdb_api/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,8 @@
-"""A Python API for NewClimate Institute's ClimatePolicy DataBase (CPDB).
-Installation
-
-```
-pip install ...
-```
-
-Example
-```
-import Request from ...
-import pandas as pd
-
-# for query to dev server
-r = request.Request()
-r.set_api_user(...)
-r.set_api_password(...)
-
-# set filters
-r.set_country("IND")
-r.set_decision_date(2010)
-r.set_policy_status("Planned")
-r.add_sector("Electricity and heat")
-r.add_sector("General")
-r.add_policy_instrument("Direct investment")
-r.add_policy_instrument("Energy efficiency")
-r.add_policy_type("")
-
-# obtain filtered result as pandas Dataframe
-df = r.issue()
-
-# save the result to CSV file
-r.save_csv("filtered_cpdb.csv")
-```
-"""
+"""A Python API for NewClimate Institute's ClimatePolicy DataBase (CPDB)."""
 
 import json
 
 import pandas as pd
 import requests
 from requests.auth import HTTPBasicAuth
 
@@ -59,38 +26,14 @@
         self._response = ""
         self._sector = ""
         self._policy_instrument = ""
         self._policy_type = ""
         self._data_frame = ""
         self._properties = dict()
 
-    # Pre-formatted requests
-    def set_request(self, r):
-        """
-        :param r: the request, in proper JSON format per https://github/<path>/<to>/<version>/<controlled>/<schema>
-        :return: none
-        """
-        self._request = r
-
-    def set_api_user(self, u):
-        """
-        Sets the API username for the request.
-        :param u: the username to be used for authenticating to the API
-        :return: none
-        """
-        self._api_user = u
-
-    def set_api_password(self, p):
-        """
-        Sets the API password for the request.
-        :param p: the password to be used for authenticating to the API
-        :return: none
-        """
-        self._api_password = p
-
     def set_country(self, c):
         """
         :param c: the name of the ISO country code
         :return: none
         """
         # sets a string country for this request
         self._country = c
@@ -134,24 +77,24 @@
         e.g. performance label, the server will treat it as a query for all contained groups.
 
         :param policy_instrument: a list of policy instruments to add to the query.
         :return: none
         """
         self._policy_instrument = ",".join(policy_instrument)
 
-    def add_policy_type(self, policy_type):
+    def add_mitigation_area(self, mitigation_area):
         """
-        A list of policy types (mitigation areas) to query. Items must be one of:
+        A list of mitigation areas to query. Items must be one of:
         energy efficiency, energy service demand reduction and resource efficiency, 
         non energy use, other low carbon technologies and fuel switch, renewables, unknown
 
         :param policy_type: a list of policy types to add to the query.
         :return: none
         """
-        self._policy_type = ",".join(policy_type)
+        self._policy_type = ",".join(mitigation_area)
 
     # For request issuing & data retrieval.
     def issue(self):
         """
         Issues this request against the API.
         :return: the response from the server
         """
@@ -203,7 +146,32 @@
             properties["sector"] = self._sector
         if self._policy_instrument != "":
             properties["policy_instrument"] = self._policy_instrument
         if self._policy_type != "":
             properties["policy_type"] = self._policy_type
         self._properties = properties
         return properties
+
+    # Helpers for testing
+    def set_request(self, r):
+        """
+        :param r: the request, in proper JSON format (for testing)
+        :return: none
+        """
+        self._request = r
+
+    def set_api_user(self, u):
+        """
+        Sets the API username for the request.
+        :param u: the username to be used for authenticating to the API
+        :return: none
+        """
+        self._api_user = u
+
+    def set_api_password(self, p):
+        """
+        Sets the API password for the request.
+        :param p: the password to be used for authenticating to the API
+        :return: none
+        """
+        self._api_password = p
+
```

### Comparing `cpdb_api-1.0.5/src/cpdb_api.egg-info/PKG-INFO` & `cpdb_api-1.0.6/src/cpdb_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpdb-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: An API to access the NewClimate Institute's Climate Policy Database
 Author-email: NewClimate Institute <info@newclimate.org>
 Project-URL: Homepage, https://climatepolicydatabase.org
 Project-URL: Source Code, https://github.com/KevinDackow/CPDB-API
 Keywords: nci,cpdb,climatepolicydatabase,newclimateinstitute
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -34,19 +34,19 @@
 from cpdb_api import request 
 
 r = request.Request()
 
 # set filters
 r.set_country("IND")
 r.set_decision_date(2010)
-r.set_policy_status("Planned")
+r.set_policy_status("In force")
 r.add_sector("Electricity and heat")
-r.add_sector("General")
-r.add_policy_instrument("Direct investment")
-r.add_policy_instrument("Energy efficiency")
+r.add_sector("Coal")
+r.add_policy_instrument("Energy and other taxes")
+r.add_mitigation_area("Renewables")
 
 # Issue the request (this returns a pandas dataframe, if you want to parse it programmatically)
 r.issue()
 
 # save the result to CSV file
 r.save_csv("filtered_cpdb.csv")
 ```
```

