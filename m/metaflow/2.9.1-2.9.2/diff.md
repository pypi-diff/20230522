# Comparing `tmp/metaflow-2.9.1.tar.gz` & `tmp/metaflow-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-2.9.1.tar", last modified: Tue May 16 03:15:05 2023, max compression
+gzip compressed data, was "metaflow-2.9.2.tar", last modified: Mon May 22 17:27:09 2023, max compression
```

## Comparing `metaflow-2.9.1.tar` & `metaflow-2.9.2.tar`

### file list

```diff
@@ -1,334 +1,334 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.565020 metaflow-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-16 03:14:53.000000 metaflow-2.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-16 03:14:53.000000 metaflow-2.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-16 03:15:05.565020 metaflow-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-16 03:14:53.000000 metaflow-2.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.541020 metaflow-2.9.1/metaflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/R.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.541020 metaflow-2.9.1/metaflow/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.541020 metaflow-2.9.1/metaflow/_vendor/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/_bashcomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/_termui_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/_textwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/_unicodefun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/_winconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.541020 metaflow-2.9.1/metaflow/_vendor/v3_5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.541020 metaflow-2.9.1/metaflow/_vendor/v3_5/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_5/zipp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.545020 metaflow-2.9.1/metaflow/_vendor/v3_6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.545020 metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_6/typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/_vendor/v3_6/zipp.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.545020 metaflow-2.9.1/metaflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69157 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/client/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/client/filecache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.545020 metaflow-2.9.1/metaflow/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32848 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/cmd/configure_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/cmd/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/cmd/tutorials_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/cmd/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/cmd_with_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.545020 metaflow-2.9.1/metaflow/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/datastore/content_addressed_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/datastore/datastore_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/datastore/datastore_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/datastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/datastore/flow_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/datastore/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/datastore/task_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/event_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.545020 metaflow-2.9.1/metaflow/extension_support/
--rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/extension_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/extension_support/_empty_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/extension_support/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/extension_support/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/extension_support/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/flowspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/includefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.545020 metaflow-2.9.1/metaflow/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/metadata/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/metadata/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/metaflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/metaflow_config_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/metaflow_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/metaflow_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/metaflow_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.549020 metaflow-2.9.1/metaflow/mflog/
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/mflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/mflog/mflog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/mflog/save_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/mflog/save_logs_periodically.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/mflog/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/multicore_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.549020 metaflow-2.9.1/metaflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.549020 metaflow-2.9.1/metaflow/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/airflow/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/airflow/airflow_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/airflow/airflow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/airflow/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/airflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/airflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.549020 metaflow-2.9.1/metaflow/plugins/airflow/plumbing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/airflow/plumbing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/airflow/plumbing/set_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.549020 metaflow-2.9.1/metaflow/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/airflow/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/airflow/sensors/base_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/airflow/sensors/external_task_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/airflow/sensors/s3_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.553020 metaflow-2.9.1/metaflow/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/argo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/argo/argo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/argo/argo_events.py
--rw-r--r--   0 runner    (1001) docker     (123)   103729 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/argo/argo_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    20011 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/argo/argo_workflows_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/argo/argo_workflows_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/argo/process_input_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.553020 metaflow-2.9.1/metaflow/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/aws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.553020 metaflow-2.9.1/metaflow/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/batch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/batch/batch_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/batch/batch_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/batch/batch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.553020 metaflow-2.9.1/metaflow/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/secrets_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.553020 metaflow-2.9.1/metaflow/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/step_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/step_functions/dynamo_db_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/step_functions/event_bridge_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/step_functions/production_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/step_functions/schedule_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/step_functions/set_batch_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/step_functions/step_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/step_functions/step_functions_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/step_functions/step_functions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/aws/step_functions/step_functions_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.553020 metaflow-2.9.1/metaflow/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/azure/azure_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/azure/azure_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/azure/azure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/azure/blob_service_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/azure/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.553020 metaflow-2.9.1/metaflow/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.557020 metaflow-2.9.1/metaflow/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.557020 metaflow-2.9.1/metaflow/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/chevron/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/chevron/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/chevron/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/chevron/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/convert_to_native_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/renderer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_modules/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/card_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/component_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/cards/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/catch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.557020 metaflow-2.9.1/metaflow/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/conda/batch_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/conda/conda_step_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.557020 metaflow-2.9.1/metaflow/plugins/datastores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/datastores/azure_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/datastores/gs_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/datastores/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/datastores/s3_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.557020 metaflow-2.9.1/metaflow/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/datatools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/datatools/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.557020 metaflow-2.9.1/metaflow/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/datatools/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62975 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/datatools/s3/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/datatools/s3/s3op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/datatools/s3/s3tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/datatools/s3/s3util.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/debug_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/debug_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.561020 metaflow-2.9.1/metaflow/plugins/env_escape/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/client_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.561020 metaflow-2.9.1/metaflow/plugins/env_escape/communication/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/communication/bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/communication/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/communication/socket_bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/communication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.561020 metaflow-2.9.1/metaflow/plugins/env_escape/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.561020 metaflow-2.9.1/metaflow/plugins/env_escape/configurations/emulate_test_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.561020 metaflow-2.9.1/metaflow/plugins/env_escape/configurations/test_lib_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/data_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/exception_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/override_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/env_escape/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/environment_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/events_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.561020 metaflow-2.9.1/metaflow/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/frameworks/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.561020 metaflow-2.9.1/metaflow/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/gcp/gs_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/gcp/gs_storage_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/gcp/gs_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/gcp/gs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/gcp/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.561020 metaflow-2.9.1/metaflow/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/kubernetes/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/kubernetes/kubernetes_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/kubernetes/kubernetes_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19778 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/kubernetes/kubernetes_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27804 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/kubernetes/kubernetes_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.561020 metaflow-2.9.1/metaflow/plugins/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/metadata/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/metadata/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/package_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/parallel_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/project_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/resources_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/retry_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.561020 metaflow-2.9.1/metaflow/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/secrets/inline_secrets_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/secrets/secrets_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/storage_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/tag_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/test_unbounded_foreach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/plugins/timeout_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/procpoll.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/pylint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.561020 metaflow-2.9.1/metaflow/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/sidecar/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/sidecar/sidecar_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/sidecar/sidecar_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/sidecar/sidecar_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tagging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.537020 metaflow-2.9.1/metaflow/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.561020 metaflow-2.9.1/metaflow/tutorials/00-helloworld/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/00-helloworld/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/00-helloworld/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.565020 metaflow-2.9.1/metaflow/tutorials/01-playlist/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/01-playlist/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/01-playlist/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/01-playlist/playlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/01-playlist/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.565020 metaflow-2.9.1/metaflow/tutorials/02-statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/02-statistics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/02-statistics/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/02-statistics/stats.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/02-statistics/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.565020 metaflow-2.9.1/metaflow/tutorials/03-playlist-redux/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/03-playlist-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/03-playlist-redux/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.565020 metaflow-2.9.1/metaflow/tutorials/04-playlist-plus/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/04-playlist-plus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/04-playlist-plus/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.565020 metaflow-2.9.1/metaflow/tutorials/05-hello-cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/05-hello-cloud/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/05-hello-cloud/hello-cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.565020 metaflow-2.9.1/metaflow/tutorials/06-statistics-redux/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/06-statistics-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/06-statistics-redux/stats.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.565020 metaflow-2.9.1/metaflow/tutorials/07-worldview/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/07-worldview/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/07-worldview/worldview.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.565020 metaflow-2.9.1/metaflow/tutorials/08-autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/08-autopilot/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/tutorials/08-autopilot/autopilot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/unbounded_foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-16 03:14:53.000000 metaflow-2.9.1/metaflow/vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:15:05.541020 metaflow-2.9.1/metaflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-16 03:15:05.000000 metaflow-2.9.1/metaflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-16 03:15:05.000000 metaflow-2.9.1/metaflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 03:15:05.000000 metaflow-2.9.1/metaflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 03:15:05.000000 metaflow-2.9.1/metaflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 03:15:05.000000 metaflow-2.9.1/metaflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 03:15:05.000000 metaflow-2.9.1/metaflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 03:15:05.565020 metaflow-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-16 03:14:53.000000 metaflow-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-22 17:26:56.000000 metaflow-2.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 17:26:56.000000 metaflow-2.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-05-22 17:27:09.194964 metaflow-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-22 17:26:56.000000 metaflow-2.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.162963 metaflow-2.9.2/metaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/R.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.162963 metaflow-2.9.2/metaflow/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.166963 metaflow-2.9.2/metaflow/_vendor/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/_bashcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/_unicodefun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.166963 metaflow-2.9.2/metaflow/_vendor/v3_5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.166963 metaflow-2.9.2/metaflow/_vendor/v3_5/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_5/zipp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.166963 metaflow-2.9.2/metaflow/_vendor/v3_6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.166963 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/_vendor/v3_6/zipp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.166963 metaflow-2.9.2/metaflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69283 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/client/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/client/filecache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.170963 metaflow-2.9.2/metaflow/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33396 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cmd/configure_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cmd/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cmd/tutorials_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cmd/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/cmd_with_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.170963 metaflow-2.9.2/metaflow/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/content_addressed_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/datastore_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/datastore_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/flow_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/datastore/task_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/event_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.170963 metaflow-2.9.2/metaflow/extension_support/
+-rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/extension_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/extension_support/_empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/extension_support/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/extension_support/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/extension_support/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/flowspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19721 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/includefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.170963 metaflow-2.9.2/metaflow/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metadata/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metadata/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18629 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metaflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metaflow_config_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metaflow_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metaflow_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/metaflow_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.170963 metaflow-2.9.2/metaflow/mflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/mflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/mflog/mflog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/mflog/save_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/mflog/save_logs_periodically.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/mflog/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/multicore_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31438 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/airflow_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/airflow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/airflow/plumbing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/plumbing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/plumbing/set_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/sensors/base_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/sensors/external_task_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/airflow/sensors/s3_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/argo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/argo_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103837 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/argo_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20011 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/argo_workflows_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/argo_workflows_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/argo/process_input_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/aws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/batch/batch_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/batch/batch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/batch/batch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.174963 metaflow-2.9.2/metaflow/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.178964 metaflow-2.9.2/metaflow/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/dynamo_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/event_bridge_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/production_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/schedule_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/set_batch_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.178964 metaflow-2.9.2/metaflow/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/azure/azure_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/azure/azure_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/azure/azure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/azure/blob_service_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/azure/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.178964 metaflow-2.9.2/metaflow/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.182963 metaflow-2.9.2/metaflow/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.182963 metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/convert_to_native_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/renderer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_modules/test_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/card_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/component_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/cards/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/catch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.182963 metaflow-2.9.2/metaflow/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/conda/batch_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/conda/conda_step_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.182963 metaflow-2.9.2/metaflow/plugins/datastores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datastores/azure_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datastores/gs_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datastores/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datastores/s3_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.182963 metaflow-2.9.2/metaflow/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.182963 metaflow-2.9.2/metaflow/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62975 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/s3/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/s3/s3op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/s3/s3tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/datatools/s3/s3util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/debug_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/debug_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/env_escape/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/client_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/env_escape/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/communication/bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/communication/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/communication/socket_bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/communication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/test_lib_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/data_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/exception_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/override_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/env_escape/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/environment_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/events_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/frameworks/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/gcp/gs_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/gcp/gs_storage_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/gcp/gs_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/gcp/gs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/gcp/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.186964 metaflow-2.9.2/metaflow/plugins/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/metadata/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/metadata/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/package_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/parallel_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/project_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/resources_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/retry_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/secrets/inline_secrets_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/secrets/secrets_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/storage_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/tag_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/test_unbounded_foreach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/plugins/timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/procpoll.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/pylint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/sidecar/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/sidecar/sidecar_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/sidecar/sidecar_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/sidecar/sidecar_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tagging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.158963 metaflow-2.9.2/metaflow/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/00-helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/00-helloworld/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/00-helloworld/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/01-playlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/01-playlist/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/01-playlist/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/01-playlist/playlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/01-playlist/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/02-statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/02-statistics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/02-statistics/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/02-statistics/stats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/02-statistics/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/03-playlist-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/03-playlist-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/03-playlist-redux/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/04-playlist-plus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/04-playlist-plus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/04-playlist-plus/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/hello-cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/06-statistics-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/06-statistics-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/06-statistics-redux/stats.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/07-worldview/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/07-worldview/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/07-worldview/worldview.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.190964 metaflow-2.9.2/metaflow/tutorials/08-autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/08-autopilot/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/tutorials/08-autopilot/autopilot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/unbounded_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-22 17:26:56.000000 metaflow-2.9.2/metaflow/vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:09.162963 metaflow-2.9.2/metaflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-05-22 17:27:09.000000 metaflow-2.9.2/metaflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-22 17:27:09.000000 metaflow-2.9.2/metaflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:27:09.000000 metaflow-2.9.2/metaflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 17:27:09.000000 metaflow-2.9.2/metaflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 17:27:09.000000 metaflow-2.9.2/metaflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 17:27:09.000000 metaflow-2.9.2/metaflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 17:27:09.194964 metaflow-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-22 17:26:56.000000 metaflow-2.9.2/setup.py
```

### Comparing `metaflow-2.9.1/LICENSE` & `metaflow-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/R.py` & `metaflow-2.9.2/metaflow/R.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/__init__.py` & `metaflow-2.9.2/metaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/__init__.py` & `metaflow-2.9.2/metaflow/_vendor/click/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/_bashcomplete.py` & `metaflow-2.9.2/metaflow/_vendor/click/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/_compat.py` & `metaflow-2.9.2/metaflow/_vendor/click/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/_termui_impl.py` & `metaflow-2.9.2/metaflow/_vendor/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/_textwrap.py` & `metaflow-2.9.2/metaflow/_vendor/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/_unicodefun.py` & `metaflow-2.9.2/metaflow/_vendor/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/_winconsole.py` & `metaflow-2.9.2/metaflow/_vendor/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/core.py` & `metaflow-2.9.2/metaflow/_vendor/click/core.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/decorators.py` & `metaflow-2.9.2/metaflow/_vendor/click/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/exceptions.py` & `metaflow-2.9.2/metaflow/_vendor/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/formatting.py` & `metaflow-2.9.2/metaflow/_vendor/click/formatting.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/globals.py` & `metaflow-2.9.2/metaflow/_vendor/click/globals.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/parser.py` & `metaflow-2.9.2/metaflow/_vendor/click/parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/termui.py` & `metaflow-2.9.2/metaflow/_vendor/click/termui.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/testing.py` & `metaflow-2.9.2/metaflow/_vendor/click/testing.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/types.py` & `metaflow-2.9.2/metaflow/_vendor/click/types.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/click/utils.py` & `metaflow-2.9.2/metaflow/_vendor/click/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/v3_5/importlib_metadata/__init__.py` & `metaflow-2.9.2/metaflow/_vendor/v3_5/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/v3_5/importlib_metadata/_compat.py` & `metaflow-2.9.2/metaflow/_vendor/v3_5/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/v3_5/zipp.py` & `metaflow-2.9.2/metaflow/_vendor/v3_5/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/__init__.py` & `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py` & `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_collections.py` & `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_compat.py` & `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_functools.py` & `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py` & `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_meta.py` & `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/v3_6/importlib_metadata/_text.py` & `metaflow-2.9.2/metaflow/_vendor/v3_6/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/v3_6/typing_extensions.py` & `metaflow-2.9.2/metaflow/_vendor/v3_6/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/_vendor/v3_6/zipp.py` & `metaflow-2.9.2/metaflow/_vendor/v3_6/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/cli.py` & `metaflow-2.9.2/metaflow/cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/cli_args.py` & `metaflow-2.9.2/metaflow/cli_args.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/client/core.py` & `metaflow-2.9.2/metaflow/client/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1705,14 +1705,16 @@
         True if the run completed successfully.
     finished : bool
         True if the run completed.
     finished_at : datetime
         Time this run finished.
     code : MetaflowCode
         Code package for this run (if present). See `MetaflowCode`.
+    trigger : MetaflowTrigger
+        Information about event(s) that triggered this run (if present). See `MetaflowTrigger`.
     end_task : Task
         `Task` for the end step (if it is present already).
     """
 
     _NAME = "run"
     _PARENT_CLASS = "flow"
     _CHILD_CLASS = "step"
```

### Comparing `metaflow-2.9.1/metaflow/client/filecache.py` & `metaflow-2.9.2/metaflow/client/filecache.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/cmd/configure_cmd.py` & `metaflow-2.9.2/metaflow/cmd/configure_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -584,48 +584,61 @@
 
 def configure_argo_events(existing_env):
     env = {}
 
     # Argo events service account
     env["METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT"] = click.prompt(
         cyan("[METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT]")
-        + " Argo events service account ",
+        + " Service Account for Argo Events. ",
         default=existing_env.get("METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT", ""),
         show_default=True,
     )
 
     # Argo events event bus
     env["METAFLOW_ARGO_EVENTS_EVENT_BUS"] = click.prompt(
         cyan("[METAFLOW_ARGO_EVENTS_EVENT_BUS]")
         + yellow(" (optional)")
-        + " Argo events event bus ",
+        + " Event Bus for Argo Events.",
         default=existing_env.get("METAFLOW_ARGO_EVENTS_EVENT_BUS", "default"),
         show_default=True,
     )
 
     # Argo events event source
     env["METAFLOW_ARGO_EVENTS_EVENT_SOURCE"] = click.prompt(
-        cyan("[METAFLOW_ARGO_EVENTS_EVENT_SOURCE]") + " Argo events event source ",
+        cyan("[METAFLOW_ARGO_EVENTS_EVENT_SOURCE]") + " Event Source for Argo Events.",
         default=existing_env.get("METAFLOW_ARGO_EVENTS_EVENT_SOURCE", ""),
         show_default=True,
     )
 
     # Argo events event name
     env["METAFLOW_ARGO_EVENTS_EVENT"] = click.prompt(
-        cyan("[METAFLOW_ARGO_EVENTS_EVENT]") + " Argo events event ",
+        cyan("[METAFLOW_ARGO_EVENTS_EVENT]") + " Event name for Argo Events.",
         default=existing_env.get("METAFLOW_ARGO_EVENTS_EVENT", ""),
         show_default=True,
     )
 
     # Argo events webhook url
     env["METAFLOW_ARGO_EVENTS_WEBHOOK_URL"] = click.prompt(
-        cyan("[METAFLOW_ARGO_EVENTS_WEBHOOK_URL]") + " Argo events webhook url ",
+        cyan("[METAFLOW_ARGO_EVENTS_WEBHOOK_URL]")
+        + " Publicly accessible URL for Argo Events Webhook.",
         default=existing_env.get("METAFLOW_ARGO_EVENTS_WEBHOOK_URL", ""),
         show_default=True,
     )
+    # Set internal URL for Argo events webhook
+    env["METAFLOW_ARGO_EVENTS_INTERNAL_WEBHOOK_URL"] = click.prompt(
+        cyan("[METAFLOW_ARGO_EVENTS_INTERNAL_WEBHOOK_URL]")
+        + yellow(" (optional)")
+        + " URL for Argo Events Webhook "
+        + "(Accessible only within a Kubernetes cluster).",
+        default=existing_env.get(
+            "METAFLOW_ARGO_EVENTS_INTERNAL_WEBHOOK_URL",
+            env["METAFLOW_ARGO_EVENTS_WEBHOOK_URL"],
+        ),
+        show_default=True,
+    )
 
     return env
 
 
 def configure_kubernetes(existing_env):
     empty_profile = False
     if not existing_env:
@@ -768,15 +781,14 @@
     "-p",
     default="",
     help="Configure a named profile. Activate the profile by setting "
     "`METAFLOW_PROFILE` environment variable.",
 )
 @click.pass_context
 def azure(ctx, profile):
-
     # Greet the user!
     echo(
         "Welcome to Metaflow! Follow the prompts to configure your installation.\n",
         bold=True,
     )
 
     # Check for existing configuration.
@@ -810,15 +822,14 @@
     "-p",
     default="",
     help="Configure a named profile. Activate the profile by setting "
     "`METAFLOW_PROFILE` environment variable.",
 )
 @click.pass_context
 def gcp(ctx, profile):
-
     # Greet the user!
     echo(
         "Welcome to Metaflow! Follow the prompts to configure your installation.\n",
         bold=True,
     )
 
     # Check for existing configuration.
@@ -852,15 +863,14 @@
     "-p",
     default="",
     help="Configure a named profile. Activate the profile by setting "
     "`METAFLOW_PROFILE` environment variable.",
 )
 @click.pass_context
 def aws(ctx, profile):
-
     # Greet the user!
     echo(
         "Welcome to Metaflow! Follow the prompts to configure your " "installation.\n",
         bold=True,
     )
 
     # Check for existing configuration.
@@ -900,15 +910,14 @@
     "-p",
     default="",
     help="Configure a named profile. Activate the profile by setting "
     "`METAFLOW_PROFILE` environment variable.",
 )
 @click.pass_context
 def kubernetes(ctx, profile):
-
     check_kubernetes_client(ctx)
 
     # Greet the user!
     echo(
         "Welcome to Metaflow! Follow the prompts to configure your " "installation.\n",
         bold=True,
     )
```

### Comparing `metaflow-2.9.1/metaflow/cmd/main_cli.py` & `metaflow-2.9.2/metaflow/cmd/main_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/cmd/tutorials_cmd.py` & `metaflow-2.9.2/metaflow/cmd/tutorials_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/cmd_with_io.py` & `metaflow-2.9.2/metaflow/cmd_with_io.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/current.py` & `metaflow-2.9.2/metaflow/current.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/datastore/content_addressed_store.py` & `metaflow-2.9.2/metaflow/datastore/content_addressed_store.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/datastore/datastore_set.py` & `metaflow-2.9.2/metaflow/datastore/datastore_set.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/datastore/datastore_storage.py` & `metaflow-2.9.2/metaflow/datastore/datastore_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/datastore/flow_datastore.py` & `metaflow-2.9.2/metaflow/datastore/flow_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/datastore/task_datastore.py` & `metaflow-2.9.2/metaflow/datastore/task_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/debug.py` & `metaflow-2.9.2/metaflow/debug.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/decorators.py` & `metaflow-2.9.2/metaflow/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/event_logger.py` & `metaflow-2.9.2/metaflow/event_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/events.py` & `metaflow-2.9.2/metaflow/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -134,15 +134,21 @@
                 if obj.type == "run"
             ]
 
         return list(self._runs) or None
 
     def __getitem__(self, key):
         """
-        If triggering events are runs, `key` corresponds to the flow name of the triggering run. Returns a triggering `Run` object corresponding to the key. If triggering events are not runs, `key` corresponds to the event name and a `MetaflowEvent` object is returned.
+        If triggering events are runs, `key` corresponds to the flow name of the triggering run.
+        Otherwise, `key` corresponds to the event name and a `MetaflowEvent` object is returned.
+
+        Returns
+        -------
+        Run or MetaflowEvent
+            `Run` object if triggered by a run. Otherwise returns a `MetaflowEvent`.
         """
         if self.runs:
             for run in self.runs:
                 if run.path_components[0] == key:
                     return run
         elif self.events:
             for event in self.events:
```

### Comparing `metaflow-2.9.1/metaflow/exception.py` & `metaflow-2.9.2/metaflow/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/extension_support/__init__.py` & `metaflow-2.9.2/metaflow/extension_support/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/extension_support/cmd.py` & `metaflow-2.9.2/metaflow/extension_support/cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/extension_support/integrations.py` & `metaflow-2.9.2/metaflow/extension_support/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/extension_support/plugins.py` & `metaflow-2.9.2/metaflow/extension_support/plugins.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/flowspec.py` & `metaflow-2.9.2/metaflow/flowspec.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/graph.py` & `metaflow-2.9.2/metaflow/graph.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/includefile.py` & `metaflow-2.9.2/metaflow/includefile.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,18 +140,21 @@
                 flow_name=ctx.obj.flow.name,
                 user_name=get_username(),
                 parameter_name=param.name,
                 logger=ctx.obj.echo,
                 ds_type=ctx.obj.datastore_impl.TYPE,
             )
 
-        if len(value) > 0 and value[0] == "{":
+        if len(value) > 0 and (value.startswith("{") or value.startswith('"{')):
             # This is a blob; no URL starts with `{`. We are thus in scenario A
             try:
                 value = json.loads(value)
+                # to handle quoted json strings
+                if not isinstance(value, dict):
+                    value = json.loads(value)
             except json.JSONDecodeError as e:
                 raise MetaflowException(
                     "IncludeFile '%s' (value: %s) is malformed" % (param.name, value)
                 )
             # All processing has already been done, so we just convert to an `IncludedFile`
             return IncludedFile(value)
 
@@ -425,15 +428,14 @@
         handler = DATACLIENTS.get(prefix)
         if handler is None:
             raise MetaflowException("Could not find data client for '%s'" % prefix)
         return handler
 
 
 class UploaderV2:
-
     file_type = "uploader-v2"
 
     @classmethod
     def encode_url(cls, url_type, url, **kwargs):
         return_value = {
             "note": "Internal representation of IncludeFile(%s)" % url,
             "type": cls.file_type,
```

### Comparing `metaflow-2.9.1/metaflow/integrations.py` & `metaflow-2.9.2/metaflow/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/lint.py` & `metaflow-2.9.2/metaflow/lint.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/metadata/heartbeat.py` & `metaflow-2.9.2/metaflow/metadata/heartbeat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/metadata/metadata.py` & `metaflow-2.9.2/metaflow/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/metadata/util.py` & `metaflow-2.9.2/metaflow/metadata/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/metaflow_config.py` & `metaflow-2.9.2/metaflow/metaflow_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,14 +279,16 @@
 KUBERNETES_SECRETS = from_conf("KUBERNETES_SECRETS", "")
 # Default GPU vendor to use by K8S jobs created by Metaflow (supports nvidia, amd)
 KUBERNETES_GPU_VENDOR = from_conf("KUBERNETES_GPU_VENDOR", "nvidia")
 # Default container image for K8S
 KUBERNETES_CONTAINER_IMAGE = from_conf(
     "KUBERNETES_CONTAINER_IMAGE", DEFAULT_CONTAINER_IMAGE
 )
+# Image pull policy for container images
+KUBERNETES_IMAGE_PULL_POLICY = from_conf("KUBERNETES_IMAGE_PULL_POLICY", None)
 # Default container registry for K8S
 KUBERNETES_CONTAINER_REGISTRY = from_conf(
     "KUBERNETES_CONTAINER_REGISTRY", DEFAULT_CONTAINER_REGISTRY
 )
 # Toggle for trying to fetch EC2 instance metadata
 KUBERNETES_FETCH_EC2_METADATA = from_conf("KUBERNETES_FETCH_EC2_METADATA", False)
 
@@ -297,14 +299,17 @@
 # Argo Events Configuration
 ##
 ARGO_EVENTS_SERVICE_ACCOUNT = from_conf("ARGO_EVENTS_SERVICE_ACCOUNT")
 ARGO_EVENTS_EVENT_BUS = from_conf("ARGO_EVENTS_EVENT_BUS", "default")
 ARGO_EVENTS_EVENT_SOURCE = from_conf("ARGO_EVENTS_EVENT_SOURCE")
 ARGO_EVENTS_EVENT = from_conf("ARGO_EVENTS_EVENT")
 ARGO_EVENTS_WEBHOOK_URL = from_conf("ARGO_EVENTS_WEBHOOK_URL")
+ARGO_EVENTS_INTERNAL_WEBHOOK_URL = from_conf(
+    "ARGO_EVENTS_INTERNAL_WEBHOOK_URL", ARGO_EVENTS_WEBHOOK_URL
+)
 
 ARGO_WORKFLOWS_UI_URL = from_conf("ARGO_WORKFLOWS_UI_URL")
 
 ##
 # Airflow Configuration
 ##
 # This configuration sets `startup_timeout_seconds` in airflow's KubernetesPodOperator.
```

### Comparing `metaflow-2.9.1/metaflow/metaflow_config_funcs.py` & `metaflow-2.9.2/metaflow/metaflow_config_funcs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/metaflow_environment.py` & `metaflow-2.9.2/metaflow/metaflow_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/metaflow_version.py` & `metaflow-2.9.2/metaflow/metaflow_version.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/mflog/__init__.py` & `metaflow-2.9.2/metaflow/mflog/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/mflog/mflog.py` & `metaflow-2.9.2/metaflow/mflog/mflog.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/mflog/save_logs.py` & `metaflow-2.9.2/metaflow/mflog/save_logs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/mflog/save_logs_periodically.py` & `metaflow-2.9.2/metaflow/mflog/save_logs_periodically.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/mflog/tee.py` & `metaflow-2.9.2/metaflow/mflog/tee.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/monitor.py` & `metaflow-2.9.2/metaflow/monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/multicore_utils.py` & `metaflow-2.9.2/metaflow/multicore_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/package.py` & `metaflow-2.9.2/metaflow/package.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/parameters.py` & `metaflow-2.9.2/metaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/__init__.py` & `metaflow-2.9.2/metaflow/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/airflow/airflow.py` & `metaflow-2.9.2/metaflow/plugins/airflow/airflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,18 +638,23 @@
             kube_deco = dict(
                 [deco for deco in node.decorators if deco.name == "kubernetes"][
                     0
                 ].attributes
             )
             if kube_deco:
                 # Only guard against use_tmpfs and tmpfs_size as these determine if tmpfs is enabled.
-                for attr in ["use_tmpfs", "tmpfs_size", "persistent_volume_claims"]:
+                for attr in [
+                    "use_tmpfs",
+                    "tmpfs_size",
+                    "persistent_volume_claims",
+                    "image_pull_policy",
+                ]:
                     if kube_deco[attr]:
                         raise AirflowException(
-                            "tmpfs attribute *%s* is currently not supported on Airflow "
+                            "The decorator attribute *%s* is currently not supported on Airflow "
                             "for the @kubernetes decorator on step *%s*"
                             % (attr, node.name)
                         )
 
             parent_is_foreach = any(  # Any immediate parent is a foreach node.
                 self.graph[n].type == "foreach" for n in node.in_funcs
             )
```

### Comparing `metaflow-2.9.1/metaflow/plugins/airflow/airflow_cli.py` & `metaflow-2.9.2/metaflow/plugins/airflow/airflow_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/airflow/airflow_decorator.py` & `metaflow-2.9.2/metaflow/plugins/airflow/airflow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/airflow/airflow_utils.py` & `metaflow-2.9.2/metaflow/plugins/airflow/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/airflow/plumbing/set_parameters.py` & `metaflow-2.9.2/metaflow/plugins/airflow/plumbing/set_parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/airflow/sensors/base_sensor.py` & `metaflow-2.9.2/metaflow/plugins/airflow/sensors/base_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/airflow/sensors/external_task_sensor.py` & `metaflow-2.9.2/metaflow/plugins/airflow/sensors/external_task_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/airflow/sensors/s3_sensor.py` & `metaflow-2.9.2/metaflow/plugins/airflow/sensors/s3_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/argo/argo_client.py` & `metaflow-2.9.2/metaflow/plugins/argo/argo_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/argo/argo_workflows.py` & `metaflow-2.9.2/metaflow/plugins/argo/argo_workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from metaflow.decorators import flow_decorators
 from metaflow.exception import MetaflowException
 from metaflow.metaflow_config import (
     ARGO_EVENTS_EVENT,
     ARGO_EVENTS_EVENT_BUS,
     ARGO_EVENTS_EVENT_SOURCE,
     ARGO_EVENTS_SERVICE_ACCOUNT,
-    ARGO_EVENTS_WEBHOOK_URL,
+    ARGO_EVENTS_INTERNAL_WEBHOOK_URL,
     ARGO_WORKFLOWS_ENV_VARS_TO_SKIP,
     ARGO_WORKFLOWS_KUBERNETES_SECRETS,
     AWS_SECRETS_MANAGER_DEFAULT_REGION,
     AZURE_STORAGE_BLOB_SERVICE_ENDPOINT,
     CARD_AZUREROOT,
     CARD_GSROOT,
     CARD_S3ROOT,
@@ -1029,15 +1029,15 @@
                     **{
                         # Configuration for Argo Events. Keep these in sync with the
                         # environment variables for @kubernetes decorator.
                         "METAFLOW_ARGO_EVENTS_EVENT": ARGO_EVENTS_EVENT,
                         "METAFLOW_ARGO_EVENTS_EVENT_BUS": ARGO_EVENTS_EVENT_BUS,
                         "METAFLOW_ARGO_EVENTS_EVENT_SOURCE": ARGO_EVENTS_EVENT_SOURCE,
                         "METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT": ARGO_EVENTS_SERVICE_ACCOUNT,
-                        "METAFLOW_ARGO_EVENTS_WEBHOOK_URL": ARGO_EVENTS_WEBHOOK_URL,
+                        "METAFLOW_ARGO_EVENTS_WEBHOOK_URL": ARGO_EVENTS_INTERNAL_WEBHOOK_URL,
                     },
                     **{
                         # Some optional values for bookkeeping
                         "METAFLOW_FLOW_NAME": self.flow.name,
                         "METAFLOW_STEP_NAME": node.name,
                         "METAFLOW_RUN_ID": run_id,
                         # "METAFLOW_TASK_ID": task_id,
@@ -1207,14 +1207,15 @@
                                     "METAFLOW_KUBERNETES_POD_NAME": "metadata.name",
                                     "METAFLOW_KUBERNETES_POD_ID": "metadata.uid",
                                     "METAFLOW_KUBERNETES_SERVICE_ACCOUNT_NAME": "spec.serviceAccountName",
                                     "METAFLOW_KUBERNETES_NODE_IP": "status.hostIP",
                                 }.items()
                             ],
                             image=resources["image"],
+                            image_pull_policy=resources["image_pull_policy"],
                             resources=kubernetes_sdk.V1ResourceRequirements(
                                 requests={
                                     "cpu": str(resources["cpu"]),
                                     "memory": "%sM" % str(resources["memory"]),
                                     "ephemeral-storage": "%sM" % str(resources["disk"]),
                                 },
                                 limits={
@@ -1380,38 +1381,38 @@
         if ARGO_EVENTS_EVENT is None:
             raise ArgoWorkflowsException(
                 "An Argo Event name hasn't been configured for your deployment yet. "
                 "Please see this article for more details on event names - "
                 "https://argoproj.github.io/argo-events/eventsources/naming/. "
                 "It is very likely that all events for your deployment share the "
                 "same name. You can configure it by executing "
-                "`metaflow configure events` or setting METAFLOW_ARGO_EVENTS_EVENT "
+                "`metaflow configure kubernetes` or setting METAFLOW_ARGO_EVENTS_EVENT "
                 "in your configuration. If in doubt, reach out for support at "
                 "http://chat.metaflow.org"
             )
         # Unfortunately argo events requires knowledge of event source today.
         # Hopefully, some day this requirement can be removed and events can be truly
         # impervious to their source and destination.
         if ARGO_EVENTS_EVENT_SOURCE is None:
             raise ArgoWorkflowsException(
                 "An Argo Event Source name hasn't been configured for your deployment "
                 "yet. Please see this article for more details on event names - "
                 "https://argoproj.github.io/argo-events/eventsources/naming/. "
-                "You can configure it by executing `metaflow configure events` or "
+                "You can configure it by executing `metaflow configure kubernetes` or "
                 "setting METAFLOW_ARGO_EVENTS_EVENT_SOURCE in your configuration. If "
                 "in doubt, reach out for support at http://chat.metaflow.org"
             )
         # Service accounts are a hard requirement since we utilize the
         # argoWorkflow trigger for resource sensors today.
         if ARGO_EVENTS_SERVICE_ACCOUNT is None:
             raise ArgoWorkflowsException(
                 "An Argo Event service account hasn't been configured for your "
                 "deployment yet. Please see this article for more details on event "
                 "names - https://argoproj.github.io/argo-events/service-accounts/. "
-                "You can configure it by executing `metaflow configure events` or "
+                "You can configure it by executing `metaflow configure kubernetes` or "
                 "setting METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT in your configuration. "
                 "If in doubt, reach out for support at http://chat.metaflow.org"
             )
 
         try:
             # Kubernetes is a soft dependency for generating Argo objects.
             # We can very well remove this dependency for Argo with the downside of
```

### Comparing `metaflow-2.9.1/metaflow/plugins/argo/argo_workflows_cli.py` & `metaflow-2.9.2/metaflow/plugins/argo/argo_workflows_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/argo/argo_workflows_decorator.py` & `metaflow-2.9.2/metaflow/plugins/argo/argo_workflows_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/argo/process_input_paths.py` & `metaflow-2.9.2/metaflow/plugins/argo/process_input_paths.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/aws_client.py` & `metaflow-2.9.2/metaflow/plugins/aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/aws_utils.py` & `metaflow-2.9.2/metaflow/plugins/aws/aws_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/batch/batch.py` & `metaflow-2.9.2/metaflow/plugins/aws/batch/batch.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/batch/batch_cli.py` & `metaflow-2.9.2/metaflow/plugins/aws/batch/batch_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/batch/batch_client.py` & `metaflow-2.9.2/metaflow/plugins/aws/batch/batch_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/batch/batch_decorator.py` & `metaflow-2.9.2/metaflow/plugins/aws/batch/batch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py` & `metaflow-2.9.2/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/step_functions/dynamo_db_client.py` & `metaflow-2.9.2/metaflow/plugins/aws/step_functions/dynamo_db_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/step_functions/event_bridge_client.py` & `metaflow-2.9.2/metaflow/plugins/aws/step_functions/event_bridge_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/step_functions/production_token.py` & `metaflow-2.9.2/metaflow/plugins/aws/step_functions/production_token.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/step_functions/schedule_decorator.py` & `metaflow-2.9.2/metaflow/plugins/aws/step_functions/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/step_functions/set_batch_environment.py` & `metaflow-2.9.2/metaflow/plugins/aws/step_functions/set_batch_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/step_functions/step_functions.py` & `metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/step_functions/step_functions_cli.py` & `metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/step_functions/step_functions_client.py` & `metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/aws/step_functions/step_functions_decorator.py` & `metaflow-2.9.2/metaflow/plugins/aws/step_functions/step_functions_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/azure/azure_tail.py` & `metaflow-2.9.2/metaflow/plugins/azure/azure_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/azure/azure_utils.py` & `metaflow-2.9.2/metaflow/plugins/azure/azure_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/azure/blob_service_client_factory.py` & `metaflow-2.9.2/metaflow/plugins/azure/blob_service_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/azure/includefile_support.py` & `metaflow-2.9.2/metaflow/plugins/azure/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_cli.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_client.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_datastore.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_decorator.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_modules/__init__.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_modules/base.html` & `metaflow-2.9.2/metaflow/plugins/cards/card_modules/base.html`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_modules/basic.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_modules/basic.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_modules/bundle.css` & `metaflow-2.9.2/metaflow/plugins/cards/card_modules/bundle.css`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_modules/card.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_modules/card.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_modules/chevron/main.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/main.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_modules/chevron/renderer.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/renderer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_modules/chevron/tokenizer.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_modules/chevron/tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_modules/components.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_modules/components.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_modules/convert_to_native_type.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_modules/convert_to_native_type.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_modules/main.js` & `metaflow-2.9.2/metaflow/plugins/cards/card_modules/main.js`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_modules/renderer_tools.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_modules/renderer_tools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_modules/test_cards.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_modules/test_cards.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/card_resolver.py` & `metaflow-2.9.2/metaflow/plugins/cards/card_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/component_serializer.py` & `metaflow-2.9.2/metaflow/plugins/cards/component_serializer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/cards/exception.py` & `metaflow-2.9.2/metaflow/plugins/cards/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/catch_decorator.py` & `metaflow-2.9.2/metaflow/plugins/catch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/conda/__init__.py` & `metaflow-2.9.2/metaflow/plugins/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/conda/batch_bootstrap.py` & `metaflow-2.9.2/metaflow/plugins/conda/batch_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/conda/conda.py` & `metaflow-2.9.2/metaflow/plugins/conda/conda.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/conda/conda_environment.py` & `metaflow-2.9.2/metaflow/plugins/conda/conda_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/conda/conda_flow_decorator.py` & `metaflow-2.9.2/metaflow/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/conda/conda_step_decorator.py` & `metaflow-2.9.2/metaflow/plugins/conda/conda_step_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/datastores/azure_storage.py` & `metaflow-2.9.2/metaflow/plugins/datastores/azure_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/datastores/gs_storage.py` & `metaflow-2.9.2/metaflow/plugins/datastores/gs_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/datastores/local_storage.py` & `metaflow-2.9.2/metaflow/plugins/datastores/local_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/datastores/s3_storage.py` & `metaflow-2.9.2/metaflow/plugins/datastores/s3_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/datatools/__init__.py` & `metaflow-2.9.2/metaflow/plugins/datatools/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/datatools/local.py` & `metaflow-2.9.2/metaflow/plugins/datatools/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/datatools/s3/s3.py` & `metaflow-2.9.2/metaflow/plugins/datatools/s3/s3.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/datatools/s3/s3op.py` & `metaflow-2.9.2/metaflow/plugins/datatools/s3/s3op.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/datatools/s3/s3tail.py` & `metaflow-2.9.2/metaflow/plugins/datatools/s3/s3tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/datatools/s3/s3util.py` & `metaflow-2.9.2/metaflow/plugins/datatools/s3/s3util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/debug_logger.py` & `metaflow-2.9.2/metaflow/plugins/debug_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/debug_monitor.py` & `metaflow-2.9.2/metaflow/plugins/debug_monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/__init__.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/client.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/client_modules.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/client_modules.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/communication/bytestream.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/communication/bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/communication/channel.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/communication/channel.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/communication/socket_bytestream.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/communication/socket_bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/communication/utils.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/communication/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/consts.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/consts.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/data_transferer.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/data_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/exception_transferer.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/exception_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/override_decorators.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/override_decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/server.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/server.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/stub.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/stub.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/env_escape/utils.py` & `metaflow-2.9.2/metaflow/plugins/env_escape/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/environment_decorator.py` & `metaflow-2.9.2/metaflow/plugins/environment_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/events_decorator.py` & `metaflow-2.9.2/metaflow/plugins/events_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/frameworks/pytorch.py` & `metaflow-2.9.2/metaflow/plugins/frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/gcp/gs_storage_client_factory.py` & `metaflow-2.9.2/metaflow/plugins/gcp/gs_storage_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/gcp/gs_tail.py` & `metaflow-2.9.2/metaflow/plugins/gcp/gs_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/gcp/gs_utils.py` & `metaflow-2.9.2/metaflow/plugins/gcp/gs_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/gcp/includefile_support.py` & `metaflow-2.9.2/metaflow/plugins/gcp/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/kubernetes/kubernetes.py` & `metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from metaflow import current, util
 from metaflow.exception import MetaflowException
 from metaflow.metaflow_config import (
     ARGO_EVENTS_EVENT,
     ARGO_EVENTS_EVENT_BUS,
     ARGO_EVENTS_EVENT_SOURCE,
     ARGO_EVENTS_SERVICE_ACCOUNT,
-    ARGO_EVENTS_WEBHOOK_URL,
+    ARGO_EVENTS_INTERNAL_WEBHOOK_URL,
     AWS_SECRETS_MANAGER_DEFAULT_REGION,
     AZURE_STORAGE_BLOB_SERVICE_ENDPOINT,
     CARD_AZUREROOT,
     CARD_GSROOT,
     CARD_S3ROOT,
     DATASTORE_SYSROOT_AZURE,
     DATASTORE_SYSROOT_GS,
@@ -141,14 +141,15 @@
         attempt,
         user,
         code_package_sha,
         code_package_url,
         code_package_ds,
         step_cli,
         docker_image,
+        docker_image_pull_policy,
         service_account=None,
         secrets=None,
         node_selector=None,
         namespace=None,
         cpu=None,
         gpu=None,
         gpu_vendor=None,
@@ -180,14 +181,15 @@
                     step_name=step_name,
                     task_id=task_id,
                     attempt=attempt,
                     code_package_url=code_package_url,
                     step_cmds=[step_cli],
                 ),
                 image=docker_image,
+                image_pull_policy=docker_image_pull_policy,
                 cpu=cpu,
                 memory=memory,
                 disk=disk,
                 gpu=gpu,
                 gpu_vendor=gpu_vendor,
                 timeout_in_seconds=run_time_limit,
                 # Retries are handled by Metaflow runtime
@@ -249,15 +251,15 @@
             # assumes metadata is stored in DATASTORE_LOCAL_DIR on the Kubernetes
             # pod; this happens when METAFLOW_DATASTORE_SYSROOT_LOCAL is NOT set (
             # see get_datastore_root_from_config in datastore/local.py).
         )
 
         # Set environment variables to support metaflow.integrations.ArgoEvent
         job.environment_variable(
-            "METAFLOW_ARGO_EVENTS_WEBHOOK_URL", ARGO_EVENTS_WEBHOOK_URL
+            "METAFLOW_ARGO_EVENTS_WEBHOOK_URL", ARGO_EVENTS_INTERNAL_WEBHOOK_URL
         )
         job.environment_variable("METAFLOW_ARGO_EVENTS_EVENT", ARGO_EVENTS_EVENT)
         job.environment_variable(
             "METAFLOW_ARGO_EVENTS_EVENT_BUS", ARGO_EVENTS_EVENT_BUS
         )
         job.environment_variable(
             "METAFLOW_ARGO_EVENTS_EVENT_SOURCE", ARGO_EVENTS_EVENT_SOURCE
```

### Comparing `metaflow-2.9.1/metaflow/plugins/kubernetes/kubernetes_cli.py` & `metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,19 @@
 @click.argument("code-package-url")
 @click.option(
     "--executable",
     help="Executable requirement for Kubernetes pod.",
 )
 @click.option("--image", help="Docker image requirement for Kubernetes pod.")
 @click.option(
+    "--image-pull-policy",
+    default=None,
+    help="Optional Docker Image Pull Policy for Kubernetes pod.",
+)
+@click.option(
     "--service-account",
     help="IRSA requirement for Kubernetes pod.",
 )
 @click.option(
     "--secrets",
     multiple=True,
     default=None,
@@ -104,14 +109,15 @@
 def step(
     ctx,
     step_name,
     code_package_sha,
     code_package_url,
     executable=None,
     image=None,
+    image_pull_policy=None,
     service_account=None,
     secrets=None,
     node_selector=None,
     k8s_namespace=None,
     cpu=None,
     disk=None,
     memory=None,
@@ -216,14 +222,15 @@
                 attempt=str(retry_count),
                 user=util.get_username(),
                 code_package_sha=code_package_sha,
                 code_package_url=code_package_url,
                 code_package_ds=ctx.obj.flow_datastore.TYPE,
                 step_cli=step_cli,
                 docker_image=image,
+                docker_image_pull_policy=image_pull_policy,
                 service_account=service_account,
                 secrets=secrets,
                 node_selector=node_selector,
                 namespace=k8s_namespace,
                 cpu=cpu,
                 disk=disk,
                 memory=memory,
```

### Comparing `metaflow-2.9.1/metaflow/plugins/kubernetes/kubernetes_client.py` & `metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/kubernetes/kubernetes_decorator.py` & `metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from metaflow.exception import MetaflowException
 from metaflow.metadata import MetaDatum
 from metaflow.metadata.util import sync_local_metadata_to_datastore
 from metaflow.metaflow_config import (
     DATASTORE_LOCAL_DIR,
     KUBERNETES_CONTAINER_IMAGE,
     KUBERNETES_CONTAINER_REGISTRY,
+    KUBERNETES_IMAGE_PULL_POLICY,
     KUBERNETES_GPU_VENDOR,
     KUBERNETES_NAMESPACE,
     KUBERNETES_NODE_SELECTOR,
     KUBERNETES_TOLERATIONS,
     KUBERNETES_SERVICE_ACCOUNT,
     KUBERNETES_SECRETS,
     KUBERNETES_FETCH_EC2_METADATA,
@@ -81,14 +82,15 @@
 
     name = "kubernetes"
     defaults = {
         "cpu": "1",
         "memory": "4096",
         "disk": "10240",
         "image": None,
+        "image_pull_policy": None,
         "service_account": None,
         "secrets": None,  # e.g., mysecret
         "node_selector": None,  # e.g., kubernetes.io/os=linux
         "namespace": None,
         "gpu": None,  # value of 0 implies that the scheduled node should not have GPUs
         "gpu_vendor": None,
         "tolerations": None,  # e.g., [{"key": "arch", "operator": "Equal", "value": "amd"},
@@ -119,14 +121,16 @@
         if (
             not self.attributes["persistent_volume_claims"]
             and KUBERNETES_PERSISTENT_VOLUME_CLAIMS
         ):
             self.attributes["persistent_volume_claims"] = json.loads(
                 KUBERNETES_PERSISTENT_VOLUME_CLAIMS
             )
+        if not self.attributes["image_pull_policy"] and KUBERNETES_IMAGE_PULL_POLICY:
+            self.attributes["image_pull_policy"] = KUBERNETES_IMAGE_PULL_POLICY
 
         if isinstance(self.attributes["node_selector"], str):
             self.attributes["node_selector"] = self.parse_node_selector(
                 self.attributes["node_selector"].split(",")
             )
 
         if self.attributes["tolerations"]:
```

### Comparing `metaflow-2.9.1/metaflow/plugins/kubernetes/kubernetes_job.py` & `metaflow-2.9.2/metaflow/plugins/kubernetes/kubernetes_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,15 @@
                                         )
                                     )
                                     for k in list(self._kwargs.get("secrets", []))
                                     + KUBERNETES_SECRETS.split(",")
                                     if k
                                 ],
                                 image=self._kwargs["image"],
+                                image_pull_policy=self._kwargs["image_pull_policy"],
                                 name=self._kwargs["step_name"].replace("_", "-"),
                                 resources=client.V1ResourceRequirements(
                                     requests={
                                         "cpu": str(self._kwargs["cpu"]),
                                         "memory": "%sM" % str(self._kwargs["memory"]),
                                         "ephemeral-storage": "%sM"
                                         % str(self._kwargs["disk"]),
```

### Comparing `metaflow-2.9.1/metaflow/plugins/metadata/local.py` & `metaflow-2.9.2/metaflow/plugins/metadata/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/metadata/service.py` & `metaflow-2.9.2/metaflow/plugins/metadata/service.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/package_cli.py` & `metaflow-2.9.2/metaflow/plugins/package_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/parallel_decorator.py` & `metaflow-2.9.2/metaflow/plugins/parallel_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/project_decorator.py` & `metaflow-2.9.2/metaflow/plugins/project_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/resources_decorator.py` & `metaflow-2.9.2/metaflow/plugins/resources_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/retry_decorator.py` & `metaflow-2.9.2/metaflow/plugins/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/secrets/secrets_decorator.py` & `metaflow-2.9.2/metaflow/plugins/secrets/secrets_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/storage_executor.py` & `metaflow-2.9.2/metaflow/plugins/storage_executor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/tag_cli.py` & `metaflow-2.9.2/metaflow/plugins/tag_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/test_unbounded_foreach_decorator.py` & `metaflow-2.9.2/metaflow/plugins/test_unbounded_foreach_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/plugins/timeout_decorator.py` & `metaflow-2.9.2/metaflow/plugins/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/procpoll.py` & `metaflow-2.9.2/metaflow/procpoll.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/pylint_wrapper.py` & `metaflow-2.9.2/metaflow/pylint_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/runtime.py` & `metaflow-2.9.2/metaflow/runtime.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/sidecar/sidecar.py` & `metaflow-2.9.2/metaflow/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/sidecar/sidecar_messages.py` & `metaflow-2.9.2/metaflow/sidecar/sidecar_messages.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/sidecar/sidecar_subprocess.py` & `metaflow-2.9.2/metaflow/sidecar/sidecar_subprocess.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/sidecar/sidecar_worker.py` & `metaflow-2.9.2/metaflow/sidecar/sidecar_worker.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tagging_util.py` & `metaflow-2.9.2/metaflow/tagging_util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/task.py` & `metaflow-2.9.2/metaflow/task.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/00-helloworld/helloworld.py` & `metaflow-2.9.2/metaflow/tutorials/00-helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/01-playlist/README.md` & `metaflow-2.9.2/metaflow/tutorials/01-playlist/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/01-playlist/movies.csv` & `metaflow-2.9.2/metaflow/tutorials/01-playlist/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/01-playlist/playlist.ipynb` & `metaflow-2.9.2/metaflow/tutorials/01-playlist/playlist.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/01-playlist/playlist.py` & `metaflow-2.9.2/metaflow/tutorials/01-playlist/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/02-statistics/README.md` & `metaflow-2.9.2/metaflow/tutorials/02-statistics/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/02-statistics/movies.csv` & `metaflow-2.9.2/metaflow/tutorials/02-statistics/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/02-statistics/stats.ipynb` & `metaflow-2.9.2/metaflow/tutorials/02-statistics/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/02-statistics/stats.py` & `metaflow-2.9.2/metaflow/tutorials/02-statistics/stats.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/03-playlist-redux/README.md` & `metaflow-2.9.2/metaflow/tutorials/03-playlist-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/03-playlist-redux/playlist.py` & `metaflow-2.9.2/metaflow/tutorials/03-playlist-redux/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/04-playlist-plus/README.md` & `metaflow-2.9.2/metaflow/tutorials/04-playlist-plus/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/04-playlist-plus/playlist.py` & `metaflow-2.9.2/metaflow/tutorials/04-playlist-plus/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/05-hello-cloud/README.md` & `metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb` & `metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/05-hello-cloud/hello-cloud.py` & `metaflow-2.9.2/metaflow/tutorials/05-hello-cloud/hello-cloud.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/06-statistics-redux/README.md` & `metaflow-2.9.2/metaflow/tutorials/06-statistics-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/06-statistics-redux/stats.ipynb` & `metaflow-2.9.2/metaflow/tutorials/06-statistics-redux/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/07-worldview/worldview.ipynb` & `metaflow-2.9.2/metaflow/tutorials/07-worldview/worldview.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/08-autopilot/README.md` & `metaflow-2.9.2/metaflow/tutorials/08-autopilot/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/tutorials/08-autopilot/autopilot.ipynb` & `metaflow-2.9.2/metaflow/tutorials/08-autopilot/autopilot.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/util.py` & `metaflow-2.9.2/metaflow/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow/vendor.py` & `metaflow-2.9.2/metaflow/vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/metaflow.egg-info/SOURCES.txt` & `metaflow-2.9.2/metaflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.1/setup.py` & `metaflow-2.9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "2.9.1"
+version = "2.9.2"
 
 setup(
     include_package_data=True,
     name="metaflow",
     version=version,
     description="Metaflow: More Data Science, Less Engineering",
     long_description=open("README.md").read(),
```

