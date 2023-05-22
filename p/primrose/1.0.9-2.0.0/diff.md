# Comparing `tmp/primrose-1.0.9.tar.gz` & `tmp/primrose-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/primrose-1.0.9.tar", last modified: Fri Jan 10 22:09:53 2020, max compression
+gzip compressed data, was "primrose-2.0.0.tar", last modified: Mon May 22 17:30:36 2023, max compression
```

## Comparing `primrose-1.0.9.tar` & `primrose-2.0.0.tar`

### file list

```diff
@@ -1,189 +1,402 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)      181 2020-01-10 22:08:23.000000 primrose-1.0.9/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      470 2020-01-10 22:08:23.000000 primrose-1.0.9/requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13095 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     5427 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      640 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       52 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    13095 2020-01-10 22:09:53.000000 primrose-1.0.9/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7390 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/base/pipeline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1264 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/base/transformer_sequence.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      248 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/base/reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      426 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/base/postprocess.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1826 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/base/conditional_path_node.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4817 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/base/search_engine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1208 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/base/transformer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      240 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/base/writer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1661 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/base/node.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      382 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/base/success.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5471 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/base/sql_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3618 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/base/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8892 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/data_object.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/dataviz/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1922 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/dataviz/cluster_plotter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/dataviz/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      748 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2525 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/notification_utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/notifications/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3732 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/notifications/success_notification.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/notifications/abstract_notification.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/notifications/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/transformers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2606 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/transformers/sklearn_preprocessing_transformer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6434 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/transformers/categoricals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3520 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/transformers/combine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1907 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/transformers/strings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4816 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/transformers/impute.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/transformers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3124 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/transformers/filter.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3175 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/templates/run_plot_dag.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1918 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/templates/awesome_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2498 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/templates/user_registration_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1583 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/templates/awesome_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/templates/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1988 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/templates/run_primrose.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/cleanup/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1421 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/cleanup/logging_success.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/cleanup/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/readers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3282 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/r_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1824 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/csv_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1342 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/mysql_helper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      560 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/postgres_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1628 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/postgres_helper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2713 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/gcs_dill_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1690 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/sklearn_dataset_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      367 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/database_helper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1544 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/dill_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      508 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/redshift_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5165 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/deserializer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      496 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/oracle_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      528 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/mysql_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1005 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/readers/sqlite_reader.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/configuration/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1823 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/configuration/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19873 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/configuration/configuration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12875 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/configuration/configuration_dag.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/configuration/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12043 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/dag_runner.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/models/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5391 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/models/sklearn_classifier_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/models/sklearn_cluster_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/models/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      970 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/models/sklearn_regression_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8303 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/models/sklearn_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1571 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/models/minimal_search_engine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8347 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/node_factory.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/writers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1430 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/writers/abstract_file_writer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/writers/file_writer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1823 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/writers/csv_writer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3350 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/writers/s3_writer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2562 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/writers/serializer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1582 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/writers/dill_writer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/writers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7932 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/conditionalpath/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1363 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/conditionalpath/simple_switch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/conditionalpath/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/dag/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2710 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/dag/traverser_factory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1162 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/dag/dag_traverser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1843 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/dag/config_layer_traverser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1156 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/dag/depth_first_traverser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/dag/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/primrose/pipelines/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1541 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/pipelines/encode_train_test_split.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8847 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/pipelines/train_test_split.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2777 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/pipelines/dataframe_joiner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2045 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/pipelines/sklearn_preprocessing_pipeline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/primrose/pipelines/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10961 2020-01-10 22:08:23.000000 primrose-1.0.9/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/data/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      444 2020-01-10 22:08:23.000000 primrose-1.0.9/data/tennis.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    11311 2020-01-10 22:08:23.000000 primrose-1.0.9/data/unclustered.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-01-10 22:09:53.000000 primrose-1.0.9/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)      532 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_traverser_factory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2482 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_factory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4028 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_combine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3789 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_csv_writer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2779 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_abstract_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1694 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_sqlite_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15454 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_configuration_dag.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2510 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_postprocess.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2377 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_cluster_plotter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2955 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_s3_writer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1723 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_postgres_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2338 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_sklearn_classifier_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1838 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_notification_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2959 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_config_layer_traverser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1727 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_mysql_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      804 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_configuration_util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1408 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_dill_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      599 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_abstract_transformer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2197 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_r_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2566 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_categoricals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2945 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_encode_train_test_split.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2211 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_dill_writer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1512 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_transformers_strings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_transformers_imputer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1203 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_simple_switch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3202 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_gcs_dill_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4244 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_serializer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      859 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_register_module_classes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_minimal_search_engine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1413 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_logging_success.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11734 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_data_object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1042 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_transformer_sequence.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      322 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      476 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_sklearn_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18837 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_configuration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1043 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_sklearn_dataset_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      638 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_sklearn_preprocessing_pipeline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      245 2020-01-10 22:08:23.000000 primrose-1.0.9/test/ext_node_example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      916 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_mysql_helper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3506 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_abstract_search_engine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1534 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_depth_first_traverser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9997 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_deserializer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3729 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_conditional_path_node.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_sklearn_regression_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2215 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_file_writer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5785 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_abstract_pipeline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      756 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_implicit_categorical_transform.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-10 22:08:23.000000 primrose-1.0.9/test/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4653 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_abstract_sql_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3105 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_success_notification.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4471 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_dataframe_joiner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1287 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_transformer_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      987 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_sklearn_preprocessing_transformer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23896 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_dag_runner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2012 2020-01-10 22:08:23.000000 primrose-1.0.9/test/test_csv_reader.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-10 22:09:53.000000 primrose-1.0.9/config/
--rw-rw-r--   0 travis    (2000) travis    (2000)      245 2020-01-10 22:08:23.000000 primrose-1.0.9/config/example_read_r.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_classifier_predict.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      601 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_read_write.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1477 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_cluster_simple_train.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2456 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_cluster_eval.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2807 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_cluster_train.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1445 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_classifier_predict.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_custom_nodes.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1318 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_regression_train.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      336 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_read_write.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1725 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_classifier_train.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1252 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_classifier_train.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2039 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_regression_train.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2210 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_cluster_simple_train.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      790 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_custom_nodes.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1865 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_cluster_train.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1488 2020-01-10 22:08:23.000000 primrose-1.0.9/config/hello_world_cluster_eval.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1615 2020-01-10 22:09:23.000000 primrose-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.992723 primrose-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-22 17:30:21.000000 primrose-2.0.0/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.932723 primrose-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-22 17:30:21.000000 primrose-2.0.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.936723 primrose-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-22 17:30:21.000000 primrose-2.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-22 17:30:21.000000 primrose-2.0.0/.github/workflows/issues.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-22 17:30:21.000000 primrose-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-22 17:30:21.000000 primrose-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-22 17:30:21.000000 primrose-2.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 17:30:21.000000 primrose-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-22 17:30:21.000000 primrose-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26132 2023-05-22 17:30:36.992723 primrose-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-05-22 17:30:21.000000 primrose-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-22 17:30:21.000000 primrose-2.0.0/README_CLI.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18510 2023-05-22 17:30:21.000000 primrose-2.0.0/README_DAG_CONFIG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-05-22 17:30:21.000000 primrose-2.0.0/README_DATAOBJECT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-05-22 17:30:21.000000 primrose-2.0.0/README_DEVELOPER_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-05-22 17:30:21.000000 primrose-2.0.0/README_GETTING_STARTED.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-22 17:30:21.000000 primrose-2.0.0/README_METADATA.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-22 17:30:21.000000 primrose-2.0.0/README_NOTIFICATIONS.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.936723 primrose-2.0.0/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-22 17:30:21.000000 primrose-2.0.0/config/example_read_r.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_classifier_predict.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_classifier_predict.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_classifier_train.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_classifier_train.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_cluster_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_cluster_eval.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_cluster_simple_train.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_cluster_simple_train.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_cluster_train.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_cluster_train.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_custom_nodes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_custom_nodes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_read_write.json
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_read_write.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_regression_train.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-22 17:30:21.000000 primrose-2.0.0/config/hello_world_regression_train.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.936723 primrose-2.0.0/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      444 2023-05-22 17:30:21.000000 primrose-2.0.0/data/tennis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-05-22 17:30:21.000000 primrose-2.0.0/data/unclustered.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.940723 primrose-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)    29983 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/README.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/README_CLI.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55702 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/README_DAG_CONFIG.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27295 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/README_DATAOBJECT.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27827 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/README_DEVELOPER_NOTES.html
+-rw-r--r--   0 runner    (1001) docker     (123)    41904 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/README_GETTING_STARTED.html
+-rw-r--r--   0 runner    (1001) docker     (123)    30291 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/README_METADATA.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.940723 primrose-2.0.0/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    63424 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_images/clusters.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38455 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_images/conditional_path.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41494 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_images/hw_cluster.png
+-rw-r--r--   0 runner    (1001) docker     (123)   182474 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_images/primrose_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46825 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_images/sections_df.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_images/simple_graph.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.940723 primrose-2.0.0/docs/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/README.md.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/README_CLI.md.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15574 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/README_DAG_CONFIG.md.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/README_DATAOBJECT.md.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/README_DEVELOPER_NOTES.md.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/README_GETTING_STARTED.md.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/README_METADATA.md.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/index.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.928723 primrose-2.0.0/docs/_sources/tmp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.944723 primrose-2.0.0/docs/_sources/tmp/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/base.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/cleanup.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/conditionalpath.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/configuration.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/dag.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/dataviz.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/models.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/modules.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/pipelines.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/primrose.base.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/primrose.cleanup.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/primrose.conditionalpath.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/primrose.configuration.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/primrose.dag.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/primrose.dataviz.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/primrose.models.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/primrose.pipelines.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/primrose.readers.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/primrose.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/primrose.templates.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/primrose.transformers.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/primrose.writers.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/readers.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/transformers.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_sources/tmp/source/writers.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.944723 primrose-2.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/basic.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.948723 primrose-2.0.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/css/badge_only.css
+-rw-r--r--   0 runner    (1001) docker     (123)   118340 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/css/theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/file.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.952723 primrose-2.0.0/docs/_static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   109948 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Inconsolata-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    96964 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Inconsolata-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    63184 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Inconsolata.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.960723 primrose-2.0.0/docs/_static/fonts/Lato/
+-rw-r--r--   0 runner    (1001) docker     (123)   256056 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-bold.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   600856 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   309728 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   184912 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   266158 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-bolditalic.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   622572 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-bolditalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   323344 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-bolditalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   193308 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-bolditalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   268604 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-italic.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   639388 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   328412 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   195704 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   253461 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   607720 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   309192 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   182708 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato/lato-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   656544 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   656568 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/Lato-Regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.960723 primrose-2.0.0/docs/_static/fonts/RobotoSlab/
+-rw-r--r--   0 runner    (1001) docker     (123)    79520 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   170616 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    87624 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    78331 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   169064 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    86288 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   170616 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/RobotoSlab-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   169064 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/RobotoSlab-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   268039 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/jquery-3.2.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86659 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.960723 primrose-2.0.0/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/js/modernizr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35168 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/underscore-1.3.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/_static/underscore.js
+-rw-r--r--   0 runner    (1001) docker     (123)   114292 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/genindex.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.964723 primrose-2.0.0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    63424 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/img/clusters.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38455 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/img/conditional_path.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49147 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/img/hello_world_tennis.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41494 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/img/hw_cluster.png
+-rw-r--r--   0 runner    (1001) docker     (123)   167688 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/img/play_tennis.png
+-rw-r--r--   0 runner    (1001) docker     (123)   182474 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/img/primrose_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46825 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/img/sections_df.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/img/simple_graph.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16855 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)    42116 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)    59349 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.928723 primrose-2.0.0/docs/tmp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.968723 primrose-2.0.0/docs/tmp/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    55096 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/cleanup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/conditionalpath.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15182 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/configuration.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17606 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/dag.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/dataviz.html
+-rw-r--r--   0 runner    (1001) docker     (123)    28544 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/models.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/modules.html
+-rw-r--r--   0 runner    (1001) docker     (123)    25121 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/pipelines.html
+-rw-r--r--   0 runner    (1001) docker     (123)    56437 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/primrose.base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/primrose.cleanup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/primrose.conditionalpath.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35791 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/primrose.configuration.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18040 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/primrose.dag.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/primrose.dataviz.html
+-rw-r--r--   0 runner    (1001) docker     (123)    49270 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/primrose.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29177 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/primrose.models.html
+-rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/primrose.pipelines.html
+-rw-r--r--   0 runner    (1001) docker     (123)    49108 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/primrose.readers.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17350 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/primrose.templates.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32101 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/primrose.transformers.html
+-rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/primrose.writers.html
+-rw-r--r--   0 runner    (1001) docker     (123)    47632 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/readers.html
+-rw-r--r--   0 runner    (1001) docker     (123)    31309 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/transformers.html
+-rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-05-22 17:30:21.000000 primrose-2.0.0/docs/tmp/source/writers.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.968723 primrose-2.0.0/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    63424 2023-05-22 17:30:21.000000 primrose-2.0.0/img/clusters.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38455 2023-05-22 17:30:21.000000 primrose-2.0.0/img/conditional_path.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49147 2023-05-22 17:30:21.000000 primrose-2.0.0/img/hello_world_tennis.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41494 2023-05-22 17:30:21.000000 primrose-2.0.0/img/hw_cluster.png
+-rw-r--r--   0 runner    (1001) docker     (123)   167688 2023-05-22 17:30:21.000000 primrose-2.0.0/img/play_tennis.png
+-rw-r--r--   0 runner    (1001) docker     (123)   182474 2023-05-22 17:30:21.000000 primrose-2.0.0/img/primrose_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46825 2023-05-22 17:30:21.000000 primrose-2.0.0/img/sections_df.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-05-22 17:30:21.000000 primrose-2.0.0/img/simple_graph.png
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-22 17:30:21.000000 primrose-2.0.0/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   360882 2023-05-22 17:30:21.000000 primrose-2.0.0/pdm.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.968723 primrose-2.0.0/primrose/
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.972723 primrose-2.0.0/primrose/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/conditional_path_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/do_nothing_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/search_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/sql_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/success.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/transformer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/base/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.972723 primrose-2.0.0/primrose/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/cleanup/logging_success.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.972723 primrose-2.0.0/primrose/conditionalpath/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/conditionalpath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/conditionalpath/simple_switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.972723 primrose-2.0.0/primrose/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/configuration/configuration_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/configuration/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.972723 primrose-2.0.0/primrose/dag/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/dag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/dag/config_layer_traverser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/dag/dag_traverser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/dag/depth_first_traverser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/dag/traverser_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/dag_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/data_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.972723 primrose-2.0.0/primrose/dataviz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/dataviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/dataviz/cluster_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.976723 primrose-2.0.0/primrose/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/models/minimal_search_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/models/sklearn_classifier_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/models/sklearn_cluster_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/models/sklearn_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/node_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/notification_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.976723 primrose-2.0.0/primrose/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/notifications/abstract_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/notifications/success_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.976723 primrose-2.0.0/primrose/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/pipelines/dataframe_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/pipelines/encode_train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/pipelines/sklearn_preprocessing_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/pipelines/train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/pipelines/transformer_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.976723 primrose-2.0.0/primrose/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/database_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/dill_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/gcs_dill_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/mysql_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/mysql_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/oracle_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/postgres_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/postgres_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/r_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/redshift_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/sklearn_dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/readers/sqlite_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.976723 primrose-2.0.0/primrose/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/templates/awesome_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/templates/awesome_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/templates/run_plot_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/templates/run_primrose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/templates/user_registration_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.980723 primrose-2.0.0/primrose/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/transformers/categoricals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/transformers/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/transformers/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/transformers/impute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/transformers/sklearn_preprocessing_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/transformers/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.980723 primrose-2.0.0/primrose/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/writers/abstract_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/writers/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/writers/dill_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/writers/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/writers/s3_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-22 17:30:21.000000 primrose-2.0.0/primrose/writers/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.968723 primrose-2.0.0/primrose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26132 2023-05-22 17:30:36.000000 primrose-2.0.0/primrose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11785 2023-05-22 17:30:36.000000 primrose-2.0.0/primrose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:30:36.000000 primrose-2.0.0/primrose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-22 17:30:36.000000 primrose-2.0.0/primrose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-22 17:30:36.000000 primrose-2.0.0/primrose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 17:30:36.000000 primrose-2.0.0/primrose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-22 17:30:21.000000 primrose-2.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.980723 primrose-2.0.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-22 17:30:21.000000 primrose-2.0.0/scripts/bump_script.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-22 17:30:21.000000 primrose-2.0.0/scripts/generate_docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-22 17:30:21.000000 primrose-2.0.0/scripts/linux_install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 17:30:21.000000 primrose-2.0.0/scripts/mac_install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:30:36.992723 primrose-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.980723 primrose-2.0.0/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-22 17:30:21.000000 primrose-2.0.0/sphinx/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-22 17:30:21.000000 primrose-2.0.0/sphinx/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:36.992723 primrose-2.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-22 17:30:21.000000 primrose-2.0.0/test/config_substitution.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-22 17:30:21.000000 primrose-2.0.0/test/config_with_comments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-22 17:30:21.000000 primrose-2.0.0/test/ext_node_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-22 17:30:21.000000 primrose-2.0.0/test/hello_world_tennis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-22 17:30:21.000000 primrose-2.0.0/test/hello_world_tennis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-22 17:30:21.000000 primrose-2.0.0/test/merge_right.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 17:30:21.000000 primrose-2.0.0/test/merge_right2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-22 17:30:21.000000 primrose-2.0.0/test/merge_right3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 17:30:21.000000 primrose-2.0.0/test/merge_right4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-22 17:30:21.000000 primrose-2.0.0/test/metadata_fragment.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 17:30:21.000000 primrose-2.0.0/test/metadata_fragment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 17:30:21.000000 primrose-2.0.0/test/minimal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-22 17:30:21.000000 primrose-2.0.0/test/read_write_fragment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-22 17:30:21.000000 primrose-2.0.0/test/read_write_fragment.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      444 2023-05-22 17:30:21.000000 primrose-2.0.0/test/tennis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_abstract_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_abstract_search_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_abstract_sql_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_abstract_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_categoricals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_cluster_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_conditional_path_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_config_layer_traverser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19863 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_configuration_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_configuration_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24013 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_dag_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_data_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_dataframe_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_depth_first_traverser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_dill_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_dill_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_dupe_toplevel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_encode_train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_gcs_dill_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_implicit_categorical_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_logging_success.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_minimal_search_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_mysql_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_mysql_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_notification_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_postgres_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_r_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_register_module_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_s3_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_simple_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_sklearn_classifier_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_sklearn_dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_sklearn_preprocessing_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_sklearn_preprocessing_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_sklearn_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_sqlite_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_success_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_transformer_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_transformer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_transformer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_transformer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_transformers_imputer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_transformers_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_traverser_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-22 17:30:21.000000 primrose-2.0.0/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-22 17:30:21.000000 primrose-2.0.0/test/tinymodel.dill
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-22 17:30:21.000000 primrose-2.0.0/test/tinymodel.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-22 17:30:21.000000 primrose-2.0.0/test/tinymodel_skl_0_24.dill
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-22 17:30:21.000000 primrose-2.0.0/test/tinymodel_skl_0_24.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-22 17:30:21.000000 primrose-2.0.0/test/unclustered.csv
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `primrose-1.0.9/primrose.egg-info/PKG-INFO` & `primrose-2.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,201 +1,211 @@
-Metadata-Version: 2.1
-Name: primrose
-Version: 1.0.9
-Summary: Primrose: a framework for simple, quick modeling deployments
-Home-page: https://github.com/ww-tech/primrose
-Author: Carl Anderson
-Author-email: carl.anderson@weightwatchers.com
-License: Apache 2.0
-Project-URL: Documentation, https://ww-tech.github.io/primrose/
-Project-URL: Source, https://github.com/ww-tech/primrose
-Description: # Overview
-        [![Build Status](https://travis-ci.org/ww-tech/primrose.svg?branch=master)](https://travis-ci.org/ww-tech/primrose)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/primrose.svg)](https://pypi.python.org/pypi/primrose/)
-        [![PyPI version](https://badge.fury.io/py/primrose.svg)](https://badge.fury.io/py/primrose)
-        [![PyPI license](https://img.shields.io/pypi/l/primrose.svg)](https://pypi.python.org/pypi/primrose/)
-        [![Docs status](https://img.shields.io/website/https/ww-tech.github.io/primrose?down_color=red&down_message=docs&label=docs&up_color=success&up_message=up)](https://ww-tech.github.io/primrose/)
-        
-        
-        <p align="center">
-           <img src="img/primrose_logo.png" width="100">
-        </p>
-        
-        ## Primrose at a glance
-        
-        `Primrose` is a simple **Python** framework for executing **in-memory** workflows defined by directed acyclic graphs (**DAGs**) via configuration files. Data in `primrose` flows from one node to another while **avoiding serialization**, except for when explicitly specified by the user. `Primrose` nodes are designed for **simple batch-based machine learning workflows**, which have datasets small enough to fit into a single machine's memory.
-        
-        ## Table of Contents
-        We suggest reading the documentation in the following order:
-        
-         - Overview and motivation for `primrose`&mdash;this file.
-         - [Getting Started](README_GETTING_STARTED.md): run your first `primrose` jobs.
-         - [DAG Configurations](README_DAG_CONFIG.md): `primrose` adopts a configuration-as-code paradigm. This section introduces `primrose` configuration files.
-         - [Metadata](README_METADATA.md): this covers more advanced options of the configuration files.
-         - [Command Line Interface (CLI)](README_CLI.md): run commands using the CLI.
-         - [Developer Notes](README_DEVELOPER_NOTES.md): how to create your own new Node classes.
-         - [DataObject](README_DATAOBJECT.md): a deep dive into `DataObject`, the core data handling and book-keeping object.
-        
-        ## Introduction
-        
-         `Primrose` is a Python framework for quick, simple machine learning and recommender deployments developed by the data science team at [WW](https://www.weightwatchers.com/us/). It is essentially a workflow management tool which is specialized for the needs of machine learning tasks with small to medium sized datasets (&le; 100GB). Like many orchestration tools, `Primrose` *nodes* are defined in a [directed-acyclic-graph](https://en.wikipedia.org/wiki/Directed_acyclic_graph) which defines dependencies and control flow.
-        
-         Here's an example DAG showing data cleaning, model training, and model serialization:
-        
-         <p align="center">
-           <img src="img/hello_world_tennis.png" width="500">
-        </p>
-        
-         It exists within an ecosystem of other great open source workflow management tools (like [Airflow](https://airflow.apache.org/), [Luigi](https://luigi.readthedocs.io/en/stable/), [Kubeflow](https://www.kubeflow.org/docs/about/kubeflow/) or [Prefect](https://docs.prefect.io/guide/)) while carving it's own niche based on the following design goals:
-        
-        1. **Avoid unnecessary serialization:** `Primrose` keeps data in-memory between task steps, and only performs (de)serialization operations when explicitly requested by the user. Data is transported between nodes through use of a `DataObject` abstraction, which contextually delivers the correct data to each `Primrose` node at runtime. As a consequence of this design choice, `Primrose` runs on a single machine and can be deployed as a job within a single container, like any other Python script or cron job. In addition to operating on persistent data passed between nodes, `Primrose` can also be used to call external services in a manner similar to a [Luigi](https://luigi.readthedocs.io/en/stable/) job. In this way, Spark jobs or Hadoop scripts can be called and the framework simply dictates dependencies.
-        
-            * *As a comparison...* many solutions in this space are focused on long-running jobs which may be distributed across several computing nodes. Furthermore, to facilitate parallelization, save states for redundancy, and process datasets which are too large for memory, orchestrators often require that data is serialized between each workflow task. For smaller datasets, the IO time associated with these steps can be much longer than the time spent in computation.
-        
-            * *Primrose is not...* a solution which scales across clusters or a complex dependency management solution with dynamic DAGs (yet).
-        
-        2. **Batch processesing for ML:** `Primrose` was built to facilitate frequent batches of model training or predictions that must read and write from/to multiple sources. Rather than requiring users to define their DAG structure in Python code, `Primrose` adopts a `configuration-as-code` approach. `Primrose` users create implementations of node objects once, then any DAG structural modifications or parameterization changes are processed through configuration json files. This way, deployment changes to DAG operations (such as modifying a DAG to serve model predictions instead of training) can be handled purely through configuration files. This avoids the need to build new Python scripts for production modifications. Furthermore, `Primrose` nodes are based on common machine learning tasks to make data scientist's lives easier. This cuts down on development time for building new models and maximizes code re-use among projects and teams. See the modeling examples in the source and documentation for more info!
-            * *As a comparison...* in `Primrose`, users simply need to specify in their configuration file that they want common ML operations to act on the `DataObject`. These ML operations can certainly be implemented by users in Luigi or Airflow, but we found operations such as test-train splits or classifier cross-validation to be so common that they warranted nodes pre-dedicated to these operations.  [Prefect](https://docs.prefect.io/guide/) has made some great strides in this area, and we encourage users to check their solution out.
-        
-            * *Primrose is not...* an auto-ml tool or machine-learning toolkit which implements its own algorithms. Any Python machine learning library can be used with `Primrose`, simply by building model or pipeline nodes that implement the user's choice of library.
-        
-        3. **Simplicity:**
-        
-            **Standardization of deployments:** `Primrose` is meant to help make deployment and model building as simple as possible. From a developer operations perspective, it requires no external scheduler or cluster to run deployments. `Primrose` code can simply be containerized with a `primrose` Python entrypoint, and deployed as a job on a k8s or any other container management service.
-        
-            **Standardization of development:** From a software engineering perspective, another advantage of `Primrose` stems form the standardization of model and recommender code. Modifying feature engineering pipelines or adding recommender features is simplified by writing additions to self-contained `Primrose` nodes and making additions to a configuration file.
-        
-            * *As a comparison...* `Primrose` can be leveraged as a piece of a larger ETL job (a `Primrose` job could be a job within an Airflow DAG), or run on it's own as a self-contained, single node ETL job. Some orchestration solutions (Airflow, for example) require running persistent clusters and services for managing jobs.
-        
-            * *Primrose is not...* able to manage its own job scheduling or timing. This is left to user using k8s job scheduling or manual cron job assignments on a virtual machine.
-        
-        
-        There are many solutions in this space, and we encourage users to explore other options that may be most appropriate for their workflows. We view `Primrose` as a simple solution for managing production ML jobs.
-        
-        
-        ## Getting Started
-        
-        `Primrose` has a couple of optional tools:
-        * a PostgreSQL database reader
-        * a plotting tool
-        * an R-dataset reader. E.g., to read in R's iris dataset see config/example_read_r.json
-        
-        These require a few external dependencies, prior to its installation. If interested in their functionality, follow the appropriate instructions for your OS below. Otherwise, you can proceed with the basic package installation.
-        
-        ### Installation
-        
-        You can install the latest `Primrose` release via pypi
-        ```
-        pip install primrose
-        ```
-        or you can clone the repository and install via `setup.py`.
-        ```
-        git clone https://github.com/ww-tech/primrose.git
-        cd primrose
-        python setup.py install
-        ```
-        
-        To install the complete `Primrose` package (after dependencies have been installed):
-        ```
-            pip install primrose[postgres, plotting]
-        ```
-        
-        To install `Primrose` with just the PostgreSQL option:
-        
-        ```
-        pip install primrose[postgres]
-        ```
-        
-        To install `primrose` with just the plotting option:
-        
-        ```
-        pip install primrose[plotting]
-        ```
-        
-        To install `primrose` with just the R dataset reading option:
-        
-        ```
-        pip install primrose[R]
-        ```
-        ### External dependenices
-        
-        **PostgreSQL**
-        
-        #### MacOSX
-        
-        We recommend using homebrew to manage OS level external packages. If you do not already have homebrew installed, please visit [their website](https://brew.sh/).
-        
-        Instructions:
-        1. Use homebrew to install `postgresql` library.
-           ```
-           brew install postgresql
-           ```
-        
-        2. Use `pip` to install `psycopg2`
-           ```
-            pip install psycopg2
-           ```
-        
-        #### Debian/Ubuntu
-        
-        Instructions:
-        1. Install the `libpq-dev` library
-           ```
-           apt-get install libpq-dev
-           ```
-        
-        **Plotting**
-        
-        #### MacOSX
-        
-        We recommend using homebrew to manage OS level external packages. If you do not already have homebrew installed, please visit [their website](https://brew.sh/).
-        
-        Instructions:
-        1. Use homebrew to install `graphviz` library.
-           ```
-           brew install graphviz
-           ```
-        2. If you are using a virtual environment such as `Anaconda` or `virtualenv`, you may need to specify a backend for `matplotlib`.
-           ```
-           mkdir -p ~/.matplotlib && touch ~/.matplotlib/matplotlibrc
-           echo backend: TkAgg >> ~/.matplotlib/matplotlibrc
-            ```
-        
-        #### Debian/Ubuntu
-        
-        Instructions:
-        1. Install `graphviz` library.
-           ```
-           apt-get install graphviz
-           ```
-        2. If you are using a virtual environment such as `Anaconda` or `virtualenv`, you may need to specify a backend for `matplotlib`.
-           ```
-           mkdir -p ~/.config/matplotlib && touch ~/.config/matplotlib/matplotlibrc
-           echo backend: Agg >> ~/.config/matplotlib/matplotlibrc
-           ```
-        
-        ## Next
-        You are now ready to run your first `primrose` jobs: [Getting Started](README_GETTING_STARTED.md).
-        
-        ## License
-        Copyright 2019 WW International, Inc.
-        
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-           http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: postgres
-Provides-Extra: plotting
-Provides-Extra: R
-Provides-Extra: all
+# Overview
+[![CI/CD](https://github.com/ww-tech/primrose/actions/workflows/ci.yml/badge.svg)](https://github.com/ww-tech/primrose/actions/workflows/ci.yml)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/primrose.svg)](https://pypi.python.org/pypi/primrose/)
+[![PyPI version](https://badge.fury.io/py/primrose.svg)](https://badge.fury.io/py/primrose)
+[![PyPI license](https://img.shields.io/pypi/l/primrose.svg)](https://pypi.python.org/pypi/primrose/)
+[![Docs status](https://img.shields.io/website/https/ww-tech.github.io/primrose?down_color=red&down_message=docs&label=docs&up_color=success&up_message=up)](https://ww-tech.github.io/primrose/)
+
+
+<p align="center">
+   <img src="img/primrose_logo.png" width="100">
+</p>
+
+## Primrose at a glance
+
+`Primrose` is a simple **Python** framework for executing **in-memory** workflows defined by directed acyclic graphs (**DAGs**) via configuration files. Data in `primrose` flows from one node to another while **avoiding serialization**, except for when explicitly specified by the user. `Primrose` nodes are designed for **simple batch-based machine learning workflows**, which have datasets small enough to fit into a single machine's memory.
+
+## Table of Contents
+We suggest reading the documentation in the following order:
+
+ - Overview and motivation for `primrose`&mdash;this file.
+ - [Getting Started](README_GETTING_STARTED.md): run your first `primrose` jobs.
+ - [DAG Configurations](README_DAG_CONFIG.md): `primrose` adopts a configuration-as-code paradigm. This section introduces `primrose` configuration files.
+ - [Metadata](README_METADATA.md): this covers more advanced options of the configuration files.
+ - [Command Line Interface (CLI)](README_CLI.md): run commands using the CLI.
+ - [Developer Notes](README_DEVELOPER_NOTES.md): how to create your own new Node classes.
+ - [DataObject](README_DATAOBJECT.md): a deep dive into `DataObject`, the core data handling and book-keeping object.
+
+## Introduction
+
+ `Primrose` is a Python framework for quick, simple machine learning and recommender deployments developed by the data science team at [WW](https://www.weightwatchers.com/us/). It is essentially a workflow management tool which is specialized for the needs of machine learning tasks with small to medium sized datasets (&le; 100GB). Like many orchestration tools, `Primrose` *nodes* are defined in a [directed-acyclic-graph](https://en.wikipedia.org/wiki/Directed_acyclic_graph) which defines dependencies and control flow.
+
+ Here's an example DAG showing data cleaning, model training, and model serialization:
+
+ <p align="center">
+   <img src="img/hello_world_tennis.png" width="500">
+</p>
+
+ It exists within an ecosystem of other great open source workflow management tools (like [Airflow](https://airflow.apache.org/), [Luigi](https://luigi.readthedocs.io/en/stable/), [Kubeflow](https://www.kubeflow.org/docs/about/kubeflow/) or [Prefect](https://docs.prefect.io/guide/)) while carving it's own niche based on the following design goals:
+
+1. **Avoid unnecessary serialization:** `Primrose` keeps data in-memory between task steps, and only performs (de)serialization operations when explicitly requested by the user. Data is transported between nodes through use of a `DataObject` abstraction, which contextually delivers the correct data to each `Primrose` node at runtime. As a consequence of this design choice, `Primrose` runs on a single machine and can be deployed as a job within a single container, like any other Python script or cron job. In addition to operating on persistent data passed between nodes, `Primrose` can also be used to call external services in a manner similar to a [Luigi](https://luigi.readthedocs.io/en/stable/) job. In this way, Spark jobs or Hadoop scripts can be called and the framework simply dictates dependencies.
+
+    * *As a comparison...* many solutions in this space are focused on long-running jobs which may be distributed across several computing nodes. Furthermore, to facilitate parallelization, save states for redundancy, and process datasets which are too large for memory, orchestrators often require that data is serialized between each workflow task. For smaller datasets, the IO time associated with these steps can be much longer than the time spent in computation.
+
+    * *Primrose is not...* a solution which scales across clusters or a complex dependency management solution with dynamic DAGs (yet).
+
+2. **Batch processesing for ML:** `Primrose` was built to facilitate frequent batches of model training or predictions that must read and write from/to multiple sources. Rather than requiring users to define their DAG structure in Python code, `Primrose` adopts a `configuration-as-code` approach. `Primrose` users create implementations of node objects once, then any DAG structural modifications or parameterization changes are processed through configuration json files. This way, deployment changes to DAG operations (such as modifying a DAG to serve model predictions instead of training) can be handled purely through configuration files. This avoids the need to build new Python scripts for production modifications. Furthermore, `Primrose` nodes are based on common machine learning tasks to make data scientist's lives easier. This cuts down on development time for building new models and maximizes code re-use among projects and teams. See the modeling examples in the source and documentation for more info!
+    * *As a comparison...* in `Primrose`, users simply need to specify in their configuration file that they want common ML operations to act on the `DataObject`. These ML operations can certainly be implemented by users in Luigi or Airflow, but we found operations such as test-train splits or classifier cross-validation to be so common that they warranted nodes pre-dedicated to these operations.  [Prefect](https://docs.prefect.io/guide/) has made some great strides in this area, and we encourage users to check their solution out.
+
+    * *Primrose is not...* an auto-ml tool or machine-learning toolkit which implements its own algorithms. Any Python machine learning library can be used with `Primrose`, simply by building model or pipeline nodes that implement the user's choice of library.
+
+3. **Simplicity:**
+
+    **Standardization of deployments:** `Primrose` is meant to help make deployment and model building as simple as possible. From a developer operations perspective, it requires no external scheduler or cluster to run deployments. `Primrose` code can simply be containerized with a `primrose` Python entrypoint, and deployed as a job on a k8s or any other container management service.
+
+    **Standardization of development:** From a software engineering perspective, another advantage of `Primrose` stems form the standardization of model and recommender code. Modifying feature engineering pipelines or adding recommender features is simplified by writing additions to self-contained `Primrose` nodes and making additions to a configuration file.
+
+    * *As a comparison...* `Primrose` can be leveraged as a piece of a larger ETL job (a `Primrose` job could be a job within an Airflow DAG), or run on it's own as a self-contained, single node ETL job. Some orchestration solutions (Airflow, for example) require running persistent clusters and services for managing jobs.
+
+    * *Primrose is not...* able to manage its own job scheduling or timing. This is left to user using k8s job scheduling or manual cron job assignments on a virtual machine.
+
+
+There are many solutions in this space, and we encourage users to explore other options that may be most appropriate for their workflows. We view `Primrose` as a simple solution for managing production ML jobs.
+
+
+## Getting Started
+
+`Primrose` has a couple of optional tools:
+* a PostgreSQL database reader
+* a plotting tool
+* an R-dataset reader. E.g., to read in R's iris dataset see config/example_read_r.json
+
+These require a few external dependencies, prior to its installation. If interested in their functionality, follow the appropriate instructions for your OS below. Otherwise, you can proceed with the basic package installation.
+
+### Installation
+
+You can install the latest `Primrose` release via pypi
+```
+pip install primrose
+```
+or you can clone the repository and install via `setup.py`.
+```
+git clone https://github.com/ww-tech/primrose.git
+cd primrose
+python setup.py install
+```
+
+To install the complete `Primrose` package (after dependencies have been installed):
+```
+    pip install primrose[postgres, plotting]
+```
+
+To install `Primrose` with just the PostgreSQL option:
+
+```
+pip install primrose[postgres]
+```
+
+To install `primrose` with just the plotting option:
+
+```
+pip install primrose[plotting]
+```
+
+To install `primrose` with just the R dataset reading option:
+
+```
+pip install primrose[R]
+```
+### External dependenices
+
+**PostgreSQL**
+
+#### MacOSX
+
+We recommend using homebrew to manage OS level external packages. If you do not already have homebrew installed, please visit [their website](https://brew.sh/).
+
+Instructions:
+1. Use homebrew to install `postgresql` library.
+   ```
+   brew install postgresql
+   ```
+
+2. Use `pip` to install `psycopg2`
+   ```
+    pip install psycopg2
+   ```
+
+#### Debian/Ubuntu
+
+Instructions:
+1. Install the `libpq-dev` library
+   ```
+   apt-get install libpq-dev
+   ```
+
+**Plotting**
+
+#### MacOSX
+
+We recommend using homebrew to manage OS level external packages. If you do not already have homebrew installed, please visit [their website](https://brew.sh/).
+
+Instructions:
+1. Use homebrew to install `graphviz` library.
+   ```
+   brew install graphviz
+   ```
+2. If you are using a virtual environment such as `Anaconda` or `virtualenv`, you may need to specify a backend for `matplotlib`.
+   ```
+   mkdir -p ~/.matplotlib && touch ~/.matplotlib/matplotlibrc
+   echo backend: TkAgg >> ~/.matplotlib/matplotlibrc
+    ```
+
+#### Debian/Ubuntu
+
+Instructions:
+1. Install `graphviz` library.
+   ```
+   apt-get install graphviz
+   ```
+2. If you are using a virtual environment such as `Anaconda` or `virtualenv`, you may need to specify a backend for `matplotlib`.
+   ```
+   mkdir -p ~/.config/matplotlib && touch ~/.config/matplotlib/matplotlibrc
+   echo backend: Agg >> ~/.config/matplotlib/matplotlibrc
+   ```
+
+## Next
+You are now ready to run your first `primrose` jobs: [Getting Started](README_GETTING_STARTED.md).
+
+## License
+Copyright 2019 WW International, Inc.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+## Contributing
+To contribute, start a feature branch and install
+[black](https://github.com/psf/black) in your dev environment.
+
+```
+pip install black
+```
+
+
+Black is our python formatter of choice. We have also set up
+[pre-commit](https://pre-commit.com/) hooks to enforce this formatting.
+This means you will get a commit error when you try to commit without
+adhering to our black formatting. Check out these packages for further
+instructions on their usage.
+
+Once you have made your commits, make a PR to master! We have dedicated
+time to review open PRs at least once per week, so we shouldn't miss any
+new PRs.
+
+Please adhere to coding best practices and make sure to do everything in
+the PR template checklist.
+* Write small, modular, reusable, and testable code where possible.
+* Write tests ([pytest](https://docs.pytest.org/en/latest/) or
+  [unittest](https://docs.python.org/3/library/unittest.html)) for that
+  code and make sure it passes (pytest).
+* [Squash your commits](https://github.com/wprig/wprig/wiki/How-to-squash-commits) so that commits are [fewer but more meaningful](https://blog.carbonfive.com/2017/08/28/always-squash-and-rebase-your-git-commits/).
+* Update our [documentation](https://ww-tech.github.io/primrose/).
+That means adhering to our [docstring format](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html) and adding [markdown](https://www.markdownguide.org/) when necessary.
```

### Comparing `primrose-1.0.9/PKG-INFO` & `primrose-2.0.0/docs/_sources/README.md.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,201 +1,176 @@
-Metadata-Version: 2.1
-Name: primrose
-Version: 1.0.9
-Summary: Primrose: a framework for simple, quick modeling deployments
-Home-page: https://github.com/ww-tech/primrose
-Author: Carl Anderson
-Author-email: carl.anderson@weightwatchers.com
-License: Apache 2.0
-Project-URL: Documentation, https://ww-tech.github.io/primrose/
-Project-URL: Source, https://github.com/ww-tech/primrose
-Description: # Overview
-        [![Build Status](https://travis-ci.org/ww-tech/primrose.svg?branch=master)](https://travis-ci.org/ww-tech/primrose)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/primrose.svg)](https://pypi.python.org/pypi/primrose/)
-        [![PyPI version](https://badge.fury.io/py/primrose.svg)](https://badge.fury.io/py/primrose)
-        [![PyPI license](https://img.shields.io/pypi/l/primrose.svg)](https://pypi.python.org/pypi/primrose/)
-        [![Docs status](https://img.shields.io/website/https/ww-tech.github.io/primrose?down_color=red&down_message=docs&label=docs&up_color=success&up_message=up)](https://ww-tech.github.io/primrose/)
-        
-        
-        <p align="center">
-           <img src="img/primrose_logo.png" width="100">
-        </p>
-        
-        ## Primrose at a glance
-        
-        `Primrose` is a simple **Python** framework for executing **in-memory** workflows defined by directed acyclic graphs (**DAGs**) via configuration files. Data in `primrose` flows from one node to another while **avoiding serialization**, except for when explicitly specified by the user. `Primrose` nodes are designed for **simple batch-based machine learning workflows**, which have datasets small enough to fit into a single machine's memory.
-        
-        ## Table of Contents
-        We suggest reading the documentation in the following order:
-        
-         - Overview and motivation for `primrose`&mdash;this file.
-         - [Getting Started](README_GETTING_STARTED.md): run your first `primrose` jobs.
-         - [DAG Configurations](README_DAG_CONFIG.md): `primrose` adopts a configuration-as-code paradigm. This section introduces `primrose` configuration files.
-         - [Metadata](README_METADATA.md): this covers more advanced options of the configuration files.
-         - [Command Line Interface (CLI)](README_CLI.md): run commands using the CLI.
-         - [Developer Notes](README_DEVELOPER_NOTES.md): how to create your own new Node classes.
-         - [DataObject](README_DATAOBJECT.md): a deep dive into `DataObject`, the core data handling and book-keeping object.
-        
-        ## Introduction
-        
-         `Primrose` is a Python framework for quick, simple machine learning and recommender deployments developed by the data science team at [WW](https://www.weightwatchers.com/us/). It is essentially a workflow management tool which is specialized for the needs of machine learning tasks with small to medium sized datasets (&le; 100GB). Like many orchestration tools, `Primrose` *nodes* are defined in a [directed-acyclic-graph](https://en.wikipedia.org/wiki/Directed_acyclic_graph) which defines dependencies and control flow.
-        
-         Here's an example DAG showing data cleaning, model training, and model serialization:
-        
-         <p align="center">
-           <img src="img/hello_world_tennis.png" width="500">
-        </p>
-        
-         It exists within an ecosystem of other great open source workflow management tools (like [Airflow](https://airflow.apache.org/), [Luigi](https://luigi.readthedocs.io/en/stable/), [Kubeflow](https://www.kubeflow.org/docs/about/kubeflow/) or [Prefect](https://docs.prefect.io/guide/)) while carving it's own niche based on the following design goals:
-        
-        1. **Avoid unnecessary serialization:** `Primrose` keeps data in-memory between task steps, and only performs (de)serialization operations when explicitly requested by the user. Data is transported between nodes through use of a `DataObject` abstraction, which contextually delivers the correct data to each `Primrose` node at runtime. As a consequence of this design choice, `Primrose` runs on a single machine and can be deployed as a job within a single container, like any other Python script or cron job. In addition to operating on persistent data passed between nodes, `Primrose` can also be used to call external services in a manner similar to a [Luigi](https://luigi.readthedocs.io/en/stable/) job. In this way, Spark jobs or Hadoop scripts can be called and the framework simply dictates dependencies.
-        
-            * *As a comparison...* many solutions in this space are focused on long-running jobs which may be distributed across several computing nodes. Furthermore, to facilitate parallelization, save states for redundancy, and process datasets which are too large for memory, orchestrators often require that data is serialized between each workflow task. For smaller datasets, the IO time associated with these steps can be much longer than the time spent in computation.
-        
-            * *Primrose is not...* a solution which scales across clusters or a complex dependency management solution with dynamic DAGs (yet).
-        
-        2. **Batch processesing for ML:** `Primrose` was built to facilitate frequent batches of model training or predictions that must read and write from/to multiple sources. Rather than requiring users to define their DAG structure in Python code, `Primrose` adopts a `configuration-as-code` approach. `Primrose` users create implementations of node objects once, then any DAG structural modifications or parameterization changes are processed through configuration json files. This way, deployment changes to DAG operations (such as modifying a DAG to serve model predictions instead of training) can be handled purely through configuration files. This avoids the need to build new Python scripts for production modifications. Furthermore, `Primrose` nodes are based on common machine learning tasks to make data scientist's lives easier. This cuts down on development time for building new models and maximizes code re-use among projects and teams. See the modeling examples in the source and documentation for more info!
-            * *As a comparison...* in `Primrose`, users simply need to specify in their configuration file that they want common ML operations to act on the `DataObject`. These ML operations can certainly be implemented by users in Luigi or Airflow, but we found operations such as test-train splits or classifier cross-validation to be so common that they warranted nodes pre-dedicated to these operations.  [Prefect](https://docs.prefect.io/guide/) has made some great strides in this area, and we encourage users to check their solution out.
-        
-            * *Primrose is not...* an auto-ml tool or machine-learning toolkit which implements its own algorithms. Any Python machine learning library can be used with `Primrose`, simply by building model or pipeline nodes that implement the user's choice of library.
-        
-        3. **Simplicity:**
-        
-            **Standardization of deployments:** `Primrose` is meant to help make deployment and model building as simple as possible. From a developer operations perspective, it requires no external scheduler or cluster to run deployments. `Primrose` code can simply be containerized with a `primrose` Python entrypoint, and deployed as a job on a k8s or any other container management service.
-        
-            **Standardization of development:** From a software engineering perspective, another advantage of `Primrose` stems form the standardization of model and recommender code. Modifying feature engineering pipelines or adding recommender features is simplified by writing additions to self-contained `Primrose` nodes and making additions to a configuration file.
-        
-            * *As a comparison...* `Primrose` can be leveraged as a piece of a larger ETL job (a `Primrose` job could be a job within an Airflow DAG), or run on it's own as a self-contained, single node ETL job. Some orchestration solutions (Airflow, for example) require running persistent clusters and services for managing jobs.
-        
-            * *Primrose is not...* able to manage its own job scheduling or timing. This is left to user using k8s job scheduling or manual cron job assignments on a virtual machine.
-        
-        
-        There are many solutions in this space, and we encourage users to explore other options that may be most appropriate for their workflows. We view `Primrose` as a simple solution for managing production ML jobs.
-        
-        
-        ## Getting Started
-        
-        `Primrose` has a couple of optional tools:
-        * a PostgreSQL database reader
-        * a plotting tool
-        * an R-dataset reader. E.g., to read in R's iris dataset see config/example_read_r.json
-        
-        These require a few external dependencies, prior to its installation. If interested in their functionality, follow the appropriate instructions for your OS below. Otherwise, you can proceed with the basic package installation.
-        
-        ### Installation
-        
-        You can install the latest `Primrose` release via pypi
-        ```
-        pip install primrose
-        ```
-        or you can clone the repository and install via `setup.py`.
-        ```
-        git clone https://github.com/ww-tech/primrose.git
-        cd primrose
-        python setup.py install
-        ```
-        
-        To install the complete `Primrose` package (after dependencies have been installed):
-        ```
-            pip install primrose[postgres, plotting]
-        ```
-        
-        To install `Primrose` with just the PostgreSQL option:
-        
-        ```
-        pip install primrose[postgres]
-        ```
-        
-        To install `primrose` with just the plotting option:
-        
-        ```
-        pip install primrose[plotting]
-        ```
-        
-        To install `primrose` with just the R dataset reading option:
-        
-        ```
-        pip install primrose[R]
-        ```
-        ### External dependenices
-        
-        **PostgreSQL**
-        
-        #### MacOSX
-        
-        We recommend using homebrew to manage OS level external packages. If you do not already have homebrew installed, please visit [their website](https://brew.sh/).
-        
-        Instructions:
-        1. Use homebrew to install `postgresql` library.
-           ```
-           brew install postgresql
-           ```
-        
-        2. Use `pip` to install `psycopg2`
-           ```
-            pip install psycopg2
-           ```
-        
-        #### Debian/Ubuntu
-        
-        Instructions:
-        1. Install the `libpq-dev` library
-           ```
-           apt-get install libpq-dev
-           ```
-        
-        **Plotting**
-        
-        #### MacOSX
-        
-        We recommend using homebrew to manage OS level external packages. If you do not already have homebrew installed, please visit [their website](https://brew.sh/).
-        
-        Instructions:
-        1. Use homebrew to install `graphviz` library.
-           ```
-           brew install graphviz
-           ```
-        2. If you are using a virtual environment such as `Anaconda` or `virtualenv`, you may need to specify a backend for `matplotlib`.
-           ```
-           mkdir -p ~/.matplotlib && touch ~/.matplotlib/matplotlibrc
-           echo backend: TkAgg >> ~/.matplotlib/matplotlibrc
-            ```
-        
-        #### Debian/Ubuntu
-        
-        Instructions:
-        1. Install `graphviz` library.
-           ```
-           apt-get install graphviz
-           ```
-        2. If you are using a virtual environment such as `Anaconda` or `virtualenv`, you may need to specify a backend for `matplotlib`.
-           ```
-           mkdir -p ~/.config/matplotlib && touch ~/.config/matplotlib/matplotlibrc
-           echo backend: Agg >> ~/.config/matplotlib/matplotlibrc
-           ```
-        
-        ## Next
-        You are now ready to run your first `primrose` jobs: [Getting Started](README_GETTING_STARTED.md).
-        
-        ## License
-        Copyright 2019 WW International, Inc.
-        
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-           http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: postgres
-Provides-Extra: plotting
-Provides-Extra: R
-Provides-Extra: all
+# Overview
+[![Build Status](https://travis-ci.org/ww-tech/primrose.svg?branch=master)](https://travis-ci.org/ww-tech/primrose)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/primrose.svg)](https://pypi.python.org/pypi/primrose/)
+[![PyPI version](https://badge.fury.io/py/primrose.svg)](https://badge.fury.io/py/primrose)
+[![PyPI license](https://img.shields.io/pypi/l/primrose.svg)](https://pypi.python.org/pypi/primrose/)
+[![Docs status](https://img.shields.io/website/https/ww-tech.github.io/primrose?down_color=red&down_message=docs&label=docs&up_color=success&up_message=up)](https://ww-tech.github.io/primrose/)
+
+
+<p align="center">
+   <img src="img/primrose_logo.png" width="100">
+</p>
+
+## Primrose at a glance
+
+`Primrose` is a simple **Python** framework for executing **in-memory** workflows defined by directed acyclic graphs (**DAGs**) via configuration files. Data in `primrose` flows from one node to another while **avoiding serialization**, except for when explicitly specified by the user. `Primrose` nodes are designed for **simple batch-based machine learning workflows**, which have datasets small enough to fit into a single machine's memory.
+
+## Table of Contents
+We suggest reading the documentation in the following order:
+
+ - Overview and motivation for `primrose`&mdash;this file.
+ - [Getting Started](README_GETTING_STARTED.md): run your first `primrose` jobs.
+ - [DAG Configurations](README_DAG_CONFIG.md): `primrose` adopts a configuration-as-code paradigm. This section introduces `primrose` configuration files.
+ - [Metadata](README_METADATA.md): this covers more advanced options of the configuration files.
+ - [Command Line Interface (CLI)](README_CLI.md): run commands using the CLI.
+ - [Developer Notes](README_DEVELOPER_NOTES.md): how to create your own new Node classes.
+ - [DataObject](README_DATAOBJECT.md): a deep dive into `DataObject`, the core data handling and book-keeping object.
+
+## Introduction
+
+ `Primrose` is a Python framework for quick, simple machine learning and recommender deployments developed by the data science team at [WW](https://www.weightwatchers.com/us/). It is essentially a workflow management tool which is specialized for the needs of machine learning tasks with small to medium sized datasets (&le; 100GB). Like many orchestration tools, `Primrose` *nodes* are defined in a [directed-acyclic-graph](https://en.wikipedia.org/wiki/Directed_acyclic_graph) which defines dependencies and control flow.
+
+ Here's an example DAG showing data cleaning, model training, and model serialization:
+
+ <p align="center">
+   <img src="img/hello_world_tennis.png" width="500">
+</p>
+
+ It exists within an ecosystem of other great open source workflow management tools (like [Airflow](https://airflow.apache.org/), [Luigi](https://luigi.readthedocs.io/en/stable/), [Kubeflow](https://www.kubeflow.org/docs/about/kubeflow/) or [Prefect](https://docs.prefect.io/guide/)) while carving it's own niche based on the following design goals:
+
+1. **Avoid unnecessary serialization:** `Primrose` keeps data in-memory between task steps, and only performs (de)serialization operations when explicitly requested by the user. Data is transported between nodes through use of a `DataObject` abstraction, which contextually delivers the correct data to each `Primrose` node at runtime. As a consequence of this design choice, `Primrose` runs on a single machine and can be deployed as a job within a single container, like any other Python script or cron job. In addition to operating on persistent data passed between nodes, `Primrose` can also be used to call external services in a manner similar to a [Luigi](https://luigi.readthedocs.io/en/stable/) job. In this way, Spark jobs or Hadoop scripts can be called and the framework simply dictates dependencies.
+
+    * *As a comparison...* many solutions in this space are focused on long-running jobs which may be distributed across several computing nodes. Furthermore, to facilitate parallelization, save states for redundancy, and process datasets which are too large for memory, orchestrators often require that data is serialized between each workflow task. For smaller datasets, the IO time associated with these steps can be much longer than the time spent in computation.
+
+    * *Primrose is not...* a solution which scales across clusters or a complex dependency management solution with dynamic DAGs (yet).
+
+2. **Batch processesing for ML:** `Primrose` was built to facilitate frequent batches of model training or predictions that must read and write from/to multiple sources. Rather than requiring users to define their DAG structure in Python code, `Primrose` adopts a `configuration-as-code` approach. `Primrose` users create implementations of node objects once, then any DAG structural modifications or parameterization changes are processed through configuration json files. This way, deployment changes to DAG operations (such as modifying a DAG to serve model predictions instead of training) can be handled purely through configuration files. This avoids the need to build new Python scripts for production modifications. Furthermore, `Primrose` nodes are based on common machine learning tasks to make data scientist's lives easier. This cuts down on development time for building new models and maximizes code re-use among projects and teams. See the modeling examples in the source and documentation for more info!
+    * *As a comparison...* in `Primrose`, users simply need to specify in their configuration file that they want common ML operations to act on the `DataObject`. These ML operations can certainly be implemented by users in Luigi or Airflow, but we found operations such as test-train splits or classifier cross-validation to be so common that they warranted nodes pre-dedicated to these operations.  [Prefect](https://docs.prefect.io/guide/) has made some great strides in this area, and we encourage users to check their solution out.
+
+    * *Primrose is not...* an auto-ml tool or machine-learning toolkit which implements its own algorithms. Any Python machine learning library can be used with `Primrose`, simply by building model or pipeline nodes that implement the user's choice of library.
+
+3. **Simplicity:**
+
+    **Standardization of deployments:** `Primrose` is meant to help make deployment and model building as simple as possible. From a developer operations perspective, it requires no external scheduler or cluster to run deployments. `Primrose` code can simply be containerized with a `primrose` Python entrypoint, and deployed as a job on a k8s or any other container management service.
+
+    **Standardization of development:** From a software engineering perspective, another advantage of `Primrose` stems form the standardization of model and recommender code. Modifying feature engineering pipelines or adding recommender features is simplified by writing additions to self-contained `Primrose` nodes and making additions to a configuration file.
+
+    * *As a comparison...* `Primrose` can be leveraged as a piece of a larger ETL job (a `Primrose` job could be a job within an Airflow DAG), or run on it's own as a self-contained, single node ETL job. Some orchestration solutions (Airflow, for example) require running persistent clusters and services for managing jobs.
+
+    * *Primrose is not...* able to manage its own job scheduling or timing. This is left to user using k8s job scheduling or manual cron job assignments on a virtual machine.
+
+
+There are many solutions in this space, and we encourage users to explore other options that may be most appropriate for their workflows. We view `Primrose` as a simple solution for managing production ML jobs.
+
+
+## Getting Started
+
+`Primrose` has a couple of optional tools:
+* a postgres database reader
+* a plotting tool
+
+These require a few external dependencies, prior to its installation. If interested in their functionality, follow the appropriate instructions for your OS below. Otherwise, you can proceed with the basic package installation.
+
+### Installation
+
+You can install the latest `Primrose` release via pypi
+```
+pip install primrose
+```
+or you can clone the repository and install via `setup.py`.
+```
+git clone https://github.com/ww-tech/primrose.git
+cd primrose
+python setup.py install
+```
+
+To install the complete `Primrose` package (after dependencies have been installed):
+```
+    pip install primrose[postgres, plotting]
+```
+
+To install `Primrose` with just the postgres option:
+
+```
+pip install primrose[postgres]
+```
+
+To install `primrose` with just the plotting option:
+
+```
+pip install primrose[plotting]
+```
+
+### External dependenices
+
+**Postgres**
+
+#### MacOSX
+
+We recommend using homebrew to manage OS level external packages. If you do not already have homebrew installed, please visit [their website](https://brew.sh/).
+
+Instructions:
+1. Use homebrew to install `postgresql` library.
+   ```
+   brew install postgresql
+   ```
+
+2. Use `pip` to install `psycopg2`
+   ```
+    pip install psycopg2
+   ```
+
+#### Debian/Ubuntu
+
+Instructions:
+1. Install the `libpq-dev` library
+   ```
+   apt-get install libpq-dev
+   ```
+
+**Plotting**
+
+#### MacOSX
+
+We recommend using homebrew to manage OS level external packages. If you do not already have homebrew installed, please visit [their website](https://brew.sh/).
+
+Instructions:
+1. Use homebrew to install `graphviz` library.
+   ```
+   brew install graphviz
+   ```
+2. If you are using a virtual environment such as `Anaconda` or `virtualenv`, you may need to specify a backend for `matplotlib`.
+   ```
+   mkdir -p ~/.matplotlib && touch ~/.matplotlib/matplotlibrc
+   echo backend: TkAgg >> ~/.matplotlib/matplotlibrc
+    ```
+
+#### Debian/Ubuntu
+
+Instructions:
+1. Install `graphviz` library.
+   ```
+   apt-get install graphviz
+   ```
+2. If you are using a virtual environment such as `Anaconda` or `virtualenv`, you may need to specify a backend for `matplotlib`.
+   ```
+   mkdir -p ~/.config/matplotlib && touch ~/.config/matplotlib/matplotlibrc
+   echo backend: Agg >> ~/.config/matplotlib/matplotlibrc
+   ```
+
+## Next
+You are now ready to run your first `primrose` jobs: [Getting Started](README_GETTING_STARTED.md).
+
+## License
+Copyright 2019 WW International, Inc.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `primrose-1.0.9/primrose/base/pipeline.py` & `primrose-2.0.0/primrose/base/pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
     Note:
         FIT = fit data to transformer object only
         TRANSFORM = transform data only from (previously) fit transformers in a pipeline
         FIT_TRANSFORM = fit data then transform data in a pipeline
 
     """
+
     FIT = "FIT"
     FIT_TRANSFORM = "FIT_TRANSFORM"
     TRANSFORM = "TRANSFORM"
 
     @staticmethod
     def names():
         """list of all the names in the enum
@@ -80,23 +81,29 @@
 
         # look for upstream transformer objects
         for source in source_dict:
 
             # NOTE: some readers in primrose have objects nested TransformerSequences one level deeper than others
             # we will allow for this scenario by checking both the first and second level keys for a TransformerSequence
             if isinstance(source_dict[source], TransformerSequence):
-                logging.info('Upstream TransformerSequence found, initializing pipeline...')
+                logging.info(
+                    "Upstream TransformerSequence found, initializing pipeline..."
+                )
                 return source_dict[source]
             elif isinstance(source_dict[source], dict):
                 for subkey in source_dict[source]:
                     if isinstance(source_dict[source][subkey], TransformerSequence):
-                        logging.info('Upstream TransformerSequence found, initializing pipeline...')
+                        logging.info(
+                            "Upstream TransformerSequence found, initializing pipeline..."
+                        )
                         return source_dict[source][subkey]
 
-        logging.info('No upstream TransformerSequence found. Creating new TransformerSequence...')
+        logging.info(
+            "No upstream TransformerSequence found. Creating new TransformerSequence..."
+        )
 
         return self.init_pipeline()
 
     def run(self, data_object):
         """Run pipeline on the data object
 
         Args:
@@ -106,18 +113,20 @@
             (tuple): tuple containing:
 
                 data_object (DataObject): instance of DataObject
 
                 terminate (bool): terminate the DAG?
 
         """
-        is_training = self.node_config.get('is_training', None)
+        is_training = self.node_config.get("is_training", None)
 
         if is_training is None:
-            logging.info('"is_training" key not found in the node_config, assuming production data')
+            logging.info(
+                '"is_training" key not found in the node_config, assuming production data'
+            )
             is_training = False
         else:
             is_training = str(is_training).lower() == "true"
 
         self.transformer_sequence = self.check_for_upstream_transformers(data_object)
 
         if is_training:
@@ -137,15 +146,15 @@
 
         After adding this list, validation automatically occurs before instantiation in the pipeline factory.
 
         Returns:
             set of keys necessary to run implementation
 
         """
-        return set(['is_training']) # pragma: no cover
+        return set(["is_training"])  # pragma: no cover
 
     def fit_transform(self, data_object):
         """Clean/transform or filter data using a pipeline of functions
 
         The method should also cache results and report on sizing for debugging. fit_transform must store the
         information necessary for data transformations on test data, so any encodings or model-based imputations must be
         cached in this method, to be called when the transform method is used.
@@ -170,15 +179,15 @@
         Args:
             data_object (DataObject): DataObject instance
 
         Returns:
             data_object (DataObject)
 
         """
-        return data_object # pragma: no cover
+        return data_object  # pragma: no cover
 
     def init_pipeline(self):
         """Initialize the pipeline if no pipeline object is found in the upstream data objects
 
         Returns:
             TransformerSequence
 
@@ -193,18 +202,20 @@
             mode: enum object for fit, transform, or fit_transform
 
         Returns:
             transformed data (usually a pandas dataframe) after running through all functions in the pipeline
 
         """
         if not self.transformer_sequence:
-            raise Exception("run() must be called to extract/create a TransformerSequence")
-
-        if mode not in PipelineModeType.names() and mode not in PipelineModeType:
-            raise Exception('mode must be of type PipelineModeType Enum object.')
+            raise Exception(
+                "run() must be called to extract/create a TransformerSequence"
+            )
+        
+        if not isinstance(mode, PipelineModeType):
+            raise Exception("mode must be of type PipelineModeType Enum object.")
 
         for transformer in self.transformer_sequence.transformers():
 
             if mode == PipelineModeType.FIT:
 
                 transformer.fit(input_)
```

### Comparing `primrose-1.0.9/primrose/base/transformer_sequence.py` & `primrose-2.0.0/primrose/base/transformer_sequence.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 
 from primrose.base.transformer import AbstractTransformer
 
-class TransformerSequence():
+
+class TransformerSequence:
     """A container for list of transformers"""
 
     def __init__(self, sequence=[]):
         """init a transformer sequence
 
         Args:
             sequence (list of transformers): list of transformers
 
         Returns:
             nothing. Transformers in sequence are added to the internal list
 
         """
         self.sequence = []
-        
+
         for s in sequence:
             self.add(s)
 
     def add(self, transformer):
         """add a transformer to the sequence
 
         Returns:
```

### Comparing `primrose-1.0.9/primrose/base/conditional_path_node.py` & `primrose-2.0.0/primrose/base/conditional_path_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,52 +3,57 @@
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 from abc import abstractmethod
 from primrose.base.node import AbstractNode
 
+
 class AbstractConditionalPath(AbstractNode):
-    """A class that supports conditional pathing through the DAG. 
-    After running, prune() can provide a list of destination nodes, representing start of paths to prune. 
+    """A class that supports conditional pathing through the DAG.
+    After running, prune() can provide a list of destination nodes, representing start of paths to prune.
     DAGRunner can then prune those nodes, and all paths downstream of those nodes, from the DAG"""
 
     def all_nodes_to_prune(self):
         """What are all the nodes we should prune from the DAG?
 
         Note:
-            this call destinations_to_prune() and then uses the DAG to identify 
+            this call destinations_to_prune() and then uses the DAG to identify
             the complete subgraphs starting with those destinations
 
         Returns:
             set of all nodes to prune
 
         """
-        if not 'destinations' in self.node_config:
+        if not "destinations" in self.node_config:
             raise Exception("Destinations key is missing")
 
         destinations_to_prune = self.destinations_to_prune()
 
         if destinations_to_prune:
 
             all_nodes_to_prune = set()
 
             for destination in destinations_to_prune:
-                if not destination in self.node_config['destinations']:
-                    raise Exception("Destination " + destination + " is not in destinations list")
+                if not destination in self.node_config["destinations"]:
+                    raise Exception(
+                        "Destination " + destination + " is not in destinations list"
+                    )
 
                 all_nodes_to_prune.add(destination)
-                all_nodes_to_prune.update(self.configuration.dag.descendents(destination))
+                all_nodes_to_prune.update(
+                    self.configuration.dag.descendents(destination)
+                )
 
             return all_nodes_to_prune
 
         return None
 
     @abstractmethod
     def destinations_to_prune(self):
         """Which destinations, if any, should we prune from DAG?
 
         Returns:
             list of destinations nodes to prune from DAG, None otherwise
 
         """
-        return None # pragma: no cover
+        return None  # pragma: no cover
```

### Comparing `primrose-1.0.9/primrose/base/search_engine.py` & `primrose-2.0.0/primrose/base/search_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from primrose.base.model import AbstractModel
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.metrics.pairwise import cosine_similarity
 from primrose.data_object import DataObjectResponseType
 import pandas as pd
 import logging
 
+
 class AbstractSearchEngine(AbstractModel):
     """an abstract search engine"""
 
     def __init__(self, configuration, instance_name):
         """abstract search engine
 
         Args:
@@ -24,15 +25,15 @@
 
         """
         super(AbstractSearchEngine, self).__init__(configuration, instance_name)
         self.ids = None
         self.docs = None
         self.tfidf = None
         self.term_document_matrix = None
-        self.corpus_key = self.node_config.get('corpus_key','corpus')
+        self.corpus_key = self.node_config.get("corpus_key", "corpus")
 
     @staticmethod
     def necessary_config(node_config):
         """Return a list of necessary configuration keys for AbstractSearchEngine
 
         Args:
             node_config (dict): set of parameters / attributes for the node
@@ -41,55 +42,65 @@
             id_key: key used in the corpus object for ids
             doc_key: key used in the corpus object for docs
 
         Returns:
             set of keys necessary to run AbstractSearchEngine
 
         """
-        return set(['id_key', 'doc_key']).union(AbstractModel.necessary_config(node_config))
+        return set(["id_key", "doc_key"]).union(
+            AbstractModel.necessary_config(node_config)
+        )
 
     def train_model(self, data_object):
         """train the model which means run fit_transform on a TFIDF model
 
         Args:
             data_object (DataObject): instance of DataObject
 
         Returns:
             data_object (DataObject): instance of DataObject
 
         """
 
-        upstream_data = data_object.get_upstream_data(self.instance_name,
-            rtype=DataObjectResponseType.VALUE.value)
+        upstream_data = data_object.get_upstream_data(
+            self.instance_name, rtype=DataObjectResponseType.VALUE.value
+        )
 
         if isinstance(upstream_data, pd.DataFrame):
             corpus = upstream_data
 
         # if a data dict was passed, loop through data objects searching for a corpus dataframe
         elif isinstance(upstream_data, dict):
             for data_key, data in upstream_data.items():
 
                 # check that the data object is a dataframe, if not skip
                 if not isinstance(data, pd.DataFrame):
-                    logging.info("Upstream data from {}.{} not in necessary format, skipping".format(self.instance_name,
-                                                                                                            data_key))
+                    logging.info(
+                        "Upstream data from {}.{} not in necessary format, skipping".format(
+                            self.instance_name, data_key
+                        )
+                    )
                     continue
 
                 if data_key == self.corpus_key:
                     corpus = data
                 else:
-                    logging.info("{} key not found for data entry in upstream {} object, skipping".format(
-                        self.corpus_key, data_key))
+                    logging.info(
+                        "{} key not found for data entry in upstream {} object, skipping".format(
+                            self.corpus_key, data_key
+                        )
+                    )
         else:
-            raise Exception('Search Engine requires a corpus dataframe'.format())
-
+            raise Exception("Search Engine requires a corpus dataframe".format())
 
-        self.ids = list(corpus[self.node_config['id_key']])
-        self.docs = list(corpus[self.node_config['doc_key']])
-        self.tfidf = TfidfVectorizer(tokenizer=self.tokenize,stop_words=None,ngram_range=(1,1))
+        self.ids = list(corpus[self.node_config["id_key"]])
+        self.docs = list(corpus[self.node_config["doc_key"]])
+        self.tfidf = TfidfVectorizer(
+            tokenizer=self.tokenize, stop_words=None, ngram_range=(1, 1)
+        )
         self.term_document_matrix = self.tfidf.fit_transform(self.docs)
 
         return data_object
 
     def eval_model(self, data_object):
         """evaluate the model
 
@@ -128,15 +139,15 @@
             s (str): input string
 
         Returns:
             list of tokens
 
         """
         # this code is essentially unreachable as it has to be overridden in concrete subclass
-        pass # pragma: no cover
+        pass  # pragma: no cover
 
     def cosine_similarity_matrix(self):
         """compute the cosine similarities between all document pairs in the corpus
 
         Returns:
             matrix (numpy): square matrix of cosine similarities where index of matrix is index of corpus IDs
```

### Comparing `primrose-1.0.9/primrose/base/transformer.py` & `primrose-2.0.0/primrose/base/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,48 +5,49 @@
 
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 
 from abc import ABC, abstractmethod
 
+
 class AbstractTransformer(ABC):
     """Serializable object that can be string together within a pipeline"""
 
     @abstractmethod
     def fit(self, data):
         """User implements fit operation on a single data element from a data_object
-        
+
         Args:
             data (object): some data
 
         Returns:
             data
 
         """
-        pass # pragma: no cover
+        pass  # pragma: no cover
 
     @abstractmethod
     def transform(self, data):
         """User implements internal transform function which operates on a single data element from a data_object
-        
+
         Args:
             data (object): input data
 
         Returns:
             data, transformed
 
         """
-        return data # pragma: no cover
+        return data  # pragma: no cover
 
     def fit_transform(self, data):
         """fit then transform data
 
         Args:
             data (object): input data
 
         Returns:
             data, transformed
 
         """
         self.fit(data)
-        return self.transform(data)
+        return self.transform(data)
```

### Comparing `primrose-1.0.9/primrose/base/node.py` & `primrose-2.0.0/primrose/base/node.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-'''Top level notion of a node in the graph
+"""Top level notion of a node in the graph
 
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
-'''
+"""
 from abc import ABC, abstractmethod
 
-class AbstractNode(ABC):
 
+class AbstractNode(ABC):
     def __init__(self, configuration, instance_name):
         """
 
         Args:
             configuration (Configuration): configuration object defined in primrose/Configuration with validated inputs
                 from the result of necessary_config, all inputs are described in that method
 
@@ -33,15 +33,15 @@
         After adding this list, validation automatically occurs before instantiation in the
         configuration
 
         Returns:
             set of keys necessary to run implementation
 
         """
-        return set() # pragma: no cover
+        return set()  # pragma: no cover
 
     @abstractmethod
     def run(self, data_object):
         """
             run the node. For a reader, that means read, for a writer that means write etc.
 
         Args:
@@ -51,8 +51,8 @@
             (tuple): tuple containing:
 
                 data_object (DataObject): instance of DataObject
 
                 terminate (bool): terminate the DAG?
 
         """
-        pass # pragma: no cover
+        pass  # pragma: no cover
```

### Comparing `primrose-1.0.9/primrose/base/sql_reader.py` & `primrose-2.0.0/primrose/base/sql_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from primrose.base.reader import AbstractReader
 from abc import abstractmethod
 import pandas as pd
 import logging
 import hashlib
 from jinja2 import Environment, FileSystemLoader
 
+
 class AbstractSqlReader(AbstractReader):
     """A reader that explicitly reads from relational DB using SQL and is able to run pd.read_sql."""
 
     @staticmethod
     def necessary_config(node_config):
         """Return a list of necessary configuration keys within the implementation
 
@@ -25,22 +26,22 @@
         Note:
             After adding this list, validation automatically occurs before instantiation in the pipeline factory.
 
         Returns:
             set of keys necessary to run implementation
 
         """
-        return set(['query_json']) # pragma: no cover
+        return set(["query_json"])  # pragma: no cover
 
     @staticmethod
     def _substitute_query(query_json):
         """Substitue our paramters in a query string. Renders the file as a jinja template to allow for advanced
-        query nesting and logic. Uses a jinja environment which searches for templates (sql queries) using relative 
+        query nesting and logic. Uses a jinja environment which searches for templates (sql queries) using relative
         path and absolute path.
-        
+
         Note:
             given JSON:
 
             {
                 "query": "somequery.sql",
                 "parameters": {
                     "x": 3,
@@ -55,26 +56,28 @@
 
             This function will read in the SQL file via jinja, and if parameters is present, substitue out the parameters, returning the final query string
 
         Returns:
             query_json (JSON): JSON
 
         """
-        assert 'query' in query_json
-        assert os.path.exists(query_json['query'])
+        assert "query" in query_json
+        assert os.path.exists(query_json["query"])
 
         sql_input = {}
-        if 'parameters' in query_json:
-            sql_input = query_json['parameters']
+        if "parameters" in query_json:
+            sql_input = query_json["parameters"]
 
-        jinja_env = Environment(loader=FileSystemLoader(['.', '/']), 
-                                variable_start_string='{',
-                                variable_end_string='}')
-        
-        query = jinja_env.get_template(query_json['query'])
+        jinja_env = Environment(
+            loader=FileSystemLoader([".", "/"]),
+            variable_start_string="{",
+            variable_end_string="}",
+        )
+
+        query = jinja_env.get_template(query_json["query"])
         return query.render(**sql_input)
 
     def _generate_queries(self):
         """generate final queries, using parameter substitution, if requested
 
         Note:
             query_json should be structured as: \
@@ -98,37 +101,37 @@
 
             This generator will return each query string with variables substituted from parameters (if any) 
 
         Yields:
             query (str): query
 
         """
-        for individual_query_json in self.node_config['query_json']:
+        for individual_query_json in self.node_config["query_json"]:
             yield self._substitute_query(individual_query_json)
 
     def _get_key(self, i):
         """Returns the key name for the ith query in the query_json list. This is the key used when adding the dataframe to the dataobject.
         If none is provided, default to `query_i`
 
         Args:
             i (int): the index of the query
-        
+
         Returns:
             key (str): key name for placement in a `DataObject`
         """
         key = "query_" + str(i)
-        this_query_config = self.node_config['query_json'][i]
+        this_query_config = self.node_config["query_json"][i]
         if "key" in this_query_config.keys():
-            key = this_query_config['key']
+            key = this_query_config["key"]
         return key
 
     @abstractmethod
     def get_connection(self):
         """return a database connection, one that is compatible with pd.read_sql"""
-        pass # pragma: no cover
+        pass  # pragma: no cover
 
     def run(self, data_object):
         """run SQL queries into pandas dataframes
 
         Args:
             data_object (DataObject): instance of DataObject
 
@@ -137,21 +140,21 @@
 
                 data_object (DataObject): instance of DataObject
 
                 terminate (bool): terminate the DAG?
 
         """
         conn = self.get_connection()
-        debug = self.node_config.setdefault('debug',False)
+        debug = self.node_config.setdefault("debug", False)
         for i, query in enumerate(self._generate_queries()):
 
             if debug:
-                with open('debug_query_' + str(i) + '.sql', 'w') as qfile:
+                with open("debug_query_" + str(i) + ".sql", "w") as qfile:
                     qfile.write(os.path.join(query))
-            df = self.query_db(query,conn)
+            df = self.query_db(query, conn)
             key = self._get_key(i)
             logging.info("Adding df with key %s", key)
             data_object.add(self, df, key)
             if df.empty:
                 return data_object, True
 
         terminate = False
```

### Comparing `primrose-1.0.9/primrose/base/model.py` & `primrose-2.0.0/primrose/base/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             data_object (DataObject): instance of DataObject
 
         Returns:
             data_object (DataObject): instance of DataObject
 
         """
 
-        mode = self.node_config['mode'].lower()
+        mode = self.node_config["mode"].lower()
         assert mode in RunModes.values()
 
         if mode == RunModes.TRAIN.value:
             data_object = self.train_model(data_object)
 
         if mode in [RunModes.EVAL.value, RunModes.TRAIN.value]:
             data_object = self.eval_model(data_object)
@@ -50,49 +50,49 @@
         Note:
             After adding this list, validation automatically occurs before instantiation in the pipeline factory.
 
         Returns:
             set of keys necessary to run implementation
 
         """
-        return set(['mode']) # pragma: no cover
+        return set(["mode"])  # pragma: no cover
 
     @abstractmethod
     def train_model(self, data_object):
         """Train an internal model attribute, then save the trained model with the save_model method
 
             Using the training features in feature_df (pandas dataframe object) and the target_variable (pandas series),
             cross-validation or other training scripts will happen in theis method, according to the parameters
             in parameters
 
         Args:
             data_object (DataObject): instance of DataObject
 
-        Returns: 
+        Returns:
             data_object (DataObject): instance of DataObject
 
         """
-        pass # pragma: no cover
+        pass  # pragma: no cover
 
     @abstractmethod
     def eval_model(self, data_object):
         """Evaluate a previously trained model performance using labeled data
 
             Method should be able to load a serialized model if necessary (load_model method), or work from a model
             trained in-scope with the train_model method. This method should calculate and store some aspect of
             model error into attributes that are serialized with the save_model method
 
         Args:
             data_object (DataObject): instance of DataObject
 
-        Returns: 
+        Returns:
             data_object (DataObject): instance of DataObject
 
         """
-        pass # pragma: no cover
+        pass  # pragma: no cover
 
     @abstractmethod
     def predict(self, data_object):
         """Make predictions using a pre-trained model on the features in the feature_df dataframe
 
             Using a pre-trained model (either from an in-scope run of train_model or a call to the load_model method)
             this method should append predictions to each row of features in the input, feature_df. This method may
@@ -105,8 +105,8 @@
             (tuple): tuple containing:
 
                 data_object (DataObject): instance of DataObject
 
                 terminate (bool): terminate the DAG?
 
         """
-        pass # pragma: no cover
+        pass  # pragma: no cover
```

### Comparing `primrose-1.0.9/primrose/data_object.py` & `primrose-2.0.0/primrose/data_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,58 +6,61 @@
 """
 import os
 from collections import defaultdict
 import logging
 from enum import Enum
 import dill
 
+
 class DataObjectResponseType(Enum):
     """Type of object when getting data from DataObject
 
-    INSTANCE_KEY_VALUE = dictionary of instance_name keys and their data dictionaries: 
+    INSTANCE_KEY_VALUE = dictionary of instance_name keys and their data dictionaries:
         {'instance_name': {'key':value}, 'instance_name2': {'key2':value2}, ... }
         e.g. {'corpus_reader': {'data': dataframe}}
         this is useful if there is a set of upstream data arriving from mulitple sources
 
     KEY_VALUE = dictonary of data for given instance name: {'key':value}
         e.g. {'data': dataframe} or {'data': dataframe, 'query': 'select * from table'}
         this is useful if there are multiple keys for a given instance_name
         or if you want to explicitly check against expected keys
 
-    VALUE = value only (for 1st or only instance name and for only key): 
+    VALUE = value only (for 1st or only instance name and for only key):
         e.g. dataframe
         this is useful if you know a node in DAG has only a single upsteam source and only a single
         value. Readers are often a good example as they typically read in and provide a single data frame
 
     """
+
     INSTANCE_KEY_VALUE = "ikv"
     KEY_VALUE = "kv"
     VALUE = "v"
 
     @staticmethod
     def values():
-        ''' list of all the values in the enum'''
+        """ list of all the values in the enum"""
         return list(map(lambda t: t.value, DataObjectResponseType))
 
-class DataObject():
+
+class DataObject:
     """DataObject: a container for "data" (strings, dicts, arbitrary objects etc)"""
 
     # when we are storing some basic data, what is key we use?
-    DATA_KEY = 'data'
+    DATA_KEY = "data"
 
     DEFAULT_RESPONSE_TYPE = DataObjectResponseType.KEY_VALUE.value
 
     def __init__(self, config):
         """instantiate the DataObject
 
         Args:
             config (Configuration): Configuration instance
 
         """
-        #assert isinstance(config, Configuration)
+        # assert isinstance(config, Configuration)
         self.config = config
         self.data_dict = defaultdict(dict)
 
     @staticmethod
     def read_from_cache(filename):
         """restore DatObject from dill-cached file
 
@@ -65,33 +68,33 @@
             filename (str): cache filename
 
         Returns:
             data_object (DataObject): DataObject instance from cache
 
         """
         assert os.path.exists(filename)
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             data_object = dill.load(f)
             assert isinstance(data_object, DataObject)
             return data_object
 
     def write_to_cache(self, filename):
         """write data_object (self) to dill-cache
 
         Returns:
             nothing. Side effect is to cache object to file
 
         """
-        with open(filename, 'wb') as f:
-            logging.info("Cache DataObect to " + filename) 
+        with open(filename, "wb") as f:
+            logging.info("Cache DataObect to " + filename)
             dill.dump(self, f)
 
     def __repr__(self):
         """string representation of the class
-        
+
         Returns:
             string representation
 
         """
         return self.__class__.__name__ + ":" + str(self.data_dict)
 
     def add(self, requestor, data, key=DATA_KEY, overwrite=False):
@@ -102,16 +105,22 @@
             data (object): some object
             key (string): if not supplied default data key is used
 
         Returns:
             nothing.
         """
         assert isinstance(key, str)
-        if not overwrite and requestor.instance_name in self.data_dict and key in self.data_dict[requestor.instance_name]:
-            raise Exception("Key already exists for %s:%s" % (requestor.instance_name, key))
+        if (
+            not overwrite
+            and requestor.instance_name in self.data_dict
+            and key in self.data_dict[requestor.instance_name]
+        ):
+            raise Exception(
+                "Key already exists for %s:%s" % (requestor.instance_name, key)
+            )
 
         # as this is  defaultdict(dict) it should update existing dict with new key
         self.data_dict[requestor.instance_name][key] = data
 
     def get(self, instance_name, pop_data=False, rtype=DEFAULT_RESPONSE_TYPE):
         """get some data from storage, optionally popping it off.
 
@@ -169,73 +178,92 @@
             list of keys, if any
 
         """
         assert instance_name
         keys = self.config.dag.upstream_keys(instance_name)
 
         if operation_type_filter:
-            keys = [k for k in keys if self.config.dag.node_map[k] == operation_type_filter.value]
+            keys = [
+                k
+                for k in keys
+                if self.config.dag.node_map[k] == operation_type_filter.value
+            ]
 
         return keys
 
-    def get_upstream_data(self, instance_name, pop_data=False, rtype=DEFAULT_RESPONSE_TYPE, operation_type_filter=None):
+    def get_upstream_data(
+        self,
+        instance_name,
+        pop_data=False,
+        rtype=DEFAULT_RESPONSE_TYPE,
+        operation_type_filter=None,
+    ):
         """Return data from upstream source(s), choose to pop or not from the dict
 
         Note:
             returns dictionary, where keys are instance_names and each value is a dictionary.
             However, if
             i) there is only 1 upstream key
             and
             ii) value_only=True
             then return the value only.
-            
+
             This option is useful if you expect 1 upstream source only and it returns
             a single artifact, such as a single dataframe. In that case just the dataframe
             is returned
 
         Returns:
             object (type depends on DEFAULT_RESPONSE_TYPE)
 
         Raises:
             Exception if no upstream data found
 
         """
         assert instance_name
-        upstream_keys = self.upstream_keys(instance_name, operation_type_filter=operation_type_filter)
+        upstream_keys = self.upstream_keys(
+            instance_name, operation_type_filter=operation_type_filter
+        )
 
         # While upstream_keys list the upstream sources, it doesn't mean any data were set for them.
         # Thus, we need to see which of these we have data for
-        upstream_keys_with_data = set(upstream_keys).intersection(set(self.data_dict.keys()))
+        upstream_keys_with_data = set(upstream_keys).intersection(
+            set(self.data_dict.keys())
+        )
 
         if not upstream_keys_with_data:
             raise Exception("No upstream keys with data found for %s" % instance_name)
 
         # if there are multiple keys, returning key:value or value makes no sense so ignore rtype
         if len(upstream_keys) > 1:
-            return {iname_key: self.get(iname_key, pop_data) for iname_key in upstream_keys}
+            return {
+                iname_key: self.get(iname_key, pop_data) for iname_key in upstream_keys
+            }
 
         # we must have only 1 key now so this is now simple:
         return self.get(upstream_keys[0], pop_data, rtype)
 
     def get_filtered_upstream_data(self, instance_name, filter_for_key):
         """Upstream data where first level dict keys are first checked for the presence of a filter key
-        
+
         Args:
             instance_name (str): name of instance to look upstream from
 
             filter_for_key (str): the key data was saved with (not instance name but the data value key)
 
         Returns:
             dictionary of stored data for that instance if only one matching dict,
             if more than one valid dictionary then return list of dicts,
             None otherwise
 
         """
-        data = self.get_upstream_data(instance_name, pop_data=False,
-                                        rtype=DataObjectResponseType.INSTANCE_KEY_VALUE.value)
+        data = self.get_upstream_data(
+            instance_name,
+            pop_data=False,
+            rtype=DataObjectResponseType.INSTANCE_KEY_VALUE.value,
+        )
 
         data_to_return = []
 
         for ikey in data:
             if filter_for_key in data[ikey]:
                 data_to_return.append(data[ikey])
```

### Comparing `primrose-1.0.9/primrose/dataviz/cluster_plotter.py` & `primrose-2.0.0/primrose/dataviz/cluster_plotter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 """Module to plot scatter plot of clusters
 
 Author(s): 
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
+import os
+import logging
+
 from primrose.base.node import AbstractNode
 from primrose.data_object import DataObjectResponseType
+import matplotlib as mpl
+
+if os.environ.get("DISPLAY", "") == "":
+    logging.info("no display found. Using non-interactive Agg backend")
+    mpl.use("Agg")
 import matplotlib.pyplot as plt
-import logging
+
 
 class ClusterPlotter(AbstractNode):
     """Plot clusters on a 2D scatter plot"""
 
     @staticmethod
     def necessary_config(node_config):
         """Returns the necessary configuration keys for the ClusterPlotter object
 
         Note:
             id_col (str): name of column with cluster IDs
             filename (str): name of the file
 
-        Returns: 
+        Returns:
             set of necessary keys for the CsvReader object
 
         """
-        return set(['id_col', 'filename'])
+        return set(["id_col", "filename"])
 
     def run(self, data_object):
         """Create a PNG image of the clustered data
 
         Note:
             saves image to file specified in filename key
             optional key: `title` which is title of plot
 
         Returns:
             data_object (DataObject): DataObject instance. Here, it is unmodified
             terminate (bool): should we terminate the DAG? true or false. Terminate if empty data
 
         """
-        dat = data_object.get_upstream_data(self.instance_name, pop_data=False, rtype=DataObjectResponseType.KEY_VALUE.value)
-        X = dat['data']
-        cluster_ids = X[self.node_config['id_col']]
-        centers = X.groupby(self.node_config['id_col']).mean()
-        del X[self.node_config['id_col']]
+        dat = data_object.get_upstream_data(
+            self.instance_name, pop_data=False, rtype=DataObjectResponseType.KEY_VALUE.value,
+        )
+        X = dat["data"]
+        cluster_ids = X[self.node_config["id_col"]]
+        centers = X.groupby(self.node_config["id_col"]).mean()
 
-        plt.scatter(X.iloc[:,0],X.iloc[:,1], c=cluster_ids, s=50, cmap='viridis')
-        plt.scatter(centers.iloc[:,0], centers.iloc[:,1], c='black', s=200, alpha=0.5)
+        plt.scatter(X.iloc[:, 0], X.iloc[:, 1], c=cluster_ids, s=50, cmap="viridis")
+        plt.scatter(centers.iloc[:, 0], centers.iloc[:, 1], c="black", s=200, alpha=0.5)
 
-        if self.node_config['title']:
-            plt.title(self.node_config['title'])
+        if self.node_config["title"]:
+            plt.title(self.node_config["title"])
 
-        plt.savefig(self.node_config['filename'])
-        logging.info("Saved cluster plot to " + self.node_config['filename'])
+        plt.savefig(self.node_config["filename"])
+        logging.info("Saved cluster plot to " + self.node_config["filename"])
 
         terminate = X.empty
         return data_object, terminate
```

### Comparing `primrose-1.0.9/primrose/util.py` & `primrose-2.0.0/primrose/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,21 @@
     Michael Skarlinski (michael.skarlinski@weightwatchers.com)
 
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 from enum import Enum
 
+
 class RunModes(Enum):
     """set of operation type identifiers"""
-    TRAIN = 'train'
-    PREDICT = 'predict'
-    EVAL = 'eval'
+
+    TRAIN = "train"
+    PREDICT = "predict"
+    EVAL = "eval"
 
     @staticmethod
     def names():
         """list of all the names in the enum
 
         Returns:
             list of Enum's names
```

### Comparing `primrose-1.0.9/primrose/notification_utils.py` & `primrose-2.0.0/primrose/notification_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,20 +64,28 @@
         params (`dict`): parameters for client instantiation
         (example. {'client': 'SlackClient', 'channel': 'my_channel', 'token': 'some-token'})
 
     Returns:
         instantiated client object
 
     """
-    exclude = ["class", "client", "message", "destinations"]
+    exclude = [
+        "class",
+        "client",
+        "message",
+        "destinations",
+        "use_configuration_file_message",
+        "node_name",
+        "message_key",
+    ]
     client_params = {k: v for k, v in params.items() if k not in exclude}
 
     # instantiate client
     module = importlib.import_module(__loader__.name)
     try:
         client = getattr(module, params["client"])
 
         return client(**client_params)
 
-    except AttributeError as error:
+    except AttributeError:
         msg = "Are you sure {} is in {}?".format(params["client"], module)
-        logging.error(msg, error)
+        logging.exception(msg)
```

### Comparing `primrose-1.0.9/primrose/notifications/success_notification.py` & `primrose-2.0.0/primrose/notifications/success_notification.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,62 +7,64 @@
 """
 
 import importlib
 import os
 import logging
 
 from primrose.base.success import AbstractSuccess
+from primrose.data_object import DataObjectResponseType
 
 from primrose.notification_utils import get_notification_client
 
 
-
 def get_client_params(params: dict):
     """
-        Creates the parameter dictionary to be read by the
-        `get_notification_client` method.
+    Creates the parameter dictionary to be read by the
+    `get_notification_client` method.
 
-        Args:
-            params (`dict`): The parameter dictionary where keys are
-                - the primrose `client` (required key),
-                - neccessary arguments to instantiate the client
-                - the `message` if used in the `implementation` section of the DAG.
-
-                Values can be explicitly or stored as environment variables.
-                Environment variables are stored as {CLIENT_NAME}_{CLIENT_KEY}.
-
-                For example, using the built-in SlackClient, environment variables
-                will be stored as:
-                    SLACKCLIENT_TOKEN="some-token"
-                    SLACKCLIENT_CHANNEL="some-channel"
-                    SLACKCLIENT_MEMBER_ID="USomeUserID"
+    Args:
+        params (`dict`): The parameter dictionary where keys are
+            - the primrose `client` (required key),
+            - neccessary arguments to instantiate the client
+            - the `message` if used in the `implementation` section of the DAG.
+
+            Values can be explicitly or stored as environment variables.
+            Environment variables are stored as {CLIENT_NAME}_{CLIENT_KEY}.
+
+            For example, using the built-in SlackClient, environment variables
+            will be stored as:
+                SLACKCLIENT_TOKEN="some-token"
+                SLACKCLIENT_CHANNEL="some-channel"
+                SLACKCLIENT_MEMBER_ID="USomeUserID"
 
-        Returns:
-            A `dict` with the key-value pairs necessary to be read by the
-            `get_notification_client` method.
+    Returns:
+        A `dict` with the key-value pairs necessary to be read by the
+        `get_notification_client` method.
 
-        Example:
-            >>> node_config = {
-                    "client": "SlackClient",
-                    "message": "starting job...",
-                }
-            >>> get_client_params(node_config)
-            {'client': 'SlackClient',
-            'channel': 'some-channel',
-            'message': 'starting job...',
-            'token': 'some-token',
-            'member_id': 'USomeUserID'
+    Example:
+        >>> node_config = {
+                "client": "SlackClient",
+                "message": "starting job...",
             }
+        >>> get_client_params(node_config)
+        {'client': 'SlackClient',
+        'channel': 'some-channel',
+        'message': 'starting job...',
+        'token': 'some-token',
+        'member_id': 'USomeUserID'
+        }
 
     """
-    client = params['client'].upper()
+    client = params["client"].upper()
     env_var = {
-        k.split(f'{client}_')[-1].lower(): v for k, v in os.environ.items()
+        k.split(f"{client}_")[-1].lower(): v
+        for k, v in os.environ.items()
         if client.upper() in k
-        and k.split(f'{client}_')[-1].lower() not in params.keys() # config params take precedence
+        and k.split(f"{client}_")[-1].lower()
+        not in params.keys()  # config params take precedence
     }
 
     # combine environment variables and params
     return {**params, **env_var}
 
 
 class ClientNotification(AbstractSuccess):
@@ -77,37 +79,91 @@
 
         Returns:
             None
 
         """
         super().__init__(configuration, instance_name)
         self.message = self.node_config.get("message", "SUCCESS! DAG Completed")
+        self.use_configuration_file_message = self.node_config.get(
+            "use_configuration_file_message", True
+        )
+        self.node_name = self.node_config.get("node_name", "")
+        self.message_key = self.node_config.get("message_key", "")
 
         # read from config dict or environment variables
-        self.client = get_notification_client(params=get_client_params(self.node_config))
+        self.client = get_notification_client(
+            params=get_client_params(self.node_config)
+        )
 
     @staticmethod
     def necessary_config(node_config):
         """Returns the necessary configuration keys for the ClientNotification object
 
-            Notes:
-                client (`str`): The client object to be instantiated (ex. 'SlackClient')
-                token (`str`): The token used to initialize the client
+        Notes:
+            client (`str`): The client object to be instantiated (ex. 'SlackClient')
+            token (`str`): The token used to initialize the client
 
         """
         config_params = set(["client", "token"])
         return config_params.union(AbstractSuccess.necessary_config(node_config))
 
+    @staticmethod
+    def optional_config(node_config):
+        """Returns the optional configuration keys
+
+        Args:
+            node_config (dict): set of parameters for the node
+
+        optional keys:
+            use_configuration_file_message(bool): True if you want the slack client to send message from
+            configuration file. This is the default behavior. If you set it to false
+            pass the next two parameters to send alternate message passed from another node.
+
+            node_name(str): the name of the node where this module will find the message to
+            post
+
+            message_key(str): the key in the node that should be used for getting the message
+        Returns:
+            Set of optional keys for the pipeline object
+        """
+        return set(
+            [
+                "use_config_message",
+                "node_name",
+                "message_key",
+            ]
+        )
+
     def run(self, data_object):
         """
-            Run job to post slack message
+        Run job to post slack message
 
-            Args:
-                data_object (`DataObject`): primrose data object instance
-                terminate (`bool`). Should we terminate the DAG? True or False
+        Args:
+            data_object (`DataObject`): primrose data object instance
+            terminate (`bool`). Should we terminate the DAG? True or False
 
         """
+
+        if not self.use_configuration_file_message:
+            logging.info("Posting message passed by a node")
+
+            if self.node_name and self.message_key:
+                upstream_data = data_object.get_upstream_data(
+                    self.instance_name,
+                    pop_data=False,
+                    rtype=DataObjectResponseType.INSTANCE_KEY_VALUE.value,
+                )
+
+                self.message = upstream_data[self.node_name][self.message_key]
+            else:
+                logging.info(
+                    """Do not have adequate information to retrieve message from
+                                an upstream node; reverting to default behavior.
+                                If you want to post message from an upstream node, provide
+                                values for node_name and message_key """
+                )
+
         # execute response
         _ = self.client.post_message(message=self.message)
 
         terminate = False
         return data_object, terminate
```

### Comparing `primrose-1.0.9/primrose/transformers/sklearn_preprocessing_transformer.py` & `primrose-2.0.0/primrose/transformers/sklearn_preprocessing_transformer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,58 @@
 """primrose wrapper around sklearn preprocessor
 
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
+    Brian Graham (brian.graham@ww.com)
 
 """
+import importlib
 import logging
 import pandas as pd
 
 from primrose.base.transformer import AbstractTransformer
 
-class SklearnPreprocessingTransformer(AbstractTransformer):
 
-    def __init__(self, preprocessor, columns):
+class SklearnPreprocessingTransformer(AbstractTransformer):
+    def __init__(self, preprocessor, columns, args=None):
         """initialize the proprocessor
 
         Args:
-            preprocessor (SKlearn preprocessor): preprocesor from Sklearn
+            preprocessor (SKlearn preprocessor or str specifying the preprocessor): preprocesor from Sklearn
             columns (list of str): list of columns
 
         """
-        #Ideally, would check that this is a preprocessor but there is no good class to check against
-        self.preprocessor = preprocessor
+        # Ideally, would check that this is a preprocessor but there is no good class to check against
+        self.preprocessor = self._instantiate_preprocessor(preprocessor, args)
         self.columns = columns
 
+    def _instantiate_preprocessor(self, preprocessor, args):
+        if isinstance(preprocessor, str):
+            sk_module_name, sk_transformer_name = preprocessor.split(".")
+            sk_module = importlib.import_module("sklearn.{}".format(sk_module_name))
+
+            try:
+                t = getattr(sk_module, sk_transformer_name)
+            except AttributeError:
+                raise Exception(
+                    "Preprocessor {} not found in {} module".format(
+                        sk_transformer_name, sk_module_name
+                    )
+                )
+
+            if args:
+                return t(**args)
+
+            return t()
+
+        return preprocessor
+
     def fit(self, data):
         """User implements fit operation on a single data element from a data_object
-        
+
         Args:
             data (object): some data
 
         Returns:
             data
 
         """
@@ -39,37 +62,41 @@
             else:
                 self.preprocessor.fit(data.values)
         else:
             self.preprocessor.fit(data)
 
     def transform(self, data):
         """User implements internal transform function which operates on a single data element from a data_object
-        
+
         Args:
             data (object): input data
 
         Returns:
             data, transformed
 
         """
         if isinstance(data, pd.DataFrame):
             if self.columns:
                 scaled_features_df = data.copy()
 
                 # transform select columns
                 scaled_features = self.preprocessor.transform(data[self.columns].values)
                 for idx, colname in enumerate(self.columns):
-                    scaled_features_df[colname] = scaled_features[:,idx]
+                    scaled_features_df[colname] = scaled_features[:, idx]
 
             else:
                 scaled_features = self.preprocessor.transform(data.values)
                 try:
-                    scaled_features_df = pd.DataFrame(scaled_features, index=data.index, columns=data.columns)
+                    scaled_features_df = pd.DataFrame(
+                        scaled_features, index=data.index, columns=data.columns
+                    )
                 except ValueError:
-                    logging.info(f'{self.preprocessor.__class__.__name__} instance changed the number of columns. Returning raw values')
+                    logging.info(
+                        f"{self.preprocessor.__class__.__name__} instance changed the number of columns. Returning raw values"
+                    )
                     return pd.DataFrame(scaled_features)
             return scaled_features_df
 
         return self.preprocessor.transform(data)
 
     def fit_transform(self, data):
         """fit then transform data
@@ -78,8 +105,8 @@
             data (data): input data
 
         Returns:
             data, transformed
 
         """
         self.fit(data)
-        return self.transform(data)
+        return self.transform(data)
```

### Comparing `primrose-1.0.9/primrose/transformers/categoricals.py` & `primrose-2.0.0/primrose/transformers/categoricals.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,19 @@
 
             x (str): transformation string
 
         Returns:
             data (dataframe)
 
         """
-        if 'transformations' in input_data.keys():
-            logging.info("Applying key {} to variable {}".format('transformations', categorical))
-            for transformation in input_data['transformations']:
+        if "transformations" in input_data.keys():
+            logging.info(
+                "Applying key {} to variable {}".format("transformations", categorical)
+            )
+            for transformation in input_data["transformations"]:
                 exec(transformation.format(x=x))
 
     @staticmethod
     def _process_rename(data, input_data, categorical):
         """rename a field
 
         Args:
@@ -66,18 +68,18 @@
         Returns:
             (tuple): tuple containing:
 
                 data (dataframe): dataframe
 
                 name (str): original name (if not "to_numeric": True), new_name otherwise
         """
-        if 'rename' in input_data.keys():
-            logging.info("Applying key {} to variable {}".format('rename', categorical))
-            data = data.rename({categorical: input_data['rename']}, axis='columns')
-            return data, input_data['rename']
+        if "rename" in input_data.keys():
+            logging.info("Applying key {} to variable {}".format("rename", categorical))
+            data = data.rename({categorical: input_data["rename"]}, axis="columns")
+            return data, input_data["rename"]
         return data, categorical
 
     @staticmethod
     def _process_numeric(data, input_data, name):
         """convert column to numeric
 
         Args:
@@ -87,33 +89,41 @@
 
             name (str): field name
 
         Returns:
             data with the colun converted to numeric
 
         """
-        if 'to_numeric' in input_data.keys():
+        if input_data.get("to_numeric", False):
 
-            logging.info("Applying key {} to variable {}".format('to_numeric', name))
+            logging.info("Applying key {} to variable {}".format("to_numeric", name))
 
-            if input_data['to_numeric']:
+            # if there are errors converting to numerical values, we need to sub in a reasonable value
+            if sum(pd.to_numeric(data[name], errors="coerce").isnull()) > 0:
+                logging.info(
+                    "Can't convert these entries in {}. Replacing with {}: {}".format(
+                        name,
+                        ExplicitCategoricalTransform.DEFAULT_NUMERIC,
+                        np.unique(
+                            data[name][
+                                pd.to_numeric(data[name], errors="coerce").isnull()
+                            ].astype(str)
+                        ),
+                    )
+                )
+
+                data[name][
+                    pd.to_numeric(data[name], errors="coerce").isnull()
+                ] = ExplicitCategoricalTransform.DEFAULT_NUMERIC
+            try:
+                data[name] = pd.to_numeric(data[name])
+                return data
 
-                # if there are errors converting to numerical values, we need to sub in a reasonable value
-                if sum(pd.to_numeric(data[name], errors='coerce').isnull()) > 0:
-                    logging.info("Can't convert these entries in {}. Replacing with {}: {}".format(
-                        name, ExplicitCategoricalTransform.DEFAULT_NUMERIC,
-                        np.unique(data[name][pd.to_numeric(data[name], errors='coerce').isnull()])))
-
-                    data[name][pd.to_numeric(data[name], errors='coerce').isnull()] = ExplicitCategoricalTransform.DEFAULT_NUMERIC
-                try:
-                    data[name] = pd.to_numeric(data[name])
-                    return data
-
-                except:
-                    raise TypeError('Failed to convert feature {} to numeric'.format(name))
+            except:
+                raise TypeError("Failed to convert feature {} to numeric".format(name))
 
         else:
             return data
 
     def transform(self, data):
         """Transform categorical variables into one or more numeric ones, no need to separate testing & training data
 
@@ -126,19 +136,25 @@
         """
         for categorical in self.categoricals.keys():
 
             x = "data['{}']".format(categorical)
 
             input_data = self.categoricals[categorical]
 
-            ExplicitCategoricalTransform._process_transformations(data, input_data, categorical, x)
-
-            data, new_name = ExplicitCategoricalTransform._process_rename(data, input_data, categorical)
-
-            data = ExplicitCategoricalTransform._process_numeric(data, input_data, new_name)
+            ExplicitCategoricalTransform._process_transformations(
+                data, input_data, categorical, x
+            )
+
+            data, new_name = ExplicitCategoricalTransform._process_rename(
+                data, input_data, categorical
+            )
+
+            data = ExplicitCategoricalTransform._process_numeric(
+                data, input_data, new_name
+            )
 
         return data
 
 
 class ImplicitCategoricalTransform(AbstractTransformer):
     """Class which implicitly transforms all string columns of a dataframe with sklearn LabelEncoder"""
 
@@ -160,23 +176,23 @@
             data (dataframe)
 
         Returns:
             dataframe (dataframe)
 
         """
 
-        logging.info('Fitting LabelEncoders on all string-based dataframe columns...')
+        logging.info("Fitting LabelEncoders on all string-based dataframe columns...")
 
         data.is_copy = False
 
         for column_name in data.columns:
 
             if data[column_name].dtype == object:
 
-                logging.info('Fitting LabelEncoder for column {}'.format(column_name))
+                logging.info("Fitting LabelEncoder for column {}".format(column_name))
 
                 self._encoder[column_name] = preprocessing.LabelEncoder()
                 self._encoder[column_name].fit(data[column_name])
 
                 if column_name == self.target_variable:
                     self.target_encoder = self._encoder[column_name]
             else:
@@ -197,12 +213,14 @@
 
         data.is_copy = False
 
         for column_name in data.columns:
 
             if column_name in self._encoder:
 
-                logging.info('LabelEncoding column {}'.format(column_name))
+                logging.info("LabelEncoding column {}".format(column_name))
 
-                data[column_name] = self._encoder[column_name].transform(data[column_name])
+                data[column_name] = self._encoder[column_name].transform(
+                    data[column_name]
+                )
 
         return data
```

### Comparing `primrose-1.0.9/primrose/transformers/combine.py` & `primrose-2.0.0/primrose/transformers/combine.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,31 +31,48 @@
     else:
 
         initial_data_length = len(left_df)
 
         for j in join_keys:
 
             if not j in left_df.columns:
-                raise Exception('Join key {} not in left {}. Aborting merge.'.format(j, left_df.columns))
+                raise Exception(
+                    "Join key {} not in left {}. Aborting merge.".format(
+                        j, left_df.columns
+                    )
+                )
             elif not j in right_df.columns:
-                raise Exception('Join key {} not in right {}. Aborting merge.'.format(j, right_df.columns))
+                raise Exception(
+                    "Join key {} not in right {}. Aborting merge.".format(
+                        j, right_df.columns
+                    )
+                )
 
             if not left_df[j].dtype == right_df[j].dtype:
-                logging.info('Join key {} is not of type {}. Casting.'.format(j, right_df[j].dtype))
+                logging.info(
+                    "Join key {} is not of type {}. Casting.".format(
+                        j, right_df[j].dtype
+                    )
+                )
                 try:
                     right_df[j] = right_df[j].astype(left_df[j].dtype)
                 except:
-                    raise Exception('Cannot cast join key {} as {}'.format(j, left_df[j].dtype))
+                    raise Exception(
+                        "Cannot cast join key {} as {}".format(j, left_df[j].dtype)
+                    )
 
-        left_df = left_df.merge(right_df, on=join_keys, how='left')
+        left_df = left_df.merge(right_df, on=join_keys, how="left")
         left_df.reset_index(inplace=True, drop=True)
 
         if len(left_df) > initial_data_length:
-            logging.warning("Merge increased data size by {} rows.".format(
-                len(left_df) - initial_data_length))
+            logging.warning(
+                "Merge increased data size by {} rows.".format(
+                    len(left_df) - initial_data_length
+                )
+            )
 
         return left_df
 
 
 class LeftJoinDataCombiner(AbstractTransformer):
     """combine two dataframes doing a left join"""
 
@@ -66,15 +83,15 @@
             join_key (list): the columns to perform the left join on
 
         """
         self.join_key = join_key
 
     def fit(self, data):
         """fit the data, here doing nothing
-        
+
         Args:
             data (list)L : list of pandas data frames
 
         Returns:
             nothing
         """
         pass
@@ -86,30 +103,40 @@
             data (list): list of dataframes
 
         Returns:
             dataframe
 
         """
         if not isinstance(data, list):
-            raise Exception("In this transformer, data needs to be a list of dataframes")
+            raise Exception(
+                "In this transformer, data needs to be a list of dataframes"
+            )
 
         if len(data) < 2:
 
-            logging.warning("Combiner needs at least two reader inputs, passing unchanged data.")
+            logging.warning(
+                "Combiner needs at least two reader inputs, returning input data from list to dataframe."
+            )
 
-            return data
+            return pd.DataFrame(data[0])
 
         elif not isinstance(data[0], pd.DataFrame):
 
-            raise Exception('LeftJoinDataCombiner must operate on an iterable of pandas.DataFrame objects.')
+            raise Exception(
+                "LeftJoinDataCombiner must operate on an iterable of pandas.DataFrame objects."
+            )
 
         else:
 
             combined_data = None
 
             # loop over each reader key and merge into a single combined dataframe
             for d in data:
-                combined_data = d if combined_data is None else left_merge_dataframe_on_validated_join_keys(
-                    combined_data, d, self.join_key)
+                combined_data = (
+                    d
+                    if combined_data is None
+                    else left_merge_dataframe_on_validated_join_keys(
+                        combined_data, d, self.join_key
+                    )
+                )
 
             return combined_data
-
```

### Comparing `primrose-1.0.9/primrose/transformers/strings.py` & `primrose-2.0.0/primrose/transformers/strings.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 """
 
 import pandas as pd
 import logging
 from primrose.base.transformer import AbstractTransformer
 
+
 class StringTransformer(AbstractTransformer):
     """Transforms Series of strings in a Series or DataFrame."""
-    def __init__(self,method,columns,*args,**kwargs):
+
+    def __init__(self, method, columns, *args, **kwargs):
         """
 
         Args:
             method (str): pandas.Series.str method
             columns (str or list): single column name str or list of columns to operate on
             *args: args for given string method
             **kwargs: kwargs for given string method
@@ -41,24 +43,26 @@
         Args:
             df (pd.DataFrame): pandas dataframe
 
         Returns:
             df (pd.DataFrame): pandas dataframe
 
         """
-        if isinstance(self.columns,str):
+        if isinstance(self.columns, str):
             df[self.columns] = self._execute_str_method(df[self.columns])
-        elif isinstance(self.columns,list):
+        elif isinstance(self.columns, list):
             for col in self.columns:
                 df[col] = self._execute_str_method(df[col])
         else:
-            logging.info('Column not passed as string or list of columns, returning original dataframe.')
+            logging.info(
+                "Column not passed as string or list of columns, returning original dataframe."
+            )
         return df
 
-    def _execute_str_method(self,series):
+    def _execute_str_method(self, series):
         """Executes string method on pandas series.
 
         Args:
             series (pd.Series): pandas series to transform
 
         Returns:
             series (pd.Series): transformed pandas series
```

### Comparing `primrose-1.0.9/primrose/transformers/impute.py` & `primrose-2.0.0/primrose/transformers/impute.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,27 @@
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 import pandas as pd
 import logging
 from primrose.base.transformer import AbstractTransformer
 
+
 class ColumnSpecificImpute(AbstractTransformer):
     """Transform config specified columns NULL values into zero, mean, median, mode, inf or negative inf"""
 
-    def __init__(self, columns_to_zero, columns_to_mean, columns_to_median, columns_to_mode,
-                columns_to_infinity, columns_to_neg_infinity):
+    def __init__(
+        self,
+        columns_to_zero,
+        columns_to_mean,
+        columns_to_median,
+        columns_to_mode,
+        columns_to_infinity,
+        columns_to_neg_infinity,
+    ):
         """Transform config specified columns NULL values into zero, mean, median, mode, inf or negative inf
 
         Args:
             columns_to_zero (list): list of columns to impute zeros
             columns_to_mean (list): list of columns to impute means
             columns_to_median (list): list of columns to impute medians
             columns_to_mode (list): list of columns to impute modes
@@ -52,50 +60,58 @@
             Exception if a column appears in multiple lists, or if column not recognized
 
         """
 
         self.encoder = {}
         columns_so_far = set()
 
-        for cols in [self.columns_to_zero,
-                    self.columns_to_mean,
-                    self.columns_to_median,
-                    self.columns_to_mode,
-                    self.columns_to_infinity,
-                    self.columns_to_neg_infinity]:
+        for cols in [
+            self.columns_to_zero,
+            self.columns_to_mean,
+            self.columns_to_median,
+            self.columns_to_mode,
+            self.columns_to_infinity,
+            self.columns_to_neg_infinity,
+        ]:
 
             # does column exist?
             for col in cols:
                 if not col in data.columns:
                     raise Exception("Unrecognized impute column '" + str(col) + "'")
 
             # is it in some previous list?
             in_common = columns_so_far.intersection(set(cols))
             if in_common:
-                raise Exception("There are columns in multiple lists "+ str(in_common))
+                raise Exception("There are columns in multiple lists " + str(in_common))
             columns_so_far = columns_so_far.union(set(cols))
 
-        logging.info('Specifying columns to impute 0')
+        logging.info("Specifying columns to impute 0")
         [self.encoder.setdefault(col, 0) for col in self.columns_to_zero]
 
-        logging.info('Specifying columns to impute median')
-        [self.encoder.setdefault(col, data[col].median()) for col in self.columns_to_median]
+        logging.info("Specifying columns to impute median")
+        [
+            self.encoder.setdefault(col, data[col].median())
+            for col in self.columns_to_median
+        ]
 
-        logging.info('Specifying columns to impute mean')
+        logging.info("Specifying columns to impute mean")
         [self.encoder.setdefault(col, data[col].mean()) for col in self.columns_to_mean]
 
-        logging.info('Specifying columns to impute large values')
-        [self.encoder.setdefault(col, 999999999.) for col in self.columns_to_infinity]
+        logging.info("Specifying columns to impute large values")
+        [self.encoder.setdefault(col, 999999999.0) for col in self.columns_to_infinity]
 
-        logging.info('Specifying columns to impute large negative values')
-        [self.encoder.setdefault(col, -999999999.) for col in self.columns_to_neg_infinity]
+        logging.info("Specifying columns to impute large negative values")
+        [
+            self.encoder.setdefault(col, -999999999.0)
+            for col in self.columns_to_neg_infinity
+        ]
 
-        logging.info('Specifying columns to impute mode')
+        logging.info("Specifying columns to impute mode")
         for col in self.columns_to_mode:
-            logging.info('imputing {}'.format(col))
+            logging.info("imputing {}".format(col))
             try:
                 if pd.notnull(data[col].mode().values[0]):
                     col_mode = data[col].mode().values[0]
                 else:
                     col_mode = 0
             except Exception:
                 col_mode = 0
@@ -113,13 +129,15 @@
 
         Raises:
             Exception if train is not called before transfoorm
 
         """
 
         if self.encoder is None:
-            raise Exception('ColumnSpecificImpute must train imputations with fit before calling transform.')
+            raise Exception(
+                "ColumnSpecificImpute must train imputations with fit before calling transform."
+            )
 
         for col, val in self.encoder.items():
             data[col] = data[col].fillna(val)
 
         return data
```

### Comparing `primrose-1.0.9/primrose/transformers/filter.py` & `primrose-2.0.0/primrose/transformers/filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import operator
 import logging
 import numpy as np
 import pandas as pd
 
 from primrose.base.transformer import AbstractTransformer
 
+
 class FilterByPandasExpression(AbstractTransformer):
     """Applies filters to data as defined in feature_filters"""
 
     def __init__(self, feature_filters):
         """initialize filter with a list of feature_filters"""
         self.feature_filters = feature_filters
 
@@ -45,15 +46,15 @@
 
         Args:
             data (dict): dictionary with dataframes from all readers
             data_key (str): key to pull the dataframe from within the data object
             feature_filters (list): list of lists with columns and operators to filter on
             instance_name (str): name of this pipeline instance
 
-        Returns: 
+        Returns:
             dataframe with filtered data
 
         Raises:
             Exception if not a pandas dataframe, operation not supported, or column name not recognized
 
         """
         if not isinstance(data, pd.DataFrame):
@@ -62,15 +63,15 @@
         ops = {
             "==": operator.eq,
             "!=": operator.ne,
             "<>": operator.ne,
             "<": operator.lt,
             "<=": operator.le,
             ">": operator.gt,
-            ">=": operator.ge
+            ">=": operator.ge,
         }
 
         if len(self.feature_filters) == 0:
             logging.info("no filters found; returning combined_data as filtered_data")
             return data
 
         else:
@@ -86,10 +87,10 @@
                     raise Exception("Unsupported filter operation '" + str(op) + "'")
 
                 filters.append(ops[op](data[col], val))
 
             filtered_data = data[np.all(filters, axis=0)]
             filtered_data = filtered_data.reset_index(drop=True)
 
-            logging.info('Filtered out %d rows' % (len(data) - len(filtered_data)))
+            logging.info("Filtered out %d rows" % (len(data) - len(filtered_data)))
 
         return filtered_data
```

### Comparing `primrose-1.0.9/primrose/templates/run_plot_dag.py` & `primrose-2.0.0/primrose/templates/run_plot_dag.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,93 @@
 import logging
 import argparse
 
 from primrose.configuration.configuration import Configuration
 from primrose.dag.traverser_factory import TraverserFactory
 
+
 def parse_arguments():
     """Parse command line arguments
     Use environment variables as default if passed.
     Returns: argument objects with flags as attributes
     """
     parser = argparse.ArgumentParser()
-    parser.add_argument('--config_loc',
-                        help='Location of the configuration file',
-                        required=True)
-    parser.add_argument('--node_size',
-                        help='Size of nodes',
-                        required=False)
-    parser.add_argument('--label_font_size',
-                        help='Size of font for text labels',
-                        required=False)
-    parser.add_argument('--text_angle',
-                        help='Angle to rotate text (counterclockwise)',
-                        required=False)
-    parser.add_argument('--image_width',
-                        help='width of image in inches',
-                        required=False)
-    parser.add_argument('--image_height',
-                        help='height of image in inches',
-                        required=False)
-    parser.add_argument('--nodesequence',
-                        help='Show node sequences numbers? "true" or "false"?',
-                        required=False)
-    parser.add_argument('--outfile',
-                        help='Path for the output image file',
-                        required=True)
+    parser.add_argument(
+        "--config_loc", help="Location of the configuration file", required=True
+    )
+    parser.add_argument("--node_size", help="Size of nodes", required=False)
+    parser.add_argument(
+        "--label_font_size", help="Size of font for text labels", required=False
+    )
+    parser.add_argument(
+        "--text_angle", help="Angle to rotate text (counterclockwise)", required=False
+    )
+    parser.add_argument(
+        "--image_width", help="width of image in inches", required=False
+    )
+    parser.add_argument(
+        "--image_height", help="height of image in inches", required=False
+    )
+    parser.add_argument(
+        "--nodesequence",
+        help='Show node sequences numbers? "true" or "false"?',
+        required=False,
+    )
+    parser.add_argument(
+        "--outfile", help="Path for the output image file", required=True
+    )
     known_args, pipeline_args = parser.parse_known_args()
     return known_args, pipeline_args
 
+
 def main():
     """Train, evaluate or predict with a machine learning model from a user defined data source
-        The function can optionally upload the results to an external source
+    The function can optionally upload the results to an external source
     """
     args, _ = parse_arguments()
 
-    logging.basicConfig(format='%(asctime)s %(filename)s %(funcName)s: %(message)s', level=logging.INFO)
+    logging.basicConfig(
+        format="%(asctime)s %(filename)s %(funcName)s: %(message)s", level=logging.INFO
+    )
     logging.getLogger().setLevel(logging.INFO)
 
     config = Configuration(config_location=args.config_loc)
 
     filename = args.outfile
     other_args = {}
-    other_args['filename'] = args.outfile
+    other_args["filename"] = args.outfile
 
     if args.node_size:
-        other_args['node_size'] = int(args.node_size)
+        other_args["node_size"] = int(args.node_size)
 
     if args.label_font_size:
-        other_args['label_font_size'] = int(args.label_font_size)
+        other_args["label_font_size"] = int(args.label_font_size)
 
     if args.text_angle:
-        other_args['text_angle'] = int(args.text_angle)
+        other_args["text_angle"] = int(args.text_angle)
 
     if args.image_width:
-        other_args['image_width'] = int(args.image_width)
+        other_args["image_width"] = int(args.image_width)
 
     if args.image_height:
-        other_args['image_height'] = int(args.image_height)
+        other_args["image_height"] = int(args.image_height)
 
-    other_args['traverser'] = None
+    other_args["traverser"] = None
     if args.nodesequence and args.nodesequence.lower() == "true":
         traverser = TraverserFactory().default_traverser(config)
 
-        if config.config_metadata and 'traverser' in config.config_metadata:
-            traverser = TraverserFactory().instantiate(config.config_metadata['traverser'], config)
-            logging.info("Setting to Traverser to %s", config.config_metadata['traverser'])
+        if config.config_metadata and "traverser" in config.config_metadata:
+            traverser = TraverserFactory().instantiate(
+                config.config_metadata["traverser"], config
+            )
+            logging.info(
+                "Setting to Traverser to %s", config.config_metadata["traverser"]
+            )
 
-        other_args['traverser'] = traverser
+        other_args["traverser"] = traverser
 
     logging.info("passing in %s", other_args)
     config.dag.plot_dag(**other_args)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     main()
```

### Comparing `primrose-1.0.9/primrose/templates/awesome_model.py` & `primrose-2.0.0/primrose/templates/awesome_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,33 +34,33 @@
         return AbstractModel.necessary_config(node_config)
 
     def train_model(self, data_object):
         """Code to train your model and return a data_object after adding any training or model info"""
 
         # Example model training code for building your own model
         # ----------------------------------
-        print('I am training my model.')
+        print("I am training my model.")
 
         # Example showing how to get upstream data
         # get some training data if it exists
         try:
             training_data = data_object.get_upstream_data(self.instance_name)
 
         except:
-            print('No upstream data exists')
+            print("No upstream data exists")
         # ----------------------------------
 
         return data_object
 
     def eval_model(self, data_object):
         """Code to evaluate your models performance"""
 
-        print('My model is doing pretty well.')
+        print("My model is doing pretty well.")
 
         return data_object
 
     def predict(self, data_object):
         """Make predictions using your model"""
 
-        print('I am predicting!')
+        print("I am predicting!")
 
         return data_object
```

### Comparing `primrose-1.0.9/primrose/templates/user_registration_template.py` & `primrose-2.0.0/primrose/templates/user_registration_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 # Alternatively, if you would like to register classes yourself via `node_factory.NodeFactory`, you can follow the steps below.
 #
 # Overview
 # ========
 # There are three steps to registering your own classes:
 #
 # 1) you need to generate a script to run primrose from your own project. To do that
-# run 
-# 
+# run
+#
 #   primrose generate_script --destination path/to/myproject/
-# 
+#
 # and it copies a run_primrose.py script to your project path
 #
 # 2) You need to register your own classes. This is the code in this script.
 #
 # 3) You need to reference this code in the run_primrose script.
 #
 # Step 1:
@@ -40,37 +40,41 @@
 # which will create path/to/myproject/run_primrose.py
 #
 # Open up the file and see where it tells you to reference this code.
 #
 # Step2:
 # ========
 # Modify this file to register your own classes.
-# As can be seen below, 
+# As can be seen below,
 #  - you first need to import the NodeFactory singleton
 #  - next, import your new classes
 #  - finally, use NodeFactory to register those classes
 #
 # Step 3:
 # ========
 # *Importantly*, this factory registration has to occur *before* Configuration is instantiated
-# in the run_primrose script. 
-# To that end, we suggest putting this registration code below into something 
-# like `src/__init__.py` in your project. Wherever you put it, you will need to reference 
+# in the run_primrose script.
+# To that end, we suggest putting this registration code below into something
+# like `src/__init__.py` in your project. Wherever you put it, you will need to reference
 # it in the run_primrose script.
 #
 # That is, if you put this code into `src/__init__.py`, you will need to add
 #
 #  from src.__init__ import *
 #
-# at the head of the run_primrose script. 
+# at the head of the run_primrose script.
 #
 #########################################################################################
 
 import logging
-logging.basicConfig(format='%(asctime)s %(levelname)s %(filename)s %(funcName)s: %(message)s', level=logging.INFO)
+
+logging.basicConfig(
+    format="%(asctime)s %(levelname)s %(filename)s %(funcName)s: %(message)s",
+    level=logging.INFO,
+)
 
 from primrose.node_factory import NodeFactory
 
 # Add your imports here
 from src.yourpackage.awesome_reader import AwesomeReader
 from src.yourpackage.awesome_model import AwesomeModel
```

### Comparing `primrose-1.0.9/primrose/templates/awesome_reader.py` & `primrose-2.0.0/primrose/templates/awesome_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,29 +22,29 @@
         Note:
             filename: name of the file
 
         Returns:
             set of necessary keys for the AwesomeReader object
 
         """
-        return set(['data_to_read'])
+        return set(["data_to_read"])
 
     def run(self, data_object):
         """Read data from node_config
 
         Returns:
             data_object (DataObject): DataObject instance
             terminate (bool): should we terminate the DAG? true or false
 
         """
 
         # Example showing data being created directly from the config file
         # any valid python can be used here for reading data into the data_object
         # examples of other readers can be found in primrose/readers/*
         # -------------------------------
-        data = self.node_config['data_to_read']
-        print('Reading in data!: {}'.format(data))
+        data = self.node_config["data_to_read"]
+        print("Reading in data!: {}".format(data))
         # -------------------------------
         # add data into data object for use downstream
         data_object.add(self, data)
         terminate = data is None
         return data_object, terminate
```

### Comparing `primrose-1.0.9/primrose/templates/run_primrose.py` & `primrose-2.0.0/primrose/templates/run_primrose.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-'''
+"""
     Run a job: i.e. run a configuration file through the DAGRunner
-'''
+"""
 import argparse
 import logging
 import warnings
 
 ######################################
 ######################################
 # Important:
@@ -23,40 +23,48 @@
 from primrose.configuration.configuration import Configuration
 from primrose.dag_runner import DagRunner
 from primrose.dag.config_layer_traverser import ConfigLayerTraverser
 from primrose.dag.depth_first_traverser import DepthFirstTraverser
 
 warnings.filterwarnings("ignore")
 
+
 def parse_arguments():
     """
-        Parse command line arguments
+    Parse command line arguments
 
-        Returns:
-            argument objects with flags as attributes
+    Returns:
+        argument objects with flags as attributes
     """
     parser = argparse.ArgumentParser()
-    parser.add_argument('--config_loc',
-                        help='Location of the configuration file',
-                        required=True)
-    parser.add_argument('--is_dry_run',
-                        help='do a dry run of the DAG which will validatre config and log which nodes would be run',
-                        default=False,
-                        type=lambda x: (str(x).lower() == 'true'))
+    parser.add_argument(
+        "--config_loc", help="Location of the configuration file", required=True
+    )
+    parser.add_argument(
+        "--is_dry_run",
+        help="do a dry run of the DAG which will validatre config and log which nodes would be run",
+        default=False,
+        type=lambda x: (str(x).lower() == "true"),
+    )
 
     known_args, pipeline_args = parser.parse_known_args()
     return known_args, pipeline_args
 
+
 def main():
     """
-        Run a job: i.e. run a configuration file through the DAGRunner
+    Run a job: i.e. run a configuration file through the DAGRunner
     """
     args, _ = parse_arguments()
 
-    logging.basicConfig(format='%(asctime)s %(levelname)s %(filename)s %(funcName)s: %(message)s', level=logging.INFO)
+    logging.basicConfig(
+        format="%(asctime)s %(levelname)s %(filename)s %(funcName)s: %(message)s",
+        level=logging.INFO,
+    )
 
     configuration = Configuration(config_location=args.config_loc)
 
     DagRunner(configuration).run(dry_run=args.is_dry_run)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     main()
```

### Comparing `primrose-1.0.9/primrose/cleanup/logging_success.py` & `primrose-2.0.0/primrose/cleanup/logging_success.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 import logging
 from primrose.base.success import AbstractSuccess
 
+
 class LoggingSuccess(AbstractSuccess):
     """simple success node: log a message"""
 
     @staticmethod
     def necessary_config(node_config):
         """Return a list of necessary configuration keys within the implementation
 
@@ -21,29 +22,29 @@
             msg: message you want logged
             level: one of 'DEBUG', 'INFO', 'WARN', 'ERROR', 'CRITICAL'
 
         Returns:
             set of keys necessary to run implementation
 
         """
-        return set(['msg', 'level']) 
+        return set(["msg", "level"])
 
     def run(self, data_object):
         """Signal success by logging a message at specified log level
 
         Args:
             data_object (DataObject): DataObject instance
 
         Returns:
             nothing. Side effect is to signal success via logging
 
         """
-        msg = self.node_config['msg']
+        msg = self.node_config["msg"]
 
-        level = str(self.node_config['level']).upper()
+        level = str(self.node_config["level"]).upper()
 
         # check whether valid level: will throw KeyError if level not recognized
         logging._nameToLevel[level]
 
         level = logging.getLevelName(level)
 
         logging.getLogger("")._log(level, msg, None, None)
```

### Comparing `primrose-1.0.9/primrose/readers/r_reader.py` & `primrose-2.0.0/primrose/readers/r_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,74 +12,77 @@
     Carl Anderson (carl.anderson@ww.com)
 
 """
 from primrose.base.reader import AbstractReader
 import logging
 import pandas as pd
 
+
 class RReader(AbstractReader):
     """Reads in canned dataset from R"""
 
     @staticmethod
     def necessary_config(node_config):
         """Return a list of necessary configuration keys within the implementation
 
         Args:
             dataset (string): name of dataset in R
 
         Returns:
             set of keys necessary to run implementation
 
         """
-        return set(['dataset'])
+        return set(["dataset"])
 
     def run(self, data_object):
         """Read canned dataset from R to a pandas dataframe
 
         Returns:
             data_object (DataObject): DataObject instance
             terminate (bool): should we terminate the DAG? true or false
 
         """
-        dataset = self.node_config['dataset']
-        logging.info('Reading {} from R'.format(dataset))
+        dataset = self.node_config["dataset"]
+        logging.info("Reading {} from R".format(dataset))
 
         try:
             from rpy2.robjects.packages import importr, data
-        except ImportError: # pragma: no cover
+        except ImportError:  # pragma: no cover
             raise ImportError(
                 "This example needs Rpy2."
                 "Please refer to the R requirements in the README"
-            )        
-        datasets = importr('datasets')
+            )
+        datasets = importr("datasets")
         r_env = data(datasets).fetch(dataset)
 
         import rpy2.robjects as robjects
+
         # why we do this:
-        #> data(euro)
-        #> euro
-        #ATS         BEF         DEM         ESP         FIM         FRF         IEP         ITL         LUF         NLG         PTE 
-        #13.760300   40.339900    1.955830  166.386000    5.945730    6.559570    0.787564 1936.270000   40.339900    2.203710  200.482000 
+        # > data(euro)
+        # > euro
+        # ATS         BEF         DEM         ESP         FIM         FRF         IEP         ITL         LUF         NLG         PTE
+        # 13.760300   40.339900    1.955830  166.386000    5.945730    6.559570    0.787564 1936.270000   40.339900    2.203710  200.482000
         #
-        #> as.data.frame(euro)
+        # > as.data.frame(euro)
         #        euro
-        #ATS   13.760300
-        #BEF   40.339900
-        #DEM    1.955830
-        data = robjects.r('as.data.frame(%s)' % dataset)
+        # ATS   13.760300
+        # BEF   40.339900
+        # DEM    1.955830
+        data = robjects.r("as.data.frame(%s)" % dataset)
 
         # at time of writing, rpy2's R dataframe to pandas dataframe was not fully supported
         # However, as python list() seems to work for FloatVector, StrVector, and FactorVector, let's use it
         from rpy2.robjects import r
+
         colnames = r.colnames(data)
         pandas_data = {}
         # convert each column of the R dataframe in turn
         for i, colname in enumerate(colnames):
             pandas_data[colname] = list(data[i])
-        # Unfortunately, some datasets have rownames that should be an ID column (e.g., see mtcars where rownames=names of the cars). 
+        # Unfortunately, some datasets have rownames that should be an ID column (e.g., see mtcars where rownames=names of the cars).
         # This is the best we can do: pull it out as an additional column for each and every dataset
-        pandas_data['row_names'] = list(data.rownames)
+        pandas_data["row_names"] = list(data.rownames)
 
         df = pd.DataFrame(pandas_data)
         data_object.add(self, df)
         terminate = df.empty
         return data_object, terminate
```

### Comparing `primrose-1.0.9/primrose/readers/csv_reader.py` & `primrose-2.0.0/primrose/readers/csv_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 
 """
 
 import logging
 import pandas as pd
 from primrose.base.reader import AbstractReader
 
+
 class CsvReader(AbstractReader):
     """Reads CSV file into a pandas dataframe"""
 
     @staticmethod
     def necessary_config(node_config):
         """Returns the necessary configuration keys for the CsvReader object
 
         Args:
             node_config (dict): set of parameters / attributes for the node
 
         Note:
             filename: name of the file
 
-        Returns: 
+        Returns:
             set of necessary keys for the CsvReader object
 
         """
-        return set(['filename'])
+        return set(["filename"])
 
     def get_optional_config(self):
         """Optionally get kwargs to pass to pandas csv reader.
 
         Notes:
             kwargs (dict): dictionary of kwargs key-value pairs
 
@@ -41,27 +42,27 @@
                 "kwargs": { \
                 "header": None, \
                 "sep": ":" \
                 } \
             } \
 
         """
-        if 'kwargs' in self.node_config:
-            return self.node_config['kwargs']
+        if "kwargs" in self.node_config:
+            return self.node_config["kwargs"]
         else:
             return {}
 
     def run(self, data_object):
         """Read CSV to a pandas dataframe
 
         Returns:
             data_object (DataObject): DataObject instance
             terminate (bool): should we terminate the DAG? true or false
 
         """
-        filename = self.node_config['filename']
-        logging.info('Reading {} from CSV'.format(filename))
+        filename = self.node_config["filename"]
+        logging.info("Reading {} from CSV".format(filename))
         kwargs = self.get_optional_config()
         df = pd.read_csv(filename, **kwargs)
         data_object.add(self, df)
         terminate = df.empty
         return data_object, terminate
```

### Comparing `primrose-1.0.9/primrose/readers/mysql_helper.py` & `primrose-2.0.0/primrose/readers/mysql_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 import mysql.connector
 from primrose.readers.database_helper import get_env_val
 
-class MySQLHelper():
+
+class MySQLHelper:
     """"some utility methods for connecting to MySQL"""
 
     @staticmethod
     def extract_mysql_credentials():
         """extract MySQL credentials from config
 
         Returns:
@@ -28,17 +29,30 @@
         database = get_env_val("MYSQL_DB")
         username = get_env_val("MYSQL_USER")
         password = get_env_val("MYSQL_PASS")
         return (host, port, username, password, database)
 
     @staticmethod
     def create_db_connection():
-        '''authenticate with MySQL database
+        """authenticate with MySQL database
 
         Returns:
             db (connection object): MySQL db object
 
-        '''
+        """
 
-        host, port, username, password, database = MySQLHelper.extract_mysql_credentials()
-        conn = mysql.connector.connect(database=database, user=username, passwd=password, host=host, port=port, auth_plugin='mysql_native_password')
+        (
+            host,
+            port,
+            username,
+            password,
+            database,
+        ) = MySQLHelper.extract_mysql_credentials()
+        conn = mysql.connector.connect(
+            database=database,
+            user=username,
+            passwd=password,
+            host=host,
+            port=port,
+            auth_plugin="mysql_native_password",
+        )
         return conn
```

### Comparing `primrose-1.0.9/primrose/readers/postgres_reader.py` & `primrose-2.0.0/primrose/readers/postgres_reader.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 from primrose.base.sql_reader import AbstractSqlReader
 from primrose.readers.postgres_helper import PostgresHelper
 
+
 class PostgresReader(AbstractSqlReader):
     """Runs PostgreSQL queries into pandas dataframes"""
 
     def get_connection(self):
         """return connection to PostgreSQL DB
 
         Returns:
```

### Comparing `primrose-1.0.9/primrose/readers/postgres_helper.py` & `primrose-2.0.0/primrose/readers/postgres_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 
 """
 import os
 from primrose.readers.database_helper import get_env_val
 
 try:
     import psycopg2
+
     HAS_PSYCOPG2 = True
 
 except ImportError:
     HAS_PSYCOPG2 = False
 
 
-class PostgresHelper():
-    '''
-        some utility methods for connecting to postgres
-    '''
+class PostgresHelper:
+    """
+    some utility methods for connecting to postgres
+    """
 
     @staticmethod
     def extract_postgres_credentials():
         """extract PostgreSQL credentials from config
 
         Returns:
             (tuple): tuple containing: \
@@ -42,18 +43,30 @@
         password = get_env_val("POSTGRES_PASS")
         return (host, port, username, password, database)
 
     @staticmethod
     def create_db_connection():
         """authenticate with postgres database
 
-            Returns:
-                db (connection): postgres db object
+        Returns:
+            db (connection): postgres db object
 
         """
         if not HAS_PSYCOPG2:
             raise ImportError("psycopg2 is necessary to establish connection")
 
-        host, port, username, password, database = PostgresHelper.extract_postgres_credentials()
-        conn = psycopg2.connect(dbname=database, user=username, password=password, host=host, port=port, sslmode='require')
+        (
+            host,
+            port,
+            username,
+            password,
+            database,
+        ) = PostgresHelper.extract_postgres_credentials()
+        conn = psycopg2.connect(
+            dbname=database,
+            user=username,
+            password=password,
+            host=host,
+            port=port,
+            sslmode="require",
+        )
         return conn
-
```

### Comparing `primrose-1.0.9/primrose/readers/gcs_dill_reader.py` & `primrose-2.0.0/primrose/readers/gcs_dill_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,19 @@
 
 from primrose.base.reader import AbstractReader
 
 
 class GcsDillReader(AbstractReader):
     """Read a file from Gcs and un-dills it into memory"""
 
-    DATA_KEY = 'reader_data'
-    warnings.warn('Use Deserializer instead. GcsDillReader will be deprecated in a future release.', DeprecationWarning)
+    DATA_KEY = "reader_data"
+    warnings.warn(
+        "Use Deserializer instead. GcsDillReader will be deprecated in a future release.",
+        DeprecationWarning,
+    )
 
     @staticmethod
     def necessary_config(node_config):
         """Returns the necessary configuration keys for the GcsDillReader object
 
         Args:
             node_config (dict): set of parameters / attributes for the node
@@ -30,42 +33,46 @@
             bucket_name: name of the GCS bucket
             blob_name: name of the blob
 
         Returns:
             set of necessary keys for the CsvReader object
 
         """
-        return set(['bucket_name', 'blob_name'])
+        return set(["bucket_name", "blob_name"])
 
     def download_blobs_as_strings(self):
         """Downloads a blob from the bucket contining the user specified blob_name
 
         Returns:
             list of strings
 
         """
 
-        if 'gcs_project' in self.node_config:
-            storage_client = storage.Client(project=self.node_config['gcs_project'])
+        if "gcs_project" in self.node_config:
+            storage_client = storage.Client(project=self.node_config["gcs_project"])
         else:
             storage_client = storage.Client()
 
-        bucket = storage_client.get_bucket(self.node_config['bucket_name'])
+        bucket = storage_client.get_bucket(self.node_config["bucket_name"])
 
-        if 'prefix' in self.node_config:
-            prefix = self.node_config['prefix']
+        if "prefix" in self.node_config:
+            prefix = self.node_config["prefix"]
         else:
             prefix = None
 
         blob_list = bucket.list_blobs(prefix=prefix)
 
-        valid_blobs = [blob for blob in blob_list if self.node_config['blob_name'] in blob.name]
+        valid_blobs = [
+            blob for blob in blob_list if self.node_config["blob_name"] in blob.name
+        ]
 
         if len(valid_blobs) == 0:
-            raise Exception('{} not found in GCS bucket.'.format(self.node_config['blob_name']))
+            raise Exception(
+                "{} not found in GCS bucket.".format(self.node_config["blob_name"])
+            )
 
         return [blob.download_as_string() for blob in valid_blobs]
 
     def run(self, data_object):
         """Read dill object(s) from GCS bucket which contain the blob_name
 
         Args:
@@ -75,15 +82,15 @@
             (tuple): tuple containing:
 
                 data_object (DataObject): instance of DataObject
 
                 terminate (bool): terminate the DAG?
 
         """
-        logging.info('Reading {} from GCS'.format(self.node_config['blob_name']))
+        logging.info("Reading {} from GCS".format(self.node_config["blob_name"]))
         objects = [dill.loads(obj) for obj in self.download_blobs_as_strings()]
 
         terminate = len(objects) == 0
 
         if len(objects) == 1:
             data_object.add(self, objects[0], key=GcsDillReader.DATA_KEY)
         else:
```

### Comparing `primrose-1.0.9/primrose/readers/sklearn_dataset_reader.py` & `primrose-2.0.0/primrose/readers/sklearn_dataset_reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,54 +4,62 @@
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 from primrose.base.sql_reader import AbstractReader
 from sklearn.datasets import *
 import pandas as pd
 
+
 class SklearnDatasetReader(AbstractReader):
     """Read data from sklearn.dataset into a pandas dataframe"""
 
     @staticmethod
     def necessary_config(node_config):
         """Returns the necessary configuration keys for the SklearnDatasetReader object
 
         Note:
             dataset (str): name of supported sklearn.dataset. One of "iris", "boston", "diabetes", "breast_cancer", "linnerud", "wine"
-            
-        Returns: 
+
+        Returns:
             set of necessary keys for the SklearnDatasetReader object
 
         """
-        return set(['dataset'])
+        return set(["dataset"])
 
     def run(self, data_object):
         """Read sklearn dataset to a pandas dataframe
 
         Returns:
             data_object (DataObject): DataObject instance
             terminate (bool): should we terminate the DAG? true or false
 
         """
-        dataset = self.node_config['dataset']
+        dataset = self.node_config["dataset"]
 
         function_map = {
             "iris": load_iris,
-            "boston": load_boston,
             "diabetes": load_diabetes,
             "breast_cancer": load_breast_cancer,
             "linnerud": load_linnerud,
-            "wine": load_wine
+            "wine": load_wine,
         }
 
+        try:
+            _boston = load_boston
+            function_map["boston"] = _boston
+        except NameError:
+            # the boston housing dataset is deprecated in sklearn>1.0
+            # https://scikit-learn.org/stable/whats_new/v1.0.html#id10
+            ...
+
         if not dataset in function_map.keys():
             raise Exception("Dataset not supported " + dataset)
 
         data = function_map[dataset]()
 
-        df = pd.DataFrame(data['data'], columns = data['feature_names'])
-        df['target'] = data['target']
+        df = pd.DataFrame(data["data"], columns=data["feature_names"])
+        df["target"] = data["target"]
 
         data_object.add(self, df)
 
         terminate = False
         return data_object, terminate
```

### Comparing `primrose-1.0.9/primrose/readers/dill_reader.py` & `primrose-2.0.0/primrose/readers/dill_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,31 +11,35 @@
 
 from primrose.base.reader import AbstractReader
 
 
 class DillReader(AbstractReader):
     """Read a file from Gcs and un-dills it into memory"""
 
-    DATA_KEY = 'reader_data'
-    warnings.warn('Use Deserializer instead. DillReader will be deprecated in a future release.', DeprecationWarning)
+    DATA_KEY = "reader_data"
+    warnings.warn(
+        "Use Deserializer instead. DillReader will be deprecated in a future release.",
+        DeprecationWarning,
+    )
+
     @staticmethod
     def necessary_config(node_config):
         """Returns the necessary configuration keys for the DillReader object
 
         Args:
             node_config (dict): set of parameters / attributes for the node
 
         Note:
             filename: local filename to be de-serialized
 
         Returns:
             set of necessary keys for the DillReader object
 
         """
-        return set(['filename'])
+        return set(["filename"])
 
     def run(self, data_object):
         """Read dill object(s) from local filesystem
 
         Args:
             data_object: DataObject instance
 
@@ -43,16 +47,18 @@
             (tuple): tuple containing:
 
                 data_object (DataObject): instance of DataObject
 
                 terminate (bool): terminate the DAG?
 
         """
-        logging.info('Reading {} from local filesystem'.format(self.node_config['filename']))
+        logging.info(
+            "Reading {} from local filesystem".format(self.node_config["filename"])
+        )
 
-        object = dill.load(open(self.node_config['filename'], 'rb'))
+        object = dill.load(open(self.node_config["filename"], "rb"))
 
         data_object.add(self, object, key=DillReader.DATA_KEY)
 
         terminate = False
 
         return data_object, terminate
```

### Comparing `primrose-1.0.9/primrose/readers/deserializer.py` & `primrose-2.0.0/primrose/readers/deserializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 import pickle
 from google.cloud import storage
 from primrose.base.reader import AbstractReader
 
 
 class Deserializer(AbstractReader):
     """Read a local file and de-serialize it into memory."""
-    DATA_KEY = 'reader_data'
-    SUPPORTED_DESERIALIZERS = {'dill': dill, 'pickle': pickle}
+
+    DATA_KEY = "reader_data"
+    SUPPORTED_DESERIALIZERS = {"dill": dill, "pickle": pickle}
 
     @staticmethod
     def necessary_config(node_config):
         """Returns the necessary configuration keys for the Deserializer object
 
         Args:
             node_config (dict): set of parameters / attributes for the node
@@ -29,15 +30,15 @@
             filename (str): local filename to be de-serialized
             deserializer (str): 'dill' or 'pickle'
 
         Returns:
             set of necessary keys for the Deserializer object
 
         """
-        return set(['filename','deserializer'])
+        return set(["filename", "deserializer"])
 
     def run(self, data_object):
         """Read dill object(s) from local filesystem
 
         Args:
             data_object: DataObject instance
 
@@ -45,36 +46,50 @@
             (tuple): tuple containing:
 
                 data_object (DataObject): instance of DataObject
 
                 terminate (bool): terminate the DAG?
 
         """
-        logging.info('Reading {} from local filesystem'.format(self.node_config['filename']))
-
-        if self.node_config['deserializer'] not in Deserializer.SUPPORTED_DESERIALIZERS.keys():
-            logging.warning(f"{self.node_config['deserializer']} deserializer not supported.")
-            logging.warning(f"The following deserializers are supported {Deserializer.SUPPORTED_DESERIALIZERS.keys()}.")
-            raise Exception(f"Unsupported Deserializer: {self.node_config['deserializer']}")
-
-        deserializer = Deserializer.SUPPORTED_DESERIALIZERS[self.node_config['deserializer']]
+        logging.info(
+            "Reading {} from local filesystem".format(self.node_config["filename"])
+        )
+
+        if (
+            self.node_config["deserializer"]
+            not in Deserializer.SUPPORTED_DESERIALIZERS.keys()
+        ):
+            logging.warning(
+                f"{self.node_config['deserializer']} deserializer not supported."
+            )
+            logging.warning(
+                f"The following deserializers are supported {Deserializer.SUPPORTED_DESERIALIZERS.keys()}."
+            )
+            raise Exception(
+                f"Unsupported Deserializer: {self.node_config['deserializer']}"
+            )
+
+        deserializer = Deserializer.SUPPORTED_DESERIALIZERS[
+            self.node_config["deserializer"]
+        ]
 
-        object = deserializer.load(open(self.node_config['filename'], 'rb'))
+        object = deserializer.load(open(self.node_config["filename"], "rb"))
 
         data_object.add(self, object, key=Deserializer.DATA_KEY)
 
         terminate = False
 
         return data_object, terminate
 
+
 class GcsDeserializer(AbstractReader):
     """Read a file from GCS and de-serialize it into memory."""
 
-    DATA_KEY = 'reader_data'
-    SUPPORTED_DESERIALIZERS = {'dill': dill, 'pickle': pickle}
+    DATA_KEY = "reader_data"
+    SUPPORTED_DESERIALIZERS = {"dill": dill, "pickle": pickle}
 
     @staticmethod
     def necessary_config(node_config):
         """Returns the necessary configuration keys for the GcsDeserializer object
 
         Args:
             node_config (dict): set of parameters / attributes for the node
@@ -84,42 +99,46 @@
             blob_name: name of the blob
             deserializer (str): 'dill' or 'pickle'
 
         Returns:
             set of necessary keys for the GcsDeserializer object
 
         """
-        return set(['bucket_name', 'blob_name','deserializer'])
+        return set(["bucket_name", "blob_name", "deserializer"])
 
     def download_blobs_as_strings(self):
         """Downloads a blob from the bucket contining the user specified blob_name
 
         Returns:
             list of strings
 
         """
 
-        if 'gcs_project' in self.node_config:
-            storage_client = storage.Client(project=self.node_config['gcs_project'])
+        if "gcs_project" in self.node_config:
+            storage_client = storage.Client(project=self.node_config["gcs_project"])
         else:
             storage_client = storage.Client()
 
-        bucket = storage_client.get_bucket(self.node_config['bucket_name'])
+        bucket = storage_client.get_bucket(self.node_config["bucket_name"])
 
-        if 'prefix' in self.node_config:
-            prefix = self.node_config['prefix']
+        if "prefix" in self.node_config:
+            prefix = self.node_config["prefix"]
         else:
             prefix = None
 
         blob_list = bucket.list_blobs(prefix=prefix)
 
-        valid_blobs = [blob for blob in blob_list if self.node_config['blob_name'] in blob.name]
+        valid_blobs = [
+            blob for blob in blob_list if self.node_config["blob_name"] in blob.name
+        ]
 
         if len(valid_blobs) == 0:
-            raise Exception('{} not found in GCS bucket.'.format(self.node_config['blob_name']))
+            raise Exception(
+                "{} not found in GCS bucket.".format(self.node_config["blob_name"])
+            )
 
         return [blob.download_as_string() for blob in valid_blobs]
 
     def run(self, data_object):
         """Read serialized object(s) from GCS bucket which contain the blob_name
 
         Args:
@@ -129,26 +148,37 @@
             (tuple): tuple containing:
 
                 data_object (DataObject): instance of DataObject
 
                 terminate (bool): terminate the DAG?
 
         """
-        logging.info('Reading {} from GCS'.format(self.node_config['blob_name']))
-
-        if self.node_config['deserializer'] not in Deserializer.SUPPORTED_DESERIALIZERS.keys():
-            logging.warning(f"{self.node_config['deserializer']} deserializer not supported.")
-            logging.warning(f"The following deserializers are supported {Deserializer.SUPPORTED_DESERIALIZERS.keys()}.")
-            raise Exception(f"Unsupported Deserializer: {self.node_config['deserializer']}")
+        logging.info("Reading {} from GCS".format(self.node_config["blob_name"]))
 
-        deserializer = Deserializer.SUPPORTED_DESERIALIZERS[self.node_config['deserializer']]
+        if (
+            self.node_config["deserializer"]
+            not in Deserializer.SUPPORTED_DESERIALIZERS.keys()
+        ):
+            logging.warning(
+                f"{self.node_config['deserializer']} deserializer not supported."
+            )
+            logging.warning(
+                f"The following deserializers are supported {Deserializer.SUPPORTED_DESERIALIZERS.keys()}."
+            )
+            raise Exception(
+                f"Unsupported Deserializer: {self.node_config['deserializer']}"
+            )
+
+        deserializer = Deserializer.SUPPORTED_DESERIALIZERS[
+            self.node_config["deserializer"]
+        ]
 
         objects = [deserializer.loads(obj) for obj in self.download_blobs_as_strings()]
 
         terminate = len(objects) == 0
 
         if len(objects) == 1:
             data_object.add(self, objects[0], key=GcsDeserializer.DATA_KEY)
         else:
             data_object.add(self, objects, key=GcsDeserializer.DATA_KEY)
 
-        return data_object, terminate
+        return data_object, terminate
```

### Comparing `primrose-1.0.9/primrose/readers/mysql_reader.py` & `primrose-2.0.0/primrose/readers/mysql_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 from primrose.base.sql_reader import AbstractSqlReader
 from primrose.readers.mysql_helper import MySQLHelper
 
+
 class MySQLReader(AbstractSqlReader):
     """Runs MySQL queries into pandas dataframes"""
 
     def get_connection(self):
         """return connection to MySQL DB
 
         Returns:
```

### Comparing `primrose-1.0.9/primrose/readers/sqlite_reader.py` & `primrose-2.0.0/primrose/readers/sqlite_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 import sqlite3
 from primrose.base.sql_reader import AbstractSqlReader
 
+
 class SQLiteReader(AbstractSqlReader):
     """Runs SQLite queries into pandas dataframes"""
 
     @staticmethod
     def necessary_config(node_config):
         """Return a list of necessary configuration keys within the implementation
 
@@ -20,17 +21,17 @@
         Note:
             After adding this list, validation automatically occurs before instantiation in the pipeline factory.
 
         Returns:
             set of keys necessary to run implementation
 
         """
-        return set(['filename', 'query_json'])
+        return set(["filename", "query_json"])
 
     def get_connection(self):
         """return connection to SQLite DB
 
         Returns:
             connection to SQLite DB file
 
         """
-        return sqlite3.connect(self.node_config['filename'])
+        return sqlite3.connect(self.node_config["filename"])
```

### Comparing `primrose-1.0.9/primrose/configuration/util.py` & `primrose-2.0.0/primrose/configuration/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,43 +2,50 @@
 
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 from enum import Enum
 
+
 class ConfigurationError(Exception):
-    ''' named error specifically for configuration errors'''
+    """ named error specifically for configuration errors"""
+
     pass
 
+
 ########################################################################
-# note: am adding this Enum in file separate from configuration.py 
+# note: am adding this Enum in file separate from configuration.py
 # to fend off circular dependencies:
 #   configuration -> factory -> individual operation classes -> configuration
 ########################################################################
 
+
 class ConfigurationSectionType(Enum):
     """set of top-level sections in config"""
-    METADATA = 'metadata'
-    IMPLEMENTATION_CONFIG = 'implementation_config'
+
+    METADATA = "metadata"
+    IMPLEMENTATION_CONFIG = "implementation_config"
 
     @staticmethod
     def values():
-        '''list of the enum's values'''
+        """list of the enum's values"""
         return list(map(lambda t: t.value, ConfigurationSectionType))
 
+
 class OperationType(Enum):
     """set of operation type identifiers"""
-    reader = 'reader_config'
-    pipeline = 'pipeline_config'
-    model = 'model_config'
-    postprocess = 'postprocess_config'
-    writer = 'writer_config'
-    dataviz = 'dataviz_config'
-    cleanup = 'cleanup_config'
+
+    reader = "reader_config"
+    pipeline = "pipeline_config"
+    model = "model_config"
+    postprocess = "postprocess_config"
+    writer = "writer_config"
+    dataviz = "dataviz_config"
+    cleanup = "cleanup_config"
 
     @staticmethod
     def names():
         """list of the enum's names
 
         Returns:
             list of (name, OperationType) pairs
```

### Comparing `primrose-1.0.9/primrose/configuration/configuration.py` & `primrose-2.0.0/primrose/configuration/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,21 +15,26 @@
 from jinja2.exceptions import TemplateNotFound
 import hashlib
 import os
 import logging
 import importlib
 import glob
 from primrose.node_factory import NodeFactory
-from primrose.configuration.util import OperationType, ConfigurationError, ConfigurationSectionType
+from primrose.configuration.util import (
+    OperationType,
+    ConfigurationError,
+    ConfigurationSectionType,
+)
 from primrose.configuration.configuration_dag import ConfigurationDag
 from primrose.dag.traverser_factory import TraverserFactory
 
 
-SUPPORTED_EXTS = frozenset(['.json', '.yaml', '.yml'])
-CLASS_ENV_PACKAGE_KEY = 'PRIMROSE_EXT_NODE_PACKAGE'
+SUPPORTED_EXTS = frozenset([".json", ".yaml", ".yml"])
+CLASS_ENV_PACKAGE_KEY = "PRIMROSE_EXT_NODE_PACKAGE"
+
 
 class Configuration:
     """Stores user defined configuration for primrose job"""
 
     def __init__(self, config_location, is_dict_config=False, dict_config=None):
         """Read in configuration file and parse into specified values
 
@@ -39,43 +44,47 @@
             dict_config (dict): dictionary object, if is_dict_config
 
         """
         if is_dict_config:
             ext = None
 
             if dict_config is None:
-                raise Exception('expected dict_config was None')
+                raise Exception("expected dict_config was None")
 
             if not isinstance(dict_config, dict):
-                raise Exception('did not receive expected dict_config')
+                raise Exception("did not receive expected dict_config")
 
             dict_str = jstyleson.dumps(dict_config)
 
             config_str = Configuration.perform_any_config_fragment_substitution(dict_str)
 
         else:
-            logging.info('Loading config file at {}'.format(config_location))
+            logging.info("Loading config file at {}".format(config_location))
             self.config_location = config_location
 
             if os.path.exists(config_location):
                 ext = os.path.splitext(config_location)[1].lower()
                 if ext not in SUPPORTED_EXTS:
-                    raise ValueError('config file at: {} has improper extension type - please use a .json or .yml file'.format(config_location))
+                    raise ValueError(
+                        "config file at: {} has improper extension type - please use a .json or .yml file".format(
+                            config_location
+                        )
+                    )
 
-                with open(config_location, 'r') as f:
+                with open(config_location, "r") as f:
                     config_str = f.read()
 
                 config_str = Configuration.perform_any_config_fragment_substitution(config_str)
 
             else:
-                raise Exception('config file at: {} not found'.format(config_location))
+                raise Exception("config file at: {} not found".format(config_location))
 
-        if ext is None or ext == '.json':
+        if ext is None or ext == ".json":
             self.config = jstyleson.loads(config_str, object_pairs_hook=self.dict_raise_on_duplicates)
-        elif ext in ['.yaml', '.yml']:
+        elif ext in [".yaml", ".yml"]:
             self.config = yaml.load(config_str, Loader=yaml.FullLoader)
 
         assert isinstance(self.config, dict)
 
         # check top-level keys
         for k in self.config:
             if k not in ConfigurationSectionType.values():
@@ -86,30 +95,32 @@
         # metadata section can be optional
         self.config_metadata = None
         if ConfigurationSectionType.METADATA.value in self.config:
             self.config_metadata = self.config[ConfigurationSectionType.METADATA.value]
 
         # implemetation_config section is required
         if not ConfigurationSectionType.IMPLEMENTATION_CONFIG.value in self.config:
-            raise ConfigurationError("Did not find required top-level key %s" % ConfigurationSectionType.IMPLEMENTATION_CONFIG.value)
+            raise ConfigurationError(
+                "Did not find required top-level key %s" % ConfigurationSectionType.IMPLEMENTATION_CONFIG.value
+            )
 
         # keep a copy of the complete configuration
         self.complete_config = self.config.copy()
 
         # note: config is now just the implementation component of the dictionary
         self.config = self.config[ConfigurationSectionType.IMPLEMENTATION_CONFIG.value]
 
         # store the dag object
         self.dag = ConfigurationDag(self.config)
 
         # populate configuration file string and hash
         self.config_string, self.config_hash = self._get_configuration_hash()
 
         # get the formatted time this file was instantiated
-        self.config_time = datetime.datetime.now().strftime('%Y%m%d_%H%M')
+        self.config_time = datetime.datetime.now().strftime("%Y%m%d_%H%M")
 
         # parse the file into an internal config object
         self._parse_config()
 
         self.check_config()
 
     @staticmethod
@@ -129,19 +140,24 @@
         Args:
             config_str (str): content of some configuration file that may or may not contain substition variables
 
         Returns:
             config_str (str): the post-substituted configuration string
 
         """
-        jinja_env = Environment(loader=FileSystemLoader(['.', '/']))
+
+        def env_override(value, key):
+            return os.getenv(key, value)
+
+        jinja_env = Environment(loader=FileSystemLoader([".", "/"]))
+        jinja_env.filters["env_override"] = env_override
         try:
             config_str_template = jinja_env.from_string(config_str)
             config_str = config_str_template.render()
-        except(TemplateNotFound) as error:
+        except (TemplateNotFound) as error:
             filenames = str(error)
             raise ConfigurationError(f"Substitution files do not exist: {filenames}")
         return config_str
 
     def dict_raise_on_duplicates(self, ordered_pairs):
         """Reject duplicate keys in JSON string, ie. sections and node names.
 
@@ -150,15 +166,15 @@
             Example: ordered_pairs `[('class', 'CsvReader'), ('filename', 'data/tennis.csv'), ('destinations', ['write_output'])]` \
             ordered_pairs `[('read_data', {'class': 'CsvReader', 'filename': 'data/tennis.csv', 'destinations': ['write_output']})]`
 
         Returns:
             dictionary (dict): dictionary of key (node type) and value (node name)
 
         """
-        #https://stackoverflow.com/questions/14902299/json-loads-allows-duplicate-keys-in-a-dictionary-overwriting-the-first-value
+        # https://stackoverflow.com/questions/14902299/json-loads-allows-duplicate-keys-in-a-dictionary-overwriting-the-first-value
 
         d = {}
         for k, v in ordered_pairs:
             if k in d:
                 raise ConfigurationError("duplicate key: %r" % (k,))
             else:
                 d[k] = v
@@ -172,63 +188,75 @@
 
                 configuration_string (str):  configuration_string
 
                 configuration_file_hashname (str): terminate the DAG?
 
         """
         configuration_string = json.dumps(self.complete_config, sort_keys=True)
-        configuration_file_hashname = hashlib.sha256(configuration_string.encode('utf-8')).hexdigest()
+        configuration_file_hashname = hashlib.sha256(configuration_string.encode("utf-8")).hexdigest()
         return configuration_string, configuration_file_hashname
 
     def check_metadata(self):
         """checks some dependencies among metadata keys
 
         Raises:
             ConfigurationError is issues found
 
         """
         if self.config_metadata:
 
-            if 'traverser' in self.config_metadata:
-                classname = self.config_metadata['traverser']
+            if "traverser" in self.config_metadata:
+                classname = self.config_metadata["traverser"]
                 try:
                     TraverserFactory().instantiate(classname, self)
                 except KeyError:
                     raise Exception(classname + " is not a valid and/or registered Traverser")
 
-            if 'data_object' in self.config_metadata:
-
-                cfg = self.config_metadata['data_object']
-
-                if 'read_from_cache' in cfg and (cfg['read_from_cache'] or str(cfg['read_from_cache']).lower() == "true"):
+            if "data_object" in self.config_metadata:
 
-                    if not 'read_filename' in cfg:
-                        raise ConfigurationError("metadata.data_object: if read_from_cache==true, you must set 'read_filename'")
+                cfg = self.config_metadata["data_object"]
 
-                    #just check path exists but not that one can read into a DataObject
-                    if not os.path.exists(cfg['read_filename']):
-                        raise ConfigurationError("Invalid metadata.data_object.read_filename: " + str(cfg['read_filename']))
-
-                if 'write_to_cache' in cfg and (cfg['write_to_cache'] or str(cfg['write_to_cache']).lower() == "true"):
-
-                    if not 'write_filename' in cfg:
-                        raise ConfigurationError("metadata.data_object: if write_to_cache==true, you must set 'write_filename'")
+                if "read_from_cache" in cfg and (
+                    cfg["read_from_cache"] or str(cfg["read_from_cache"]).lower() == "true"
+                ):
+
+                    if not "read_filename" in cfg:
+                        raise ConfigurationError(
+                            "metadata.data_object: if read_from_cache==true, you must set 'read_filename'"
+                        )
+
+                    # just check path exists but not that one can read into a DataObject
+                    if not os.path.exists(cfg["read_filename"]):
+                        raise ConfigurationError(
+                            "Invalid metadata.data_object.read_filename: " + str(cfg["read_filename"])
+                        )
+
+                if "write_to_cache" in cfg and (cfg["write_to_cache"] or str(cfg["write_to_cache"]).lower() == "true"):
+
+                    if not "write_filename" in cfg:
+                        raise ConfigurationError(
+                            "metadata.data_object: if write_to_cache==true, you must set 'write_filename'"
+                        )
 
     def check_sections(self):
         """Check that all the sections in implementation are supported ones.
         Either the user supplied metata.section_registry, or they are using default sections
 
         Raises:
             ConfigurationError if declaring metadata.section_registry and sections from implementation were not found in metadata
             or vice versa, or if using default operations but sections found that were not supported
 
         """
-        if self.config_metadata and 'section_registry' in self.config_metadata and len(self.config_metadata['section_registry']) > 0:
+        if (
+            self.config_metadata
+            and "section_registry" in self.config_metadata
+            and len(self.config_metadata["section_registry"]) > 0
+        ):
             actual_set = set(self.config.keys())
-            user_set = set(self.config_metadata['section_registry'])
+            user_set = set(self.config_metadata["section_registry"])
 
             if actual_set != user_set:
 
                 diff = user_set.difference(actual_set)
                 if len(diff) > 0:
                     msg = "Following sections from metadata were not found implementation: " + str(diff)
                     raise ConfigurationError(msg)
@@ -274,21 +302,29 @@
             (tuple): tuple containing:
 
                 section names (list): list of sections
 
                 source (str): where did the list come from? section_run, section_registry, or default?
 
         """
-        if self.config_metadata and 'section_run' in self.config_metadata and len(self.config_metadata['section_run']) > 0:
-            return self.config_metadata['section_run'], 'section_run'
+        if (
+            self.config_metadata
+            and "section_run" in self.config_metadata
+            and len(self.config_metadata["section_run"]) > 0
+        ):
+            return self.config_metadata["section_run"], "section_run"
+
+        if (
+            self.config_metadata
+            and "section_registry" in self.config_metadata
+            and len(self.config_metadata["section_registry"]) > 0
+        ):
+            return self.config_metadata["section_registry"], "section_registry"
 
-        if self.config_metadata and 'section_registry' in self.config_metadata and len(self.config_metadata['section_registry']) > 0:
-            return self.config_metadata['section_registry'], 'section_registry'
-
-        return [k for k in OperationType.values() if k in self.config.keys()], 'default'
+        return [k for k in OperationType.values() if k in self.config.keys()], "default"
 
     def check_config(self):
         """check the configuration as much as we can as early as we can
 
         Raises:
             various exceptions if any checks fail
 
@@ -309,39 +345,54 @@
             for child_key in self.config[section_key].keys():
 
                 child = self.config[section_key][child_key]
 
                 self.instance_to_config[child_key] = child
 
                 if not NodeFactory.CLASS_KEY in child:
-                    raise ConfigurationError("No class key found in %s.%s" % (section_key,child_key))
+                    raise ConfigurationError("No class key found in %s.%s" % (section_key, child_key))
 
                 self.nodename_to_classname[child_key] = child[NodeFactory.CLASS_KEY]
 
                 unique_class_keys.add((child[NodeFactory.CLASS_KEY], child.get(NodeFactory.CLASS_PREFIX)))
 
-                for k in ['destination_pipeline', 'destination_models', 'destination_postprocesses', 'destination_writer']:
+                for k in [
+                    "destination_pipeline",
+                    "destination_models",
+                    "destination_postprocesses",
+                    "destination_writer",
+                ]:
                     if k in child:
-                        raise Exception("Do you have a old config file? You have %s. Nodes just have 'destinations':[] now", k)
+                        raise Exception(
+                            "Do you have a old config file? You have %s. Nodes just have 'destinations':[] now", k,
+                        )
 
         logging.info("OK: all class keys are present")
 
         # get class_prefixes by traversing node package
         unique_class_keys = self._traverse_node_package(unique_class_keys)
+        unique_nodes = set([x[0] for x in unique_class_keys])
 
         # check that each referenced class is registered in NodeFactory
+        # Regex pattern in `_traverse_node_package` should capture the right file (class prefix) to register
+        # node (class_key). Here we attempt to register any class that is not already registered.
         for class_key, class_prefix in unique_class_keys:
             if not NodeFactory().is_registered(class_key):
                 try:
-                    logging.info(f'attempting to register {class_key}')
+                    logging.info(f"attempting to register {class_key}")
                     self._register_class(class_key, class_prefix)
-                except:
-                    raise ConfigurationError(f"Cannot register node class {class_key}")
+                except Exception as exc:
+                    logging.exception(
+                        f"Cannot register node class {class_key} with prefix {class_prefix}", exc_info=True
+                    )
+        for class_key in unique_nodes:
+            if not NodeFactory().is_registered(class_key):
+                raise ConfigurationError(f"Cannot register node class {class_key}")
 
-        #check necessary_configs
+        # check necessary_configs
         for instance_name in self.nodename_to_classname:
             class_key = self.nodename_to_classname[instance_name]
 
             configuration_dict = self.instance_to_config[instance_name]
 
             instance = NodeFactory().instantiate(class_key, self, instance_name)
 
@@ -362,25 +413,24 @@
                 or a full path `path/to/module`.
 
         Returns:
             None - attempts to register the class with it's default name
         """
         # convert to string before checking if file
         if class_prefix is None:
-            class_prefix = ''
+            class_prefix = ""
 
         if os.path.isfile(class_prefix):
             modulename = self._import_file(class_key, class_prefix)
 
         # loading from module
         else:
-            if self.config_metadata:
-                if 'class_package' in self.config_metadata:
-                    class_package = self.config_metadata['class_package']
-                    prefix = '.'.join(filter(None, [class_package, class_prefix]))
+            if self.config_metadata and "class_package" in self.config_metadata:
+                class_package = self.config_metadata["class_package"]
+                prefix = ".".join(filter(None, [class_package, class_prefix]))
             else:
                 prefix = class_prefix
 
             modulename = importlib.import_module(prefix)
 
         clz = getattr(modulename, class_key)
         NodeFactory().register(None, clz)
@@ -412,16 +462,16 @@
         Returns:
             list of potential files to search for classes to register
         """
         # for now assume packages/top level only
         if CLASS_ENV_PACKAGE_KEY in os.environ:
             pkg_name = os.environ[CLASS_ENV_PACKAGE_KEY]
         elif self.config_metadata:
-            if 'class_package' in self.config_metadata:
-                pkg_name = self.config_metadata['class_package']
+            if "class_package" in self.config_metadata:
+                pkg_name = self.config_metadata["class_package"]
             else:
                 return []
         else:
             return []
         # look for path to module to find potential file candidates
         try:
             # if we are passed something like __init__.py, grab the package
@@ -430,15 +480,15 @@
             # if we have an actual package from pip install
             if not os.path.isdir(pkg_name):
                 pkg_name = os.path.dirname(importlib.import_module(pkg_name).__file__)
         except ModuleNotFoundError:
             logging.warning("Could not find module specified for external node configuration")
             return []
 
-        candidates = glob.glob(os.path.join(pkg_name, '**', '*.py'), recursive=True)
+        candidates = glob.glob(os.path.join(pkg_name, "**", "*.py"), recursive=True)
 
         return candidates
 
     def _traverse_node_package(self, unique_class_keys, overwrite=False):
         """Traverse node package to find classes in the DAG to register.
 
         Args:
@@ -447,19 +497,20 @@
 
         Returns:
             (class_name, class_prefix) tuples
         """
         class_keys_prefix = []
         candidates = self._get_file_candidates()
         for filename in candidates:
-            with open(filename, 'r') as f:
+            with open(filename, "r") as f:
                 src_str = f.read()
                 for class_key, class_key_prefix in unique_class_keys:
                     if (class_key_prefix is None) or (overwrite == True):
-                        pattern = "class\s" + class_key + "\(?.*\)?:\s"
+                        pattern = "class\s" + class_key + "(?:\(|:)"
+                        # pattern to look for strings of the form "class MyNode:" OR "class MyNode("
                         if re.search(pattern, src_str) is not None:
                             class_keys_prefix.append((class_key, filename))
                             continue
         for class_key, class_key_prefix in unique_class_keys:
             if class_key not in [x[0] for x in class_keys_prefix]:
                 class_keys_prefix.append((class_key, class_key_prefix))
         return class_keys_prefix
@@ -478,10 +529,12 @@
         # Here, we check next-level down and error out on first duplicate found
         all_keys = set()
         for key in self.config.keys():
             section_dict = self.config[key]
             self.__setattr__(key, section_dict)
             for k2 in section_dict.keys():
                 if k2 in all_keys:
-                    raise ConfigurationError("Operations must all have unique names in the configuration. Duplicate key: '%s'" % k2)
+                    raise ConfigurationError(
+                        "Operations must all have unique names in the configuration. Duplicate key: '%s'" % k2
+                    )
                 else:
                     all_keys.add(k2)
```

### Comparing `primrose-1.0.9/primrose/configuration/configuration_dag.py` & `primrose-2.0.0/primrose/configuration/configuration_dag.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-'''A class that creates a directed acyclic graph (DAG) and perhaps a number of checks,
+"""A class that creates a directed acyclic graph (DAG) and perhaps a number of checks,
 such as detecting cycles, orphans, and unrecognized nodes
 
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
-'''
+"""
 import logging
 import networkx as nx
 from primrose.configuration.util import OperationType, ConfigurationError
 import matplotlib.pyplot as plt
 from networkx.algorithms.shortest_paths.generic import has_path
 from primrose.node_factory import NodeFactory
 from primrose.base.conditional_path_node import AbstractConditionalPath
 
 
-class ConfigurationDag():
-
+class ConfigurationDag:
     def __init__(self, config):
         """instantiate ComfigurationDAG instance
 
         Args:
             config (Configuration): Configuration instance
 
         """
@@ -77,15 +76,21 @@
         Args:
             operation_type (OperationType): OperationType
 
         Returns:
             set of keys, if any, of the given operation type
 
         """
-        return set([k for k in self.node_map.keys() if self.node_map[k] == operation_type.value])
+        return set(
+            [
+                k
+                for k in self.node_map.keys()
+                if self.node_map[k] == operation_type.value
+            ]
+        )
 
     def upstream_nodes_of_type(self, target_node_name, operation_type):
         """get set of nodes of a given operation type (OperationType.reader, OperationType.writer etc)
             upstream of some given target node
 
         Args:
             operation_type (OperationType): OperationType
@@ -139,32 +144,35 @@
         cycles = None
         try:
             cycles = nx.find_cycle(self.G2)
             logging.info("cycles:" + str(cycles))
         except nx.exception.NetworkXNoCycle as e:
             # it throws an error if there are no cycles, the opposite of what we want
             if str(e) != "No cycle found.":
-                raise e # pragma: no cover
+                raise e  # pragma: no cover
             else:
                 logging.info("OK: no cycles found")
-        #to get here, we must have cycles!
+        # to get here, we must have cycles!
         if cycles:
             raise ConfigurationError("Cycle(s) found: %s" % str(cycles))
 
     def check_connected_components(self):
         """now we can count the number of connected components. >1 is problem
 
         Raises:
             ConfigurationError if multiuple connected components
 
         """
         connected_components = nx.connected_components(self.G)
         n = sum([1 for c in connected_components])
         if n > 1:
-            raise ConfigurationError("Found multiple connected components: %s" % str(list( nx.connected_components(self.G) )))
+            raise ConfigurationError(
+                "Found multiple connected components: %s"
+                % str(list(nx.connected_components(self.G)))
+            )
         else:
             logging.info("OK: 1 connected component")
 
     def upstream_keys(self, instance_name):
         """get list of keys (names of nodes in the DAG) that feed into instance_name node
 
         Args:
@@ -210,57 +218,67 @@
         some_postprocess_node = None
 
         # key to section type
         node_map = {}
 
         self.conditional_nodes = set()
 
-        #add the nodes to the graph:
+        # add the nodes to the graph:
         for section_key in self.config.keys():
 
             for key in self.config[section_key].keys():
                 logging.debug("Adding node '%s'" % key)
                 G.add_node(key)
                 G2.add_node(key)
                 node_names.add(key)
 
                 node_map[key] = section_key
 
                 # root out conditional nodes...
                 node_config = self.config[section_key][key]
-                node_class = node_config['class']
+                node_class = node_config["class"]
                 class_obj = NodeFactory().name_dict[node_class]
                 if issubclass(class_obj, AbstractConditionalPath):
                     self.conditional_nodes.add(key)
 
                 # cleanup section can be disconnected from rest of graph so let's keep track of these nodes
                 if section_key == OperationType.cleanup.value:
                     cleanup_nodes.add(key)
 
                 # hack: we are going to add an edge from a postprcocess step (any one) to cleanup nodes so they
                 # are not a separate connected component
-                if section_key == OperationType.postprocess.value and some_postprocess_node is None:
+                if (
+                    section_key == OperationType.postprocess.value
+                    and some_postprocess_node is None
+                ):
                     some_postprocess_node = key
 
         # add the edges
         for section_key in self.config.keys():
 
             for key in self.config[section_key].keys():
                 d = self.config[section_key][key]
 
-                if 'destinations' in d:
-                    for destination in d['destinations']:
+                if "destinations" in d:
+                    for destination in d["destinations"]:
 
                         if not isinstance(destination, str):
-                            raise ConfigurationError("Unrecognized destination type: %s" % destination)
+                            raise ConfigurationError(
+                                "Unrecognized destination type: %s" % destination
+                            )
 
                         if destination in node_map:
-                            ConfigurationDag.add_edge(G,G2,node_names,key,destination)
+                            ConfigurationDag.add_edge(
+                                G, G2, node_names, key, destination
+                            )
                         else:
-                            raise ConfigurationError("Did not find %s destination in %s.%s" % (destination, section_key, key))
+                            raise ConfigurationError(
+                                "Did not find %s destination in %s.%s"
+                                % (destination, section_key, key)
+                            )
 
         logging.info("OK: good referential integrity")
 
         self.G = G
         self.G2 = G2
         self.node_map = node_map
 
@@ -278,15 +296,24 @@
         """
         self.create_dag()
 
         self.check_connected_components()
 
         self.check_for_cycles()
 
-    def plot_dag(self, filename, traverser, node_size=500, label_font_size=12, text_angle=0, image_width=16, image_height=12):
+    def plot_dag(
+        self,
+        filename,
+        traverser,
+        node_size=500,
+        label_font_size=12,
+        text_angle=0,
+        image_width=16,
+        image_height=12,
+    ):
         """plot the DAG to image file
 
         Args:
             filename (str): path to write image to
             title (str): title to add to chart
             node_size (int): node size
             label_font_size (int): font size
@@ -297,72 +324,90 @@
         Returns:
             nothing. Saves image to file
 
         """
         # map nodes to a color for their operation type
         # https://stackoverflow.com/questions/27030473/how-to-set-colors-for-nodes-in-networkx-python
         color_map = []
-        colors = ['#fbb4ae','#b3cde3','#ccebc5','#decbe4','#fed9a6']
+        colors = ["#fbb4ae", "#b3cde3", "#ccebc5", "#decbe4", "#fed9a6"]
         for node in self.G2:
             if self.node_map[node] == OperationType.reader.value:
                 color_map.append(colors[0])
             elif self.node_map[node] == OperationType.pipeline.value:
                 color_map.append(colors[1])
             elif self.node_map[node] == OperationType.model.value:
                 color_map.append(colors[2])
             elif self.node_map[node] == OperationType.writer.value:
                 color_map.append(colors[3])
             else:
                 color_map.append(colors[4])
 
-        fig = plt.figure(figsize=(image_width,image_height))
+        fig = plt.figure(figsize=(image_width, image_height))
         ax = plt.subplot(111)
         ax.set_title(filename, fontsize=10)
 
         try:
             import pydot
             from networkx.drawing.nx_pydot import graphviz_layout
-        except ImportError: # pragma: no cover
+        except ImportError:  # pragma: no cover
             raise ImportError(
                 "This example needs Graphviz and pydot."
                 "Please refer to the Plotting requirements in the README"
             )
 
         # pos = nx.spring_layout(G)
         # pos = nx.circular_layout(G)
         # pos = nx.kamada_kawai_layout(G)
         # pos = nx.shell_layout(G)
         # pos = nx.spectral_layout(G)
-        pos = graphviz_layout(self.G2, prog='dot') #, prog='twopi', args='')
+        pos = graphviz_layout(self.G2, prog="dot")  # , prog='twopi', args='')
 
-        nx.draw(self.G2, pos, node_size=node_size,node_color = color_map, edge_color='#939393', font_size=8, font_weight='bold')
+        nx.draw(
+            self.G2,
+            pos,
+            node_size=node_size,
+            node_color=color_map,
+            edge_color="#939393",
+            font_size=8,
+            font_weight="bold",
+        )
         # nx.draw_networkx_nodes(G, pos, node_color='b', node_size=500, alpha=0.8)
 
         if len(self.conditional_nodes) > 0:
-            cnodes = nx.draw_networkx_nodes(self.G2, pos, node_color='#e6b655', node_size=1.5*node_size, alpha=0.8, node_shape="D", nodelist=list(self.conditional_nodes))
-            cnodes.set_edgecolor('red')
+            cnodes = nx.draw_networkx_nodes(
+                self.G2,
+                pos,
+                node_color="#e6b655",
+                node_size=1.5 * node_size,
+                alpha=0.8,
+                node_shape="D",
+                nodelist=list(self.conditional_nodes),
+            )
+            cnodes.set_edgecolor("red")
 
-#        nx.draw_networkx_labels(self.G2,pos, font_size=9)
+        #        nx.draw_networkx_labels(self.G2,pos, font_size=9)
 
-        text = nx.draw_networkx_labels(self.G2,pos,with_labels=False, font_size=label_font_size) #, bbox=Bbox.from_bounds(x0, y0, 20,30)) #, wrap=True)
+        text = nx.draw_networkx_labels(
+            self.G2, pos, font_size=label_font_size
+        )
 
         if traverser:
-            #map node name to sequence number
+            # map node name to sequence number
             sequence = traverser.traversal_list()
-            idx = list(range(1,len(sequence) + 1))
-            d = dict(zip(sequence,idx))
+            idx = list(range(1, len(sequence) + 1))
+            d = dict(zip(sequence, idx))
 
             # let's plot the sequence numner above the node. How far above it?
-            ys = [t._y for _,t in text.items()]
+            ys = [t._y for _, t in text.items()]
             ysrange = max(ys) - min(ys)
             offset = 0.02 * abs(ysrange)
 
-        for _,t in text.items():
+        for _, t in text.items():
             t.set_rotation(text_angle)
 
             if traverser:
-                plt.text(t._x, t._y + offset, d[t._text], fontsize=24, color='red')
+                plt.text(t._x, t._y + offset, d[t._text], fontsize=24, color="red")
 
-        plt.axis('off')
+        plt.axis("off")
         plt.tight_layout()
         plt.savefig(filename, format="PNG")
         logging.info("Graph written to %s" % filename)
```

### Comparing `primrose-1.0.9/primrose/dag_runner.py` & `primrose-2.0.0/primrose/dag_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 
 """
 from primrose.data_object import DataObject
 import networkx as nx
 import os
 import logging
 import collections
+import traceback
 from primrose.node_factory import NodeFactory
 from primrose.configuration.configuration import OperationType
 from primrose.notification_utils import get_notification_client
 from primrose.dag.traverser_factory import TraverserFactory
 from primrose.base.conditional_path_node import AbstractConditionalPath
 
 
-class DagRunner():
+class DagRunner:
     """class that runs the DAG: gets the list of nodes to traverse and then asks them to run"""
 
     def __init__(self, configuration):
         """instantiate the DagRunner
 
         Args:
             configuration (Configuration): configuration object defined in primrose/Configuration with validated inputs
@@ -28,35 +29,37 @@
 
             instance_name (str): how the code knows where it is from
 
         """
         self.configuration = configuration
         self.dag = self.configuration.dag
 
-        if configuration.config_metadata and 'traverser' in configuration.config_metadata:
-            self.dag_traverser = TraverserFactory().instantiate(configuration.config_metadata['traverser'], configuration)
+        if configuration.config_metadata and "traverser" in configuration.config_metadata:
+            self.dag_traverser = TraverserFactory().instantiate(
+                configuration.config_metadata["traverser"], configuration
+            )
         else:
             self.dag_traverser = TraverserFactory().default_traverser(configuration)
 
         logging.info("Traverser is of class %s", self.dag_traverser.__class__)
 
     def create_data_object(self):
         """restore data_object from cache
 
         Returns:
             data_object (DataObject)
 
         """
-        if self.configuration.config_metadata and 'data_object' in self.configuration.config_metadata:
+        if self.configuration.config_metadata and "data_object" in self.configuration.config_metadata:
 
-            cfg = self.configuration.config_metadata['data_object']
+            cfg = self.configuration.config_metadata["data_object"]
 
-            if "read_from_cache" in cfg and cfg['read_from_cache']:
+            if "read_from_cache" in cfg and cfg["read_from_cache"]:
                 # we can assume that read_filename exists due to configuration checks
-                filename = cfg['read_filename']
+                filename = cfg["read_filename"]
                 assert os.path.exists(filename)
 
                 logging.info("Reading DataObject from cache " + filename)
                 return DataObject.read_from_cache(filename)
 
         data_object = DataObject(self.configuration)
 
@@ -69,19 +72,19 @@
             data_object (DataObject): instance of DataObject
 
         Returns:
             whether it was cached (bool)
 
         """
 
-        if self.configuration.config_metadata and 'data_object' in self.configuration.config_metadata:
+        if self.configuration.config_metadata and "data_object" in self.configuration.config_metadata:
 
-            cfg = self.configuration.config_metadata['data_object']
+            cfg = self.configuration.config_metadata["data_object"]
 
-            if "write_to_cache" in cfg and cfg['write_to_cache']:
+            if "write_to_cache" in cfg and cfg["write_to_cache"]:
 
                 assert "write_filename" in cfg
                 filename = cfg["write_filename"]
                 data_object.write_to_cache(filename)
                 return True
 
         return False
@@ -124,15 +127,15 @@
         Raises:
             Exception if there are dupes in the sequence, or if nodes are not in config, or we have nodes from other sections.
             The latter can happen if we mix up nodes from sections. That is, suppose we have section1 (1 node) and section 2 (2 nodes) and
             we want to run section2 and then section1 and we receive sequence [section2_node1, section1_node1, section2_node2], it will
             complain about the partition [section2_node1, section1_node1] [section2_node2] as they are mixed from sections.
 
         """
-        self. initial_check_sequence(sequence)
+        self.initial_check_sequence(sequence)
 
         # it might be that traverser provides a sequence of all config nodes and we only want to run those in section2
         # Thus, first, let's only consider the nodes in that section
         nodes_to_run = set()
         sections, source = self.configuration.sections_in_order()
 
         logging.info("Taking nodes to run from " + source)
@@ -145,31 +148,31 @@
             self.check_for_upstream(sequence)
             return sequence
 
         filtered_sequence = []
 
         for section_name in sections:
 
-            #get a set of all nodes in this section
+            # get a set of all nodes in this section
             this_section = set(self.configuration.config[section_name].keys())
 
             n = len(this_section)
 
             # do we have enough nodes in sequence to compare against?
             if len(sequence) >= n:
 
                 subset = sequence[:n]
 
-                #logic: the set of first n nodes of sequence should match this set of this_section
+                # logic: the set of first n nodes of sequence should match this set of this_section
                 if this_section == set(subset):
 
-                    #these nodes passed the checks
+                    # these nodes passed the checks
                     filtered_sequence.extend(sequence[:n])
 
-                    #pop off the first n nodes and repeat until we've gone through each section
+                    # pop off the first n nodes and repeat until we've gone through each section
                     sequence = sequence[n:]
                 else:
                     # We can't get here if there is only 1 section to run as we raise on dupes and importantly, we now filter on sections earlier.
                     # This means that we cannot pull in nodes from a later section. That is, suppose the sequence was
                     # [section2_node1, section1_node1, section2_node2] and we wanted to run section 2 only (which has two nodes).
                     # We wouldn't grab first two nodes of sequence [section2_node1, section1_node1] which is what code below was
                     # meant to detect, but instead we would get [section2_node1, section2_node2] from the section filter.
@@ -200,16 +203,16 @@
             Exception if any upstream paths found
 
         """
 
         for idx_from in range(len(sequence)):
             for idx_to in range(len(sequence)):
                 if idx_from > idx_to:
-                    if self.configuration.dag.paths(sequence[idx_from],  sequence[idx_to]):
-                        msg = "Upstream path found, from %s to %s" % (sequence[idx_from], sequence[idx_to])
+                    if self.configuration.dag.paths(sequence[idx_from], sequence[idx_to]):
+                        msg = "Upstream path found, from %s to %s" % (sequence[idx_from], sequence[idx_to],)
                         raise Exception(msg)
         return False
 
     def run(self, dry_run=False):
         """run the whole DAG. Optonally, you can call dry_run=True
             which will log what would be run and in what order
             but not actually run it
@@ -229,72 +232,73 @@
         sequence = self.filter_sequence(candidate_sequence)
 
         if len(candidate_sequence) > len(sequence):
             logging.info("Sequence of nodes to be run: %s", sequence)
 
         pruned_nodes = set()
 
-        if (self.configuration.config_metadata and
-            'notify_on_error' in self.configuration.config_metadata):
+        if self.configuration.config_metadata and "notify_on_error" in self.configuration.config_metadata:
             try:
-                params = self.configuration.config_metadata['notify_on_error']
+                params = self.configuration.config_metadata["notify_on_error"]
+                slack_exception_label = params.get("message", "Job error")
                 client = get_notification_client(params)
 
             except Exception as error:
-                msg = (
-                    'Error trying to instantiate notification client.'
-                    'Check class name and parameters"'
-                )
+                msg = "Error trying to instantiate notification client." 'Check class name and parameters"'
                 logging.error(error)
-                raise(msg)
+                raise (msg)
         else:
             client = None
 
         for i, node in enumerate(sequence):
 
             if node in pruned_nodes:
                 logging.info("Skipping pruned node " + node)
                 continue
 
             section = self.dag.node_map[node]
             class_name = self.configuration.nodename_to_classname[node]
 
             if dry_run:
-                logging.info("DRY RUN %s: would run node %s of type %s and class %s", i, node, section, class_name)
+                logging.info(
+                    "DRY RUN %s: would run node %s of type %s and class %s", i, node, section, class_name,
+                )
                 continue
             else:
-                logging.info("received node %s of type %s and class %s", node, section, class_name)
+                logging.info(
+                    "received node %s of type %s and class %s", node, section, class_name,
+                )
 
             try:
                 node_instance = NodeFactory().instantiate(class_name, self.configuration, node)
             except Exception as e:
                 msg = "Issue instantiating %s and class %s" % (node, class_name)
                 logging.error(msg)
                 if client:
-                    client.post_message(msg)
+                    client.post_message(f"{slack_exception_label}: {msg}")
                 raise Exception(msg)
 
             try:
                 data_object, terminate = node_instance.run(data_object)
 
                 if isinstance(node_instance, AbstractConditionalPath):
                     to_prune = node_instance.all_nodes_to_prune()
                     if to_prune:
                         pruned_nodes.update(to_prune)
 
             except Exception as e:
                 msg = "Issue with %s" % node
                 logging.error(msg)
                 if client:
-                    client.post_message(msg)
+                    client.post_message(f"{slack_exception_label}: {msg}\n{traceback.format_exc()}")
                 raise e
 
             if terminate:
                 logging.info("Terminating early due to signal from %s", node)
                 if client:
-                    client.post_message(msg)
+                    client.post_message(f"{slack_exception_label}: {msg}")
                 break
 
         self.cache_data_object(data_object)
 
         logging.info("All done. Bye bye!")
         return data_object
```

### Comparing `primrose-1.0.9/primrose/models/sklearn_classifier_model.py` & `primrose-2.0.0/primrose/models/sklearn_classifier_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from sklearn.metrics import recall_score
 from sklearn.metrics import precision_score
 from sklearn.metrics import accuracy_score
 from sklearn.metrics import auc
 from primrose.readers.dill_reader import DillReader
 from primrose.models.sklearn_model import SklearnModel
 
-class SklearnClassifierModel(SklearnModel):
 
+class SklearnClassifierModel(SklearnModel):
     @staticmethod
     def necessary_config(node_config):
         """Return a list of necessary configuration keys
 
         Args:
             node_config (dict): set of parameters / attributes for the node
 
@@ -33,15 +33,23 @@
             grid_search_scoring: scoring function name from sklearn CV docs
             cv_folds: number of CV folds
 
         Returns:
             set of required keys
 
         """
-        return set(["model_parameters", "mode", "sklearn_classifier_name", "grid_search_scoring", "cv_folds"])
+        return set(
+            [
+                "model_parameters",
+                "mode",
+                "sklearn_classifier_name",
+                "grid_search_scoring",
+                "cv_folds",
+            ]
+        )
 
     def train_model(self, data_object):
         """train the model using CV, according to user specified options
 
         Args:
             data_object (DataObject): instance of DataObject
 
@@ -49,36 +57,40 @@
             Nothing
 
         """
         X_train, y_train, X_test, y_test = self._get_data(data_object)
 
         logging.info("Fitting model")
 
-        self.model = SklearnModel._instantiate_model(self.node_config['sklearn_classifier_name'], args=None)
-
-        self.model = GridSearchCV(self.model,
-                                self.node_config['model_parameters'],
-                                n_jobs=-1,
-                                scoring=self.node_config['grid_search_scoring'],
-                                verbose=2,
-                                cv=self.node_config['cv_folds'],
-                                refit=True)
+        self.model = SklearnModel._instantiate_model(
+            self.node_config["sklearn_classifier_name"], args=None
+        )
+
+        self.model = GridSearchCV(
+            self.model,
+            self.node_config["model_parameters"],
+            n_jobs=-1,
+            scoring=self.node_config["grid_search_scoring"],
+            verbose=2,
+            cv=self.node_config["cv_folds"],
+            refit=True,
+        )
 
         self.model.fit(X_train, y_train)
 
-        data_object.add(self, self.model.best_estimator_, 'model')
+        data_object.add(self, self.model.best_estimator_, "model")
 
         return data_object
 
     def eval_model(self, data_object):
         """Evaluate model perfomance on a labeled testing dataset
-        
+
         Returns:
             data_object (DataObject): instance of DataObject
-        
+
         """
 
         if self.model is None:
             self.model = self.load_model(data_object)
 
         logging.info("Evaluating model performance on testing data")
 
@@ -90,57 +102,72 @@
         model_predictions = model_predictions.astype(int)
 
         model_f1 = f1_score(y_test, model_predictions, labels=None, pos_label=1)
         recall = recall_score(y_test, model_predictions, labels=None, pos_label=1)
         prec = precision_score(y_test, model_predictions, labels=None, pos_label=1)
         accuracy = accuracy_score(y_test, model_predictions)
 
-        logging.info('positive class fraction: {}'.format(float(sum(y_test)) / len(y_test)))
-        logging.info('positive class predicted fraction: {}'.format(float(sum(model_predictions)) / len(y_test)))
-        logging.info('f1: {}, recall: {}, precision: {}, accuracy: {}'.format(model_f1, recall, prec, accuracy))
+        logging.info(
+            "positive class fraction: {}".format(float(sum(y_test)) / len(y_test))
+        )
+        logging.info(
+            "positive class predicted fraction: {}".format(
+                float(sum(model_predictions)) / len(y_test)
+            )
+        )
+        logging.info(
+            "f1: {}, recall: {}, precision: {}, accuracy: {}".format(
+                model_f1, recall, prec, accuracy
+            )
+        )
         roc_auc = self._get_roc_score(y_test, model_probability)
-        logging.info('AUC: {}'.format(roc_auc))
+        logging.info("AUC: {}".format(roc_auc))
 
         # write performance and timing information to scores attribute
-        self.scores['auc'] = roc_auc
-        self.scores['f1'] = model_f1
-        self.scores['recall'] = recall  # Recall=TP/(TP+FN)
-        self.scores['precision'] = prec  # Precison=TP/(TP+FP)
-        self.scores['positive_class_fraction'] = float(sum(y_test)) / len(y_test)
-        self.scores['predicted_class_fraction'] = float(sum(model_predictions)) / len(y_test)
-        self.scores['eval_time'] = datetime.datetime.now()
+        self.scores["auc"] = roc_auc
+        self.scores["f1"] = model_f1
+        self.scores["recall"] = recall  # Recall=TP/(TP+FN)
+        self.scores["precision"] = prec  # Precison=TP/(TP+FP)
+        self.scores["positive_class_fraction"] = float(sum(y_test)) / len(y_test)
+        self.scores["predicted_class_fraction"] = float(sum(model_predictions)) / len(
+            y_test
+        )
+        self.scores["eval_time"] = datetime.datetime.now()
 
         return data_object
 
     def predict(self, data_object):
         """Make distance-based predictions using the prebuilt matrix
 
         Args:
             data_object: DataObject instance
             load_model: load model object from gcs or not
 
-        Returns: 
+        Returns:
             data_object with prediction data added
 
         """
 
         if self.model is None:
             self.model = self.load_model(data_object)
 
         X_train, y_train, X_test, y_test = self._get_data(data_object)
 
         predictions = self.model.predict(X_test)
 
         # get the upstream target_encoder if it exists
-        data = data_object.get_filtered_upstream_data(self.instance_name, filter_for_key='target_encoder')
-
-        if 'target_encoder' in data:
-            logging.info("Reversing label encoding")
-            predictions = data['target_encoder'].inverse_transform(predictions)
+        data = data_object.get_filtered_upstream_data(
+            self.instance_name, filter_for_key="target_encoder"
+        )
+
+        if data:
+            if "target_encoder" in data:
+                logging.info("Reversing label encoding")
+                predictions = data["target_encoder"].inverse_transform(predictions)
 
         # get original data frame and tack on column of predictions
         data_out = X_test
-        data_out['predictions'] = predictions
+        data_out["predictions"] = predictions
 
-        data_object.add(self, data_out, 'predictions')
+        data_object.add(self, data_out, "predictions")
 
         return data_object
```

### Comparing `primrose-1.0.9/primrose/models/sklearn_regression_model.py` & `primrose-2.0.0/primrose/models/sklearn_regression_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 import logging
 from primrose.models.sklearn_model import SklearnModel
 
-class SklearnRegressionModel(SklearnModel):
 
+class SklearnRegressionModel(SklearnModel):
     @staticmethod
     def necessary_config(node_config):
         """Return a list of necessary configuration keys
 
         Note:
             While you might expect `model` here, we do not need it when in predict or eval mode as the model is cached, only in train
 
@@ -24,13 +24,13 @@
 
     def fit_training_data(self):
         """fit training data to model"""
         self.model.fit(self.X_train, self.y_train)
 
     def get_scores(self):
         """get the scores for y_test
-        
+
         Returns:
             dictionary of scores
-        
+
         """
         return SklearnModel.evaluate_regression_metrics(self.y_test, self.predictions)
```

### Comparing `primrose-1.0.9/primrose/models/sklearn_model.py` & `primrose-2.0.0/primrose/models/sklearn_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from primrose.base.model import AbstractModel
 import importlib
 import logging
 from sklearn.metrics import roc_curve, auc
 from sklearn import metrics
 import datetime
 
-class SklearnModel(AbstractModel):
 
+class SklearnModel(AbstractModel):
     def __init__(self, configuration, instance_name):
         """A Sklearn-based model to train, evaluate and predict on dataframe feature data
 
         Args:
             configuration (Configuration): user defined configuration object
             instance_name (str): name to identify the correct configuration key
 
@@ -33,20 +33,24 @@
 
         Returns:
             Sklearn model
 
         """
 
         # check for a valid pipeline object inside the data object
-        model = data_object.get_filtered_upstream_data(self.instance_name, filter_for_key='reader_data')['reader_data']
+        model = data_object.get_filtered_upstream_data(
+            self.instance_name, filter_for_key="reader_data"
+        )["reader_data"]
 
         if model is None:
-            raise Exception('No valid upstream model found in the data object for model.')
+            raise Exception(
+                "No valid upstream model found in the data object for model."
+            )
 
-        logging.info('Model successfully loaded from upstream data_object.')
+        logging.info("Model successfully loaded from upstream data_object.")
 
         return model
 
     @staticmethod
     def _instantiate_model(classname, args):
         """instantiates a Sklearn model from class name
 
@@ -55,21 +59,25 @@
 
             args (dict): dictionary of arguments/parameters for model instantiation
 
         Returns:
             instance of a sklearn mode
 
         """
-        sk_module_name, sk_model_name = classname.split('.')
-        sk_module = importlib.import_module('sklearn.{}'.format(sk_module_name))
+        sk_module_name, sk_model_name = classname.split(".")
+        sk_module = importlib.import_module("sklearn.{}".format(sk_module_name))
 
         try:
             m = getattr(sk_module, sk_model_name)
         except AttributeError:
-            raise Exception('Sklearn model {} not found in {} module'.format(sk_model_name, sk_module_name))
+            raise Exception(
+                "Sklearn model {} not found in {} module".format(
+                    sk_model_name, sk_module_name
+                )
+            )
         logging.info("Instantiating model " + classname)
         if args:
             return m(**args)
         else:
             return m()
 
     @staticmethod
@@ -92,148 +100,161 @@
         """get the upstream data, split into X and Y from config, return data frame
 
         Returns:
             dataframe (dataframe)
 
         """
 
-        # get upstream data dict which contains the subkey data_test
-        data = data_object.get_filtered_upstream_data(self.instance_name, 'data_test')
+        # get upstream data dict which contains the subkey data_test or data_train
+        data = data_object.get_filtered_upstream_data(
+            self.instance_name, "data_test"
+        ) or data_object.get_filtered_upstream_data(self.instance_name, "data_train")
 
         X_train = None
-        if 'data_train' in data:
-            X_train = data['data_train']
-            if 'features' in self.node_config:
-                X_train = X_train[self.node_config['features']]
+        if "data_train" in data:
+            X_train = data["data_train"]
+            if "features" in self.node_config:
+                X_train = X_train[self.node_config["features"]]
 
         y_train = None
-        if 'target_train' in data:
-            y_train = data['target_train']
+        if "target_train" in data:
+            y_train = data["target_train"]
 
         X_test = None
-        if 'data_test' in data:
-            X_test = data['data_test']
-            if 'features' in self.node_config:
-                X_test = X_test[self.node_config['features']]
+        if "data_test" in data:
+            X_test = data["data_test"]
+            if "features" in self.node_config:
+                X_test = X_test[self.node_config["features"]]
 
         y_test = None
-        if 'target_test' in data:
-            y_test = data['target_test']
+        if "target_test" in data:
+            y_test = data["target_test"]
 
         def size(obj):
             if obj is None:
                 return None
-            return(str(obj.shape))
+            return str(obj.shape)
 
-        logging.info("Get_data, X_train %s, y_train %s, X_test %s, y_test %s", size(X_train), size(y_train), size(X_test), size(y_test))
+        logging.info(
+            "Get_data, X_train %s, y_train %s, X_test %s, y_test %s",
+            size(X_train),
+            size(y_train),
+            size(X_test),
+            size(y_test),
+        )
 
         return X_train, y_train, X_test, y_test
 
     def train_model(self, data_object):
         """train the model
 
         Args:
             data_object (DataObject): instance of DataObject
 
         Returns:
             data_object (DataObject): instance of DataObject
 
         """
-        self.X_train, self.y_train, self.X_test, self.y_test = self._get_data(data_object)
+        self.X_train, self.y_train, self.X_test, self.y_test = self._get_data(
+            data_object
+        )
 
         args = None
-        if 'args' in self.node_config['model']:
-            args = self.node_config['model']['args']
+        if "args" in self.node_config["model"]:
+            args = self.node_config["model"]["args"]
 
-        self.model = SklearnModel._instantiate_model(self.node_config['model']['class'], args)
+        self.model = self._instantiate_model(self.node_config["model"]["class"], args)
 
         logging.info("Fitting model")
-        self.fit_training_data() #delegate down as args to self.model.fit() vary by model
+        self.fit_training_data()  # delegate down as args to self.model.fit() vary by model
 
-        data_object.add(self, self.model, 'model')
+        data_object.add(self, self.model, "model")
 
         return data_object
 
     def _make_predictions(self, data_object):
         """Make predictions from X_test
 
         Args:
             data_object (DataObject): instance of DataObject
 
         Returns:
             nothing. Predictions stored in self.predictions
 
         """
-        if hasattr(self, 'predictions') and self.predictions is not None:
+        if hasattr(self, "predictions") and self.predictions is not None:
             return
 
         if self.model is None:
             self.model = self.load_model(data_object)
 
-        self.X_train, self.y_train, self.X_test, self.y_test = self._get_data(data_object)
+        self.X_train, self.y_train, self.X_test, self.y_test = self._get_data(
+            data_object
+        )
 
         logging.info("Making predictions with model")
         self.predictions = self.model.predict(self.X_test)
 
     def predict(self, data_object, load_model=False, use_serial=False):
         """Predict y_test from X_test
 
         Args:
             data_object (DataObject): instance of DataObject
 
             load_model: load model object from gcs or not
 
-        Returns: 
+        Returns:
             data_object (DataObject): instance of DataObject
 
         """
         self._make_predictions(data_object)
 
         data = self.X_test
-        data['predictions'] = self.predictions
+        data["predictions"] = self.predictions
         if self.y_test is not None:
-            data['actual'] = self.y_test
+            data["actual"] = self.y_test
 
         data_object.add(self, data)
         return data_object
 
     def eval_model(self, data_object, load_model=False):
         """evalute a model by getting the scores
 
         Returns:
             data_object (DataObject): instance of DataObject
 
         """
         self._make_predictions(data_object)
 
         logging.info("Evaluating metrics")
-        scores = self.get_scores() #delegate down as appropriate metrics vary by model
-        scores['eval_time'] = datetime.datetime.now()
+        scores = self.get_scores()  # delegate down as appropriate metrics vary by model
+        scores["eval_time"] = datetime.datetime.now()
         logging.info("Scores" + str(scores))
 
         data_object.add(self, scores, "scores")
         return data_object
 
-
     @staticmethod
     def evaluate_no_ground_truth_classifier_metrics(X, labels):
         """Compute a set of metric for a classifier where there is no ground truth
 
         Args:
             X (datafframe): the data
             labels: the predicted classes
 
         Returns:
             dictionary of score name: value
 
         """
         scores = {}
-        scores['Silhouette Score']         = metrics.silhouette_score(X, labels, metric='euclidean')
-        scores['Calinski Harabasz Score']  = metrics.calinski_harabasz_score(X, labels)
-        scores['Davies Bouldin Score']     = metrics.davies_bouldin_score(X, labels)
+        scores["Silhouette Score"] = metrics.silhouette_score(
+            X, labels, metric="euclidean"
+        )
+        scores["Calinski Harabasz Score"] = metrics.calinski_harabasz_score(X, labels)
+        scores["Davies Bouldin Score"] = metrics.davies_bouldin_score(X, labels)
         return scores
 
     @staticmethod
     def evaluate_regression_metrics(actual, predictions):
         """compute set of metrics for a regression
 
         Args:
@@ -241,15 +262,21 @@
             predictions: vector of predictions
 
         Returns:
             dictionary of score name: value
 
         """
         scores = {}
-        scores['Explained variance']       = metrics.explained_variance_score(actual, predictions)
-        scores['Max error']                = metrics.max_error(actual, predictions)
-        scores['Mean absolute error']      = metrics.mean_absolute_error(actual, predictions)
-        scores['MSE']                      = metrics.mean_squared_error(actual, predictions)
-        scores['Mean squared log error']   = metrics.mean_squared_log_error(actual, predictions)
-        scores['Mean absolute error']      = metrics.median_absolute_error(actual, predictions)
-        scores['R2']                       = metrics.r2_score(actual, predictions)
-        return scores
+        scores["Explained variance"] = metrics.explained_variance_score(
+            actual, predictions
+        )
+        scores["Max error"] = metrics.max_error(actual, predictions)
+        scores["Mean absolute error"] = metrics.mean_absolute_error(actual, predictions)
+        scores["MSE"] = metrics.mean_squared_error(actual, predictions)
+        scores["Mean squared log error"] = metrics.mean_squared_log_error(
+            actual, predictions
+        )
+        scores["Mean absolute error"] = metrics.median_absolute_error(
+            actual, predictions
+        )
+        scores["R2"] = metrics.r2_score(actual, predictions)
+        return scores
```

### Comparing `primrose-1.0.9/primrose/models/minimal_search_engine.py` & `primrose-2.0.0/primrose/models/minimal_search_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 from nltk import ngrams
 from primrose.base.search_engine import AbstractSearchEngine
 from nltk import WordNetLemmatizer
 
+
 class MinimalSearchEngine(AbstractSearchEngine):
     """simple TFIDF search engine"""
 
     def __init__(self, configuration, instance_name):
         """instantiate the search engine
 
         Args:
@@ -19,15 +20,15 @@
             instance_name (str): name of instance
 
         """
         AbstractSearchEngine.__init__(self, configuration, instance_name)
         self.lemmatizer = WordNetLemmatizer()
 
     def tokenize(self, s, stopwords=[], add_ngrams=True):
-        """ tokenize a string document, optimized for recipe names given default stopwords and other
+        """tokenize a string document, optimized for recipe names given default stopwords and other
             string cleanup operations
 
         Args:
             s (str): some document string
             stopwords (list): list of stopwords
             add_ngrams (bool): whehter to include ngrams on tokens
```

### Comparing `primrose-1.0.9/primrose/node_factory.py` & `primrose-2.0.0/primrose/node_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,16 +22,18 @@
 from primrose.readers.postgres_reader import PostgresReader
 
 from primrose.conditionalpath.simple_switch import SimpleSwitch
 
 from primrose.pipelines.dataframe_joiner import DataFrameJoiner
 from primrose.pipelines.encode_train_test_split import EncodeTrainTestSplit
 from primrose.pipelines.train_test_split import TrainTestSplit
-from primrose.pipelines.sklearn_preprocessing_pipeline import SklearnPreprocessingPipeline
-
+from primrose.pipelines.sklearn_preprocessing_pipeline import (
+    SklearnPreprocessingPipeline,
+)
+from primrose.pipelines.transformer_pipeline import TransformerPipeline
 from primrose.models.sklearn_classifier_model import SklearnClassifierModel
 from primrose.models.sklearn_cluster_model import SklearnClusterModel
 from primrose.models.sklearn_regression_model import SklearnRegressionModel
 
 from primrose.notifications.success_notification import ClientNotification
 
 from primrose.writers.csv_writer import CsvWriter
@@ -41,26 +43,27 @@
 from primrose.writers.s3_writer import S3Writer
 
 from primrose.dataviz.cluster_plotter import ClusterPlotter
 
 from primrose.cleanup.logging_success import LoggingSuccess
 from primrose.readers.r_reader import RReader
 
+
 class NodeFactory:
     """Singleton Factory where one can register objects/classes for instantiation"""
-    #https://python-3-patterns-idioms-test.readthedocs.io/en/latest/Singleton.html
+
+    # https://python-3-patterns-idioms-test.readthedocs.io/en/latest/Singleton.html
 
     instance = None
 
     CLASS_KEY = "class"
     CLASS_PREFIX = "class_prefix"
 
     def __init__(self):
-        """instantiate the factory but as a singleton. The guard raails are here
-        """
+        """instantiate the factory but as a singleton. The guard raails are here"""
         # where the magic happens, only one instance allowed:
         if not NodeFactory.instance:
             NodeFactory.instance = NodeFactory.__HiddenFactory()
 
     def __getattr__(self, name):
         """getattr with instance name
 
@@ -74,40 +77,43 @@
         return getattr(self.instance, name)
 
     class __HiddenFactory:
         """actual factory where registry and instantiation happens"""
 
         def __init__(self):
             """instantiate the HiddenFactory"""
-            self.name_dict = {'CsvReader': CsvReader,
-                'SQLiteReader': SQLiteReader,
-                'MySQLReader': MySQLReader,
-                'PostgresReader': PostgresReader,
-                'GcsDillReader': GcsDillReader,
-                'DillReader': DillReader,
-                'Deserializer': Deserializer,
-                'GcsDeserializer': GcsDeserializer,
-                'DataFrameJoiner': DataFrameJoiner,
-                'EncodeTrainTestSplit': EncodeTrainTestSplit,
-                'TrainTestSplit': TrainTestSplit,
-                'CsvWriter': CsvWriter,
-                'FileWriter': FileWriter,
-                'DillWriter': DillWriter,
-                'Serializer': Serializer,
-                'S3Writer': S3Writer,
-                'SklearnClassifierModel': SklearnClassifierModel,
-                'LoggingSuccess': LoggingSuccess,
-                'ClusterPlotter': ClusterPlotter,
-                'SklearnClusterModel': SklearnClusterModel,
-                'SklearnPreprocessingPipeline': SklearnPreprocessingPipeline,
-                'SklearnDatasetReader': SklearnDatasetReader,
-                'SklearnRegressionModel': SklearnRegressionModel,
-                'SimpleSwitch': SimpleSwitch,
-                'ClientNotification': ClientNotification,
-                'RReader': RReader}
+            self.name_dict = {
+                "CsvReader": CsvReader,
+                "SQLiteReader": SQLiteReader,
+                "MySQLReader": MySQLReader,
+                "PostgresReader": PostgresReader,
+                "GcsDillReader": GcsDillReader,
+                "DillReader": DillReader,
+                "Deserializer": Deserializer,
+                "GcsDeserializer": GcsDeserializer,
+                "DataFrameJoiner": DataFrameJoiner,
+                "EncodeTrainTestSplit": EncodeTrainTestSplit,
+                "TrainTestSplit": TrainTestSplit,
+                "CsvWriter": CsvWriter,
+                "FileWriter": FileWriter,
+                "DillWriter": DillWriter,
+                "Serializer": Serializer,
+                "S3Writer": S3Writer,
+                "SklearnClassifierModel": SklearnClassifierModel,
+                "LoggingSuccess": LoggingSuccess,
+                "ClusterPlotter": ClusterPlotter,
+                "SklearnClusterModel": SklearnClusterModel,
+                "SklearnPreprocessingPipeline": SklearnPreprocessingPipeline,
+                "SklearnDatasetReader": SklearnDatasetReader,
+                "SklearnRegressionModel": SklearnRegressionModel,
+                "SimpleSwitch": SimpleSwitch,
+                "TransformerPipeline": TransformerPipeline,
+                "ClientNotification": ClientNotification,
+                "RReader": RReader,
+            }
 
         def register(self, key, class_obj, raise_on_overwrite=False):
             """Registering class_obj with key
 
             Args:
                 key (str): key such as class name, e.g. 'BQWriter'
                 class_obj (class obj), e.g. BQWriter
@@ -116,21 +122,25 @@
                 nothing. Side effect is to register the class
 
             """
             if raise_on_overwrite and key in self.name_dict:
                 raise Exception("Node already exist with the key " + key)
 
             if not (inspect.isclass(class_obj) and issubclass(class_obj, AbstractNode)):
-                raise Exception("NodeFactory can only register classes that implement AbstractNode")
+                raise Exception(
+                    "NodeFactory can only register classes that implement AbstractNode"
+                )
 
             if key is None:
                 try:
                     key = class_obj.__name__
                 except AttributeError as e:
-                    raise Exception(f"Cannot register {class_obj}, no __name__ attribute found. Please explicity specify a name when registering this class.")
+                    raise Exception(
+                        f"Cannot register {class_obj}, no __name__ attribute found. Please explicity specify a name when registering this class."
+                    )
 
             self.name_dict[key] = class_obj
             logging.debug("Registered %s : %s" % (key, class_obj))
 
         def is_registered(self, class_key):
             """is this class registered?
 
@@ -156,24 +166,24 @@
             if key in self.name_dict:
                 del self.name_dict[key]
                 logging.info("Unregistered %s", key)
             else:
                 raise Exception("Key not found %s" % key)
 
         def instantiate(self, class_name, configuration, instance_name):
-            '''instantiate instances of node, given name key of node (typically a classname but is not required to be)
+            """instantiate instances of node, given name key of node (typically a classname but is not required to be)
 
             Args:
                 class_name (str): name key for the class
                 configuration (Configuration): Configuration instance
 
             Returns:
                 instance (Traverser): instance of a traverser
 
-            '''
+            """
             return self.name_dict[class_name](configuration, instance_name)
 
         def valid_configuration(self, instance_class, configuration_dict):
             """Check for all the correct configuration keys via the necessary_config method
 
                 For instance, if a CSVWriter has a required filename key,
                 check that it exists as a key in the configuration
@@ -185,31 +195,37 @@
             Returns:
                 True for valid configuration
 
             Raises:
                 Exception if keys not valid
 
             """
-            configuration_requirements = instance_class.necessary_config(configuration_dict)
+            configuration_requirements = instance_class.necessary_config(
+                configuration_dict
+            )
 
             if all([key in configuration_dict for key in configuration_requirements]):
                 return True
             else:
-                raise Exception('Configuration missing necessary keys for '
-                                '{}, required keys: {}\n\n{}'.format(instance_class,
-                                                                    configuration_requirements,
-                                                                    instance_class.necessary_config.__doc__))
+                raise Exception(
+                    "Configuration missing necessary keys for "
+                    "{}, required keys: {}\n\n{}".format(
+                        instance_class,
+                        configuration_requirements,
+                        instance_class.necessary_config.__doc__,
+                    )
+                )
 
         def register_module_classes(self, module):
             """Given some module, find and register any AbstractNode classes it finds in that module
 
             Args:
                 module (str): e.g. __name__, 'src'
 
             Returns:
                 nothing. Side effect is to register the Node classes found
 
             """
             for name, obj in inspect.getmembers(sys.modules[module]):
                 if inspect.isclass(obj) and issubclass(obj, AbstractNode):
                     logging.info("Discovered class " + name + " (" + str(obj) + ")")
-                    self.register(name, obj)
+                    self.register(name, obj)
```

### Comparing `primrose-1.0.9/primrose/writers/abstract_file_writer.py` & `primrose-2.0.0/primrose/writers/abstract_file_writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 import pathlib
 from primrose.base.writer import AbstractWriter
 
+
 class AbstractFileWriter(AbstractWriter):
     """write some data to a some file"""
 
-    def __init__(self,configuration, instance_name):
+    def __init__(self, configuration, instance_name):
         """
 
         Args:
             configuration (Configuration): configuration object defined in primrose/Configuration with validated inputs
                 from the result of necessary_config, all inputs are described in that method
 
             instance_name (str): how the code knows where it is from
 
         """
         super().__init__(configuration, instance_name)
         self._check_directory()
 
     def _check_directory(self):
         """Create directory or directory structure if it does not already exist."""
-        pathlib.Path(self.node_config['dir']).mkdir(parents=True, exist_ok=True)
+        pathlib.Path(self.node_config["dir"]).mkdir(parents=True, exist_ok=True)
 
     @staticmethod
     def necessary_config(node_config):
         """Necessary inputs for file writers:
 
         Args:
             node_config (dict): set of parameters / attributes for the node
```

### Comparing `primrose-1.0.9/primrose/writers/file_writer.py` & `primrose-2.0.0/primrose/writers/file_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 """
 import os
 import logging
 from primrose.writers.abstract_file_writer import AbstractFileWriter
 from primrose.data_object import DataObjectResponseType
 
+
 class FileWriter(AbstractFileWriter):
-    ''' write some data object to a local file '''
+    """ write some data object to a local file """
 
     def run(self, data_object):
         """write some data to a local file
 
         Note:
             this will write object under config['key'] in data_object
 
@@ -22,18 +23,20 @@
             (tuple): tuple containing:
 
                 data_object (DataObject): instance of DataObject
 
                 terminate (bool): terminate the DAG?
 
         """
-        filename = self.node_config['dir'] + os.path.sep + self.node_config['filename']
-        data_key = self.node_config['key']
+        filename = self.node_config["dir"] + os.path.sep + self.node_config["filename"]
+        data_key = self.node_config["key"]
         logging.info("Saving %s data to %s", data_key, filename)
-        data_to_write = data_object.get_upstream_data(self.instance_name, pop_data=False, rtype=DataObjectResponseType.VALUE.value)
+        data_to_write = data_object.get_upstream_data(
+            self.instance_name, pop_data=False, rtype=DataObjectResponseType.VALUE.value
+        )
 
-        with open(filename, 'w') as f:
+        with open(filename, "w") as f:
             f.write(data_to_write)
         f.close()
 
         terminate = False
         return data_object, terminate
```

### Comparing `primrose-1.0.9/primrose/writers/csv_writer.py` & `primrose-2.0.0/primrose/writers/csv_writer.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 
 """
 import os
 import logging
 from primrose.data_object import DataObjectResponseType
 from primrose.writers.abstract_file_writer import AbstractFileWriter
 
+
 class CsvWriter(AbstractFileWriter):
     """write some dataframe to a local CSV file."""
 
     def get_optional_config(self):
-        '''
+        """
         Optionally get kwargs to pass to pandas csv reader.
 
         Notes:
             kwargs (dict): dictionary of kwargs key-value pairs
 
         Example:
             "csv_reader": { \
@@ -25,19 +26,19 @@
                 "filename": "data/mydata.csv", \
                 "kwargs": { \
                 "header": None, \
                 "sep": ":" \
                 } \
             }
 
-        '''
-        if 'kwargs' in self.node_config:
-            kwargs = self.node_config['kwargs']
-            if 'index' not in kwargs:
-                kwargs['index'] = False
+        """
+        if "kwargs" in self.node_config:
+            kwargs = self.node_config["kwargs"]
+            if "index" not in kwargs:
+                kwargs["index"] = False
             return kwargs
         else:
             return {"index": False}
 
     def run(self, data_object):
         """write some dataframe to a local CSV file
 
@@ -45,16 +46,19 @@
             (tuple): tuple containing:
 
                 data_object (DataObject): instance of DataObject
 
                 terminate (bool): terminate the DAG?
 
         """
-        filename = self.node_config['dir'] + os.path.sep + self.node_config['filename']
-        key = self.node_config['key']
+        filename = self.node_config["dir"] + os.path.sep + self.node_config["filename"]
+        key = self.node_config["key"]
         logging.info("Saving %s data to %s", key, filename)
-        data_to_write = data_object.get_upstream_data(self.instance_name, pop_data=False, rtype=DataObjectResponseType.KEY_VALUE.value)
+        data_to_write = data_object.get_upstream_data(
+            self.instance_name,
+            pop_data=False,
+            rtype=DataObjectResponseType.KEY_VALUE.value,
+        )
         kwargs = self.get_optional_config()
         data_to_write[key].to_csv(filename, **kwargs)
         terminate = False
         return data_object, terminate
-
```

### Comparing `primrose-1.0.9/primrose/writers/s3_writer.py` & `primrose-2.0.0/primrose/writers/s3_writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,24 +49,28 @@
         Returns:
             filename (str)
 
         """
         # save dataframe to CSV file first
 
         unique_filename = str(uuid.uuid4())
-        filename = self.node_config['dir'] + os.path.sep + unique_filename
-        key = self.node_config['key']
+        filename = self.node_config["dir"] + os.path.sep + unique_filename
+        key = self.node_config["key"]
         logging.info("Saving %s data to %s", key, filename)
 
-        data_to_write = data_object.get_upstream_data(self.instance_name, pop_data=False, rtype=DataObjectResponseType.KEY_VALUE.value)
+        data_to_write = data_object.get_upstream_data(
+            self.instance_name,
+            pop_data=False,
+            rtype=DataObjectResponseType.KEY_VALUE.value,
+        )
         assert key in data_to_write
         data_to_write[key].to_csv(filename, index=False)
 
         assert os.path.exists(filename)
-        return  filename
+        return filename
 
     def run(self, data_object):
         """write some data to a local CSV file then from there to S3 bucket
 
         Returns:
             (tuple): tuple containing:
 
@@ -77,29 +81,29 @@
         """
         filename = self._write_locally(data_object)
 
         # Create an S3 client
         # Boto3 will check these environment variables for credentials:
         # AWS_ACCESS_KEY_ID
         # AWS_SECRET_ACCESS_KEY
-        s3 = boto3.client('s3')
+        s3 = boto3.client("s3")
 
         # Uploads the given file using a managed uploader, which will split up large
         # files automatically and upload parts in parallel.
-        bucket_name = self.node_config['bucket_name']
-        key = self.node_config['bucket_filename']
+        bucket_name = self.node_config["bucket_name"]
+        key = self.node_config["bucket_filename"]
         logging.info("uploading to %s %s", bucket_name, key)
         s3.upload_file(filename, bucket_name, key)
 
         # TODO check for success
         # see https://stackoverflow.com/questions/41565766/make-a-unittest-for-a-function-that-uploads-a-file-to-s3-using-boto3
-        #s3 = boto3.resource('s3')
-        #mytname = nameOfFile
-        #obj = s3.Object(bucket_name='cloud-test-cf', key=mytname)
-        #response = obj.get()
-        #self.assertEqual(response['ContentLength'], len(contentsOfFile))
-        #remoteData = response['Body'].read()
-        #self.assertEqual(remoteData, contentsOfFile)
+        # s3 = boto3.resource('s3')
+        # mytname = nameOfFile
+        # obj = s3.Object(bucket_name='cloud-test-cf', key=mytname)
+        # response = obj.get()
+        # self.assertEqual(response['ContentLength'], len(contentsOfFile))
+        # remoteData = response['Body'].read()
+        # self.assertEqual(remoteData, contentsOfFile)
 
         logging.info("upload complete!")
         terminate = False
-        return data_object, terminate
+        return data_object, terminate
```

### Comparing `primrose-1.0.9/primrose/writers/serializer.py` & `primrose-2.0.0/primrose/writers/serializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 import pickle
 from primrose.data_object import DataObjectResponseType
 from primrose.writers.abstract_file_writer import AbstractFileWriter
 
 
 class Serializer(AbstractFileWriter):
     """Serialize some object to a local file."""
-    SUPPORTED_SERIALIZERS = {'dill': dill, 'pickle': pickle}
+
+    SUPPORTED_SERIALIZERS = {"dill": dill, "pickle": pickle}
 
     @staticmethod
     def necessary_config(node_config):
         """Returns the necessary configuration keys for the Serializer object:
 
         Args:
             node_config (dict): set of parameters / attributes for the node
@@ -28,15 +29,15 @@
             serializer (str): 'dill' or 'pickle'
 
         Returns:
             set of necessary configuration keys
 
         """
 
-        config_params = set(['serializer'])
+        config_params = set(["serializer"])
         return config_params.union(AbstractFileWriter.necessary_config(node_config))
 
     def run(self, data_object):
         """serialize some data to a local filesystem using Dill
 
         Note:
             this will write object under config['key'] in data_object
@@ -48,30 +49,41 @@
             (tuple): tuple containing:
 
                 data_object (DataObject): instance of DataObject
 
                 terminate (bool): terminate the DAG?
 
         """
-        filename = self.node_config['dir'] + os.path.sep + self.node_config['filename']
-        data_key = self.node_config['key']
+        filename = self.node_config["dir"] + os.path.sep + self.node_config["filename"]
+        data_key = self.node_config["key"]
 
         logging.info("Saving {} data to {}".format(data_key, filename))
 
-        data_to_write = data_object.get_upstream_data(self.instance_name, pop_data=False, rtype=DataObjectResponseType.KEY_VALUE.value)
+        data_to_write = data_object.get_upstream_data(
+            self.instance_name,
+            pop_data=False,
+            rtype=DataObjectResponseType.KEY_VALUE.value,
+        )
 
         if data_key not in data_to_write:
             raise Exception("Key {} not found inside data_key object".format(data_key))
 
-        if self.node_config['serializer'] not in Serializer.SUPPORTED_SERIALIZERS.keys():
-            logging.warning(f"{self.node_config['serializer']} serializer not supported.")
-            logging.warning(f"The following serializers are supported {Serializer.SUPPORTED_SERIALIZERS.keys()}.")
+        if (
+            self.node_config["serializer"]
+            not in Serializer.SUPPORTED_SERIALIZERS.keys()
+        ):
+            logging.warning(
+                f"{self.node_config['serializer']} serializer not supported."
+            )
+            logging.warning(
+                f"The following serializers are supported {Serializer.SUPPORTED_SERIALIZERS.keys()}."
+            )
             raise Exception(f"Unsupported serializer: {self.node_config['serializer']}")
 
-        serializer = Serializer.SUPPORTED_SERIALIZERS[self.node_config['serializer']]
+        serializer = Serializer.SUPPORTED_SERIALIZERS[self.node_config["serializer"]]
 
-        with open(filename, 'wb') as f:
+        with open(filename, "wb") as f:
             serializer.dump(data_to_write[data_key], f)
 
         terminate = False
 
         return data_object, terminate
```

### Comparing `primrose-1.0.9/primrose/writers/dill_writer.py` & `primrose-2.0.0/primrose/writers/dill_writer.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 import warnings
 
 from primrose.writers.abstract_file_writer import AbstractFileWriter
 from primrose.data_object import DataObjectResponseType
 
 
 class DillWriter(AbstractFileWriter):
-    ''' write some specified data object to a dill file '''
-    warnings.warn('Use Serializer instead. DillWriter will be deprecated in a future release.', DeprecationWarning)
+    """ write some specified data object to a dill file """
+
+    warnings.warn(
+        "Use Serializer instead. DillWriter will be deprecated in a future release.",
+        DeprecationWarning,
+    )
 
     def run(self, data_object):
         """serialize some data to a local filesystem using Dill
 
         Note:
             this will write object under config['key'] in data_object
 
@@ -30,23 +34,27 @@
             (tuple): tuple containing:
 
                 data_object (DataObject): instance of DataObject
 
                 terminate (bool): terminate the DAG?
 
         """
-        filename = self.node_config['dir'] + os.path.sep + self.node_config['filename']
-        data_key = self.node_config['key']
+        filename = self.node_config["dir"] + os.path.sep + self.node_config["filename"]
+        data_key = self.node_config["key"]
 
         logging.info("Saving {} data to {}".format(data_key, filename))
 
-        data_to_write = data_object.get_upstream_data(self.instance_name, pop_data=False, rtype=DataObjectResponseType.KEY_VALUE.value)
+        data_to_write = data_object.get_upstream_data(
+            self.instance_name,
+            pop_data=False,
+            rtype=DataObjectResponseType.KEY_VALUE.value,
+        )
 
         if data_key not in data_to_write:
             raise Exception("Key {} not found inside data_key object".format(data_key))
 
-        with open(filename, 'wb') as f:
+        with open(filename, "wb") as f:
             dill.dump(data_to_write[data_key], f)
 
         terminate = False
 
         return data_object, terminate
```

### Comparing `primrose-1.0.9/primrose/__init__.py` & `primrose-2.0.0/primrose/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,198 +1,243 @@
 import click
 import logging
 import os
 import sys
 import importlib
 import pkg_resources
 
-logging.basicConfig(format='%(asctime)s %(levelname)s %(filename)s %(funcName)s: %(message)s', level=logging.INFO)
+logging.basicConfig(
+    format="%(asctime)s %(levelname)s %(filename)s %(funcName)s: %(message)s",
+    level=logging.INFO,
+)
 
 
 def replace_line(file_name, line_num, text):
     """Replace a single line of a file with text
 
     Args:
         file_name (str): name of file
         line_num (int): line to replace
         text (str): string to replace at line_num
 
     Returns:
         Nothing, the file is modified and rewritten
 
     """
-    lines = open(file_name, 'r').readlines()
+    lines = open(file_name, "r").readlines()
     lines[line_num] = text
-    out = open(file_name, 'w')
+    out = open(file_name, "w")
     out.writelines(lines)
     out.close()
 
 
 @click.group()
 def cli():
     """This is the command line interface for primrose.
     The command most people need is `primrose run` to run a primrose job.
     Type primrose commandname --help for more detailed help on a command"""
     pass
 
 
 @click.command()
-@click.option('--config', required=True, help="Path to Config file")
+@click.option("--config", required=True, help="Path to Config file")
 def validate(config):
     """Validate a primrose config"""
     from primrose.configuration.configuration import Configuration
+
     configuration = Configuration(config_location=config)
 
 
 @click.command()
-@click.option('--config', required=True, help="Path to Config file")
-@click.option('--dry_run', default=False, help="Config file")
+@click.option("--config", required=True, help="Path to Config file")
+@click.option("--dry_run", default=False, help="Config file")
 def run(config, dry_run=False):
     """Run a primrose job"""
     from primrose.configuration.configuration import Configuration
     from primrose.dag_runner import DagRunner
 
     configuration = Configuration(config_location=config)
     DagRunner(configuration).run(dry_run=dry_run)
 
 
 @click.command()
-@click.option('--config', required=True, help="Path to Config file")
-@click.option('--node_size', help='Size of nodes', required=False, default=500)
-@click.option('--label_font_size', help='Size of font for text labels', required=False, default=12)
-@click.option('--text_angle', help='Angle to rotate text (counterclockwise)', required=False, default=0)
-@click.option('--image_width', help='width of image in inches', required=False, default=16)
-@click.option('--image_height', help='height of image in inches', required=False, default=12)
-@click.option('--nodesequence', help='Show node sequences numbers? "true" or "false"?', required=False)
-@click.option('--outfile', help='Path for the output image file', required=True)
-def plot(config, node_size, label_font_size, text_angle, image_width, image_height, nodesequence, outfile):
-    '''Create an image of the DAG'''
+@click.option("--config", required=True, help="Path to Config file")
+@click.option("--node_size", help="Size of nodes", required=False, default=500)
+@click.option(
+    "--label_font_size", help="Size of font for text labels", required=False, default=12
+)
+@click.option(
+    "--text_angle",
+    help="Angle to rotate text (counterclockwise)",
+    required=False,
+    default=0,
+)
+@click.option(
+    "--image_width", help="width of image in inches", required=False, default=16
+)
+@click.option(
+    "--image_height", help="height of image in inches", required=False, default=12
+)
+@click.option(
+    "--nodesequence",
+    help='Show node sequences numbers? "true" or "false"?',
+    required=False,
+)
+@click.option("--outfile", help="Path for the output image file", required=True)
+def plot(
+    config,
+    node_size,
+    label_font_size,
+    text_angle,
+    image_width,
+    image_height,
+    nodesequence,
+    outfile,
+):
+    """Create an image of the DAG"""
     from primrose.configuration.configuration import Configuration
     from primrose.dag.traverser_factory import TraverserFactory
 
     config = Configuration(config_location=config)
 
     filename = outfile
     other_args = {}
-    other_args['filename'] = outfile
+    other_args["filename"] = outfile
 
     if node_size:
-        other_args['node_size'] = int(node_size)
+        other_args["node_size"] = int(node_size)
 
     if label_font_size:
-        other_args['label_font_size'] = int(label_font_size)
+        other_args["label_font_size"] = int(label_font_size)
 
     if text_angle:
-        other_args['text_angle'] = int(text_angle)
+        other_args["text_angle"] = int(text_angle)
 
     if image_width:
-        other_args['image_width'] = int(image_width)
+        other_args["image_width"] = int(image_width)
 
     if image_height:
-        other_args['image_height'] = int(image_height)
+        other_args["image_height"] = int(image_height)
 
-    other_args['traverser'] = None
+    other_args["traverser"] = None
     if nodesequence and nodesequence.lower() == "true":
         traverser = TraverserFactory().default_traverser(config)
 
-        if config.config_metadata and 'traverser' in config.config_metadata:
-            traverser = TraverserFactory().instantiate(config.config_metadata['traverser'], config)
-            logging.info("Setting to Traverser to %s", config.config_metadata['traverser'])
+        if config.config_metadata and "traverser" in config.config_metadata:
+            traverser = TraverserFactory().instantiate(
+                config.config_metadata["traverser"], config
+            )
+            logging.info(
+                "Setting to Traverser to %s", config.config_metadata["traverser"]
+            )
 
-        other_args['traverser'] = traverser
+        other_args["traverser"] = traverser
 
     logging.info("passing in %s", other_args)
     config.dag.plot_dag(**other_args)
 
 
 @click.command()
-@click.option('--destination', required=True, help="Path to destination")
+@click.option("--destination", required=True, help="Path to destination")
 def generate_run_script(destination):
     """Create primrose run script in your project--if you need to register your own primrose classes.
-    This will also allow you to register and use your own primrose node classes. 
+    This will also allow you to register and use your own primrose node classes.
     To register your own classes you will also need to run the primrose generate_class_registration_template command"""
     from shutil import copyfile
-    run_primrose_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'templates', 'run_primrose.py')
+
+    run_primrose_path = os.path.join(
+        os.path.dirname(os.path.realpath(__file__)), "templates", "run_primrose.py"
+    )
     copyfile(run_primrose_path, destination)
     print("Primrose's run_primrose.py script copied to " + destination)
     print("Don't forget to set where your new classes are to be imported. See script.")
 
 
 @click.command()
-@click.option('--destination', required=True, help="Path to destination")
+@click.option("--destination", required=True, help="Path to destination")
 def generate_class_registration_template(destination):
     """Create template to register your own classes. This will copy a template to your destination, such as src/__init__.py"""
     from shutil import copyfile
-    user_registration_template_path = os.path.join(os.path.dirname(os.path.realpath(__file__)),
-                                                   'templates',
-                                                   'user_registration_template.py')
+
+    user_registration_template_path = os.path.join(
+        os.path.dirname(os.path.realpath(__file__)),
+        "templates",
+        "user_registration_template.py",
+    )
     copyfile(user_registration_template_path, destination)
     print("Primrose's user_registration_template.py script copied to " + destination)
 
+
 @click.command()
-@click.option('--name', required=True, help="Name of primrose project to be generated")
+@click.option("--name", required=True, help="Name of primrose project to be generated")
 def create_project(name):
     """Create template project filled with example configuration"""
 
     from shutil import copyfile, copytree
 
     # get local directories to copy from the package dir
-    package_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'templates')
+    package_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "templates")
     env_dir = sys.prefix
 
-    config_dir_path = os.path.join(env_dir, 'config')
+    config_dir_path = os.path.join(env_dir, "config")
 
-    data_dir_path = os.path.join(env_dir, 'data')
+    data_dir_path = os.path.join(env_dir, "data")
 
-    user_registration_template_path = os.path.join(package_dir, 'user_registration_template.py')
+    user_registration_template_path = os.path.join(
+        package_dir, "user_registration_template.py"
+    )
 
-    run_primrose_path = os.path.join(package_dir, 'run_primrose.py')
+    run_primrose_path = os.path.join(package_dir, "run_primrose.py")
 
     # make empty cache and src dir
-    os.makedirs(os.path.join(name, 'cache'))
-    os.makedirs(os.path.join(name, 'src', 'yourpackage'))
+    os.makedirs(os.path.join(name, "cache"))
+    os.makedirs(os.path.join(name, "src", "yourpackage"))
 
     # copy relevant files to user path
-    copytree(config_dir_path, os.path.join(name, 'config'))
+    copytree(config_dir_path, os.path.join(name, "config"))
 
-    copytree(data_dir_path, os.path.join(name, 'data'))
+    copytree(data_dir_path, os.path.join(name, "data"))
 
-    copyfile(os.path.join(package_dir, 'awesome_model.py'), os.path.join(name,
-                                                                         'src',
-                                                                         'yourpackage',
-                                                                         'awesome_model.py'))
+    copyfile(
+        os.path.join(package_dir, "awesome_model.py"),
+        os.path.join(name, "src", "yourpackage", "awesome_model.py"),
+    )
 
-    copyfile(os.path.join(package_dir, 'awesome_reader.py'), os.path.join(name,
-                                                                          'src',
-                                                                          'yourpackage',
-                                                                          'awesome_reader.py'))
+    copyfile(
+        os.path.join(package_dir, "awesome_reader.py"),
+        os.path.join(name, "src", "yourpackage", "awesome_reader.py"),
+    )
 
-    copyfile(user_registration_template_path, os.path.join(name, 'src', '__init__.py'))
+    copyfile(user_registration_template_path, os.path.join(name, "src", "__init__.py"))
 
-    copyfile(run_primrose_path, os.path.join(name, 'run_primrose.py'))
+    copyfile(run_primrose_path, os.path.join(name, "run_primrose.py"))
 
     # modify run_primrose to take into account the templated extention functions
-    replacement_line = 'from src.__init__ import *\n'
+    replacement_line = "from src.__init__ import *\n"
 
-    replace_line(os.path.join(name, 'run_primrose.py'), 14, replacement_line)
+    replace_line(os.path.join(name, "run_primrose.py"), 14, replacement_line)
 
     # make __init__ file for the yourpackage directory
-    with open(os.path.join(name, 'src', 'yourpackage','__init__.py'), 'w') as f:
-        f.write('')
+    with open(os.path.join(name, "src", "yourpackage", "__init__.py"), "w") as f:
+        f.write("")
 
     print("New primrose project, {} built!".format(name))
 
+
 @cli.command()
 def version():
-    '''Print the installed primrose version'''
+    """Print the installed primrose version"""
     print(pkg_resources.get_distribution("primrose").version)
 
+
 cli.add_command(validate)
 cli.add_command(run)
 cli.add_command(plot)
-cli.add_command(generate_run_script, name='generate-run-script')
-cli.add_command(generate_class_registration_template, name='generate-class-registration-template')
-cli.add_command(create_project, name='create-project')
+cli.add_command(generate_run_script, name="generate-run-script")
+cli.add_command(
+    generate_class_registration_template, name="generate-class-registration-template"
+)
+cli.add_command(create_project, name="create-project")
 cli.add_command(version)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `primrose-1.0.9/primrose/conditionalpath/simple_switch.py` & `primrose-2.0.0/primrose/conditionalpath/simple_switch.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 from primrose.base.conditional_path_node import AbstractConditionalPath
 
-class SimpleSwitch(AbstractConditionalPath):
 
+class SimpleSwitch(AbstractConditionalPath):
     @staticmethod
-    def necessary_config(node_config): 
+    def necessary_config(node_config):
         """Return a list of necessary configuration keys within the implementation
 
         Args:
             node_config (dict): set of parameters / attributes for the node
 
         Returns:
             set of keys necessary to run implementation
 
         """
-        return set(['path_to_travel'])
+        return set(["path_to_travel"])
 
     def destinations_to_prune(self):
         """List destinations that the node wishes to be pruned from the DAG
-        
+
         Returns:
             destinations (list): list of destinations
 
         """
-        destinations = self.node_config['destinations']
-        destinations.remove(self.node_config['path_to_travel'])
+        destinations = self.node_config["destinations"]
+        destinations.remove(self.node_config["path_to_travel"])
         return destinations
 
     def run(self, data_object):
         """Run this node. Here, do nothing
 
         Args:
             data_object (DataObject): DataObject instance
@@ -42,8 +42,8 @@
             (tuple): tuple containing:
 
                 data_object (DataObject): instance of DataObject
 
                 terminate (bool): terminate the DAG?
 
         """
-        return data_object, False
+        return data_object, False
```

### Comparing `primrose-1.0.9/primrose/dag/traverser_factory.py` & `primrose-2.0.0/primrose/dag/traverser_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,45 +5,44 @@
 
 """
 
 import logging
 from primrose.dag.config_layer_traverser import ConfigLayerTraverser
 from primrose.dag.depth_first_traverser import DepthFirstTraverser
 
+
 class TraverserFactory:
     """Singleton Factory where one can register traversers for instantiation"""
 
     instance = None
 
     def __init__(self):
-        """instantiate the factory but as a singleton. The guard raails are here
-        """
+        """instantiate the factory but as a singleton. The guard raails are here"""
         # where the magic happens, only one instance allowed:
         if not TraverserFactory.instance:
             TraverserFactory.instance = TraverserFactory.__HiddenFactory()
 
     def __getattr__(self, name):
         """getattr with instance name
 
         Returns:
             gettattr
 
         """
         return getattr(self.instance, name)
 
-    class __HiddenFactory():
+    class __HiddenFactory:
         """actual factory where registry and instantiation happens"""
 
-        
         def __init__(self):
             """instantiate the HiddenFactory"""
             self.name_dict = {}
-            self.register('ConfigLayerTraverser', ConfigLayerTraverser)
-            self.register('DepthFirstTraverser', DepthFirstTraverser)
-            self.DEFAULT_TRAVERSER = 'ConfigLayerTraverser'
+            self.register("ConfigLayerTraverser", ConfigLayerTraverser)
+            self.register("DepthFirstTraverser", DepthFirstTraverser)
+            self.DEFAULT_TRAVERSER = "ConfigLayerTraverser"
 
         def register(self, key, class_obj, raise_on_overwrite=False):
             """Registering class_obj with key
 
             Args:
                 key (str): key such as class name, e.g. 'ConfigLayerTraverser'
                 class_obj (class obj), e.g. ConfigLayerTraverser
@@ -66,18 +65,18 @@
             Returns:
                 Traverser instance
 
             """
             return self.instantiate(self.DEFAULT_TRAVERSER, configuration)
 
         def instantiate(self, class_name, configuration):
-            '''instantiate instances of rule, given name of rule class
+            """instantiate instances of rule, given name of rule class
 
             Args:
                 class_name (str): name of the class
                 configuration (Configuration): Configuration instance
 
             Returns:
                 instance (Traverser): instance of a traverser
 
-            '''
+            """
             return self.name_dict[class_name](configuration)
```

### Comparing `primrose-1.0.9/primrose/dag/dag_traverser.py` & `primrose-2.0.0/primrose/dag/dag_traverser.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 from abc import ABC, abstractmethod
 
+
 class DagTraverser(ABC):
     """Abstract module to traverse a DAG"""
 
     def __init__(self, configuration):
         """instantiate the traverser
 
         Args:
@@ -37,8 +38,8 @@
     def traversal_list(self):
         """get list of nodes to traverse
 
         Returns:
             sequence (list): list of node name in the order that they should be run
 
         """
-        pass # pragma: no cover
+        pass  # pragma: no cover
```

### Comparing `primrose-1.0.9/primrose/dag/config_layer_traverser.py` & `primrose-2.0.0/primrose/dag/config_layer_traverser.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 from primrose.dag.dag_traverser import DagTraverser
 from primrose.dag.depth_first_traverser import DepthFirstTraverser
 
+
 class ConfigLayerTraverser(DagTraverser):
     """Module to traverse DAG by running all readers, then all pipelines,
     then all models, then all postprocess, then all cleanup
 
     """
 
     def _sort_by_depth_first(self, candidates):
```

### Comparing `primrose-1.0.9/primrose/dag/depth_first_traverser.py` & `primrose-2.0.0/primrose/dag/depth_first_traverser.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 import networkx as nx
 from primrose.dag.dag_traverser import DagTraverser
 
+
 class DepthFirstTraverser(DagTraverser):
     """a traverser that traverses in depth first manner"""
 
     def run_section_by_section(self):
         """Do we want go through section by section?
 
         Note:
```

### Comparing `primrose-1.0.9/primrose/pipelines/encode_train_test_split.py` & `primrose-2.0.0/primrose/pipelines/encode_train_test_split.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,31 +16,31 @@
         """create the pipeline's TransformerSequence
 
         Returns:
             a TransformerSequence
 
         """
         ts = TransformerSequence()
-        ts.add(ImplicitCategoricalTransform(self.node_config['target_variable']))
+        ts.add(ImplicitCategoricalTransform(self.node_config["target_variable"]))
         return ts
 
     @property
     def first_transformer_in_sequence(self):
         """returns 1st transformer in a sequence
 
         Returns:
             a transformer
 
         """
         return self.transformer_sequence.sequence[0]
 
     def final_data_object_additions(self, data_object):
         """Overload function which adds the label encoder after running fit_transform or transform
-        
+
         Returns:
             data_object (DataObject): instance of DataObject
-        
+
         """
         # add target label encoder to the data object if it's needed downstream
         target_label_encoder = self.first_transformer_in_sequence.target_encoder
-        data_object.add(self, target_label_encoder, key='target_encoder')
+        data_object.add(self, target_label_encoder, key="target_encoder")
         return data_object
```

### Comparing `primrose-1.0.9/primrose/pipelines/train_test_split.py` & `primrose-2.0.0/primrose/pipelines/train_test_split.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,14 +22,19 @@
         Otherwise, make a child class and write an init_pipeline method to perform operations on your data.
 
         This class also handles writing your transformer_sequence into the data_object, so there's no need
         to write in child classes.
 
     """
 
+    def __init__(self, configuration, instance_name):
+        super(TrainTestSplit, self).__init__(configuration, instance_name)
+        self.training_fraction = self.node_config.get("training_fraction", 0)
+        self.seed = self.node_config.get("seed", 0)
+
     @staticmethod
     def necessary_config(node_config):
         """Return the necessary configuration keys for the DataFrameJoiner object
 
         Args:
             node_config (dict): set of parameters / attributes for the node
 
@@ -38,75 +43,98 @@
             training_fraction (float): 0->1 float for the fraction of data rows to be used for training \
             seed (int): random number to control the stochastic row selection \
 
         Returns:
             set of keys
 
         """
-        return set(['training_fraction', 'seed'])
+        return set(["training_fraction", "seed"]).union(
+            AbstractPipeline.necessary_config(node_config)
+        )
 
     def features(self, data):
         """Use user-specified features if available, otherwise use all non-target columns
-        
+
         Args:
             data (DataFrame): pandas dataframe
 
         Returns:
             lsit of feature names
-        
+
         """
-        if 'features' in self.node_config:
-            return self.node_config['features']
+        if "features" in self.node_config:
+            return self.node_config["features"]
 
         else:
-            if 'target_variable' in self.node_config:
-                return [f for f in data.columns if f != self.node_config['target_variable']]
+            if "target_variable" in self.node_config:
+                return [
+                    f for f in data.columns if f != self.node_config["target_variable"]
+                ]
             else:
                 return data.columns
 
     def _train_test_split(self, data):
         """Split data into test/train sets
-        
+
         Returns:
             train_data_to_transform (DataFrame)
-            
+
             test_data_to_transform (DataFrame)
-        
+
         """
         logging.info("Splitting data into testing and training sets.")
 
-        test_size = (1.0 - float(self.node_config['training_fraction']))
+        test_size = 1.0 - float(self.training_fraction)
 
         if test_size == 0:
             train_data_to_transform = data
             test_data_to_transform = pd.DataFrame()
-        
+
         else:
-            if 'target_variable' in self.node_config:
+            if "target_variable" in self.node_config:
                 data_train, data_test, target_train, target_test = train_test_split(
-                    data[self.features(data)],
-                    data[self.node_config['target_variable']],
-                    test_size=(1.0 - float(self.node_config['training_fraction'])),
-                    random_state=self.node_config['seed'])
+                    data[
+                        sorted(
+                            list(
+                                set(data.columns)
+                                - set([self.node_config.get("target_variable")])
+                            )
+                        )
+                    ],
+                    data[self.node_config["target_variable"]],
+                    test_size=(1.0 - float(self.training_fraction)),
+                    random_state=self.seed,
+                )
 
                 # re-merge training and target data into a single dataframe for transforming
                 train_data_to_transform = pd.concat([data_train, target_train], axis=1)
                 test_data_to_transform = pd.concat([data_test, target_test], axis=1)
 
             else:
                 data_train, data_test = train_test_split(
-                    data[self.features(data)],
-                    test_size=(1.0 - float(self.node_config['training_fraction'])),
-                    random_state=self.node_config['seed'])
+                    data[
+                        sorted(
+                            list(
+                                set(data.columns)
+                                - set([self.node_config.get("target_variable")])
+                            )
+                        )
+                    ],
+                    test_size=(1.0 - float(self.training_fraction)),
+                    random_state=self.seed,
+                )
 
                 train_data_to_transform = data_train
                 test_data_to_transform = data_test
 
-        logging.info('Training data rows: {}, Testing data rows: {}'.format(len(train_data_to_transform),
-                                                                            len(test_data_to_transform)))
+        logging.info(
+            "Training data rows: {}, Testing data rows: {}".format(
+                len(train_data_to_transform), len(test_data_to_transform)
+            )
+        )
 
         return train_data_to_transform, test_data_to_transform
 
     def final_data_object_additions(self, data_object):
         """DataObject: Template method to be overloaded in child classes
 
         Note:
@@ -143,62 +171,90 @@
         for source in data:
 
             for key in data[source]:
 
                 if isinstance(data[source][key], pd.DataFrame):
 
                     if dataframes_to_join:
-                        if set(data[source][key].columns) != set(dataframes_to_join[0].columns):
-                            logging.warning('Concatenated dataframe schemas do not match, subbed with NULL values.')
+                        if set(data[source][key].columns) != set(
+                            dataframes_to_join[0].columns
+                        ):
+                            logging.warning(
+                                "Concatenated dataframe schemas do not match, subbed with NULL values."
+                            )
 
                     dataframes_to_join.append(data[source][key])
 
-        return pd.concat(dataframes_to_join)
+        return pd.concat(dataframes_to_join).reset_index(drop=True)
 
     def fit_transform(self, data_object):
         """Split data into testing and training sets, then applies the categorical transform to each
 
         Args:
             data_object (DataObject): instance of DataObject
 
         Returns:
             data_object (DataObject): instance of DataObject
 
         """
 
         # we're can expect multiple objects from a reader, so we need to concatenate
-        data_list = data_object.get_upstream_data(self.instance_name,
-                                            pop_data=False,
-                                            rtype=DataObjectResponseType.INSTANCE_KEY_VALUE.value)
+        data_list = data_object.get_upstream_data(
+            self.instance_name,
+            pop_data=False,
+            rtype=DataObjectResponseType.INSTANCE_KEY_VALUE.value,
+        )
 
         data = self._concatenate_upstream_dataframes(data_list)
 
         train_data, test_data = self._train_test_split(data)
 
         if not train_data.empty:
-            train_data = self.execute_pipeline(train_data, PipelineModeType.FIT_TRANSFORM)
-            data_object.add(self, train_data[self.features(train_data)], key='data_train', overwrite=False)
-
-            if 'target_variable' in self.node_config:
-                data_object.add(self, train_data[self.node_config['target_variable']], key='target_train',
-                            overwrite=False)
+            train_data = self.execute_pipeline(
+                train_data, PipelineModeType.FIT_TRANSFORM
+            )
+            data_object.add(
+                self,
+                train_data[self.features(train_data)],
+                key="data_train",
+                overwrite=False,
+            )
+
+            if "target_variable" in self.node_config:
+                data_object.add(
+                    self,
+                    train_data[self.node_config["target_variable"]],
+                    key="target_train",
+                    overwrite=False,
+                )
 
         # run the pre-trained pipeline on the testing data
         if not test_data.empty:
             # run the pipeline in Transform mode since we've already fit the pipeline with training data
             test_data = self.execute_pipeline(test_data, PipelineModeType.TRANSFORM)
             self.data = test_data  # assign the data to the testing data if available
-            data_object.add(self, test_data[self.features(train_data)], key='data_test', overwrite=False)
-
-            if 'target_variable' in self.node_config:
-                data_object.add(self, test_data[self.node_config['target_variable']], key='target_test',
-                            overwrite=False)
+            data_object.add(
+                self,
+                test_data[self.features(train_data)],
+                key="data_test",
+                overwrite=False,
+            )
+
+            if "target_variable" in self.node_config:
+                data_object.add(
+                    self,
+                    test_data[self.node_config["target_variable"]],
+                    key="target_test",
+                    overwrite=False,
+                )
 
         # save pipeline for writing later
-        data_object.add(self, self.transformer_sequence, key='transformer_sequence', overwrite=False)
+        data_object.add(
+            self, self.transformer_sequence, key="transformer_sequence", overwrite=False
+        )
         data_object = self.final_data_object_additions(data_object)
 
         return data_object
 
     def transform(self, data_object):
         """Transform the data into label encoded data using the pre-trained transformer sequence
 
@@ -206,25 +262,36 @@
             data_object (DataObject): instance of DataObject
 
         Returns:
             data_object (DataObject): instance of DataObject
 
         """
         # we're can expect multiple objects from a reader, so we need to concatenate
-        data_list = data_object.get_upstream_data(self.instance_name,
-                                                pop_data=False,
-                                                rtype=DataObjectResponseType.INSTANCE_KEY_VALUE.value)
+        data_list = data_object.get_upstream_data(
+            self.instance_name,
+            pop_data=False,
+            rtype=DataObjectResponseType.INSTANCE_KEY_VALUE.value,
+        )
 
         data = self._concatenate_upstream_dataframes(data_list)
 
         data = self.execute_pipeline(data, PipelineModeType.TRANSFORM)
 
-        self.data = data  # keep the data for use in the final_data_object_additions method
-
-        data_object.add(self, data[self.features(data)], key='data_test', overwrite=False)
-
-        if 'target_variable' in self.node_config:
-            data_object.add(self, data[self.node_config['target_variable']], key='target_test', overwrite=False)
+        self.data = (
+            data  # keep the data for use in the final_data_object_additions method
+        )
+
+        data_object.add(
+            self, data[self.features(data)], key="data_test", overwrite=False
+        )
+
+        if "target_variable" in self.node_config:
+            data_object.add(
+                self,
+                data[self.node_config["target_variable"]],
+                key="target_test",
+                overwrite=False,
+            )
 
         data_object = self.final_data_object_additions(data_object)
 
         return data_object
```

### Comparing `primrose-1.0.9/primrose/pipelines/dataframe_joiner.py` & `primrose-2.0.0/primrose/pipelines/dataframe_joiner.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 import logging
 from primrose.base.pipeline import AbstractPipeline, PipelineModeType
 from primrose.transformers.combine import LeftJoinDataCombiner
 from primrose.base.transformer_sequence import TransformerSequence
 from primrose.data_object import DataObject
 
+
 class DataFrameJoiner(AbstractPipeline):
     """Join upstream dataframes"""
 
     @staticmethod
     def necessary_config(node_config):
         """Return the necessary configuration keys for the DataFrameJoiner object
 
@@ -24,56 +25,60 @@
             start_table: first table index in alpha order which defines who is eligible for this analysis (all other tables will be left joined to this)
             join_key: list of column names to join dataframes from different readers on
 
         Returns:
             set of keys
 
         """
-        return set(['start_table', 'join_key'])
+        return set(["start_table", "join_key"])
 
     def init_pipeline(self):
         """create the pipeline's TransformerSequence
 
         Returns:
             a TransformerSequence
 
         """
         ts = TransformerSequence()
         # Note: this is a trasnformer that does not striclty adhere to Transformer interface
         # It takes a in *list* of data frames, not a single data, and returns a single dataframe
-        ts.add(LeftJoinDataCombiner(self.node_config['join_key']))
+        ts.add(LeftJoinDataCombiner(self.node_config["join_key"]))
         return ts
 
     def transform(self, data_object):
         """Get DataFrames from the data object then put them into a alphabetical list for constant join order
 
         Args:
             data_object (DataObject): instance of DataObject
 
         Returns:
             data_object (DataObject): instance of DataObject
 
         """
 
-        upstream_data = data_object.get_upstream_data(self.instance_name,
-                                                pop_data=False)
+        upstream_data = data_object.get_upstream_data(
+            self.instance_name, pop_data=False
+        )
 
         upstream_keys = sorted([k for k in upstream_data.keys()])
 
-        start_key = self.node_config['start_table']
+        start_key = self.node_config["start_table"]
 
         if start_key not in upstream_keys:
             raise Exception("Could not find start_table in upstream keys: " + start_key)
 
         upstream_keys = [start_key] + [k for k in upstream_keys if k != start_key]
 
-        logging.info('Joining dataframes from {} sources'.format(len(upstream_keys)))
+        logging.info("Joining dataframes from {} sources".format(len(upstream_keys)))
 
         # note we are passing in a list of dataframes here
         # note: we assume default DATA_KEY
-        data = self.execute_pipeline([upstream_data[k][DataObject.DATA_KEY] for k in upstream_keys], PipelineModeType.TRANSFORM)
+        data = self.execute_pipeline(
+            [upstream_data[k][DataObject.DATA_KEY] for k in upstream_keys],
+            PipelineModeType.TRANSFORM,
+        )
 
-        logging.info('Final size of joined data is {} rows.'.format(len(data)))
+        logging.info("Final size of joined data is {} rows.".format(len(data)))
 
         data_object.add(self, data, overwrite=False)
 
         return data_object
```

### Comparing `primrose-1.0.9/primrose/pipelines/sklearn_preprocessing_pipeline.py` & `primrose-2.0.0/primrose/pipelines/sklearn_preprocessing_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,65 +2,75 @@
 
 Author(s):
     Carl Anderson (carl.anderson@weightwatchers.com)
 
 """
 import importlib
 from primrose.base.transformer_sequence import TransformerSequence
-from primrose.transformers.sklearn_preprocessing_transformer import SklearnPreprocessingTransformer
+from primrose.transformers.sklearn_preprocessing_transformer import (
+    SklearnPreprocessingTransformer,
+)
 from primrose.data_object import DataObjectResponseType
 from primrose.pipelines.train_test_split import TrainTestSplit
+import warnings
+
 
 class SklearnPreprocessingPipeline(TrainTestSplit):
+    warnings.warn(
+        "SklearnPreprocessingPipeline will be deprecated in a future release. Please use TransformerPipeline instead",
+        DeprecationWarning,
+    )
 
     @staticmethod
     def necessary_config(node_config):
         """Return the necessary configuration keys for the SklearnPreprocessingPipeline object
 
         Returns:
             set of keys
 
         """
-        return set(['operations']).union(TrainTestSplit.necessary_config(node_config))
+        return set(["operations"]).union(TrainTestSplit.necessary_config(node_config))
 
     def init_pipeline(self):
         """create the pipeline's TransformerSequence
 
         Returns:
             a TransformerSequence
 
         """
         ts = TransformerSequence()
 
         for operation in self.node_config["operations"]:
 
-            args = operation.get('args', None)
-            columns = operation.get('columns', None)
-            
-            p = SklearnPreprocessingPipeline._instantiate_preprocessor(operation['class'], args, columns)
+            args = operation.get("args", None)
+            columns = operation.get("columns", None)
+
+            p = self._instantiate_preprocessor(operation["class"], args, columns)
             ts.add(p)
 
         return ts
 
     @staticmethod
     def _instantiate_preprocessor(classname, args=None, columns=None):
         """Import and validate user-defined sklearn preprocessor
-        
+
         Returns:
             SklearnPreprocessingTransformer
-        
+
         """
 
-        sk_module_name, sk_transformer_name = classname.split('.')
-        sk_module = importlib.import_module('sklearn.{}'.format(sk_module_name))
+        sk_module_name, sk_transformer_name = classname.split(".")
+        sk_module = importlib.import_module("sklearn.{}".format(sk_module_name))
 
         try:
             t = getattr(sk_module, sk_transformer_name)
         except AttributeError:
-            raise Exception('Preprocessor {} not found in {} module'.format(sk_transformer_name, sk_module_name))
+            raise Exception(
+                "Preprocessor {} not found in {} module".format(
+                    sk_transformer_name, sk_module_name
+                )
+            )
 
         if args:
             return SklearnPreprocessingTransformer(t(**args), columns)
 
         return SklearnPreprocessingTransformer(t(), columns)
-
-
```

### Comparing `primrose-1.0.9/data/unclustered.csv` & `primrose-2.0.0/data/unclustered.csv`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/test/test_traverser_factory.py` & `primrose-2.0.0/test/test_traverser_factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 import pytest
 from primrose.dag.depth_first_traverser import DepthFirstTraverser
 from primrose.dag.config_layer_traverser import ConfigLayerTraverser
 from primrose.dag.traverser_factory import TraverserFactory
 
+
 def test_instantiate():
-    assert isinstance(TraverserFactory().instantiate('DepthFirstTraverser', None), DepthFirstTraverser)
-    assert isinstance(TraverserFactory().instantiate('ConfigLayerTraverser', None), ConfigLayerTraverser)
-    assert isinstance(TraverserFactory().default_traverser(None), ConfigLayerTraverser)
+    assert isinstance(
+        TraverserFactory().instantiate("DepthFirstTraverser", None), DepthFirstTraverser
+    )
+    assert isinstance(
+        TraverserFactory().instantiate("ConfigLayerTraverser", None),
+        ConfigLayerTraverser,
+    )
+    assert isinstance(TraverserFactory().default_traverser(None), ConfigLayerTraverser)
```

### Comparing `primrose-1.0.9/test/test_factory.py` & `primrose-2.0.0/test/test_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-
 import pytest
 from primrose.node_factory import NodeFactory
 from primrose.writers.abstract_file_writer import AbstractFileWriter
 from primrose.configuration.configuration import Configuration
 from primrose.readers.csv_reader import CsvReader
 
+
 def test_init():
     f1 = NodeFactory()
     f2 = NodeFactory()
 
     class TestWriter(AbstractFileWriter):
         def __init__(self, configuration, instance_name):
             pass
+
         def write(self, data_dict):
             pass
 
     f1.register("TestWriter", TestWriter)
 
     n = len(set(f1.name_dict.keys()))
     assert set(f1.name_dict.keys()) == set(f2.name_dict.keys())
@@ -26,60 +27,63 @@
     # we are doing this to cleanup the singleton and maintain state
     f1.unregister("TestWriter")
 
     # but we as well make into a test
     assert len(set(f1.name_dict.keys())) == n - 1
     assert "TestWriter" not in f1.name_dict
 
+
 def test_unregister():
     f1 = NodeFactory()
+
     class TestWriter(AbstractFileWriter):
         def __init__(self, configuration, instance_name):
             pass
+
         def write(self, data_dict):
             pass
 
     n_before = len(set(f1.name_dict.keys()))
     f1.register("TestWriter", TestWriter)
     n_after = len(set(f1.name_dict.keys()))
     assert n_after == n_before + 1
 
-    f1.unregister('TestWriter')
+    f1.unregister("TestWriter")
 
     assert len(set(f1.name_dict.keys())) == n_before
 
     with pytest.raises(Exception) as e:
-        f1.unregister('doesnotexist')
-    assert 'Key not found doesnotexist' in str(e)
+        f1.unregister("doesnotexist")
+    assert "Key not found doesnotexist" in str(e)
+
 
 def test_valid_configuration():
     f = NodeFactory()
+
     class TestWriter(AbstractFileWriter):
         def __init__(self, configuration, instance_name):
             super(TestWriter, self).__init__(configuration, instance_name)
+
         @staticmethod
         def necessary_config(node_config):
-            return set(['key1', 'key2'])
+            return set(["key1", "key2"])
+
         def write(self, data_dict):
             pass
 
-    f.register('TestWriter', TestWriter)
+    f.register("TestWriter", TestWriter)
 
     config = {
         "class": "TestWriter",
         "key1": "someval1",
         "key2": "someval2",
-        "destinations": []
+        "destinations": [],
     }
 
     is_valid = f.valid_configuration(TestWriter, config)
     assert is_valid
 
-    missing_config = {
-        "class": "TestWriter",
-        "key2": "someval2",
-        "destinations": []
-    }
+    missing_config = {"class": "TestWriter", "key2": "someval2", "destinations": []}
 
     with pytest.raises(Exception) as e:
         f.valid_configuration(TestWriter, missing_config)
-    assert 'Configuration missing necessary keys for' in str(e)
+    assert "Configuration missing necessary keys for" in str(e)
```

### Comparing `primrose-1.0.9/test/test_csv_writer.py` & `primrose-2.0.0/test/test_csv_writer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,124 +1,127 @@
-
 import pytest
 import sys
 import os
 import pandas as pd
 from primrose.configuration.configuration import Configuration
 from primrose.writers.csv_writer import CsvWriter
 from primrose.readers.csv_reader import CsvReader
 from primrose.data_object import DataObject
 
+
 @pytest.fixture()
 def config():
     config = {
         "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ["recipe_csv_writer"]
+                    "destinations": ["recipe_csv_writer"],
                 }
             },
             "writer_config": {
                 "recipe_csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
+                    "filename": "unittest_similar_recipes.csv",
                 }
-            }
+            },
         }
     }
     return config
 
+
 def test_necessary_config(config):
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
-    writer = CsvWriter(configuration, 'recipe_csv_writer')
+    writer = CsvWriter(configuration, "recipe_csv_writer")
     node_config = {
-                    "class": "CsvWriter",
-                    "key":"test_data",
-                    "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
-                }
+        "class": "CsvWriter",
+        "key": "test_data",
+        "dir": "cache",
+        "filename": "unittest_similar_recipes.csv",
+    }
     assert isinstance(writer.necessary_config(node_config), set)
     assert len(writer.necessary_config(node_config)) > 0
 
+
 def test_init_ok(config):
     corpus = pd.read_csv("test/minimal.csv")
 
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
-    writer = CsvWriter(configuration, 'recipe_csv_writer')
+    writer = CsvWriter(configuration, "recipe_csv_writer")
 
     data_object = DataObject(configuration)
-    requestor = CsvReader(configuration, 'csv_reader')
-    data_object.add(requestor, key='test_data', data=corpus)
+    requestor = CsvReader(configuration, "csv_reader")
+    data_object.add(requestor, key="test_data", data=corpus)
 
+    c = configuration.config_for_instance(
+        "recipe_csv_writer"
+    )  # configuration.sec .writer_config['recipe_csv_writer']
+    filename = c["dir"] + os.path.sep + c["filename"]
 
-    c = configuration.config_for_instance('recipe_csv_writer') #configuration.sec .writer_config['recipe_csv_writer']
-    filename = c['dir'] + os.path.sep + c['filename']
-
-    #clean out test file location 
+    # clean out test file location
     if os.path.exists(filename):
         os.remove(filename)
 
     writer.run(data_object)
 
     assert os.path.exists(filename)
 
     df = pd.read_csv(filename)
 
     assert corpus.equals(df)
 
+
 @pytest.fixture()
 def kwargs_config():
     config = {
         "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ["recipe_csv_writer"]
+                    "destinations": ["recipe_csv_writer"],
                 }
             },
             "writer_config": {
                 "recipe_csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
                     "filename": "unittest_similar_recipes.csv",
-                    "kwargs": {
-                        "header": None,
-                        "sep": ":"
-                    }
+                    "kwargs": {"header": None, "sep": ":"},
                 }
-            }
+            },
         }
     }
     return config
 
+
 def test_kwargs(kwargs_config):
     corpus = pd.read_csv("test/minimal.csv")
 
     configuration = Configuration(None, is_dict_config=True, dict_config=kwargs_config)
-    writer = CsvWriter(configuration, 'recipe_csv_writer')
+    writer = CsvWriter(configuration, "recipe_csv_writer")
 
     data_object = DataObject(configuration)
-    requestor = CsvReader(configuration, 'csv_reader')
-    data_object.add(requestor, key='test_data', data=corpus)
-
+    requestor = CsvReader(configuration, "csv_reader")
+    data_object.add(requestor, key="test_data", data=corpus)
 
-    c = configuration.config_for_instance('recipe_csv_writer') #configuration.sec .writer_config['recipe_csv_writer']
-    filename = c['dir'] + os.path.sep + c['filename']
+    c = configuration.config_for_instance(
+        "recipe_csv_writer"
+    )  # configuration.sec .writer_config['recipe_csv_writer']
+    filename = c["dir"] + os.path.sep + c["filename"]
 
-    #clean out test file location
+    # clean out test file location
     if os.path.exists(filename):
         os.remove(filename)
 
     writer.run(data_object)
 
     assert os.path.exists(filename)
 
-    df = pd.read_csv(filename,header=None, sep=':')
+    df = pd.read_csv(filename, header=None, sep=":")
 
-    assert df.shape == (2,2)
+    assert df.shape == (2, 2)
```

### Comparing `primrose-1.0.9/test/test_abstract_model.py` & `primrose-2.0.0/test/test_postprocess.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,87 @@
 import pytest
-import logging
 from primrose.node_factory import NodeFactory
-from primrose.base.model import AbstractModel
-from primrose.data_object import DataObject
-from testfixtures import LogCapture
+from primrose.base.postprocess import AbstractPostprocess
+from primrose.base.node import AbstractNode
 from primrose.configuration.configuration import Configuration
-from primrose.readers.csv_reader import CsvReader
-import pandas as pd
+from primrose.data_object import DataObject, DataObjectResponseType
 
-def test_run():
-    class TestModel(AbstractModel):
 
-        @staticmethod 
-        def necessary_config(node_config): return set(['mode']) 
+def test_init():
+    class TestPostprocess(AbstractPostprocess):
+        #        def __init__(self, configuration, instance_name):
+        #            super(TestPostprocess, self).__init__(configuration, instance_name)
+        @staticmethod
+        def necessary_config(node_config):
+            return set(["key1"])
 
-        def train_model(self, data_object):
-            logging.info("TRAIN called")
-            return data_object
-
-        def eval_model(self, data_object):
-            logging.info("EVAL called")
-            return data_object
-
-        def predict(self, data_object):
-            logging.info("PREDICT called")
-            return data_object
+        def run(self, data_object):
+            data_object.add(self, "some data")
+            return data_object, False
 
-    NodeFactory().register("TestModel", TestModel)
-
-    config = {
-        "implementation_config": {
-            "reader_config": {
-                "myreader": {
-                    "class": "CsvReader",
-                    "filename": "test/minimal.csv",
-                    "destinations": ["mymodel"]
-                }
-            },
-            "model_config": {
-                "mymodel": {
-                    "class": "TestModel",
-                    "mode": "train"
-                }
-            }
-        }
-    }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+        # def process(self, data):
+        #    return "some data"
 
-    data_object = DataObject(configuration)
-
-    reader = CsvReader(configuration, "myreader")
-    df = pd.read_csv("test/minimal.csv")
+    NodeFactory().register("TestPostprocess", TestPostprocess)
 
-    data_object.add(reader, df)
+    class TestModel(AbstractNode):
+        def __init__(self, configuration, instance_name):
+            pass
 
-    model = TestModel(configuration, "mymodel")
+        @staticmethod
+        def necessary_config(node_config):
+            return set(["key1"])
 
+        def run(self, data_object):
+            return data_object, False
 
-    with LogCapture() as l:
-        model.run(data_object)
-    l.check(
-        ('root', 'INFO', 'TRAIN called'),
-        ('root', 'INFO', 'EVAL called'),
-        ('root', 'INFO', 'PREDICT called')
-    )
-
+    NodeFactory().register("TestModel", TestModel)
 
     config = {
         "implementation_config": {
-            "reader_config": {
-                "myreader": {
-                    "class": "CsvReader",
-                    "filename": "test/minimal.csv",
-                    "destinations": ["mymodel"]
-                }
-            },
             "model_config": {
-                "mymodel": {
+                "modelname": {
                     "class": "TestModel",
-                    "mode": "eval"
+                    "key1": "val1",
+                    "destinations": ["nodename"],
                 }
-            }
+            },
+            "postprocess_config": {
+                "nodename": {
+                    "class": "TestPostprocess",
+                    "key1": "val1",
+                    "key2": "val2",
+                    "destinations": [],
+                }
+            },
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     data_object = DataObject(configuration)
 
-    reader = CsvReader(configuration, "myreader")
+    tp = TestPostprocess(configuration, "nodename")
+    node_config = {
+        "class": "TestPostprocess",
+        "key1": "val1",
+        "key2": "val2",
+        "destinations": [],
+    }
+    assert set(["key1"]) == tp.necessary_config(node_config)
+
+    # assert tp.process(None) == "some data"
 
-    data_object.add(reader, df)
+    data_object, terminate = tp.run(data_object)
 
-    model = TestModel(configuration, "mymodel")
+    assert not terminate
 
-    with LogCapture() as l:
-        model.run(data_object)
-    l.check(
-        ('root', 'INFO', 'EVAL called'),
-        ('root', 'INFO', 'PREDICT called')
+    assert (
+        data_object.get("nodename", rtype=DataObjectResponseType.VALUE.value)
+        == "some data"
     )
+
+
+#    assert tp.upstream_model_keys() == ["modelname"]
+
+#    assert tp.single_upstream_model_key() == "modelname"
```

### Comparing `primrose-1.0.9/test/test_sqlite_reader.py` & `primrose-2.0.0/test/test_dill_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,49 @@
 import pytest
-import os
-import sys
-import sqlite3
+from sklearn.tree import DecisionTreeClassifier
 from primrose.configuration.configuration import Configuration
-from primrose.readers.sqlite_reader import SQLiteReader
+from primrose.readers.dill_reader import DillReader
 from primrose.data_object import DataObject, DataObjectResponseType
 
-def test_necessary_config():
-    assert isinstance(SQLiteReader.necessary_config({}), set)
-    assert len(SQLiteReader.necessary_config({})) == 2
 
-def test_read():
+def test_init_ok():
+    try:
+        import sklearn.tree.tree
+        model_filename = "test/tinymodel.dill"
+    except ModuleNotFoundError:
+        model_filename = "test/tinymodel_skl_0_24.dill"
+
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
-                "mynode": {
-                    "class": "SQLiteReader",
-                    "filename": "test/test_sqlite.db",
-                    "query_json": [
-                        {"query": "test/test_sqlite.sql"}
-                    ],
-                    "destinations": []
+                "dill_reader": {
+                    "class": "DillReader",
+                    "filename": model_filename,
+                    "destinations": [],
                 }
             }
         }
     }
-
-    filename = "test/test_sqlite.db"
-    if os.path.exists(filename):
-        os.remove(filename)
-
-    conn = sqlite3.connect(filename)
-    c = conn.cursor()
-    c.execute("create table test(firstname text, lastname text);")
-    c.execute("insert into test(firstname, lastname) values('joe', 'doe'), ('mary','poppins');")
-    conn.commit()
-    conn.close()
-
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    reader = SQLiteReader(configuration, "mynode")
-
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     data_object = DataObject(configuration)
 
+    reader = DillReader(configuration, "dill_reader")
     data_object, terminate = reader.run(data_object)
     assert not terminate
-    dd = data_object.get('mynode', rtype=DataObjectResponseType.KEY_VALUE.value)
-    assert "query_0" in dd
-    df = dd['query_0']
-    assert df is not None
-    assert df.shape == (2, 2)
+    data = data_object.get("dill_reader", rtype=DataObjectResponseType.VALUE.value)
+
+    assert data is not None
+    assert set(data.keys()) == {"test", "model"}
+
+    node_config = {
+        "class": "DillReader",
+        "filename": model_filename,
+        "destinations": [],
+    }
+
+    assert isinstance(DillReader.necessary_config(node_config), set)
+    assert len(DillReader.necessary_config(node_config)) > 0
 
-    if os.path.exists(filename):
-        os.remove(filename)
+    assert data["test"] == [1, 2, 3]
+    assert isinstance(data["model"], DecisionTreeClassifier)
```

### Comparing `primrose-1.0.9/test/test_configuration_dag.py` & `primrose-2.0.0/test/test_configuration_dag.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,238 +5,251 @@
 from primrose.configuration.configuration_dag import ConfigurationDag
 from primrose.configuration.configuration import Configuration
 from primrose.configuration.configuration import OperationType
 from primrose.node_factory import NodeFactory
 from primrose.base.node import AbstractNode
 from primrose.dag.config_layer_traverser import ConfigLayerTraverser
 
+
 def test_check_node_exists():
     with pytest.raises(Exception) as e:
-        ConfigurationDag.check_node_exists(["a","b","c"],"d")
-    assert 'Destination d does not exist' in str(e)
+        ConfigurationDag.check_node_exists(["a", "b", "c"], "d")
+    assert "Destination d does not exist" in str(e)
+
 
 def test_check_cycles_OK():
     config = {
-          "implementation_config":{
-            "reader_config":{
+        "implementation_config": {
+            "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['csv_writer']
+                    "destinations": ["csv_writer"],
                 }
             },
             "writer_config": {
                 "csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
+                    "filename": "unittest_similar_recipes.csv",
                 }
-            }
+            },
         }
     }
 
-    dag = ConfigurationDag(config['implementation_config'])
+    dag = ConfigurationDag(config["implementation_config"])
     dag.create_dag()
     assert dag.check_for_cycles() is None
 
+
 def test_check_cycles_bad():
     config = {
         "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['csv_writer']
+                    "destinations": ["csv_writer"],
                 }
             },
             "writer_config": {
                 "csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
                     "filename": "unittest_similar_recipes.csv",
-                    "destinations": ["csv_reader"]
+                    "destinations": ["csv_reader"],
                 }
-            }
+            },
         }
     }
 
-    dag = ConfigurationDag(config['implementation_config'])
+    dag = ConfigurationDag(config["implementation_config"])
     dag.create_dag()
     with pytest.raises(Exception) as e:
         dag.check_for_cycles()
     assert "Cycle(s) found:" in str(e)
     # it turns out cycle finding code is stochastic so the order of the nodes in the found cycle is not stable. Thus, we look for initial phrase only
     # assert "Cycle(s) found: [('corpus_pipeline', 'recipe_name_model'), ('recipe_name_model', 'corpus_pipeline')]" in str(e)
 
+
 def test_check_cycles_bad2():
     config = {
         "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             },
             "writer_config": {
                 "csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
                     "filename": "unittest_similar_recipes.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
-            }
+            },
         }
     }
 
-    dag = ConfigurationDag(config['implementation_config'])
+    dag = ConfigurationDag(config["implementation_config"])
     dag.create_dag()
     with pytest.raises(Exception) as e:
         dag.check_connected_components()
     assert "Found multiple connected components:" in str(e)
 
+
 def test_type_bad():
     config = {
         "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": [1234]
+                    "destinations": [1234],
                 }
             },
             "writer_config": {
                 1234: {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
                     "filename": "unittest_similar_recipes.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
-            }
+            },
         }
     }
 
-    dag = ConfigurationDag(config['implementation_config'])
+    dag = ConfigurationDag(config["implementation_config"])
     with pytest.raises(Exception) as e:
         dag.create_dag()
     assert "Unrecognized destination type: 1234" in str(e)
 
+
 def test_type_bad2():
     config = {
         "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['doesnotexist']
+                    "destinations": ["doesnotexist"],
                 }
             },
             "writer_config": {
                 "csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
                     "filename": "unittest_similar_recipes.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
-            }
+            },
         }
     }
 
-    dag = ConfigurationDag(config['implementation_config'])
+    dag = ConfigurationDag(config["implementation_config"])
     with pytest.raises(Exception) as e:
         dag.create_dag()
     assert "Did not find doesnotexist destination in" in str(e)
 
+
 @pytest.mark.optional
 @pytest.mark.plotting
 def test_plot_dag():
-
     class TestPostprocess(AbstractNode):
         @staticmethod
         def necessary_config(node_config):
-            return set(['key1', 'key2'])
+            return set(["key1", "key2"])
+
         def run(self, data_object):
             return data_object
+
     NodeFactory().register("TestPostprocess", TestPostprocess)
 
     class Testpipeline(AbstractNode):
-        #def __init__(self, configuration, instance_name):
+        # def __init__(self, configuration, instance_name):
         #    pass
         @staticmethod
         def necessary_config(node_config):
             return set([])
+
         def run(self, data_object):
             return data_object
+
     NodeFactory().register("Testpipeline", Testpipeline)
+
     class TestCleanup(AbstractNode):
         @staticmethod
         def necessary_config(node_config):
             return set([])
+
         def run(self, data_object):
             return data_object
+
     NodeFactory().register("TestCleanup", TestCleanup)
 
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "some/path/to/file",
-                    "destinations": ["pipeline1"]
+                    "destinations": ["pipeline1"],
                 }
             },
             "pipeline_config": {
                 "pipeline1": {
                     "class": "Testpipeline",
-                    "destinations": ["decision_tree_model"]
+                    "destinations": ["decision_tree_model"],
                 }
             },
             "model_config": {
                 "decision_tree_model": {
                     "class": "SklearnClassifierModel",
                     "model_parameters": {},
                     "sklearn_classifier_name": "tree.DecisionTreeClassifier",
                     "grid_search_scoring": "roc_auc",
                     "cv_folds": 3,
                     "mode": "predict",
-                    "destinations": ["nodename"]
+                    "destinations": ["nodename"],
                 }
             },
             "postprocess_config": {
                 "nodename": {
                     "class": "TestPostprocess",
-                    "key1":"val1",
-                    "key2":"val2",
-                    "destinations": ["write_output"]
+                    "key1": "val1",
+                    "key2": "val2",
+                    "destinations": ["write_output"],
                 }
             },
             "writer_config": {
                 "write_output": {
                     "class": "CsvWriter",
                     "key": "read_data",
                     "dir": "cache",
                     "filename": "some/path/to/file.csv",
-                    "destinations": ["donothingsuccess"]
+                    "destinations": ["donothingsuccess"],
                 }
             },
             "cleanup_config": {
                 "donothingsuccess": {
                     "class": "TestCleanup",
                 }
-            }
+            },
         }
     }
 
     cfilename = "test/test_dag_plotting.json"
-    with open(cfilename, 'w') as f:
+    with open(cfilename, "w") as f:
         jstyleson.dump(config, f)
     config = Configuration(config_location=cfilename)
     dag = config.dag
     dag.create_dag()
 
     filename = "test/test_dag_plotting.png"
     if os.path.exists(filename):
@@ -248,215 +261,230 @@
 
     if os.path.exists(cfilename):
         os.remove(cfilename)
 
     if os.path.exists(filename):
         os.remove(filename)
 
+
 def test_upstream_keys1():
     config = {
-        "implementation_config":{
-            "reader_config":{
+        "implementation_config": {
+            "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['csv_writer']
+                    "destinations": ["csv_writer"],
                 }
             },
             "writer_config": {
                 "csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
+                    "filename": "unittest_similar_recipes.csv",
                 }
-            }
+            },
         }
     }
-    dag = ConfigurationDag(config['implementation_config'])
+    dag = ConfigurationDag(config["implementation_config"])
     dag.create_dag()
-    ukeys = dag.upstream_keys('csv_writer')
-    assert list(ukeys) == ['csv_reader']
+    ukeys = dag.upstream_keys("csv_writer")
+    assert list(ukeys) == ["csv_reader"]
 
     with pytest.raises(Exception) as e:
-        dag.upstream_keys('doesnotexist')
+        dag.upstream_keys("doesnotexist")
     assert "Node not found in the DAG:" in str(e)
 
+
 def test_upstream_typed_keys():
     config = {
-        "implementation_config":{
-            "reader_config":{
+        "implementation_config": {
+            "reader_config": {
                 "csv_reader1": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['csv_writer']
+                    "destinations": ["csv_writer"],
                 },
                 "csv_reader2": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['csv_writer']
-                }
+                    "destinations": ["csv_writer"],
+                },
             },
             "writer_config": {
                 "csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
+                    "filename": "unittest_similar_recipes.csv",
                 }
-            }
+            },
         }
     }
-    dag = ConfigurationDag(config['implementation_config'])
+    dag = ConfigurationDag(config["implementation_config"])
     dag.create_dag()
-    ukeys = dag.upstream_typed_keys('csv_writer')
-    assert ukeys == {'csv_reader1': 'reader_config', 'csv_reader2': 'reader_config'}
+    ukeys = dag.upstream_typed_keys("csv_writer")
+    assert ukeys == {"csv_reader1": "reader_config", "csv_reader2": "reader_config"}
+
 
 def test_starting_nodes():
-    #here, we also test descendents()
+    # here, we also test descendents()
 
     config = {
         "metadata": {},
-
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["decision_tree_model"]
+                    "destinations": ["decision_tree_model"],
                 },
                 "read_data2": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["decision_tree_model"]
-                }
+                    "destinations": ["decision_tree_model"],
+                },
             },
             "model_config": {
                 "decision_tree_model": {
                     "class": "SklearnClassifierModel",
                     "model_parameters": {},
                     "sklearn_classifier_name": "tree.DecisionTreeClassifier",
                     "grid_search_scoring": "roc_auc",
                     "cv_folds": 3,
                     "mode": "predict",
-                    "destinations": ["write_output"]
+                    "destinations": ["write_output"],
                 }
             },
             "writer_config": {
                 "write_output": {
                     "class": "CsvWriter",
                     "key": "predictions",
                     "dir": "cache",
-                    "filename": "hello_world_predictions.csv"
+                    "filename": "hello_world_predictions.csv",
                 }
-            }
-        }
+            },
+        },
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     nodes = configuration.dag.starting_nodes()
     assert nodes == set(["read_data", "read_data2"])
 
     downstream_nodes = configuration.dag.descendents("read_data2")
     assert downstream_nodes == set(["decision_tree_model", "write_output"])
 
+
 def test_nodes_of_type():
     config = {
         "metadata": {},
-
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["decision_tree_model"]
+                    "destinations": ["decision_tree_model"],
                 },
                 "read_data2": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["decision_tree_model"]
-                }
+                    "destinations": ["decision_tree_model"],
+                },
             },
             "model_config": {
                 "decision_tree_model": {
                     "class": "SklearnClassifierModel",
                     "mode": "predict",
                     "sklearn_classifier_name": "tree.DecisionTreeClassifier",
                     "grid_search_scoring": "roc_auc",
                     "cv_folds": 3,
                     "model_parameters": {},
-                    "destinations": ["write_output"]
+                    "destinations": ["write_output"],
                 }
             },
             "writer_config": {
                 "write_output": {
                     "class": "CsvWriter",
                     "key": "predictions",
                     "dir": "cache",
-                    "filename": "hello_world_predictions.csv"
+                    "filename": "hello_world_predictions.csv",
                 }
-            }
-        }
+            },
+        },
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     nodes = configuration.dag.nodes_of_type(OperationType.reader)
     assert nodes == set(["read_data", "read_data2"])
 
     nodes = configuration.dag.nodes_of_type(OperationType.pipeline)
     assert nodes == set([])
 
-    nodes = configuration.dag.upstream_nodes_of_type("write_output", OperationType.reader)
+    nodes = configuration.dag.upstream_nodes_of_type(
+        "write_output", OperationType.reader
+    )
     assert nodes == set(["read_data", "read_data2"])
 
-    nodes = configuration.dag.upstream_nodes_of_type("write_output", OperationType.cleanup)
+    nodes = configuration.dag.upstream_nodes_of_type(
+        "write_output", OperationType.cleanup
+    )
     assert nodes == set([])
 
 
 def test_paths():
     config = {
         "metadata": {},
-
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["read_data2", "decision_tree_model"]
+                    "destinations": ["read_data2", "decision_tree_model"],
                 },
                 "read_data2": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["decision_tree_model"]
-                }
+                    "destinations": ["decision_tree_model"],
+                },
             },
             "model_config": {
                 "decision_tree_model": {
                     "class": "SklearnClassifierModel",
                     "mode": "train",
                     "sklearn_classifier_name": "tree.DecisionTreeClassifier",
                     "grid_search_scoring": "roc_auc",
                     "cv_folds": 3,
                     "model_parameters": {},
-                    "destinations": ["write_output"]
+                    "destinations": ["write_output"],
                 }
             },
             "writer_config": {
                 "write_output": {
                     "class": "CsvWriter",
                     "key": "predictions",
                     "dir": "cache",
-                    "filename": "hello_world_predictions.csv"
+                    "filename": "hello_world_predictions.csv",
                 }
-            }
-        }
+            },
+        },
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     paths = list(configuration.dag.paths("read_data", "write_output"))
     assert len(paths) == 2
-    assert paths[0] == ['read_data', 'read_data2', 'decision_tree_model', 'write_output']
-    assert paths[1] == ['read_data', 'decision_tree_model', 'write_output']
+    assert paths[0] == [
+        "read_data",
+        "read_data2",
+        "decision_tree_model",
+        "write_output",
+    ]
+    assert paths[1] == ["read_data", "decision_tree_model", "write_output"]
 
     paths = configuration.dag.paths("write_output", "decision_tree_model")
     assert not paths
-
```

### Comparing `primrose-1.0.9/test/test_cluster_plotter.py` & `primrose-2.0.0/test/test_cluster_plotter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,73 @@
-
 import pytest
 from primrose.configuration.configuration import Configuration
 from primrose.dag_runner import DagRunner
 import os
 
+
 def test_run():
     config = {
         "metadata": {
             "section_registry": [
                 "reader_config",
                 "pipeline_config",
                 "model_config",
-                "dataviz_config"
+                "dataviz_config",
             ]
         },
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/unclustered.csv",
-                    "destinations": [
-                        "normalize_data"
-                    ]
+                    "destinations": ["normalize_data"],
                 }
             },
             "pipeline_config": {
                 "normalize_data": {
                     "class": "SklearnPreprocessingPipeline",
                     "operations": [
-                        {"class":"preprocessing.StandardScaler", "columns": ["x", "y"], "args": {"with_mean": True, "with_std": True}},
+                        {
+                            "class": "preprocessing.StandardScaler",
+                            "columns": ["x", "y"],
+                            "args": {"with_mean": True, "with_std": True},
+                        },
                     ],
                     "is_training": True,
                     "training_fraction": 0.65,
                     "seed": 42,
-                    "destinations": [
-                        "cluster_model"
-                    ]
+                    "destinations": ["cluster_model"],
                 }
             },
             "model_config": {
-                "cluster_model":{
+                "cluster_model": {
                     "class": "SklearnClusterModel",
                     "mode": "train",
-                    "features": ["x","y"],
-                    "model": {"class": "cluster.KMeans", "args": {"n_clusters": 6, "random_state": 42}},
-                    "destinations": [
-                        "cluster_plotter"
-                    ]
+                    "features": ["x", "y"],
+                    "model": {
+                        "class": "cluster.KMeans",
+                        "args": {"n_clusters": 6, "random_state": 42},
+                    },
+                    "destinations": ["cluster_plotter"],
                 }
             },
             "dataviz_config": {
                 "cluster_plotter": {
                     "class": "ClusterPlotter",
                     "id_col": "predictions",
                     "filename": "clusters.png",
                     "title": "Results of KMeans(k=6)",
-                    "destinations": []
+                    "destinations": [],
                 }
-            }
-        }
+            },
+        },
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     fname = "clusters.png"
 
     if os.path.exists(fname):
         os.remove(fname)
 
     DagRunner(configuration).run()
```

### Comparing `primrose-1.0.9/test/test_s3_writer.py` & `primrose-2.0.0/test/test_s3_writer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,81 @@
-
 import pytest
 import sys
 import os
 import boto3
 from moto import mock_s3
 import pandas as pd
 from primrose.configuration.configuration import Configuration
 from primrose.writers.s3_writer import S3Writer
 from primrose.node_factory import NodeFactory
 from primrose.data_object import DataObject
 from primrose.base.node import AbstractNode
 
+
 @mock_s3
 def test_init_ok():
     config = {
         "implementation_config": {
             "postprocess_config": {
                 "nodename": {
                     "class": "TestPostprocess",
-                    "key1":"val1",
-                    "key2":"val2",
-                    "destinations": ["recipe_s3_writer"]
+                    "key1": "val1",
+                    "key2": "val2",
+                    "destinations": ["recipe_s3_writer"],
                 }
             },
             "writer_config": {
                 "recipe_s3_writer": {
                     "class": "S3Writer",
                     "dir": "cache",
                     "key": DataObject.DATA_KEY,
                     "bucket_name": "does_not_exist_bucket_name",
-                    "bucket_filename": "does_not_exist.csv"
+                    "bucket_filename": "does_not_exist.csv",
                 }
-            }
+            },
         }
     }
+
     class TestPostprocess(AbstractNode):
         @staticmethod
         def necessary_config(node_config):
-            return set(['key1', 'key2'])
-        def run(self, data_object): return data_object
+            return set(["key1", "key2"])
+
+        def run(self, data_object):
+            return data_object
+
     NodeFactory().register("TestPostprocess", TestPostprocess)
 
-    #this is to mock out the boto connection
-    os.environ["AWS_ACCESS_KEY_ID"] = "fake" 
+    # this is to mock out the boto connection
+    os.environ["AWS_ACCESS_KEY_ID"] = "fake"
     os.environ["AWS_SECRET_ACCESS_KEY"] = "fake"
-    conn = boto3.resource('s3')
+    conn = boto3.resource("s3")
     # We need to create the bucket since this is all in Moto's 'virtual' AWS account
-    conn.create_bucket(Bucket='does_not_exist_bucket_name')
+    conn.create_bucket(Bucket="does_not_exist_bucket_name")
 
     reference_file_path = "test/minimal.csv"
 
     corpus = pd.read_csv(reference_file_path)
 
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     data_object = DataObject(configuration)
 
-    requestor = TestPostprocess(configuration, 'nodename')
+    requestor = TestPostprocess(configuration, "nodename")
 
     data_object.add(requestor, corpus)
 
-    writer = S3Writer(configuration, 'recipe_s3_writer')
+    writer = S3Writer(configuration, "recipe_s3_writer")
     node_config = {
-                    "class": "S3Writer",
-                    "dir": "cache",
-                    "key": DataObject.DATA_KEY,
-                    "bucket_name": "does_not_exist_bucket_name",
-                    "bucket_filename": "does_not_exist.csv"
-                }
+        "class": "S3Writer",
+        "dir": "cache",
+        "key": DataObject.DATA_KEY,
+        "bucket_name": "does_not_exist_bucket_name",
+        "bucket_filename": "does_not_exist.csv",
+    }
     keys = writer.necessary_config(node_config)
     assert keys is not None
     assert isinstance(keys, set)
     assert len(keys) > 0
 
     # write to file
     filename = writer._write_locally(data_object)
@@ -82,9 +86,14 @@
     just_written = pd.read_csv(filename)
 
     assert reference.equals(just_written)
 
     os.remove(filename)
 
     data_object = writer.run(data_object)
-    body = conn.Object('does_not_exist_bucket_name', 'does_not_exist.csv').get()['Body'].read().decode("utf-8")
-    assert body == open(reference_file_path).read()
+    body = (
+        conn.Object("does_not_exist_bucket_name", "does_not_exist.csv")
+        .get()["Body"]
+        .read()
+        .decode("utf-8")
+    )
+    assert body == open(reference_file_path).read()
```

### Comparing `primrose-1.0.9/test/test_postgres_reader.py` & `primrose-2.0.0/test/test_postgres_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,61 @@
-
 import pytest
 import os
 import pandas as pd
 
 from primrose.readers.postgres_reader import PostgresReader
 from primrose.configuration.configuration import Configuration
 from primrose.data_object import DataObject, DataObjectResponseType
 from unittest.mock import patch
 
+
 def test_necessary_config():
     assert len(PostgresReader.necessary_config({})) == 1
 
 
 @pytest.mark.optional
 @pytest.mark.postgres
 def test_run(monkeypatch):
     config = {
         "implementation_config": {
             "reader_config": {
                 "mynode": {
                     "class": "PostgresReader",
-                    "query_json": [
-                        {"query": "test/test_mysql.sql"}
-                    ],
-                    "destinations": []
+                    "query_json": [{"query": "test/test_mysql.sql"}],
+                    "destinations": [],
                 }
             }
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     data_object = DataObject(configuration)
 
-    keys = ["POSTGRES_HOST",
-            "POSTGRES_PORT",
-            "POSTGRES_DB",
-            "POSTGRES_USER",
-            "POSTGRES_PASS"]
+    keys = [
+        "POSTGRES_HOST",
+        "POSTGRES_PORT",
+        "POSTGRES_DB",
+        "POSTGRES_USER",
+        "POSTGRES_PASS",
+    ]
     for i, k in enumerate(keys):
         os.environ[k] = str(i)
 
-    reader = PostgresReader(configuration, 'mynode')
+    reader = PostgresReader(configuration, "mynode")
 
-    with patch('psycopg2.connect') as mock_connect:
+    with patch("psycopg2.connect") as mock_connect:
 
         def fake_df(query, con):
-            return pd.DataFrame({'Name':['Tom', 'nick', 'krish', 'jack'], 'Age':[20, 21, 19, 18]})
-        monkeypatch.setattr(pd,'read_sql',fake_df)
+            return pd.DataFrame(
+                {"Name": ["Tom", "nick", "krish", "jack"], "Age": [20, 21, 19, 18]}
+            )
+
+        monkeypatch.setattr(pd, "read_sql", fake_df)
 
         data_object, terminate = reader.run(data_object)
 
         assert not terminate
 
-        dd = data_object.get('mynode', rtype=DataObjectResponseType.KEY_VALUE.value)
-        assert 'query_0' in dd
-        df = dd['query_0']
-        assert list(df.T.to_dict().values())[0] == {'Name': "Tom", "Age": 20}
+        dd = data_object.get("mynode", rtype=DataObjectResponseType.KEY_VALUE.value)
+        assert "query_0" in dd
+        df = dd["query_0"]
+        assert list(df.T.to_dict().values())[0] == {"Name": "Tom", "Age": 20}
```

### Comparing `primrose-1.0.9/test/test_sklearn_classifier_model.py` & `primrose-2.0.0/test/test_sklearn_classifier_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,55 +12,72 @@
     return Configuration("test/hello_world_tennis.json")
 
 
 @pytest.fixture()
 def data_obj(config):
     df = pd.read_csv("test/tennis.csv")
     data_object = DataObject(config)
-    reader = CsvReader(config, 'read_data')
+    reader = CsvReader(config, "read_data")
     data_object.add(reader, df)
-    encoder = EncodeTrainTestSplit(config, 'encode_and_split')
+    encoder = EncodeTrainTestSplit(config, "encode_and_split")
     data_object, terminate = encoder.run(data_object)
     return data_object
 
 
 @pytest.fixture
 def model(config):
     return SklearnClassifierModel(config, "decision_tree_model")
 
 
 def test_necessary_config():
-    assert SklearnClassifierModel.necessary_config({}) == set(["model_parameters", "mode", "sklearn_classifier_name",
-                                                             "grid_search_scoring", "cv_folds"])
+    assert SklearnClassifierModel.necessary_config({}) == set(
+        [
+            "model_parameters",
+            "mode",
+            "sklearn_classifier_name",
+            "grid_search_scoring",
+            "cv_folds",
+        ]
+    )
 
 
 def test_get_data(model, data_obj):
     x_train, y_train, x_test, y_test = model._get_data(data_obj)
     assert x_train.shape[0] == y_train.shape[0]
-    assert x_test.shape[0] == y_test.shape[0]  # we removed the ID column by not specifying it in X
+    assert (
+        x_test.shape[0] == y_test.shape[0]
+    )  # we removed the ID column by not specifying it in X
 
 
 def test_train_model(model, data_obj):
     model.train_model(data_obj)
     assert model.model is not None
     x_train, y_train, x_test, y_test = model._get_data(data_obj)
     predictions = model.model.predict(x_test)
-    assert list(predictions) == [1, 1, 0, 1, 1]
+    assert list(predictions) == [1, 0, 0, 1, 1]
 
 
 def test_eval(model, data_obj):
     model.train_model(data_obj)
     model.eval_model(data_obj)
     print(model.scores)
-    assert model.scores['recall'] == 1.0
-    assert model.scores['precision'] == 0.75
-    assert model.scores['predicted_class_fraction'] == 0.8
-    assert model.scores['positive_class_fraction'] == 0.6
+    assert round(model.scores["recall"], 2) == 0.67
+    assert round(model.scores["precision"], 2) == 0.67
+    assert model.scores["predicted_class_fraction"] == 0.6
+    assert model.scores["positive_class_fraction"] == 0.6
 
 
 def test_predict(model, data_obj):
     model.train_model(data_obj)
     data_object = model.predict(data_obj)
-    predicted = data_object.get('decision_tree_model', rtype=DataObjectResponseType.KEY_VALUE.value)
-
-    assert predicted['predictions'].shape[0] == 5
-    assert list(predicted['predictions'].predictions) == ['yes', 'yes', 'no', 'yes', 'yes']
+    predicted = data_object.get(
+        "decision_tree_model", rtype=DataObjectResponseType.KEY_VALUE.value
+    )
+
+    assert predicted["predictions"].shape[0] == 5
+    assert list(predicted["predictions"].predictions) == [
+        "yes",
+        "no",
+        "no",
+        "yes",
+        "yes",
+    ]
```

### Comparing `primrose-1.0.9/test/test_notification_utils.py` & `primrose-2.0.0/test/test_notification_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,51 @@
 """e
     Module with all tests for the slack integration implementations
     author(s): Parul Laul (parul.laul@ww.com)
 """
-
-import os
-import unittest
 import unittest.mock as mock
+import pytest
+import logging
 
 from primrose.notification_utils import SlackClient, get_notification_client
 
 
-class TestSlackClient(unittest.TestCase):
-    """Tests for SlackClient in notification_utils.py"""
-
-    def test_post(self):
-        client_mock = mock.Mock(return_value=mock.Mock())
-
-        # instantiate instance
-        slack_instance = SlackClient(channel='some_channel', member_id='USomeUserID', token='some_token')
-        slack_instance.client = client_mock.return_value
-
-        slack_instance.post_message(message='test message')
-
-        # check method is called
-        slack_instance.client.chat_postMessage.assert_called_once_with(
-            channel='some_channel',
-            text='test message\n <@USomeUserID>'
-        )
-
-
-class TestGetNotificationClient(unittest.TestCase):
-    """Tests for get_notification_client in notification_utils.py"""
-
-    def test_get_notification_client(self):
-        importlib_mock = mock.Mock()
-        getattr_mock = mock.Mock()
-
-        patches = {
-            'importlib': importlib_mock,
-            'getattr': getattr_mock
-        }
-        path = 'primrose.notification_utils'
-        with mock.patch.multiple(path, **patches):
-            client_params = {'some': 'params', 'client': 'needed', 'token': 'needed'}
-
-            _ = get_notification_client(client_params)
-
-        self.assertEqual(importlib_mock.import_module.call_count, 1)
-        self.assertEqual(getattr_mock.call_count, 1)
-
-    def test_get_notification_client_exc(self):
-        client_params = {'client': 'DoesNotExist'}
-        self.assertRaises(AttributeError, get_notification_client(client_params))
-
+def test_post():
+    client_mock = mock.Mock(return_value=mock.Mock())
 
-if __name__ == '__main__':
-    unittest.main()
+    # instantiate instance
+    slack_instance = SlackClient(
+        channel="some_channel", member_id="USomeUserID", token="some_token"
+    )
+    slack_instance.client = client_mock.return_value
+
+    slack_instance.post_message(message="test message")
+
+    # check method is called
+    slack_instance.client.chat_postMessage.assert_called_once_with(
+        channel="some_channel", text="test message\n <@USomeUserID>"
+    )
+
+
+def test_get_notification_client():
+    importlib_mock = mock.Mock()
+    getattr_mock = mock.Mock()
+
+    patches = {"importlib": importlib_mock, "getattr": getattr_mock}
+    path = "primrose.notification_utils"
+    with mock.patch.multiple(path, **patches):
+        client_params = {"some": "params", "client": "needed", "token": "needed"}
+
+        _ = get_notification_client(client_params)
+
+    assert importlib_mock.import_module.call_count == 1
+    assert getattr_mock.call_count == 1
+
+
+def test_get_notification_client_exc(caplog):
+    client_params = {"client": "DoesNotExist"}
+    with caplog.at_level(logging.ERROR):
+        get_notification_client(client_params)
+    assert (
+        "Are you sure DoesNotExist is in <module 'primrose.notification_utils'"
+        in caplog.text
+    )
```

### Comparing `primrose-1.0.9/test/test_config_layer_traverser.py` & `primrose-2.0.0/test/test_dill_writer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,76 @@
-
 import pytest
+import os
+import dill
 from primrose.configuration.configuration import Configuration
-from primrose.dag.config_layer_traverser import ConfigLayerTraverser
+from primrose.writers.dill_writer import DillWriter
+from primrose.data_object import DataObject
+from primrose.readers.csv_reader import CsvReader
+
 
-def test__sort_by_depth_first():
+@pytest.fixture()
+def config():
     config = {
-        "implementation_config":{
-            "reader_config":{
+        "implementation_config": {
+            "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['csv_writer']
-                },
-                "csv_reader2": {
-                    "class": "CsvReader",
-                    "filename": "test/minimal.csv",
-                    "destinations": ['successlogger']
+                    "destinations": ["recipe_file_writer"],
                 }
             },
             "writer_config": {
-                "csv_writer": {
-                    "class": "CsvWriter",
-                    "key":"test_data",
+                "recipe_file_writer": {
+                    "class": "FileWriter",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv",
-                    "destinations": ["successlogger"]
+                    "filename": "unittest_file_writer.dill",
                 }
             },
-            "cleanup_config": {
-                "successlogger": {
-                    "class": "LoggingSuccess",
-                    "msg": "woohoo, all done!",
-                    "level": "INFO",
-                }
-            }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    traverser = ConfigLayerTraverser(configuration)
+    return config
 
-    sequence = traverser._sort_by_depth_first(['successlogger', 'csv_reader', 'csv_writer','csv_reader2'])
-    assert sequence == ['csv_reader2', 'csv_reader', 'csv_writer', 'successlogger']
 
-def test_traversal_list():
-    config = {
-        "implementation_config":{
-            "reader_config":{
-                "csv_reader": {
-                    "class": "CsvReader",
-                    "filename": "test/minimal.csv",
-                    "destinations": ['csv_writer']
-                },
-                "csv_reader2": {
-                    "class": "CsvReader",
-                    "filename": "test/minimal.csv",
-                    "destinations": ['successlogger']
-                }
-            },
-            "writer_config": {
-                "csv_writer": {
-                    "class": "CsvWriter",
-                    "key":"test_data",
-                    "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv",
-                    "destinations": ["successlogger"]
-                }
-            },
-            "cleanup_config": {
-                "successlogger": {
-                    "class": "LoggingSuccess",
-                    "msg": "woohoo, all done!",
-                    "level": "INFO",
-                }
-            }
-        }
+def test_necessary_config(config):
+    configuration = Configuration(None, is_dict_config=True, dict_config=config)
+    writer = DillWriter(configuration, "recipe_file_writer")
+    node_config = {
+        "class": "FileWriter",
+        "key": "test_data",
+        "dir": "cache",
+        "filename": "unittest_file_writer.dill",
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    traverser = ConfigLayerTraverser(configuration)
-    sequence = traverser.traversal_list()
-    assert sequence == ['csv_reader2', 'csv_reader', 'csv_writer', 'successlogger']
+    assert isinstance(writer.necessary_config(node_config), set)
+    assert len(writer.necessary_config(node_config)) > 0
+
+
+def test_init_ok(config):
+
+    test_data_string = "some test data"
+
+    configuration = Configuration(None, is_dict_config=True, dict_config=config)
+
+    data_object = DataObject(configuration)
+
+    requestor = CsvReader(configuration, "csv_reader")
+
+    data_object.add(requestor, test_data_string, "test_data")
+
+    writer = DillWriter(configuration, "recipe_file_writer")
+
+    c = configuration.config_for_instance("recipe_file_writer")
+    filename = c["dir"] + os.path.sep + c["filename"]
+
+    # clean out test file location
+    if os.path.exists(filename):
+        os.remove(filename)
+
+    data_object, terminate = writer.run(data_object)
+
+    assert not terminate
+
+    assert os.path.exists(filename)
+
+    read_data = dill.load(open(filename, "rb"))
+
+    assert test_data_string == read_data
```

### Comparing `primrose-1.0.9/test/test_mysql_reader.py` & `primrose-2.0.0/test/test_mysql_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,56 @@
-
 import pytest
 import os
 import pandas as pd
 
 from primrose.readers.mysql_reader import MySQLReader
 from primrose.configuration.configuration import Configuration
 import mysql.connector
 from primrose.data_object import DataObject, DataObjectResponseType
 from unittest.mock import patch
 
+
 def test_necessary_config():
     assert len(MySQLReader.necessary_config({})) == 1
 
+
 def test_run(monkeypatch):
     config = {
         "implementation_config": {
             "reader_config": {
                 "mynode": {
                     "class": "MySQLReader",
-                    "query_json": [
-                        {"query": "test/test_mysql.sql"}
-                    ],
-                    "destinations": []
+                    "query_json": [{"query": "test/test_mysql.sql"}],
+                    "destinations": [],
                 }
             }
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     data_object = DataObject(configuration)
 
-    keys = ["MYSQL_HOST",
-            "MYSQL_PORT",
-            "MYSQL_DB",
-            "MYSQL_USER",
-            "MYSQL_PASS"]
+    keys = ["MYSQL_HOST", "MYSQL_PORT", "MYSQL_DB", "MYSQL_USER", "MYSQL_PASS"]
     for i, k in enumerate(keys):
         os.environ[k] = str(i)
 
-    reader = MySQLReader(configuration, 'mynode')
+    reader = MySQLReader(configuration, "mynode")
 
-    #FIXME need to test reader.run(data_object)
+    # FIXME need to test reader.run(data_object)
 
-    with patch(target='mysql.connector.connect') as mock:
+    with patch(target="mysql.connector.connect") as mock:
 
         def fake_df(query, con):
-            return pd.DataFrame({'Name':['Tom', 'nick', 'krish', 'jack'], 'Age':[20, 21, 19, 18]})
+            return pd.DataFrame(
+                {"Name": ["Tom", "nick", "krish", "jack"], "Age": [20, 21, 19, 18]}
+            )
 
-        monkeypatch.setattr(pd,'read_sql',fake_df)
+        monkeypatch.setattr(pd, "read_sql", fake_df)
 
         data_object, terminate = reader.run(data_object)
 
         assert not terminate
 
-        dd = data_object.get('mynode', rtype=DataObjectResponseType.KEY_VALUE.value)
-        assert 'query_0' in dd
-        df = dd['query_0']
-        assert list(df.T.to_dict().values())[0] == {'Name': "Tom", "Age": 20}
+        dd = data_object.get("mynode", rtype=DataObjectResponseType.KEY_VALUE.value)
+        assert "query_0" in dd
+        df = dd["query_0"]
+        assert list(df.T.to_dict().values())[0] == {"Name": "Tom", "Age": 20}
```

### Comparing `primrose-1.0.9/test/test_dill_reader.py` & `primrose-2.0.0/test/test_sklearn_dataset_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,30 @@
 import pytest
-from sklearn.tree import DecisionTreeClassifier
+from primrose.readers.sklearn_dataset_reader import SklearnDatasetReader
 from primrose.configuration.configuration import Configuration
-from primrose.readers.dill_reader import DillReader
 from primrose.data_object import DataObject, DataObjectResponseType
 
 
-def test_init_ok():
+def test_run():
     config = {
         "implementation_config": {
             "reader_config": {
-                "dill_reader": {
-                    "class": "DillReader",
-                    "filename": "test/tinymodel.dill",
-                    "destinations": []
+                "dataset_reader": {
+                    "class": "SklearnDatasetReader",
+                    "dataset": "iris",
+                    "destinations": [],
                 }
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     data_object = DataObject(configuration)
-
-    reader = DillReader(configuration, "dill_reader")
+    reader = SklearnDatasetReader(configuration, "dataset_reader")
     data_object, terminate = reader.run(data_object)
     assert not terminate
-    data = data_object.get('dill_reader', rtype=DataObjectResponseType.VALUE.value)
-
-    assert data is not None
-    assert set(data.keys()) == {'test', 'model'}
-
-    node_config = {
-                    "class": "DillReader",
-                    "filename": "test/tinymodel.dill",
-                    "destinations": []
-                }
-
-    assert isinstance(DillReader.necessary_config(node_config), set)
-    assert len(DillReader.necessary_config(node_config)) > 0
-
-    assert data['test'] == [1, 2, 3]
-    assert isinstance(data['model'], DecisionTreeClassifier)
+    df = data_object.get("dataset_reader", rtype=DataObjectResponseType.VALUE.value)
+    assert len(df.columns) == 5
+    assert "target" in df.columns
+    assert df.shape == (150, 5)
+    assert "sepal length (cm)" in df.columns
```

### Comparing `primrose-1.0.9/test/test_r_reader.py` & `primrose-2.0.0/test/test_r_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import pytest
 import sys
 import os
 import pandas as pd
 from primrose.configuration.configuration import Configuration
 from primrose.readers.r_reader import RReader
 from primrose.node_factory import NodeFactory
@@ -10,58 +9,64 @@
 from primrose.base.node import AbstractNode
 from primrose.data_object import DataObject, DataObjectResponseType
 
 
 def check_rpy2():
     try:
         import rpy2
+
         return False
     except ImportError as e:
         return True
 
+
 @pytest.mark.skipif(check_rpy2(), reason="primrose[R] is optional")
 def test_run():
     config = {
         "implementation_config": {
             "reader_config": {
-                "read_data": {
-                    "class": "RReader",
-                    "dataset": "iris",
-                    "destinations": []
-                }
+                "read_data": {"class": "RReader", "dataset": "iris", "destinations": []}
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     data_object = DataObject(configuration)
 
     reader = RReader(configuration, "read_data")
     data_object, terminate = reader.run(data_object)
     assert not terminate
-    df = data_object.get('read_data', rtype=DataObjectResponseType.VALUE.value)
+    df = data_object.get("read_data", rtype=DataObjectResponseType.VALUE.value)
     assert df is not None
     assert df.shape == (150, 6)
-    assert list(df.columns) == ["Sepal.Length", "Sepal.Width", "Petal.Length", "Petal.Width", "Species", "row_names"]
+    assert list(df.columns) == [
+        "Sepal.Length",
+        "Sepal.Width",
+        "Petal.Length",
+        "Petal.Width",
+        "Species",
+        "row_names",
+    ]
+
 
 @pytest.mark.skipif(check_rpy2(), reason="primrose[R] is optional")
 def test_run2():
     config = {
         "implementation_config": {
             "reader_config": {
-                "read_data": {
-                    "class": "RReader",
-                    "dataset": "euro",
-                    "destinations": []
-                }
+                "read_data": {"class": "RReader", "dataset": "euro", "destinations": []}
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     data_object = DataObject(configuration)
 
     reader = RReader(configuration, "read_data")
     data_object, terminate = reader.run(data_object)
     assert not terminate
-    df = data_object.get('read_data', rtype=DataObjectResponseType.VALUE.value)
+    df = data_object.get("read_data", rtype=DataObjectResponseType.VALUE.value)
     assert df is not None
     assert df.shape == (11, 2)
     assert list(df.columns) == ["euro", "row_names"]
```

### Comparing `primrose-1.0.9/test/test_categoricals.py` & `primrose-2.0.0/test/test_categoricals.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,81 @@
-
 import pytest
 import pandas as pd
 from primrose.transformers.categoricals import ExplicitCategoricalTransform
 
+
 def test__process_transformations():
     categoricals = {
         "currency": {
-            "transformations": [
-                "{x}[{x}=='USD'] = 1",
-                "{x}[{x}=='EUR'] = 2"
-            ],
+            "transformations": ["{x}[{x}=='USD'] = 1", "{x}[{x}=='EUR'] = 2"],
             "rename": "money",
-            "to_numeric": True
+            "to_numeric": True,
         }
     }
     x = "data['{}']".format("currency")
     input_data = categoricals["currency"]
 
-    data = pd.DataFrame(data={"currency": ['EUR', 'USD', 'USD']})
+    data = pd.DataFrame(data={"currency": ["EUR", "USD", "USD"]})
 
-    ExplicitCategoricalTransform._process_transformations(data, input_data, "currency", x)
+    ExplicitCategoricalTransform._process_transformations(
+        data, input_data, "currency", x
+    )
 
     assert list(data.currency) == [2, 1, 1]
     assert "money" not in list(data.columns)
 
-    data, new_name = ExplicitCategoricalTransform._process_rename(data, input_data, "currency")
+    data, new_name = ExplicitCategoricalTransform._process_rename(
+        data, input_data, "currency"
+    )
 
     assert "money" in list(data.columns)
     assert list(data.money) == [2, 1, 1]
 
-    assert str(data.dtypes['money']) == "object"
+    assert str(data.dtypes["money"]) == "object"
 
     data = ExplicitCategoricalTransform._process_numeric(data, input_data, new_name)
 
-    assert str(data.dtypes['money']) == "int64"
+    assert str(data.dtypes["money"]) == "int64"
+
 
 def test__process_numeric():
-    input_data = {
-        "to_numeric": True
-    }
-    data = pd.DataFrame(data={"currency": ['EUR', 'USD', 'USD']})
+    input_data = {"to_numeric": True}
+    data = pd.DataFrame(data={"currency": ["EUR", "USD", "USD"]})
     data = ExplicitCategoricalTransform._process_numeric(data, input_data, "currency")
 
-    assert list(data.currency) == 3*[ExplicitCategoricalTransform.DEFAULT_NUMERIC]
+    assert list(data.currency) == 3 * [ExplicitCategoricalTransform.DEFAULT_NUMERIC]
+
 
 def test__process_numeric_no_config_key():
     input_data = {}
-    data = pd.DataFrame(data={"currency": ['EUR', 'USD', 'USD']})
+    data = pd.DataFrame(data={"currency": ["EUR", "USD", "USD"]})
     data = ExplicitCategoricalTransform._process_numeric(data, input_data, "currency")
 
     assert data is not None
 
+
 def test__process_rename():
-    input_data = {
-        "transformations": [
-            "{x}[{x}=='USD'] = 1",
-            "{x}[{x}=='EUR'] = 2"
-        ]
-    }
-    data = pd.DataFrame(data={"currency": ['EUR', 'USD', 'USD']})
-    data, new_name = ExplicitCategoricalTransform._process_rename(data, input_data, "currency")
+    input_data = {"transformations": ["{x}[{x}=='USD'] = 1", "{x}[{x}=='EUR'] = 2"]}
+    data = pd.DataFrame(data={"currency": ["EUR", "USD", "USD"]})
+    data, new_name = ExplicitCategoricalTransform._process_rename(
+        data, input_data, "currency"
+    )
     assert new_name == "currency"
 
+
 def test_transform():
     categoricals = {
         "currency": {
-            "transformations": [
-                "{x}[{x}=='USD'] = 1",
-                "{x}[{x}=='EUR'] = 2"
-            ],
+            "transformations": ["{x}[{x}=='USD'] = 1", "{x}[{x}=='EUR'] = 2"],
             "rename": "money",
-            "to_numeric": True
+            "to_numeric": True,
         }
     }
-    data = pd.DataFrame(data={"currency": ['EUR', 'USD', 'USD']})
+    data = pd.DataFrame(data={"currency": ["EUR", "USD", "USD"]})
     t = ExplicitCategoricalTransform(categoricals)
 
-    #does nothing
+    # does nothing
     t.fit(data)
 
     data_out = t.transform(data)
     assert list(data_out.money) == [2, 1, 1]
-    assert str(data_out.dtypes['money']) == "int64"
+    assert str(data_out.dtypes["money"]) == "int64"
```

### Comparing `primrose-1.0.9/test/test_encode_train_test_split.py` & `primrose-2.0.0/test/test_encode_train_test_split.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 @pytest.fixture()
 def configuration():
     return Configuration("test/hello_world_tennis.json")
 
 
 @pytest.fixture
 def data_obj_factory(configuration):
-
     def data_object_factory():
         df = pd.read_csv("test/tennis.csv")
 
         data_object = DataObject(configuration)
 
         csv_reader = CsvReader(configuration, "read_data")
 
@@ -39,53 +38,57 @@
 
     df1 = pd.read_csv("test/tennis.csv")
     df2 = pd.read_csv("test/tennis.csv")
 
     data_object = DataObject(configuration)
     csv_reader = CsvReader(configuration, "read_data")
 
-    data_object.add(csv_reader, df1, 'query1')
-    data_object.add(csv_reader, df2, 'query2')
+    data_object.add(csv_reader, df1, "query1")
+    data_object.add(csv_reader, df2, "query2")
 
     data_object, terminate = pipeline_obj.run(data_object)
 
-    encoded_data = data_object.get('encode_and_split')['data_train']
+    encoded_data = data_object.get("encode_and_split")["data_train"]
 
     assert len(encoded_data) == 18
 
 
 def test_encode_data(data_obj_factory, pipeline_obj):
 
     data_obj = data_obj_factory()
 
     data_object, terminate = pipeline_obj.run(data_obj)
 
-    encoded_data = data_object.get('encode_and_split')['data_train']
-    encoded_target = data_object.get('encode_and_split')['target_train']
+    encoded_data = data_object.get("encode_and_split")["data_train"]
+    encoded_target = data_object.get("encode_and_split")["target_train"]
 
     assert set(list(encoded_data.outlook.unique())) == set([0, 1, 2])
     assert set(list(encoded_data.temp.unique())) == set([0, 1, 2])
     assert set(list(encoded_data.humidity.unique())) == set([0, 1])
     assert set(list(encoded_data.windy.unique())) == set([True, False])
     assert set(list(encoded_target.unique())) == set([0, 1])
 
     assert pipeline_obj.transformer_sequence is not None
-    assert list(pipeline_obj.first_transformer_in_sequence.target_encoder.inverse_transform([1, 0])) == ['yes', 'no']
+    assert list(
+        pipeline_obj.first_transformer_in_sequence.target_encoder.inverse_transform(
+            [1, 0]
+        )
+    ) == ["yes", "no"]
 
 
 def test_transform_after_fit(data_obj_factory, pipeline_obj):
 
     to_fit_object = data_obj_factory()
     data_obj = data_obj_factory()
 
     _data_object, _terminate = pipeline_obj.run(to_fit_object)
 
     data_object = pipeline_obj.transform(data_obj)
 
-    transform_test_data_to_compare = data_object.get('encode_and_split')['data_test']
+    transform_test_data_to_compare = data_object.get("encode_and_split")["data_test"]
 
     assert len(transform_test_data_to_compare) == 14
 
     for col in transform_test_data_to_compare:
         assert transform_test_data_to_compare[col].dtype != object
 
 
@@ -93,8 +96,7 @@
 
     df = pd.read_csv("test/tennis.csv")
     train_data, test_data = pipeline_obj._train_test_split(df)
 
     assert len(train_data) == 9
     assert len(test_data) == 5
     assert not train_data.equals(test_data)
-
```

### Comparing `primrose-1.0.9/test/test_dill_writer.py` & `primrose-2.0.0/test/test_abstract_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,91 @@
-
 import pytest
-import os
-import dill
-from primrose.configuration.configuration import Configuration
-from primrose.writers.dill_writer import DillWriter
+import logging
+from primrose.node_factory import NodeFactory
+from primrose.base.model import AbstractModel
 from primrose.data_object import DataObject
+from testfixtures import LogCapture
+from primrose.configuration.configuration import Configuration
 from primrose.readers.csv_reader import CsvReader
+import pandas as pd
+
+
+def test_run():
+    class TestModel(AbstractModel):
+        @staticmethod
+        def necessary_config(node_config):
+            return set(["mode"])
+
+        def train_model(self, data_object):
+            logging.info("TRAIN called")
+            return data_object
+
+        def eval_model(self, data_object):
+            logging.info("EVAL called")
+            return data_object
+
+        def predict(self, data_object):
+            logging.info("PREDICT called")
+            return data_object
+
+    NodeFactory().register("TestModel", TestModel)
 
-@pytest.fixture()
-def config():
     config = {
         "implementation_config": {
             "reader_config": {
-                "csv_reader": {
+                "myreader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['recipe_file_writer']
+                    "destinations": ["mymodel"],
                 }
             },
-            "writer_config": {
-                "recipe_file_writer": {
-                    "class": "FileWriter",
-                    "key": "test_data",
-                    "dir": "cache",
-                    "filename": "unittest_file_writer.dill"
-                }
-            }
+            "model_config": {"mymodel": {"class": "TestModel", "mode": "train"}},
         }
     }
-    return config
-
-
-def test_necessary_config(config):
-    configuration = Configuration(None, is_dict_config=True, dict_config=config)
-    writer = DillWriter(configuration, 'recipe_file_writer')
-    node_config = {
-                    "class": "FileWriter",
-                    "key": "test_data",
-                    "dir": "cache",
-                    "filename": "unittest_file_writer.dill"
-                }
-    assert isinstance(writer.necessary_config(node_config), set)
-    assert len(writer.necessary_config(node_config)) > 0
-
-
-def test_init_ok(config):
-
-    test_data_string = "some test data"
-
-    configuration = Configuration(None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     data_object = DataObject(configuration)
 
-    requestor = CsvReader(configuration, 'csv_reader')
+    reader = CsvReader(configuration, "myreader")
+    df = pd.read_csv("test/minimal.csv")
 
-    data_object.add(requestor, test_data_string, 'test_data')
+    data_object.add(reader, df)
 
-    writer = DillWriter(configuration, 'recipe_file_writer')
+    model = TestModel(configuration, "mymodel")
 
-    c = configuration.config_for_instance('recipe_file_writer')
-    filename = c['dir'] + os.path.sep + c['filename']
+    with LogCapture() as l:
+        model.run(data_object)
+    l.check(
+        ("root", "INFO", "TRAIN called"),
+        ("root", "INFO", "EVAL called"),
+        ("root", "INFO", "PREDICT called"),
+    )
 
-    #clean out test file location
-    if os.path.exists(filename):
-        os.remove(filename)
+    config = {
+        "implementation_config": {
+            "reader_config": {
+                "myreader": {
+                    "class": "CsvReader",
+                    "filename": "test/minimal.csv",
+                    "destinations": ["mymodel"],
+                }
+            },
+            "model_config": {"mymodel": {"class": "TestModel", "mode": "eval"}},
+        }
+    }
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
-    data_object, terminate = writer.run(data_object)
+    data_object = DataObject(configuration)
 
-    assert not terminate
+    reader = CsvReader(configuration, "myreader")
 
-    assert os.path.exists(filename)
+    data_object.add(reader, df)
 
-    read_data = dill.load(open(filename, 'rb'))
+    model = TestModel(configuration, "mymodel")
 
-    assert test_data_string == read_data
+    with LogCapture() as l:
+        model.run(data_object)
+    l.check(("root", "INFO", "EVAL called"), ("root", "INFO", "PREDICT called"))
```

### Comparing `primrose-1.0.9/test/test_transformers_strings.py` & `primrose-2.0.0/test/test_transformers_strings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 import pytest
 import pandas as pd
 
 from primrose.transformers.strings import StringTransformer
 
+
 @pytest.fixture
 def dataframe():
-    df = pd.DataFrame({
-        "caps":['TEST!','TEST@'],
-        "splits":['a,b,c','def'],
-        "strips":['aaa,,,,',',,,bbb'],
-        "caps2":['TEST#','TEST$']})
+    df = pd.DataFrame(
+        {
+            "caps": ["TEST!", "TEST@"],
+            "splits": ["a,b,c", "def"],
+            "strips": ["aaa,,,,", ",,,bbb"],
+            "caps2": ["TEST#", "TEST$"],
+        }
+    )
     return df
 
+
 def test_StringTransformer_single_column_str(dataframe):
     df_test = dataframe.copy()
-    df_test['splits'] = df_test['splits'].str.split(',')
-    t = StringTransformer('split','splits',',')
+    df_test["splits"] = df_test["splits"].str.split(",")
+    t = StringTransformer("split", "splits", ",")
     df_out = t.transform(dataframe)
-    pd.testing.assert_frame_equal(df_test,df_out)
+    pd.testing.assert_frame_equal(df_test, df_out)
+
 
 def test_StringTransformer_multiple_column_list(dataframe):
     df_test = dataframe.copy()
-    df_test['caps'] = df_test['caps'].str.lower()
-    df_test['caps2'] = df_test['caps2'].str.lower()
-    t = StringTransformer('lower',['caps','caps2'])
+    df_test["caps"] = df_test["caps"].str.lower()
+    df_test["caps2"] = df_test["caps2"].str.lower()
+    t = StringTransformer("lower", ["caps", "caps2"])
     df_out = t.transform(dataframe)
-    pd.testing.assert_frame_equal(df_test,df_out)
+    pd.testing.assert_frame_equal(df_test, df_out)
+
 
 def test_StringTransformer_kwargs(dataframe):
     df_test = dataframe.copy()
-    df_test['strips'] = df_test['strips'].str.rstrip(to_strip=',')
-    t = StringTransformer('rstrip', ['strips'],to_strip=',')
+    df_test["strips"] = df_test["strips"].str.rstrip(to_strip=",")
+    t = StringTransformer("rstrip", ["strips"], to_strip=",")
     df_out = t.transform(dataframe)
     pd.testing.assert_frame_equal(df_test, df_out)
 
+
 def test__execute_str_method(dataframe):
     df_test = dataframe.copy()
-    test_series = df_test['splits'].str.split(',')
-    t = StringTransformer('split', 'splits', ',')
-    result_series = t._execute_str_method(df_test['splits'])
-    pd.testing.assert_series_equal(result_series,test_series)
+    test_series = df_test["splits"].str.split(",")
+    t = StringTransformer("split", "splits", ",")
+    result_series = t._execute_str_method(df_test["splits"])
+    pd.testing.assert_series_equal(result_series, test_series)
```

### Comparing `primrose-1.0.9/test/test_transformers_imputer.py` & `primrose-2.0.0/test/test_transformers_imputer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,130 @@
-
 import math
 import pytest
 import pandas as pd
 import numpy as np
 
 from primrose.transformers.impute import ColumnSpecificImpute
 
+
 def test_fit():
-    d = {'col1': [1, 2, 3],
-         'col2': [4, 6, 11.2],
-         'col3': [1, 1, 1],
-         'col4': [3, 2, 3],
-         'col5': [1, 2, 3],
-         'col6': [1, 2, 3],
-         'col7': [None, None, None],
-         'col8': np.nan}
+    d = {
+        "col1": [1, 2, 3],
+        "col2": [4, 6, 11.2],
+        "col3": [1, 1, 1],
+        "col4": [3, 2, 3],
+        "col5": [1, 2, 3],
+        "col6": [1, 2, 3],
+        "col7": [None, None, None],
+        "col8": np.nan,
+    }
     df = pd.DataFrame(data=d)
 
-    imputer = ColumnSpecificImpute(columns_to_zero=['col1'],columns_to_mean=['col2'],columns_to_median=['col3'],columns_to_mode=['col4','col7', 'col8'], columns_to_infinity=['col5'],columns_to_neg_infinity=['col6'])
+    imputer = ColumnSpecificImpute(
+        columns_to_zero=["col1"],
+        columns_to_mean=["col2"],
+        columns_to_median=["col3"],
+        columns_to_mode=["col4", "col7", "col8"],
+        columns_to_infinity=["col5"],
+        columns_to_neg_infinity=["col6"],
+    )
 
     imputer.fit(df)
 
     encoder = imputer.encoder
-    assert encoder['col1'] == 0
-    assert math.isclose(encoder['col2'], 21.2/3, abs_tol=0.001)
-    assert encoder['col3'] == 1
-    assert encoder['col4'] == 3
-    assert math.isclose(encoder['col5'], 999999999, abs_tol=0.001)
-    assert math.isclose(encoder['col6'], -999999999, abs_tol=0.001)
-    assert encoder['col7'] == 0
-    assert encoder['col8'] == 0
+    assert encoder["col1"] == 0
+    assert math.isclose(encoder["col2"], 21.2 / 3, abs_tol=0.001)
+    assert encoder["col3"] == 1
+    assert encoder["col4"] == 3
+    assert math.isclose(encoder["col5"], 999999999, abs_tol=0.001)
+    assert math.isclose(encoder["col6"], -999999999, abs_tol=0.001)
+    assert encoder["col7"] == 0
+    assert encoder["col8"] == 0
+
 
 def test_fit2():
-    d = {'col1': [1, 2, 3],
-         'col2': [4, 6, 11.2],
-         'col3': [1, 1, 1],
-         'col4': [3, 2, 3],
-         'col5': [1, 2, 3],
-         'col6': [1, 2, 3]}
+    d = {
+        "col1": [1, 2, 3],
+        "col2": [4, 6, 11.2],
+        "col3": [1, 1, 1],
+        "col4": [3, 2, 3],
+        "col5": [1, 2, 3],
+        "col6": [1, 2, 3],
+    }
     df = pd.DataFrame(data=d)
 
-    imputer = ColumnSpecificImpute(columns_to_zero=['col1'],columns_to_mean=['col2', 'col1'],columns_to_median=['col3'],columns_to_mode=['col4'], columns_to_infinity=['col5'],columns_to_neg_infinity=['col6'])
+    imputer = ColumnSpecificImpute(
+        columns_to_zero=["col1"],
+        columns_to_mean=["col2", "col1"],
+        columns_to_median=["col3"],
+        columns_to_mode=["col4"],
+        columns_to_infinity=["col5"],
+        columns_to_neg_infinity=["col6"],
+    )
 
     with pytest.raises(Exception) as e:
         imputer.fit(df)
     assert "There are columns in multiple lists {'col1'}" in str(e)
 
+
 def test_fit3():
-    d = {'col1': [1, 2, 3],
-         'col2': [4, 6, 11.2],
-         'col3': [1, 1, 1],
-         'col4': [3, 2, 3],
-         'col5': [1, 2, 3],
-         'col6': [1, 2, 3]}
+    d = {
+        "col1": [1, 2, 3],
+        "col2": [4, 6, 11.2],
+        "col3": [1, 1, 1],
+        "col4": [3, 2, 3],
+        "col5": [1, 2, 3],
+        "col6": [1, 2, 3],
+    }
     df = pd.DataFrame(data=d)
 
-    imputer = ColumnSpecificImpute(columns_to_zero=['col1'],columns_to_mean=['JUNK'],columns_to_median=['col3'],columns_to_mode=['col4'], columns_to_infinity=['col5'],columns_to_neg_infinity=['col6'])
+    imputer = ColumnSpecificImpute(
+        columns_to_zero=["col1"],
+        columns_to_mean=["JUNK"],
+        columns_to_median=["col3"],
+        columns_to_mode=["col4"],
+        columns_to_infinity=["col5"],
+        columns_to_neg_infinity=["col6"],
+    )
 
     with pytest.raises(Exception) as e:
         imputer.fit(df)
     assert "Unrecognized impute column 'JUNK'" in str(e)
 
+
 def test_transform():
     df = pd.DataFrame()
-    imputer = ColumnSpecificImpute(columns_to_zero=['col1'],columns_to_mean=['col2'],columns_to_median=['col3'],columns_to_mode=['col4'], columns_to_infinity=['col5'],columns_to_neg_infinity=['col6'])
+    imputer = ColumnSpecificImpute(
+        columns_to_zero=["col1"],
+        columns_to_mean=["col2"],
+        columns_to_median=["col3"],
+        columns_to_mode=["col4"],
+        columns_to_infinity=["col5"],
+        columns_to_neg_infinity=["col6"],
+    )
     with pytest.raises(Exception) as e:
         imputer.transform(df)
-    assert 'ColumnSpecificImpute must train imputations with fit before calling transform' in str(e)
+    assert (
+        "ColumnSpecificImpute must train imputations with fit before calling transform"
+        in str(e)
+    )
+
 
 def test_transform2():
-    d = {'col1': [1, np.nan, 3],
-         'col2': [4, 6, np.nan]}
+    d = {"col1": [1, np.nan, 3], "col2": [4, 6, np.nan]}
     df = pd.DataFrame(data=d)
 
-    imputer = ColumnSpecificImpute(columns_to_zero=['col1'],columns_to_mean=['col2'],columns_to_median=[],columns_to_mode=[], columns_to_infinity=[],columns_to_neg_infinity=[])
+    imputer = ColumnSpecificImpute(
+        columns_to_zero=["col1"],
+        columns_to_mean=["col2"],
+        columns_to_median=[],
+        columns_to_mode=[],
+        columns_to_infinity=[],
+        columns_to_neg_infinity=[],
+    )
 
     imputer.fit(df)
 
     transormed_df = imputer.transform(df)
 
     assert list(transormed_df.col1) == [1, 0, 3]
     assert list(transormed_df.col2) == [4, 6, 5]
-
```

### Comparing `primrose-1.0.9/test/test_simple_switch.py` & `primrose-2.0.0/test/test_simple_switch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-
 import pytest
 from primrose.configuration.configuration import Configuration
 from primrose.conditionalpath.simple_switch import SimpleSwitch
 
+
 def test_destinations_to_prune():
     config = {
         "implementation_config": {
             "reader_config": {
                 "conditional_node": {
                     "class": "SimpleSwitch",
                     "path_to_travel": "left",
-                    "destinations": ['left', 'right']
+                    "destinations": ["left", "right"],
                 }
             },
             "writer_config": {
                 "left": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
+                    "filename": "unittest_similar_recipes.csv",
                 },
                 "right": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
-                }
-            }
+                    "filename": "unittest_similar_recipes.csv",
+                },
+            },
         }
     }
 
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     node = SimpleSwitch(configuration, "conditional_node")
     to_prune = node.destinations_to_prune()
-    assert to_prune == ['right']
+    assert to_prune == ["right"]
```

### Comparing `primrose-1.0.9/test/test_gcs_dill_reader.py` & `primrose-2.0.0/test/test_gcs_dill_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,110 +1,115 @@
-
 import pytest
 from primrose.readers.gcs_dill_reader import GcsDillReader
 from primrose.data_object import DataObject
 from primrose.readers.csv_reader import CsvReader
 from primrose.configuration.configuration import Configuration
 import dill
 import os
 
+
 def test_necessary_config():
     assert len(GcsDillReader.necessary_config({})) == 2
 
+
 def test_run(monkeypatch):
     # returns 2 objects from dill reader
     config = {
         "implementation_config": {
             "reader_config": {
                 "myreader": {
                     "class": "GcsDillReader",
                     "bucket_name": "test1",
                     "blob_name": "test2",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     reader = GcsDillReader(configuration, "myreader")
 
     data_object = DataObject(configuration)
 
     def fake_blobs():
         with open("test/dill_reader_blob1.pkl", "wb") as dill_file:
             dill.dump("some_data", dill_file)
         with open("test/dill_reader_blob2.pkl", "wb") as dill_file:
             dill.dump("some_other_data", dill_file)
         dat1 = open("test/dill_reader_blob1.pkl", "rb").read()
         dat2 = open("test/dill_reader_blob2.pkl", "rb").read()
         return [dat1, dat2]
 
-    monkeypatch.setattr(reader,'download_blobs_as_strings',fake_blobs)
+    monkeypatch.setattr(reader, "download_blobs_as_strings", fake_blobs)
 
     reader_object, terminate = reader.run(data_object)
 
     assert not terminate
 
     assert "myreader" in reader_object.data_dict
 
-    dat = reader_object.data_dict['myreader']
+    dat = reader_object.data_dict["myreader"]
 
     assert "reader_data" in dat
-    datlist = dat['reader_data']
+    datlist = dat["reader_data"]
 
     assert len(datlist) == 2
 
     assert "some_data" in datlist
     assert "some_other_data" in datlist
 
     files = ["test/dill_reader_blob1.pkl", "test/dill_reader_blob2.pkl"]
     for f in files:
         if os.path.exists(f):
             os.remove(f)
 
+
 def test_run2(monkeypatch):
     # returns 1 objects from dill reader
     config = {
         "implementation_config": {
             "reader_config": {
                 "myreader": {
                     "class": "GcsDillReader",
                     "bucket_name": "test1",
                     "blob_name": "test2",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     reader = GcsDillReader(configuration, "myreader")
 
     data_object = DataObject(configuration)
 
     def fake_blobs():
         with open("test/dill_reader_blob1.pkl", "wb") as dill_file:
             dill.dump("some_data", dill_file)
         dat1 = open("test/dill_reader_blob1.pkl", "rb").read()
         return [dat1]
 
-    monkeypatch.setattr(reader,'download_blobs_as_strings',fake_blobs)
+    monkeypatch.setattr(reader, "download_blobs_as_strings", fake_blobs)
 
     reader_object, terminate = reader.run(data_object)
 
     assert not terminate
 
     assert "myreader" in reader_object.data_dict
 
-    dat = reader_object.data_dict['myreader']
+    dat = reader_object.data_dict["myreader"]
 
     assert "reader_data" in dat
-    data = dat['reader_data']
+    data = dat["reader_data"]
 
     assert "some_data" == data
 
     files = ["test/dill_reader_blob1.pkl"]
     for f in files:
         if os.path.exists(f):
             os.remove(f)
-
```

### Comparing `primrose-1.0.9/test/test_serializer.py` & `primrose-2.0.0/test/test_serializer.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,135 +3,146 @@
 import pickle
 import pytest
 from primrose.configuration.configuration import Configuration
 from primrose.data_object import DataObject
 from primrose.readers.csv_reader import CsvReader
 from primrose.writers.serializer import Serializer
 
+
 @pytest.fixture()
 def config():
     config = {
         "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['recipe_file_writer']
+                    "destinations": ["recipe_file_writer"],
                 }
             },
             "writer_config": {
                 "recipe_file_writer": {
                     "class": "Serializer",
                     "key": "test_data",
                     "dir": "cache",
                     "filename": "unittest_file_writer.dill",
-                    "serializer": "dill"
+                    "serializer": "dill",
                 }
-            }
+            },
         }
     }
     return config
 
 
 def test_necessary_config(config):
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
-    writer = Serializer(configuration, 'recipe_file_writer')
+    writer = Serializer(configuration, "recipe_file_writer")
     node_config = {
-                    "class": "Serializer",
-                    "key": "test_data",
-                    "dir": "cache",
-                    "filename": "unittest_file_writer.dill",
-                    "serializer": "dill"
-                }
+        "class": "Serializer",
+        "key": "test_data",
+        "dir": "cache",
+        "filename": "unittest_file_writer.dill",
+        "serializer": "dill",
+    }
     assert isinstance(writer.necessary_config(node_config), set)
     assert len(writer.necessary_config(node_config)) > 0
 
 
 def test_init_dill_ok(config):
 
     test_data_string = "some test data"
 
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     data_object = DataObject(configuration)
 
-    requestor = CsvReader(configuration, 'csv_reader')
+    requestor = CsvReader(configuration, "csv_reader")
 
-    data_object.add(requestor, test_data_string, 'test_data')
+    data_object.add(requestor, test_data_string, "test_data")
 
-    writer = Serializer(configuration, 'recipe_file_writer')
+    writer = Serializer(configuration, "recipe_file_writer")
 
-    c = configuration.config_for_instance('recipe_file_writer')
-    filename = c['dir'] + os.path.sep + c['filename']
+    c = configuration.config_for_instance("recipe_file_writer")
+    filename = c["dir"] + os.path.sep + c["filename"]
 
-    #clean out test file location
+    # clean out test file location
     if os.path.exists(filename):
         os.remove(filename)
 
     data_object, terminate = writer.run(data_object)
 
     assert not terminate
 
     assert os.path.exists(filename)
 
-    read_data = dill.load(open(filename, 'rb'))
+    read_data = dill.load(open(filename, "rb"))
 
     assert test_data_string == read_data
 
+
 def test_init_pickle_ok(config):
-    config["implementation_config"]["writer_config"]["recipe_file_writer"]["filename"] = "unittest_file_writer.pickle"
-    config["implementation_config"]["writer_config"]["recipe_file_writer"]["serializer"] = "pickle"
+    config["implementation_config"]["writer_config"]["recipe_file_writer"][
+        "filename"
+    ] = "unittest_file_writer.pickle"
+    config["implementation_config"]["writer_config"]["recipe_file_writer"][
+        "serializer"
+    ] = "pickle"
 
     test_data_string = "some test data"
 
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     data_object = DataObject(configuration)
 
-    requestor = CsvReader(configuration, 'csv_reader')
+    requestor = CsvReader(configuration, "csv_reader")
 
-    data_object.add(requestor, test_data_string, 'test_data')
+    data_object.add(requestor, test_data_string, "test_data")
 
-    writer = Serializer(configuration, 'recipe_file_writer')
+    writer = Serializer(configuration, "recipe_file_writer")
 
-    c = configuration.config_for_instance('recipe_file_writer')
-    filename = c['dir'] + os.path.sep + c['filename']
+    c = configuration.config_for_instance("recipe_file_writer")
+    filename = c["dir"] + os.path.sep + c["filename"]
 
-    #clean out test file location
+    # clean out test file location
     if os.path.exists(filename):
         os.remove(filename)
 
     data_object, terminate = writer.run(data_object)
 
     assert not terminate
 
     assert os.path.exists(filename)
 
-    read_data = pickle.load(open(filename, 'rb'))
+    read_data = pickle.load(open(filename, "rb"))
 
     assert test_data_string == read_data
 
+
 def test_init_other_ok(config):
-    config["implementation_config"]["writer_config"]["recipe_file_writer"]["filename"] = "unittest_file_writer.other"
-    config["implementation_config"]["writer_config"]["recipe_file_writer"]["serializer"] = "other"
+    config["implementation_config"]["writer_config"]["recipe_file_writer"][
+        "filename"
+    ] = "unittest_file_writer.other"
+    config["implementation_config"]["writer_config"]["recipe_file_writer"][
+        "serializer"
+    ] = "other"
 
     test_data_string = "some test data"
 
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     data_object = DataObject(configuration)
 
-    requestor = CsvReader(configuration, 'csv_reader')
+    requestor = CsvReader(configuration, "csv_reader")
 
-    data_object.add(requestor, test_data_string, 'test_data')
+    data_object.add(requestor, test_data_string, "test_data")
 
-    writer = Serializer(configuration, 'recipe_file_writer')
+    writer = Serializer(configuration, "recipe_file_writer")
 
-    c = configuration.config_for_instance('recipe_file_writer')
-    filename = c['dir'] + os.path.sep + c['filename']
+    c = configuration.config_for_instance("recipe_file_writer")
+    filename = c["dir"] + os.path.sep + c["filename"]
 
-    #clean out test file location
+    # clean out test file location
     if os.path.exists(filename):
         os.remove(filename)
 
     with pytest.raises(Exception, match=r"Unsupported"):
         writer.run(data_object)
```

### Comparing `primrose-1.0.9/test/test_register_module_classes.py` & `primrose-2.0.0/test/test_register_module_classes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,36 @@
-
 import pytest
 from primrose.node_factory import NodeFactory
 from testfixtures import LogCapture
 
 from primrose.readers.csv_reader import CsvReader
 from primrose.writers.dill_writer import DillWriter
 
+
 def test_register_module_classes():
 
     with LogCapture() as l:
         NodeFactory().register_module_classes(__name__)
     l.check(
-        ('root','INFO','Discovered class CsvReader (<class '
-            "'primrose.readers.csv_reader.CsvReader'>)"),
-        ('root',
-            'DEBUG',
-            "Registered CsvReader : <class 'primrose.readers.csv_reader.CsvReader'>"),
-        ('root',
-            'INFO',
-            'Discovered class DillWriter (<class '
-            "'primrose.writers.dill_writer.DillWriter'>)"),
-        ('root',
-            'DEBUG',
-            "Registered DillWriter : <class 'primrose.writers.dill_writer.DillWriter'>")
-    )
+        (
+            "root",
+            "INFO",
+            "Discovered class CsvReader (<class "
+            "'primrose.readers.csv_reader.CsvReader'>)",
+        ),
+        (
+            "root",
+            "DEBUG",
+            "Registered CsvReader : <class 'primrose.readers.csv_reader.CsvReader'>",
+        ),
+        (
+            "root",
+            "INFO",
+            "Discovered class DillWriter (<class "
+            "'primrose.writers.dill_writer.DillWriter'>)",
+        ),
+        (
+            "root",
+            "DEBUG",
+            "Registered DillWriter : <class 'primrose.writers.dill_writer.DillWriter'>",
+        ),
+    )
```

### Comparing `primrose-1.0.9/test/test_logging_success.py` & `primrose-2.0.0/test/test_logging_success.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,47 @@
-
 import pytest
 from primrose.cleanup.logging_success import LoggingSuccess
 from primrose.configuration.configuration import Configuration
 from testfixtures import LogCapture
 from primrose.data_object import DataObject
 
+
 def test_necessary_config():
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['successlogger']
+                    "destinations": ["successlogger"],
                 }
             },
             "cleanup_config": {
                 "successlogger": {
                     "class": "LoggingSuccess",
                     "msg": "woohoo, all done!",
                     "level": "INFO",
                 }
-            }
+            },
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     ls = LoggingSuccess(configuration, "successlogger")
     node_config = {
-                    "class": "LoggingSuccess",
-                    "msg": "woohoo, all done!",
-                    "level": "INFO",
-                }
+        "class": "LoggingSuccess",
+        "msg": "woohoo, all done!",
+        "level": "INFO",
+    }
     assert isinstance(ls.necessary_config(node_config), set)
     assert len(ls.necessary_config(node_config)) == 2
 
     data_object = DataObject(configuration)
 
     assert ls.run(data_object)
 
     with LogCapture() as l:
-        ls.run(data_object) 
-    l.check(('root', 'INFO', 'woohoo, all done!'),)
+        ls.run(data_object)
+    l.check(
+        ("root", "INFO", "woohoo, all done!"),
+    )
```

### Comparing `primrose-1.0.9/test/test_data_object.py` & `primrose-2.0.0/test/test_data_object.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,238 +1,265 @@
-
 import pytest
 import sys
 import os
 from primrose.data_object import DataObject
 from primrose.data_object import DataObjectResponseType
 from primrose.configuration.configuration import Configuration
 from primrose.configuration.util import OperationType
 from primrose.readers.csv_reader import CsvReader
 
+
 @pytest.fixture()
 def setup_vars():
     config = {
         "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['recipe_s3_writer']
+                    "destinations": ["recipe_s3_writer"],
                 }
             },
             "writer_config": {
                 "recipe_s3_writer": {
                     "class": "S3Writer",
                     "dir": "cache",
                     "key": "data",
                     "bucket_name": "does_not_exist_bucket_name",
-                    "bucket_filename": "does_not_exist.csv"
+                    "bucket_filename": "does_not_exist.csv",
                 }
-            }
+            },
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     data_object = DataObject(configuration)
     return configuration, data_object
 
+
 def test_repr(setup_vars):
     configuration, data_object = setup_vars
-    reader = CsvReader(configuration, 'csv_reader')
+    reader = CsvReader(configuration, "csv_reader")
     data_to_save = "TESTING"
     data_object.add(reader, data_to_save)
 
-    assert str(data_object) == "DataObject:defaultdict(<class 'dict'>, {'csv_reader': {'data': 'TESTING'}})"
+    assert (
+        str(data_object)
+        == "DataObject:defaultdict(<class 'dict'>, {'csv_reader': {'data': 'TESTING'}})"
+    )
+
 
 def test_add(setup_vars):
-    '''test value'''
+    """test value"""
     configuration, data_object = setup_vars
-    reader = CsvReader(configuration, 'csv_reader')
+    reader = CsvReader(configuration, "csv_reader")
     data_to_save = "TESTING"
     data_object.add(reader, data_to_save)
 
-    response = data_object.get('csv_reader',rtype=DataObjectResponseType.VALUE.value)
+    response = data_object.get("csv_reader", rtype=DataObjectResponseType.VALUE.value)
     assert response == data_to_save
 
+
 def test_add2(setup_vars):
-    '''test key value'''
+    """test key value"""
     configuration, data_object = setup_vars
-    reader = CsvReader(configuration, 'csv_reader')
+    reader = CsvReader(configuration, "csv_reader")
     data_to_save = "TESTING"
     data_object.add(reader, data_to_save)
 
-    response = data_object.get('csv_reader',rtype=DataObjectResponseType.KEY_VALUE.value)
+    response = data_object.get(
+        "csv_reader", rtype=DataObjectResponseType.KEY_VALUE.value
+    )
     assert isinstance(response, dict)
     assert DataObject.DATA_KEY in response
     assert response[DataObject.DATA_KEY] == data_to_save
 
+
 def test_add3(setup_vars):
-    '''test instance key value'''
+    """test instance key value"""
     configuration, data_object = setup_vars
-    reader = CsvReader(configuration, 'csv_reader')
+    reader = CsvReader(configuration, "csv_reader")
     data_to_save = "TESTING"
     data_object.add(reader, data_to_save)
 
-    response = data_object.get('csv_reader',rtype=DataObjectResponseType.INSTANCE_KEY_VALUE.value)
+    response = data_object.get(
+        "csv_reader", rtype=DataObjectResponseType.INSTANCE_KEY_VALUE.value
+    )
     assert isinstance(response, dict)
-    assert 'csv_reader' in response
+    assert "csv_reader" in response
     assert 1 == len(list(response.keys()))
-    assert response['csv_reader'][DataObject.DATA_KEY] == data_to_save
+    assert response["csv_reader"][DataObject.DATA_KEY] == data_to_save
+
 
 def test_add4(setup_vars):
-    '''test add 2 items'''
+    """test add 2 items"""
     configuration, data_object = setup_vars
-    reader = CsvReader(configuration, 'csv_reader')
+    reader = CsvReader(configuration, "csv_reader")
     data_to_save = "TESTING"
     data_object.add(reader, data_to_save)
 
     data_object.add(reader, data_to_save, overwrite=True)
 
     with pytest.raises(Exception) as e:
         data_object.add(reader, data_to_save, overwrite=False)
     assert "Key already exists for csv_reader" in str(e)
 
+
 def test_get(setup_vars):
     configuration, data_object = setup_vars
-    reader = CsvReader(configuration, 'csv_reader')
+    reader = CsvReader(configuration, "csv_reader")
     data_to_save = "TESTING"
     data_object.add(reader, data_to_save)
 
     with pytest.raises(Exception) as e:
-        data_object.get('reader', rtype='junk')
+        data_object.get("reader", rtype="junk")
     assert "Unrecognized rtype: junk" in str(e)
 
+
 def test_get2(setup_vars):
     configuration, data_object = setup_vars
     with pytest.raises(Exception) as e:
-        data_object.get('junk')
+        data_object.get("junk")
     assert "Key not found: junk" in str(e)
 
+
 def test_get3(setup_vars):
     configuration, data_object = setup_vars
     assert len(data_object.data_dict.keys()) == 0
 
-    reader = CsvReader(configuration, 'csv_reader')
+    reader = CsvReader(configuration, "csv_reader")
     data_to_save = "TESTING"
     data_object.add(reader, data_to_save)
     assert len(data_object.data_dict.keys()) == 1
 
-    data_object.get('csv_reader',pop_data=False)
+    data_object.get("csv_reader", pop_data=False)
     assert len(data_object.data_dict.keys()) == 1
 
-    data_object.get('csv_reader',pop_data=True)
+    data_object.get("csv_reader", pop_data=True)
     assert len(data_object.data_dict.keys()) == 0
 
+
 def test_get4(setup_vars):
     configuration, data_object = setup_vars
-    reader = CsvReader(configuration, 'csv_reader')
-    data_object.add(reader, key='k1', data='v1')
-    data_object.add(reader, key='k2', data='v2')
-    response = data_object.get(reader.instance_name, rtype=DataObjectResponseType.VALUE.value)
+    reader = CsvReader(configuration, "csv_reader")
+    data_object.add(reader, key="k1", data="v1")
+    data_object.add(reader, key="k2", data="v2")
+    response = data_object.get(
+        reader.instance_name, rtype=DataObjectResponseType.VALUE.value
+    )
     assert isinstance(response, dict)
     assert len(response.keys()) == 2
 
+
 def test_upstream_keys(setup_vars):
     configuration, data_object = setup_vars
-    reader = CsvReader(configuration, 'csv_reader')
+    reader = CsvReader(configuration, "csv_reader")
     data_to_save = "TESTING"
     data_object.add(reader, data_to_save)
 
-    keys = data_object.upstream_keys('recipe_s3_writer')
-    assert keys == ['csv_reader']
-
-    keys = data_object.upstream_keys('recipe_s3_writer', operation_type_filter=OperationType.reader)
-    assert keys == ['csv_reader']
+    keys = data_object.upstream_keys("recipe_s3_writer")
+    assert keys == ["csv_reader"]
 
-    keys = data_object.upstream_keys('recipe_s3_writer', operation_type_filter=OperationType.writer)
+    keys = data_object.upstream_keys(
+        "recipe_s3_writer", operation_type_filter=OperationType.reader
+    )
+    assert keys == ["csv_reader"]
+
+    keys = data_object.upstream_keys(
+        "recipe_s3_writer", operation_type_filter=OperationType.writer
+    )
     assert keys == []
 
+
 def test_get_upstream_data(setup_vars):
     configuration, data_object = setup_vars
     with pytest.raises(Exception) as e:
-        data_object.get_upstream_data('recipe_s3_writer')
+        data_object.get_upstream_data("recipe_s3_writer")
     assert "No upstream keys with data found for recipe_s3_writer" in str(e)
 
+
 def test_get_upstream_data2(setup_vars):
     configuration, data_object = setup_vars
-    reader = CsvReader(configuration, 'csv_reader')
+    reader = CsvReader(configuration, "csv_reader")
     data_to_save = "TESTING"
     data_object.add(reader, data_to_save)
-    response = data_object.get_upstream_data('recipe_s3_writer')
+    response = data_object.get_upstream_data("recipe_s3_writer")
     assert isinstance(response, dict)
     assert DataObject.DATA_KEY in response
     assert response[DataObject.DATA_KEY] == data_to_save
 
+
 def test_get_upstream_data3(setup_vars):
     configuration, data_object = setup_vars
-    reader = CsvReader(configuration, 'csv_reader')
+    reader = CsvReader(configuration, "csv_reader")
     data_to_save = "TESTING"
     data_object.add(reader, data_to_save)
-    response = data_object.get_upstream_data('recipe_s3_writer')
+    response = data_object.get_upstream_data("recipe_s3_writer")
     assert isinstance(response, dict)
     assert DataObject.DATA_KEY in response
     assert response[DataObject.DATA_KEY] == data_to_save
 
+
 def test_get_upstream_data4():
     config = {
         "implementation_config": {
             "reader_config": {
                 "csv_reader1": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['recipe_s3_writer']
+                    "destinations": ["recipe_s3_writer"],
                 },
-
                 "csv_reader2": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['recipe_s3_writer']
-                }
+                    "destinations": ["recipe_s3_writer"],
+                },
             },
             "writer_config": {
                 "recipe_s3_writer": {
                     "class": "S3Writer",
                     "dir": "cache",
                     "key": "data",
                     "bucket_name": "does_not_exist_bucket_name",
-                    "bucket_filename": "does_not_exist.csv"
+                    "bucket_filename": "does_not_exist.csv",
                 }
-            }
+            },
         }
     }
 
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     data_object = DataObject(configuration)
 
-    reader1 = CsvReader(configuration, 'csv_reader1')
-    reader2 = CsvReader(configuration, 'csv_reader2')
+    reader1 = CsvReader(configuration, "csv_reader1")
+    reader2 = CsvReader(configuration, "csv_reader2")
 
     data_object.add(reader1, "data1")
     data_object.add(reader2, "data2")
 
-    response = data_object.get_upstream_data('recipe_s3_writer')
+    response = data_object.get_upstream_data("recipe_s3_writer")
     assert isinstance(response, dict)
-    assert 'csv_reader1' in response
-    assert 'csv_reader2' in response
-    assert response['csv_reader1'][DataObject.DATA_KEY] == "data1"
-    assert response['csv_reader2'][DataObject.DATA_KEY] == "data2"
+    assert "csv_reader1" in response
+    assert "csv_reader2" in response
+    assert response["csv_reader1"][DataObject.DATA_KEY] == "data1"
+    assert response["csv_reader2"][DataObject.DATA_KEY] == "data2"
 
-    response = data_object.get_upstream_data('recipe_s3_writer')
+    response = data_object.get_upstream_data("recipe_s3_writer")
     assert isinstance(response, dict)
-    assert response['csv_reader1'][DataObject.DATA_KEY] == "data1"
-    assert response['csv_reader2'][DataObject.DATA_KEY] == "data2"
+    assert response["csv_reader1"][DataObject.DATA_KEY] == "data1"
+    assert response["csv_reader2"][DataObject.DATA_KEY] == "data2"
+
 
 def test_caching():
     config = {
         "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     data_object = DataObject(configuration)
 
@@ -248,93 +275,97 @@
 
     assert os.path.exists(filename)
 
     restored_data_object = DataObject.read_from_cache(filename)
 
     assert isinstance(restored_data_object, DataObject)
 
-    assert restored_data_object.get("csv_reader", rtype=DataObjectResponseType.VALUE.value) == "some_data"
+    assert (
+        restored_data_object.get("csv_reader", rtype=DataObjectResponseType.VALUE.value)
+        == "some_data"
+    )
 
     if os.path.exists(filename):
         os.remove(filename)
 
+
 def test_get_filtered_upstream_data():
     config = {
         "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['recipe_s3_writer']
+                    "destinations": ["recipe_s3_writer"],
                 }
             },
             "writer_config": {
                 "recipe_s3_writer": {
                     "class": "S3Writer",
                     "dir": "cache",
                     "key": "data",
                     "bucket_name": "does_not_exist_bucket_name",
-                    "bucket_filename": "does_not_exist.csv"
+                    "bucket_filename": "does_not_exist.csv",
                 }
-            }
+            },
         }
     }
 
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     data_object = DataObject(configuration)
 
-    reader = CsvReader(configuration, 'csv_reader')
+    reader = CsvReader(configuration, "csv_reader")
 
     data_object.add(reader, "some_data_to_save")
 
     data = data_object.get_filtered_upstream_data("recipe_s3_writer", "data")
-    assert data == {'data': 'some_data_to_save'}
+    assert data == {"data": "some_data_to_save"}
     assert not isinstance(data, list)
 
     data = data_object.get_filtered_upstream_data("recipe_s3_writer", "JUNK")
     assert not data
 
 
 def test_get_filtered_multiple_upstream_data():
     config = {
         "implementation_config": {
             "reader_config": {
                 "csv_reader1": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['recipe_s3_writer']
+                    "destinations": ["recipe_s3_writer"],
                 },
                 "csv_reader2": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['recipe_s3_writer']
-                }
+                    "destinations": ["recipe_s3_writer"],
+                },
             },
             "writer_config": {
                 "recipe_s3_writer": {
                     "class": "S3Writer",
                     "dir": "cache",
                     "key": "data",
                     "bucket_name": "does_not_exist_bucket_name",
-                    "bucket_filename": "does_not_exist.csv"
+                    "bucket_filename": "does_not_exist.csv",
                 }
-            }
+            },
         }
     }
 
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     data_object = DataObject(configuration)
 
-    reader1 = CsvReader(configuration, 'csv_reader1')
-    reader2 = CsvReader(configuration, 'csv_reader2')
+    reader1 = CsvReader(configuration, "csv_reader1")
+    reader2 = CsvReader(configuration, "csv_reader2")
 
     data_object.add(reader1, "some_data_to_save")
     data_object.add(reader2, "some_data_to_save")
 
     data = data_object.get_filtered_upstream_data("recipe_s3_writer", "data")
-    assert data == [{'data': 'some_data_to_save'}, {'data': 'some_data_to_save'}]
+    assert data == [{"data": "some_data_to_save"}, {"data": "some_data_to_save"}]
     assert isinstance(data, list)
 
     data = data_object.get_filtered_upstream_data("recipe_s3_writer", "JUNK")
-    assert not data
+    assert not data
```

### Comparing `primrose-1.0.9/test/test_transformer_sequence.py` & `primrose-2.0.0/test/test_transformer_sequence.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,43 @@
-
 import pytest
 from primrose.base.transformer_sequence import TransformerSequence
 from primrose.base.transformer import AbstractTransformer
 
+
 @pytest.fixture
 def transformer_class():
     class TestTransformer(AbstractTransformer):
         def fit(self, data):
             return data
+
         def transform(self, data):
             return data
+
     return TestTransformer()
 
+
 def test_init(transformer_class):
     t1 = transformer_class
     t2 = transformer_class
     ts = TransformerSequence([t1, t2])
     array = list(ts.transformers())
     assert len(array) == 2
     assert array[0] == t1
 
+
 def test_add(transformer_class):
     ts = TransformerSequence()
     assert len(ts.sequence) == 0
     t = transformer_class
     ts.add(t)
     assert len(ts.sequence) == 1
-    
+
     with pytest.raises(Exception) as e:
         ts.add(0)
-    assert 'Transformer needs to extend AbstractTransformer' in str(e)
+    assert "Transformer needs to extend AbstractTransformer" in str(e)
 
     ts.add(transformer_class)
     ts.add(transformer_class)
 
     array = list(ts.transformers())
     assert len(array) == 3
-    assert array[0] == t
+    assert array[0] == t
```

### Comparing `primrose-1.0.9/test/test_configuration.py` & `primrose-2.0.0/test/test_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,411 +2,454 @@
 import sys
 import os
 import json
 from primrose.configuration.configuration import Configuration
 from primrose.writers.abstract_file_writer import AbstractFileWriter
 from primrose.node_factory import NodeFactory
 
+
+@pytest.fixture
+def mock_env(monkeypatch):
+    monkeypatch.setenv("PRIMROSE_EXT_NODE_PACKAGE", "test")
+
+
 def test_init_error0():
     config = {}
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    assert 'Did not find required top-level key implementation_config' in str(e)
+    assert "Did not find required top-level key implementation_config" in str(e)
+
 
 def test_init_error1():
     with pytest.raises(Exception) as e:
         Configuration(None)
     if sys.version_info[:2] == (3, 5):
         assert "stat: can't specify None for path argument" in str(e)
     else:
-        assert 'stat: path should be string, bytes, os.PathLike or integer, not NoneType' in str(e)
+        assert (
+            "stat: path should be string, bytes, os.PathLike or integer, not NoneType"
+            in str(e)
+        )
+
 
 def test_init_error2():
     with pytest.raises(Exception) as e:
         Configuration(config_location="junky_path_does_not_exist")
-    assert 'config file at: junky_path_does_not_exist not found' in str(e)
+    assert "config file at: junky_path_does_not_exist not found" in str(e)
+
 
 def test_init_error3():
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config=None)
-    assert 'expected dict_config was None' in str(e)
+    assert "expected dict_config was None" in str(e)
+
 
 def test_init_error4():
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config="1234")
-    assert 'did not receive expected dict_config' in str(e)
+    assert "did not receive expected dict_config" in str(e)
+
 
 def test_init_error5():
-    config = {  
-        "implementation_config": {
-            "k1": {"a":1},
-            "k2": {"a":2}
-        }
-    }
+    config = {"implementation_config": {"k1": {"a": 1}, "k2": {"a": 2}}}
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    assert 'Operations must all have unique names in the configuration' in str(e)
+    assert "Operations must all have unique names in the configuration" in str(e)
+
 
 def test_init_error6():
     with pytest.raises(Exception) as e:
         filename = "test/test_dupe_toplevel.json"
         Configuration(config_location=filename, is_dict_config=False, dict_config=None)
     assert "duplicate key: 'model_config'" in str(e)
 
+
 def test_init_error7():
-    config = {  
-        "junk": {}
-    }
+    config = {"junk": {}}
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    assert 'Unsupported top-level key: junk. Supported keys are [\'metadata\', \'implementation_config\']' in str(e)
+    assert (
+        "Unsupported top-level key: junk. Supported keys are ['metadata', 'implementation_config']"
+        in str(e)
+    )
+
 
 def test_init_error8():
     with pytest.raises(ValueError) as e:
-        Configuration('test/tennis.csv')
-    assert 'config file at: test/tennis.csv has improper extension type - please use a .json or .yml file' in str(e)
+        Configuration("test/tennis.csv")
+    assert (
+        "config file at: test/tennis.csv has improper extension type - please use a .json or .yml file"
+        in str(e)
+    )
+
 
 def test_metadata():
-    config = {
-        "metadata":{"k":"v"},
-        "implementation_config":{}
-    }
+    config = {"metadata": {"k": "v"}, "implementation_config": {}}
     c = Configuration(config_location=None, is_dict_config=True, dict_config=config)
     assert c.config_metadata["k"] == "v"
 
+
 def test_init_ok():
-    config = {"implementation_config":{}}
+    config = {"implementation_config": {}}
     c = Configuration(config_location=None, is_dict_config=True, dict_config=config)
     assert c.config_string
     assert c.config_hash
 
+
 def test_init_ok2():
     config = {
-        "metadata": {
-            "traverser": "DepthFirstTraverser"
-        },
+        "metadata": {"traverser": "DepthFirstTraverser"},
         "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "some/path/to/file",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
-        }
+        },
     }
     c = Configuration(config_location=None, is_dict_config=True, dict_config=config)
     assert c.config_string
-    assert c.config_hash == 'b434870806fe0c61ddf2b417ae62c1be519b069fb6e12572f4ff8143f98086ff'
+    assert (
+        c.config_hash
+        == "b434870806fe0c61ddf2b417ae62c1be519b069fb6e12572f4ff8143f98086ff"
+    )
+
 
 def test_unrecognized():
     config = {
         "implementation_config": {
             "junky_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "some/path/to/file",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    assert 'Unspported operation: junky_config' in str(e)
+    assert "Unspported operation: junky_config" in str(e)
+
 
 def test_nopipelinekey():
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "pipeline_config": {
-                "corpus_pipeline": {
-                    "destinations": ["recipe_name_model"]
-                }
+                "corpus_pipeline": {"destinations": ["recipe_name_model"]}
             }
         }
     }
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    assert 'No class key found in pipeline_config.corpus_pipeline' in str(e)
+    assert "No class key found in pipeline_config.corpus_pipeline" in str(e)
+
 
 def test_metadata2():
-    config = {
-        "metadata": {
-            "traverser": "doesnotexist"
-        },
-        "implementation_config":{
-        }
-    }
+    config = {"metadata": {"traverser": "doesnotexist"}, "implementation_config": {}}
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    assert 'doesnotexist is not a valid and/or registered Traverser' in str(e)
+    assert "doesnotexist is not a valid and/or registered Traverser" in str(e)
+
 
 def test_check_metadata():
     config = {
-        "metadata": {
-            "data_object": {
-                "read_from_cache": True
-            }
-        },
-        "implementation_config":{
-        }
+        "metadata": {"data_object": {"read_from_cache": True}},
+        "implementation_config": {},
     }
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    assert "metadata.data_object: if read_from_cache==true, you must set 'read_filename'" in str(e)
+    assert (
+        "metadata.data_object: if read_from_cache==true, you must set 'read_filename'"
+        in str(e)
+    )
+
 
 def test_check_metadata2():
     config = {
         "metadata": {
             "data_object": {
                 "read_from_cache": True,
-                "read_filename": "path/does/not/exist"
+                "read_filename": "path/does/not/exist",
             }
         },
-        "implementation_config":{
-        }
+        "implementation_config": {},
     }
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config=config)
     assert "Invalid metadata.data_object.read_filename: path/does/not/exist" in str(e)
 
+
 def test_check_metadata3():
     config = {
-        "metadata": {
-            "data_object": {
-                "write_to_cache": True
-            }
-        },
-        "implementation_config":{
-        }
+        "metadata": {"data_object": {"write_to_cache": True}},
+        "implementation_config": {},
     }
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    assert "metadata.data_object: if write_to_cache==true, you must set 'write_filename'" in str(e)
+    assert (
+        "metadata.data_object: if write_to_cache==true, you must set 'write_filename'"
+        in str(e)
+    )
+
 
 def test_check_setions():
     config = {
-        "metadata": {
-            "section_registry": [
-                "phase_1"
-            ]
-        },
+        "metadata": {"section_registry": ["phase_1"]},
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
-        }
+        },
     }
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    assert "Following sections from metadata were not found implementation: {'phase_1'}" in str(e)
+    assert (
+        "Following sections from metadata were not found implementation: {'phase_1'}"
+        in str(e)
+    )
+
 
 def test_check_setions2():
     config = {
-        "metadata": {
-            "section_registry": [
-                "reader_config"
-            ]
-        },
+        "metadata": {"section_registry": ["reader_config"]},
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             },
-            "writer_config": {}
-        }
+            "writer_config": {},
+        },
     }
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    assert "Following sections from implementation were not found in metadata: {'writer_config'}" in str(e)
+    assert (
+        "Following sections from implementation were not found in metadata: {'writer_config'}"
+        in str(e)
+    )
+
 
 def test_check_setions3():
     config = {
-        "metadata": {
-            "section_registry": [
-                "reader_config",
-                "writer_config"
-            ]
-        },
+        "metadata": {"section_registry": ["reader_config", "writer_config"]},
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             },
-            "writer_config": {}
-        }
+            "writer_config": {},
+        },
     }
     # this should not raise an exception
     Configuration(config_location=None, is_dict_config=True, dict_config=config)
 
+
 def test_check_setions4():
     config = {
-        "metadata": {
-            "section_registry": [
-                "phase1",
-                "phase2"
-            ]
-        },
+        "metadata": {"section_registry": ["phase1", "phase2"]},
         "implementation_config": {
             "phase1": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             },
-            "phase2": {}
-        }
+            "phase2": {},
+        },
     }
     # this should not raise an exception
     Configuration(config_location=None, is_dict_config=True, dict_config=config)
 
+
 def test_sections_in_order1():
     config = {
-        "metadata": {
-            "section_registry": [
-                "phase1",
-                "phase2"
-            ]
-        },
+        "metadata": {"section_registry": ["phase1", "phase2"]},
         "implementation_config": {
             "phase1": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             },
-            "phase2": {}
-        }
+            "phase2": {},
+        },
     }
-    config = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    config = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     sections, source = config.sections_in_order()
     assert sections == ["phase1", "phase2"]
     assert source == "section_registry"
 
+
 def test_sections_in_order2():
     config = {
-        "metadata": {
-        },
+        "metadata": {},
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             },
-            "writer_config": {
-
-            }
-        }
+            "writer_config": {},
+        },
     }
-    config = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    config = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     sections, source = config.sections_in_order()
     assert sections == ["reader_config", "writer_config"]
-    assert source == 'default'
+    assert source == "default"
+
 
 def test_sections_in_order3():
     config = {
-        "metadata": {
-            "section_run": [
-                "writer_config"
-            ]
-        },
+        "metadata": {"section_run": ["writer_config"]},
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["recipe_csv_writer"]
+                    "destinations": ["recipe_csv_writer"],
                 }
             },
             "writer_config": {
                 "recipe_csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
+                    "filename": "unittest_similar_recipes.csv",
                 }
-            }
-        }
+            },
+        },
     }
-    config = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    config = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     sections, source = config.sections_in_order()
     assert sections == ["writer_config"]
     assert source == "section_run"
 
+
 def test_registration():
     class TestWriterUnreg(AbstractFileWriter):
         def __init__(self, configuration, instance_name):
             pass
+
         def write(self, data_dict):
             pass
-    
+
     config = {
         "implementation_config": {
             "reader_config": {
-                "read_data": {
-                    "class": "TestWriterUnreg",
-                    "destinations": []
-                }
+                "read_data": {"class": "TestWriterUnreg", "destinations": []}
             }
         }
     }
     with pytest.raises(Exception) as e:
         Configuration(config_location=None, is_dict_config=True, dict_config=config)
-    assert 'Cannot register node class TestWriterUnreg' in str(e)
+    assert "Cannot register node class TestWriterUnreg" in str(e)
 
 
 def test_comments_in_json():
     # should not raise exception even though there are comments in the JSON
     config = Configuration(config_location="test/config_with_comments.json")
-    assert list(config.config.keys()) == ['reader_config', 'writer_config']
-    assert config.config['reader_config']['read_data']['class'] == 'CsvReader'
-    assert list(config.config['reader_config']['read_data']['destinations']) == ['write_output']
-    #"{'reader_config': {'read_data': {'class': 'CsvReader', 'filename': 'data/tennis.csv', 'destinations': ['write_output']}}, 'writer_config': {'write_output': {'class': 'CsvWriter', 'key': 'data', 'dir': 'cache', 'filename': 'tennis_output.csv'}}}"
+    assert list(config.config.keys()) == ["reader_config", "writer_config"]
+    assert config.config["reader_config"]["read_data"]["class"] == "CsvReader"
+    assert list(config.config["reader_config"]["read_data"]["destinations"]) == [
+        "write_output"
+    ]
+    # "{'reader_config': {'read_data': {'class': 'CsvReader', 'filename': 'data/tennis.csv', 'destinations': ['write_output']}}, 'writer_config': {'write_output': {'class': 'CsvWriter', 'key': 'data', 'dir': 'cache', 'filename': 'tennis_output.csv'}}}"
 
 
 def test_perform_any_config_fragment_substitution_bad():
     config_str = """
     {
         {% include "does/not/exist" %}
         "implementation_config": {
         }
     }
     """
     with pytest.raises(Exception) as e:
         Configuration.perform_any_config_fragment_substitution(config_str)
-    assert 'Substitution files do not exist: does/not/exist' in str(e)
+    assert "Substitution files do not exist: does/not/exist" in str(e)
+
+
+def test_perform_any_config_fragment_substitution_default():
+    config_str = """
+    {
+        {% include "test/metadata_fragment.json" %}
+        "implementation_config": {
+            {% include "test/read_write_fragment.json" %}
+        }
+    }
+    """
+    final_str = Configuration.perform_any_config_fragment_substitution(config_str)
+    expected = """
+    {
+        "metadata":{
+            "test": "default"
+        },
+        "implementation_config": {
 
+        "reader_config": {
+            "read_data": {
+                "class": "CsvReader",
+                "filename": "data/tennis.csv",
+                "destinations": [
+                    "write_output"
+                ]
+            }
+        },
+        "writer_config": {
+            "write_output": {
+                "class": "CsvWriter",
+                "key": "data",
+                "dir": "cache",
+                "filename": "tennis_output.csv"
+            }
+        }
 
-def test_perform_any_config_fragment_substitution():
+        }
+    }
+    """
+    assert json.loads(final_str) == json.loads(expected)
+
+def test_perform_any_config_fragment_substitution_env_var(monkeypatch):
+    monkeypatch.setenv("TEST","foo")
     config_str = """
     {
         {% include "test/metadata_fragment.json" %}
         "implementation_config": {
             {% include "test/read_write_fragment.json" %}
         }
     }
     """
     final_str = Configuration.perform_any_config_fragment_substitution(config_str)
     expected = """
     {
-        "metadata":{},
+        "metadata":{
+            "test": "foo"
+        },
         "implementation_config": {
 
         "reader_config": {
             "read_data": {
                 "class": "CsvReader",
                 "filename": "data/tennis.csv",
                 "destinations": [
@@ -418,39 +461,69 @@
             "write_output": {
                 "class": "CsvWriter",
                 "key": "data",
                 "dir": "cache",
                 "filename": "tennis_output.csv"
             }
         }
-        
+
         }
     }
     """
     assert json.loads(final_str) == json.loads(expected)
 
 def test_yaml_config1():
-    config_yaml = Configuration(config_location='test/hello_world_tennis.yml')
-    config_json = Configuration(config_location='test/hello_world_tennis.json')
+    config_yaml = Configuration(config_location="test/hello_world_tennis.yml")
+    config_json = Configuration(config_location="test/hello_world_tennis.json")
     assert config_yaml.config_hash == config_json.config_hash
 
+
 def test_yaml_config2():
-    c = Configuration('test/config_substitution.yml')
+    c = Configuration("test/config_substitution.yml")
     assert c.config_string
     assert c.config_hash
 
-def test_yaml_perform_any_config_fragment_substitution():
+
+def test_yaml_perform_any_config_fragment_substitution_default():
+    config_str = """
+{% include "test/metadata_fragment.yml" %}
+implementation_config:
+{% include "test/read_write_fragment.yml" %}
+    """
+    final_str = Configuration.perform_any_config_fragment_substitution(config_str)
+    expected = """
+metadata:
+  test: default
+implementation_config:
+  reader_config:
+    read_data:
+      class: CsvReader
+      destinations:
+      - write_output
+      filename: data/tennis.csv
+  writer_config:
+    write_output:
+      class: CsvWriter
+      dir: cache
+      filename: tennis_output.csv
+      key: data
+    """
+    assert final_str == expected
+
+def test_yaml_perform_any_config_fragment_substitution_env_var(monkeypatch):
+    monkeypatch.setenv("TEST","foo")
     config_str = """
 {% include "test/metadata_fragment.yml" %}
 implementation_config:
 {% include "test/read_write_fragment.yml" %}
     """
     final_str = Configuration.perform_any_config_fragment_substitution(config_str)
     expected = """
-metadata: {}
+metadata:
+  test: foo
 implementation_config:
   reader_config:
     read_data:
       class: CsvReader
       destinations:
       - write_output
       filename: data/tennis.csv
@@ -459,143 +532,121 @@
       class: CsvWriter
       dir: cache
       filename: tennis_output.csv
       key: data
     """
     assert final_str == expected
 
-def test_class_prefix():
+
+def test_class_prefix(mock_env):
     config_path = {
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "TestExtNode",
                     "class_prefix": "test/ext_node_example.py",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
     config_dot = {
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "TestExtNode",
                     "class_prefix": "test.ext_node_example",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
     for config in [config_path, config_dot]:
-        config = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+        config = Configuration(
+            config_location=None, is_dict_config=True, dict_config=config
+        )
         assert config.config_string
         assert config.config_hash
-        NodeFactory().unregister('TestExtNode')
-        
+        NodeFactory().unregister("TestExtNode")
+
 
-def test_class_package():
+def test_class_package(mock_env):
     config_path = {
-        "metadata": {
-            "class_package": "test"
-        },
+        "metadata": {"class_package": "test"},
         "implementation_config": {
-            "reader_config": {
-                "read_data": {
-                    "class": "TestExtNode",
-                    "destinations": []
-                }
-            }
-        }
+            "reader_config": {"read_data": {"class": "TestExtNode", "destinations": []}}
+        },
     }
     config_full_path = {
-        "metadata": {
-            "class_package": "test/ext_node_example.py"
-        },
+        "metadata": {"class_package": "test/ext_node_example.py"},
         "implementation_config": {
-            "reader_config": {
-                "read_data": {
-                    "class": "TestExtNode",
-                    "destinations": []
-                }
-            }
-        }
+            "reader_config": {"read_data": {"class": "TestExtNode", "destinations": []}}
+        },
     }
     config_full_dot = {
-        "metadata": {
-            "class_package": "test"
-        },
+        "metadata": {"class_package": "test"},
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "TestExtNode",
                     "class_prefix": "ext_node_example",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
-        }
+        },
     }
     for config in [config_full_path, config_path, config_full_dot]:
-        config = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+        config = Configuration(
+            config_location=None, is_dict_config=True, dict_config=config
+        )
         assert config.config_string
         assert config.config_hash
-        NodeFactory().unregister('TestExtNode')
+        NodeFactory().unregister("TestExtNode")
 
 
-def test_env_override_class_package():
+def test_env_override_class_package(mock_env):
     config = {
-        "metadata": {
-            "class_package": "junk"
-        },
+        "metadata": {"class_package": "junk"},
         "implementation_config": {
-            "reader_config": {
-                "read_data": {
-                    "class": "TestExtNode",
-                    "destinations": []
-                }
-            }
-        }
+            "reader_config": {"read_data": {"class": "TestExtNode", "destinations": []}}
+        },
     }
-    os.environ['PRIMROSE_EXT_NODE_PACKAGE'] = 'test'
-    config = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    config = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     assert config.config_string
     assert config.config_hash
-    NodeFactory().unregister('TestExtNode')
-    os.environ.pop('PRIMROSE_EXT_NODE_PACKAGE')
+    NodeFactory().unregister("TestExtNode")
 
 
 def test_incorrect_class_package():
     config = {
-        "metadata": {
-            "class_package": "junk"
-        },
+        "metadata": {"class_package": "junk"},
         "implementation_config": {
-            "reader_config": {
-                "read_data": {
-                    "class": "TestExtNode",
-                    "destinations": []
-                }
-            }
-        }
+            "reader_config": {"read_data": {"class": "TestExtNode", "destinations": []}}
+        },
     }
     with pytest.raises(Exception) as e:
-        config = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+        config = Configuration(
+            config_location=None, is_dict_config=True, dict_config=config
+        )
     assert "Cannot register node class TestExtNode" in str(e)
 
+
 def test_incorrect_class_package2():
     config = {
-        "metadata": {
-            "class_package": "test"
-        },
+        "metadata": {"class_package": "test"},
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "TestExtNode",
                     "class_prefix": "junk",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
-        }
+        },
     }
     with pytest.raises(Exception) as e:
-        config = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+        config = Configuration(
+            config_location=None, is_dict_config=True, dict_config=config
+        )
     assert "Cannot register node class TestExtNode" in str(e)
```

### Comparing `primrose-1.0.9/test/test_sklearn_preprocessing_pipeline.py` & `primrose-2.0.0/test/test_sklearn_preprocessing_pipeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 import pytest
 
-from primrose.pipelines.sklearn_preprocessing_pipeline import SklearnPreprocessingPipeline
-from primrose.transformers.sklearn_preprocessing_transformer import SklearnPreprocessingTransformer
+from primrose.pipelines.sklearn_preprocessing_pipeline import (
+    SklearnPreprocessingPipeline,
+)
+from primrose.transformers.sklearn_preprocessing_transformer import (
+    SklearnPreprocessingTransformer,
+)
+
 
 def test__instantiate_preprocessor():
-    processor = SklearnPreprocessingPipeline._instantiate_preprocessor("preprocessing.StandardScaler", args=None)
+    processor = SklearnPreprocessingPipeline._instantiate_preprocessor(
+        "preprocessing.StandardScaler", args=None
+    )
     assert isinstance(processor, SklearnPreprocessingTransformer)
 
     with pytest.raises(Exception) as e:
-        SklearnPreprocessingPipeline._instantiate_preprocessor("preprocessing.junk", args=None)
+        SklearnPreprocessingPipeline._instantiate_preprocessor(
+            "preprocessing.junk", args=None
+        )
     assert "Preprocessor junk not found in preprocessing module" in str(e)
-
```

### Comparing `primrose-1.0.9/test/test_mysql_helper.py` & `primrose-2.0.0/test/test_mysql_helper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-
 import pytest
 import os
 from primrose.readers.mysql_helper import MySQLHelper
 
+
 def test_extract_mongo_credentials():
-    keys=["MYSQL_HOST",
-            "MYSQL_PORT",
-            "MYSQL_DB",
-            "MYSQL_USER",
-            "MYSQL_PASS"]
+    keys = ["MYSQL_HOST", "MYSQL_PORT", "MYSQL_DB", "MYSQL_USER", "MYSQL_PASS"]
     for k in keys:
         if k in os.environ:
             del os.environ[k]
 
     with pytest.raises(Exception) as e:
         MySQLHelper.extract_mysql_credentials()
-    assert 'Did not find env variable for MYSQL_HOST' in str(e)
+    assert "Did not find env variable for MYSQL_HOST" in str(e)
+
 
 def test_extract_mongo_credentials2():
-    keys=["MYSQL_HOST",
-            "MYSQL_PORT",
-            "MYSQL_DB",
-            "MYSQL_USER",
-            "MYSQL_PASS"]
-    for i,k in enumerate(keys):
+    keys = ["MYSQL_HOST", "MYSQL_PORT", "MYSQL_DB", "MYSQL_USER", "MYSQL_PASS"]
+    for i, k in enumerate(keys):
         os.environ[k] = str(i)
 
     host, port, username, password, database = MySQLHelper.extract_mysql_credentials()
     assert host == "0"
     assert port == 1
     assert username == "3"
     assert password == "4"
-    assert database == "2" 
+    assert database == "2"
```

### Comparing `primrose-1.0.9/test/test_abstract_search_engine.py` & `primrose-2.0.0/test/test_abstract_search_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,94 +5,106 @@
 from primrose.configuration.configuration import Configuration
 from primrose.base.search_engine import AbstractSearchEngine
 from primrose.base.node import AbstractNode
 from nltk import ngrams
 from primrose.node_factory import NodeFactory
 from primrose.data_object import DataObject, DataObjectResponseType
 
-'''we can't instatiate AbstractSearchEngine but this will test some of the methods'''
+"""we can't instatiate AbstractSearchEngine but this will test some of the methods"""
 
-def test_cosine_similarity_matrix():
 
+def test_cosine_similarity_matrix():
     class Testpipeline(AbstractNode):
         def __init__(self, configuration, instance_name):
             self.configuration = configuration
             self.instance_name = instance_name
+
         @staticmethod
         def necessary_config(node_config):
             return set([])
+
         def run(self, data_object):
             return data_object, False
+
     NodeFactory().register("Testpipeline", Testpipeline)
 
     class TestSimpleSearchEngine(AbstractSearchEngine):
-        '''
-            simple TFIDF search engine
-        '''
+        """
+        simple TFIDF search engine
+        """
 
         def __init__(self, configuration, instance_name):
             AbstractSearchEngine.__init__(self, configuration, instance_name)
 
         def tokenize(self, s, stopwords=[], add_ngrams=True):
             q = s.lower()
-            tokens = q.replace("-", " ").replace(",", "").replace("(", "").replace(")", "").split(" ")
+            tokens = (
+                q.replace("-", " ")
+                .replace(",", "")
+                .replace("(", "")
+                .replace(")", "")
+                .split(" ")
+            )
             tokens = [w for w in tokens if w not in stopwords]
             if add_ngrams:
                 bigrams = list(ngrams(tokens, 2))
                 strbigrams = ["_".join(t) for t in bigrams]
                 tokens.extend(strbigrams)
             return tokens
 
-        def eval_model(data_object): return data_object
+        def eval_model(data_object):
+            return data_object
 
     NodeFactory().register("TestSimpleSearchEngine", TestSimpleSearchEngine)
 
     config = {
-          "implementation_config":{
+        "implementation_config": {
             "pipeline_config": {
                 "pipeline1": {
                     "class": "Testpipeline",
-                    "destinations": ["recipe_name_model"]
+                    "destinations": ["recipe_name_model"],
                 }
             },
             "model_config": {
                 "recipe_name_model": {
                     "class": "TestSimpleSearchEngine",
                     "id_key": "id",
                     "doc_key": "name",
                     "mode": "precict",
-                    "destinations": []
+                    "destinations": [],
                 }
-            }
+            },
         }
     }
 
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
-    #set that pipeline provided the corpus
-    corpus = [{"id":1,"name":"spinach omelet"},
-        {"id":2,"name":"kale omelet"},
-        {"id":3,"name":"cherry pie"}]
+    # set that pipeline provided the corpus
+    corpus = [
+        {"id": 1, "name": "spinach omelet"},
+        {"id": 2, "name": "kale omelet"},
+        {"id": 3, "name": "cherry pie"},
+    ]
     data_object = DataObject(configuration)
-    pipeline = Testpipeline(configuration, 'pipeline1')
+    pipeline = Testpipeline(configuration, "pipeline1")
     data_object.add(pipeline, pd.DataFrame(corpus))
 
-    engine = TestSimpleSearchEngine(configuration, 'recipe_name_model')
+    engine = TestSimpleSearchEngine(configuration, "recipe_name_model")
     engine.predict(data_object)
 
     m = engine.cosine_similarity_matrix()
 
-    assert math.isclose(m[0, 0], 1., abs_tol=0.001)
+    assert math.isclose(m[0, 0], 1.0, abs_tol=0.001)
     assert math.isclose(m[0, 1], 0.224325, abs_tol=0.001)
-    assert math.isclose(m[0, 2], 0., abs_tol=0.001)
+    assert math.isclose(m[0, 2], 0.0, abs_tol=0.001)
 
     assert math.isclose(m[1, 0], 0.224325, abs_tol=0.001)
-    assert math.isclose(m[1, 1], 1., abs_tol=0.001)
-    assert math.isclose(m[1, 2], 0., abs_tol=0.001)
+    assert math.isclose(m[1, 1], 1.0, abs_tol=0.001)
+    assert math.isclose(m[1, 2], 0.0, abs_tol=0.001)
 
-    assert math.isclose(m[2, 0], 0., abs_tol=0.001)
-    assert math.isclose(m[2, 1], 0., abs_tol=0.001)
-    assert math.isclose(m[2, 2], 1., abs_tol=0.001)
-
-    assert engine.ids == [1,2,3]
-    assert engine.docs == ["spinach omelet","kale omelet","cherry pie"]
-    assert engine.tfidf is not None
+    assert math.isclose(m[2, 0], 0.0, abs_tol=0.001)
+    assert math.isclose(m[2, 1], 0.0, abs_tol=0.001)
+    assert math.isclose(m[2, 2], 1.0, abs_tol=0.001)
+
+    assert engine.ids == [1, 2, 3]
+    assert engine.docs == ["spinach omelet", "kale omelet", "cherry pie"]
+    assert engine.tfidf is not None
```

### Comparing `primrose-1.0.9/test/test_depth_first_traverser.py` & `primrose-2.0.0/test/test_depth_first_traverser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-
 import pytest
 from primrose.configuration.configuration import Configuration
 from primrose.dag.depth_first_traverser import DepthFirstTraverser
 
+
 def test_traversal_list():
     config = {
-        "implementation_config":{
-            "reader_config":{
+        "implementation_config": {
+            "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['csv_writer']
+                    "destinations": ["csv_writer"],
                 },
                 "csv_reader2": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['successlogger']
-                }
+                    "destinations": ["successlogger"],
+                },
             },
             "writer_config": {
                 "csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
                     "filename": "unittest_similar_recipes.csv",
-                    "destinations": ["successlogger"]
+                    "destinations": ["successlogger"],
                 }
             },
             "cleanup_config": {
                 "successlogger": {
                     "class": "LoggingSuccess",
                     "msg": "woohoo, all done!",
                     "level": "INFO",
                 }
-            }
+            },
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     traverser = DepthFirstTraverser(configuration)
     sequence = traverser.traversal_list()
     print(sequence)
-    assert sequence == ['csv_reader2', 'csv_reader', 'csv_writer', 'successlogger']
+    assert sequence == ["csv_reader2", "csv_reader", "csv_writer", "successlogger"]
```

### Comparing `primrose-1.0.9/test/test_deserializer.py` & `primrose-2.0.0/test/test_deserializer.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,320 +7,359 @@
 from primrose.configuration.configuration import Configuration
 from primrose.data_object import DataObject, DataObjectResponseType
 from primrose.readers.csv_reader import CsvReader
 from primrose.readers.deserializer import Deserializer, GcsDeserializer
 
 
 def test_init_ok_dill():
+    try:
+        import sklearn.tree.tree
+        model_filename = "test/tinymodel.dill"
+    except ModuleNotFoundError:
+        # deprecation from sklearn>0.24 
+        # https://stackoverflow.com/questions/60598050/the-sklearn-tree-tree-module-is-deprecated-in-version-0-22-and-will-be-removed-i
+        model_filename = "test/tinymodel_skl_0_24.dill"
+
     config = {
         "implementation_config": {
             "reader_config": {
                 "dill_reader": {
                     "class": "Deserializer",
-                    "filename": "test/tinymodel.dill",
-                    "deserializer": 'dill',
-                    "destinations": []
+                    "filename": model_filename,
+                    "deserializer": "dill",
+                    "destinations": [],
                 }
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     data_object = DataObject(configuration)
 
     reader = Deserializer(configuration, "dill_reader")
     data_object, terminate = reader.run(data_object)
     assert not terminate
-    data = data_object.get('dill_reader', rtype=DataObjectResponseType.VALUE.value)
+    data = data_object.get("dill_reader", rtype=DataObjectResponseType.VALUE.value)
 
     assert data is not None
-    assert set(data.keys()) == {'test', 'model'}
+    assert set(data.keys()) == {"test", "model"}
 
     node_config = {
-                    "class": "Deserializer",
-                    "filename": "test/tinymodel.dill",
-                    "deserializer": 'dill',
-                    "destinations": []
-                }
+        "class": "Deserializer",
+        "filename": model_filename,
+        "deserializer": "dill",
+        "destinations": [],
+    }
 
     assert isinstance(Deserializer.necessary_config(node_config), set)
     assert len(Deserializer.necessary_config(node_config)) > 0
 
-    assert data['test'] == [1, 2, 3]
-    assert isinstance(data['model'], DecisionTreeClassifier)
+    assert data["test"] == [1, 2, 3]
+    assert isinstance(data["model"], DecisionTreeClassifier)
 
 
 def test_init_ok_pickle():
+    try:
+        import sklearn.tree.tree
+        model_filename = "test/tinymodel.pickle"
+    except ModuleNotFoundError:
+        model_filename = "test/tinymodel_skl_0_24.pickle"
+
     config = {
         "implementation_config": {
             "reader_config": {
                 "pickle_reader": {
                     "class": "Deserializer",
-                    "filename": "test/tinymodel.pickle",
-                    "deserializer": 'pickle',
-                    "destinations": []
+                    "filename": model_filename,
+                    "deserializer": "pickle",
+                    "destinations": [],
                 }
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     data_object = DataObject(configuration)
 
     reader = Deserializer(configuration, "pickle_reader")
     data_object, terminate = reader.run(data_object)
     assert not terminate
-    data = data_object.get('pickle_reader', rtype=DataObjectResponseType.VALUE.value)
+    data = data_object.get("pickle_reader", rtype=DataObjectResponseType.VALUE.value)
 
     assert data is not None
-    assert set(data.keys()) == {'test', 'model'}
+    assert set(data.keys()) == {"test", "model"}
+
+    assert data["test"] == [1, 2, 3]
+    assert isinstance(data["model"], DecisionTreeClassifier)
 
-    assert data['test'] == [1, 2, 3]
-    assert isinstance(data['model'], DecisionTreeClassifier)
 
 def test_init_ok_unsupported():
+    try:
+        import sklearn.tree.tree
+        model_filename = "test/tinymodel.pickle"
+    except ModuleNotFoundError:
+        model_filename = "test/tinymodel_skl_0_24.pickle"
+
     config = {
         "implementation_config": {
             "reader_config": {
                 "other_reader": {
                     "class": "Deserializer",
-                    "filename": "test/tinymodel.pickle",
-                    "deserializer": 'other',
-                    "destinations": []
+                    "filename": model_filename,
+                    "deserializer": "other",
+                    "destinations": [],
                 }
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     data_object = DataObject(configuration)
 
     reader = Deserializer(configuration, "other_reader")
     with pytest.raises(Exception, match=r"Unsupported"):
         reader.run(data_object)
 
+
 def test_gcsdeserializer_necessary_config():
     assert len(GcsDeserializer.necessary_config({})) == 3
 
+
 def test_run_dill(monkeypatch):
     # returns 2 objects from dill reader
     config = {
         "implementation_config": {
             "reader_config": {
                 "myreader": {
                     "class": "GcsDeserializer",
                     "bucket_name": "test1",
                     "blob_name": "test2",
                     "deserializer": "dill",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     reader = GcsDeserializer(configuration, "myreader")
 
     data_object = DataObject(configuration)
 
     def fake_blobs():
         with open("test/dill_reader_blob1.pkl", "wb") as dill_file:
             dill.dump("some_data", dill_file)
         with open("test/dill_reader_blob2.pkl", "wb") as dill_file:
             dill.dump("some_other_data", dill_file)
         dat1 = open("test/dill_reader_blob1.pkl", "rb").read()
         dat2 = open("test/dill_reader_blob2.pkl", "rb").read()
         return [dat1, dat2]
 
-    monkeypatch.setattr(reader,'download_blobs_as_strings',fake_blobs)
+    monkeypatch.setattr(reader, "download_blobs_as_strings", fake_blobs)
 
     reader_object, terminate = reader.run(data_object)
 
     assert not terminate
 
     assert "myreader" in reader_object.data_dict
 
-    dat = reader_object.data_dict['myreader']
+    dat = reader_object.data_dict["myreader"]
 
     assert "reader_data" in dat
-    datlist = dat['reader_data']
+    datlist = dat["reader_data"]
 
     assert len(datlist) == 2
 
     assert "some_data" in datlist
     assert "some_other_data" in datlist
 
     files = ["test/dill_reader_blob1.pkl", "test/dill_reader_blob2.pkl"]
     for f in files:
         if os.path.exists(f):
             os.remove(f)
 
+
 def test_run_dill_2(monkeypatch):
     # returns 1 objects from dill reader
     config = {
         "implementation_config": {
             "reader_config": {
                 "myreader": {
                     "class": "GcsDillReader",
                     "bucket_name": "test1",
                     "blob_name": "test2",
                     "deserializer": "dill",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     reader = GcsDeserializer(configuration, "myreader")
 
     data_object = DataObject(configuration)
 
     def fake_blobs():
         with open("test/dill_reader_blob1.pkl", "wb") as dill_file:
             dill.dump("some_data", dill_file)
         dat1 = open("test/dill_reader_blob1.pkl", "rb").read()
         return [dat1]
 
-    monkeypatch.setattr(reader,'download_blobs_as_strings',fake_blobs)
+    monkeypatch.setattr(reader, "download_blobs_as_strings", fake_blobs)
 
     reader_object, terminate = reader.run(data_object)
 
     assert not terminate
 
     assert "myreader" in reader_object.data_dict
 
-    dat = reader_object.data_dict['myreader']
+    dat = reader_object.data_dict["myreader"]
 
     assert "reader_data" in dat
-    data = dat['reader_data']
+    data = dat["reader_data"]
 
     assert "some_data" == data
 
     files = ["test/dill_reader_blob1.pkl"]
     for f in files:
         if os.path.exists(f):
             os.remove(f)
 
+
 def test_run_pickle(monkeypatch):
     # returns 2 objects from pickle reader
     config = {
         "implementation_config": {
             "reader_config": {
                 "myreader": {
                     "class": "GcsDeserializer",
                     "bucket_name": "test1",
                     "blob_name": "test2",
                     "deserializer": "pickle",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     reader = GcsDeserializer(configuration, "myreader")
 
     data_object = DataObject(configuration)
 
     def fake_blobs():
         with open("test/pickle_reader_blob1.pkl", "wb") as pickle_file:
             pickle.dump("some_data", pickle_file)
         with open("test/pickle_reader_blob2.pkl", "wb") as pickle_file:
             pickle.dump("some_other_data", pickle_file)
         dat1 = open("test/pickle_reader_blob1.pkl", "rb").read()
         dat2 = open("test/pickle_reader_blob2.pkl", "rb").read()
         return [dat1, dat2]
 
-    monkeypatch.setattr(reader,'download_blobs_as_strings',fake_blobs)
+    monkeypatch.setattr(reader, "download_blobs_as_strings", fake_blobs)
 
     reader_object, terminate = reader.run(data_object)
 
     assert not terminate
 
     assert "myreader" in reader_object.data_dict
 
-    dat = reader_object.data_dict['myreader']
+    dat = reader_object.data_dict["myreader"]
 
     assert "reader_data" in dat
-    datlist = dat['reader_data']
+    datlist = dat["reader_data"]
 
     assert len(datlist) == 2
 
     assert "some_data" in datlist
     assert "some_other_data" in datlist
 
     files = ["test/pickle_reader_blob1.pkl", "test/pickle_reader_blob2.pkl"]
     for f in files:
         if os.path.exists(f):
             os.remove(f)
 
+
 def test_run_pickle_2(monkeypatch):
     # returns 1 objects from pickle reader
     config = {
         "implementation_config": {
             "reader_config": {
                 "myreader": {
                     "class": "GcsDillReader",
                     "bucket_name": "test1",
                     "blob_name": "test2",
                     "deserializer": "pickle",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     reader = GcsDeserializer(configuration, "myreader")
 
     data_object = DataObject(configuration)
 
     def fake_blobs():
         with open("test/pickle_reader_blob1.pkl", "wb") as pickle_file:
             pickle.dump("some_data", pickle_file)
         dat1 = open("test/pickle_reader_blob1.pkl", "rb").read()
         return [dat1]
 
-    monkeypatch.setattr(reader,'download_blobs_as_strings',fake_blobs)
+    monkeypatch.setattr(reader, "download_blobs_as_strings", fake_blobs)
 
     reader_object, terminate = reader.run(data_object)
 
     assert not terminate
 
     assert "myreader" in reader_object.data_dict
 
-    dat = reader_object.data_dict['myreader']
+    dat = reader_object.data_dict["myreader"]
 
     assert "reader_data" in dat
-    data = dat['reader_data']
+    data = dat["reader_data"]
 
     assert "some_data" == data
 
     files = ["test/pickle_reader_blob1.pkl"]
     for f in files:
         if os.path.exists(f):
             os.remove(f)
 
+
 def test_run_other(monkeypatch):
     config = {
         "implementation_config": {
             "reader_config": {
                 "myreader": {
                     "class": "GcsDillReader",
                     "bucket_name": "test1",
                     "blob_name": "test2",
                     "deserializer": "other",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     reader = GcsDeserializer(configuration, "myreader")
 
     data_object = DataObject(configuration)
 
     with pytest.raises(Exception, match=r"Unsupported"):
         reader.run(data_object)
-
-
-
-
```

### Comparing `primrose-1.0.9/test/test_conditional_path_node.py` & `primrose-2.0.0/test/test_conditional_path_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,105 +1,110 @@
 import pytest
 from primrose.base.conditional_path_node import AbstractConditionalPath
 from primrose.configuration.configuration import Configuration
 from primrose.node_factory import NodeFactory
 
+
 def test_all_nodes_to_prune():
     class TestConditionalNode(AbstractConditionalPath):
         @staticmethod
-        def necessary_config(node_config): return set()
+        def necessary_config(node_config):
+            return set()
+
         def destinations_to_prune(self):
             return ["csv_writer2"]
+
         def run(self, data_object):
             return data_object, False
 
     NodeFactory().register("TestConditionalNode", TestConditionalNode)
 
     config = {
         "implementation_config": {
             "reader_config": {
                 "conditional_node": {
                     "class": "TestConditionalNode",
-                    "destinations": ['csv_writer', 'csv_writer2']
+                    "destinations": ["csv_writer", "csv_writer2"],
                 }
             },
             "writer_config": {
                 "csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
+                    "filename": "unittest_similar_recipes.csv",
                 },
                 "csv_writer2": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
                     "filename": "unittest_similar_recipes.csv",
-                    "destinations": ["csv_writer3"]
+                    "destinations": ["csv_writer3"],
                 },
                 "csv_writer3": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
-                }
-            }
+                    "filename": "unittest_similar_recipes.csv",
+                },
+            },
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     node = TestConditionalNode(configuration, "conditional_node")
     assert node.destinations_to_prune() == ["csv_writer2"]
     all_nodes = node.all_nodes_to_prune()
     assert len(all_nodes) == 2
     assert "csv_writer2" in all_nodes
     assert "csv_writer3" in all_nodes
 
     config = {
         "implementation_config": {
-            "reader_config": {
-                "conditional_node": {
-                    "class": "TestConditionalNode"
-                }
-            }
+            "reader_config": {"conditional_node": {"class": "TestConditionalNode"}}
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     node = TestConditionalNode(configuration, "conditional_node")
 
     with pytest.raises(Exception) as e:
         node.all_nodes_to_prune()
     assert "Destinations key is missing" in str(e)
 
+
 def test_all_nodes_to_prune2():
     class TestConditionalNode(AbstractConditionalPath):
         @staticmethod
-        def necessary_config(node_config): return set()
+        def necessary_config(node_config):
+            return set()
+
         def destinations_to_prune(self):
             return ["junk"]
+
         def run(self, data_object):
             return data_object, False
+
     NodeFactory().register("TestConditionalNode", TestConditionalNode)
 
     config = {
         "implementation_config": {
             "reader_config": {
                 "conditional_node": {
                     "class": "TestConditionalNode",
-                    "destinations": ['csv_writer']
+                    "destinations": ["csv_writer"],
                 }
             },
             "writer_config": {
                 "csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
+                    "filename": "unittest_similar_recipes.csv",
                 }
-            }
+            },
         }
     }
 
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     node = TestConditionalNode(configuration, "conditional_node")
 
     with pytest.raises(Exception) as e:
```

### Comparing `primrose-1.0.9/test/test_sklearn_regression_model.py` & `primrose-2.0.0/test/test_sklearn_regression_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,55 @@
-
 import pytest
 from primrose.configuration.configuration import Configuration
 from primrose.dag_runner import DagRunner
 import os
 import math
 
+
 def test_run():
     config = {
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "SklearnDatasetReader",
                     "dataset": "iris",
-                    "destinations": [
-                        "train_test_split"
-                    ]
+                    "destinations": ["train_test_split"],
                 }
             },
             "pipeline_config": {
                 "train_test_split": {
                     "class": "TrainTestSplit",
-                    "features": ["sepal length (cm)", "petal length (cm)", "petal width (cm)"],
+                    "features": [
+                        "sepal length (cm)",
+                        "petal length (cm)",
+                        "petal width (cm)",
+                    ],
                     "target_variable": "sepal width (cm)",
                     "training_fraction": 0.65,
                     "is_training": True,
                     "seed": 42,
-                    "destinations": [
-                        "regression_model"
-                    ]
+                    "destinations": ["regression_model"],
                 }
             },
             "model_config": {
-                "regression_model":{
+                "regression_model": {
                     "class": "SklearnRegressionModel",
                     "mode": "train",
                     "model": {"class": "linear_model.LinearRegression"},
-                    "destinations": []
+                    "destinations": [],
                 }
-            }
+            },
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     data_object = DagRunner(configuration).run()
-    scores = data_object.data_dict['regression_model']['scores']
+    scores = data_object.data_dict["regression_model"]["scores"]
     print(scores)
 
-    assert math.isclose(scores['Explained variance'], 0.531103247696713, abs_tol = 0.00001)
-#{'Explained variance': 0.531103247696713, 'Max error': 0.8037485197869163, 'Mean absolute error': 0.2050877131438389, 'MSE': 0.09214453355442812, 'Mean squared log error': 0.005413269099842543, 'R2': 0.5252494593646577, 'eval_time': datetime.datetime(2019, 7, 26, 13, 12, 13, 185343)}
+    assert math.isclose(
+        scores["Explained variance"], 0.531103247696713, abs_tol=0.00001
+    )
+
+
+# {'Explained variance': 0.531103247696713, 'Max error': 0.8037485197869163, 'Mean absolute error': 0.2050877131438389, 'MSE': 0.09214453355442812, 'Mean squared log error': 0.005413269099842543, 'R2': 0.5252494593646577, 'eval_time': datetime.datetime(2019, 7, 26, 13, 12, 13, 185343)}
```

### Comparing `primrose-1.0.9/test/test_file_writer.py` & `primrose-2.0.0/test/test_file_writer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,77 @@
-
 import pytest
 import sys
 import os
 import pandas as pd
 from primrose.configuration.configuration import Configuration
 from primrose.writers.file_writer import FileWriter
 from primrose.data_object import DataObject
 from primrose.readers.csv_reader import CsvReader
 
+
 @pytest.fixture()
 def config():
     config = {
         "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ['recipe_file_writer']
+                    "destinations": ["recipe_file_writer"],
                 }
             },
             "writer_config": {
                 "recipe_file_writer": {
                     "class": "FileWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_file_writer.txt"
+                    "filename": "unittest_file_writer.txt",
                 }
-            }
+            },
         }
     }
     return config
 
+
 def test_necessary_config(config):
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
-    writer = FileWriter(configuration, 'recipe_file_writer')
+    writer = FileWriter(configuration, "recipe_file_writer")
     node_config = {
-                    "class": "FileWriter",
-                    "key":"test_data",
-                    "dir": "cache",
-                    "filename": "unittest_file_writer.txt"
-                }
+        "class": "FileWriter",
+        "key": "test_data",
+        "dir": "cache",
+        "filename": "unittest_file_writer.txt",
+    }
     assert isinstance(writer.necessary_config(node_config), set)
     assert len(writer.necessary_config(node_config)) > 0
 
+
 def test_init_ok(config):
 
     test_data_string = "some test data"
 
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     data_object = DataObject(configuration)
 
-    requestor = CsvReader(configuration, 'csv_reader')
+    requestor = CsvReader(configuration, "csv_reader")
 
-    data_object.add(requestor, test_data_string, 'test_data')
+    data_object.add(requestor, test_data_string, "test_data")
 
-    writer = FileWriter(configuration, 'recipe_file_writer')
+    writer = FileWriter(configuration, "recipe_file_writer")
 
-    c = configuration.config_for_instance('recipe_file_writer')
-    filename = c['dir'] + os.path.sep + c['filename']
+    c = configuration.config_for_instance("recipe_file_writer")
+    filename = c["dir"] + os.path.sep + c["filename"]
 
-    #clean out test file location 
+    # clean out test file location
     if os.path.exists(filename):
         os.remove(filename)
 
     data_object, terminate = writer.run(data_object)
 
     assert not terminate
 
     assert os.path.exists(filename)
 
     read_data = open(filename).read()
 
-    assert test_data_string == read_data
+    assert test_data_string == read_data
```

### Comparing `primrose-1.0.9/test/test_abstract_pipeline.py` & `primrose-2.0.0/test/test_abstract_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,102 +1,120 @@
-
 import pytest
 from primrose.base.pipeline import AbstractPipeline
 from primrose.base.pipeline import PipelineModeType
 from primrose.configuration.configuration import Configuration
 from primrose.data_object import DataObject
 from primrose.readers.csv_reader import CsvReader
 from primrose.base.transformer_sequence import TransformerSequence
 from primrose.base.transformer import AbstractTransformer
 from primrose.node_factory import NodeFactory
 import pandas as pd
 import logging
 from testfixtures import LogCapture
 
+
 def test_names():
-    assert PipelineModeType.names() == ['FIT', 'FIT_TRANSFORM', 'TRANSFORM']
+    assert PipelineModeType.names() == ["FIT", "FIT_TRANSFORM", "TRANSFORM"]
+
 
 def test_values():
-    assert PipelineModeType.values() == ['FIT', 'FIT_TRANSFORM', 'TRANSFORM']
+    assert PipelineModeType.values() == ["FIT", "FIT_TRANSFORM", "TRANSFORM"]
 
-def test_run():
 
+def test_run():
     class TestPipeline(AbstractPipeline):
         def transform(self, data_object):
             logging.info("TRANSFORM CALLED")
-            return data_object 
+            return data_object
 
         def fit_transform(self, data_object):
             logging.info("FIT_TRANSFORM CALLED")
             return self.transform(data_object)
 
         @staticmethod
-        def necessary_config(node_config): return set(['is_training'])
+        def necessary_config(node_config):
+            return set(["is_training"])
 
     NodeFactory().register("TestPipeline", TestPipeline)
 
     config = {
         "implementation_config": {
             "reader_config": {
                 "myreader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ["mypipeline"]
+                    "destinations": ["mypipeline"],
                 }
             },
             "pipeline_config": {
-                "mypipeline":{
-                    "class": "TestPipeline",
-                    "is_training": True
-                }
-            }
+                "mypipeline": {"class": "TestPipeline", "is_training": True}
+            },
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     reference_file_path = "test/minimal.csv"
     corpus = pd.read_csv(reference_file_path)
 
     reader = CsvReader(configuration, "myreader")
 
     data_object = DataObject(configuration)
     data_object.add(reader, corpus)
 
     pipeline = TestPipeline(configuration, "mypipeline")
 
     with LogCapture() as l:
         pipeline.run(data_object)
     l.check(
-        ('root', 'INFO', 'No upstream TransformerSequence found. Creating new TransformerSequence...'),
-        ('root', 'INFO', 'FIT_TRANSFORM CALLED'),
-        ('root', 'INFO', 'TRANSFORM CALLED')
+        (
+            "root",
+            "INFO",
+            "No upstream TransformerSequence found. Creating new TransformerSequence...",
+        ),
+        ("root", "INFO", "FIT_TRANSFORM CALLED"),
+        ("root", "INFO", "TRANSFORM CALLED"),
     )
 
     data_object.add(reader, TransformerSequence(), "tsequence")
     with LogCapture() as l:
         pipeline.run(data_object)
     l.check(
-        ('root', 'INFO', 'Upstream TransformerSequence found, initializing pipeline...'),
-        ('root', 'INFO', 'FIT_TRANSFORM CALLED'),
-        ('root', 'INFO', 'TRANSFORM CALLED')
+        (
+            "root",
+            "INFO",
+            "Upstream TransformerSequence found, initializing pipeline...",
+        ),
+        ("root", "INFO", "FIT_TRANSFORM CALLED"),
+        ("root", "INFO", "TRANSFORM CALLED"),
     )
 
-    config['implementation_config']['pipeline_config']['mypipeline']['is_training'] = False
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    config["implementation_config"]["pipeline_config"]["mypipeline"][
+        "is_training"
+    ] = False
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     reader = CsvReader(configuration, "myreader")
     data_object = DataObject(configuration)
     data_object.add(reader, corpus)
     pipeline = TestPipeline(configuration, "mypipeline")
     with LogCapture() as l:
         pipeline.run(data_object)
     l.check(
-        ('root', 'INFO', 'No upstream TransformerSequence found. Creating new TransformerSequence...'),
-        ('root', 'INFO', 'TRANSFORM CALLED')
+        (
+            "root",
+            "INFO",
+            "No upstream TransformerSequence found. Creating new TransformerSequence...",
+        ),
+        ("root", "INFO", "TRANSFORM CALLED"),
     )
 
+
 def test_execute_pipeline():
     class TestTransformer(AbstractTransformer):
         def fit(self, data):
             logging.info("Transfer FIT CALLED")
 
         def transform(self, data):
             logging.info("Transfer TRANSFORM CALLED")
@@ -104,69 +122,69 @@
 
         def fit_transform(self, data):
             logging.info("Transfer FIT_TRANSFORM CALLED")
             self.fit(data)
             return self.transform(data)
 
     class TestPipeline2(AbstractPipeline):
-        def transform(self, data_object): return data_object 
+        def transform(self, data_object):
+            return data_object
+
         @staticmethod
-        def necessary_config(node_config): return set(['is_training'])
+        def necessary_config(node_config):
+            return set(["is_training"])
+
     NodeFactory().register("TestPipeline2", TestPipeline2)
 
     config = {
         "implementation_config": {
             "reader_config": {
                 "myreader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ["mypipeline"]
+                    "destinations": ["mypipeline"],
                 }
             },
             "pipeline_config": {
-                "mypipeline":{
-                    "class": "TestPipeline",
-                    "is_training": True
-                }
-            }
+                "mypipeline": {"class": "TestPipeline", "is_training": True}
+            },
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     reference_file_path = "test/minimal.csv"
     corpus = pd.read_csv(reference_file_path)
 
     reader = CsvReader(configuration, "myreader")
 
     data_object = DataObject(configuration)
     data_object.add(reader, corpus)
 
     sequence = TransformerSequence()
     sequence.add(TestTransformer())
     data_object.add(reader, sequence, "tsequence")
 
-
     pipeline = TestPipeline2(configuration, "mypipeline")
 
     with pytest.raises(Exception) as e:
-         pipeline.execute_pipeline(corpus, PipelineModeType.FIT)
+        pipeline.execute_pipeline(corpus, PipelineModeType.FIT)
     assert "run() must be called to extract/create a TransformerSequence" in str(e)
 
     pipeline.run(data_object)
 
     with pytest.raises(Exception) as e:
-         pipeline.execute_pipeline(corpus,"JUNK")
+        pipeline.execute_pipeline(corpus, "JUNK")
     assert "mode must be of type PipelineModeType Enum object." in str(e)
 
     with LogCapture() as l:
         pipeline.execute_pipeline(corpus, PipelineModeType.FIT)
-    l.check(
-        ('root', 'INFO', 'Transfer FIT CALLED')
-    )
+    l.check(("root", "INFO", "Transfer FIT CALLED"))
 
     with LogCapture() as l:
         pipeline.execute_pipeline(corpus, PipelineModeType.FIT_TRANSFORM)
     l.check(
-        ('root', 'INFO', 'Transfer FIT_TRANSFORM CALLED'),
-        ('root', 'INFO', 'Transfer FIT CALLED'),
-        ('root', 'INFO', 'Transfer TRANSFORM CALLED')
-    )
+        ("root", "INFO", "Transfer FIT_TRANSFORM CALLED"),
+        ("root", "INFO", "Transfer FIT CALLED"),
+        ("root", "INFO", "Transfer TRANSFORM CALLED"),
+    )
```

### Comparing `primrose-1.0.9/test/test_abstract_sql_reader.py` & `primrose-2.0.0/test/test_abstract_sql_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,73 @@
-
 import pytest
 import os
 from primrose.base.sql_reader import AbstractSqlReader
 from primrose.configuration.configuration import Configuration
 from primrose.readers.sqlite_reader import SQLiteReader
 import sqlite3
 
+
 def test__substitute_query():
 
     query = """SELECT * FROM TABLE where field={x} and otherfield='{y}'"""
 
     filename = "test/test_substitute.sql"
     if os.path.exists(filename):
         os.remove(filename)
 
-    with open(filename, 'w') as f:
+    with open(filename, "w") as f:
         f.write(query)
 
     individual_query_json = {
         "query": "test/test_substitute.sql",
-        "parameters": {
-            "x": 3,
-            "y": "somestring"
-        }
+        "parameters": {"x": 3, "y": "somestring"},
     }
+
     class TestSqlReader(AbstractSqlReader):
-        pass   
-    
+        pass
+
     transformed_query = TestSqlReader._substitute_query(individual_query_json)
 
-    assert transformed_query == "SELECT * FROM TABLE where field=3 and otherfield='somestring'"
+    assert (
+        transformed_query
+        == "SELECT * FROM TABLE where field=3 and otherfield='somestring'"
+    )
 
     if os.path.exists(filename):
         os.remove(filename)
 
+
 def test__substitute_query2():
     query_00 = """SELECT * FROM TABLE where field={x} and otherfield='{y}'"""
     query_01 = """SELECT * FROM TABLE where field={a} and otherfield='{b}'"""
     query_02 = """
     {% include 'test/test_substitute_00.sql' %}
     UNION ALL
     {% include 'test/test_substitute_01.sql' %}
     """
     queries = [query_00, query_01, query_02]
-    
+
     filenames = []
     for i in range(3):
         filename = "test/test_substitute_{:02d}.sql".format(i)
         filenames.append(filename)
         if os.path.exists(filename):
             os.remove(filename)
 
-        with open(filename, 'w') as f:
+        with open(filename, "w") as f:
             f.write(queries[i])
 
     individual_query_json = {
         "query": "test/test_substitute_02.sql",
-        "parameters": {
-            "a": 2,
-            "b": "somestring2",
-            "x": 3,
-            "y": "somestring"
-        }
+        "parameters": {"a": 2, "b": "somestring2", "x": 3, "y": "somestring"},
     }
+
     class TestSqlReader(AbstractSqlReader):
-        pass   
-    
+        pass
+
     transformed_query = TestSqlReader._substitute_query(individual_query_json)
 
     expected_query = """
     SELECT * FROM TABLE where field=3 and otherfield='somestring'
     UNION ALL
     SELECT * FROM TABLE where field=2 and otherfield='somestring2'
     """
@@ -77,75 +75,76 @@
 
     assert transformed_query == expected_query
 
     for filename in filenames:
         if os.path.exists(filename):
             os.remove(filename)
 
+
 def test__generate_queries():
 
     config = {
         "implementation_config": {
             "reader_config": {
                 "myreader": {
                     "class": "SQLiteReader",
                     "filename": "test/test_abstract_sqlite.db",
                     "destinations": [],
                     "query_json": [
                         {
                             "query": "test/test_substitute1.sql",
-                            "parameters": {
-                                "firstname": "joe",
-                                "lastname": "doe2"
-                            }
+                            "parameters": {"firstname": "joe", "lastname": "doe2"},
                         },
                         {
                             "query": "test/test_substitute2.sql",
-                            "parameters": {
-                                "firstname": 'mary',
-                                "lastname": "poppins"
-                            }
-                        }
-                    ]
+                            "parameters": {"firstname": "mary", "lastname": "poppins"},
+                        },
+                    ],
                 }
             }
         }
     }
 
     filenames = ["test/test_substitute1.sql", "test/test_substitute2.sql"]
 
     for filename in filenames:
 
         query = """SELECT * FROM test where firstname='{firstname}' and lastname='{lastname}'"""
 
         if os.path.exists(filename):
             os.remove(filename)
 
-        with open(filename, 'w') as f:
+        with open(filename, "w") as f:
             f.write(query)
 
     db_filename = "test/test_abstract_sqlite.db"
     if os.path.exists(db_filename):
         os.remove(db_filename)
 
     conn = sqlite3.connect(db_filename)
     c = conn.cursor()
     c.execute("create table test(firstname text, lastname text);")
-    c.execute("insert into test(firstname, lastname) values('joe', 'doe'), ('joe', 'doe2'), ('mary','poppins');")
+    c.execute(
+        "insert into test(firstname, lastname) values('joe', 'doe'), ('joe', 'doe2'), ('mary','poppins');"
+    )
     conn.commit()
     conn.close()
 
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     reader = SQLiteReader(configuration, "myreader")
     queries = [q for q in reader._generate_queries()]
 
     assert len(queries) == 2
     assert queries[0] == "SELECT * FROM test where firstname='joe' and lastname='doe2'"
-    assert queries[1] == "SELECT * FROM test where firstname='mary' and lastname='poppins'"
+    assert (
+        queries[1] == "SELECT * FROM test where firstname='mary' and lastname='poppins'"
+    )
 
     for filename in filenames:
         if os.path.exists(filename):
             os.remove(filename)
-    
+
     if os.path.exists(db_filename):
-        os.remove(db_filename)
+        os.remove(db_filename)
```

### Comparing `primrose-1.0.9/test/test_dataframe_joiner.py` & `primrose-2.0.0/test/test_dataframe_joiner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import pytest
 from primrose.pipelines.dataframe_joiner import DataFrameJoiner
 from primrose.base.transformer_sequence import TransformerSequence
 from primrose.configuration.configuration import Configuration
 from primrose.readers.csv_reader import CsvReader
 import pandas as pd
 from primrose.data_object import DataObject
@@ -12,58 +11,63 @@
 def test_init_pipeline():
     config = {
         "implementation_config": {
             "reader_config": {
                 "myreader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ["mypipeline"]
+                    "destinations": ["mypipeline"],
                 }
             },
             "pipeline_config": {
-                "mypipeline":{
+                "mypipeline": {
                     "class": "DataFrameJoiner",
                     "join_key": ["first"],
-                    "start_table": "myreader"
+                    "start_table": "myreader",
                 }
-            }
+            },
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     pipeline = DataFrameJoiner(configuration, "mypipeline")
     ts = pipeline.init_pipeline()
     assert isinstance(ts, TransformerSequence)
 
+
 def test_transform():
     config = {
         "implementation_config": {
             "reader_config": {
                 "myreader_left": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ["mypipeline"]
+                    "destinations": ["mypipeline"],
                 },
                 "myreader_right": {
                     "class": "CsvReader",
                     "filename": "test/merge_right3.csv",
-                    "destinations": ["mypipeline"]
-                }
+                    "destinations": ["mypipeline"],
+                },
             },
             "pipeline_config": {
-                "mypipeline":{
+                "mypipeline": {
                     "class": "DataFrameJoiner",
                     "join_key": ["first"],
                     "start_table": "myreader_left",
-                    "is_training": True
+                    "is_training": True,
                 }
-            }
+            },
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     data_object = DataObject(configuration)
 
     left_df = pd.read_csv("test/minimal.csv")
     reader_left = CsvReader(configuration, "myreader_left")
     data_object.add(reader_left, left_df)
 
@@ -73,57 +77,69 @@
 
     pipeline = DataFrameJoiner(configuration, "mypipeline")
 
     data_object, terminate = pipeline.run(data_object)
 
     assert not terminate
 
-    joined_data = data_object.get("mypipeline", pop_data=True, rtype=DataObjectResponseType.VALUE.value)
+    joined_data = data_object.get(
+        "mypipeline", pop_data=True, rtype=DataObjectResponseType.VALUE.value
+    )
     assert joined_data.shape[0] == 2
 
-    assert list(joined_data.T.to_dict().values())[0] == {'first': 'joe', 'last': 'doe', 'age': 47}
-    assert list(joined_data.T.to_dict().values())[1] == {'first': 'mary', 'last': 'poppins', 'age': 42}
+    assert list(joined_data.T.to_dict().values())[0] == {
+        "first": "joe",
+        "last": "doe",
+        "age": 47,
+    }
+    assert list(joined_data.T.to_dict().values())[1] == {
+        "first": "mary",
+        "last": "poppins",
+        "age": 42,
+    }
 
 
 def test_transform2():
     config = {
         "implementation_config": {
             "reader_config": {
                 "myreader_left": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ["mypipeline"]
+                    "destinations": ["mypipeline"],
                 },
                 "myreader_right": {
                     "class": "CsvReader",
                     "filename": "test/merge_right3.csv",
-                    "destinations": ["mypipeline"]
-                }
+                    "destinations": ["mypipeline"],
+                },
             },
             "pipeline_config": {
-                "mypipeline":{
+                "mypipeline": {
                     "class": "DataFrameJoiner",
                     "join_key": ["first"],
                     "start_table": "JUNK",
-                    "is_training": True
+                    "is_training": True,
                 }
-            }
+            },
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
 
     data_object = DataObject(configuration)
 
     left_df = pd.read_csv("test/minimal.csv")
     reader_left = CsvReader(configuration, "myreader_left")
 
     right_df = pd.read_csv("test/merge_right3.csv")
     reader_right = CsvReader(configuration, "myreader_right")
 
-    #note: am deliberately swapping order to right is first
+    # note: am deliberately swapping order to right is first
     data_object.add(reader_right, right_df)
     data_object.add(reader_left, left_df)
 
     pipeline = DataFrameJoiner(configuration, "mypipeline")
 
     with pytest.raises(Exception) as e:
         pipeline.run(data_object)
```

### Comparing `primrose-1.0.9/test/test_transformer_filters.py` & `primrose-2.0.0/test/test_transformer_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,53 @@
-
 import pytest
 import pandas as pd
 
 from primrose.transformers.filter import FilterByPandasExpression
 
+
 def test_transform():
     df = pd.read_csv("test/tennis.csv")
 
     ft = FilterByPandasExpression([["outlook", "==", "sunny"]])
 
     assert not ft.fit(df)
 
     assert df.shape == (14, 6)
 
     filtered_df = ft.transform(df)
 
     assert filtered_df.shape == (5, 6)
 
+
 def test_transform2():
     df = pd.read_csv("test/tennis.csv")
 
     ft = FilterByPandasExpression([])
 
     assert df.shape == (14, 6)
 
     filtered_df = ft.transform(df)
 
     assert filtered_df.shape == df.shape
 
+
 def test_transform3():
     ft = FilterByPandasExpression([["outlook", "==", "sunny"]])
     with pytest.raises(Exception) as e:
         ft.transform(42)
     assert "Data is not a pandas DataFrame" in str(e)
 
+
 def test_transform4():
     df = pd.read_csv("test/tennis.csv")
     ft = FilterByPandasExpression([["JUNK", "==", "sunny"]])
     with pytest.raises(Exception) as e:
         ft.transform(df)
     assert "Unrecognized filter column 'JUNK'" in str(e)
 
+
 def test_transform5():
     df = pd.read_csv("test/tennis.csv")
     ft = FilterByPandasExpression([["outlook", "JUNK", "sunny"]])
     with pytest.raises(Exception) as e:
         ft.transform(df)
     assert "Unsupported filter operation 'JUNK'" in str(e)
-
```

### Comparing `primrose-1.0.9/test/test_sklearn_preprocessing_transformer.py` & `primrose-2.0.0/test/test_sklearn_preprocessing_transformer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-
-from primrose.transformers.sklearn_preprocessing_transformer import SklearnPreprocessingTransformer
+from primrose.transformers.sklearn_preprocessing_transformer import (
+    SklearnPreprocessingTransformer,
+)
 from sklearn.preprocessing import StandardScaler
 import pytest
 import pandas as pd
 import math
 
+
 def test_fit():
     scaler = StandardScaler(with_mean=True, with_std=True)
-    t = SklearnPreprocessingTransformer(scaler, columns=['x','y'])
+    t = SklearnPreprocessingTransformer(scaler, columns=["x", "y"])
 
-    df = pd.DataFrame({'x':[1,2,3,4,5], 'y': [5,20,30,40,90]})
+    df = pd.DataFrame({"x": [1, 2, 3, 4, 5], "y": [5, 20, 30, 40, 90]})
     t.fit(df)
 
     transformed_data = t.transform(df)
 
     assert list(t.preprocessor.mean_) == [3.0, 37.0]
-    assert list(t.preprocessor.var_) == [2., 836.]
-    assert math.isclose(transformed_data.x.mean(), 0.0, abs_tol = 0.0001)
-    #note setting this default degrees of freedom=0 is important as it won't match numpy's std for same data otherwise
-    assert math.isclose(transformed_data.x.std(ddof=0), 1.0, abs_tol = 0.0001)
-    assert math.isclose(transformed_data.y.mean(), 0.0, abs_tol = 0.0001)
-    assert math.isclose(transformed_data.y.std(ddof=0), 1.0, abs_tol = 0.0001)
+    assert list(t.preprocessor.var_) == [2.0, 836.0]
+    assert math.isclose(transformed_data.x.mean(), 0.0, abs_tol=0.0001)
+    # note setting this default degrees of freedom=0 is important as it won't match numpy's std for same data otherwise
+    assert math.isclose(transformed_data.x.std(ddof=0), 1.0, abs_tol=0.0001)
+    assert math.isclose(transformed_data.y.mean(), 0.0, abs_tol=0.0001)
+    assert math.isclose(transformed_data.y.std(ddof=0), 1.0, abs_tol=0.0001)
```

### Comparing `primrose-1.0.9/test/test_dag_runner.py` & `primrose-2.0.0/test/test_dag_runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import os
 import unittest
 import unittest.mock as mock
 
 import pytest
 
 from primrose.configuration.configuration import Configuration
@@ -13,261 +12,294 @@
 from primrose.writers.abstract_file_writer import AbstractFileWriter
 from primrose.dag.config_layer_traverser import ConfigLayerTraverser
 from primrose.data_object import DataObject
 from primrose.data_object import DataObjectResponseType
 from primrose.dag.dag_traverser import DagTraverser
 from primrose.dag.traverser_factory import TraverserFactory
 from abc import abstractmethod
-from primrose.base.writer import  AbstractWriter
+from primrose.base.writer import AbstractWriter
 
 
 def test_run():
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     runner = DagRunner(configuration)
     runner.run()
 
+
 def test_run2():
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     runner = DagRunner(configuration)
     with LogCapture() as l:
         runner.run(dry_run=True)
-    l.check(('root', 'INFO', 'Taking nodes to run from default'),
-            ('root', 'INFO', 'DRY RUN 0: would run node csv_reader of type reader_config and class CsvReader'),
-            ('root', 'INFO', 'All done. Bye bye!'))
+    l.check(
+        ("root", "INFO", "Taking nodes to run from default"),
+        (
+            "root",
+            "INFO",
+            "DRY RUN 0: would run node csv_reader of type reader_config and class CsvReader",
+        ),
+        ("root", "INFO", "All done. Bye bye!"),
+    )
+
 
 def test_run3():
     config = {
         "metadata": "ConfigLayerTraverser",
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ["csv_writer"]
+                    "destinations": ["csv_writer"],
                 }
             },
             "writer_config": {
                 "csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "test/unittest_similar_recipes.csv"
+                    "filename": "test/unittest_similar_recipes.csv",
                 }
-            }
-        }
+            },
+        },
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     runner = DagRunner(configuration)
 
     with LogCapture() as l:
         runner.run(dry_run=True)
-    l.check(('root', 'INFO', 'Taking nodes to run from default'),
-            ('root', 'INFO', 'DRY RUN 0: would run node csv_reader of type reader_config and class CsvReader'),
-            ('root', 'INFO', 'DRY RUN 1: would run node csv_writer of type writer_config and class CsvWriter'),
-            ('root', 'INFO', 'All done. Bye bye!'))
+    l.check(
+        ("root", "INFO", "Taking nodes to run from default"),
+        (
+            "root",
+            "INFO",
+            "DRY RUN 0: would run node csv_reader of type reader_config and class CsvReader",
+        ),
+        (
+            "root",
+            "INFO",
+            "DRY RUN 1: would run node csv_writer of type writer_config and class CsvWriter",
+        ),
+        ("root", "INFO", "All done. Bye bye!"),
+    )
 
-def test_run4():
 
+def test_run4():
     class TestWriter(AbstractFileWriter):
         def __init__(self, configuration, instance_name):
             pass
+
         @staticmethod
         def necessary_config(node_config):
             return set([])
+
         def run(self, data_object):
             terminate = True
             return data_object, terminate
+
     NodeFactory().register("TestWriter", TestWriter)
 
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ["csv_writer"]
+                    "destinations": ["csv_writer"],
                 }
             },
-            "writer_config": {
-                "csv_writer": {
-                    "class": "TestWriter"
-                }
-            }
+            "writer_config": {"csv_writer": {"class": "TestWriter"}},
         }
     }
 
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     runner = DagRunner(configuration)
 
     with LogCapture() as l:
         runner.run(dry_run=False)
-    l.check(('root', 'INFO', 'Taking nodes to run from default'),
-        ('root','INFO','received node csv_reader of type reader_config and class CsvReader'),
-        ('root', 'INFO', 'Reading test/minimal.csv from CSV'),
-        ('root', 'INFO', 'received node csv_writer of type writer_config and class TestWriter'),
-        ('root', 'INFO', 'Terminating early due to signal from csv_writer'),
-        ('root', 'INFO', 'All done. Bye bye!'))
+    l.check(
+        ("root", "INFO", "Taking nodes to run from default"),
+        (
+            "root",
+            "INFO",
+            "received node csv_reader of type reader_config and class CsvReader",
+        ),
+        ("root", "INFO", "Reading test/minimal.csv from CSV"),
+        (
+            "root",
+            "INFO",
+            "received node csv_writer of type writer_config and class TestWriter",
+        ),
+        ("root", "INFO", "Terminating early due to signal from csv_writer"),
+        ("root", "INFO", "All done. Bye bye!"),
+    )
+
 
 def test_run5():
     config = {
-        "metadata": {
-            "section_registry":[
-                "phase1",
-                "phase2"
-            ]
-        },
-        "implementation_config":{
+        "metadata": {"section_registry": ["phase1", "phase2"]},
+        "implementation_config": {
             "phase1": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ["csv_writer"]
+                    "destinations": ["csv_writer"],
                 }
             },
             "phase2": {
                 "csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "test/unittest_similar_recipes.csv"
+                    "filename": "test/unittest_similar_recipes.csv",
                 }
-            }
-        }
+            },
+        },
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     runner = DagRunner(configuration)
 
     with LogCapture() as l:
         runner.run(dry_run=True)
-    l.check(('root', 'INFO', 'Taking nodes to run from section_registry'),
-            ('root', 'INFO', 'DRY RUN 0: would run node csv_reader of type phase1 and class CsvReader'),
-            ('root', 'INFO', 'DRY RUN 1: would run node csv_writer of type phase2 and class CsvWriter'),
-            ('root', 'INFO', 'All done. Bye bye!'))
+    l.check(
+        ("root", "INFO", "Taking nodes to run from section_registry"),
+        (
+            "root",
+            "INFO",
+            "DRY RUN 0: would run node csv_reader of type phase1 and class CsvReader",
+        ),
+        (
+            "root",
+            "INFO",
+            "DRY RUN 1: would run node csv_writer of type phase2 and class CsvWriter",
+        ),
+        ("root", "INFO", "All done. Bye bye!"),
+    )
 
 
 def test_run6():
     config = {
         "metadata": {
-            "section_registry": [
-                "phase1",
-                "cleanup_config"
-            ],
+            "section_registry": ["phase1", "cleanup_config"],
             "notify_on_error": {
                 "client": "SlackClient",
                 "channel": "some-channel",
                 "token": "slack-api-token",
-                "member_id": "optional-key"
-            }
+                "member_id": "optional-key",
+            },
         },
         "implementation_config": {
             "phase1": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": ["notification"]
+                    "destinations": ["notification"],
                 }
             },
             "cleanup_config": {
                 "notification": {
                     "class": "ClientNotification",
                     "client": "SlackClient",
                     "channel": "some-channel",
                     "token": "slack-api-token",
                     "member_id": "optional-key",
-                    "message": "Yay! Sucess"
+                    "message": "Yay! Sucess",
                 }
-            }
-        }
+            },
+        },
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     runner = DagRunner(configuration)
 
     with LogCapture() as l:
         runner.run(dry_run=True)
-    l.check(('root', 'INFO', 'Taking nodes to run from section_registry'),
-            ('root', 'INFO', 'DRY RUN 0: would run node csv_reader of type phase1 and class CsvReader'),
-            ('root', 'INFO', 'DRY RUN 1: would run node notification of type cleanup_config and class ClientNotification'),
-            ('root', 'INFO', 'All done. Bye bye!'))
+    l.check(
+        ("root", "INFO", "Taking nodes to run from section_registry"),
+        (
+            "root",
+            "INFO",
+            "DRY RUN 0: would run node csv_reader of type phase1 and class CsvReader",
+        ),
+        (
+            "root",
+            "INFO",
+            "DRY RUN 1: would run node notification of type cleanup_config and class ClientNotification",
+        ),
+        ("root", "INFO", "All done. Bye bye!"),
+    )
 
 
 def test_run_notification_error():
     config = {
         "metadata": {
-            "section_registry": [
-                "phase1"
-            ],
+            "section_registry": ["phase1"],
             "notify_on_error": {
                 "client": "SlackClient",
                 "channel": "some-channel",
                 "token": "slack-api-token",
-                "member_id": "optional-key"
-            }
+                "member_id": "optional-key",
+            },
         },
         "implementation_config": {
-            "phase1": {
-                "csv_reader": {
-                    "class": "CsvReader",
-                    "filename": "bad/path.csv"
-                }
-            }
-        }
+            "phase1": {"csv_reader": {"class": "CsvReader", "filename": "bad/path.csv"}}
+        },
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     runner = DagRunner(configuration)
 
     mock_client = mock.Mock()
     mock_client.post_message = mock.Mock()
     mock_get_notification_client = mock.Mock(return_value=mock_client)
 
-    path = 'primrose.notification_utils.get_notification_client'
+    path = "primrose.notification_utils.get_notification_client"
     with mock.patch(path) as mock_get_notification_client:
         with pytest.raises(Exception) as error:
             runner.run()
             assert mock_get_notification_client.post_message.call_count == 1
 
 
 def test_cache_data_object():
     config = {
         "metadata": {
             "data_object": {
                 "write_to_cache": True,
-                "write_filename": "dag_runner_test_cache_data_object.pkl"
+                "write_filename": "dag_runner_test_cache_data_object.pkl",
             }
         },
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
-        }
+        },
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     data_object = DataObject(configuration)
     writer = CsvReader(configuration, "csv_reader")
     data_object.add(writer, "some_data")
 
@@ -282,36 +314,37 @@
     assert cached
 
     assert os.path.exists(filename)
 
     if os.path.exists(filename):
         os.remove(filename)
 
+
 def test_create_data_object():
 
     filename = "dag_runner_create_data_object.pkl"
     # hack part 1: make sure this filename exists so that checks in Configuration pass
-    open(filename, 'w+')
+    open(filename, "w+")
 
     config = {
         "metadata": {
             "data_object": {
                 "read_from_cache": True,
-                "read_filename": "dag_runner_create_data_object.pkl"
+                "read_filename": "dag_runner_create_data_object.pkl",
             }
         },
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
-        }
+        },
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     # hack part 2: now get rid of it
     if os.path.exists(filename):
         os.remove(filename)
 
@@ -324,295 +357,296 @@
 
     # now we get to the code to test
     runner = DagRunner(configuration)
     restored_data_object = runner.create_data_object()
 
     # run some checks
     assert isinstance(restored_data_object, DataObject)
-    assert restored_data_object.get("csv_reader", rtype=DataObjectResponseType.VALUE.value) == "some_data"
+    assert (
+        restored_data_object.get("csv_reader", rtype=DataObjectResponseType.VALUE.value)
+        == "some_data"
+    )
 
-    #cleanup
+    # cleanup
     if os.path.exists(filename):
         os.remove(filename)
 
-def test_init_traverser_from_config():
 
+def test_init_traverser_from_config():
     class TestTraverser(DagTraverser):
-        def traversal_list(self): return []
-        def run_section_by_section(self): return False
+        def traversal_list(self):
+            return []
+
+        def run_section_by_section(self):
+            return False
 
     TraverserFactory().register("TestTraverser", TestTraverser)
 
     config = {
-        "metadata": {
-            "traverser": "TestTraverser"
-        },
-        "implementation_config":{
+        "metadata": {"traverser": "TestTraverser"},
+        "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
-        }
+        },
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     runner = DagRunner(configuration)
 
     assert isinstance(runner.dag_traverser, TestTraverser)
 
+
 def test_filter_sequence1():
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     runner = DagRunner(configuration)
 
     with pytest.raises(Exception) as e:
         runner.filter_sequence(["csv_reader", "csv_reader"])
     assert "You have duplicate nodes from traverser!" in str(e)
 
+
 def test_filter_sequence2():
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     runner = DagRunner(configuration)
 
     with pytest.raises(Exception) as e:
         runner.filter_sequence(["csv_reader", "junk!"])
     assert "Unknown key junk!" in str(e)
 
+
 def test_filter_sequence3():
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
                 "csv_reader": {
                     "class": "CsvReader",
                     "filename": "test/minimal.csv",
-                    "destinations": []
+                    "destinations": [],
                 }
             }
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     runner = DagRunner(configuration)
 
     with pytest.raises(Exception) as e:
         runner.filter_sequence([])
     assert "Ran out of nodes for section reader_config. Only received []" in str(e)
 
+
 def test_filter_sequence4():
     config = {
-        "metadata": {
-            "section_run": [
-                "writer_config"
-            ]
-        },
+        "metadata": {"section_run": ["writer_config"]},
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["recipe_csv_writer"]
+                    "destinations": ["recipe_csv_writer"],
                 }
             },
             "writer_config": {
                 "recipe_csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
+                    "filename": "unittest_similar_recipes.csv",
                 }
-            }
-        }
+            },
+        },
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     runner = DagRunner(configuration)
 
-    sequence = runner.filter_sequence(["read_data","recipe_csv_writer"])
+    sequence = runner.filter_sequence(["read_data", "recipe_csv_writer"])
     assert sequence == ["recipe_csv_writer"]
 
+
 def test_filter_sequence5():
     config = {
-        "metadata": {
-            "section_run": [
-                "writer_config",
-                "reader_config"
-            ]
-        },
+        "metadata": {"section_run": ["writer_config", "reader_config"]},
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["recipe_csv_writer","recipe_csv_writer2"]
+                    "destinations": ["recipe_csv_writer", "recipe_csv_writer2"],
                 }
             },
             "writer_config": {
                 "recipe_csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
+                    "filename": "unittest_similar_recipes.csv",
                 },
                 "recipe_csv_writer2": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
-                }
-            }
-        }
+                    "filename": "unittest_similar_recipes.csv",
+                },
+            },
+        },
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     runner = DagRunner(configuration)
     with pytest.raises(Exception) as e:
         runner.filter_sequence(["recipe_csv_writer", "read_data", "recipe_csv_writer2"])
-    assert "Traverser is mismatched with section writer_config. Expecting set ['recipe_csv_writer', 'recipe_csv_writer2']" in str(e)
+    assert (
+        "Traverser is mismatched with section writer_config. Expecting set ['recipe_csv_writer', 'recipe_csv_writer2']"
+        in str(e)
+    )
+
 
 def test_filter_sequence6():
-    #test of dependencies with a section
+    # test of dependencies with a section
     config = {
-        "metadata": {
-            "traverser": "DepthFirstTraverser"
-        },
+        "metadata": {"traverser": "DepthFirstTraverser"},
         "implementation_config": {
             "reader_config": {
                 "read_data1": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["csv_writer"]
+                    "destinations": ["csv_writer"],
                 },
                 "read_data2": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["csv_writer"]
+                    "destinations": ["csv_writer"],
                 },
                 "read_data3": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["read_data2"]
-                }
+                    "destinations": ["read_data2"],
+                },
             },
             "writer_config": {
                 "csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
+                    "filename": "unittest_similar_recipes.csv",
                 }
-            }
-        }
+            },
+        },
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     runner = DagRunner(configuration)
     s_in = ["read_data3", "read_data2", "read_data1", "csv_writer"]
     s_out = runner.filter_sequence(s_in)
     assert s_out == s_in
 
     with pytest.raises(Exception) as e:
-        runner.filter_sequence([ "read_data1", "csv_writer", "read_data3", "read_data2"])
+        runner.filter_sequence(["read_data1", "csv_writer", "read_data3", "read_data2"])
     assert "Upstream path found, from read_data3 to csv_writer" in str(e.value)
 
+
 def test_check_upstream():
     config = {
-        "metadata": {
-            "section_run": [
-                "reader_config",
-                "writer_config"
-            ]
-        },
+        "metadata": {"section_run": ["reader_config", "writer_config"]},
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["recipe_csv_writer","recipe_csv_writer2"]
+                    "destinations": ["recipe_csv_writer", "recipe_csv_writer2"],
                 }
             },
             "writer_config": {
                 "recipe_csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
+                    "filename": "unittest_similar_recipes.csv",
                 },
                 "recipe_csv_writer2": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
-                }
-            }
-        }
+                    "filename": "unittest_similar_recipes.csv",
+                },
+            },
+        },
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     runner = DagRunner(configuration)
-    assert runner.check_for_upstream(['read_data', 'recipe_csv_writer', 'recipe_csv_writer2']) == False
+    assert (
+        runner.check_for_upstream(
+            ["read_data", "recipe_csv_writer", "recipe_csv_writer2"]
+        )
+        == False
+    )
+
 
 def test_check_upstream2():
     config = {
-        "metadata": {
-            "section_run": [
-                "writer_config",
-                "reader_config"
-            ]
-        },
+        "metadata": {"section_run": ["writer_config", "reader_config"]},
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "test/tennis.csv",
-                    "destinations": ["recipe_csv_writer","recipe_csv_writer2"]
+                    "destinations": ["recipe_csv_writer", "recipe_csv_writer2"],
                 }
             },
             "writer_config": {
                 "recipe_csv_writer": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
+                    "filename": "unittest_similar_recipes.csv",
                 },
                 "recipe_csv_writer2": {
                     "class": "CsvWriter",
-                    "key":"test_data",
+                    "key": "test_data",
                     "dir": "cache",
-                    "filename": "unittest_similar_recipes.csv"
-                }
-            }
-        }
+                    "filename": "unittest_similar_recipes.csv",
+                },
+            },
+        },
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     runner = DagRunner(configuration)
     with pytest.raises(Exception) as e:
-        runner.check_for_upstream(['recipe_csv_writer2', 'read_data', 'recipe_csv_writer'])
+        runner.check_for_upstream(
+            ["recipe_csv_writer2", "read_data", "recipe_csv_writer"]
+        )
     assert "Upstream path found, from read_data to recipe_csv_writer2" in str(e.value)
 
 
 def test_run_bad():
     class TestWriterTmp(AbstractWriter):
         @staticmethod
         def necessary_config(node_config):
@@ -620,105 +654,115 @@
 
         def run(self, data_object):
             return data_object, False
 
     NodeFactory().register("TestWriterTmp", TestWriterTmp)
 
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "writer_config": {
-                "mywriter": {
-                    "class": "TestWriterTmp",
-                    "destinations": []
-                }
+                "mywriter": {"class": "TestWriterTmp", "destinations": []}
             }
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     runner = DagRunner(configuration)
 
     # unregister this class
     del NodeFactory().name_dict["TestWriterTmp"]
 
     with pytest.raises(Exception) as e:
         runner.run()
     assert "Issue instantiating mywriter and class TestWriterTmp" in str(e)
 
+
 def test_run_bad2():
     class TestWriterTmp(AbstractWriter):
         @staticmethod
         def necessary_config(node_config):
             return set([])
 
         def run(self, data_object):
             raise Exception("Deliberate error")
-            #return data_object, False
+            # return data_object, False
 
     NodeFactory().register("TestWriterTmp", TestWriterTmp)
 
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "writer_config": {
-                "mywriter": {
-                    "class": "TestWriterTmp",
-                    "destinations": []
-                }
+                "mywriter": {"class": "TestWriterTmp", "destinations": []}
             }
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
 
     runner = DagRunner(configuration)
 
     with pytest.raises(Exception) as e:
         runner.run()
     assert "Deliberate error" in str(e)
 
+
 def test_run_pruned():
     config = {
         "implementation_config": {
             "reader_config": {
                 "read_data": {
                     "class": "CsvReader",
                     "filename": "data/tennis.csv",
-                    "destinations": ["conditional_node"]
+                    "destinations": ["conditional_node"],
                 },
                 "conditional_node": {
                     "class": "SimpleSwitch",
                     "path_to_travel": "left",
-                    "destinations": ['left', 'right']
-                }
+                    "destinations": ["left", "right"],
+                },
             },
             "writer_config": {
                 "left": {
                     "class": "LoggingSuccess",
                     "msg": "left node!",
                     "level": "INFO",
                 },
                 "right": {
                     "class": "LoggingSuccess",
                     "msg": "right node!",
                     "level": "INFO",
-                    "destinations": ["right2"]
+                    "destinations": ["right2"],
                 },
                 "right2": {
                     "class": "LoggingSuccess",
                     "msg": "right node2!",
                     "level": "INFO",
-                }
-            }
+                },
+            },
         }
     }
     configuration = Configuration(None, is_dict_config=True, dict_config=config)
     runner = DagRunner(configuration)
     with LogCapture() as l:
         runner.run()
-    l.check(('root', 'INFO', 'Taking nodes to run from default'),
-            ('root', 'INFO', 'received node read_data of type reader_config and class CsvReader'),
-            ('root', 'INFO', 'Reading data/tennis.csv from CSV'),
-            ('root', 'INFO', 'received node conditional_node of type reader_config and class SimpleSwitch'),
-            ('root', 'INFO', 'Skipping pruned node right'),
-            ('root', 'INFO', 'Skipping pruned node right2'),
-            ('root', 'INFO', 'received node left of type writer_config and class LoggingSuccess'),
-            ('root', 'INFO', 'left node!'),
-            ('root', 'INFO', 'All done. Bye bye!'))
+    l.check(
+        ("root", "INFO", "Taking nodes to run from default"),
+        (
+            "root",
+            "INFO",
+            "received node read_data of type reader_config and class CsvReader",
+        ),
+        ("root", "INFO", "Reading data/tennis.csv from CSV"),
+        (
+            "root",
+            "INFO",
+            "received node conditional_node of type reader_config and class SimpleSwitch",
+        ),
+        ("root", "INFO", "Skipping pruned node right"),
+        ("root", "INFO", "Skipping pruned node right2"),
+        (
+            "root",
+            "INFO",
+            "received node left of type writer_config and class LoggingSuccess",
+        ),
+        ("root", "INFO", "left node!"),
+        ("root", "INFO", "All done. Bye bye!"),
+    )
```

### Comparing `primrose-1.0.9/test/test_csv_reader.py` & `primrose-2.0.0/test/test_csv_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 import pytest
 from primrose.configuration.configuration import Configuration
 from primrose.readers.csv_reader import CsvReader
 from primrose.data_object import DataObject, DataObjectResponseType
 
+
 def test_init_ok():
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
-            "csv_reader": {
-                "class": "CsvReader",
-                "filename": "test/minimal.csv",
-                "destinations": []
+                "csv_reader": {
+                    "class": "CsvReader",
+                    "filename": "test/minimal.csv",
+                    "destinations": [],
                 }
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     data_object = DataObject(configuration)
 
     reader = CsvReader(configuration, "csv_reader")
     data_object, terminate = reader.run(data_object)
     assert not terminate
-    df = data_object.get('csv_reader', rtype=DataObjectResponseType.VALUE.value)
+    df = data_object.get("csv_reader", rtype=DataObjectResponseType.VALUE.value)
     assert df is not None
     assert df.shape == (2, 2)
 
     node_config = {
-                "class": "CsvReader",
-                "filename": "test/minimal.csv",
-                "destinations": []
-                }
+        "class": "CsvReader",
+        "filename": "test/minimal.csv",
+        "destinations": [],
+    }
 
     assert isinstance(CsvReader.necessary_config(node_config), set)
     assert len(CsvReader.necessary_config(node_config)) > 0
 
 
 def test_kwargs():
     config = {
-        "implementation_config":{
+        "implementation_config": {
             "reader_config": {
-            "csv_reader": {
-                "class": "CsvReader",
-                "filename": "test/minimal.csv",
-                "kwargs": {
-                    "header": None,
-                    "sep": ":"
-                },
-                "destinations": []
+                "csv_reader": {
+                    "class": "CsvReader",
+                    "filename": "test/minimal.csv",
+                    "kwargs": {"header": None, "sep": ":"},
+                    "destinations": [],
                 }
             }
         }
     }
-    configuration = Configuration(config_location=None, is_dict_config=True, dict_config=config)
+    configuration = Configuration(
+        config_location=None, is_dict_config=True, dict_config=config
+    )
     data_object = DataObject(configuration)
 
     reader = CsvReader(configuration, "csv_reader")
     data_object, terminate = reader.run(data_object)
     assert not terminate
-    df = data_object.get('csv_reader', rtype=DataObjectResponseType.VALUE.value)
+    df = data_object.get("csv_reader", rtype=DataObjectResponseType.VALUE.value)
     assert df is not None
     assert df.shape == (3, 1)
```

### Comparing `primrose-1.0.9/config/hello_world_classifier_predict.yml` & `primrose-2.0.0/config/hello_world_classifier_predict.yml`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/config/hello_world_read_write.json` & `primrose-2.0.0/config/hello_world_read_write.json`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/config/hello_world_cluster_simple_train.yml` & `primrose-2.0.0/config/hello_world_cluster_simple_train.yml`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/config/hello_world_cluster_eval.json` & `primrose-2.0.0/config/hello_world_cluster_eval.json`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/config/hello_world_cluster_train.json` & `primrose-2.0.0/config/hello_world_cluster_train.json`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/config/hello_world_classifier_predict.json` & `primrose-2.0.0/config/hello_world_classifier_predict.json`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/config/hello_world_regression_train.yml` & `primrose-2.0.0/config/hello_world_regression_train.yml`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/config/hello_world_classifier_train.json` & `primrose-2.0.0/config/hello_world_classifier_train.json`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/config/hello_world_classifier_train.yml` & `primrose-2.0.0/config/hello_world_classifier_train.yml`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/config/hello_world_regression_train.json` & `primrose-2.0.0/config/hello_world_regression_train.json`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/config/hello_world_cluster_simple_train.json` & `primrose-2.0.0/config/hello_world_cluster_simple_train.json`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/config/hello_world_custom_nodes.json` & `primrose-2.0.0/config/hello_world_custom_nodes.json`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/config/hello_world_cluster_train.yml` & `primrose-2.0.0/config/hello_world_cluster_train.yml`

 * *Files identical despite different names*

### Comparing `primrose-1.0.9/config/hello_world_cluster_eval.yml` & `primrose-2.0.0/config/hello_world_cluster_eval.yml`

 * *Files identical despite different names*

