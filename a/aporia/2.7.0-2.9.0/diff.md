# Comparing `tmp/aporia-2.7.0.tar.gz` & `tmp/aporia-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporia-2.7.0.tar", max compression
+gzip compressed data, was "aporia-2.9.0.tar", max compression
```

## Comparing `aporia-2.7.0.tar` & `aporia-2.9.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0      273 2022-08-30 10:46:21.472373 aporia-2.7.0/README.md
--rw-r--r--   0        0        0     1965 2022-08-30 10:46:21.476373 aporia-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     1051 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/__init__.py
--rw-r--r--   0        0        0        0 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/__init__.py
--rw-r--r--   0        0        0        0 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/api/__init__.py
--rw-r--r--   0        0        0     2727 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/api/create_model_version.py
--rw-r--r--   0        0        0     2778 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/base_model.py
--rw-r--r--   0        0        0     3427 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/config.py
--rw-r--r--   0        0        0       24 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/consts.py
--rw-r--r--   0        0        0     1647 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/context.py
--rw-r--r--   0        0        0    11807 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/core_api.py
--rw-r--r--   0        0        0     2407 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/errors.py
--rw-r--r--   0        0        0     1612 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/event_loop.py
--rw-r--r--   0        0        0    10615 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/http_client.py
--rw-r--r--   0        0        0      666 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/logging_utils.py
--rw-r--r--   0        0        0     1713 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/model_tags.py
--rw-r--r--   0        0        0        0 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/types/__init__.py
--rw-r--r--   0        0        0     8849 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/types/data_source.py
--rw-r--r--   0        0        0      955 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/types/field.py
--rw-r--r--   0        0        0      765 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/types/model.py
--rw-r--r--   0        0        0     1152 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/core/utils.py
--rw-r--r--   0        0        0      350 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/experimental/__init__.py
--rw-r--r--   0        0        0     5119 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/experimental/model_versions_api.py
--rw-r--r--   0        0        0     3307 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/experimental/monitor_api.py
--rw-r--r--   0        0        0        0 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/inference/__init__.py
--rw-r--r--   0        0        0        0 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/inference/api/__init__.py
--rw-r--r--   0        0        0     2688 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/inference/api/dataset.py
--rw-r--r--   0        0        0     7806 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/inference/api/inference_fragment.py
--rw-r--r--   0        0        0     1669 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/inference/api/log_inference.py
--rw-r--r--   0        0        0     1227 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/inference/api/log_json.py
--rw-r--r--   0        0        0     2389 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/inference/api/log_model_properties.py
--rw-r--r--   0        0        0    19403 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/inference/inference_model.py
--rw-r--r--   0        0        0     4175 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/inference/inference_queue.py
--rw-r--r--   0        0        0        0 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/inference/types/__init__.py
--rw-r--r--   0        0        0      120 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/inference/types/model_artifact.py
--rw-r--r--   0        0        0    19047 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/model.py
--rw-r--r--   0        0        0      179 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pandas/__init__.py
--rw-r--r--   0        0        0     8210 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pandas/pandas_utils.py
--rw-r--r--   0        0        0        0 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/py.typed
--rw-r--r--   0        0        0      279 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/__init__.py
--rw-r--r--   0        0        0       87 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/experimental/__init__.py
--rw-r--r--   0        0        0    10749 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/experimental/batch_api.py
--rw-r--r--   0        0        0     7193 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/pyspark_inference_model.py
--rw-r--r--   0        0        0     6618 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/pyspark_training.py
--rw-r--r--   0        0        0     4885 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/pyspark_training_model.py
--rw-r--r--   0        0        0     4688 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/pyspark_training_validator.py
--rw-r--r--   0        0        0     4388 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/pyspark_utils.py
--rw-r--r--   0        0        0      270 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/training/__init__.py
--rw-r--r--   0        0        0     3170 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/training/pyspark_aggregation_alias.py
--rw-r--r--   0        0        0    11187 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/training/pyspark_calculate_fields.py
--rw-r--r--   0        0        0     1354 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/training/pyspark_create_fields.py
--rw-r--r--   0        0        0     1139 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/training/pyspark_field_metadata.py
--rw-r--r--   0        0        0     1654 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/pyspark/training/utils.py
--rw-r--r--   0        0        0       71 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/training/__init__.py
--rw-r--r--   0        0        0        0 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/training/api/__init__.py
--rw-r--r--   0        0        0     1781 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/training/api/get_model_version.py
--rw-r--r--   0        0        0     7592 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/training/api/log_training.py
--rw-r--r--   0        0        0     5796 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/training/training.py
--rw-r--r--   0        0        0    10045 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/training/training_model.py
--rw-r--r--   0        0        0     7256 2022-08-30 10:46:21.476373 aporia-2.7.0/src/aporia/training/training_validator.py
--rw-r--r--   0        0        0     2176 2022-08-30 10:46:29.587254 aporia-2.7.0/setup.py
--rw-r--r--   0        0        0     1588 2022-08-30 10:46:29.587622 aporia-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0      273 2022-09-01 10:19:27.334202 aporia-2.9.0/README.md
+-rw-r--r--   0        0        0     1965 2022-09-01 10:19:27.334202 aporia-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1051 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/api/__init__.py
+-rw-r--r--   0        0        0     4390 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/api/create_model_version.py
+-rw-r--r--   0        0        0     2778 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/base_model.py
+-rw-r--r--   0        0        0     3427 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/config.py
+-rw-r--r--   0        0        0       24 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/consts.py
+-rw-r--r--   0        0        0     1647 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/context.py
+-rw-r--r--   0        0        0    11915 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/core_api.py
+-rw-r--r--   0        0        0     2407 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/errors.py
+-rw-r--r--   0        0        0     1612 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/event_loop.py
+-rw-r--r--   0        0        0    10615 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/http_client.py
+-rw-r--r--   0        0        0      666 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/logging_utils.py
+-rw-r--r--   0        0        0     1713 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/model_tags.py
+-rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/types/__init__.py
+-rw-r--r--   0        0        0     8849 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/types/data_source.py
+-rw-r--r--   0        0        0     1038 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/types/field.py
+-rw-r--r--   0        0        0      765 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/types/model.py
+-rw-r--r--   0        0        0     1152 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/utils.py
+-rw-r--r--   0        0        0      350 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/experimental/__init__.py
+-rw-r--r--   0        0        0     5119 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/experimental/model_versions_api.py
+-rw-r--r--   0        0        0     3307 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/experimental/monitor_api.py
+-rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/api/__init__.py
+-rw-r--r--   0        0        0     2688 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/api/dataset.py
+-rw-r--r--   0        0        0     7806 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/api/inference_fragment.py
+-rw-r--r--   0        0        0     1669 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/api/log_inference.py
+-rw-r--r--   0        0        0     1227 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/api/log_json.py
+-rw-r--r--   0        0        0     2389 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/api/log_model_properties.py
+-rw-r--r--   0        0        0    20593 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/inference_model.py
+-rw-r--r--   0        0        0     4175 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/inference_queue.py
+-rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/types/__init__.py
+-rw-r--r--   0        0        0      120 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/types/model_artifact.py
+-rw-r--r--   0        0        0    19047 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/model.py
+-rw-r--r--   0        0        0      179 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pandas/__init__.py
+-rw-r--r--   0        0        0     8860 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pandas/pandas_utils.py
+-rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/py.typed
+-rw-r--r--   0        0        0      279 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/__init__.py
+-rw-r--r--   0        0        0       87 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/experimental/__init__.py
+-rw-r--r--   0        0        0    10749 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/experimental/batch_api.py
+-rw-r--r--   0        0        0     7193 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/pyspark_inference_model.py
+-rw-r--r--   0        0        0     6689 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/pyspark_training.py
+-rw-r--r--   0        0        0     4885 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/pyspark_training_model.py
+-rw-r--r--   0        0        0     4688 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/pyspark_training_validator.py
+-rw-r--r--   0        0        0     4388 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/pyspark_utils.py
+-rw-r--r--   0        0        0      270 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/training/__init__.py
+-rw-r--r--   0        0        0     3170 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/training/pyspark_aggregation_alias.py
+-rw-r--r--   0        0        0    11205 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/pyspark/training/pyspark_calculate_fields.py
+-rw-r--r--   0        0        0     1354 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/pyspark/training/pyspark_create_fields.py
+-rw-r--r--   0        0        0     1139 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/pyspark/training/pyspark_field_metadata.py
+-rw-r--r--   0        0        0     1654 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/pyspark/training/utils.py
+-rw-r--r--   0        0        0       71 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/api/__init__.py
+-rw-r--r--   0        0        0     1781 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/api/get_model_version.py
+-rw-r--r--   0        0        0     7592 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/api/log_training.py
+-rw-r--r--   0        0        0     5814 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/training.py
+-rw-r--r--   0        0        0    10045 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/training_model.py
+-rw-r--r--   0        0        0     7414 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/training_validator.py
+-rw-r--r--   0        0        0     2184 1970-01-01 00:00:00.000000 aporia-2.9.0/setup.py
+-rw-r--r--   0        0        0     1588 1970-01-01 00:00:00.000000 aporia-2.9.0/PKG-INFO
```

### Comparing `aporia-2.7.0/pyproject.toml` & `aporia-2.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aporia"
-version = "v2.7.0"
+version = "v2.9.0"
 description = "Aporia SDK"
 authors = []
 readme = "README.md"
 repository = "https://github.com/aporia-ai/sdk"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `aporia-2.7.0/src/aporia/__init__.py` & `aporia-2.9.0/src/aporia/__init__.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/core/base_model.py` & `aporia-2.9.0/src/aporia/core/base_model.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/core/config.py` & `aporia-2.9.0/src/aporia/core/config.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/core/context.py` & `aporia-2.9.0/src/aporia/core/context.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/core/core_api.py` & `aporia-2.9.0/src/aporia/core/core_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from contextlib import suppress
 from functools import wraps
 from http import HTTPStatus
 import logging
 from typing import Any, Callable, Dict, List, Optional, Union
 import warnings
 
+from aporia.core.types.field import FieldSchema
 from aporia.model import Model
 from .api.create_model_version import run_create_model_version_query
 from .config import Config
 from .context import get_context, init_context, reset_context
 from .errors import AporiaError, AporiaHTTPError, handle_error
 from .event_loop import EventLoop
 from .http_client import HttpClient
@@ -210,17 +211,17 @@
 
 
 @safe_api_function("Creating model version failed, error: {}")
 def create_model_version(
     model_id: str,
     model_version: str,
     model_type: str,
-    features: Dict[str, str],
-    predictions: Dict[str, str],
-    raw_inputs: Optional[Dict[str, str]] = None,
+    features: Dict[str, Union[str, FieldSchema]],
+    predictions: Dict[str, Union[str, FieldSchema]],
+    raw_inputs: Optional[Dict[str, Union[str, FieldSchema]]] = None,
     metrics: Optional[Dict[str, str]] = None,
     model_data_type: Optional[str] = None,
     labels: Optional[List[str]] = None,
     multiclass_labels: Optional[List[str]] = None,
     feature_importance: Optional[Dict[str, float]] = None,
     mapping: Optional[Dict[str, str]] = None,
 ) -> Optional[Model]:
```

### Comparing `aporia-2.7.0/src/aporia/core/errors.py` & `aporia-2.9.0/src/aporia/core/errors.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/core/event_loop.py` & `aporia-2.9.0/src/aporia/core/event_loop.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/core/http_client.py` & `aporia-2.9.0/src/aporia/core/http_client.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/core/logging_utils.py` & `aporia-2.9.0/src/aporia/core/logging_utils.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/core/model_tags.py` & `aporia-2.9.0/src/aporia/core/model_tags.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/core/types/data_source.py` & `aporia-2.9.0/src/aporia/core/types/data_source.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/core/types/field.py` & `aporia-2.9.0/src/aporia/core/types/field.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from datetime import datetime
 from enum import Enum
-from typing import Union
+from typing import Any, Dict, List, Union
 
-FieldValue = Union[float, int, str, bool, datetime]
+FieldValue = Union[float, int, str, bool, datetime, List[int]]
+
+FieldSchema = Dict[str, Any]
 
 
 class FieldType(Enum):
     """Field types."""
 
     NUMERIC = "numeric"
     CATEGORICAL = "categorical"
     STRING = "string"
     BOOLEAN = "boolean"
     DATETIME = "datetime"
     VECTOR = "vector"
     TEXT = "text"
     DICT = "dict"
+    TENSOR = "tensor"
 
 
 class FieldCategory(Enum):
     """Field categories."""
 
     FEATURES = "features"
     PREDICTIONS = "predictions"
```

### Comparing `aporia-2.7.0/src/aporia/core/types/model.py` & `aporia-2.9.0/src/aporia/core/types/model.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/core/utils.py` & `aporia-2.9.0/src/aporia/core/utils.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/experimental/model_versions_api.py` & `aporia-2.9.0/src/aporia/experimental/model_versions_api.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/experimental/monitor_api.py` & `aporia-2.9.0/src/aporia/experimental/monitor_api.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/inference/api/dataset.py` & `aporia-2.9.0/src/aporia/inference/api/dataset.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/inference/api/inference_fragment.py` & `aporia-2.9.0/src/aporia/inference/api/inference_fragment.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/inference/api/log_inference.py` & `aporia-2.9.0/src/aporia/inference/api/log_inference.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/inference/api/log_json.py` & `aporia-2.9.0/src/aporia/inference/api/log_json.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/inference/api/log_model_properties.py` & `aporia-2.9.0/src/aporia/inference/api/log_model_properties.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/inference/inference_model.py` & `aporia-2.9.0/src/aporia/inference/inference_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -368,14 +368,45 @@
                     predictions=predictions,
                     labels=labels,
                     raw_inputs=raw_inputs,
                 )
             )
 
     @validate_model_ready
+    def connect_actuals(
+        self,
+        data_source: DataSource,
+        id_column: str,
+        timestamp_column: str,
+        labels: Optional[Dict[str, str]] = None,
+    ):
+        """Connect to external actual data set.
+
+        Args:
+            data_source: The data source to fetch the data set from.
+            id_column: The name of the id column.
+            timestamp_column: The name of a column contains the times actual was updated.
+            labels: Mapping from the predictions name to column holding the actual value.
+        """
+        with self.handle_error("Connection to actuals failed, error: {}"):
+            self._event_loop.run_coroutine(
+                connect_dataset(
+                    http_client=self._http_client,
+                    model_id=self.model_id,
+                    model_version=self.model_version,
+                    environment=self._config.environment,
+                    dataset="actuals",
+                    data_source=data_source,
+                    id_column=id_column,
+                    timestamp_column=timestamp_column,
+                    labels=labels,
+                )
+            )
+
+    @validate_model_ready
     def connect_training(
         self,
         data_source: DataSource,
         id_column: str,
         timestamp_column: str,
         predictions: Optional[Dict[str, str]] = None,
         features: Optional[Dict[str, str]] = None,
```

### Comparing `aporia-2.7.0/src/aporia/inference/inference_queue.py` & `aporia-2.9.0/src/aporia/inference/inference_queue.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/model.py` & `aporia-2.9.0/src/aporia/model.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/pandas/pandas_utils.py` & `aporia-2.9.0/src/aporia/pandas/pandas_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 from collections import abc, OrderedDict
-from typing import Dict, Iterable, Optional, Union
+from typing import Any, Dict, Iterable, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from aporia.core.context import get_context
 from aporia.core.errors import AporiaError, handle_error
-from aporia.core.types.field import FieldType, FieldValue
+from aporia.core.types.field import FieldSchema, FieldType, FieldValue
+
+
+def _dtype_to_field_type(dtype: str) -> Optional[FieldSchema]:
+    # This is based on https://numpy.org/doc/stable/reference/generated/numpy.dtype.kind.html#numpy.dtype.kind
+    DTYPE_TO_FIELD_TYPE = {
+        "b": FieldType.BOOLEAN,
+        "i": FieldType.NUMERIC,
+        "u": FieldType.NUMERIC,
+        "f": FieldType.NUMERIC,
+        "M": FieldType.DATETIME,
+        "O": FieldType.STRING,
+        "S": FieldType.STRING,
+        "U": FieldType.STRING,
+    }
+    field_type = DTYPE_TO_FIELD_TYPE.get(dtype)
+    if field_type is None:
+        return None
+    return {"type": field_type.value}
 
-# This is based on https://numpy.org/doc/stable/reference/generated/numpy.dtype.kind.html#numpy.dtype.kind
-DTYPE_TO_FIELD_TYPE = {
-    "b": FieldType.BOOLEAN,
-    "i": FieldType.NUMERIC,
-    "u": FieldType.NUMERIC,
-    "f": FieldType.NUMERIC,
-    "M": FieldType.DATETIME,
-    "O": FieldType.STRING,
-    "S": FieldType.STRING,
-    "U": FieldType.STRING,
-}
 
 NUMERIC_DTYPES = ["i", "u", "f"]
 STRING_DTYPES = ["O", "S", "U"]
 STRING_UNIQUE_RATIO = 0.25
 MIN_UNIQUE_VALUES_FOR_TEXT = 50
 
 
-def _infer_string_data_for_text_or_string(data: pd.Series) -> FieldType:
+def _infer_string_data_for_text_or_string(data: pd.Series) -> FieldSchema:
     """Convert a numpy/pandas of series contains only strings to a FieldType.
 
     Args:
         data: pandas data series
 
     Returns:
         FieldType that matches the dtype
     """
     # We need to decided if a string type is str or text
     # We check if there are more than 50 unique values
     # which are more than 25% of the total values
     _, unique_counts = np.unique(data.values, return_counts=True)
     uniques = len(unique_counts)
     if uniques > MIN_UNIQUE_VALUES_FOR_TEXT and uniques > data.shape[0] * STRING_UNIQUE_RATIO:
-        return FieldType.TEXT
+        return {"type": FieldType.TEXT.value}
 
-    return FieldType.STRING
+    return {"type": FieldType.STRING.value}
 
 
 def _replace_na_type(data: pd.Series) -> pd.Series:
     """Replace NAType with NA (since they are not removed by dropna).
 
     Args:
         data: pandas data series
@@ -60,67 +67,72 @@
         result = data.copy()
         for i, value in result.iteritems():
             if value == pd._libs.missing.NAType:
                 result.at[i] = pd.NA
     return result
 
 
-def _infer_object_dtype_column(data: pd.Series) -> Optional[FieldType]:
+def _infer_object_dtype_column(data: pd.Series) -> Optional[FieldSchema]:
     """Attempts to convert a numpy/pandas series of object dtype to a FieldType.
 
     Args:
         data: pandas data series
 
     Returns:
         FieldType that matches the dtype, or None if conversion is impossible
     """
     if data.size == 0:
         return None
     elif data.apply(lambda x: isinstance(x, dict)).all():
-        return FieldType.DICT
+        return {"type": FieldType.DICT.value}
     elif data.apply(lambda x: isinstance(x, str)).all():
         return _infer_string_data_for_text_or_string(data=data)
-
+    elif data.apply(lambda x: isinstance(x, abc.Iterable)).all():
+        return {"type": FieldType.TENSOR.value, "dimensions": [len(data.values[0])]}
     return None
 
 
-def infer_type_from_dtype_and_data(
+def infer_field_schema_from_dtype_and_data(
     dtype: np.dtype, data: Optional[pd.Series]
-) -> Optional[FieldType]:
+) -> Optional[FieldSchema]:
     """Attempts to convert a numpy/pandas dtype to a FieldType.
 
     Args:
         dtype: Dtype to convert
         data: pandas data series
 
     Returns:
         FieldType that matches the dtype, or None if conversion is impossible
     """
     if isinstance(dtype, pd.api.types.CategoricalDtype):
-        category_type = DTYPE_TO_FIELD_TYPE.get(dtype.categories.dtype.kind)
+        category_type = _dtype_to_field_type(dtype.categories.dtype.kind)
         # We only support categorical fields with numeric categories
-        if category_type == FieldType.NUMERIC:
-            return FieldType.CATEGORICAL
+        if category_type is None:
+            return None
+        if category_type["type"] == FieldType.NUMERIC.value:
+            return {"type": FieldType.CATEGORICAL.value}
 
         return category_type
 
     if dtype.kind == "O":
         return _infer_object_dtype_column(data=data)
 
     if data is not None and not data.empty:
         if dtype.kind in NUMERIC_DTYPES and isinstance(data.values[0], abc.Iterable):
-            return FieldType.VECTOR
+            arr: Any = data.values[0]
+            return {"type": FieldType.TENSOR.value, "dimensions": [len(arr)]}
 
         # We need to decided if a string type is str or text
         # We check if there are more than 50 unique values
         # which are more than 25% of the total values
         if dtype.kind in STRING_DTYPES and len(data.shape) > 0:
+
             return _infer_string_data_for_text_or_string(data=data)
 
-    return DTYPE_TO_FIELD_TYPE.get(dtype.kind)  # type: ignore
+    return _dtype_to_field_type(dtype.kind)  # type: ignore
 
 
 def pandas_to_dict(data: Union[pd.DataFrame, pd.Series]) -> Optional[Dict[str, FieldValue]]:
     """Converts a pandas DataFrame or Series to a dict for log_* functions.
 
     Args:
         data: DataFrame or Series to convert.
@@ -155,15 +167,15 @@
             debug=False if context is None else context.config.debug,
             original_exception=err,
         )
 
     return None
 
 
-def infer_schema_from_dataframe(data: pd.DataFrame) -> Optional[Dict[str, str]]:
+def infer_schema_from_dataframe(data: pd.DataFrame) -> Optional[Dict[str, Dict]]:
     """Infers model version schema from a pandas DataFrame or Series.
 
     Field names and types are inferred from column names and types.
 
     Args:
         data: pandas DataFrame or Series
 
@@ -191,21 +203,21 @@
     not_inferable_columns = []
     for column_name, values in data.items():
         column_name = str(column_name)
 
         values_without_nulls = _replace_na_type(values)
         values_without_nulls = values_without_nulls.dropna().infer_objects()
 
-        column_type = infer_type_from_dtype_and_data(
+        column_type = infer_field_schema_from_dtype_and_data(
             values_without_nulls.dtype, values_without_nulls
         )
         if column_type is None:
             not_inferable_columns.append(column_name)
         else:
-            schema[column_name] = column_type.value
+            schema[column_name] = column_type
 
     if len(not_inferable_columns) > 0:
         raise AporiaError(
             f"Could not infer the type of columns {not_inferable_columns}. "
             "To fix, make sure to set column dtype. For example "
             f"df['{not_inferable_columns[0]}'] = df['{not_inferable_columns[0]}'].astype(np.int32)"
         )
```

### Comparing `aporia-2.7.0/src/aporia/pyspark/experimental/batch_api.py` & `aporia-2.9.0/src/aporia/pyspark/experimental/batch_api.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/pyspark/pyspark_inference_model.py` & `aporia-2.9.0/src/aporia/pyspark/pyspark_inference_model.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/pyspark/pyspark_training.py` & `aporia-2.9.0/src/aporia/pyspark/pyspark_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,21 @@
         field_data: Field data
         field_type: Field type
 
     Returns:
         Field training data.
     """
     # We currently don't support datetime, vector, text and dict training data
-    if field_type in [FieldType.DATETIME, FieldType.VECTOR, FieldType.TEXT, FieldType.DICT]:
+    if field_type in [
+        FieldType.DATETIME,
+        FieldType.VECTOR,
+        FieldType.TEXT,
+        FieldType.DICT,
+        FieldType.TENSOR,
+    ]:
         return _calculate_training_data_without_histogram(
             field_name=field_name, field_data=field_data
         )
     elif field_type == FieldType.NUMERIC:
         return _calculate_numeric_training_data(field_name=field_name, field_data=field_data)
     elif field_type in [FieldType.BOOLEAN, FieldType.STRING, FieldType.CATEGORICAL]:
         return _calculate_categorical_training_data(
```

### Comparing `aporia-2.7.0/src/aporia/pyspark/pyspark_training_model.py` & `aporia-2.9.0/src/aporia/pyspark/pyspark_training_model.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/pyspark/pyspark_training_validator.py` & `aporia-2.9.0/src/aporia/pyspark/pyspark_training_validator.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/pyspark/pyspark_utils.py` & `aporia-2.9.0/src/aporia/pyspark/pyspark_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             if isinstance(column.dataType, BooleanType):
                 field_type = FieldType.BOOLEAN
             elif isinstance(column.dataType, (TimestampType, DateType)):
                 field_type = FieldType.DATETIME
             elif isinstance(column.dataType, ArrayType) and isinstance(
                 column.dataType.elementType, NumericType
             ):
-                field_type = FieldType.VECTOR
+                field_type = FieldType.TENSOR
             elif isinstance(column.dataType, NumericType):
                 # See the heuristic described in the function notes
                 if (
                     total_count > 0
                     and unique_count < UNIQUE_VALUES_THRESHOLD
                     and unique_count < total_count * UNIQUE_RATIO
                 ):
```

### Comparing `aporia-2.7.0/src/aporia/pyspark/training/pyspark_aggregation_alias.py` & `aporia-2.9.0/src/aporia/pyspark/training/pyspark_aggregation_alias.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/pyspark/training/pyspark_calculate_fields.py` & `aporia-2.9.0/src/aporia/pyspark/training/pyspark_calculate_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         result: List[Column] = []
         for field in fields:
             result.extend(self._generate_column_aggregations(field))
         return result
 
     def _generate_column_aggregations(self, field: PySparkFieldMetadata) -> List[Column]:
         logger.debug("Generating aggregations for:" f"{field}")
-        if field.type in [FieldType.DATETIME, FieldType.VECTOR, FieldType.TEXT]:
+        if field.type in [FieldType.DATETIME, FieldType.VECTOR, FieldType.TEXT, FieldType.TENSOR]:
             return self._aggregate_any_column(field)
         elif field.type == FieldType.NUMERIC:
             return self._aggregate_numeric_column(field)
         elif field.type == FieldType.BOOLEAN:
             return self._aggregate_boolean_column(field)
         elif field.type in [FieldType.STRING, FieldType.CATEGORICAL]:
             return self._aggregate_categorical_column(field)
```

### Comparing `aporia-2.7.0/src/aporia/pyspark/training/pyspark_create_fields.py` & `aporia-2.9.0/src/aporia/pyspark/training/pyspark_create_fields.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/pyspark/training/pyspark_field_metadata.py` & `aporia-2.9.0/src/aporia/pyspark/training/pyspark_field_metadata.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/pyspark/training/utils.py` & `aporia-2.9.0/src/aporia/pyspark/training/utils.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/training/api/get_model_version.py` & `aporia-2.9.0/src/aporia/training/api/get_model_version.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/training/api/log_training.py` & `aporia-2.9.0/src/aporia/training/api/log_training.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/training/training.py` & `aporia-2.9.0/src/aporia/training/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         field_data: Field data
         field_type: Field type
 
     Returns:
         Field training data.
     """
     # We currently don't support datetime, vector, text & dict training data
-    if field_type in [FieldType.DATETIME, FieldType.VECTOR, FieldType.TEXT]:
+    if field_type in [FieldType.DATETIME, FieldType.VECTOR, FieldType.TEXT, FieldType.TENSOR]:
         return [
             _calculate_training_data_without_histogram(field_name=field_name, field_data=field_data)
         ]
     elif field_type == FieldType.NUMERIC:
         return [_calculate_numeric_training_data(field_name=field_name, field_data=field_data)]
     elif field_type == FieldType.DICT:
         return _calculate_dict_training_data(field_name=field_name, field_data=field_data)
```

### Comparing `aporia-2.7.0/src/aporia/training/training_model.py` & `aporia-2.9.0/src/aporia/training/training_model.py`

 * *Files identical despite different names*

### Comparing `aporia-2.7.0/src/aporia/training/training_validator.py` & `aporia-2.9.0/src/aporia/training/training_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from numpy import ndarray
 from pandas import DataFrame
 
 from aporia.core.errors import AporiaError
 from aporia.core.logging_utils import LOGGER_NAME
 from aporia.core.types.field import FieldCategory, FieldType
 from aporia.core.utils import generate_features_schema_from_shape
-from aporia.pandas.pandas_utils import infer_type_from_dtype_and_data
+from aporia.pandas.pandas_utils import infer_field_schema_from_dtype_and_data
 
 logger = logging.getLogger(LOGGER_NAME)
 
 
 class TrainingDataset(Enum):
     """Training dataset names."""
 
@@ -111,20 +111,23 @@
         missing_fields = self.schema[field_category].keys() - set(data.columns)
 
         for field_name, field_type in self.schema[field_category].items():
             if field_name in missing_fields:
                 continue
 
             column_data_without_nulls = data[field_name].dropna().infer_objects()
-            inferred_field_type = infer_type_from_dtype_and_data(
+            inferred_field_schema = infer_field_schema_from_dtype_and_data(
                 dtype=column_data_without_nulls.dtype, data=column_data_without_nulls  # type: ignore
             )
 
             # Don't verify boolean fields, since we're going to cast them anyway
-            if field_type != FieldType.BOOLEAN and field_type != inferred_field_type:
+            inferred_type = (
+                inferred_field_schema["type"] if inferred_field_schema is not None else None
+            )
+            if field_type != FieldType.BOOLEAN and field_type.value != inferred_type:
                 logger.warning(
                     "Detected type mismatch on field {field_name}: expected {expected_type} "
                     "type, got {actual_type}".format(
                         field_name=field_name,
                         expected_type=field_type.value,
                         actual_type=column_data_without_nulls.dtype,
                     )
```

### Comparing `aporia-2.7.0/setup.py` & `aporia-2.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,21 +40,21 @@
  'pandas:python_version >= "3.8" and python_version < "4.0"': ['pandas>=1.0,<2.0'],
  'pyspark': ['pyspark>=3.0,<4.0'],
  'training:python_version >= "3.7" and python_version < "3.8"': ['pandas>=1.0,<1.4'],
  'training:python_version >= "3.8" and python_version < "4.0"': ['pandas>=1.0,<2.0']}
 
 setup_kwargs = {
     'name': 'aporia',
-    'version': '2.7.0',
+    'version': '2.9.0',
     'description': 'Aporia SDK',
     'long_description': '# Aporia SDK\n\n## Testing\n\nTo run the tests, first install the library locally:\n```\npip install ".[all]" --upgrade\n```\n\nThen run the tests using `pytest`:\n```\npytest -v\n```\n\nIf you don\'t have Spark installed, skip the pyspark tests:\n```\npytest -v --ignore=tests/pyspark\n```\n',
-    'author': None,
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
+    'author': 'None',
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/aporia-ai/sdk',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.7,<4.0',
```

### Comparing `aporia-2.7.0/PKG-INFO` & `aporia-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: aporia
-Version: 2.7.0
+Version: 2.9.0
 Summary: Aporia SDK
 Home-page: https://github.com/aporia-ai/sdk
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: all
 Provides-Extra: pandas
 Provides-Extra: pyspark
 Provides-Extra: training
 Requires-Dist: aiohttp (>=3.8.0,<4.0.0)
 Requires-Dist: certifi (>=2022.6.15,<2023.0.0)
 Requires-Dist: importlib-metadata (>=1.5.0,<2.0.0); python_version < "3.8"
```

