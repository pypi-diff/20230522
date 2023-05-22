# Comparing `tmp/censius-1.6.8.tar.gz` & `tmp/censius-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censius-1.6.8.tar", last modified: Mon Feb 27 14:58:42 2023, max compression
+gzip compressed data, was "censius-1.6.9.tar", last modified: Wed Apr  5 05:53:54 2023, max compression
```

## Comparing `censius-1.6.8.tar` & `censius-1.6.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:58:42.861607 censius-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-27 14:58:42.857607 censius-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-27 14:58:41.000000 censius-1.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-27 14:58:41.000000 censius-1.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 14:58:42.861607 censius-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-02-27 14:58:41.000000 censius-1.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:58:42.857607 censius-1.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:58:42.857607 censius-1.6.8/src/censius/
--rw-r--r--   0 runner    (1001) docker     (123)    37576 2023-02-27 14:58:41.000000 censius-1.6.8/src/censius/CensiusClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-27 14:58:41.000000 censius-1.6.8/src/censius/Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-27 14:58:41.000000 censius-1.6.8/src/censius/DatasetType.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-27 14:58:41.000000 censius-1.6.8/src/censius/Explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-27 14:58:41.000000 censius-1.6.8/src/censius/ExplanationType.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-27 14:58:41.000000 censius-1.6.8/src/censius/ModelType.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-27 14:58:41.000000 censius-1.6.8/src/censius/Prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-27 14:58:41.000000 censius-1.6.8/src/censius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-02-27 14:58:41.000000 censius-1.6.8/src/censius/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-27 14:58:41.000000 censius-1.6.8/src/censius/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-02-27 14:58:41.000000 censius-1.6.8/src/censius/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    21185 2023-02-27 14:58:41.000000 censius-1.6.8/src/censius/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:58:42.857607 censius-1.6.8/src/censius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-27 14:58:42.000000 censius-1.6.8/src/censius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-02-27 14:58:42.000000 censius-1.6.8/src/censius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 14:58:42.000000 censius-1.6.8/src/censius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-27 14:58:42.000000 censius-1.6.8/src/censius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-27 14:58:42.000000 censius-1.6.8/src/censius.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:53:54.372840 censius-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-05 05:53:54.372840 censius-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-05 05:53:50.000000 censius-1.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-05 05:53:50.000000 censius-1.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 05:53:54.372840 censius-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-05 05:53:50.000000 censius-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:53:54.372840 censius-1.6.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:53:54.372840 censius-1.6.9/src/censius/
+-rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/CensiusClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/DatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/Explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/ExplanationType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/ModelType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/Prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25007 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:53:54.372840 censius-1.6.9/src/censius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-05 05:53:54.000000 censius-1.6.9/src/censius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-05 05:53:54.000000 censius-1.6.9/src/censius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 05:53:54.000000 censius-1.6.9/src/censius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-05 05:53:54.000000 censius-1.6.9/src/censius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-05 05:53:54.000000 censius-1.6.9/src/censius.egg-info/top_level.txt
```

### Comparing `censius-1.6.8/PKG-INFO` & `censius-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censius
-Version: 1.6.8
+Version: 1.6.9
 Summary: API for Censius
 Home-page: https://github.com/Censius/censius-logs-python-sdk
 Author: Censius
 Author-email: dev@censius.ai
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `censius-1.6.8/setup.py` & `censius-1.6.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="censius",
-    version="1.6.8",
+    version="1.6.9",
     description="API for Censius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["censius/client"],
     package_dir={"": "src"},
     packages=["censius"],
     install_requires=["requests", "jsonschema", "pandas", "numpy"],
```

### Comparing `censius-1.6.8/src/censius/CensiusClient.py` & `censius-1.6.9/src/censius/CensiusClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,24 +192,48 @@
             return {"error": error_message}
         else:
             file.to_csv(file_name, index=False)
 
         """
             Validation for matching provided features and dataframe columns
             1. Check if provided features are present in the dataframe
-            2. Check if provided features are of type string
+            2. Check if provided features are of type string and alphanumeric
+            3. Check if provided features are of type string
+            4. Identify categorical features columns
         """
         provided_columns = [i["name"] for i in kwargs["features"]]
         dataframe_columns = list(file.columns)
         missing_columns = dataset_validation.check_provided_column_with_input_columns(
             provided_columns, dataframe_columns, []
         )
         if missing_columns:
             return {"error": f"Missing columns in the input dataframe: {missing_columns}"}
 
+        # 2. Check if provided features are of type string and alphanumeric
+        error_flag, error_list = dataset_validation.check_for_alphanumeric_features(
+            provided_columns
+        )
+        if error_flag:
+            return {"error": error_list}
+
+        # 3. Check if provided features are of type string
+        error_flag, error_list, cat_map = dataset_validation.fetch_categorical_features(
+            kwargs["features"]
+        )
+        if error_flag:
+            return {"error": error_list}
+
+        # 4. Identify categorical features columns
+        if cat_map:
+            error_flag, error_list = dataset_validation.validate_categorical_feature_from_input(
+                file, cat_map
+            )
+            if error_flag:
+                return {"error": error_list}
+
         headers = {"Authorization": f"Bearer {self.api_key}"}
 
         payload = {
             "name": kwargs["name"],
             "projectId": kwargs["project_id"],
             "version": Version,
             "features": json.dumps(kwargs["features"]),
@@ -222,14 +246,15 @@
         }
         files = [("File", (file_name, open(os.getcwd() + "/" + file_name, "rb"), "text/csv"))]
 
         response = requests.request(
             "POST", REGISTER_DATASET_URL(), headers=headers, data=payload, files=files
         )
         os.remove(os.getcwd() + "/" + file_name)
+
         return self.__return_message(response)
 
     def process_model(self, *args, **kwargs):
         try:
             validate(instance=kwargs, schema=process_model_schema)
         except ValidationError as e:
             return e.message
@@ -445,15 +470,18 @@
             """
                 Standard Validation for <timestamp_column>
                 1. Check if <timestamp_column> is in <input>
                 2. Check if <timestamp_column> is not Null
                 3. Check if <timestamp_column> is of type datetime
                 ↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓
             """
-            (error_flag, error_message,) = bulk_input_validation.timestamp_column_checks(
+            (
+                error_flag,
+                error_message,
+            ) = bulk_input_validation.timestamp_column_checks(
                 prediction_tabular["timestamp_column"], input
             )
             if error_flag:
                 return {"error": True, "message": error_message}
 
         if "explanations" in kwargs.keys():
             try:
@@ -593,15 +621,18 @@
 
             if no, then perform further checks
                 1. Check if all registered_features are present input dataframe columns
                     1.1: Except "registered_model_target"
                 2. Check if datatype of dataframe column is same as registered_features
                 3. Check if datatype of prediction column is same as registered_model_target
             """
-            (error_flag, error_message,) = bulk_input_validation.prediction_tabular_checks(
+            (
+                error_flag,
+                error_message,
+            ) = bulk_input_validation.prediction_tabular_checks(
                 input,
                 registered_dataset_to_datatype,
                 registered_model_target,
                 registered_to_provided,
             )
 
             if error_flag:
```

### Comparing `censius-1.6.8/src/censius/constants.py` & `censius-1.6.9/src/censius/constants.py`

 * *Files identical despite different names*

### Comparing `censius-1.6.8/src/censius/schemas.py` & `censius-1.6.9/src/censius/schemas.py`

 * *Files identical despite different names*

### Comparing `censius-1.6.8/src/censius/utils.py` & `censius-1.6.9/src/censius/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import random
+import re
 import string
 import threading
 import time
 from multiprocessing.pool import ThreadPool
 from typing import Any, Tuple
 from urllib import request
 from datetime import datetime
@@ -30,14 +31,35 @@
         if input.empty:
             return True, "  ValidationError: <input> dataframe is empty"
         # ..> if dataframe has empty row in middle return error
         # if input.isnull().any().any():
         #     return True, "  ValidationError: <input> dataframe has empty row in middle"
         return False, ""
 
+    def check_for_alphanumeric_features(self, provided_columns: list) -> Tuple[bool, str]:
+        # ..> if dataframe column name should only have alphanumeric characters, or underscore is allowed
+        error_columns = []
+        for column in provided_columns:
+            if re.match(r"^[a-z0-9_]+$", column) is None:
+                error_columns.append(column)
+
+        if len(error_columns) > 0:
+            message = (
+                f"""
+                    ValidationError: Dataset feature, and target variable name are 
+                    only accepted if they satisfy following constraints: 
+                    Lowercase Alphanumeric, and underscore. 
+                    <input> dataframe has columns violating rule : {error_columns}
+                """,
+            )
+            # strip new line and spaces from the message
+            message = " ".join(message[0].split())
+            return (True, message)
+        return False, ""
+
     def check_provided_column_with_input_columns(
         self,
         provided_columns: list,
         input_columns: list,
         missing_columns=[],
     ) -> list:
         for column in provided_columns:
@@ -45,14 +67,71 @@
             if column not in input_columns:
                 missing_columns.append(column)
         return missing_columns
 
     def generate_random_string(self):
         return "".join(random.choices(string.ascii_uppercase + string.digits, k=10))
 
+    def fetch_categorical_features(self, input: dict) -> Tuple[bool, list, dict]:
+        categorical_features_map = {}
+        error_list = []
+        for column in input:
+            if "categorical" in column and column["categorical"]:
+                if "category_map" not in column:
+                    error_list.append(
+                        f"  ValidationError: <category_map> key not found for <column>='{column['name']}'"
+                    )
+                    break
+                if not isinstance(column["category_map"], dict):
+                    error_list.append(
+                        f"  ValidationError: <category_map> for <column>='{column['name']}' is not a dictionary"
+                    )
+                    break
+                if len(column["category_map"]) == 0:
+                    error_list.append(
+                        f"  ValidationError: <category_map> for <column>='{column['name']}' is empty"
+                    )
+                    break
+                categorical_features_map[column["name"]] = column["category_map"]
+        return len(error_list) > 0, error_list, categorical_features_map
+
+    def validate_categorical_feature_from_input(
+        self, input: pd.DataFrame, categorical_features_map: dict
+    ) -> Tuple[bool, list]:
+        error_list = []
+        for column in categorical_features_map:
+            if column not in input.columns:
+                error_list.append(
+                    f"  ValidationError: <column>='{column}' not found in <input> dataframe"
+                )
+                break
+            if input[column].isnull().any():
+                error_list.append(
+                    f"  ValidationError: <column>='{column}' has null values, <column> must be NOT NULL"
+                )
+                break
+            if len(input[column].unique()) != len(categorical_features_map[column]):
+                len_input_unique_values = len(input[column].unique())
+                len_category_map_unique_values = len(categorical_features_map[column])
+
+                error_list.append(
+                    f"ValidationError: <column>='{column}' has unique values not equal to <category_map> ie: {len_input_unique_values} != {len_category_map_unique_values}"
+                )
+                break
+            if not set(input[column].unique()).issubset(
+                set(categorical_features_map[column].keys())
+            ):
+                input_unique_values = set(input[column].unique())
+                category_map_unique_values = set(categorical_features_map[column].keys())
+                error_list.append(
+                    f"ValidationError: <column>='{column}' has unique values not equal to <category_map> ie: {input_unique_values} != {category_map_unique_values}"
+                )
+                break
+        return len(error_list) > 0, error_list
+
 
 class BulkLogsValidation(DataSetValidation):
     def __init__(self):
         self.datatype_mapper = {
             "int64": "integer",
             "float64": "decimal",
             "object": "text",
@@ -74,15 +153,14 @@
                 f"  ValidationError: <prediction_column>='{prediction_column}' has null values, <prediction_column> must be NOT NULL",
             )
         return False, ""
 
     def prediction_confidence_column_checks(
         self, prediction_confidence_column: str, input: pd.DataFrame
     ) -> Tuple[bool, str]:
-
         if prediction_confidence_column not in input.columns:
             return (
                 True,
                 f"  ValidationError: <prediction_confidence_column>='{prediction_confidence_column}' not found in <input>",
             )
 
         # if prediction_confidence_column has null return error
@@ -186,15 +264,15 @@
         registered_model_target: list,
         registered_to_provided: dict = None,
     ) -> list:
         """
         This function will check if the registered datatype with the input dataframe is same or not.
         """
         datatype_error_list = []
-        for (feature_name, feature_dt) in registered_dataset.items():
+        for feature_name, feature_dt in registered_dataset.items():
             if feature_name.lower() in registered_model_target:
                 continue
             if registered_to_provided is not None:
                 """
                 if Prediction.Tabular is used then registered_to_provided will be mapped to provided_columns
                 """
                 feature_name = registered_to_provided[feature_name]
@@ -406,15 +484,14 @@
             return response
         else:
             return response
 
     def process_bulk(
         self, input_dataframe: pd.DataFrame, headers: dict, model_details: dict
     ) -> dict:
-
         pool = ThreadPool(processes=1)
         background_worker_thread = pool.apply_async(
             self._dataframe_chunks,
             (
                 input_dataframe,
                 headers,
                 model_details,
@@ -455,15 +532,14 @@
         # delete input_dataframe
         del input_dataframe
         return restructure_dataframe
 
     def process_bulk_explain(
         self, input_dataframe: pd.DataFrame, headers: dict, model_details: dict
     ) -> dict:
-
         # restructure input_dataframe
         input_dataframe = self._restructure_bulk_explain_df(input_dataframe)
         pool = ThreadPool(processes=1)
         background_worker_thread = pool.apply_async(
             self._dataframe_chunks,
             (
                 input_dataframe,
```

### Comparing `censius-1.6.8/src/censius.egg-info/PKG-INFO` & `censius-1.6.9/src/censius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censius
-Version: 1.6.8
+Version: 1.6.9
 Summary: API for Censius
 Home-page: https://github.com/Censius/censius-logs-python-sdk
 Author: Censius
 Author-email: dev@censius.ai
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `censius-1.6.8/src/censius.egg-info/SOURCES.txt` & `censius-1.6.9/src/censius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

