# Comparing `tmp/aporia-2.9.0.tar.gz` & `tmp/aporia-3.0.0a18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporia-2.9.0.tar", max compression
+gzip compressed data, was "aporia-3.0.0a18.tar", max compression
```

## Comparing `aporia-2.9.0.tar` & `aporia-3.0.0a18.tar`

### file list

```diff
@@ -1,62 +1,27 @@
--rw-r--r--   0        0        0      273 2022-09-01 10:19:27.334202 aporia-2.9.0/README.md
--rw-r--r--   0        0        0     1965 2022-09-01 10:19:27.334202 aporia-2.9.0/pyproject.toml
--rw-r--r--   0        0        0     1051 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/__init__.py
--rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/__init__.py
--rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/api/__init__.py
--rw-r--r--   0        0        0     4390 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/api/create_model_version.py
--rw-r--r--   0        0        0     2778 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/base_model.py
--rw-r--r--   0        0        0     3427 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/config.py
--rw-r--r--   0        0        0       24 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/consts.py
--rw-r--r--   0        0        0     1647 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/context.py
--rw-r--r--   0        0        0    11915 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/core_api.py
--rw-r--r--   0        0        0     2407 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/errors.py
--rw-r--r--   0        0        0     1612 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/event_loop.py
--rw-r--r--   0        0        0    10615 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/http_client.py
--rw-r--r--   0        0        0      666 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/logging_utils.py
--rw-r--r--   0        0        0     1713 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/model_tags.py
--rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/types/__init__.py
--rw-r--r--   0        0        0     8849 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/types/data_source.py
--rw-r--r--   0        0        0     1038 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/types/field.py
--rw-r--r--   0        0        0      765 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/types/model.py
--rw-r--r--   0        0        0     1152 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/core/utils.py
--rw-r--r--   0        0        0      350 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/experimental/__init__.py
--rw-r--r--   0        0        0     5119 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/experimental/model_versions_api.py
--rw-r--r--   0        0        0     3307 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/experimental/monitor_api.py
--rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/__init__.py
--rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/api/__init__.py
--rw-r--r--   0        0        0     2688 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/api/dataset.py
--rw-r--r--   0        0        0     7806 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/api/inference_fragment.py
--rw-r--r--   0        0        0     1669 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/api/log_inference.py
--rw-r--r--   0        0        0     1227 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/api/log_json.py
--rw-r--r--   0        0        0     2389 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/api/log_model_properties.py
--rw-r--r--   0        0        0    20593 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/inference_model.py
--rw-r--r--   0        0        0     4175 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/inference_queue.py
--rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/types/__init__.py
--rw-r--r--   0        0        0      120 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/inference/types/model_artifact.py
--rw-r--r--   0        0        0    19047 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/model.py
--rw-r--r--   0        0        0      179 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pandas/__init__.py
--rw-r--r--   0        0        0     8860 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pandas/pandas_utils.py
--rw-r--r--   0        0        0        0 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/py.typed
--rw-r--r--   0        0        0      279 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/__init__.py
--rw-r--r--   0        0        0       87 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/experimental/__init__.py
--rw-r--r--   0        0        0    10749 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/experimental/batch_api.py
--rw-r--r--   0        0        0     7193 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/pyspark_inference_model.py
--rw-r--r--   0        0        0     6689 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/pyspark_training.py
--rw-r--r--   0        0        0     4885 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/pyspark_training_model.py
--rw-r--r--   0        0        0     4688 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/pyspark_training_validator.py
--rw-r--r--   0        0        0     4388 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/pyspark_utils.py
--rw-r--r--   0        0        0      270 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/training/__init__.py
--rw-r--r--   0        0        0     3170 2022-09-01 10:19:27.334202 aporia-2.9.0/src/aporia/pyspark/training/pyspark_aggregation_alias.py
--rw-r--r--   0        0        0    11205 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/pyspark/training/pyspark_calculate_fields.py
--rw-r--r--   0        0        0     1354 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/pyspark/training/pyspark_create_fields.py
--rw-r--r--   0        0        0     1139 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/pyspark/training/pyspark_field_metadata.py
--rw-r--r--   0        0        0     1654 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/pyspark/training/utils.py
--rw-r--r--   0        0        0       71 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/__init__.py
--rw-r--r--   0        0        0        0 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/api/__init__.py
--rw-r--r--   0        0        0     1781 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/api/get_model_version.py
--rw-r--r--   0        0        0     7592 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/api/log_training.py
--rw-r--r--   0        0        0     5814 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/training.py
--rw-r--r--   0        0        0    10045 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/training_model.py
--rw-r--r--   0        0        0     7414 2022-09-01 10:19:27.338202 aporia-2.9.0/src/aporia/training/training_validator.py
--rw-r--r--   0        0        0     2184 1970-01-01 00:00:00.000000 aporia-2.9.0/setup.py
--rw-r--r--   0        0        0     1588 1970-01-01 00:00:00.000000 aporia-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2968 2023-05-22 00:50:02.478388 aporia-3.0.0a18/README.md
+-rw-r--r--   0        0        0      833 2023-05-22 00:50:02.478388 aporia-3.0.0a18/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/__init__.py
+-rw-r--r--   0        0        0      540 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/__init__.py
+-rw-r--r--   0        0        0      926 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/base.py
+-rw-r--r--   0        0        0     1410 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/custom_metrics.py
+-rw-r--r--   0        0        0     1945 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/data_source.py
+-rw-r--r--   0        0        0     7124 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/dataset.py
+-rw-r--r--   0        0        0     3779 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/model.py
+-rw-r--r--   0        0        0     1344 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/monitor.py
+-rw-r--r--   0        0        0     1721 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/segment.py
+-rw-r--r--   0        0        0     1885 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/version.py
+-rw-r--r--   0        0        0    12757 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/stack.py
+-rw-r--r--   0        0        0        0 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/__init__.py
+-rw-r--r--   0        0        0     2928 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/aporia_api.py
+-rw-r--r--   0        0        0      699 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/base.py
+-rw-r--r--   0        0        0     1480 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/client.py
+-rw-r--r--   0        0        0     2071 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/custom_metrics.py
+-rw-r--r--   0        0        0     1810 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/dashboards.py
+-rw-r--r--   0        0        0     3530 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/data_sources.py
+-rw-r--r--   0        0        0     6479 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/datasets.py
+-rw-r--r--   0        0        0     6077 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/metrics.py
+-rw-r--r--   0        0        0     5549 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/models.py
+-rw-r--r--   0        0        0    18647 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/monitors.py
+-rw-r--r--   0        0        0     2840 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/segments.py
+-rw-r--r--   0        0        0     2872 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/versions.py
+-rw-r--r--   0        0        0     3378 1970-01-01 00:00:00.000000 aporia-3.0.0a18/PKG-INFO
```

