# Comparing `tmp/openstef_dbc-3.6.7.tar.gz` & `tmp/openstef_dbc-3.6.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstef_dbc-3.6.7.tar", last modified: Tue May  9 10:02:52 2023, max compression
+gzip compressed data, was "openstef_dbc-3.6.8a0.tar", last modified: Mon May 22 08:18:20 2023, max compression
```

## Comparing `openstef_dbc-3.6.7.tar` & `openstef_dbc-3.6.8a0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:02:52.328148 openstef_dbc-3.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-09 10:02:52.332147 openstef_dbc-3.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:02:52.328148 openstef_dbc-3.6.7/openstef_dbc/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/data_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/ktp_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:02:52.328148 openstef_dbc-3.6.7/openstef_dbc/log/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/log/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/log/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:02:52.328148 openstef_dbc-3.6.7/openstef_dbc/models/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/models/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/models/switch_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:02:52.328148 openstef_dbc-3.6.7/openstef_dbc/services/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/ems.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/model_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:02:52.328148 openstef_dbc-3.6.7/openstef_dbc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-09 10:02:52.000000 openstef_dbc-3.6.7/openstef_dbc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-09 10:02:52.000000 openstef_dbc-3.6.7/openstef_dbc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:02:52.000000 openstef_dbc-3.6.7/openstef_dbc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-09 10:02:52.000000 openstef_dbc-3.6.7/openstef_dbc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 10:02:52.000000 openstef_dbc-3.6.7/openstef_dbc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-09 10:02:52.332147 openstef_dbc-3.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:18:20.365029 openstef_dbc-3.6.8a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-22 08:18:20.365029 openstef_dbc-3.6.8a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:18:20.361029 openstef_dbc-3.6.8a0/openstef_dbc/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/data_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/ktp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:18:20.361029 openstef_dbc-3.6.8a0/openstef_dbc/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/log/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/log/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:18:20.361029 openstef_dbc-3.6.8a0/openstef_dbc/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/models/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/models/switch_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:18:20.365029 openstef_dbc-3.6.8a0/openstef_dbc/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/services/ems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/services/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/services/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/services/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/services/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/services/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/services/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/services/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15888 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/services/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/openstef_dbc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:18:20.361029 openstef_dbc-3.6.8a0/openstef_dbc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-22 08:18:20.000000 openstef_dbc-3.6.8a0/openstef_dbc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-22 08:18:20.000000 openstef_dbc-3.6.8a0/openstef_dbc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:18:20.000000 openstef_dbc-3.6.8a0/openstef_dbc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 08:18:20.000000 openstef_dbc-3.6.8a0/openstef_dbc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 08:18:20.000000 openstef_dbc-3.6.8a0/openstef_dbc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 08:18:20.365029 openstef_dbc-3.6.8a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-22 08:18:03.000000 openstef_dbc-3.6.8a0/setup.py
```

### Comparing `openstef_dbc-3.6.7/LICENSE` & `openstef_dbc-3.6.8a0/LICENSE`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/PKG-INFO` & `openstef_dbc-3.6.8a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef_dbc
-Version: 3.6.7
+Version: 3.6.8a0
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.7/README.md` & `openstef_dbc-3.6.8a0/README.md`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/__init__.py` & `openstef_dbc-3.6.8a0/openstef_dbc/__init__.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/data_interface.py` & `openstef_dbc-3.6.8a0/openstef_dbc/data_interface.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/database.py` & `openstef_dbc-3.6.8a0/openstef_dbc/database.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/ktp_api.py` & `openstef_dbc-3.6.8a0/openstef_dbc/ktp_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class ApiException(Exception):
     pass
 
 
 class KtpApi:
     """Used for all api traffic to Influx API"""
 
-    __INFLUX_TEST_URL = "api/influx/ping"
+    __INFLUX_TEST_URL = "api/_core/health/liveness"
     __MEASUREMENTS_URL = "api/measurements"
     __SYSTEMS_URL = "admin/systems"
     __TRACY_JOB_URL = "admin/tracyjobs"
 
     __ALL_TRACY_JOBS = -999
 
     def __init__(
```

### Comparing `openstef_dbc-3.6.7/openstef_dbc/log/logging.py` & `openstef_dbc-3.6.8a0/openstef_dbc/log/logging.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/log/processors.py` & `openstef_dbc-3.6.8a0/openstef_dbc/log/processors.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/models/measurement.py` & `openstef_dbc-3.6.8a0/openstef_dbc/models/measurement.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/services/ems.py` & `openstef_dbc-3.6.8a0/openstef_dbc/services/ems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/services/model_input.py` & `openstef_dbc-3.6.8a0/openstef_dbc/services/model_input.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/services/prediction_job.py` & `openstef_dbc-3.6.8a0/openstef_dbc/services/prediction_job.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/services/predictions.py` & `openstef_dbc-3.6.8a0/openstef_dbc/services/predictions.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/services/predictor.py` & `openstef_dbc-3.6.8a0/openstef_dbc/services/predictor.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/services/splitting.py` & `openstef_dbc-3.6.8a0/openstef_dbc/services/splitting.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/services/systems.py` & `openstef_dbc-3.6.8a0/openstef_dbc/services/systems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/services/weather.py` & `openstef_dbc-3.6.8a0/openstef_dbc/services/weather.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc/services/write.py` & `openstef_dbc-3.6.8a0/openstef_dbc/services/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,22 +84,32 @@
 
         # Cast columns to correct type, as influx is extremely picky
         casting_dict = {"prediction": float, "stdev": float}
         for col, cast in casting_dict.items():
             if col in field_columns:
                 forecast = forecast.astype({col: cast})
 
-        result = _DataInterface.get_instance().exec_influx_write(
-            forecast.copy(),
-            database=dbname,
-            measurement=influxtable,
-            tag_columns=tag_columns,
-            field_columns=field_columns,
-            time_precision="s",
-        )
+        try:
+            result = _DataInterface.get_instance().exec_influx_write(
+                forecast.copy(),
+                database=dbname,
+                measurement=influxtable,
+                tag_columns=tag_columns,
+                field_columns=field_columns,
+                time_precision="s",
+            )
+        except Exception as e:
+            result = _DataInterface.get_instance().exec_influx_write(
+                forecast.copy().rename(columns={"created": "created_temp"}),
+                database=dbname,
+                measurement=influxtable,
+                tag_columns=tag_columns,
+                field_columns=field_columns,
+                time_precision="s",
+            )
 
         message = ""
 
         if result:
             num_rows = str(len(forecast))
             self.logger.info(
                 "Succesfully written Forecast to database",
```

### Comparing `openstef_dbc-3.6.7/openstef_dbc/utils.py` & `openstef_dbc-3.6.8a0/openstef_dbc/utils.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/openstef_dbc.egg-info/PKG-INFO` & `openstef_dbc-3.6.8a0/openstef_dbc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef-dbc
-Version: 3.6.7
+Version: 3.6.8a0
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.7/openstef_dbc.egg-info/SOURCES.txt` & `openstef_dbc-3.6.8a0/openstef_dbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.7/setup.py` & `openstef_dbc-3.6.8a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def read_long_description_from_readme():
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setup(
     name="openstef_dbc",
-    version="3.6.7",
+    version="3.6.8a",
     packages=find_packages(include=["openstef_dbc", "openstef_dbc.*"]),
     description="Database Connection for OpenSTEF",
     long_description=read_long_description_from_readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/openstef/openstef-dbc",
     author="Alliander N.V",
     author_email="korte.termijn.prognoses@alliander.com",
```

