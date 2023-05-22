# Comparing `tmp/sarus-0.6.4.dev0.tar.gz` & `tmp/sarus-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus-0.6.4.dev0.tar", last modified: Mon May 15 16:11:45 2023, max compression
+gzip compressed data, was "sarus-0.6.5.tar", last modified: Mon May 22 16:45:34 2023, max compression
```

## Comparing `sarus-0.6.4.dev0.tar` & `sarus-0.6.5.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.567939 sarus-0.6.4.dev0/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1558 2023-05-15 16:11:45.567939 sarus-0.6.4.dev0/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.6.4.dev0/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.6.4.dev0/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.555940 sarus-0.6.4.dev0/sarus/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      544 2023-05-15 16:11:21.000000 sarus-0.6.4.dev0/sarus/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    12831 2023-05-15 16:11:06.000000 sarus-0.6.4.dev0/sarus/config.yaml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.555940 sarus-0.6.4.dev0/sarus/context/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/context/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-05-15 07:50:17.000000 sarus-0.6.4.dev0/sarus/context/local_sdk.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-15 07:50:17.000000 sarus-0.6.4.dev0/sarus/context/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13886 2023-05-15 16:11:06.000000 sarus-0.6.4.dev0/sarus/dataspec_wrapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-04-21 19:49:48.000000 sarus-0.6.4.dev0/sarus/debug.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.555940 sarus-0.6.4.dev0/sarus/imblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/imblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/imblearn/under_sampling.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.555940 sarus-0.6.4.dev0/sarus/legacy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/legacy/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.555940 sarus-0.6.4.dev0/sarus/legacy/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2023-01-27 14:38:46.000000 sarus-0.6.4.dev0/sarus/legacy/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    16606 2023-01-27 14:38:46.000000 sarus-0.6.4.dev0/sarus/legacy/pandas/dataframe.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.555940 sarus-0.6.4.dev0/sarus/legacy/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2022-12-01 13:21:20.000000 sarus-0.6.4.dev0/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/legacy/tensorflow/model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.559939 sarus-0.6.4.dev0/sarus/manager/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/manager/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-15 09:41:41.000000 sarus-0.6.4.dev0/sarus/manager/arrow_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-15 09:41:41.000000 sarus-0.6.4.dev0/sarus/manager/arrow_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-15 09:41:41.000000 sarus-0.6.4.dev0/sarus/manager/base_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-15 09:41:41.000000 sarus-0.6.4.dev0/sarus/manager/cache_scalar_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7609 2023-05-15 09:41:41.000000 sarus-0.6.4.dev0/sarus/manager/dataspec_api.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.559939 sarus-0.6.4.dev0/sarus/manager/ops/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      921 2023-04-21 19:49:48.000000 sarus-0.6.4.dev0/sarus/manager/ops/api.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-15 09:41:41.000000 sarus-0.6.4.dev0/sarus/manager/parquet_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    21049 2023-05-15 16:11:06.000000 sarus-0.6.4.dev0/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2556 2023-05-04 12:45:45.000000 sarus-0.6.4.dev0/sarus/manager/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-15 09:41:41.000000 sarus-0.6.4.dev0/sarus/manager/value_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-15 09:41:41.000000 sarus-0.6.4.dev0/sarus/manager/value_remote.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.559939 sarus-0.6.4.dev0/sarus/numpy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/numpy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/numpy/random.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/numpy/scalars.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.559939 sarus-0.6.4.dev0/sarus/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      822 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/pandas/core.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4918 2023-04-21 19:49:48.000000 sarus-0.6.4.dev0/sarus/pandas/dataframe.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/pandas/io.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.563939 sarus-0.6.4.dev0/sarus/pandas_profiling/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-15 07:50:17.000000 sarus-0.6.4.dev0/sarus/pandas_profiling/profile_report.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.563939 sarus-0.6.4.dev0/sarus/plotly/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/plotly/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/plotly/express.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    55850 2023-05-15 09:41:41.000000 sarus-0.6.4.dev0/sarus/sarus.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.563939 sarus-0.6.4.dev0/sarus/scripts/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-04-21 19:49:48.000000 sarus-0.6.4.dev0/sarus/scripts/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-15 09:41:41.000000 sarus-0.6.4.dev0/sarus/scripts/generate_op_list.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.563939 sarus-0.6.4.dev0/sarus/sklearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-04-21 19:49:48.000000 sarus-0.6.4.dev0/sarus/sklearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-15 07:50:17.000000 sarus-0.6.4.dev0/sarus/sklearn/cluster.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/sklearn/compose.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-15 07:50:17.000000 sarus-0.6.4.dev0/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-15 07:50:17.000000 sarus-0.6.4.dev0/sarus/sklearn/ensemble.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/sklearn/impute.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/sklearn/inspection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-04-21 19:49:48.000000 sarus-0.6.4.dev0/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/sklearn/metrics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-15 09:41:41.000000 sarus-0.6.4.dev0/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-15 09:41:41.000000 sarus-0.6.4.dev0/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-04-21 19:49:48.000000 sarus-0.6.4.dev0/sarus/sklearn/svm.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.567939 sarus-0.6.4.dev0/sarus/skopt/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/skopt/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/skopt/searchcv.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.567939 sarus-0.6.4.dev0/sarus/std/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/std/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1074 2022-11-29 13:03:29.000000 sarus-0.6.4.dev0/sarus/std/types.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.567939 sarus-0.6.4.dev0/sarus/storage/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-01-27 14:38:46.000000 sarus-0.6.4.dev0/sarus/storage/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4552 2023-01-27 14:38:46.000000 sarus-0.6.4.dev0/sarus/storage/legacy_local.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.567939 sarus-0.6.4.dev0/sarus/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1810 2023-05-15 16:11:06.000000 sarus-0.6.4.dev0/sarus/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10848 2023-05-15 16:11:06.000000 sarus-0.6.4.dev0/sarus/utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-04-21 19:49:48.000000 sarus-0.6.4.dev0/sarus/wrapper_factory.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.567939 sarus-0.6.4.dev0/sarus/xgboost/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2022-09-14 12:56:20.000000 sarus-0.6.4.dev0/sarus/xgboost/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-15 09:41:41.000000 sarus-0.6.4.dev0/sarus/xgboost/xgboost.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.555940 sarus-0.6.4.dev0/sarus.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1558 2023-05-15 16:11:45.000000 sarus-0.6.4.dev0/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2086 2023-05-15 16:11:45.000000 sarus-0.6.4.dev0/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-15 16:11:45.000000 sarus-0.6.4.dev0/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.6.4.dev0/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      344 2023-05-15 16:11:45.000000 sarus-0.6.4.dev0/sarus.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-05-15 16:11:45.000000 sarus-0.6.4.dev0/sarus.egg-info/top_level.txt
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1301 2023-05-15 16:11:45.567939 sarus-0.6.4.dev0/setup.cfg
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      111 2023-05-15 16:11:27.000000 sarus-0.6.4.dev0/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 16:11:45.567939 sarus-0.6.4.dev0/tests/
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.6.4.dev0/tests/test_sanity.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.845399 sarus-0.6.5/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2022-09-14 12:56:20.000000 sarus-0.6.5/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-22 16:45:34.845399 sarus-0.6.5/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.6.5/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.6.5/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.821399 sarus-0.6.5/sarus/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      544 2023-05-22 16:38:31.000000 sarus-0.6.5/sarus/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    12913 2023-05-22 16:34:35.000000 sarus-0.6.5/sarus/config.yaml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.825399 sarus-0.6.5/sarus/context/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/context/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-05-15 07:50:17.000000 sarus-0.6.5/sarus/context/local_sdk.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-15 07:50:17.000000 sarus-0.6.5/sarus/context/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    14066 2023-05-22 16:34:35.000000 sarus-0.6.5/sarus/dataspec_wrapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/debug.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.825399 sarus-0.6.5/sarus/imblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/imblearn/under_sampling.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.825399 sarus-0.6.5/sarus/legacy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/legacy/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.825399 sarus-0.6.5/sarus/legacy/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2023-01-27 14:38:46.000000 sarus-0.6.5/sarus/legacy/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    16606 2023-01-27 14:38:46.000000 sarus-0.6.5/sarus/legacy/pandas/dataframe.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.829399 sarus-0.6.5/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2022-12-01 13:21:20.000000 sarus-0.6.5/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/legacy/tensorflow/model.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.833399 sarus-0.6.5/sarus/manager/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/manager/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/base_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7609 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/dataspec_api.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.833399 sarus-0.6.5/sarus/manager/ops/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      921 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/manager/ops/api.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/parquet_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    21049 2023-05-15 16:20:25.000000 sarus-0.6.5/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2650 2023-05-22 16:34:35.000000 sarus-0.6.5/sarus/manager/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/value_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/manager/value_remote.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.833399 sarus-0.6.5/sarus/numpy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/numpy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/numpy/random.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/numpy/scalars.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.833399 sarus-0.6.5/sarus/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      822 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/pandas/core.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4918 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/pandas/io.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.837399 sarus-0.6.5/sarus/pandas_profiling/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-15 07:50:17.000000 sarus-0.6.5/sarus/pandas_profiling/profile_report.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.837399 sarus-0.6.5/sarus/plotly/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/plotly/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/plotly/express.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    55850 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/sarus.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.837399 sarus-0.6.5/sarus/scripts/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/scripts/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/scripts/generate_op_list.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.841399 sarus-0.6.5/sarus/sklearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-15 07:50:17.000000 sarus-0.6.5/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/sklearn/compose.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-15 07:50:17.000000 sarus-0.6.5/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-15 07:50:17.000000 sarus-0.6.5/sarus/sklearn/ensemble.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/sklearn/impute.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/sklearn/svm.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.841399 sarus-0.6.5/sarus/skopt/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/skopt/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/skopt/searchcv.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.845399 sarus-0.6.5/sarus/std/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2022-11-29 13:03:29.000000 sarus-0.6.5/sarus/std/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1600 2023-05-22 16:34:35.000000 sarus-0.6.5/sarus/std/types.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.845399 sarus-0.6.5/sarus/storage/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-01-27 14:38:46.000000 sarus-0.6.5/sarus/storage/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4552 2023-01-27 14:38:46.000000 sarus-0.6.5/sarus/storage/legacy_local.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.845399 sarus-0.6.5/sarus/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1831 2023-05-22 16:34:35.000000 sarus-0.6.5/sarus/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10848 2023-05-15 16:20:25.000000 sarus-0.6.5/sarus/utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-04-21 19:49:48.000000 sarus-0.6.5/sarus/wrapper_factory.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.845399 sarus-0.6.5/sarus/xgboost/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2022-09-14 12:56:20.000000 sarus-0.6.5/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-15 09:41:41.000000 sarus-0.6.5/sarus/xgboost/xgboost.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.821399 sarus-0.6.5/sarus.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-22 16:45:34.000000 sarus-0.6.5/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2086 2023-05-22 16:45:34.000000 sarus-0.6.5/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-22 16:45:34.000000 sarus-0.6.5/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.6.5/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      344 2023-05-22 16:45:34.000000 sarus-0.6.5/sarus.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-05-22 16:45:34.000000 sarus-0.6.5/sarus.egg-info/top_level.txt
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1301 2023-05-22 16:45:34.845399 sarus-0.6.5/setup.cfg
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      106 2023-05-22 16:38:22.000000 sarus-0.6.5/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-22 16:45:34.845399 sarus-0.6.5/tests/
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.6.5/tests/test_sanity.py
```

### Comparing `sarus-0.6.4.dev0/PKG-INFO` & `sarus-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.4.dev0
+Version: 0.6.5
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.6.4.dev0/README.rst` & `sarus-0.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/__init__.py` & `sarus-0.6.5/sarus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         std,
         xgboost,
     )
 
     from .sarus import Client, Dataset
     from .utils import eval, eval_policy, floating, integer, length
 
-VERSION = "0.6.3"
+VERSION = "0.6.5"
 
 __all__ = [
     "Dataset",
     "Client",
     "length",
     "eval",
     "eval_policy",
```

### Comparing `sarus-0.6.4.dev0/sarus/config.yaml` & `sarus-0.6.5/sarus/config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         PrettyDict:
           keys: std.KEYS
           values: std.VALUES
     dataframe:
       classes:
         DataFrame:
           __eq__: pandas.PD_EQ
+          __getitem__: pandas.PD_GETITEM
           abs: pandas.PD_ABS
           add: pandas.PD_ADD
           agg: pandas.PD_AGG
           any: pandas.PD_ANY
           append: pandas.PD_APPEND
           astype: pandas.PD_ASTYPE
           count: pandas.PD_COUNT
@@ -138,14 +139,15 @@
           sum: pandas.PD_SUM
           to_dict: pandas.PD_TO_DICT
           transpose: pandas.PD_TRANSPOSE
           nunique: pandas.PD_NUNIQUE
           value_counts: pandas.PD_VALUE_COUNTS
         Series:
           __eq__: pandas.PD_EQ
+          __getitem__: pandas.PD_GETITEM
           abs: pandas.PD_ABS
           add: pandas.PD_ADD
           agg: pandas.PD_AGG
           any: pandas.PD_ANY
           append: pandas.PD_APPEND
           astype: pandas.PD_ASTYPE
           corr: pandas.PD_CORR_SERIES
```

### Comparing `sarus-0.6.4.dev0/sarus/context/local_sdk.py` & `sarus-0.6.5/sarus/context/local_sdk.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/dataspec_wrapper.py` & `sarus-0.6.5/sarus/dataspec_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     Any,
     Dict,
     Generic,
     List,
     Optional,
     Tuple,
     TypeVar,
+    Union,
     cast,
     get_args,
 )
 
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 from sarus_data_spec.context import global_context
@@ -160,27 +161,29 @@
         symbols = dict()
         for uuid, _id in DataSpecWrapper.instances.items():
             symbols[uuid] = mapping.get(_id, None)
         return symbols
 
     def dot(
         self,
-        kind: DataSpecVariant = DataSpecVariant.ALTERNATIVE,
+        kind: Union[DataSpecVariant, str] = DataSpecVariant.ALTERNATIVE,
         remote: bool = True,
     ) -> str:
         """Graphviz's dot representation of the DataSpecWrapper graph.
 
         Uses color codes to show statuses.
 
         Args:
             kind (DataSpecVariant): the DataSpec to represent.
             remote (true): Which Manager to inspect.
                 If true shows the DataSpec's status on the server,
                 else show the DataSpec's status locally.
         """
+        if isinstance(kind, str):
+            kind = DataSpecVariant(kind)
         ds = self.dataspec(kind)
         caller_frame = inspect.currentframe().f_back
         symbols = self.dataspec_wrapper_symbols(
             caller_frame.f_locals, caller_frame.f_globals
         )
         return self.manager().dot(ds, symbols=symbols, remote=remote)
 
@@ -335,14 +338,15 @@
 
         if verbose is None:
             context: LocalSDKContext = global_context()
             verbose = context.verbose()
 
         if (
             target_epsilon is not None
+            and target_epsilon > 0
             and alt_policy == DataspecPrivacyPolicy.SYNTHETIC
             and verbose >= 1
         ):
             logger.warning(
                 "Warning: target_epsilon could not be consumed. "
                 "This might be due to privacy budget "
                 "constraints or some operations not "
@@ -352,15 +356,15 @@
         if alt_dataspec.prototype() == sp.Dataset:
             dataset = cast(st.Dataset, alt_dataspec)
             value = dataset.to(self.__wraps__)
         else:
             scalar = cast(st.Scalar, alt_dataspec)
             value = cast(st.Scalar, scalar.value())
 
-        if verbose >= 1:
+        if verbose >= 1 and alt_policy != DataspecPrivacyPolicy.PUBLIC:
             message = alt_policy.value
             if alt_policy == DataspecPrivacyPolicy.DP:
                 epsilon = self.manager().consumed_epsilon(alt_dataspec)
                 message = f"{message} (epsilon={epsilon:.2f})"
 
             print(message)
```

### Comparing `sarus-0.6.4.dev0/sarus/debug.py` & `sarus-0.6.5/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/imblearn/over_sampling.py` & `sarus-0.6.5/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/imblearn/pipeline.py` & `sarus-0.6.5/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/imblearn/under_sampling.py` & `sarus-0.6.5/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/legacy/pandas/dataframe.py` & `sarus-0.6.5/sarus/legacy/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/legacy/tensorflow/dataset.py` & `sarus-0.6.5/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/legacy/tensorflow/model.py` & `sarus-0.6.5/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/manager/arrow_local.py` & `sarus-0.6.5/sarus/manager/arrow_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/manager/arrow_remote.py` & `sarus-0.6.5/sarus/manager/arrow_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/manager/base_remote.py` & `sarus-0.6.5/sarus/manager/base_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/manager/cache_scalar_local.py` & `sarus-0.6.5/sarus/manager/cache_scalar_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/manager/dataspec_api.py` & `sarus-0.6.5/sarus/manager/dataspec_api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/manager/ops/api.py` & `sarus-0.6.5/sarus/manager/ops/api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/manager/parquet_local.py` & `sarus-0.6.5/sarus/manager/parquet_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/manager/sdk_manager.py` & `sarus-0.6.5/sarus/manager/sdk_manager.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/manager/typing.py` & `sarus-0.6.5/sarus/manager/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import typing as t
 
 import sarus_data_spec.typing as st
+from sarus_data_spec.dataspec_validator.typing import DataspecPrivacyPolicy
 from sarus_data_spec.manager.base import Computation
 from sarus_data_spec.manager.typing import Manager
 
 from sarus.typing import Client
 
 
 class SDKManager(Manager, t.Protocol):
@@ -39,15 +40,15 @@
         """Return the sarus.Client object used to make API calls."""
 
     def launch(self, dataspec: st.DataSpec) -> None:
         """Launch a Dataspec's computation on the server."""
 
     def compile(
         self, dataspec: st.DataSpec, target_epsilon: t.Optional[float] = None
-    ) -> t.Tuple[st.DataSpec, str]:
+    ) -> t.Tuple[st.DataSpec, DataspecPrivacyPolicy]:
         """Compile an alternative Dataspec on the server."""
 
     def push(self, dataspec: st.DataSpec) -> None:
         """Push a Dataspec's computation graph on the server."""
 
     def dataspec_computation(self, dataspec: st.DataSpec) -> Computation:
         """Return the Computation for getting the dataspec's value. If sql is
```

### Comparing `sarus-0.6.4.dev0/sarus/manager/value_local.py` & `sarus-0.6.5/sarus/manager/value_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/manager/value_remote.py` & `sarus-0.6.5/sarus/manager/value_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/numpy/scalars.py` & `sarus-0.6.5/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/pandas/core.py` & `sarus-0.6.5/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/pandas/dataframe.py` & `sarus-0.6.5/sarus/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/sarus.py` & `sarus-0.6.5/sarus/sarus.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/scripts/generate_op_list.py` & `sarus-0.6.5/sarus/scripts/generate_op_list.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/sklearn/__init__.py` & `sarus-0.6.5/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/sklearn/cluster.py` & `sarus-0.6.5/sarus/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/sklearn/compose.py` & `sarus-0.6.5/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/sklearn/decomposition.py` & `sarus-0.6.5/sarus/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/sklearn/ensemble.py` & `sarus-0.6.5/sarus/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/sklearn/impute.py` & `sarus-0.6.5/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/sklearn/linear_model.py` & `sarus-0.6.5/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/sklearn/model_selection.py` & `sarus-0.6.5/sarus/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/sklearn/pipeline.py` & `sarus-0.6.5/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/sklearn/preprocessing.py` & `sarus-0.6.5/sarus/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/sklearn/svm.py` & `sarus-0.6.5/sarus/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/skopt/searchcv.py` & `sarus-0.6.5/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/std/types.py` & `sarus-0.6.5/sarus/std/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,22 +22,44 @@
         ...
 
 
 class List(DataSpecWrapper[list]):
     @sarus_init("std.LIST")
     def __init__(self, *args, **kwargs) -> None:
         """Need to pass all arguments List(*args)."""
-        ...
+
+    def __iter__(self):
+        self.__sarus_idx__ = 0
+        return self
+
+    def __next__(self):
+        try:
+            idx = self.__sarus_idx__
+            self.__sarus_idx__ += 1
+            return self[idx]
+        except IndexError:
+            raise StopIteration
 
 
 class Tuple(DataSpecWrapper[tuple]):
     @sarus_init("std.TUPLE")
     def __init__(self, *args, **kwargs) -> None:
         """Need to pass all arguments Tuple(*args)."""
-        ...
+
+    def __iter__(self):
+        self.__sarus_idx__ = 0
+        return self
+
+    def __next__(self):
+        try:
+            idx = self.__sarus_idx__
+            self.__sarus_idx__ += 1
+            return self[idx]
+        except IndexError:
+            raise StopIteration
 
 
 class Int(DataSpecWrapper[int]):
     ...
 
 
 class Float(DataSpecWrapper[float]):
```

### Comparing `sarus-0.6.4.dev0/sarus/storage/legacy_local.py` & `sarus-0.6.5/sarus/storage/legacy_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/typing.py` & `sarus-0.6.5/sarus/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 
 SPECIAL_WRAPPER_ATTRIBUTES = [
     "_alt_dataspec",
     "_dataspec",
     "_alt_policy",
     "_manager",
+    "__sarus_idx__",
 ]
 
 MOCK = "mock"
 PYTHON_TYPE = "python_type"
 ADMIN_DS = "admin_ds"
 ATTRIBUTES_DS = "attributes_ds"
```

### Comparing `sarus-0.6.4.dev0/sarus/utils.py` & `sarus-0.6.5/sarus/utils.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/wrapper_factory.py` & `sarus-0.6.5/sarus/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus/xgboost/xgboost.py` & `sarus-0.6.5/sarus/xgboost/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/sarus.egg-info/PKG-INFO` & `sarus-0.6.5/sarus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.4.dev0
+Version: 0.6.5
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.6.4.dev0/sarus.egg-info/SOURCES.txt` & `sarus-0.6.5/sarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus-0.6.4.dev0/setup.cfg` & `sarus-0.6.5/setup.cfg`

 * *Files identical despite different names*

