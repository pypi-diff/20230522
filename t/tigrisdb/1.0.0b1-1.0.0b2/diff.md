# Comparing `tmp/tigrisdb-1.0.0b1.tar.gz` & `tmp/tigrisdb-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigrisdb-1.0.0b1.tar", max compression
+gzip compressed data, was "tigrisdb-1.0.0b2.tar", max compression
```

## Comparing `tigrisdb-1.0.0b1.tar` & `tigrisdb-1.0.0b2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/LICENSE
--rw-r--r--   0        0        0      957 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/README.md
--rw-r--r--   0        0        0     1583 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      313 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     1897 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/google/api/field_behavior_pb2.py
--rw-r--r--   0        0        0      685 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/google/api/field_behavior_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/google/api/field_behavior_pb2_grpc.py
--rw-r--r--   0        0        0     2125 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/google/api/http_pb2.py
--rw-r--r--   0        0        0     2272 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0     1507 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/google/api/httpbody_pb2.py
--rw-r--r--   0        0        0      882 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/google/api/httpbody_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/google/api/httpbody_pb2_grpc.py
--rw-r--r--   0        0        0    27129 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/openapiv3/OpenAPIv3_pb2.py
--rw-r--r--   0        0        0    49576 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/openapiv3/OpenAPIv3_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/openapiv3/OpenAPIv3_pb2_grpc.py
--rw-r--r--   0        0        0     2102 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/openapiv3/annotations_pb2.py
--rw-r--r--   0        0        0      555 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/openapiv3/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 20:21:16.744852 tigrisdb-1.0.0b1/api/generated/openapiv3/annotations_pb2_grpc.py
--rw-r--r--   0        0        0    44365 2023-05-19 20:21:16.740852 tigrisdb-1.0.0b1/api/generated/server/v1/api_pb2.py
--rw-r--r--   0        0        0    37886 2023-05-19 20:21:16.740852 tigrisdb-1.0.0b1/api/generated/server/v1/api_pb2.pyi
--rw-r--r--   0        0        0    51527 2023-05-19 20:21:16.740852 tigrisdb-1.0.0b1/api/generated/server/v1/api_pb2_grpc.py
--rw-r--r--   0        0        0     7946 2023-05-19 20:21:16.740852 tigrisdb-1.0.0b1/api/generated/server/v1/auth_pb2.py
--rw-r--r--   0        0        0     6220 2023-05-19 20:21:16.740852 tigrisdb-1.0.0b1/api/generated/server/v1/auth_pb2.pyi
--rw-r--r--   0        0        0    11198 2023-05-19 20:21:16.740852 tigrisdb-1.0.0b1/api/generated/server/v1/auth_pb2_grpc.py
--rw-r--r--   0        0        0     9308 2023-05-19 20:21:16.740852 tigrisdb-1.0.0b1/api/generated/server/v1/observability_pb2.py
--rw-r--r--   0        0        0     8458 2023-05-19 20:21:16.740852 tigrisdb-1.0.0b1/api/generated/server/v1/observability_pb2.pyi
--rw-r--r--   0        0        0     7981 2023-05-19 20:21:16.740852 tigrisdb-1.0.0b1/api/generated/server/v1/observability_pb2_grpc.py
--rw-r--r--   0        0        0    14625 2023-05-19 20:21:16.740852 tigrisdb-1.0.0b1/api/generated/server/v1/search_pb2.py
--rw-r--r--   0        0        0    11907 2023-05-19 20:21:16.740852 tigrisdb-1.0.0b1/api/generated/server/v1/search_pb2.pyi
--rw-r--r--   0        0        0    23238 2023-05-19 20:21:16.740852 tigrisdb-1.0.0b1/api/generated/server/v1/search_pb2_grpc.py
--rw-r--r--   0        0        0     1147 2023-05-19 20:21:22.328864 tigrisdb-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/tigrisdb/__init__.py
--rw-r--r--   0        0        0     2799 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/tigrisdb/auth.py
--rw-r--r--   0        0        0     2333 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/tigrisdb/client.py
--rw-r--r--   0        0        0     1968 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/tigrisdb/collection.py
--rw-r--r--   0        0        0     1986 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/tigrisdb/database.py
--rw-r--r--   0        0        0      484 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/tigrisdb/errors.py
--rw-r--r--   0        0        0     1720 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/tigrisdb/search.py
--rw-r--r--   0        0        0     3664 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/tigrisdb/search_index.py
--rw-r--r--   0        0        0      458 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/tigrisdb/types/__init__.py
--rw-r--r--   0        0        0     5062 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/tigrisdb/types/search.py
--rw-r--r--   0        0        0      527 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/tigrisdb/types/sort.py
--rw-r--r--   0        0        0      722 2023-05-19 20:20:27.732631 tigrisdb-1.0.0b1/tigrisdb/utils.py
--rw-r--r--   0        0        0     1981 1970-01-01 00:00:00.000000 tigrisdb-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0      935 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/README.md
+-rw-r--r--   0        0        0     1583 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      313 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     1897 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/field_behavior_pb2.py
+-rw-r--r--   0        0        0      685 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/field_behavior_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/field_behavior_pb2_grpc.py
+-rw-r--r--   0        0        0     2125 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/http_pb2.py
+-rw-r--r--   0        0        0     2272 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0     1507 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/httpbody_pb2.py
+-rw-r--r--   0        0        0      882 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/httpbody_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/google/api/httpbody_pb2_grpc.py
+-rw-r--r--   0        0        0    27129 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/openapiv3/OpenAPIv3_pb2.py
+-rw-r--r--   0        0        0    49576 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/openapiv3/OpenAPIv3_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/openapiv3/OpenAPIv3_pb2_grpc.py
+-rw-r--r--   0        0        0     2102 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/openapiv3/annotations_pb2.py
+-rw-r--r--   0        0        0      555 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/openapiv3/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/openapiv3/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0    44365 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/api_pb2.py
+-rw-r--r--   0        0        0    37886 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/api_pb2.pyi
+-rw-r--r--   0        0        0    51527 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/api_pb2_grpc.py
+-rw-r--r--   0        0        0     7946 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/auth_pb2.py
+-rw-r--r--   0        0        0     6220 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/auth_pb2.pyi
+-rw-r--r--   0        0        0    11198 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/auth_pb2_grpc.py
+-rw-r--r--   0        0        0     9308 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/observability_pb2.py
+-rw-r--r--   0        0        0     8458 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/observability_pb2.pyi
+-rw-r--r--   0        0        0     7981 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/observability_pb2_grpc.py
+-rw-r--r--   0        0        0    14625 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/search_pb2.py
+-rw-r--r--   0        0        0    11907 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/search_pb2.pyi
+-rw-r--r--   0        0        0    23238 2023-05-22 16:31:00.189006 tigrisdb-1.0.0b2/api/generated/server/v1/search_pb2_grpc.py
+-rw-r--r--   0        0        0     1147 2023-05-22 16:31:06.181302 tigrisdb-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/__init__.py
+-rw-r--r--   0        0        0     2799 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/auth.py
+-rw-r--r--   0        0        0     2333 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/client.py
+-rw-r--r--   0        0        0     1968 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/collection.py
+-rw-r--r--   0        0        0     1986 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/database.py
+-rw-r--r--   0        0        0      484 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/errors.py
+-rw-r--r--   0        0        0     1720 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/search.py
+-rw-r--r--   0        0        0     4587 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/search_index.py
+-rw-r--r--   0        0        0      497 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/types/__init__.py
+-rw-r--r--   0        0        0     8746 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/types/search.py
+-rw-r--r--   0        0        0      527 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/types/sort.py
+-rw-r--r--   0        0        0      760 2023-05-22 16:30:10.266337 tigrisdb-1.0.0b2/tigrisdb/utils.py
+-rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 tigrisdb-1.0.0b2/PKG-INFO
```

### Comparing `tigrisdb-1.0.0b1/LICENSE` & `tigrisdb-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/README.md` & `tigrisdb-1.0.0b2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # tigris-client-python
 
 Python client for Tigris
 
 ## Installation
 
 ```commandline
-pip install tigris-client-python>=1.0.0.b1
+pip install tigrisdb
 ```
 
 # Usage
 
 See reference implementation in `./tests` directory that uses Tigris on `localhost:8081`
 
 # Development
```

### Comparing `tigrisdb-1.0.0b1/api/generated/google/api/annotations_pb2.py` & `tigrisdb-1.0.0b2/api/generated/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/google/api/field_behavior_pb2.py` & `tigrisdb-1.0.0b2/api/generated/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/google/api/field_behavior_pb2.pyi` & `tigrisdb-1.0.0b2/api/generated/google/api/field_behavior_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/google/api/http_pb2.py` & `tigrisdb-1.0.0b2/api/generated/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/google/api/http_pb2.pyi` & `tigrisdb-1.0.0b2/api/generated/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/google/api/httpbody_pb2.py` & `tigrisdb-1.0.0b2/api/generated/google/api/httpbody_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/google/api/httpbody_pb2.pyi` & `tigrisdb-1.0.0b2/api/generated/google/api/httpbody_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/openapiv3/OpenAPIv3_pb2.py` & `tigrisdb-1.0.0b2/api/generated/openapiv3/OpenAPIv3_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/openapiv3/OpenAPIv3_pb2.pyi` & `tigrisdb-1.0.0b2/api/generated/openapiv3/OpenAPIv3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/openapiv3/annotations_pb2.py` & `tigrisdb-1.0.0b2/api/generated/openapiv3/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/openapiv3/annotations_pb2.pyi` & `tigrisdb-1.0.0b2/api/generated/openapiv3/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/server/v1/api_pb2.py` & `tigrisdb-1.0.0b2/api/generated/server/v1/api_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/server/v1/api_pb2.pyi` & `tigrisdb-1.0.0b2/api/generated/server/v1/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/server/v1/api_pb2_grpc.py` & `tigrisdb-1.0.0b2/api/generated/server/v1/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/server/v1/auth_pb2.py` & `tigrisdb-1.0.0b2/api/generated/server/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/server/v1/auth_pb2.pyi` & `tigrisdb-1.0.0b2/api/generated/server/v1/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/server/v1/auth_pb2_grpc.py` & `tigrisdb-1.0.0b2/api/generated/server/v1/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/server/v1/observability_pb2.py` & `tigrisdb-1.0.0b2/api/generated/server/v1/observability_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/server/v1/observability_pb2.pyi` & `tigrisdb-1.0.0b2/api/generated/server/v1/observability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/server/v1/observability_pb2_grpc.py` & `tigrisdb-1.0.0b2/api/generated/server/v1/observability_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/server/v1/search_pb2.py` & `tigrisdb-1.0.0b2/api/generated/server/v1/search_pb2.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/server/v1/search_pb2.pyi` & `tigrisdb-1.0.0b2/api/generated/server/v1/search_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/api/generated/server/v1/search_pb2_grpc.py` & `tigrisdb-1.0.0b2/api/generated/server/v1/search_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/pyproject.toml` & `tigrisdb-1.0.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tigrisdb"
-version = "1.0.0-beta.1"
+version = "1.0.0-beta.2"
 description = "Python SDK for Tigris <http://www.tigrisdata.com>"
 authors = ["Tigris team <support@tigrisdata.com>"]
 repository = "https://www.github.com/tigrisdata/tigris-client-python"
 documentation = "https://www.tigrisdata.com/docs/"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -33,12 +33,12 @@
 
 [tool.coverage.run]
 source = ["tigrisdb"]
 branch = true
 command_line = "-m unittest discover -s tests -p 'test_*.py'"
 
 [tool.coverage.report]
-fail_under = 40
+fail_under = 70
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tigrisdb-1.0.0b1/tigrisdb/auth.py` & `tigrisdb-1.0.0b2/tigrisdb/auth.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/tigrisdb/client.py` & `tigrisdb-1.0.0b2/tigrisdb/client.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/tigrisdb/collection.py` & `tigrisdb-1.0.0b2/tigrisdb/collection.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/tigrisdb/database.py` & `tigrisdb-1.0.0b2/tigrisdb/database.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/tigrisdb/search.py` & `tigrisdb-1.0.0b2/tigrisdb/search.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/tigrisdb/types/sort.py` & `tigrisdb-1.0.0b2/tigrisdb/types/sort.py`

 * *Files identical despite different names*

### Comparing `tigrisdb-1.0.0b1/tigrisdb/utils.py` & `tigrisdb-1.0.0b2/tigrisdb/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import base64
 import json
+from typing import Union
 
 
 def obj_to_str(doc: object) -> str:
     return json.dumps(doc)
 
 
 def str_to_bytes(doc_str: str) -> bytes:
@@ -18,15 +19,15 @@
     return b.decode("utf-8")
 
 
 def str_to_obj(doc_str: str) -> object:
     return json.loads(doc_str)
 
 
-def unmarshal(b: bytes) -> object:
+def unmarshal(b: bytes) -> Union[object, dict]:
     return str_to_obj(bytes_to_str(b))
 
 
 def b64_to_object(b64_str: str) -> object:
     return unmarshal(base64.b64decode(b64_str))
```

### Comparing `tigrisdb-1.0.0b1/PKG-INFO` & `tigrisdb-1.0.0b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigrisdb
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Python SDK for Tigris <http://www.tigrisdata.com>
 Home-page: https://www.github.com/tigrisdata/tigris-client-python
 License: Apache-2.0
 Keywords: database,nosql,vector,search
 Author: Tigris team
 Author-email: support@tigrisdata.com
 Requires-Python: >=3.8,<4.0
@@ -26,15 +26,15 @@
 # tigris-client-python
 
 Python client for Tigris
 
 ## Installation
 
 ```commandline
-pip install tigris-client-python>=1.0.0.b1
+pip install tigrisdb
 ```
 
 # Usage
 
 See reference implementation in `./tests` directory that uses Tigris on `localhost:8081`
 
 # Development
```

