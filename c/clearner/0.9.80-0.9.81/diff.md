# Comparing `tmp/clearner-0.9.80.tar.gz` & `tmp/clearner-0.9.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clearner-0.9.80.tar", last modified: Thu May 18 02:06:19 2023, max compression
+gzip compressed data, was "clearner-0.9.81.tar", last modified: Sat May 20 02:59:29 2023, max compression
```

## Comparing `clearner-0.9.80.tar` & `clearner-0.9.81.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1993 2022-08-17 03:32:28.000000 clearner-0.9.80/LICENSE
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      349 2023-05-18 02:06:19.000000 clearner-0.9.80/PKG-INFO
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/clearner.egg-info/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      349 2023-05-18 02:06:19.000000 clearner-0.9.80/clearner.egg-info/PKG-INFO
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3743 2023-05-18 02:06:19.000000 clearner-0.9.80/clearner.egg-info/SOURCES.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        1 2023-05-18 02:06:19.000000 clearner-0.9.80/clearner.egg-info/dependency_links.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       53 2023-05-18 02:06:19.000000 clearner-0.9.80/clearner.egg-info/entry_points.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      706 2023-05-18 02:06:19.000000 clearner-0.9.80/clearner.egg-info/requires.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        9 2023-05-18 02:06:19.000000 clearner-0.9.80/clearner.egg-info/top_level.txt
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       22 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/__init__.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/analysis/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/analysis/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    11442 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/analysis/analysis.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7661 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/analysis/plot.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25711 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/analysis/shap.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/api_worker/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/api_worker/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10480 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/api_worker/google_drive.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/callback_manager/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/callback_manager/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9243 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/callback_manager/callback.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/combine/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/combine/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    36131 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/combine/combining_manager.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/communication/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/communication/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1702 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/communication/communication_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4359 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/communication/email_manager.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/configuration/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/configuration/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17378 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/analysis.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9619 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/column.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5138 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/combine.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3061 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/communication.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5299 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/configuration.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21627 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/connection.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    31721 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/data.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39408 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/defaults.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17803 2023-02-24 19:54:19.000000 clearner-0.9.80/learner/configuration/feature_engineering.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10916 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/model.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14853 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/configuration/outlier.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    26515 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/process.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1078 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/configuration/recommender.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7012 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/sample.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4701 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/segmenter.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      680 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/configuration/similarities.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     8309 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/supported_items.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      739 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/configuration/validation.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2113 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/configuration/workspace.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/data_worker/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/data_worker/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    27945 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/data_worker/data_loader.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15698 2023-02-24 23:02:37.000000 clearner-0.9.80/learner/data_worker/data_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7026 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/data_worker/data_mover.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    52142 2023-04-18 02:21:33.000000 clearner-0.9.80/learner/data_worker/data_processor.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13606 2023-05-18 01:54:31.000000 clearner-0.9.80/learner/data_worker/data_sampler.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23519 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/data_worker/data_segmenters.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13742 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/data_worker/data_set.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    18975 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/data_worker/deep_tabular_data_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7996 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/data_worker/image_data_loader.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10358 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/data_worker/image_data_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3322 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/data_worker/image_processor.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15533 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/data_worker/output_handler.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/engines/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/engines/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10891 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/engines/base_deep_engine.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14624 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/engines/base_standard_engine.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1290 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/engines/deep_classifier.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1341 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/engines/deep_regressor.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1842 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/engines/engine_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7553 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/engines/image_classifier.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21014 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/engines/recommender.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14685 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/engines/standard_engines.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/feature_engineering/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/feature_engineering/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    19542 2023-02-24 19:54:19.000000 clearner-0.9.80/learner/feature_engineering/feature_engineering.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/model_manager/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/model_manager/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12192 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/classifiers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15604 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/deep_classifiers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10955 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/deep_loop_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12048 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/deep_regressors.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6419 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/extenders.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25544 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/image_classifiers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7780 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/layer_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1784 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/loss_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6980 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/model_initializer.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2376 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/nn_utils.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2078 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/optimizer_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39656 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/prediction_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9454 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/regressors.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4802 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/scheduler_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      821 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/model_manager/scorers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23624 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/model_manager/scoring_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2403 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/model_manager/similarities.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/outlier_manager/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/outlier_manager/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7937 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/outlier_manager/outlier_manager.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/schema/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/schema/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      382 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/schema/credentials_schema.json
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      767 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/schema/logging.json
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       19 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/schema/meta_data.schema.json
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10921 2023-02-24 19:54:19.000000 clearner-0.9.80/learner/schema/schema.json
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/setup/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/setup/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6706 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/setup/logger.py
--rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)     2270 2023-02-14 22:39:54.000000 clearner-0.9.80/learner/setup/main.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1346 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/setup/parser.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3204 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/setup/setup.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/utilities/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/utilities/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      955 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/utilities/exclude.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3923 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/utilities/progress_bar.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1218 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/utilities/smtp.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1667 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/utilities/templates.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1333 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/utilities/timer.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-18 02:06:19.000000 clearner-0.9.80/learner/validator/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/validator/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12917 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/validator/column_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5850 2020-12-28 23:50:57.000000 clearner-0.9.80/learner/validator/data_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9262 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/validator/input_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5961 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/validator/model_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2129 2022-08-17 03:32:28.000000 clearner-0.9.80/learner/validator/output_validator.py
--rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)      296 2022-08-17 03:32:28.000000 clearner-0.9.80/main.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      706 2022-10-04 17:17:40.000000 clearner-0.9.80/requirements.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       38 2023-05-18 02:06:19.000000 clearner-0.9.80/setup.cfg
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1830 2023-05-18 02:05:33.000000 clearner-0.9.80/setup.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.913529 clearner-0.9.81/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1993 2022-08-17 03:32:28.000000 clearner-0.9.81/LICENSE
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      361 2023-05-20 02:59:29.913529 clearner-0.9.81/PKG-INFO
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/clearner.egg-info/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      361 2023-05-20 02:59:29.000000 clearner-0.9.81/clearner.egg-info/PKG-INFO
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3743 2023-05-20 02:59:29.000000 clearner-0.9.81/clearner.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        1 2023-05-20 02:59:29.000000 clearner-0.9.81/clearner.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       53 2023-05-20 02:59:29.000000 clearner-0.9.81/clearner.egg-info/entry_points.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      713 2023-05-20 02:59:29.000000 clearner-0.9.81/clearner.egg-info/requires.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        9 2023-05-20 02:59:29.000000 clearner-0.9.81/clearner.egg-info/top_level.txt
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/learner/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       22 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/__init__.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/learner/analysis/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/analysis/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    11442 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/analysis/analysis.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7661 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/analysis/plot.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25940 2023-05-19 23:24:31.000000 clearner-0.9.81/learner/analysis/shap.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/learner/api_worker/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/api_worker/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10480 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/api_worker/google_drive.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/learner/callback_manager/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/callback_manager/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9243 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/callback_manager/callback.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/learner/combine/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/combine/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    36131 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/combine/combining_manager.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/learner/communication/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/communication/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1702 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/communication/communication_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4359 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/communication/email_manager.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.901529 clearner-0.9.81/learner/configuration/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/configuration/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17378 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/analysis.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9619 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/column.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5138 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/combine.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3061 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/communication.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5299 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/configuration.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21627 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/connection.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    31721 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/data.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39408 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/defaults.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17803 2023-02-24 19:54:19.000000 clearner-0.9.81/learner/configuration/feature_engineering.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10916 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/model.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14853 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/configuration/outlier.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    26515 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/process.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1078 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/configuration/recommender.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7012 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/sample.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4701 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/segmenter.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      680 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/configuration/similarities.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     8287 2023-05-19 04:59:05.000000 clearner-0.9.81/learner/configuration/supported_items.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      739 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/configuration/validation.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2113 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/workspace.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.905529 clearner-0.9.81/learner/data_worker/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/data_worker/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    27945 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/data_loader.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15698 2023-02-24 23:02:37.000000 clearner-0.9.81/learner/data_worker/data_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7026 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/data_mover.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    52142 2023-04-18 02:21:33.000000 clearner-0.9.81/learner/data_worker/data_processor.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13606 2023-05-18 01:54:31.000000 clearner-0.9.81/learner/data_worker/data_sampler.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23519 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/data_segmenters.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13742 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/data_set.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    18975 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/deep_tabular_data_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7996 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/image_data_loader.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10358 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/image_data_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3322 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/image_processor.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15533 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/output_handler.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.905529 clearner-0.9.81/learner/engines/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/engines/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10891 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/base_deep_engine.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14624 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/base_standard_engine.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1290 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/deep_classifier.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1341 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/deep_regressor.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1842 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/engine_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7553 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/image_classifier.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21014 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/recommender.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14685 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/standard_engines.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.905529 clearner-0.9.81/learner/feature_engineering/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/feature_engineering/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    19542 2023-02-24 19:54:19.000000 clearner-0.9.81/learner/feature_engineering/feature_engineering.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.909529 clearner-0.9.81/learner/model_manager/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/model_manager/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12192 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/classifiers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15604 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/deep_classifiers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10955 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/deep_loop_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12048 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/deep_regressors.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6419 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/extenders.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25544 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/image_classifiers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7780 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/layer_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1784 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/loss_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6980 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/model_initializer.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2376 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/nn_utils.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2078 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/optimizer_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39656 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/prediction_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9454 2023-05-19 05:22:49.000000 clearner-0.9.81/learner/model_manager/regressors.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4802 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/scheduler_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      821 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/model_manager/scorers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23613 2023-05-19 04:23:21.000000 clearner-0.9.81/learner/model_manager/scoring_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2412 2023-05-19 05:05:51.000000 clearner-0.9.81/learner/model_manager/similarities.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.909529 clearner-0.9.81/learner/outlier_manager/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/outlier_manager/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7937 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/outlier_manager/outlier_manager.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.913529 clearner-0.9.81/learner/schema/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/schema/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      382 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/schema/credentials_schema.json
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      767 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/schema/logging.json
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       19 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/schema/meta_data.schema.json
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10921 2023-02-24 19:54:19.000000 clearner-0.9.81/learner/schema/schema.json
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.913529 clearner-0.9.81/learner/setup/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/setup/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6706 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/setup/logger.py
+-rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)     2270 2023-02-14 22:39:54.000000 clearner-0.9.81/learner/setup/main.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1346 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/setup/parser.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3204 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/setup/setup.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.913529 clearner-0.9.81/learner/utilities/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/utilities/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      955 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/utilities/exclude.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3905 2023-05-19 04:22:17.000000 clearner-0.9.81/learner/utilities/progress_bar.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1218 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/utilities/smtp.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1667 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/utilities/templates.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1333 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/utilities/timer.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.913529 clearner-0.9.81/learner/validator/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/validator/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12917 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/validator/column_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5850 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/validator/data_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9262 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/validator/input_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5961 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/validator/model_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2129 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/validator/output_validator.py
+-rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)      296 2022-08-17 03:32:28.000000 clearner-0.9.81/main.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      713 2023-05-19 23:17:40.000000 clearner-0.9.81/requirements.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       38 2023-05-20 02:59:29.917529 clearner-0.9.81/setup.cfg
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1831 2023-05-20 02:58:24.000000 clearner-0.9.81/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `clearner-0.9.80/LICENSE` & `clearner-0.9.81/LICENSE`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/clearner.egg-info/SOURCES.txt` & `clearner-0.9.81/clearner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/analysis/analysis.py` & `clearner-0.9.81/learner/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/analysis/plot.py` & `clearner-0.9.81/learner/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/analysis/shap.py` & `clearner-0.9.81/learner/analysis/shap.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 sorting, and writing the values as well as creating the narratives and possibly plots. The engines commonly do the
 instantiation and invocation of the classes and methods.
 """
 import pandas as pd
 import numpy as np
 import warnings
 import logging
+from numba.core.errors import NumbaDeprecationWarning, NumbaPendingDeprecationWarning
+warnings.filterwarnings('ignore', category=NumbaDeprecationWarning)
+warnings.filterwarnings('ignore', category=NumbaPendingDeprecationWarning)
 import shap
 from shap.plots._beeswarm import pl
 
 from learner.analysis.plot import Plot
 from learner.utilities.timer import timeit
 from learner.configuration.configuration import Configuration
 from learner.data_worker.output_handler import OutputHandler
```

### Comparing `clearner-0.9.80/learner/api_worker/google_drive.py` & `clearner-0.9.81/learner/api_worker/google_drive.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/callback_manager/callback.py` & `clearner-0.9.81/learner/callback_manager/callback.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/combine/combining_manager.py` & `clearner-0.9.81/learner/combine/combining_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/communication/communication_manager.py` & `clearner-0.9.81/learner/communication/communication_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/communication/email_manager.py` & `clearner-0.9.81/learner/communication/email_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/analysis.py` & `clearner-0.9.81/learner/configuration/analysis.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/column.py` & `clearner-0.9.81/learner/configuration/column.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/combine.py` & `clearner-0.9.81/learner/configuration/combine.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/communication.py` & `clearner-0.9.81/learner/configuration/communication.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/configuration.py` & `clearner-0.9.81/learner/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/connection.py` & `clearner-0.9.81/learner/configuration/connection.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/data.py` & `clearner-0.9.81/learner/configuration/data.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/defaults.py` & `clearner-0.9.81/learner/configuration/defaults.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/feature_engineering.py` & `clearner-0.9.81/learner/configuration/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/model.py` & `clearner-0.9.81/learner/configuration/model.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/outlier.py` & `clearner-0.9.81/learner/configuration/outlier.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/process.py` & `clearner-0.9.81/learner/configuration/process.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/recommender.py` & `clearner-0.9.81/learner/configuration/recommender.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/sample.py` & `clearner-0.9.81/learner/configuration/sample.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/segmenter.py` & `clearner-0.9.81/learner/configuration/segmenter.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/similarities.py` & `clearner-0.9.81/learner/configuration/similarities.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/supported_items.py` & `clearner-0.9.81/learner/configuration/supported_items.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                      "average_precision": "proba",
                      "brier_score_loss": "proba",
                      "classification_report": "class",
                      "confusion_matrix": "class",
                      "f1": "class",
                      "fbeta": "class",
                      "hamming_loss": "class",
-                     "jaccard_similarity": "class",
+                     "jaccard": "class",
                      "log_loss": "proba",
                      "matthews_corrcoef": "class",
                      "precision": "class",
                      "precision_recall_fscore_support": "class",
                      "recall": "class",
                      "roc_auc": "proba",
                      "zero_one_loss": "class"
@@ -111,15 +111,15 @@
 
 deep_classifier_scores = {"accuracy": "class",
                            "average_precision": "proba",
                            "brier_score_loss": "proba",
                            "f1": "class",
                            "fbeta": "class",
                            "hamming_loss": "class",
-                           "jaccard_similarity": "class",
+                           "jaccard": "class",
                            "log_loss": "proba",
                            "matthews_corrcoef": "class",
                            "precision": "class",
                            "recall": "class",
                           "roc_auc": "proba",
                           "zero_one_loss": "class"
                           }
```

### Comparing `clearner-0.9.80/learner/configuration/validation.py` & `clearner-0.9.81/learner/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/configuration/workspace.py` & `clearner-0.9.81/learner/configuration/workspace.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/data_worker/data_loader.py` & `clearner-0.9.81/learner/data_worker/data_loader.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/data_worker/data_manager.py` & `clearner-0.9.81/learner/data_worker/data_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/data_worker/data_mover.py` & `clearner-0.9.81/learner/data_worker/data_mover.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/data_worker/data_processor.py` & `clearner-0.9.81/learner/data_worker/data_processor.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/data_worker/data_sampler.py` & `clearner-0.9.81/learner/data_worker/data_sampler.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/data_worker/data_segmenters.py` & `clearner-0.9.81/learner/data_worker/data_segmenters.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/data_worker/data_set.py` & `clearner-0.9.81/learner/data_worker/data_set.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/data_worker/deep_tabular_data_manager.py` & `clearner-0.9.81/learner/data_worker/deep_tabular_data_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/data_worker/image_data_loader.py` & `clearner-0.9.81/learner/data_worker/image_data_loader.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/data_worker/image_data_manager.py` & `clearner-0.9.81/learner/data_worker/image_data_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/data_worker/image_processor.py` & `clearner-0.9.81/learner/data_worker/image_processor.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/data_worker/output_handler.py` & `clearner-0.9.81/learner/data_worker/output_handler.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/engines/base_deep_engine.py` & `clearner-0.9.81/learner/engines/base_deep_engine.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/engines/base_standard_engine.py` & `clearner-0.9.81/learner/engines/base_standard_engine.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/engines/deep_classifier.py` & `clearner-0.9.81/learner/engines/deep_classifier.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/engines/deep_regressor.py` & `clearner-0.9.81/learner/engines/deep_regressor.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/engines/engine_manager.py` & `clearner-0.9.81/learner/engines/engine_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/engines/image_classifier.py` & `clearner-0.9.81/learner/engines/image_classifier.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/engines/recommender.py` & `clearner-0.9.81/learner/engines/recommender.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/engines/standard_engines.py` & `clearner-0.9.81/learner/engines/standard_engines.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/feature_engineering/feature_engineering.py` & `clearner-0.9.81/learner/feature_engineering/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/classifiers.py` & `clearner-0.9.81/learner/model_manager/classifiers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/deep_classifiers.py` & `clearner-0.9.81/learner/model_manager/deep_classifiers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/deep_loop_manager.py` & `clearner-0.9.81/learner/model_manager/deep_loop_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/deep_regressors.py` & `clearner-0.9.81/learner/model_manager/deep_regressors.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/extenders.py` & `clearner-0.9.81/learner/model_manager/extenders.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/image_classifiers.py` & `clearner-0.9.81/learner/model_manager/image_classifiers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/layer_manager.py` & `clearner-0.9.81/learner/model_manager/layer_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/loss_manager.py` & `clearner-0.9.81/learner/model_manager/loss_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/model_initializer.py` & `clearner-0.9.81/learner/model_manager/model_initializer.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/nn_utils.py` & `clearner-0.9.81/learner/model_manager/nn_utils.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/optimizer_manager.py` & `clearner-0.9.81/learner/model_manager/optimizer_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/prediction_manager.py` & `clearner-0.9.81/learner/model_manager/prediction_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/regressors.py` & `clearner-0.9.81/learner/model_manager/regressors.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/scheduler_manager.py` & `clearner-0.9.81/learner/model_manager/scheduler_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/scorers.py` & `clearner-0.9.81/learner/model_manager/scorers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/model_manager/scoring_manager.py` & `clearner-0.9.81/learner/model_manager/scoring_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 import warnings
 
 import numpy as np
 import pandas as pd
 from sklearn.metrics import accuracy_score, f1_score, average_precision_score, precision_score, recall_score
 from sklearn.metrics import roc_auc_score, brier_score_loss, classification_report, confusion_matrix, fbeta_score
-from sklearn.metrics import hamming_loss, jaccard_similarity_score, log_loss, matthews_corrcoef, precision_recall_curve
+from sklearn.metrics import hamming_loss, jaccard_score, log_loss, matthews_corrcoef, precision_recall_curve
 from sklearn.metrics import precision_recall_fscore_support, zero_one_loss
 from sklearn.metrics import explained_variance_score, mean_absolute_error, mean_squared_error, mean_squared_log_error
 from sklearn.metrics import median_absolute_error, r2_score
 
 from learner.model_manager.scorers import root_mean_squared_error
 from learner.data_worker.data_loader import get_data
 from learner.configuration.supported_items import SUPPORTED_SCORE_TYPES
```

### Comparing `clearner-0.9.80/learner/model_manager/similarities.py` & `clearner-0.9.81/learner/model_manager/similarities.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         Note: the scipy pdist computes the distances. 1 - dist is returned for similarity calculations
         """
         if X.shape[1] < 2:
             logging.error("The input matrix for similarity calculations must have more than 1 columns. Exiting...")
             sys.exit(1)
 
         # Note: transpose is needed to get the correct results
-        matrix = 1 - dist.squareform(dist.pdist(X.T, metric, kwargs))
+        matrix = 1 - dist.squareform(dist.pdist(X.T, metric=metric, **kwargs))
 
         if metric is 'jaccard' and np.array_equal(X, X.astype(bool)) is False:
             logging.error("Non-binary matrix is passed when calculating Jaccard distance."
                           " Make sure the matrix is binarized")
             sys.exit(1)
 
         if return_dataframe and cols is None:
```

### Comparing `clearner-0.9.80/learner/outlier_manager/outlier_manager.py` & `clearner-0.9.81/learner/outlier_manager/outlier_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/schema/logging.json` & `clearner-0.9.81/learner/schema/logging.json`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/schema/schema.json` & `clearner-0.9.81/learner/schema/schema.json`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/setup/logger.py` & `clearner-0.9.81/learner/setup/logger.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/setup/main.py` & `clearner-0.9.81/learner/setup/main.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/setup/parser.py` & `clearner-0.9.81/learner/setup/parser.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/setup/setup.py` & `clearner-0.9.81/learner/setup/setup.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/utilities/exclude.py` & `clearner-0.9.81/learner/utilities/exclude.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/utilities/progress_bar.py` & `clearner-0.9.81/learner/utilities/progress_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Unauthorized copying or use of this file is strictly prohibited and subject to prosecution under applicable laws
 # Proprietary and confidential
 
 import sys
 import time
 from sklearn.model_selection import GridSearchCV
 from sklearn import model_selection
-from sklearn.externals.joblib import Parallel
+from joblib import Parallel
 
 
 # the code adapted from MNE-Python
 class ProgressBar:
     """Generate a command-line progressbar"""
     template = '\r[{0}{1}] {2:.0f}% | {3:.02f} sec | {4} '
```

### Comparing `clearner-0.9.80/learner/utilities/smtp.py` & `clearner-0.9.81/learner/utilities/smtp.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/utilities/templates.py` & `clearner-0.9.81/learner/utilities/templates.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/utilities/timer.py` & `clearner-0.9.81/learner/utilities/timer.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/validator/column_validator.py` & `clearner-0.9.81/learner/validator/column_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/validator/data_validator.py` & `clearner-0.9.81/learner/validator/data_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/validator/input_validator.py` & `clearner-0.9.81/learner/validator/input_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/validator/model_validator.py` & `clearner-0.9.81/learner/validator/model_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/learner/validator/output_validator.py` & `clearner-0.9.81/learner/validator/output_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.80/setup.py` & `clearner-0.9.81/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 def compile_learner():
     """Go through each package and modules, and compile them.
 
     :return: None
     """
     setup(
         name='clearner',
-        version='0.9.80',
+        version='0.9.81',
         description="Learner is a software platform for building production-ready machine learning models without writing any codes.",
         author="Prizmi LLC",
         author_email="contact@prizmi.ai",
-        python_requires='>=3.7,<3.8',
+        python_requires='>=3.8,<3.10',
         url="https://prizmi.ai/learner/home",
         license="Other",
         build_dir="build",
         install_requires=get_dependencies(),
         packages=find_packages(exclude=("tests.*", "tests", "docs.*", "docs")) + ['.'],
         package_data={'learner.schema': ['*.json'],
                       ".": ['requirements.txt', 'LICENSE'],
```

