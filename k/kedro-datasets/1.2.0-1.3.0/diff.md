# Comparing `tmp/kedro-datasets-1.2.0.tar.gz` & `tmp/kedro-datasets-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-datasets-1.2.0.tar", last modified: Fri Mar 24 16:08:35 2023, max compression
+gzip compressed data, was "kedro-datasets-1.3.0.tar", last modified: Mon May 22 20:35:33 2023, max compression
```

## Comparing `kedro-datasets-1.2.0.tar` & `kedro-datasets-1.3.0.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.723535 kedro-datasets-1.2.0/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     3797 2023-03-24 16:08:35.722811 kedro-datasets-1.2.0/PKG-INFO
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     1780 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/README.md
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.503850 kedro-datasets-1.2.0/features/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)        0 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/features/__init__.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.504286 kedro-datasets-1.2.0/kedro_datasets/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      102 2023-03-24 16:05:42.000000 kedro-datasets-1.2.0/kedro_datasets/__init__.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.521510 kedro-datasets-1.2.0/kedro_datasets/api/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      316 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/api/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     5033 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/api/api_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.529347 kedro-datasets-1.2.0/kedro_datasets/biosequence/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      232 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/biosequence/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     5343 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/biosequence/biosequence_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.535498 kedro-datasets-1.2.0/kedro_datasets/dask/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      189 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/dask/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     8105 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/dask/parquet_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.541418 kedro-datasets-1.2.0/kedro_datasets/email/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      221 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/email/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     7866 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/email/message_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.546918 kedro-datasets-1.2.0/kedro_datasets/geopandas/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      237 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/geopandas/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     6308 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/geopandas/geojson_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.552246 kedro-datasets-1.2.0/kedro_datasets/holoviews/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      226 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/holoviews/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     5010 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/holoviews/holoviews_writer.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.560079 kedro-datasets-1.2.0/kedro_datasets/json/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      211 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/json/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     5957 2023-03-24 15:23:18.000000 kedro-datasets-1.2.0/kedro_datasets/json/json_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.566756 kedro-datasets-1.2.0/kedro_datasets/matplotlib/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      230 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/matplotlib/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     8705 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/matplotlib/matplotlib_writer.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.584306 kedro-datasets-1.2.0/kedro_datasets/networkx/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      437 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/networkx/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     5737 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/networkx/gml_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     5770 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/networkx/graphml_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     5808 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/networkx/json_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.622375 kedro-datasets-1.2.0/kedro_datasets/pandas/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     1128 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/pandas/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     7433 2023-03-24 15:23:18.000000 kedro-datasets-1.2.0/kedro_datasets/pandas/csv_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)    10518 2023-03-24 15:23:18.000000 kedro-datasets-1.2.0/kedro_datasets/pandas/excel_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     7087 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/pandas/feather_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)    11580 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/pandas/gbq_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     9749 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/pandas/generic_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     7753 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/pandas/hdf_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     6980 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/pandas/json_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     8219 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/pandas/parquet_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)    20661 2023-03-24 15:23:18.000000 kedro-datasets-1.2.0/kedro_datasets/pandas/sql_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     6463 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/pandas/xml_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.628724 kedro-datasets-1.2.0/kedro_datasets/pickle/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      219 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/pickle/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)    10490 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/pickle/pickle_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.633688 kedro-datasets-1.2.0/kedro_datasets/pillow/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      200 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/pillow/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     5435 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/pillow/image_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.643999 kedro-datasets-1.2.0/kedro_datasets/plotly/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      314 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/plotly/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     6554 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/plotly/json_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     5901 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/plotly/plotly_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.650281 kedro-datasets-1.2.0/kedro_datasets/polars/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      202 2023-03-21 15:15:51.000000 kedro-datasets-1.2.0/kedro_datasets/polars/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     7154 2023-03-21 15:15:51.000000 kedro-datasets-1.2.0/kedro_datasets/polars/csv_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.654851 kedro-datasets-1.2.0/kedro_datasets/redis/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      215 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/redis/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     7808 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/redis/redis_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.659444 kedro-datasets-1.2.0/kedro_datasets/snowflake/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      195 2023-03-21 15:15:59.000000 kedro-datasets-1.2.0/kedro_datasets/snowflake/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     8528 2023-03-21 15:15:59.000000 kedro-datasets-1.2.0/kedro_datasets/snowflake/snowpark_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.676102 kedro-datasets-1.2.0/kedro_datasets/spark/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      484 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/spark/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     3733 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/spark/deltatable_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)    15918 2023-03-24 15:23:18.000000 kedro-datasets-1.2.0/kedro_datasets/spark/spark_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     8978 2023-03-24 15:23:18.000000 kedro-datasets-1.2.0/kedro_datasets/spark/spark_hive_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     6914 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/spark/spark_jdbc_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.683997 kedro-datasets-1.2.0/kedro_datasets/svmlight/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      246 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/svmlight/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     5918 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/svmlight/svmlight_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.691803 kedro-datasets-1.2.0/kedro_datasets/tensorflow/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      207 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/tensorflow/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     7377 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.700933 kedro-datasets-1.2.0/kedro_datasets/text/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      211 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/text/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     5114 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/text/text_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.709264 kedro-datasets-1.2.0/kedro_datasets/tracking/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      345 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/tracking/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     1491 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/tracking/json_dataset.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     2389 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/tracking/metrics_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.716611 kedro-datasets-1.2.0/kedro_datasets/video/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      138 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/video/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)    12160 2023-03-21 15:15:59.000000 kedro-datasets-1.2.0/kedro_datasets/video/video_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.721331 kedro-datasets-1.2.0/kedro_datasets/yaml/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)      211 2022-12-29 21:32:52.000000 kedro-datasets-1.2.0/kedro_datasets/yaml/__init__.py
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     5862 2023-02-07 12:53:06.000000 kedro-datasets-1.2.0/kedro_datasets/yaml/yaml_dataset.py
-drwxr-xr-x   0 jannic_holzer   (501) staff       (20)        0 2023-03-24 16:08:35.514619 kedro-datasets-1.2.0/kedro_datasets.egg-info/
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     3797 2023-03-24 16:08:35.000000 kedro-datasets-1.2.0/kedro_datasets.egg-info/PKG-INFO
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     2642 2023-03-24 16:08:35.000000 kedro-datasets-1.2.0/kedro_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 jannic_holzer   (501) staff       (20)        1 2023-03-24 16:08:35.000000 kedro-datasets-1.2.0/kedro_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     3665 2023-03-24 16:08:35.000000 kedro-datasets-1.2.0/kedro_datasets.egg-info/requires.txt
--rw-r--r--   0 jannic_holzer   (501) staff       (20)       24 2023-03-24 16:08:35.000000 kedro-datasets-1.2.0/kedro_datasets.egg-info/top_level.txt
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     1010 2023-03-21 15:15:59.000000 kedro-datasets-1.2.0/pyproject.toml
--rw-r--r--   0 jannic_holzer   (501) staff       (20)       38 2023-03-24 16:08:35.723615 kedro-datasets-1.2.0/setup.cfg
--rw-r--r--   0 jannic_holzer   (501) staff       (20)     5815 2023-03-21 15:15:59.000000 kedro-datasets-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/api/api_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/biosequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/biosequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/biosequence/biosequence_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/dask/parquet_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16973 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/databricks/managed_table_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/email/message_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/geopandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/geopandas/geojson_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/holoviews/holoviews_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/json/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/matplotlib/matplotlib_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets/networkx/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/networkx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/networkx/gml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/networkx/graphml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/networkx/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/feather_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/gbq_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/generic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/hdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/parquet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/sql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pandas/xml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pickle/pickle_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/pillow/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pillow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/pillow/image_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/plotly/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/plotly/plotly_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/polars/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/polars/csv_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/redis/redis_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/snowflake/snowpark_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/spark/deltatable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/spark/spark_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/spark/spark_hive_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/spark/spark_jdbc_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.052310 kedro-datasets-1.3.0/kedro_datasets/svmlight/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/svmlight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/svmlight/svmlight_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/kedro_datasets/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/kedro_datasets/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/text/text_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/kedro_datasets/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/tracking/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/tracking/metrics_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/kedro_datasets/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/video/video_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/kedro_datasets/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/kedro_datasets/yaml/yaml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:35:33.048310 kedro-datasets-1.3.0/kedro_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-22 20:35:33.000000 kedro-datasets-1.3.0/kedro_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-22 20:35:33.000000 kedro-datasets-1.3.0/kedro_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:35:33.000000 kedro-datasets-1.3.0/kedro_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-22 20:35:33.000000 kedro-datasets-1.3.0/kedro_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 20:35:33.000000 kedro-datasets-1.3.0/kedro_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:35:33.056311 kedro-datasets-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-22 20:35:21.000000 kedro-datasets-1.3.0/setup.py
```

### Comparing `kedro-datasets-1.2.0/PKG-INFO` & `kedro-datasets-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 1.2.0
+Version: 1.3.0
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
-Home-page: https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Author: Kedro
 License: Apache Software License (Apache 2.0)
-Requires-Python: >=3.7, <3.11
+Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
+Project-URL: Documentation, https://docs.kedro.org
+Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: api
 Provides-Extra: biosequence
 Provides-Extra: dask
+Provides-Extra: databricks
 Provides-Extra: docs
 Provides-Extra: geopandas
-Provides-Extra: matplotlib
 Provides-Extra: holoviews
+Provides-Extra: matplotlib
 Provides-Extra: networkx
 Provides-Extra: pandas
 Provides-Extra: pillow
-Provides-Extra: polars
-Provides-Extra: video
 Provides-Extra: plotly
+Provides-Extra: polars
 Provides-Extra: redis
+Provides-Extra: snowflake
 Provides-Extra: spark
 Provides-Extra: svmlight
 Provides-Extra: tensorflow
+Provides-Extra: video
 Provides-Extra: yaml
 Provides-Extra: api.APIDataSet
 Provides-Extra: biosequence.BioSequenceDataSet
 Provides-Extra: dask.ParquetDataSet
+Provides-Extra: databricks.ManagedTableDataSet
 Provides-Extra: geopandas.GeoJSONDataSet
-Provides-Extra: matplotlib.MatplotlibWriter
 Provides-Extra: holoviews.HoloviewsWriter
+Provides-Extra: matplotlib.MatplotlibWriter
 Provides-Extra: networkx.NetworkXDataSet
 Provides-Extra: pandas.CSVDataSet
 Provides-Extra: pandas.ExcelDataSet
 Provides-Extra: pandas.FeatherDataSet
 Provides-Extra: pandas.GBQTableDataSet
 Provides-Extra: pandas.GBQQueryDataSet
 Provides-Extra: pandas.HDFDataSet
 Provides-Extra: pandas.JSONDataSet
 Provides-Extra: pandas.ParquetDataSet
 Provides-Extra: pandas.SQLTableDataSet
 Provides-Extra: pandas.SQLQueryDataSet
 Provides-Extra: pandas.XMLDataSet
 Provides-Extra: pandas.GenericDataSet
 Provides-Extra: pillow.ImageDataSet
-Provides-Extra: polars.CSVDataSet
-Provides-Extra: video.VideoDataSet
 Provides-Extra: plotly.PlotlyDataSet
 Provides-Extra: plotly.JSONDataSet
+Provides-Extra: polars.CSVDataSet
+Provides-Extra: snowflake.SnowparkTableDataSet
 Provides-Extra: spark.SparkDataSet
 Provides-Extra: spark.SparkHiveDataSet
 Provides-Extra: spark.SparkJDBCDataSet
 Provides-Extra: spark.DeltaTableDataSet
-Provides-Extra: snowflake.SnowparkTableDataSet
 Provides-Extra: svmlight.SVMLightDataSet
-Provides-Extra: tensorflow.TensorflowModelDataset
+Provides-Extra: tensorflow.TensorFlowModelDataSet
+Provides-Extra: video.VideoDataSet
 Provides-Extra: yaml.YAMLDataSet
 Provides-Extra: all
 
 # Kedro-Datasets
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/kedro-datasets/)
```

### Comparing `kedro-datasets-1.2.0/README.md` & `kedro-datasets-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.2.0/kedro_datasets/biosequence/biosequence_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/biosequence/biosequence_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from typing import Any, Dict, List
 
 import fsspec
 from Bio import SeqIO
 from kedro.io.core import AbstractDataSet, get_filepath_str, get_protocol_and_path
 
 
-class BioSequenceDataSet(AbstractDataSet[List, List]):
+class BioSequenceDataSet(
+    AbstractDataSet[List, List]
+):  # pylint:disable=too-many-instance-attributes
     r"""``BioSequenceDataSet`` loads and saves data to a sequence file.
 
     Example:
     ::
 
         >>> from kedro_datasets.biosequence import BioSequenceDataSet
         >>> from io import StringIO
@@ -32,25 +34,26 @@
         >>> sequence_list = data_set.load()
         >>>
         >>> assert raw_data[0].id == sequence_list[0].id
         >>> assert raw_data[0].seq == sequence_list[0].seq
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """
         Creates a new instance of ``BioSequenceDataSet`` pointing
         to a concrete filepath.
 
         Args:
             filepath: Filepath in POSIX format to sequence file prefixed with a protocol like
@@ -65,14 +68,16 @@
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `r` when loading
                 and to `w` when saving.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Note: Here you can find all supported file formats: https://biopython.org/wiki/SeqIO
         """
 
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
@@ -96,14 +101,16 @@
             self._save_args.update(save_args)
 
         _fs_open_args_load.setdefault("mode", "r")
         _fs_open_args_save.setdefault("mode", "w")
         self._fs_open_args_load = _fs_open_args_load
         self._fs_open_args_save = _fs_open_args_save
 
+        self.metadata = metadata
+
     def _describe(self) -> Dict[str, Any]:
         return {
             "filepath": self._filepath,
             "protocol": self._protocol,
             "load_args": self._load_args,
             "save_args": self._save_args,
         }
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/dask/parquet_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/dask/parquet_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,25 +79,26 @@
             compression: GZIP
             schema:
               col1: [int32]
               col2: [int32]
               col3: [[int32]]
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {"write_index": False}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {"write_index": False}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``ParquetDataSet`` pointing to concrete
         parquet files.
 
         Args:
             filepath: Filepath in POSIX format to a parquet file
                 parquet collection or the directory of a multipart parquet.
@@ -105,19 +106,23 @@
                 https://docs.dask.org/en/latest/generated/dask.dataframe.read_parquet.html
             save_args: Additional saving options for `dask.dataframe.to_parquet`:
                 https://docs.dask.org/en/latest/generated/dask.dataframe.to_parquet.html
             credentials: Credentials required to get access to the underlying filesystem.
                 E.g. for ``GCSFileSystem`` it should look like `{"token": None}`.
             fs_args: Optional parameters to the backend file system driver:
                 https://docs.dask.org/en/latest/how-to/connect-to-remote-data.html#optional-parameters
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         self._filepath = filepath
         self._fs_args = deepcopy(fs_args) or {}
         self._credentials = deepcopy(credentials) or {}
 
+        self.metadata = metadata
+
         # Handle default load and save arguments
         self._load_args = deepcopy(self.DEFAULT_LOAD_ARGS)
         if load_args is not None:
             self._load_args.update(load_args)
         self._save_args = deepcopy(self.DEFAULT_SAVE_ARGS)
         if save_args is not None:
             self._save_args.update(save_args)
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/email/message_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/email/message_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,26 +48,27 @@
         >>> data_set = EmailMessageDataSet(filepath="test")
         >>> data_set.save(msg)
         >>> reloaded = data_set.load()
         >>> assert msg.__dict__ == reloaded.__dict__
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``EmailMessageDataSet`` pointing to a concrete text file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a text file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
@@ -99,27 +100,31 @@
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `r` when loading
                 and to `w` when saving.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
 
         self._protocol = protocol
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/geopandas/geojson_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/geopandas/geojson_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,26 +40,27 @@
         >>> data_set.save(data)
         >>> reloaded = data_set.load()
         >>>
         >>> assert data.equals(reloaded)
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
     DEFAULT_SAVE_ARGS = {"driver": "GeoJSON"}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``GeoJSONDataSet`` pointing to a concrete GeoJSON file
         on a specific filesystem fsspec.
 
         Args:
 
             filepath: Filepath in POSIX format to a GeoJSON file prefixed with a protocol like
@@ -81,26 +82,30 @@
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `wb` when saving.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = copy.deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _credentials = copy.deepcopy(credentials) or {}
         protocol, path = get_protocol_and_path(filepath, version)
         self._protocol = protocol
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/holoviews/holoviews_writer.py` & `kedro-datasets-1.3.0/kedro_datasets/holoviews/holoviews_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,24 +33,25 @@
         >>> curve = hv.Curve(range(10))
         >>> holoviews_writer = HoloviewsWriter("/tmp/holoviews")
         >>>
         >>> holoviews_writer.save(curve)
 
     """
 
-    DEFAULT_SAVE_ARGS = {"fmt": "png"}  # type: Dict[str, Any]
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {"fmt": "png"}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         fs_args: Dict[str, Any] = None,
         credentials: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``HoloviewsWriter``.
 
         Args:
             filepath: Filepath in POSIX format to a text file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
                 The prefix should be any protocol supported by ``fsspec``.
@@ -66,27 +67,31 @@
                 `{'key': '<id>', 'secret': '<key>'}}`
             save_args: Extra save args passed to `holoviews.save()`. See
                 https://holoviews.org/reference_manual/holoviews.util.html#holoviews.util.save
             version: If specified, should be an instance of
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _credentials = deepcopy(credentials) or {}
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _fs_open_args_save.setdefault("mode", "wb")
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/json/json_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/json/json_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,24 +45,25 @@
         >>> data_set = JSONDataSet(filepath="test.json")
         >>> data_set.save(data)
         >>> reloaded = data_set.load()
         >>> assert data == reloaded
 
     """
 
-    DEFAULT_SAVE_ARGS = {"indent": 2}  # type: Dict[str, Any]
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {"indent": 2}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``JSONDataSet`` pointing to a concrete JSON file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a JSON file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
@@ -82,27 +83,31 @@
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `r` when loading
                 and to `w` when saving.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
 
         self._protocol = protocol
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/matplotlib/matplotlib_writer.py` & `kedro-datasets-1.3.0/kedro_datasets/matplotlib/matplotlib_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,25 +100,26 @@
         >>> list_plot_writer = MatplotlibWriter(
         >>>     filepath="data/08_reporting/plots"
         >>> )
         >>> list_plot_writer.save(plots_list)
 
     """
 
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         fs_args: Dict[str, Any] = None,
         credentials: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         overwrite: bool = False,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``MatplotlibWriter``.
 
         Args:
             filepath: Filepath in POSIX format to save Matplotlib objects to, prefixed with a
                 protocol like `s3://`. If prefix is not provided, `file` protocol (local filesystem)
                 will be used. The prefix should be any protocol supported by ``fsspec``.
@@ -136,27 +137,31 @@
             version: If specified, should be an instance of
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             overwrite: If True, any existing image files will be removed.
                 Only relevant when saving multiple Matplotlib objects at
                 once.
+            metadata: Any arbitrary Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _credentials = deepcopy(credentials) or {}
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _fs_open_args_save.setdefault("mode", "wb")
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/networkx/gml_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/networkx/gml_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,26 +32,27 @@
         >>> graph_dataset = GMLDataSet(filepath="test.gml")
         >>> graph_dataset.save(graph)
         >>> reloaded = graph_dataset.load()
         >>> assert nx.is_isomorphic(graph, reloaded)
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``GMLDataSet``.
 
         Args:
             filepath: Filepath in POSIX format to the NetworkX GML file.
             load_args: Arguments passed on to ``networkx.read_gml``.
                 See the details in
@@ -69,27 +70,31 @@
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `r` when loading
                 and to `w` when saving.
+            metadata: Any Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/networkx/graphml_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/networkx/graphml_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,26 +31,27 @@
         >>> graph_dataset = GraphMLDataSet(filepath="test.graphml")
         >>> graph_dataset.save(graph)
         >>> reloaded = graph_dataset.load()
         >>> assert nx.is_isomorphic(graph, reloaded)
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``GraphMLDataSet``.
 
         Args:
             filepath: Filepath in POSIX format to the NetworkX GraphML file.
             load_args: Arguments passed on to ``networkx.read_graphml``.
                 See the details in
@@ -68,27 +69,31 @@
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `r` when loading
                 and to `w` when saving.
+            metadata: Any arbitrary Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/networkx/json_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/networkx/json_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,26 +32,27 @@
         >>> graph_dataset = JSONDataSet(filepath="test.json")
         >>> graph_dataset.save(graph)
         >>> reloaded = graph_dataset.load()
         >>> assert nx.is_isomorphic(graph, reloaded)
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``JSONDataSet``.
 
         Args:
             filepath: Filepath in POSIX format to the NetworkX graph JSON file.
             load_args: Arguments passed on to ``networkx.node_link_graph``.
                 See the details in
@@ -69,27 +70,31 @@
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `r` when loading
                 and to `w` when saving.
+            metadata: Any Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/pandas/__init__.py` & `kedro-datasets-1.3.0/kedro_datasets/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.2.0/kedro_datasets/pandas/csv_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/pandas/csv_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,26 +61,27 @@
         >>> data_set = CSVDataSet(filepath="test.csv")
         >>> data_set.save(data)
         >>> reloaded = data_set.load()
         >>> assert data.equals(reloaded)
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {"index": False}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {"index": False}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``CSVDataSet`` pointing to a concrete CSV file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a CSV file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
@@ -98,26 +99,30 @@
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             credentials: Credentials required to get access to the underlying filesystem.
                 E.g. for ``GCSFileSystem`` it should look like `{"token": None}`.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
+            metadata: Any Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._storage_options = {**_credentials, **_fs_args}
         self._fs = fsspec.filesystem(self._protocol, **self._storage_options)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/pandas/excel_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/pandas/excel_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         filepath: str,
         engine: str = "openpyxl",
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``ExcelDataSet`` pointing to a concrete Excel file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a Excel file prefixed with a protocol like
                 `s3://`. If prefix is not provided, `file` protocol (local filesystem) will be used.
@@ -146,14 +147,16 @@
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             credentials: Credentials required to get access to the underlying filesystem.
                 E.g. for ``GCSFileSystem`` it should look like `{"token": None}`.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             DataSetError: If versioning is enabled while in append mode.
         """
         _fs_args = deepcopy(fs_args) or {}
         _credentials = deepcopy(credentials) or {}
 
@@ -161,14 +164,16 @@
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._storage_options = {**_credentials, **_fs_args}
         self._fs = fsspec.filesystem(self._protocol, **self._storage_options)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/pandas/feather_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/pandas/feather_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,26 +61,27 @@
         >>> data_set.save(data)
         >>> reloaded = data_set.load()
         >>>
         >>> assert data.equals(reloaded)
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``FeatherDataSet`` pointing to a concrete
         filepath.
 
         Args:
             filepath: Filepath in POSIX format to a feather file prefixed with a protocol like
                 `s3://`. If prefix is not provided, `file` protocol (local filesystem) will be used.
@@ -98,26 +99,30 @@
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             credentials: Credentials required to get access to the underlying filesystem.
                 E.g. for ``GCSFileSystem`` it should look like `{"token": None}`.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._storage_options = {**_credentials, **_fs_args}
         self._fs = fsspec.filesystem(self._protocol, **self._storage_options)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/pandas/gbq_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/pandas/gbq_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,17 @@
     DataSetError,
     get_filepath_str,
     get_protocol_and_path,
     validate_on_forbidden_chars,
 )
 
 
-class GBQTableDataSet(AbstractDataSet[None, pd.DataFrame]):
+class GBQTableDataSet(
+    AbstractDataSet[None, pd.DataFrame]
+):  # pylint:disable=too-many-instance-attributes
     """``GBQTableDataSet`` loads and saves data from/to Google BigQuery.
     It uses pandas-gbq to read and write from/to BigQuery table.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
 
@@ -58,26 +60,27 @@
         >>> data_set.save(data)
         >>> reloaded = data_set.load()
         >>>
         >>> assert data.equals(reloaded)
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {"progress_bar": False}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {"progress_bar": False}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         dataset: str,
         table_name: str,
         project: str = None,
         credentials: Union[Dict[str, Any], Credentials] = None,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``GBQTableDataSet``.
 
         Args:
             dataset: Google BigQuery dataset.
             table_name: Google BigQuery table name.
             project: Google BigQuery Account project ID.
@@ -92,14 +95,16 @@
                 Here you can find all available arguments:
                 https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_gbq.html
                 All defaults are preserved.
             save_args: Pandas options for saving DataFrame to BigQuery table.
                 Here you can find all available arguments:
                 https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_gbq.html
                 All defaults are preserved, but "progress_bar", which is set to False.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             DataSetError: When ``load_args['location']`` and ``save_args['location']``
                 are different.
         """
         # Handle default load and save arguments
         self._load_args = copy.deepcopy(self.DEFAULT_LOAD_ARGS)
@@ -121,14 +126,16 @@
         self._credentials = credentials
         self._client = bigquery.Client(
             project=self._project_id,
             credentials=self._credentials,
             location=self._save_args.get("location"),
         )
 
+        self.metadata = metadata
+
     def _describe(self) -> Dict[str, Any]:
         return {
             "dataset": self._dataset,
             "table_name": self._table_name,
             "load_args": self._load_args,
             "save_args": self._save_args,
         }
@@ -167,15 +174,17 @@
                 """"load_args['location']" is different from "save_args['location']". """
                 "The 'location' defines where BigQuery data is stored, therefore has "
                 "to be the same for save and load args. "
                 "Details: https://cloud.google.com/bigquery/docs/locations"
             )
 
 
-class GBQQueryDataSet(AbstractDataSet[None, pd.DataFrame]):
+class GBQQueryDataSet(
+    AbstractDataSet[None, pd.DataFrame]
+):  # pylint:disable=too-many-instance-attributes
     """``GBQQueryDataSet`` loads data from a provided SQL query from Google
     BigQuery. It uses ``pandas.read_gbq`` which itself uses ``pandas-gbq``
     internally to read from BigQuery table. Therefore it supports all allowed
     pandas options on ``read_gbq``.
 
     Example adding a catalog entry with the ``YAML API``:
 
@@ -199,25 +208,26 @@
         >>>
         >>> data_set = GBQQueryDataSet(sql, project='my-project')
         >>>
         >>> sql_data = data_set.load()
         >>>
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         sql: str = None,
         project: str = None,
         credentials: Union[Dict[str, Any], Credentials] = None,
         load_args: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
         filepath: str = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``GBQQueryDataSet``.
 
         Args:
             sql: The sql query statement.
             project: Google BigQuery Account project ID.
                 Optional when available from the environment.
@@ -231,14 +241,16 @@
                 Here you can find all available arguments:
                 https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_gbq.html
                 All defaults are preserved.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``) used for reading the
                 SQL query from filepath.
             filepath: A path to a file with a sql query statement.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             DataSetError: When ``sql`` and ``filepath`` parameters are either both empty
                 or both provided, as well as when the `save()` method is invoked.
         """
         if sql and filepath:
             raise DataSetError(
@@ -279,14 +291,16 @@
             _fs_credentials = _fs_args.pop("credentials", {})
             protocol, path = get_protocol_and_path(str(filepath))
 
             self._protocol = protocol
             self._fs = fsspec.filesystem(self._protocol, **_fs_credentials, **_fs_args)
             self._filepath = path
 
+        self.metadata = metadata
+
     def _describe(self) -> Dict[str, Any]:
         load_args = copy.deepcopy(self._load_args)
         desc = {}
         desc["sql"] = str(load_args.pop("query", None))
         desc["filepath"] = str(self._filepath)
         desc["load_args"] = str(load_args)
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/pandas/generic_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/pandas/generic_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     "records",
     "timestamp",
     "xarray",
     "sql_table",
 ]
 
 
-class GenericDataSet(AbstractVersionedDataSet[pd.DataFrame, pd.DataFrame]):
+class GenericDataSet(
+    AbstractVersionedDataSet[pd.DataFrame, pd.DataFrame]
+):  # pylint:disable=too-many-instance-attributes
     """`pandas.GenericDataSet` loads/saves data from/to a data file using an underlying
     filesystem (e.g.: local, S3, GCS). It uses pandas to dynamically select the
     appropriate type of read/write target on a best effort basis.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
@@ -77,27 +79,28 @@
         >>> data_set = GenericDataSet(filepath="test.csv", file_format='csv')
         >>> data_set.save(data)
         >>> reloaded = data_set.load()
         >>> assert data.equals(reloaded)
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         file_format: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ):
         """Creates a new instance of ``GenericDataSet`` pointing to a concrete data file
         on a specific filesystem. The appropriate pandas load/save methods are
         dynamically identified by string matching on a best effort basis.
 
         Args:
             filepath: Filepath in POSIX format to a file prefixed with a protocol like `s3://`.
@@ -130,14 +133,16 @@
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `r` when loading
                 and to `w` when saving.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             DataSetError: Will be raised if at least less than one appropriate
                 read or write methods are identified.
         """
 
         self._file_format = file_format.lower()
@@ -150,14 +155,16 @@
         protocol, path = get_protocol_and_path(filepath)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
 
@@ -177,30 +184,28 @@
         if self._file_format in NON_FILE_SYSTEM_TARGETS:
             raise DataSetError(
                 f"Cannot create a dataset of file_format '{self._file_format}' as it "
                 f"does not support a filepath target/source."
             )
 
     def _load(self) -> pd.DataFrame:
-
         self._ensure_file_system_target()
 
         load_path = get_filepath_str(self._get_load_path(), self._protocol)
         load_method = getattr(pd, f"read_{self._file_format}", None)
         if load_method:
             with self._fs.open(load_path, **self._fs_open_args_load) as fs_file:
                 return load_method(fs_file, **self._load_args)
         raise DataSetError(
             f"Unable to retrieve 'pandas.read_{self._file_format}' method, please ensure that your "
             "'file_format' parameter has been defined correctly as per the Pandas API "
             "https://pandas.pydata.org/docs/reference/io.html"
         )
 
     def _save(self, data: pd.DataFrame) -> None:
-
         self._ensure_file_system_target()
 
         save_path = get_filepath_str(self._get_save_path(), self._protocol)
         save_method = getattr(data, f"to_{self._file_format}", None)
         if save_method:
             with self._fs.open(save_path, **self._fs_open_args_save) as fs_file:
                 # KEY ASSUMPTION - first argument is path/buffer/io
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/pandas/hdf_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/svmlight/svmlight_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,189 +1,183 @@
-"""``HDFDataSet`` loads/saves data from/to a hdf file using an underlying
-filesystem (e.g.: local, S3, GCS). It uses pandas.HDFStore to handle the hdf file.
+"""``SVMLightDataSet`` loads/saves data from/to a svmlight/libsvm file using an
+underlying filesystem (e.g.: local, S3, GCS). It uses sklearn functions
+``dump_svmlight_file`` to save and ``load_svmlight_file`` to load a file.
 """
 from copy import deepcopy
 from pathlib import PurePosixPath
-from threading import Lock
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Tuple, Union
 
 import fsspec
-import pandas as pd
 from kedro.io.core import (
     AbstractVersionedDataSet,
     DataSetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
+from numpy import ndarray
+from scipy.sparse.csr import csr_matrix
+from sklearn.datasets import dump_svmlight_file, load_svmlight_file
 
-HDFSTORE_DRIVER = "H5FD_CORE"
+# NOTE: kedro.extras.datasets will be removed in Kedro 0.19.0.
+# Any contribution to datasets should be made in kedro-datasets
+# in kedro-plugins (https://github.com/kedro-org/kedro-plugins)
 
+# Type of data input
+_DI = Tuple[Union[ndarray, csr_matrix], ndarray]
+# Type of data output
+_DO = Tuple[csr_matrix, ndarray]
 
-class HDFDataSet(AbstractVersionedDataSet[pd.DataFrame, pd.DataFrame]):
-    """``HDFDataSet`` loads/saves data from/to a hdf file using an underlying
-    filesystem (e.g. local, S3, GCS). It uses pandas.HDFStore to handle the hdf file.
+
+class SVMLightDataSet(AbstractVersionedDataSet[_DI, _DO]):
+    """``SVMLightDataSet`` loads/saves data from/to a svmlight/libsvm file using an
+    underlying filesystem (e.g.: local, S3, GCS). It uses sklearn functions
+    ``dump_svmlight_file`` to save and ``load_svmlight_file`` to load a file.
+
+    Data is loaded as a tuple of features and labels. Labels is NumPy array,
+    and features is Compressed Sparse Row matrix.
+
+    This format is a text-based format, with one sample per line. It does
+    not store zero valued features hence it is suitable for sparse datasets.
+
+    This format is used as the default format for both svmlight and the
+    libsvm command line programs.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
 
     .. code-block:: yaml
 
-        hdf_dataset:
-          type: pandas.HDFDataSet
-          filepath: s3://my_bucket/raw/sensor_reading.h5
-          credentials: aws_s3_creds
-          key: data
+        svm_dataset:
+          type: svmlight.SVMLightDataSet
+          filepath: data/01_raw/location.svm
+          load_args:
+            zero_based: False
+          save_args:
+            zero_based: False
+
+        cars:
+          type: svmlight.SVMLightDataSet
+          filepath: gcs://your_bucket/cars.svm
+          fs_args:
+            project: my-project
+          credentials: my_gcp_credentials
+          load_args:
+            zero_based: False
+          save_args:
+            zero_based: False
 
     Example usage for the
     `Python API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-code-api>`_:
     ::
 
-        >>> from kedro_datasets.pandas import HDFDataSet
-        >>> import pandas as pd
+        >>> from kedro_datasets.svmlight import SVMLightDataSet
+        >>> import numpy as np
         >>>
-        >>> data = pd.DataFrame({'col1': [1, 2], 'col2': [4, 5],
-        >>>                      'col3': [5, 6]})
+        >>> # Features and labels.
+        >>> data = (np.array([[0, 1], [2, 3.14159]]), np.array([7, 3]))
         >>>
-        >>> data_set = HDFDataSet(filepath="test.h5", key='data')
+        >>> data_set = SVMLightDataSet(filepath="test.svm")
         >>> data_set.save(data)
-        >>> reloaded = data_set.load()
-        >>> assert data.equals(reloaded)
+        >>> reloaded_features, reloaded_labels = data_set.load()
+        >>> assert (data[0] == reloaded_features).all()
+        >>> assert (data[1] == reloaded_labels).all()
 
     """
 
-    # _lock is a class attribute that will be shared across all the instances.
-    # It is used to make dataset safe for threads.
-    _lock = Lock()
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
-        key: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
-        version: Version = None,
+        version: Optional[Version] = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
-        """Creates a new instance of ``HDFDataSet`` pointing to a concrete hdf file
-        on a specific filesystem.
+        """Creates a new instance of SVMLightDataSet to load/save data from a svmlight/libsvm file.
 
         Args:
-            filepath: Filepath in POSIX format to a hdf file prefixed with a protocol like `s3://`.
+            filepath: Filepath in POSIX format to a text file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
                 The prefix should be any protocol supported by ``fsspec``.
-                Note: `http(s)` doesn't support versioning.
-            key: Identifier to the group in the HDF store.
-            load_args: PyTables options for loading hdf files.
-                You can find all available arguments at:
-                https://www.pytables.org/usersguide/libref/top_level.html#tables.open_file
-                All defaults are preserved.
-            save_args: PyTables options for saving hdf files.
-                You can find all available arguments at:
-                https://www.pytables.org/usersguide/libref/top_level.html#tables.open_file
-                All defaults are preserved.
+            load_args: Arguments passed on to ``load_svmlight_file``.
+                See the details in
+                https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_svmlight_file.html
+            save_args: Arguments passed on to ``dump_svmlight_file``.
+                See the details in
+                https://scikit-learn.org/stable/modules/generated/sklearn.datasets.dump_svmlight_file.html
             version: If specified, should be an instance of
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             credentials: Credentials required to get access to the underlying filesystem.
                 E.g. for ``GCSFileSystem`` it should look like `{"token": None}`.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
-                (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
-                to pass to the filesystem's `open` method through nested keys
-                `open_args_load` and `open_args_save`.
-                Here you can find all available arguments for `open`:
-                https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
-                All defaults are preserved, except `mode`, which is set `wb` when saving.
+                (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
-        if protocol == "file":
-            _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
+        if protocol == "file":
+            _fs_args.setdefault("auto_mkdir", True)
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
 
-        self._key = key
-
-        # Handle default load and save arguments
         self._load_args = deepcopy(self.DEFAULT_LOAD_ARGS)
         if load_args is not None:
             self._load_args.update(load_args)
         self._save_args = deepcopy(self.DEFAULT_SAVE_ARGS)
         if save_args is not None:
             self._save_args.update(save_args)
 
+        _fs_open_args_load.setdefault("mode", "rb")
         _fs_open_args_save.setdefault("mode", "wb")
         self._fs_open_args_load = _fs_open_args_load
         self._fs_open_args_save = _fs_open_args_save
 
-    def _describe(self) -> Dict[str, Any]:
+    def _describe(self):
         return {
             "filepath": self._filepath,
-            "key": self._key,
             "protocol": self._protocol,
             "load_args": self._load_args,
             "save_args": self._save_args,
             "version": self._version,
         }
 
-    def _load(self) -> pd.DataFrame:
+    def _load(self) -> _DO:
         load_path = get_filepath_str(self._get_load_path(), self._protocol)
-
         with self._fs.open(load_path, **self._fs_open_args_load) as fs_file:
-            binary_data = fs_file.read()
+            return load_svmlight_file(fs_file, **self._load_args)
 
-        with HDFDataSet._lock:
-            # Set driver_core_backing_store to False to disable saving
-            # contents of the in-memory h5file to disk
-            with pd.HDFStore(
-                "in-memory-load-file",
-                mode="r",
-                driver=HDFSTORE_DRIVER,
-                driver_core_backing_store=0,
-                driver_core_image=binary_data,
-                **self._load_args,
-            ) as store:
-                return store[self._key]
-
-    def _save(self, data: pd.DataFrame) -> None:
+    def _save(self, data: _DI) -> None:
         save_path = get_filepath_str(self._get_save_path(), self._protocol)
-
-        with HDFDataSet._lock:
-            with pd.HDFStore(
-                "in-memory-save-file",
-                mode="w",
-                driver=HDFSTORE_DRIVER,
-                driver_core_backing_store=0,
-                **self._save_args,
-            ) as store:
-                store.put(self._key, data, format="table")
-                # pylint: disable=protected-access
-                binary_data = store._handle.get_file_image()
-
         with self._fs.open(save_path, **self._fs_open_args_save) as fs_file:
-            fs_file.write(binary_data)
+            dump_svmlight_file(data[0], data[1], fs_file, **self._save_args)
 
         self._invalidate_cache()
 
     def _exists(self) -> bool:
         try:
             load_path = get_filepath_str(self._get_load_path(), self._protocol)
         except DataSetError:
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/pandas/json_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/pandas/json_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,26 +56,27 @@
         >>> data_set = JSONDataSet(filepath="test.json")
         >>> data_set.save(data)
         >>> reloaded = data_set.load()
         >>> assert data.equals(reloaded)
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``JSONDataSet`` pointing to a concrete JSON file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a JSON file prefixed with a protocol like `s3://`.
                 If prefix is not provided `file` protocol (local filesystem) will be used.
@@ -93,25 +94,29 @@
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             credentials: Credentials required to get access to the underlying filesystem.
                 E.g. for ``GCSFileSystem`` it should look like `{'token': None}`.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _credentials = deepcopy(credentials) or {}
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._storage_options = {**_credentials, **_fs_args}
         self._fs = fsspec.filesystem(self._protocol, **self._storage_options)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/pandas/parquet_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/pandas/parquet_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,26 +67,27 @@
         >>> data_set = ParquetDataSet(filepath="test.parquet")
         >>> data_set.save(data)
         >>> reloaded = data_set.load()
         >>> assert data.equals(reloaded)
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``ParquetDataSet`` pointing to a concrete Parquet file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a Parquet file prefixed with a protocol like
                 `s3://`. If prefix is not provided, `file` protocol (local filesystem) will be used.
@@ -107,26 +108,30 @@
             version: If specified, should be an instance of ``kedro.io.core.Version``.
                 If its ``load`` attribute is None, the latest version will be loaded. If
                 its ``save`` attribute is None, save version will be autogenerated.
             credentials: Credentials required to get access to the underlying filesystem.
                 E.g. for ``GCSFileSystem`` it should look like `{"token": None}`.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._storage_options = {**_credentials, **_fs_args}
         self._fs = fsspec.filesystem(self._protocol, **self._storage_options)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/pandas/sql_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/pandas/sql_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 import pandas as pd
 from kedro.io.core import (
     AbstractDataSet,
     DataSetError,
     get_filepath_str,
     get_protocol_and_path,
 )
-from sqlalchemy import create_engine
+from sqlalchemy import create_engine, inspect
 from sqlalchemy.exc import NoSuchModuleError
 
 __all__ = ["SQLTableDataSet", "SQLQueryDataSet"]
 
 KNOWN_PIP_INSTALL = {
     "psycopg2": "psycopg2",
     "mysqldb": "mysqlclient",
     "cx_Oracle": "cx_Oracle",
     "mssql": "pyodbc",
 }
 
 DRIVER_ERROR_MESSAGE = """
 A module/driver is missing when connecting to your SQL server. SQLDataSet
  supports SQLAlchemy drivers. Please refer to
- https://docs.sqlalchemy.org/en/13/core/engines.html#supported-databases
+ https://docs.sqlalchemy.org/core/engines.html#supported-databases
  for more information.
 \n\n
 """
 
 
 def _find_known_drivers(module_import_error: ImportError) -> Optional[str]:
     """Looks up known keywords in a ``ModuleNotFoundError`` so that it can
@@ -79,29 +79,29 @@
     return DataSetError(f"{DRIVER_ERROR_MESSAGE}{missing_module_instruction}")
 
 
 def _get_sql_alchemy_missing_error() -> DataSetError:
     return DataSetError(
         "The SQL dialect in your connection is not supported by "
         "SQLAlchemy. Please refer to "
-        "https://docs.sqlalchemy.org/en/13/core/engines.html#supported-databases "
+        "https://docs.sqlalchemy.org/core/engines.html#supported-databases "
         "for more information."
     )
 
 
 class SQLTableDataSet(AbstractDataSet[pd.DataFrame, pd.DataFrame]):
     """``SQLTableDataSet`` loads data from a SQL table and saves a pandas
     dataframe to a table. It uses ``pandas.DataFrame`` internally,
     so it supports all allowed pandas options on ``read_sql_table`` and
     ``to_sql`` methods. Since Pandas uses SQLAlchemy behind the scenes, when
     instantiating ``SQLTableDataSet`` one needs to pass a compatible connection
     string either in ``credentials`` (see the example code snippet below) or in
     ``load_args`` and ``save_args``. Connection string formats supported by
     SQLAlchemy can be found here:
-    https://docs.sqlalchemy.org/en/13/core/engines.html#database-urls
+    https://docs.sqlalchemy.org/core/engines.html#database-urls
 
     ``SQLTableDataSet`` modifies the save parameters and stores
     the data with no index. This is designed to make load and save methods
     symmetric.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
@@ -152,46 +152,50 @@
 
     DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: Dict[str, Any] = {"index": False}
     # using Any because of Sphinx but it should be
     # sqlalchemy.engine.Engine or sqlalchemy.engine.base.Engine
     engines: Dict[str, Any] = {}
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         table_name: str,
         credentials: Dict[str, Any],
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new ``SQLTableDataSet``.
 
         Args:
             table_name: The table name to load or save data to. It
                 overwrites name in ``save_args`` and ``table_name``
                 parameters in ``load_args``.
             credentials: A dictionary with a ``SQLAlchemy`` connection string.
                 Users are supposed to provide the connection string 'con'
                 through credentials. It overwrites `con` parameter in
                 ``load_args`` and ``save_args`` in case it is provided. To find
                 all supported connection string formats, see here:
-                https://docs.sqlalchemy.org/en/13/core/engines.html#database-urls
+                https://docs.sqlalchemy.org/core/engines.html#database-urls
             load_args: Provided to underlying pandas ``read_sql_table``
                 function along with the connection string.
                 To find all supported arguments, see here:
                 https://pandas.pydata.org/pandas-docs/stable/generated/pandas.read_sql_table.html
                 To find all supported connection string formats, see here:
-                https://docs.sqlalchemy.org/en/13/core/engines.html#database-urls
+                https://docs.sqlalchemy.org/core/engines.html#database-urls
             save_args: Provided to underlying pandas ``to_sql`` function along
                 with the connection string.
                 To find all supported arguments, see here:
                 https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.to_sql.html
                 To find all supported connection string formats, see here:
-                https://docs.sqlalchemy.org/en/13/core/engines.html#database-urls
+                https://docs.sqlalchemy.org/core/engines.html#database-urls
                 It has ``index=False`` in the default parameters.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             DataSetError: When either ``table_name`` or ``con`` is empty.
         """
 
         if not table_name:
             raise DataSetError("'table_name' argument cannot be empty.")
@@ -212,18 +216,20 @@
 
         self._load_args["table_name"] = table_name
         self._save_args["name"] = table_name
 
         self._connection_str = credentials["con"]
         self.create_connection(self._connection_str)
 
+        self.metadata = metadata
+
     @classmethod
     def create_connection(cls, connection_str: str) -> None:
         """Given a connection string, create singleton connection
-        to be used across all instances of `SQLTableDataSet` that
+        to be used across all instances of ``SQLTableDataSet`` that
         need to connect to the same source.
         """
         if connection_str in cls.engines:
             return
 
         try:
             engine = create_engine(connection_str)
@@ -250,29 +256,29 @@
         return pd.read_sql_table(con=engine, **self._load_args)
 
     def _save(self, data: pd.DataFrame) -> None:
         engine = self.engines[self._connection_str]  # type: ignore
         data.to_sql(con=engine, **self._save_args)
 
     def _exists(self) -> bool:
-        eng = self.engines[self._connection_str]  # type: ignore
+        engine = self.engines[self._connection_str]  # type: ignore
+        insp = inspect(engine)
         schema = self._load_args.get("schema", None)
-        exists = self._load_args["table_name"] in eng.table_names(schema)
-        return exists
+        return insp.has_table(self._load_args["table_name"], schema)
 
 
 class SQLQueryDataSet(AbstractDataSet[None, pd.DataFrame]):
     """``SQLQueryDataSet`` loads data from a provided SQL query. It
     uses ``pandas.DataFrame`` internally, so it supports all allowed
     pandas options on ``read_sql_query``. Since Pandas uses SQLAlchemy behind
     the scenes, when instantiating ``SQLQueryDataSet`` one needs to pass
     a compatible connection string either in ``credentials`` (see the example
     code snippet below) or in ``load_args``. Connection string formats supported
     by SQLAlchemy can be found here:
-    https://docs.sqlalchemy.org/en/13/core/engines.html#database-urls
+    https://docs.sqlalchemy.org/core/engines.html#database-urls
 
     It does not support save method so it is a read only data set.
     To save data to a SQL server use ``SQLTableDataSet``.
 
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
@@ -376,45 +382,48 @@
         self,
         sql: str = None,
         credentials: Dict[str, Any] = None,
         load_args: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
         filepath: str = None,
         execution_options: Optional[Dict[str, Any]] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new ``SQLQueryDataSet``.
 
         Args:
             sql: The sql query statement.
             credentials: A dictionary with a ``SQLAlchemy`` connection string.
                 Users are supposed to provide the connection string 'con'
                 through credentials. It overwrites `con` parameter in
                 ``load_args`` and ``save_args`` in case it is provided. To find
                 all supported connection string formats, see here:
-                https://docs.sqlalchemy.org/en/13/core/engines.html#database-urls
+                https://docs.sqlalchemy.org/core/engines.html#database-urls
             load_args: Provided to underlying pandas ``read_sql_query``
                 function along with the connection string.
                 To find all supported arguments, see here:
                 https://pandas.pydata.org/pandas-docs/stable/generated/pandas.read_sql_query.html
                 To find all supported connection string formats, see here:
-                https://docs.sqlalchemy.org/en/13/core/engines.html#database-urls
+                https://docs.sqlalchemy.org/core/engines.html#database-urls
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `r` when loading.
             filepath: A path to a file with a sql query statement.
             execution_options: A dictionary with non-SQL advanced options for the connection to
                 be applied to the underlying engine. To find all supported execution
                 options, see here:
-                https://docs.sqlalchemy.org/en/12/core/connections.html#sqlalchemy.engine.Connection.execution_options
+                https://docs.sqlalchemy.org/core/connections.html#sqlalchemy.engine.Connection.execution_options
                 Note that this is not a standard argument supported by pandas API, but could be
                 useful for handling large datasets.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             DataSetError: When either ``sql`` or ``con`` parameters is empty.
         """
         if sql and filepath:
             raise DataSetError(
                 "'sql' and 'filepath' arguments cannot both be provided."
@@ -429,22 +438,24 @@
 
         if not (credentials and "con" in credentials and credentials["con"]):
             raise DataSetError(
                 "'con' argument cannot be empty. Please "
                 "provide a SQLAlchemy connection string."
             )
 
-        default_load_args = {}  # type: Dict[str, Any]
+        default_load_args: Dict[str, Any] = {}
 
         self._load_args = (
             {**default_load_args, **load_args}
             if load_args is not None
             else default_load_args
         )
 
+        self.metadata = metadata
+
         # load sql query from file
         if sql:
             self._load_args["sql"] = sql
             self._filepath = None
         else:
             # filesystem for loading sql file
             _fs_args = copy.deepcopy(fs_args) or {}
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/pandas/xml_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/pandas/xml_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,26 +39,27 @@
         >>> data_set = XMLDataSet(filepath="test.xml")
         >>> data_set.save(data)
         >>> reloaded = data_set.load()
         >>> assert data.equals(reloaded)
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {"index": False}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {"index": False}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``XMLDataSet`` pointing to a concrete XML file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a XML file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
@@ -76,26 +77,30 @@
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             credentials: Credentials required to get access to the underlying filesystem.
                 E.g. for ``GCSFileSystem`` it should look like `{"token": None}`.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._storage_options = {**_credentials, **_fs_args}
         self._fs = fsspec.filesystem(self._protocol, **self._storage_options)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/pickle/pickle_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/pickle/pickle_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     DataSetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
 
 
-class PickleDataSet(AbstractVersionedDataSet[Any, Any]):
+class PickleDataSet(
+    AbstractVersionedDataSet[Any, Any]
+):  # pylint:disable=too-many-instance-attributes
     """``PickleDataSet`` loads/saves data from/to a Pickle file using an underlying
     filesystem (e.g.: local, S3, GCS). The underlying functionality is supported by
     the specified backend library passed in (defaults to the ``pickle`` library), so it
     supports all allowed options for loading and saving pickle files.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
@@ -64,27 +66,28 @@
         >>>                          load_args={"compression":"lz4"},
         >>>                          save_args={"compression":"lz4"})
         >>> data_set.save(data)
         >>> reloaded = data_set.load()
         >>> assert data.equals(reloaded)
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments,too-many-locals
     def __init__(
         self,
         filepath: str,
         backend: str = "pickle",
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``PickleDataSet`` pointing to a concrete Pickle
         file on a specific filesystem. ``PickleDataSet`` supports custom backends to
         serialise/deserialise objects.
 
         Example backends that are compatible (non-exhaustive):
             * `pickle`
@@ -128,14 +131,16 @@
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `wb` when saving.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             ValueError: If ``backend`` does not satisfy the `pickle` interface.
             ImportError: If the ``backend`` module could not be imported.
         """
         # We do not store `imported_backend` as an attribute to be used in `load`/`save`
         # as this would mean the dataset cannot be deepcopied (module objects cannot be
@@ -166,14 +171,16 @@
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/pillow/image_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/pillow/image_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,24 +29,25 @@
         >>>
         >>> data_set = ImageDataSet(filepath="test.png")
         >>> image = data_set.load()
         >>> image.show()
 
     """
 
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``ImageDataSet`` pointing to a concrete image file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to an image file prefixed with a protocol like
                 `s3://`. If prefix is not provided, `file` protocol (local filesystem) will be used.
@@ -66,27 +67,31 @@
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `r` when loading
                 and to `w` when saving.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/plotly/json_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/plotly/json_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,26 +45,27 @@
         >>> fig = px.bar(x=["a", "b", "c"], y=[1, 3, 2])
         >>> data_set = JSONDataSet(filepath="test.json")
         >>> data_set.save(fig)
         >>> reloaded = data_set.load()
         >>> assert fig == reloaded
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``JSONDataSet`` pointing to a concrete JSON file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a JSON file prefixed with a protocol like `s3://`.
                 If prefix is not provided `file` protocol (local filesystem) will be used.
@@ -88,27 +89,31 @@
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `w` when
                 saving.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/plotly/plotly_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/plotly/plotly_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         filepath: str,
         plotly_args: Dict[str, Any],
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``PlotlyDataSet`` pointing to a concrete JSON file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a JSON file prefixed with a protocol like `s3://`.
                 If prefix is not provided `file` protocol (local filesystem) will be used.
@@ -105,26 +106,30 @@
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `w` when saving.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         super().__init__(filepath, load_args, save_args, version, credentials, fs_args)
         self._plotly_args = plotly_args
 
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _fs_open_args_save.setdefault("mode", "w")
 
         self._fs_open_args_load = _fs_open_args_load
         self._fs_open_args_save = _fs_open_args_save
 
+        self.metadata = metadata
+
     def _describe(self) -> Dict[str, Any]:
         return {**super()._describe(), "plotly_args": self._plotly_args}
 
     def _save(self, data: pd.DataFrame) -> None:
         fig = self._plot_dataframe(data)
         super()._save(fig)
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/polars/csv_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/polars/csv_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,26 +59,27 @@
         >>> data_set = CSVDataSet(filepath="test.csv")
         >>> data_set.save(data)
         >>> reloaded = data_set.load()
         >>> assert data.frame_equal(reloaded)
 
     """
 
-    DEFAULT_LOAD_ARGS = {"rechunk": True}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {"rechunk": True}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``CSVDataSet`` pointing to a concrete CSV file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a CSV file prefixed with a protocol
                 `s3://`.
@@ -99,26 +100,30 @@
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             credentials: Credentials required to get access to the underlying filesystem.
                 E.g. for ``GCSFileSystem`` it should look like `{"token": None}`.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._storage_options = {**_credentials, **_fs_args}
         self._fs = fsspec.filesystem(self._protocol, **self._storage_options)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/redis/redis_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/redis/redis_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from copy import deepcopy
 from typing import Any, Dict
 
 import redis
 from kedro.io.core import AbstractDataSet, DataSetError
 
 
-class PickleDataSet(AbstractDataSet[Any, Any]):
+class PickleDataSet(
+    AbstractDataSet[Any, Any]
+):  # pylint:disable=too-many-instance-attributes
     """``PickleDataSet`` loads/saves data from/to a Redis database. The
     underlying functionality is supported by the redis library, so it supports
     all allowed options for instantiating the redis app ``from_url`` and setting
     a value.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
@@ -52,26 +54,27 @@
         >>> my_data = PickleDataSet(key="my_data")
         >>> my_data.save(data)
         >>> reloaded = my_data.load()
         >>> assert data.equals(reloaded)
     """
 
     DEFAULT_REDIS_URL = os.getenv("REDIS_URL", "redis://127.0.0.1:6379")
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         key: str,
         backend: str = "pickle",
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         credentials: Dict[str, Any] = None,
         redis_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``PickleDataSet``. This loads/saves data from/to
         a Redis database while deserialising/serialising. Supports custom backends to
         serialise/deserialise objects.
 
         Example backends that are compatible (non-exhaustive):
             * `pickle`
@@ -105,14 +108,16 @@
             redis_args: Extra arguments to pass into the redis client constructor
                 ``redis.StrictRedis.from_url``. (e.g. `{"socket_timeout": 10}`), as well as to pass
                 to the ``redis.StrictRedis.set`` through nested keys `from_url_args` and `set_args`.
                 Here you can find all available arguments for `from_url`:
                 https://redis-py.readthedocs.io/en/stable/connections.html?highlight=from_url#redis.Redis.from_url
                 All defaults are preserved, except `url`, which is set to `redis://127.0.0.1:6379`.
                 You could also specify the url through the env variable ``REDIS_URL``.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             ValueError: If ``backend`` does not satisfy the `pickle` interface.
             ImportError: If the ``backend`` module could not be imported.
         """
         try:
             imported_backend = importlib.import_module(backend)
@@ -130,14 +135,16 @@
                 "Missing one of 'loads' and 'dumps' on the backend."
             )
 
         self._backend = backend
 
         self._key = key
 
+        self.metadata = metadata
+
         _redis_args = deepcopy(redis_args) or {}
         self._redis_from_url_args = _redis_args.pop("from_url_args", {})
         self._redis_from_url_args.setdefault("url", self.DEFAULT_REDIS_URL)
         self._redis_set_args = _redis_args.pop("set_args", {})
         _credentials = deepcopy(credentials) or {}
 
         self._load_args = deepcopy(self.DEFAULT_LOAD_ARGS)
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/snowflake/snowpark_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/snowflake/snowpark_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 
 import snowflake.snowpark as sp
 from kedro.io.core import AbstractDataSet, DataSetError
 
 logger = logging.getLogger(__name__)
 
 
-class SnowparkTableDataSet(AbstractDataSet):
+class SnowparkTableDataSet(
+    AbstractDataSet
+):  # pylint:disable=too-many-instance-attributes
     """``SnowparkTableDataSet`` loads and saves Snowpark dataframes.
 
     As of Mar-2023, the snowpark connector only works with Python 3.8.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
 
     .. code-block:: yaml
+
         weather:
           type: kedro_datasets.snowflake.SnowparkTableDataSet
           table_name: "weather_data"
           database: "meteorology"
           schema: "observations"
           credentials: db_credentials
           save_args:
@@ -41,14 +44,15 @@
     "weather" reuses credentials parameters, "polygons" catalog entry reuses
     all credentials parameters except providing a different schema name.
     Second example of credentials file uses ``externalbrowser`` authentication.
 
     catalog.yml
 
     .. code-block:: yaml
+
         weather:
           type: kedro_datasets.snowflake.SnowparkTableDataSet
           table_name: "weather_data"
           database: "meteorology"
           schema: "observations"
           credentials: snowflake_client
           save_args:
@@ -61,52 +65,56 @@
           table_name: "geopolygons"
           credentials: snowflake_client
           schema: "geodata"
 
     credentials.yml
 
     .. code-block:: yaml
+
         snowflake_client:
           account: 'ab12345.eu-central-1'
           port: 443
           warehouse: "datascience_wh"
           database: "detailed_data"
           schema: "observations"
           user: "service_account_abc"
           password: "supersecret"
 
     credentials.yml (with externalbrowser authenticator)
 
     .. code-block:: yaml
+
         snowflake_client:
           account: 'ab12345.eu-central-1'
           port: 443
           warehouse: "datascience_wh"
           database: "detailed_data"
           schema: "observations"
           user: "john_doe@wdomain.com"
           authenticator: "externalbrowser"
+
     """
 
     # this dataset cannot be used with ``ParallelRunner``,
     # therefore it has the attribute ``_SINGLE_PROCESS = True``
     # for parallelism within a pipeline please consider
     # ``ThreadRunner`` instead
     _SINGLE_PROCESS = True
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         table_name: str,
         schema: str = None,
         database: str = None,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         credentials: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``SnowparkTableDataSet``.
 
         Args:
             table_name: The table name to load or save data to.
             schema: Name of the schema where ``table_name`` is.
                 Optional as can be provided as part of ``credentials``
@@ -119,14 +127,16 @@
             load_args: Currently not used
             save_args: Provided to underlying snowpark ``save_as_table``
                 To find all supported arguments, see here:
                 https://docs.snowflake.com/en/developer-guide/snowpark/reference/python/api/snowflake.snowpark.DataFrameWriter.saveAsTable.html
             credentials: A dictionary with a snowpark connection string.
                 To find all supported arguments, see here:
                 https://docs.snowflake.com/en/user-guide/python-connector-api.html#connect
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
 
         if not table_name:
             raise DataSetError("'table_name' argument cannot be empty.")
 
         if not credentials:
             raise DataSetError("'credentials' argument cannot be empty.")
@@ -159,14 +169,16 @@
         connection_parameters = credentials
         connection_parameters.update(
             {"database": self._database, "schema": self._schema}
         )
         self._connection_parameters = connection_parameters
         self._session = self._get_session(self._connection_parameters)
 
+        self.metadata = metadata
+
     def _describe(self) -> Dict[str, Any]:
         return {
             "table_name": self._table_name,
             "database": self._database,
             "schema": self._schema,
         }
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/spark/deltatable_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/spark/deltatable_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """``AbstractDataSet`` implementation to access DeltaTables using
 ``delta-spark``
 """
 from pathlib import PurePosixPath
-from typing import NoReturn
+from typing import Any, Dict, NoReturn
 
 from delta.tables import DeltaTable
 from kedro.io.core import AbstractDataSet, DataSetError
 from pyspark.sql import SparkSession
 from pyspark.sql.utils import AnalysisException
 
 from kedro_datasets.spark.spark_dataset import _split_filepath, _strip_dbfs_prefix
@@ -58,27 +58,30 @@
 
     # this dataset cannot be used with ``ParallelRunner``,
     # therefore it has the attribute ``_SINGLE_PROCESS = True``
     # for parallelism within a Spark pipeline please consider
     # using ``ThreadRunner`` instead
     _SINGLE_PROCESS = True
 
-    def __init__(self, filepath: str) -> None:
+    def __init__(self, filepath: str, metadata: Dict[str, Any] = None) -> None:
         """Creates a new instance of ``DeltaTableDataSet``.
 
         Args:
             filepath: Filepath in POSIX format to a Spark dataframe. When using Databricks
                 and working with data written to mount path points,
                 specify ``filepath``s for (versioned) ``SparkDataSet``s
                 starting with ``/dbfs/mnt``.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         fs_prefix, filepath = _split_filepath(filepath)
 
         self._fs_prefix = fs_prefix
         self._filepath = PurePosixPath(filepath)
+        self.metadata = metadata
 
     @staticmethod
     def _get_spark():
         return SparkSession.builder.getOrCreate()
 
     def _load(self) -> DeltaTable:
         load_path = self._fs_prefix + str(self._filepath)
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/spark/spark_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/spark/spark_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -229,25 +229,26 @@
     """
 
     # this dataset cannot be used with ``ParallelRunner``,
     # therefore it has the attribute ``_SINGLE_PROCESS = True``
     # for parallelism within a Spark pipeline please consider
     # ``ThreadRunner`` instead
     _SINGLE_PROCESS = True
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
-    def __init__(  # pylint: disable=too-many-arguments
+    def __init__(  # pylint: disable=too-many-arguments disable=too-many-locals
         self,
         filepath: str,
         file_format: str = "parquet",
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``SparkDataSet``.
 
         Args:
             filepath: Filepath in POSIX format to a Spark dataframe. When using Databricks
                 specify ``filepath``s starting with ``/dbfs/``.
             file_format: File format used during load and save
@@ -271,20 +272,23 @@
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             credentials: Credentials to access the S3 bucket, such as
                 ``key``, ``secret``, if ``filepath`` prefix is ``s3a://`` or ``s3n://``.
                 Optional keyword arguments passed to ``hdfs.client.InsecureClient``
                 if ``filepath`` prefix is ``hdfs://``. Ignored otherwise.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         credentials = deepcopy(credentials) or {}
         fs_prefix, filepath = _split_filepath(filepath)
         path = PurePosixPath(filepath)
         exists_function = None
         glob_function = None
+        self.metadata = metadata
 
         if not filepath.startswith("/dbfs/") and _deployed_on_databricks():
             logger.warning(
                 "Using SparkDataSet on Databricks without the `/dbfs/` prefix in the "
                 "filepath is a known source of error. You must add this prefix to %s",
                 filepath,
             )
@@ -314,17 +318,17 @@
             # dbfs add prefix to Spark path by default
             # See https://github.com/kedro-org/kedro-plugins/issues/117
             dbutils = _get_dbutils(self._get_spark())
             if dbutils:
                 glob_function = partial(_dbfs_glob, dbutils=dbutils)
                 exists_function = partial(_dbfs_exists, dbutils=dbutils)
         else:
-            fs = fsspec.filesystem(fs_prefix.strip("://"), **credentials)
-            exists_function = fs.exists
-            glob_function = fs.glob
+            filesystem = fsspec.filesystem(fs_prefix.strip("://"), **credentials)
+            exists_function = filesystem.exists
+            glob_function = filesystem.glob
 
         super().__init__(
             filepath=path,
             version=version,
             exists_function=exists_function,
             glob_function=glob_function,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/spark/spark_hive_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/spark/spark_hive_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,24 +59,25 @@
         >>>                             write_mode="overwrite")
         >>> data_set.save(spark_df)
         >>> reloaded = data_set.load()
         >>>
         >>> reloaded.take(4)
     """
 
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint:disable=too-many-arguments
     def __init__(
         self,
         database: str,
         table: str,
         write_mode: str = "errorifexists",
         table_pk: List[str] = None,
         save_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``SparkHiveDataSet``.
 
         Args:
             database: The name of the hive database.
             table: The name of the table within the database.
             write_mode: ``insert``, ``upsert`` or ``overwrite`` are supported.
@@ -84,14 +85,16 @@
                 resolve preexisting data. Is required for ``write_mode="upsert"``.
             save_args: Optional mapping of any options,
                 passed to the `DataFrameWriter.saveAsTable` as kwargs.
                 Key example of this is `partitionBy` which allows data partitioning
                 on a list of column names.
                 Other `HiveOptions` can be found here:
                 https://spark.apache.org/docs/latest/sql-data-sources-hive-tables.html#specifying-storage-format-for-hive-tables
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Note:
             For users leveraging the `upsert` functionality,
             a `checkpoint` directory must be set, e.g. using
             `spark.sparkContext.setCheckpointDir("/path/to/dir")`
             or directly in the Spark conf folder.
 
@@ -115,14 +118,16 @@
         self._full_table_address = f"{database}.{table}"
         self._save_args = deepcopy(self.DEFAULT_SAVE_ARGS)
         if save_args is not None:
             self._save_args.update(save_args)
         self._format = self._save_args.pop("format", None) or "hive"
         self._eager_checkpoint = self._save_args.pop("eager_checkpoint", None) or True
 
+        self.metadata = metadata
+
     def _describe(self) -> Dict[str, Any]:
         return {
             "database": self._database,
             "table": self._table,
             "write_mode": self._write_mode,
             "table_pk": self._table_pk,
             "partition_by": self._save_args.get("partitionBy"),
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/spark/spark_jdbc_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/spark/spark_jdbc_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,25 +59,26 @@
         >>> data_set.save(data)
         >>> reloaded = data_set.load()
         >>>
         >>> assert data.toPandas().equals(reloaded.toPandas())
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         url: str,
         table: str,
         credentials: Dict[str, Any] = None,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new ``SparkJDBCDataSet``.
 
         Args:
             url: A JDBC URL of the form ``jdbc:subprotocol:subname``.
             table: The name of the table to load or save data to.
             credentials: A dictionary of JDBC database connection arguments.
@@ -89,14 +90,16 @@
                 with the JDBC URL and the name of the table. To find all
                 supported arguments, see here:
                 https://spark.apache.org/docs/latest/api/python/reference/pyspark.sql/api/pyspark.sql.DataFrameWriter.jdbc.html
             save_args: Provided to underlying PySpark ``jdbc`` function along
                 with the JDBC URL and the name of the table. To find all
                 supported arguments, see here:
                 https://spark.apache.org/docs/latest/api/python/reference/pyspark.sql/api/pyspark.sql.DataFrameWriter.jdbc.html
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             DataSetError: When either ``url`` or ``table`` is empty or
                 when a property is provided with a None value.
         """
 
         if not url:
@@ -112,25 +115,26 @@
                 "provide the name of the table to load or save "
                 "data to."
             )
 
         self._url = url
         self._table = table
 
+        self.metadata = metadata
+
         # Handle default load and save arguments
         self._load_args = deepcopy(self.DEFAULT_LOAD_ARGS)
         if load_args is not None:
             self._load_args.update(load_args)
         self._save_args = deepcopy(self.DEFAULT_SAVE_ARGS)
         if save_args is not None:
             self._save_args.update(save_args)
 
         # Update properties in load_args and save_args with credentials.
         if credentials is not None:
-
             # Check credentials for bad inputs.
             for cred_key, cred_value in credentials.items():
                 if cred_value is None:
                     raise DataSetError(
                         f"Credential property '{cred_key}' cannot be None. "
                         f"Please provide a value."
                     )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""``TensorflowModelDataset`` is a data set implementation which can save and load
+"""``TensorFlowModelDataSet`` is a data set implementation which can save and load
 TensorFlow models.
 """
 import copy
 import tempfile
 from pathlib import PurePath, PurePosixPath
 from typing import Any, Dict
 
@@ -15,69 +15,70 @@
     get_filepath_str,
     get_protocol_and_path,
 )
 
 TEMPORARY_H5_FILE = "tmp_tensorflow_model.h5"
 
 
-class TensorFlowModelDataset(AbstractVersionedDataSet[tf.keras.Model, tf.keras.Model]):
-    """``TensorflowModelDataset`` loads and saves TensorFlow models.
+class TensorFlowModelDataSet(AbstractVersionedDataSet[tf.keras.Model, tf.keras.Model]):
+    """``TensorFlowModelDataSet`` loads and saves TensorFlow models.
     The underlying functionality is supported by, and passes input arguments through to,
     TensorFlow 2.X load_model and save_model methods.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
 
     .. code-block:: yaml
 
         tensorflow_model:
-          type: tensorflow.TensorFlowModelDataset
+          type: tensorflow.TensorFlowModelDataSet
           filepath: data/06_models/tensorflow_model.h5
           load_args:
             compile: False
           save_args:
             overwrite: True
             include_optimizer: False
           credentials: tf_creds
 
     Example usage for the
     `Python API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-code-api>`_:
     ::
 
-        >>> from kedro_datasets.tensorflow import TensorFlowModelDataset
+        >>> from kedro_datasets.tensorflow import TensorFlowModelDataSet
         >>> import tensorflow as tf
         >>> import numpy as np
         >>>
-        >>> data_set = TensorFlowModelDataset("data/06_models/tensorflow_model.h5")
+        >>> data_set = TensorFlowModelDataSet("data/06_models/tensorflow_model.h5")
         >>> model = tf.keras.Model()
         >>> predictions = model.predict([...])
         >>>
         >>> data_set.save(model)
         >>> loaded_model = data_set.load()
         >>> new_predictions = loaded_model.predict([...])
         >>> np.testing.assert_allclose(predictions, new_predictions, rtol=1e-6, atol=1e-6)
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {"save_format": "tf"}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {"save_format": "tf"}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
-        """Creates a new instance of ``TensorFlowModelDataset``.
+        """Creates a new instance of ``TensorFlowModelDataSet``.
 
         Args:
             filepath: Filepath in POSIX format to a TensorFlow model directory prefixed with a
                 protocol like `s3://`. If prefix is not provided `file` protocol (local filesystem)
                 will be used. The prefix should be any protocol supported by ``fsspec``.
                 Note: `http(s)` doesn't support versioning.
             load_args: TensorFlow options for loading models.
@@ -92,23 +93,28 @@
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             credentials: Credentials required to get access to the underlying filesystem.
                 E.g. for ``GCSFileSystem`` it should look like `{'token': None}`.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = copy.deepcopy(fs_args) or {}
         _credentials = copy.deepcopy(credentials) or {}
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
+
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/text/text_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/text/text_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,20 +41,22 @@
         >>> data_set = TextDataSet(filepath="test.md")
         >>> data_set.save(string_to_write)
         >>> reloaded = data_set.load()
         >>> assert string_to_write == reloaded
 
     """
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``TextDataSet`` pointing to a concrete text file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a text file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
@@ -70,27 +72,31 @@
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `r` when loading
                 and to `w` when saving.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/tracking/json_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/tracking/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.2.0/kedro_datasets/tracking/metrics_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/tracking/metrics_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.2.0/kedro_datasets/video/video_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/video/video_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,15 +122,18 @@
         )
 
 
 class SequenceVideo(AbstractVideo):
     """A video object read from an indexable sequence of frames"""
 
     def __init__(
-        self, frames: Sequence[PIL.Image.Image], fps: float, fourcc: str = "mp4v"
+        self,
+        frames: Sequence[PIL.Image.Image],
+        fps: float,
+        fourcc: str = "mp4v",
     ) -> None:
         self._n_frames = len(frames)
         self._frames = frames
         self._fourcc = fourcc
         self._size = frames[0].size
         self._fps = fps
 
@@ -151,14 +154,15 @@
             return SlicedVideo(self, index)
         return self._frames[index]
 
 
 class GeneratorVideo(AbstractVideo):
     """A video object with frames yielded by a generator"""
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         frames: Generator[PIL.Image.Image, None, None],
         length,
         fps: float,
         fourcc: str = "mp4v",
     ) -> None:
@@ -254,42 +258,47 @@
         >>>     frame -= 1
         >>>
         >>> video = VideoDataSet("my_video.mp4")
         >>> video.save(GeneratorVideo(gen(), fps=25, length=None))
 
     """
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         fourcc: Optional[str] = "mp4v",
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of VideoDataSet to load / save video data for given filepath.
 
         Args:
             filepath: The location of the video file to load / save data.
             fourcc: The codec to use when writing video, note that depending on how opencv is
                 installed there might be more or less codecs avaiable. If set to None, the
                 fourcc from the video object will be used.
             credentials: Credentials required to get access to the underlying filesystem.
                 E.g. for ``GCSFileSystem`` it should look like `{"token": None}`.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         # parse the path and protocol (e.g. file, http, s3, etc.)
         protocol, path = get_protocol_and_path(filepath)
         self._protocol = protocol
         self._filepath = PurePosixPath(path)
         self._fourcc = fourcc
         _fs_args = deepcopy(fs_args) or {}
         _credentials = deepcopy(credentials) or {}
         self._storage_options = {**_credentials, **_fs_args}
         self._fs = fsspec.filesystem(self._protocol, **self._storage_options)
+        self.metadata = metadata
 
     def _load(self) -> AbstractVideo:
         """Loads data from the video file.
 
         Returns:
             Data from the video file as a AbstractVideo object
         """
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets/yaml/yaml_dataset.py` & `kedro-datasets-1.3.0/kedro_datasets/yaml/yaml_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,24 +42,25 @@
         >>> data_set = YAMLDataSet(filepath="test.yaml")
         >>> data_set.save(data)
         >>> reloaded = data_set.load()
         >>> assert data == reloaded
 
     """
 
-    DEFAULT_SAVE_ARGS = {"default_flow_style": False}  # type: Dict[str, Any]
+    DEFAULT_SAVE_ARGS: Dict[str, Any] = {"default_flow_style": False}
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         filepath: str,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of ``YAMLDataSet`` pointing to a concrete YAML file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a YAML file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
@@ -79,27 +80,31 @@
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `r` when loading
                 and to `w` when saving.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _credentials = deepcopy(credentials) or {}
 
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._fs = fsspec.filesystem(self._protocol, **_credentials, **_fs_args)
 
+        self.metadata = metadata
+
         super().__init__(
             filepath=PurePosixPath(path),
             version=version,
             exists_function=self._fs.exists,
             glob_function=self._fs.glob,
         )
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets.egg-info/PKG-INFO` & `kedro-datasets-1.3.0/kedro_datasets.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 1.2.0
+Version: 1.3.0
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
-Home-page: https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Author: Kedro
 License: Apache Software License (Apache 2.0)
-Requires-Python: >=3.7, <3.11
+Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
+Project-URL: Documentation, https://docs.kedro.org
+Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: api
 Provides-Extra: biosequence
 Provides-Extra: dask
+Provides-Extra: databricks
 Provides-Extra: docs
 Provides-Extra: geopandas
-Provides-Extra: matplotlib
 Provides-Extra: holoviews
+Provides-Extra: matplotlib
 Provides-Extra: networkx
 Provides-Extra: pandas
 Provides-Extra: pillow
-Provides-Extra: polars
-Provides-Extra: video
 Provides-Extra: plotly
+Provides-Extra: polars
 Provides-Extra: redis
+Provides-Extra: snowflake
 Provides-Extra: spark
 Provides-Extra: svmlight
 Provides-Extra: tensorflow
+Provides-Extra: video
 Provides-Extra: yaml
 Provides-Extra: api.APIDataSet
 Provides-Extra: biosequence.BioSequenceDataSet
 Provides-Extra: dask.ParquetDataSet
+Provides-Extra: databricks.ManagedTableDataSet
 Provides-Extra: geopandas.GeoJSONDataSet
-Provides-Extra: matplotlib.MatplotlibWriter
 Provides-Extra: holoviews.HoloviewsWriter
+Provides-Extra: matplotlib.MatplotlibWriter
 Provides-Extra: networkx.NetworkXDataSet
 Provides-Extra: pandas.CSVDataSet
 Provides-Extra: pandas.ExcelDataSet
 Provides-Extra: pandas.FeatherDataSet
 Provides-Extra: pandas.GBQTableDataSet
 Provides-Extra: pandas.GBQQueryDataSet
 Provides-Extra: pandas.HDFDataSet
 Provides-Extra: pandas.JSONDataSet
 Provides-Extra: pandas.ParquetDataSet
 Provides-Extra: pandas.SQLTableDataSet
 Provides-Extra: pandas.SQLQueryDataSet
 Provides-Extra: pandas.XMLDataSet
 Provides-Extra: pandas.GenericDataSet
 Provides-Extra: pillow.ImageDataSet
-Provides-Extra: polars.CSVDataSet
-Provides-Extra: video.VideoDataSet
 Provides-Extra: plotly.PlotlyDataSet
 Provides-Extra: plotly.JSONDataSet
+Provides-Extra: polars.CSVDataSet
+Provides-Extra: snowflake.SnowparkTableDataSet
 Provides-Extra: spark.SparkDataSet
 Provides-Extra: spark.SparkHiveDataSet
 Provides-Extra: spark.SparkJDBCDataSet
 Provides-Extra: spark.DeltaTableDataSet
-Provides-Extra: snowflake.SnowparkTableDataSet
 Provides-Extra: svmlight.SVMLightDataSet
-Provides-Extra: tensorflow.TensorflowModelDataset
+Provides-Extra: tensorflow.TensorFlowModelDataSet
+Provides-Extra: video.VideoDataSet
 Provides-Extra: yaml.YAMLDataSet
 Provides-Extra: all
 
 # Kedro-Datasets
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/kedro-datasets/)
```

### Comparing `kedro-datasets-1.2.0/kedro_datasets.egg-info/SOURCES.txt` & `kedro-datasets-1.3.0/kedro_datasets.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 README.md
 pyproject.toml
 setup.py
-features/__init__.py
 kedro_datasets/__init__.py
 kedro_datasets.egg-info/PKG-INFO
 kedro_datasets.egg-info/SOURCES.txt
 kedro_datasets.egg-info/dependency_links.txt
 kedro_datasets.egg-info/requires.txt
 kedro_datasets.egg-info/top_level.txt
 kedro_datasets/api/__init__.py
 kedro_datasets/api/api_dataset.py
 kedro_datasets/biosequence/__init__.py
 kedro_datasets/biosequence/biosequence_dataset.py
 kedro_datasets/dask/__init__.py
 kedro_datasets/dask/parquet_dataset.py
+kedro_datasets/databricks/__init__.py
+kedro_datasets/databricks/managed_table_dataset.py
 kedro_datasets/email/__init__.py
 kedro_datasets/email/message_dataset.py
 kedro_datasets/geopandas/__init__.py
 kedro_datasets/geopandas/geojson_dataset.py
 kedro_datasets/holoviews/__init__.py
 kedro_datasets/holoviews/holoviews_writer.py
 kedro_datasets/json/__init__.py
```

