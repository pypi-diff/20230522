# Comparing `tmp/squad_ds_utils-0.1.7.tar.gz` & `tmp/squad_ds_utils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squad_ds_utils-0.1.7.tar", max compression
+gzip compressed data, was "squad_ds_utils-0.1.8.tar", max compression
```

## Comparing `squad_ds_utils-0.1.7.tar` & `squad_ds_utils-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-05-19 08:44:34.686815 squad_ds_utils-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-05-22 11:28:45.283180 squad_ds_utils-0.1.7/database_connector/__init__.py
--rw-r--r--   0        0        0      563 2023-05-22 13:03:20.017766 squad_ds_utils-0.1.7/database_connector/constants.py
--rw-r--r--   0        0        0     1197 2023-05-22 11:28:45.283725 squad_ds_utils-0.1.7/database_connector/sagemaker.py
--rw-r--r--   0        0        0     1675 2023-05-22 13:15:39.958263 squad_ds_utils-0.1.7/database_connector/snowflake_ds.py
--rw-r--r--   0        0        0     1437 2023-05-22 11:28:45.284158 squad_ds_utils-0.1.7/database_connector/utils.py
--rw-r--r--   0        0        0      515 2023-05-22 13:33:12.300222 squad_ds_utils-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 08:44:34.687254 squad_ds_utils-0.1.7/squad_ds_utils/__init__.py
--rw-r--r--   0        0        0       40 2023-05-19 08:44:34.687346 squad_ds_utils-0.1.7/squad_ds_utils/exceptions.py
--rw-r--r--   0        0        0      563 2023-05-19 08:44:34.687426 squad_ds_utils-0.1.7/squad_ds_utils/parse.py
--rw-r--r--   0        0        0     2321 2023-05-19 08:44:34.687525 squad_ds_utils-0.1.7/squad_ds_utils/recordings_fetcher.py
--rw-r--r--   0        0        0      628 2023-05-19 08:44:34.687608 squad_ds_utils-0.1.7/squad_ds_utils/secrets.py
--rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 squad_ds_utils-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-19 08:44:34.686815 squad_ds_utils-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 11:28:45.283180 squad_ds_utils-0.1.8/database_connector/__init__.py
+-rw-r--r--   0        0        0      563 2023-05-22 13:03:20.017766 squad_ds_utils-0.1.8/database_connector/constants.py
+-rw-r--r--   0        0        0     1197 2023-05-22 11:28:45.283725 squad_ds_utils-0.1.8/database_connector/sagemaker.py
+-rw-r--r--   0        0        0     1642 2023-05-22 13:43:42.876396 squad_ds_utils-0.1.8/database_connector/snowflake_ds.py
+-rw-r--r--   0        0        0     1437 2023-05-22 11:28:45.284158 squad_ds_utils-0.1.8/database_connector/utils.py
+-rw-r--r--   0        0        0      515 2023-05-22 13:44:10.924304 squad_ds_utils-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 08:44:34.687254 squad_ds_utils-0.1.8/squad_ds_utils/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-19 08:44:34.687346 squad_ds_utils-0.1.8/squad_ds_utils/exceptions.py
+-rw-r--r--   0        0        0      563 2023-05-19 08:44:34.687426 squad_ds_utils-0.1.8/squad_ds_utils/parse.py
+-rw-r--r--   0        0        0     2321 2023-05-19 08:44:34.687525 squad_ds_utils-0.1.8/squad_ds_utils/recordings_fetcher.py
+-rw-r--r--   0        0        0      628 2023-05-19 08:44:34.687608 squad_ds_utils-0.1.8/squad_ds_utils/secrets.py
+-rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 squad_ds_utils-0.1.8/PKG-INFO
```

### Comparing `squad_ds_utils-0.1.7/database_connector/constants.py` & `squad_ds_utils-0.1.8/database_connector/constants.py`

 * *Files identical despite different names*

### Comparing `squad_ds_utils-0.1.7/database_connector/sagemaker.py` & `squad_ds_utils-0.1.8/database_connector/sagemaker.py`

 * *Files identical despite different names*

### Comparing `squad_ds_utils-0.1.7/database_connector/snowflake_ds.py` & `squad_ds_utils-0.1.8/database_connector/snowflake_ds.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,30 +22,30 @@
     """
     with open(SAGEMAKER_RESOURCE_PATH, 'r') as file:
         data = json.load(file)
 
     return data.get('UserProfileName')
 
 
-def get_connection(database: str, schema: str, user=None):
+def get_connection(database: str, schema: str):
     """
     makes connection with snowflake db
     :param database:
     :param schema:
     :param user:
     :return: connection
     """
     parameter_to_value_map = get_parameters([
         SNOWFLAKE_ACCOUNT_NAME_PARAMETER,
         SNOWFLAKE_WAREHOUSE_NAME_PARAMETER,
     ], AWS_REGION)
 
     account = parameter_to_value_map[SNOWFLAKE_ACCOUNT_NAME_PARAMETER]
     warehouse = parameter_to_value_map[SNOWFLAKE_WAREHOUSE_NAME_PARAMETER]
-    profile_user = get_user_details() if not user else user
+    profile_user = get_user_details()
     secrets = get_secret_value(f'snowflake/{profile_user}')
     password = secrets.get('password')
     username = secrets.get('username')
 
     return connector.connect(
         user = username,
         password = password,
```

### Comparing `squad_ds_utils-0.1.7/database_connector/utils.py` & `squad_ds_utils-0.1.8/database_connector/utils.py`

 * *Files identical despite different names*

### Comparing `squad_ds_utils-0.1.7/pyproject.toml` & `squad_ds_utils-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squad-ds-utils"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Ayush Shanker <ayush+pypi@squadstack.com>"]
 readme = "README.md"
 packages = [
     {include = "squad_ds_utils"},
     {include = "database_connector"},
 ]
```

### Comparing `squad_ds_utils-0.1.7/squad_ds_utils/parse.py` & `squad_ds_utils-0.1.8/squad_ds_utils/parse.py`

 * *Files identical despite different names*

### Comparing `squad_ds_utils-0.1.7/squad_ds_utils/recordings_fetcher.py` & `squad_ds_utils-0.1.8/squad_ds_utils/recordings_fetcher.py`

 * *Files identical despite different names*

### Comparing `squad_ds_utils-0.1.7/squad_ds_utils/secrets.py` & `squad_ds_utils-0.1.8/squad_ds_utils/secrets.py`

 * *Files identical despite different names*

### Comparing `squad_ds_utils-0.1.7/PKG-INFO` & `squad_ds_utils-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squad-ds-utils
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Ayush Shanker
 Author-email: ayush+pypi@squadstack.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

