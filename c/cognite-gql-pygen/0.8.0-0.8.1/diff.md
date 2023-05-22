# Comparing `tmp/cognite_gql_pygen-0.8.0.tar.gz` & `tmp/cognite_gql_pygen-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_gql_pygen-0.8.0.tar", max compression
+gzip compressed data, was "cognite_gql_pygen-0.8.1.tar", max compression
```

## Comparing `cognite_gql_pygen-0.8.0.tar` & `cognite_gql_pygen-0.8.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11349 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/LICENSE
--rw-r--r--   0        0        0     5286 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/README.md
--rw-r--r--   0        0        0     8651 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/README.md
--rw-r--r--   0        0        0        0 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/__init__.py
--rw-r--r--   0        0        0      167 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/__init__.py
--rw-r--r--   0        0        0    19000 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/client_dm_v3.py
--rw-r--r--   0        0        0     3909 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/data_classes_dm_v3.py
--rw-r--r--   0        0        0     2593 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/get_client.py
--rwxr-xr-x   0        0        0      399 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/config.py
--rw-r--r--   0        0        0      192 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/custom_types/__init__.py
--rw-r--r--   0        0        0      236 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/custom_types/_scalars.py
--rw-r--r--   0        0        0      760 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/custom_types/jsonobject.py
--rw-r--r--   0        0        0     4724 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/custom_types/timestamp.py
--rw-r--r--   0        0        0      196 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/__init__.py
--rw-r--r--   0        0        0     6471 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/domain_client.py
--rw-r--r--   0        0        0     4065 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/domain_model.py
--rw-r--r--   0        0        0    19106 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/domain_model_api.py
--rw-r--r--   0        0        0     5929 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/relationship_api.py
--rw-r--r--   0        0        0     7060 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/schema.py
--rw-r--r--   0        0        0     3595 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/testing.py
--rw-r--r--   0        0        0     1423 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/misc.py
--rw-r--r--   0        0        0        0 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/py.typed
--rw-r--r--   0        0        0      146 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/__init__.py
--rw-r--r--   0        0        0     1904 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/data_classes.py
--rw-r--r--   0        0        0     1634 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/generator.py
--rw-r--r--   0        0        0     9042 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/main.py
--rw-r--r--   0        0        0      596 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/misc.py
--rw-r--r--   0        0        0     1425 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/parser.py
--rw-r--r--   0        0        0     1334 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/templates/client.txt
--rw-r--r--   0        0        0      807 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/templates/schema.txt
--rw-r--r--   0        0        0       22 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/version.py
--rw-r--r--   0        0        0     1946 2023-05-14 14:38:30.222308 cognite_gql_pygen-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6370 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/LICENSE
+-rw-r--r--   0        0        0      401 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/README.md
+-rw-r--r--   0        0        0     8651 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/cdf/__init__.py
+-rw-r--r--   0        0        0    19000 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/cdf/client_dm_v3.py
+-rw-r--r--   0        0        0     3909 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/cdf/data_classes_dm_v3.py
+-rw-r--r--   0        0        0     2593 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/cdf/get_client.py
+-rwxr-xr-x   0        0        0      399 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/config.py
+-rw-r--r--   0        0        0      192 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/custom_types/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/custom_types/_scalars.py
+-rw-r--r--   0        0        0      760 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/custom_types/jsonobject.py
+-rw-r--r--   0        0        0     4724 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/custom_types/timestamp.py
+-rw-r--r--   0        0        0      196 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/domain_modeling/__init__.py
+-rw-r--r--   0        0        0     6471 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/domain_modeling/domain_client.py
+-rw-r--r--   0        0        0     4065 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/domain_modeling/domain_model.py
+-rw-r--r--   0        0        0    19106 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/domain_modeling/domain_model_api.py
+-rw-r--r--   0        0        0     5929 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/domain_modeling/relationship_api.py
+-rw-r--r--   0        0        0     7060 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/domain_modeling/schema.py
+-rw-r--r--   0        0        0     3595 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/domain_modeling/testing.py
+-rw-r--r--   0        0        0     1423 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/misc.py
+-rw-r--r--   0        0        0        0 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/dm_clients/py.typed
+-rw-r--r--   0        0        0      146 2023-05-22 17:04:32.754341 cognite_gql_pygen-0.8.1/cognite/gqlpygen/__init__.py
+-rw-r--r--   0        0        0     1904 2023-05-22 17:04:32.758341 cognite_gql_pygen-0.8.1/cognite/gqlpygen/data_classes.py
+-rw-r--r--   0        0        0     1634 2023-05-22 17:04:32.758341 cognite_gql_pygen-0.8.1/cognite/gqlpygen/generator.py
+-rw-r--r--   0        0        0     9042 2023-05-22 17:04:32.758341 cognite_gql_pygen-0.8.1/cognite/gqlpygen/main.py
+-rw-r--r--   0        0        0      596 2023-05-22 17:04:32.758341 cognite_gql_pygen-0.8.1/cognite/gqlpygen/misc.py
+-rw-r--r--   0        0        0     1425 2023-05-22 17:04:32.758341 cognite_gql_pygen-0.8.1/cognite/gqlpygen/parser.py
+-rw-r--r--   0        0        0     1334 2023-05-22 17:04:32.758341 cognite_gql_pygen-0.8.1/cognite/gqlpygen/templates/client.txt
+-rw-r--r--   0        0        0      807 2023-05-22 17:04:32.758341 cognite_gql_pygen-0.8.1/cognite/gqlpygen/templates/schema.txt
+-rw-r--r--   0        0        0       22 2023-05-22 17:04:32.758341 cognite_gql_pygen-0.8.1/cognite/gqlpygen/version.py
+-rw-r--r--   0        0        0     1946 2023-05-22 17:04:32.758341 cognite_gql_pygen-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.8.1/PKG-INFO
```

### Comparing `cognite_gql_pygen-0.8.0/LICENSE` & `cognite_gql_pygen-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/dm_clients/README.md` & `cognite_gql_pygen-0.8.1/cognite/dm_clients/README.md`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/client_dm_v3.py` & `cognite_gql_pygen-0.8.1/cognite/dm_clients/cdf/client_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/data_classes_dm_v3.py` & `cognite_gql_pygen-0.8.1/cognite/dm_clients/cdf/data_classes_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/get_client.py` & `cognite_gql_pygen-0.8.1/cognite/dm_clients/cdf/get_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/dm_clients/custom_types/jsonobject.py` & `cognite_gql_pygen-0.8.1/cognite/dm_clients/custom_types/jsonobject.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/dm_clients/custom_types/timestamp.py` & `cognite_gql_pygen-0.8.1/cognite/dm_clients/custom_types/timestamp.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/domain_client.py` & `cognite_gql_pygen-0.8.1/cognite/dm_clients/domain_modeling/domain_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/domain_model.py` & `cognite_gql_pygen-0.8.1/cognite/dm_clients/domain_modeling/domain_model.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/domain_model_api.py` & `cognite_gql_pygen-0.8.1/cognite/dm_clients/domain_modeling/domain_model_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/relationship_api.py` & `cognite_gql_pygen-0.8.1/cognite/dm_clients/domain_modeling/relationship_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/schema.py` & `cognite_gql_pygen-0.8.1/cognite/dm_clients/domain_modeling/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/testing.py` & `cognite_gql_pygen-0.8.1/cognite/dm_clients/domain_modeling/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/dm_clients/misc.py` & `cognite_gql_pygen-0.8.1/cognite/dm_clients/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/gqlpygen/data_classes.py` & `cognite_gql_pygen-0.8.1/cognite/gqlpygen/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/gqlpygen/generator.py` & `cognite_gql_pygen-0.8.1/cognite/gqlpygen/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/gqlpygen/main.py` & `cognite_gql_pygen-0.8.1/cognite/gqlpygen/main.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/gqlpygen/misc.py` & `cognite_gql_pygen-0.8.1/cognite/gqlpygen/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/gqlpygen/parser.py` & `cognite_gql_pygen-0.8.1/cognite/gqlpygen/parser.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/gqlpygen/templates/client.txt` & `cognite_gql_pygen-0.8.1/cognite/gqlpygen/templates/client.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/cognite/gqlpygen/templates/schema.txt` & `cognite_gql_pygen-0.8.1/cognite/gqlpygen/templates/schema.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.8.0/pyproject.toml` & `cognite_gql_pygen-0.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-gql-pygen"
-version = "0.8.0"
+version = "0.8.1"
 description = "Cognite GraphQL Python Generation SDK"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache-2.0"
 
 packages = [{ include="cognite", from="." }]
 exclude = ["cognite/dm_clients/*.toml"]
```

