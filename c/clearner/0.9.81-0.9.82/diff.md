# Comparing `tmp/clearner-0.9.81.tar.gz` & `tmp/clearner-0.9.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clearner-0.9.81.tar", last modified: Sat May 20 02:59:29 2023, max compression
+gzip compressed data, was "clearner-0.9.82.tar", last modified: Mon May 22 19:41:58 2023, max compression
```

## Comparing `clearner-0.9.81.tar` & `clearner-0.9.82.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.913529 clearner-0.9.81/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1993 2022-08-17 03:32:28.000000 clearner-0.9.81/LICENSE
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      361 2023-05-20 02:59:29.913529 clearner-0.9.81/PKG-INFO
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/clearner.egg-info/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      361 2023-05-20 02:59:29.000000 clearner-0.9.81/clearner.egg-info/PKG-INFO
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3743 2023-05-20 02:59:29.000000 clearner-0.9.81/clearner.egg-info/SOURCES.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        1 2023-05-20 02:59:29.000000 clearner-0.9.81/clearner.egg-info/dependency_links.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       53 2023-05-20 02:59:29.000000 clearner-0.9.81/clearner.egg-info/entry_points.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      713 2023-05-20 02:59:29.000000 clearner-0.9.81/clearner.egg-info/requires.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        9 2023-05-20 02:59:29.000000 clearner-0.9.81/clearner.egg-info/top_level.txt
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/learner/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       22 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/__init__.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/learner/analysis/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/analysis/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    11442 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/analysis/analysis.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7661 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/analysis/plot.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25940 2023-05-19 23:24:31.000000 clearner-0.9.81/learner/analysis/shap.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/learner/api_worker/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/api_worker/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10480 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/api_worker/google_drive.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/learner/callback_manager/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/callback_manager/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9243 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/callback_manager/callback.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/learner/combine/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/combine/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    36131 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/combine/combining_manager.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.897529 clearner-0.9.81/learner/communication/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/communication/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1702 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/communication/communication_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4359 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/communication/email_manager.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.901529 clearner-0.9.81/learner/configuration/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/configuration/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17378 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/analysis.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9619 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/column.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5138 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/combine.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3061 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/communication.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5299 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/configuration.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21627 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/connection.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    31721 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/data.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39408 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/defaults.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17803 2023-02-24 19:54:19.000000 clearner-0.9.81/learner/configuration/feature_engineering.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10916 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/model.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14853 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/configuration/outlier.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    26515 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/process.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1078 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/configuration/recommender.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7012 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/sample.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4701 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/segmenter.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      680 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/configuration/similarities.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     8287 2023-05-19 04:59:05.000000 clearner-0.9.81/learner/configuration/supported_items.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      739 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/configuration/validation.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2113 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/configuration/workspace.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.905529 clearner-0.9.81/learner/data_worker/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/data_worker/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    27945 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/data_loader.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15698 2023-02-24 23:02:37.000000 clearner-0.9.81/learner/data_worker/data_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7026 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/data_mover.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    52142 2023-04-18 02:21:33.000000 clearner-0.9.81/learner/data_worker/data_processor.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13606 2023-05-18 01:54:31.000000 clearner-0.9.81/learner/data_worker/data_sampler.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23519 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/data_segmenters.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13742 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/data_set.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    18975 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/deep_tabular_data_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7996 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/image_data_loader.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10358 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/image_data_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3322 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/image_processor.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15533 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/data_worker/output_handler.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.905529 clearner-0.9.81/learner/engines/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/engines/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10891 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/base_deep_engine.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14624 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/base_standard_engine.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1290 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/deep_classifier.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1341 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/deep_regressor.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1842 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/engine_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7553 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/image_classifier.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21014 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/recommender.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14685 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/engines/standard_engines.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.905529 clearner-0.9.81/learner/feature_engineering/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/feature_engineering/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    19542 2023-02-24 19:54:19.000000 clearner-0.9.81/learner/feature_engineering/feature_engineering.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.909529 clearner-0.9.81/learner/model_manager/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/model_manager/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12192 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/classifiers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15604 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/deep_classifiers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10955 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/deep_loop_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12048 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/deep_regressors.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6419 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/extenders.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25544 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/image_classifiers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7780 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/layer_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1784 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/loss_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6980 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/model_initializer.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2376 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/nn_utils.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2078 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/optimizer_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39656 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/prediction_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9454 2023-05-19 05:22:49.000000 clearner-0.9.81/learner/model_manager/regressors.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4802 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/model_manager/scheduler_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      821 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/model_manager/scorers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23613 2023-05-19 04:23:21.000000 clearner-0.9.81/learner/model_manager/scoring_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2412 2023-05-19 05:05:51.000000 clearner-0.9.81/learner/model_manager/similarities.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.909529 clearner-0.9.81/learner/outlier_manager/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/outlier_manager/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7937 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/outlier_manager/outlier_manager.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.913529 clearner-0.9.81/learner/schema/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/schema/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      382 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/schema/credentials_schema.json
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      767 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/schema/logging.json
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       19 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/schema/meta_data.schema.json
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10921 2023-02-24 19:54:19.000000 clearner-0.9.81/learner/schema/schema.json
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.913529 clearner-0.9.81/learner/setup/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/setup/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6706 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/setup/logger.py
--rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)     2270 2023-02-14 22:39:54.000000 clearner-0.9.81/learner/setup/main.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1346 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/setup/parser.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3204 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/setup/setup.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.913529 clearner-0.9.81/learner/utilities/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/utilities/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      955 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/utilities/exclude.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3905 2023-05-19 04:22:17.000000 clearner-0.9.81/learner/utilities/progress_bar.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1218 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/utilities/smtp.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1667 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/utilities/templates.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1333 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/utilities/timer.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-20 02:59:29.913529 clearner-0.9.81/learner/validator/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/validator/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12917 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/validator/column_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5850 2020-12-28 23:50:57.000000 clearner-0.9.81/learner/validator/data_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9262 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/validator/input_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5961 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/validator/model_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2129 2022-08-17 03:32:28.000000 clearner-0.9.81/learner/validator/output_validator.py
--rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)      296 2022-08-17 03:32:28.000000 clearner-0.9.81/main.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      713 2023-05-19 23:17:40.000000 clearner-0.9.81/requirements.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       38 2023-05-20 02:59:29.917529 clearner-0.9.81/setup.cfg
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1831 2023-05-20 02:58:24.000000 clearner-0.9.81/setup.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.419525 clearner-0.9.82/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1993 2022-08-17 03:32:28.000000 clearner-0.9.82/LICENSE
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      361 2023-05-22 19:41:58.415525 clearner-0.9.82/PKG-INFO
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.399525 clearner-0.9.82/clearner.egg-info/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      361 2023-05-22 19:41:58.000000 clearner-0.9.82/clearner.egg-info/PKG-INFO
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3743 2023-05-22 19:41:58.000000 clearner-0.9.82/clearner.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        1 2023-05-22 19:41:58.000000 clearner-0.9.82/clearner.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       53 2023-05-22 19:41:58.000000 clearner-0.9.82/clearner.egg-info/entry_points.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      713 2023-05-22 19:41:58.000000 clearner-0.9.82/clearner.egg-info/requires.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        9 2023-05-22 19:41:58.000000 clearner-0.9.82/clearner.egg-info/top_level.txt
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.399525 clearner-0.9.82/learner/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       22 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/__init__.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.399525 clearner-0.9.82/learner/analysis/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/analysis/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    11442 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/analysis/analysis.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7661 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/analysis/plot.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25940 2023-05-19 23:24:31.000000 clearner-0.9.82/learner/analysis/shap.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.399525 clearner-0.9.82/learner/api_worker/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/api_worker/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10480 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/api_worker/google_drive.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.399525 clearner-0.9.82/learner/callback_manager/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/callback_manager/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9243 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/callback_manager/callback.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.399525 clearner-0.9.82/learner/combine/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/combine/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    36131 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/combine/combining_manager.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.399525 clearner-0.9.82/learner/communication/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/communication/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1702 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/communication/communication_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4359 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/communication/email_manager.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.403525 clearner-0.9.82/learner/configuration/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/configuration/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17378 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/configuration/analysis.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9619 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/configuration/column.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5138 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/configuration/combine.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3061 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/configuration/communication.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5299 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/configuration/configuration.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21627 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/configuration/connection.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    31721 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/configuration/data.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39408 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/configuration/defaults.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17803 2023-02-24 19:54:19.000000 clearner-0.9.82/learner/configuration/feature_engineering.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10916 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/configuration/model.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14853 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/configuration/outlier.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    26515 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/configuration/process.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1078 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/configuration/recommender.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7012 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/configuration/sample.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4701 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/configuration/segmenter.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      680 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/configuration/similarities.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     8287 2023-05-19 04:59:05.000000 clearner-0.9.82/learner/configuration/supported_items.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      739 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/configuration/validation.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2113 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/configuration/workspace.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.407525 clearner-0.9.82/learner/data_worker/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/data_worker/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    27945 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/data_worker/data_loader.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15698 2023-02-24 23:02:37.000000 clearner-0.9.82/learner/data_worker/data_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7026 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/data_worker/data_mover.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    52142 2023-04-18 02:21:33.000000 clearner-0.9.82/learner/data_worker/data_processor.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13606 2023-05-18 01:54:31.000000 clearner-0.9.82/learner/data_worker/data_sampler.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23519 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/data_worker/data_segmenters.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13742 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/data_worker/data_set.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    18975 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/data_worker/deep_tabular_data_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7996 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/data_worker/image_data_loader.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10358 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/data_worker/image_data_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3322 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/data_worker/image_processor.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15533 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/data_worker/output_handler.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.407525 clearner-0.9.82/learner/engines/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/engines/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10891 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/engines/base_deep_engine.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14624 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/engines/base_standard_engine.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1290 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/engines/deep_classifier.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1341 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/engines/deep_regressor.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1842 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/engines/engine_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7553 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/engines/image_classifier.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21014 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/engines/recommender.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14685 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/engines/standard_engines.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.407525 clearner-0.9.82/learner/feature_engineering/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/feature_engineering/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    19542 2023-02-24 19:54:19.000000 clearner-0.9.82/learner/feature_engineering/feature_engineering.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.411525 clearner-0.9.82/learner/model_manager/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/model_manager/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12192 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/model_manager/classifiers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15604 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/model_manager/deep_classifiers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10955 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/model_manager/deep_loop_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12048 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/model_manager/deep_regressors.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6419 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/model_manager/extenders.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25544 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/model_manager/image_classifiers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7780 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/model_manager/layer_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1784 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/model_manager/loss_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6980 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/model_manager/model_initializer.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2376 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/model_manager/nn_utils.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2078 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/model_manager/optimizer_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39656 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/model_manager/prediction_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9454 2023-05-19 05:22:49.000000 clearner-0.9.82/learner/model_manager/regressors.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4802 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/model_manager/scheduler_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      821 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/model_manager/scorers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23613 2023-05-19 04:23:21.000000 clearner-0.9.82/learner/model_manager/scoring_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2412 2023-05-19 05:05:51.000000 clearner-0.9.82/learner/model_manager/similarities.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.411525 clearner-0.9.82/learner/outlier_manager/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/outlier_manager/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7937 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/outlier_manager/outlier_manager.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.415525 clearner-0.9.82/learner/schema/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/schema/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      382 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/schema/credentials_schema.json
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      767 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/schema/logging.json
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       19 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/schema/meta_data.schema.json
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10921 2023-02-24 19:54:19.000000 clearner-0.9.82/learner/schema/schema.json
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.415525 clearner-0.9.82/learner/setup/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/setup/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6706 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/setup/logger.py
+-rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)     2270 2023-02-14 22:39:54.000000 clearner-0.9.82/learner/setup/main.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1346 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/setup/parser.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3204 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/setup/setup.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.415525 clearner-0.9.82/learner/utilities/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/utilities/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      955 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/utilities/exclude.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3905 2023-05-19 04:22:17.000000 clearner-0.9.82/learner/utilities/progress_bar.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1218 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/utilities/smtp.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1667 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/utilities/templates.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1333 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/utilities/timer.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-05-22 19:41:58.415525 clearner-0.9.82/learner/validator/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/validator/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12917 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/validator/column_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5850 2020-12-28 23:50:57.000000 clearner-0.9.82/learner/validator/data_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9262 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/validator/input_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5961 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/validator/model_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2129 2022-08-17 03:32:28.000000 clearner-0.9.82/learner/validator/output_validator.py
+-rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)      296 2022-08-17 03:32:28.000000 clearner-0.9.82/main.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      713 2023-05-22 19:28:15.000000 clearner-0.9.82/requirements.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       38 2023-05-22 19:41:58.419525 clearner-0.9.82/setup.cfg
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1831 2023-05-22 19:41:47.000000 clearner-0.9.82/setup.py
```

### Comparing `clearner-0.9.81/LICENSE` & `clearner-0.9.82/LICENSE`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/clearner.egg-info/SOURCES.txt` & `clearner-0.9.82/clearner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/clearner.egg-info/requires.txt` & `clearner-0.9.82/clearner.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 numpy==1.23
 pandas==1.1.5
 scikit-learn==1.0
 scipy==1.10.1
 tqdm==4.38.0
 dill==0.3.0
 lightgbm==3.1.1
-matplotlib==3.1.0
+matplotlib==3.4.0
 seaborn==0.9.0
 shap==0.41.0
 numba==0.57.0
 valideer==0.4.2
 xgboost==1.3.1
 SQLAlchemy==1.4.0
 cryptography==38.0.4
```

### Comparing `clearner-0.9.81/learner/analysis/analysis.py` & `clearner-0.9.82/learner/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/analysis/plot.py` & `clearner-0.9.82/learner/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/analysis/shap.py` & `clearner-0.9.82/learner/analysis/shap.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/api_worker/google_drive.py` & `clearner-0.9.82/learner/api_worker/google_drive.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/callback_manager/callback.py` & `clearner-0.9.82/learner/callback_manager/callback.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/combine/combining_manager.py` & `clearner-0.9.82/learner/combine/combining_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/communication/communication_manager.py` & `clearner-0.9.82/learner/communication/communication_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/communication/email_manager.py` & `clearner-0.9.82/learner/communication/email_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/analysis.py` & `clearner-0.9.82/learner/configuration/analysis.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/column.py` & `clearner-0.9.82/learner/configuration/column.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/combine.py` & `clearner-0.9.82/learner/configuration/combine.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/communication.py` & `clearner-0.9.82/learner/configuration/communication.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/configuration.py` & `clearner-0.9.82/learner/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/connection.py` & `clearner-0.9.82/learner/configuration/connection.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/data.py` & `clearner-0.9.82/learner/configuration/data.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/defaults.py` & `clearner-0.9.82/learner/configuration/defaults.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/feature_engineering.py` & `clearner-0.9.82/learner/configuration/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/model.py` & `clearner-0.9.82/learner/configuration/model.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/outlier.py` & `clearner-0.9.82/learner/configuration/outlier.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/process.py` & `clearner-0.9.82/learner/configuration/process.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/recommender.py` & `clearner-0.9.82/learner/configuration/recommender.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/sample.py` & `clearner-0.9.82/learner/configuration/sample.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/segmenter.py` & `clearner-0.9.82/learner/configuration/segmenter.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/similarities.py` & `clearner-0.9.82/learner/configuration/similarities.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/supported_items.py` & `clearner-0.9.82/learner/configuration/supported_items.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/validation.py` & `clearner-0.9.82/learner/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/configuration/workspace.py` & `clearner-0.9.82/learner/configuration/workspace.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/data_worker/data_loader.py` & `clearner-0.9.82/learner/data_worker/data_loader.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/data_worker/data_manager.py` & `clearner-0.9.82/learner/data_worker/data_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/data_worker/data_mover.py` & `clearner-0.9.82/learner/data_worker/data_mover.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/data_worker/data_processor.py` & `clearner-0.9.82/learner/data_worker/data_processor.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/data_worker/data_sampler.py` & `clearner-0.9.82/learner/data_worker/data_sampler.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/data_worker/data_segmenters.py` & `clearner-0.9.82/learner/data_worker/data_segmenters.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/data_worker/data_set.py` & `clearner-0.9.82/learner/data_worker/data_set.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/data_worker/deep_tabular_data_manager.py` & `clearner-0.9.82/learner/data_worker/deep_tabular_data_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/data_worker/image_data_loader.py` & `clearner-0.9.82/learner/data_worker/image_data_loader.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/data_worker/image_data_manager.py` & `clearner-0.9.82/learner/data_worker/image_data_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/data_worker/image_processor.py` & `clearner-0.9.82/learner/data_worker/image_processor.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/data_worker/output_handler.py` & `clearner-0.9.82/learner/data_worker/output_handler.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/engines/base_deep_engine.py` & `clearner-0.9.82/learner/engines/base_deep_engine.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/engines/base_standard_engine.py` & `clearner-0.9.82/learner/engines/base_standard_engine.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/engines/deep_classifier.py` & `clearner-0.9.82/learner/engines/deep_classifier.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/engines/deep_regressor.py` & `clearner-0.9.82/learner/engines/deep_regressor.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/engines/engine_manager.py` & `clearner-0.9.82/learner/engines/engine_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/engines/image_classifier.py` & `clearner-0.9.82/learner/engines/image_classifier.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/engines/recommender.py` & `clearner-0.9.82/learner/engines/recommender.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/engines/standard_engines.py` & `clearner-0.9.82/learner/engines/standard_engines.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/feature_engineering/feature_engineering.py` & `clearner-0.9.82/learner/feature_engineering/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/classifiers.py` & `clearner-0.9.82/learner/model_manager/classifiers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/deep_classifiers.py` & `clearner-0.9.82/learner/model_manager/deep_classifiers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/deep_loop_manager.py` & `clearner-0.9.82/learner/model_manager/deep_loop_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/deep_regressors.py` & `clearner-0.9.82/learner/model_manager/deep_regressors.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/extenders.py` & `clearner-0.9.82/learner/model_manager/extenders.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/image_classifiers.py` & `clearner-0.9.82/learner/model_manager/image_classifiers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/layer_manager.py` & `clearner-0.9.82/learner/model_manager/layer_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/loss_manager.py` & `clearner-0.9.82/learner/model_manager/loss_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/model_initializer.py` & `clearner-0.9.82/learner/model_manager/model_initializer.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/nn_utils.py` & `clearner-0.9.82/learner/model_manager/nn_utils.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/optimizer_manager.py` & `clearner-0.9.82/learner/model_manager/optimizer_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/prediction_manager.py` & `clearner-0.9.82/learner/model_manager/prediction_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/regressors.py` & `clearner-0.9.82/learner/model_manager/regressors.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/scheduler_manager.py` & `clearner-0.9.82/learner/model_manager/scheduler_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/scorers.py` & `clearner-0.9.82/learner/model_manager/scorers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/scoring_manager.py` & `clearner-0.9.82/learner/model_manager/scoring_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/model_manager/similarities.py` & `clearner-0.9.82/learner/model_manager/similarities.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/outlier_manager/outlier_manager.py` & `clearner-0.9.82/learner/outlier_manager/outlier_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/schema/logging.json` & `clearner-0.9.82/learner/schema/logging.json`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/schema/schema.json` & `clearner-0.9.82/learner/schema/schema.json`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/setup/logger.py` & `clearner-0.9.82/learner/setup/logger.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/setup/main.py` & `clearner-0.9.82/learner/setup/main.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/setup/parser.py` & `clearner-0.9.82/learner/setup/parser.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/setup/setup.py` & `clearner-0.9.82/learner/setup/setup.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/utilities/exclude.py` & `clearner-0.9.82/learner/utilities/exclude.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/utilities/progress_bar.py` & `clearner-0.9.82/learner/utilities/progress_bar.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/utilities/smtp.py` & `clearner-0.9.82/learner/utilities/smtp.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/utilities/templates.py` & `clearner-0.9.82/learner/utilities/templates.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/utilities/timer.py` & `clearner-0.9.82/learner/utilities/timer.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/validator/column_validator.py` & `clearner-0.9.82/learner/validator/column_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/validator/data_validator.py` & `clearner-0.9.82/learner/validator/data_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/validator/input_validator.py` & `clearner-0.9.82/learner/validator/input_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/validator/model_validator.py` & `clearner-0.9.82/learner/validator/model_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/learner/validator/output_validator.py` & `clearner-0.9.82/learner/validator/output_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.81/requirements.txt` & `clearner-0.9.82/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 numpy==1.23
 pandas==1.1.5
 scikit-learn==1.0
 scipy==1.10.1
 tqdm==4.38.0
 dill==0.3.0
 lightgbm==3.1.1
-matplotlib==3.1.0
+matplotlib==3.4.0
 seaborn==0.9.0
 shap==0.41.0
 numba==0.57.0
 valideer==0.4.2
 xgboost==1.3.1
 SQLAlchemy==1.4.0
 cryptography==38.0.4
```

### Comparing `clearner-0.9.81/setup.py` & `clearner-0.9.82/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def compile_learner():
     """Go through each package and modules, and compile them.
 
     :return: None
     """
     setup(
         name='clearner',
-        version='0.9.81',
+        version='0.9.82',
         description="Learner is a software platform for building production-ready machine learning models without writing any codes.",
         author="Prizmi LLC",
         author_email="contact@prizmi.ai",
         python_requires='>=3.8,<3.10',
         url="https://prizmi.ai/learner/home",
         license="Other",
         build_dir="build",
```

