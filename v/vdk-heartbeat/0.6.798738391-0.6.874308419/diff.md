# Comparing `tmp/vdk-heartbeat-0.6.798738391.tar.gz` & `tmp/vdk-heartbeat-0.6.874308419.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-heartbeat-0.6.798738391.tar", last modified: Tue Mar  7 14:46:20 2023, max compression
+gzip compressed data, was "dist/vdk-heartbeat-0.6.874308419.tar", last modified: Mon May 22 08:15:53 2023, max compression
```

## Comparing `vdk-heartbeat-0.6.798738391.tar` & `vdk-heartbeat-0.6.874308419.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5793 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4758 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1481 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/
--rw-rw-rw-   0 root         (0) root         (0)    10284 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/config.py
--rw-rw-rw-   0 root         (0) root         (0)    10133 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/database_run_test.py
--rw-rw-rw-   0 root         (0) root         (0)      956 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/empty_run_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/hearbeat.py
--rw-rw-rw-   0 root         (0) root         (0)     2312 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/heartbeat_test.py
--rw-rw-rw-   0 root         (0) root         (0)    10027 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/impala_database_test.py
--rw-rw-rw-   0 root         (0) root         (0)    16057 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/job_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     1961 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1479 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/main.py
--rw-rw-rw-   0 root         (0) root         (0)     1926 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/reporter.py
--rw-rw-rw-   0 root         (0) root         (0)     2622 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/simple_run_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1736 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/successful_run_test.py
--rw-rw-rw-   0 root         (0) root         (0)      756 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/tracing.py
--rw-rw-rw-   0 root         (0) root         (0)     4443 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/trino_database_test.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/05_set_properties.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/10_ingest_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1512 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/20_verify_data.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/config.ini
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/empty/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/empty/10_do_nothing.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/empty/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/05_set_properties.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/10_create_table_source.sql
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/15_create_table_destination.sql
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/16_create_table_load_destination.sql
--rw-rw-rw-   0 root         (0) root         (0)      887 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/20_move_data_using_load.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/30_move_data_using_sql.sql
--rw-rw-rw-   0 root         (0) root         (0)     1251 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/40_execute_template.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/README.md
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/simple/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/simple/10_simple.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/simple/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/
--rw-rw-rw-   0 root         (0) root         (0)      574 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/05_set_properties.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/10_drop_table_destination.sql
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/15_create_table_destination.sql
--rw-rw-rw-   0 root         (0) root         (0)      969 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/20_move_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2838 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/25_execute_template.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/30_move_data_using_sql.sql
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/config.ini
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-03-07 14:46:07.000000 vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk_heartbeat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5793 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk_heartbeat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3045 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk_heartbeat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk_heartbeat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk_heartbeat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk_heartbeat.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      144 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk_heartbeat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-07 14:46:20.000000 vdk-heartbeat-0.6.798738391/src/vdk_heartbeat.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-03-07 14:46:10.000000 vdk-heartbeat-0.6.798738391/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6339 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5304 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/
+-rw-rw-rw-   0 root         (0) root         (0)    10284 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10133 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/database_run_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      956 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/empty_run_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2106 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/hearbeat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/heartbeat_base_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2474 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/heartbeat_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    10027 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/impala_database_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    16057 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/job_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     1961 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1479 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/ping_frontend_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/reporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2622 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/simple_run_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/successful_run_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      756 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/tracing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4443 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/trino_database_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/05_set_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/10_ingest_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/20_verify_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/empty/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/empty/10_do_nothing.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/empty/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/05_set_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/10_create_table_source.sql
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/15_create_table_destination.sql
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/16_create_table_load_destination.sql
+-rw-rw-rw-   0 root         (0) root         (0)      887 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/20_move_data_using_load.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/30_move_data_using_sql.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/40_execute_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/simple/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/simple/10_simple.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/simple/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/05_set_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/10_drop_table_destination.sql
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/15_create_table_destination.sql
+-rw-rw-rw-   0 root         (0) root         (0)      969 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/20_move_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2838 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/25_execute_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/30_move_data_using_sql.sql
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-05-22 08:15:37.000000 vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk_heartbeat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6339 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk_heartbeat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk_heartbeat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk_heartbeat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk_heartbeat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk_heartbeat.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk_heartbeat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-22 08:15:53.000000 vdk-heartbeat-0.6.874308419/src/vdk_heartbeat.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-05-22 08:15:41.000000 vdk-heartbeat-0.6.874308419/version.txt
```

### Comparing `vdk-heartbeat-0.6.798738391/PKG-INFO` & `vdk-heartbeat-0.6.874308419/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-heartbeat
-Version: 0.6.798738391
+Version: 0.6.874308419
 Summary: Versatile Data Kit Heartbeat and Health Test
 Home-page: https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-heartbeat
 Author: VMware Inc.
 Author-email: taurus@groups.vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki/Introduction
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-heartbeat
 Platform: any
@@ -143,7 +143,28 @@
 ```
 export VDK_HEARTBEAT_INGEST_TARGET="trino-http-datasource"
 export VDK_HEARTBEAT_INGEST_METHOD="http"
 export VDK_HEARTBEAT_INGEST_DESTINATION_TABLE="sample_destination_table"
 export DB_DEFAULT_TYPE="trino"
 export DATABASE_TEST_DB="memory.default"
 ```
+
+### Ping the frontend
+
+No additional configuration is needed for this test.
+
+Point heartbeat to the correct module and class
+
+```
+JOB_RUN_TEST_MODULE_NAME=vdk.internal.heartbeat.ping_frontend_test
+JOB_RUN_TEST_CLASS_NAME=PingFrontendTest
+```
+
+The CONTROL_API_URL environment variable doubles as the frontend url, since both
+th control service and the frontend are deployed to the same host by the helm
+chart.
+
+```
+CONTROL_API_URL=http://cicd-control-service-svc:8092
+```
+
+The test sends a `GET` request to the URL and expects a success response
```

### Comparing `vdk-heartbeat-0.6.798738391/README.md` & `vdk-heartbeat-0.6.874308419/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -119,7 +119,28 @@
 ```
 export VDK_HEARTBEAT_INGEST_TARGET="trino-http-datasource"
 export VDK_HEARTBEAT_INGEST_METHOD="http"
 export VDK_HEARTBEAT_INGEST_DESTINATION_TABLE="sample_destination_table"
 export DB_DEFAULT_TYPE="trino"
 export DATABASE_TEST_DB="memory.default"
 ```
+
+### Ping the frontend
+
+No additional configuration is needed for this test.
+
+Point heartbeat to the correct module and class
+
+```
+JOB_RUN_TEST_MODULE_NAME=vdk.internal.heartbeat.ping_frontend_test
+JOB_RUN_TEST_CLASS_NAME=PingFrontendTest
+```
+
+The CONTROL_API_URL environment variable doubles as the frontend url, since both
+th control service and the frontend are deployed to the same host by the helm
+chart.
+
+```
+CONTROL_API_URL=http://cicd-control-service-svc:8092
+```
+
+The test sends a `GET` request to the URL and expects a success response
```

### Comparing `vdk-heartbeat-0.6.798738391/setup.cfg` & `vdk-heartbeat-0.6.874308419/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/config.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/config.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/database_run_test.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/database_run_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/empty_run_test.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/empty_run_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/hearbeat.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/heartbeat_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,71 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
+from abc import ABC
+from abc import abstractmethod
 
 from vdk.internal.heartbeat.config import Config
-from vdk.internal.heartbeat.heartbeat_test import create_test_instance
-from vdk.internal.heartbeat.heartbeat_test import HeartbeatTest
+from vdk.internal.heartbeat.heartbeat_base_test import HeartbeatBaseTest
 from vdk.internal.heartbeat.job_controller import JobController
-from vdk.internal.heartbeat.reporter import TestDecorator
+from vdk.internal.heartbeat.tracing import LogDecorator
 
 log = logging.getLogger(__name__)
 
 
-class Heartbeat:
+class HeartbeatTest(HeartbeatBaseTest):
     """
     Executes a heartbeat test that verifies the correct behaviour of Data Pipelines.
 
     It has the following steps:
     - Creates a Data Job using VDK CLI for managing jobs
     - Deploys the data job using the same Versatile Data Kit SDK
     - Run database test to verify the job works correctly in cloud runtime.
     - Deletes the Data Job using VDK CLI
     """
 
     def __init__(self, config: Config):
-        self._config = config
-
-    @TestDecorator()
-    def run(self):
-        run_test = create_test_instance(self._config)
-        job_controller = JobController(self._config)
+        self.config = config
+        self.__job_controller = JobController(config)
 
+    @LogDecorator(log)
+    def run_test(self):
         try:
-            job_controller.login()
-            job_controller.create_job()
-            job_controller.deploy_job()
+            self.__job_controller.login()
+            self.__job_controller.create_job()
+            self.__job_controller.deploy_job()
 
-            job_controller.check_list_jobs()
-            job_controller.check_deployments()
-            job_controller.disable_deployment()
-            job_controller.check_deployments(enabled=False)
+            self.__job_controller.check_list_jobs()
+            self.__job_controller.check_deployments()
+            self.__job_controller.disable_deployment()
+            self.__job_controller.check_deployments(enabled=False)
 
-            run_test.setup()
+            self.setup()
 
-            job_controller.enable_deployment()
-            job_controller.show_job_details()
+            self.__job_controller.enable_deployment()
+            self.__job_controller.show_job_details()
 
-            run_test.execute_test()
-            job_controller.show_last_job_execution_logs()
+            self.execute_test()
+            self.__job_controller.show_last_job_execution_logs()
 
-            job_controller.disable_deployment()
+            self.__job_controller.disable_deployment()
 
             if self._config.check_manual_job_execution:
-                job_controller.check_job_execution_finished()
-                job_controller.start_job_execution()
-                job_controller.check_job_execution_finished()
+                self.__job_controller.check_job_execution_finished()
+                self.__job_controller.start_job_execution()
+                self.__job_controller.check_job_execution_finished()
 
-            self.clean(run_test, job_controller)
+            self.clean()
             log.info("Heartbeat has finished successfully.")
         except:
             log.info("Heartbeat has failed.")
-            job_controller.show_job_details()
-            job_controller.show_last_job_execution_logs()
+            self.__job_controller.show_job_details()
+            self.__job_controller.show_last_job_execution_logs()
             if self._config.clean_up_on_failure:
                 log.info("Heartbeat clean up on failure.")
-                self.clean(run_test, job_controller)
+                self.clean()
             raise
 
-    @staticmethod
-    def clean(run_test: HeartbeatTest, job_controller: JobController):
-        job_controller.login()
-        job_controller.delete_job()
-        run_test.clean_up()
+    def clean(self):
+        self.__job_controller.login()
+        self.__job_controller.delete_job()
+        self.clean_up()
```

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/heartbeat_test.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/hearbeat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,39 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
-from abc import ABC
-from abc import abstractmethod
 
 from vdk.internal.heartbeat.config import Config
-from vdk.internal.heartbeat.tracing import LogDecorator
+from vdk.internal.heartbeat.heartbeat_base_test import HeartbeatBaseTest
+from vdk.internal.heartbeat.reporter import TestDecorator
 
 log = logging.getLogger(__name__)
 
 
-class HeartbeatTest(ABC):
+class Heartbeat:
     """
-    Interface for defing tests
+    Executes a heartbeat test that verifies the correct behaviour of Data Pipelines.
+
+    It has the following steps:
+    - Creates a Data Job using VDK CLI for managing jobs
+    - Deploys the data job using the same Versatile Data Kit SDK
+    - Run database test to verify the job works correctly in cloud runtime.
+    - Deletes the Data Job using VDK CLI
     """
 
     def __init__(self, config: Config):
-        self.config = config
+        self._config = config
 
-    @LogDecorator(log)
-    @abstractmethod
-    def setup(self):
-        """
-        Setup the test and all that is necessary
-        """
-        pass
-
-    def __exit__(self, *exc):
-        self.clean_up()
-
-    @LogDecorator(log)
-    @abstractmethod
-    def clean_up(self):
-        """
-        After the test is finished it cleans up all resources used by the test.
-        """
-        pass
-
-    @LogDecorator(log)
-    @abstractmethod
-    def execute_test(self):
-        """
-        Execute the test and run assertion and verification. If method returns then test has passed.
-        If method throws an exception then test has failed.
-        """
-        pass
+    @TestDecorator()
+    def run(self):
+        create_test_instance(self._config).run_test()
 
 
-def create_test_instance(config: Config) -> HeartbeatTest:
+@staticmethod
+def create_test_instance(config: Config) -> HeartbeatBaseTest:
     import importlib
 
     try:
         module = importlib.import_module(config.database_test_module_name)
     except ModuleNotFoundError as e:
         raise ModuleNotFoundError(
             f"Configured database_test_module_name is not found. Error was: {e}.\n"
```

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/impala_database_test.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/impala_database_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/job_controller.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/job_controller.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/log_config.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/main.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/main.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/reporter.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/reporter.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/simple_run_test.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/simple_run_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/successful_run_test.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/successful_run_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/tracing.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/tracing.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/trino_database_test.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/trino_database_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/util.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/util.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/05_set_properties.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/05_set_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/10_ingest_data.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/10_ingest_data.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/20_verify_data.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/20_verify_data.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/20_move_data_using_load.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/20_move_data_using_load.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/40_execute_template.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/40_execute_template.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/README.md` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/README.md`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/05_set_properties.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/05_set_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/20_move_data.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/20_move_data.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/25_execute_template.py` & `vdk-heartbeat-0.6.874308419/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/25_execute_template.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk_heartbeat.egg-info/PKG-INFO` & `vdk-heartbeat-0.6.874308419/src/vdk_heartbeat.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-heartbeat
-Version: 0.6.798738391
+Version: 0.6.874308419
 Summary: Versatile Data Kit Heartbeat and Health Test
 Home-page: https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-heartbeat
 Author: VMware Inc.
 Author-email: taurus@groups.vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki/Introduction
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-heartbeat
 Platform: any
@@ -143,7 +143,28 @@
 ```
 export VDK_HEARTBEAT_INGEST_TARGET="trino-http-datasource"
 export VDK_HEARTBEAT_INGEST_METHOD="http"
 export VDK_HEARTBEAT_INGEST_DESTINATION_TABLE="sample_destination_table"
 export DB_DEFAULT_TYPE="trino"
 export DATABASE_TEST_DB="memory.default"
 ```
+
+### Ping the frontend
+
+No additional configuration is needed for this test.
+
+Point heartbeat to the correct module and class
+
+```
+JOB_RUN_TEST_MODULE_NAME=vdk.internal.heartbeat.ping_frontend_test
+JOB_RUN_TEST_CLASS_NAME=PingFrontendTest
+```
+
+The CONTROL_API_URL environment variable doubles as the frontend url, since both
+th control service and the frontend are deployed to the same host by the helm
+chart.
+
+```
+CONTROL_API_URL=http://cicd-control-service-svc:8092
+```
+
+The test sends a `GET` request to the URL and expects a success response
```

### Comparing `vdk-heartbeat-0.6.798738391/src/vdk_heartbeat.egg-info/SOURCES.txt` & `vdk-heartbeat-0.6.874308419/src/vdk_heartbeat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 setup.cfg
 setup.py
 version.txt
 src/vdk/internal/heartbeat/config.py
 src/vdk/internal/heartbeat/database_run_test.py
 src/vdk/internal/heartbeat/empty_run_test.py
 src/vdk/internal/heartbeat/hearbeat.py
+src/vdk/internal/heartbeat/heartbeat_base_test.py
 src/vdk/internal/heartbeat/heartbeat_test.py
 src/vdk/internal/heartbeat/impala_database_test.py
 src/vdk/internal/heartbeat/job_controller.py
 src/vdk/internal/heartbeat/log_config.py
 src/vdk/internal/heartbeat/main.py
+src/vdk/internal/heartbeat/ping_frontend_test.py
 src/vdk/internal/heartbeat/reporter.py
 src/vdk/internal/heartbeat/simple_run_test.py
 src/vdk/internal/heartbeat/successful_run_test.py
 src/vdk/internal/heartbeat/tracing.py
 src/vdk/internal/heartbeat/trino_database_test.py
 src/vdk/internal/heartbeat/util.py
 src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/05_set_properties.py
```

