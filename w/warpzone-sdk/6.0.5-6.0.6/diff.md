# Comparing `tmp/warpzone_sdk-6.0.5.tar.gz` & `tmp/warpzone_sdk-6.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warpzone_sdk-6.0.5.tar", max compression
+gzip compressed data, was "warpzone_sdk-6.0.6.tar", max compression
```

## Comparing `warpzone_sdk-6.0.5.tar` & `warpzone_sdk-6.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1121 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/pyproject.toml
--rw-r--r--   0        0        0     1182 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/__init__.py
--rw-r--r--   0        0        0       21 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/blobstorage/__init__.py
--rw-r--r--   0        0        0     2874 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/blobstorage/client.py
--rw-r--r--   0        0        0       24 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/enums/__init__.py
--rw-r--r--   0        0        0      187 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/enums/topicenum.py
--rw-r--r--   0        0        0       27 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/function/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/function/functionize.py
--rw-r--r--   0        0        0     3035 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/function/integrations.py
--rw-r--r--   0        0        0     2223 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/function/monitor.py
--rw-r--r--   0        0        0     1486 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/function/process.py
--rw-r--r--   0        0        0       32 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/function/processors/__init__.py
--rw-r--r--   0        0        0     1910 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/function/processors/outputs.py
--rw-r--r--   0        0        0     1727 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/function/processors/triggers.py
--rw-r--r--   0        0        0     2268 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/function/signature.py
--rw-r--r--   0        0        0       80 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/function/types.py
--rw-r--r--   0        0        0     2108 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/healthchecks/__init__.py
--rw-r--r--   0        0        0     1112 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/healthchecks/model.py
--rw-r--r--   0        0        0       87 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/monitor/__init__.py
--rw-r--r--   0        0        0     1650 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/monitor/logs.py
--rw-r--r--   0        0        0     4781 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/monitor/traces.py
--rw-r--r--   0        0        0       21 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/servicebus/data/__init__.py
--rw-r--r--   0        0        0     5403 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/servicebus/data/client.py
--rw-r--r--   0        0        0       21 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/servicebus/events/__init__.py
--rw-r--r--   0        0        0     4250 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/servicebus/events/client.py
--rw-r--r--   0        0        0       47 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/tablestorage/__init__.py
--rw-r--r--   0        0        0     2882 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/tablestorage/client.py
--rw-r--r--   0        0        0     2509 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/tablestorage/client_async.py
--rw-r--r--   0        0        0      521 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/tablestorage/helpers.py
--rw-r--r--   0        0        0     2470 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/tablestorage/operations.py
--rw-r--r--   0        0        0      219 2023-05-04 13:02:55.137435 warpzone_sdk-6.0.5/warpzone/testing/__init__.py
--rw-r--r--   0        0        0     2790 2023-05-04 13:02:55.141435 warpzone_sdk-6.0.5/warpzone/testing/assertions.py
--rw-r--r--   0        0        0     3499 2023-05-04 13:02:55.141435 warpzone_sdk-6.0.5/warpzone/testing/data.py
--rw-r--r--   0        0        0       19 2023-05-04 13:02:55.141435 warpzone_sdk-6.0.5/warpzone/transform/__init__.py
--rw-r--r--   0        0        0     1641 2023-05-04 13:02:55.141435 warpzone_sdk-6.0.5/warpzone/transform/data.py
--rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 warpzone_sdk-6.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-05-22 13:42:03.793304 warpzone_sdk-6.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1182 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/blobstorage/__init__.py
+-rw-r--r--   0        0        0     2874 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/blobstorage/client.py
+-rw-r--r--   0        0        0       24 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/enums/__init__.py
+-rw-r--r--   0        0        0      213 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/enums/topicenum.py
+-rw-r--r--   0        0        0       27 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/functionize.py
+-rw-r--r--   0        0        0     3035 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/integrations.py
+-rw-r--r--   0        0        0     2223 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/monitor.py
+-rw-r--r--   0        0        0     1486 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/process.py
+-rw-r--r--   0        0        0       32 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/processors/__init__.py
+-rw-r--r--   0        0        0     1910 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/processors/outputs.py
+-rw-r--r--   0        0        0     1727 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/processors/triggers.py
+-rw-r--r--   0        0        0     2268 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/signature.py
+-rw-r--r--   0        0        0       80 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/function/types.py
+-rw-r--r--   0        0        0     2108 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/healthchecks/__init__.py
+-rw-r--r--   0        0        0     1112 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/healthchecks/model.py
+-rw-r--r--   0        0        0       87 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/monitor/__init__.py
+-rw-r--r--   0        0        0     1650 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/monitor/logs.py
+-rw-r--r--   0        0        0     4781 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/monitor/traces.py
+-rw-r--r--   0        0        0       21 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/servicebus/data/__init__.py
+-rw-r--r--   0        0        0     5403 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/servicebus/data/client.py
+-rw-r--r--   0        0        0       21 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/servicebus/events/__init__.py
+-rw-r--r--   0        0        0     4250 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/servicebus/events/client.py
+-rw-r--r--   0        0        0       47 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/tablestorage/__init__.py
+-rw-r--r--   0        0        0     2882 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/tablestorage/client.py
+-rw-r--r--   0        0        0     2509 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/tablestorage/client_async.py
+-rw-r--r--   0        0        0      521 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/tablestorage/helpers.py
+-rw-r--r--   0        0        0     2470 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/tablestorage/operations.py
+-rw-r--r--   0        0        0      219 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/testing/__init__.py
+-rw-r--r--   0        0        0     2790 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/testing/assertions.py
+-rw-r--r--   0        0        0     3499 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/testing/data.py
+-rw-r--r--   0        0        0       19 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/transform/__init__.py
+-rw-r--r--   0        0        0     1641 2023-05-22 13:42:03.797304 warpzone_sdk-6.0.6/warpzone/transform/data.py
+-rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 warpzone_sdk-6.0.6/PKG-INFO
```

### Comparing `warpzone_sdk-6.0.5/pyproject.toml` & `warpzone_sdk-6.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "warpzone-sdk"
-version = "6.0.5"
+version = "6.0.6"
 description = "The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage"
 authors = ["Anders Launer Baek-Petersen <alp@energinet.dk>", "Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "warpzone" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^1.4.3"
 pyarrow = "^9.0.0"
 azure-data-tables = "^12.4.0"
-azure-servicebus = "^7.8.0"
+azure-servicebus = "~7.8.0"
 azure-storage-blob = "^12.14.1"
 aiohttp = "^3.8.3"
 azure-core-tracing-opentelemetry = "^1.0.0b9"
 azure-monitor-opentelemetry-exporter = "^1.0.0b11"
 opentelemetry-sdk = "1.14.0"
 azure-functions = "^1.12.0"
 typeguard = "^3.0.1"
```

### Comparing `warpzone_sdk-6.0.5/warpzone/__init__.py` & `warpzone_sdk-6.0.6/warpzone/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/blobstorage/client.py` & `warpzone_sdk-6.0.6/warpzone/blobstorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/function/functionize.py` & `warpzone_sdk-6.0.6/warpzone/function/functionize.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/function/integrations.py` & `warpzone_sdk-6.0.6/warpzone/function/integrations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/function/monitor.py` & `warpzone_sdk-6.0.6/warpzone/function/monitor.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/function/process.py` & `warpzone_sdk-6.0.6/warpzone/function/process.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/function/processors/outputs.py` & `warpzone_sdk-6.0.6/warpzone/function/processors/outputs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/function/processors/triggers.py` & `warpzone_sdk-6.0.6/warpzone/function/processors/triggers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/function/signature.py` & `warpzone_sdk-6.0.6/warpzone/function/signature.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/healthchecks/__init__.py` & `warpzone_sdk-6.0.6/warpzone/healthchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/healthchecks/model.py` & `warpzone_sdk-6.0.6/warpzone/healthchecks/model.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/monitor/logs.py` & `warpzone_sdk-6.0.6/warpzone/monitor/logs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/monitor/traces.py` & `warpzone_sdk-6.0.6/warpzone/monitor/traces.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/servicebus/data/client.py` & `warpzone_sdk-6.0.6/warpzone/servicebus/data/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/servicebus/events/client.py` & `warpzone_sdk-6.0.6/warpzone/servicebus/events/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/tablestorage/client.py` & `warpzone_sdk-6.0.6/warpzone/tablestorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/tablestorage/client_async.py` & `warpzone_sdk-6.0.6/warpzone/tablestorage/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/tablestorage/helpers.py` & `warpzone_sdk-6.0.6/warpzone/tablestorage/helpers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/tablestorage/operations.py` & `warpzone_sdk-6.0.6/warpzone/tablestorage/operations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/testing/assertions.py` & `warpzone_sdk-6.0.6/warpzone/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/testing/data.py` & `warpzone_sdk-6.0.6/warpzone/testing/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/warpzone/transform/data.py` & `warpzone_sdk-6.0.6/warpzone/transform/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.5/PKG-INFO` & `warpzone_sdk-6.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: warpzone-sdk
-Version: 6.0.5
+Version: 6.0.6
 Summary: The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage
 Author: Anders Launer Baek-Petersen
 Author-email: alp@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: azure-core-tracing-opentelemetry (>=1.0.0b9,<2.0.0)
 Requires-Dist: azure-data-tables (>=12.4.0,<13.0.0)
 Requires-Dist: azure-functions (>=1.12.0,<2.0.0)
 Requires-Dist: azure-monitor-opentelemetry-exporter (>=1.0.0b11,<2.0.0)
-Requires-Dist: azure-servicebus (>=7.8.0,<8.0.0)
+Requires-Dist: azure-servicebus (>=7.8.0,<7.9.0)
 Requires-Dist: azure-storage-blob (>=12.14.1,<13.0.0)
 Requires-Dist: opentelemetry-sdk (==1.14.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: pyarrow (>=9.0.0,<10.0.0)
 Requires-Dist: typeguard (>=3.0.1,<4.0.0)
```

