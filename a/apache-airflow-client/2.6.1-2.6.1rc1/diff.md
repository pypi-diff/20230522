# Comparing `tmp/apache-airflow-client-2.6.1.tar.gz` & `tmp/apache-airflow-client-2.6.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-client-2.6.1.tar", last modified: Wed May 17 12:35:02 2023, max compression
+gzip compressed data, was "apache-airflow-client-2.6.1rc1.tar", last modified: Wed May 17 12:40:38 2023, max compression
```

## Comparing `apache-airflow-client-2.6.1.tar` & `apache-airflow-client-2.6.1rc1.tar`

### file list

```diff
@@ -1,287 +1,287 @@
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:35:02.378609 apache-airflow-client-2.6.1/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10850 2023-05-07 14:37:06.000000 apache-airflow-client-2.6.1/LICENSE
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)      240 2023-05-07 14:37:06.000000 apache-airflow-client-2.6.1/NOTICE
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     6469 2023-05-17 12:35:02.378768 apache-airflow-client-2.6.1/PKG-INFO
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     5615 2023-05-17 06:53:44.000000 apache-airflow-client-2.6.1/README.md
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:35:02.304411 apache-airflow-client-2.6.1/airflow_client/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)      786 2023-05-17 06:53:34.000000 apache-airflow-client-2.6.1/airflow_client/__init__.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:35:02.306770 apache-airflow-client-2.6.1/airflow_client/client/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9536 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/__init__.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:35:02.313082 apache-airflow-client-2.6.1/airflow_client/client/api/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     1010 2023-05-17 06:53:44.000000 apache-airflow-client-2.6.1/airflow_client/client/api/__init__.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    13979 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/config_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    39520 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/connection_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    69062 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/dag_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    61203 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/dag_run_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    15645 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/dag_warning_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    32132 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/dataset_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19853 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/event_log_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19906 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/import_error_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    18366 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/monitoring_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    14793 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/permission_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    14780 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/plugin_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34138 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/pool_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    14230 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/provider_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34452 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/role_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    86137 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/task_instance_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34755 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/user_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34736 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/variable_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22538 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api/x_com_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    46382 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/api_client.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:35:02.313419 apache-airflow-client-2.6.1/airflow_client/client/apis/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     2311 2023-05-17 06:53:44.000000 apache-airflow-client-2.6.1/airflow_client/client/apis/__init__.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25588 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/configuration.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    13802 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/exceptions.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:35:02.347583 apache-airflow-client-2.6.1/airflow_client/client/model/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     1134 2023-05-17 06:53:44.000000 apache-airflow-client-2.6.1/airflow_client/client/model/__init__.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19821 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/action.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22705 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/action_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19973 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/action_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20253 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/action_resource.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22847 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/basic_dag_run.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20083 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/class_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20186 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/clear_dag_run.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25136 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/clear_task_instances.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20030 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/collection_info.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20250 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/color.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19983 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/config.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19999 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/config_option.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20200 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/config_section.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24468 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/connection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20200 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/connection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22885 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/connection_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20133 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/connection_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21512 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/connection_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20125 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/connection_test.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20011 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/cron_expression.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    31229 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dag.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22645 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dag_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19928 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dag_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    38045 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dag_detail.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24700 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dag_detail_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    27046 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dag_run.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22712 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dag_run_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19979 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dag_run_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20491 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dag_schedule_dataset_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20763 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dag_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20769 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dag_warning.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22797 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dag_warning_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20044 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dag_warning_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21977 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dataset.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22725 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dataset_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19988 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dataset_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22631 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dataset_event.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22832 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dataset_event_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20069 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/dataset_event_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21637 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/error.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22259 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/event_log.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22752 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/event_log_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20009 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/event_log_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20414 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/extra_link.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20009 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/extra_link_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20411 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/health_info.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20363 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/health_status.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20772 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/import_error.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22812 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/import_error_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20054 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/import_error_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20039 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/inline_response200.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19794 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/inline_response2001.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21858 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/job.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24999 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/list_dag_runs_form.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25560 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/list_task_instance_form.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19996 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/metadatabase_status.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22805 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/plugin_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20073 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/plugin_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    23836 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/plugin_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22378 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/pool.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22665 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/pool_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19943 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/pool_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20393 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/provider.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19988 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/provider_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    23021 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/relative_delta.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19801 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/resource.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20456 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/role.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22665 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/role_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19943 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/role_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25425 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/schedule_interval.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20450 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/scheduler_status.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19856 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/set_dag_run_note.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19918 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/set_task_instance_note.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21169 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/sla_miss.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19734 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/tag.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26435 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/task.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19928 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/task_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20013 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/task_extra_links.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26384 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/task_instance.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22832 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/task_instance_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20069 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/task_instance_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20656 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/task_instance_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20145 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/task_instance_reference_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20746 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/task_outlet_dataset_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22492 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/task_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20487 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/time_delta.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20596 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/trigger.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21690 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/trigger_rule.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19972 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/update_dag_run_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20555 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/update_task_instance.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22984 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/update_task_instances_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26484 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/user.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19772 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/user_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22765 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/user_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20043 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/user_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24062 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/user_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19793 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/user_collection_item_roles.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22661 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/variable.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19769 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/variable_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22845 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/variable_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20103 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/variable_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20150 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/variable_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20157 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/version_info.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20449 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/weight_rule.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    23081 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/x_com.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19779 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/x_com_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22802 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/x_com_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20079 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/x_com_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20586 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model/x_com_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    90823 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/model_utils.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:35:02.347846 apache-airflow-client-2.6.1/airflow_client/client/models/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9137 2023-05-17 06:53:44.000000 apache-airflow-client-2.6.1/airflow_client/client/models/__init__.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22933 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/client/rest.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:35:02.377022 apache-airflow-client-2.6.1/airflow_client/test/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)      786 2023-05-17 06:53:44.000000 apache-airflow-client-2.6.1/airflow_client/test/__init__.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9526 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_action.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9942 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_action_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9717 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_action_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9757 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_action_resource.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9655 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_basic_dag_run.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9583 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_class_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9563 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_clear_dag_run.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9612 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_clear_task_instances.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9583 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_collection_info.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9519 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_color.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9638 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_config.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9527 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_config_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9569 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_config_option.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9684 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_config_section.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9832 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_connection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9591 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_connection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10277 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_connection_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10060 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_connection_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9819 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_connection_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9654 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_connection_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9583 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_connection_test.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9583 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_cron_expression.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9700 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10971 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9897 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9684 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10028 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_detail.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9681 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_detail_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9619 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_run.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10715 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_run_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9945 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_run_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9719 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_run_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9676 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_schedule_dataset_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9541 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9555 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_warning.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9552 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_warning_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10005 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_warning_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9763 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dag_warning_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9869 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dataset.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9990 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dataset_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9957 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dataset_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9728 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dataset_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9674 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dataset_event.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10035 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dataset_event_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9785 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_dataset_event_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9519 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_error.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9541 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_event_log.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9675 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_event_log_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9975 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_event_log_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9741 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_event_log_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9664 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_extra_link.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9715 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_extra_link_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9807 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_health_info.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9569 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_health_status.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9562 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_import_error.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9708 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_import_error_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10020 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_import_error_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9774 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_import_error_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9604 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_inline_response200.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9611 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_inline_response2001.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9505 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_job.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9592 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_list_dag_runs_form.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9723 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_list_task_instance_form.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9719 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_metadatabase_status.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9683 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_monitoring_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9548 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_permission_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9532 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_plugin_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10000 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_plugin_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9775 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_plugin_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9626 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_plugin_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9512 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_pool.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10013 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_pool_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9912 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_pool_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9695 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_pool_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9540 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_provider.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9532 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_provider_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9702 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_provider_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9576 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_relative_delta.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9540 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_resource.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9628 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_role.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10013 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_role_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9912 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_role_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9695 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_role_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9921 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_schedule_interval.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9698 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_scheduler_status.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9578 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_set_dag_run_note.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9620 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_set_task_instance_note.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9534 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_sla_miss.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9505 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_tag.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10195 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_task.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9658 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_task_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9700 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_task_extra_links.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9911 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_task_instance.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    11213 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_task_instance_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10035 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_task_instance_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9785 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_task_instance_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9633 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_task_instance_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9849 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_task_instance_reference_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9669 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_task_outlet_dataset_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9548 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_task_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9548 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_time_delta.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9533 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_trigger.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9562 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_trigger_rule.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9606 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_update_dag_run_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9612 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_update_task_instance.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9655 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_update_task_instances_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9896 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_user.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9549 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_user_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10013 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_user_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9970 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_user_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9753 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_user_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9766 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_user_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9648 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_user_collection_item_roles.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9802 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_variable.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9577 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_variable_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10095 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_variable_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10030 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_variable_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9797 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_variable_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9640 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_variable_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9562 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_version_info.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9555 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_weight_rule.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9745 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_x_com.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9550 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_x_com_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9664 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_x_com_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9973 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_x_com_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9755 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_x_com_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9613 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/airflow_client/test/test_x_com_collection_item.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:35:02.378403 apache-airflow-client-2.6.1/apache_airflow_client.egg-info/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     6469 2023-05-17 12:35:02.000000 apache-airflow-client-2.6.1/apache_airflow_client.egg-info/PKG-INFO
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    12437 2023-05-17 12:35:02.000000 apache-airflow-client-2.6.1/apache_airflow_client.egg-info/SOURCES.txt
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)        1 2023-05-17 12:35:02.000000 apache-airflow-client-2.6.1/apache_airflow_client.egg-info/dependency_links.txt
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)        1 2023-05-17 12:35:02.000000 apache-airflow-client-2.6.1/apache_airflow_client.egg-info/not-zip-safe
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)       32 2023-05-17 12:35:02.000000 apache-airflow-client-2.6.1/apache_airflow_client.egg-info/requires.txt
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)       15 2023-05-17 12:35:02.000000 apache-airflow-client-2.6.1/apache_airflow_client.egg-info/top_level.txt
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)      795 2023-05-17 12:35:02.379166 apache-airflow-client-2.6.1/setup.cfg
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     1519 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1/setup.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:40:38.997331 apache-airflow-client-2.6.1rc1/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10850 2023-05-07 14:37:06.000000 apache-airflow-client-2.6.1rc1/LICENSE
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)      240 2023-05-07 14:37:06.000000 apache-airflow-client-2.6.1rc1/NOTICE
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     6472 2023-05-17 12:40:38.997475 apache-airflow-client-2.6.1rc1/PKG-INFO
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     5615 2023-05-17 06:53:44.000000 apache-airflow-client-2.6.1rc1/README.md
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:40:38.930461 apache-airflow-client-2.6.1rc1/airflow_client/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)      786 2023-05-17 06:53:34.000000 apache-airflow-client-2.6.1rc1/airflow_client/__init__.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:40:38.933382 apache-airflow-client-2.6.1rc1/airflow_client/client/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9536 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/__init__.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:40:38.938331 apache-airflow-client-2.6.1rc1/airflow_client/client/api/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     1010 2023-05-17 06:53:44.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/__init__.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    13979 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/config_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    39520 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/connection_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    69062 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/dag_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    61203 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/dag_run_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    15645 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/dag_warning_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    32132 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/dataset_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19853 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/event_log_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19906 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/import_error_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    18366 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/monitoring_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    14793 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/permission_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    14780 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/plugin_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34138 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/pool_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    14230 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/provider_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34452 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/role_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    86137 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/task_instance_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34755 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/user_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34736 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/variable_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22538 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api/x_com_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    46382 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/api_client.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:40:38.938561 apache-airflow-client-2.6.1rc1/airflow_client/client/apis/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     2311 2023-05-17 06:53:44.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/apis/__init__.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25588 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/configuration.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    13802 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/exceptions.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:40:38.966015 apache-airflow-client-2.6.1rc1/airflow_client/client/model/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     1134 2023-05-17 06:53:44.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/__init__.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19821 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/action.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22705 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/action_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19973 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/action_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20253 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/action_resource.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22847 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/basic_dag_run.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20083 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/class_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20186 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/clear_dag_run.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25136 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/clear_task_instances.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20030 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/collection_info.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20250 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/color.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19983 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/config.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19999 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/config_option.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20200 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/config_section.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24468 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/connection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20200 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/connection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22885 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/connection_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20133 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/connection_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21512 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/connection_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20125 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/connection_test.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20011 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/cron_expression.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    31229 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22645 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19928 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    38045 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_detail.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24700 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_detail_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    27046 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_run.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22712 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_run_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19979 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_run_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20491 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_schedule_dataset_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20763 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20769 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_warning.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22797 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_warning_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20044 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_warning_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21977 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dataset.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22725 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dataset_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19988 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dataset_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22631 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dataset_event.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22832 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dataset_event_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20069 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/dataset_event_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21637 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/error.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22259 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/event_log.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22752 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/event_log_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20009 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/event_log_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20414 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/extra_link.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20009 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/extra_link_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20411 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/health_info.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20363 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/health_status.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20772 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/import_error.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22812 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/import_error_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20054 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/import_error_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20039 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/inline_response200.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19794 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/inline_response2001.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21858 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/job.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24999 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/list_dag_runs_form.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25560 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/list_task_instance_form.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19996 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/metadatabase_status.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22805 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/plugin_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20073 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/plugin_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    23836 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/plugin_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22378 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/pool.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22665 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/pool_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19943 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/pool_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20393 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/provider.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19988 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/provider_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    23021 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/relative_delta.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19801 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/resource.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20456 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/role.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22665 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/role_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19943 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/role_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25425 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/schedule_interval.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20450 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/scheduler_status.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19856 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/set_dag_run_note.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19918 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/set_task_instance_note.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21169 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/sla_miss.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19734 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/tag.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26435 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/task.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19928 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20013 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_extra_links.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26384 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_instance.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22832 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_instance_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20069 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_instance_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20656 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_instance_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20145 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_instance_reference_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20746 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_outlet_dataset_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22492 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20487 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/time_delta.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20596 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/trigger.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21690 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/trigger_rule.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19972 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/update_dag_run_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20555 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/update_task_instance.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22984 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/update_task_instances_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26484 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/user.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19772 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/user_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22765 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/user_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20043 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/user_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24062 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/user_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19793 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/user_collection_item_roles.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22661 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/variable.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19769 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/variable_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22845 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/variable_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20103 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/variable_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20150 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/variable_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20157 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/version_info.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20449 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/weight_rule.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    23081 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/x_com.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19779 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/x_com_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22802 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/x_com_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20079 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/x_com_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20586 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model/x_com_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    90823 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/model_utils.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:40:38.966307 apache-airflow-client-2.6.1rc1/airflow_client/client/models/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9137 2023-05-17 06:53:44.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/models/__init__.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22933 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/client/rest.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:40:38.995932 apache-airflow-client-2.6.1rc1/airflow_client/test/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)      786 2023-05-17 06:53:44.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/__init__.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9526 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_action.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9942 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_action_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9717 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_action_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9757 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_action_resource.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9655 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_basic_dag_run.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9583 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_class_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9563 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_clear_dag_run.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9612 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_clear_task_instances.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9583 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_collection_info.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9519 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_color.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9638 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_config.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9527 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_config_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9569 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_config_option.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9684 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_config_section.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9832 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9591 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10277 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10060 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9819 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9654 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9583 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection_test.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9583 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_cron_expression.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9700 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10971 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9897 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9684 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10028 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_detail.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9681 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_detail_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9619 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_run.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10715 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_run_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9945 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_run_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9719 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_run_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9676 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_schedule_dataset_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9541 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9555 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_warning.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9552 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_warning_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10005 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_warning_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9763 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_warning_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9869 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9990 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9957 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9728 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9674 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset_event.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10035 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset_event_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9785 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset_event_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9519 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_error.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9541 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_event_log.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9675 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_event_log_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9975 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_event_log_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9741 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_event_log_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9664 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_extra_link.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9715 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_extra_link_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9807 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_health_info.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9569 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_health_status.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9562 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_import_error.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9708 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_import_error_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10020 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_import_error_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9774 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_import_error_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9604 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_inline_response200.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9611 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_inline_response2001.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9505 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_job.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9592 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_list_dag_runs_form.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9723 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_list_task_instance_form.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9719 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_metadatabase_status.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9683 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_monitoring_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9548 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_permission_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9532 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_plugin_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10000 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_plugin_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9775 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_plugin_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9626 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_plugin_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9512 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_pool.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10013 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_pool_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9912 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_pool_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9695 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_pool_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9540 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_provider.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9532 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_provider_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9702 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_provider_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9576 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_relative_delta.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9540 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_resource.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9628 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_role.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10013 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_role_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9912 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_role_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9695 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_role_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9921 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_schedule_interval.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9698 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_scheduler_status.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9578 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_set_dag_run_note.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9620 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_set_task_instance_note.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9534 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_sla_miss.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9505 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_tag.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10195 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_task.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9658 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9700 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_extra_links.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9911 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_instance.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    11213 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_instance_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10035 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_instance_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9785 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_instance_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9633 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_instance_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9849 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_instance_reference_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9669 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_outlet_dataset_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9548 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9548 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_time_delta.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9533 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_trigger.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9562 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_trigger_rule.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9606 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_update_dag_run_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9612 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_update_task_instance.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9655 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_update_task_instances_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9896 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_user.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9549 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_user_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10013 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_user_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9970 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_user_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9753 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_user_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9766 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_user_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9648 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_user_collection_item_roles.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9802 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_variable.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9577 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_variable_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10095 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_variable_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10030 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_variable_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9797 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_variable_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9640 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_variable_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9562 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_version_info.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9555 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_weight_rule.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9745 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_x_com.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9550 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_x_com_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9664 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_x_com_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9973 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_x_com_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9755 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_x_com_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9613 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/airflow_client/test/test_x_com_collection_item.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-17 12:40:38.997108 apache-airflow-client-2.6.1rc1/apache_airflow_client.egg-info/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     6472 2023-05-17 12:40:38.000000 apache-airflow-client-2.6.1rc1/apache_airflow_client.egg-info/PKG-INFO
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    12437 2023-05-17 12:40:38.000000 apache-airflow-client-2.6.1rc1/apache_airflow_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)        1 2023-05-17 12:40:38.000000 apache-airflow-client-2.6.1rc1/apache_airflow_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)        1 2023-05-17 12:35:02.000000 apache-airflow-client-2.6.1rc1/apache_airflow_client.egg-info/not-zip-safe
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)       32 2023-05-17 12:40:38.000000 apache-airflow-client-2.6.1rc1/apache_airflow_client.egg-info/requires.txt
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)       15 2023-05-17 12:40:38.000000 apache-airflow-client-2.6.1rc1/apache_airflow_client.egg-info/top_level.txt
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)      798 2023-05-17 12:40:38.997875 apache-airflow-client-2.6.1rc1/setup.cfg
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     1519 2023-05-17 12:31:23.000000 apache-airflow-client-2.6.1rc1/setup.py
```

### Comparing `apache-airflow-client-2.6.1/LICENSE` & `apache-airflow-client-2.6.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/PKG-INFO` & `apache-airflow-client-2.6.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-client
-Version: 2.6.1
+Version: 2.6.1rc1
 Summary: Apache Airflow API (Stable)
 Home-page: https://airflow.apache.org/
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Download-URL: https://archive.apache.org/dist/airflow/clients/python/2.6.1
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow/stable/stable-rest-api-ref.html
```

### Comparing `apache-airflow-client-2.6.1/README.md` & `apache-airflow-client-2.6.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/__init__.py` & `apache-airflow-client-2.6.1rc1/airflow_client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/__init__.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/__init__.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/config_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/config_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/connection_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/connection_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/dag_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/dag_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/dag_run_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/dag_run_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/dag_warning_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/dag_warning_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/dataset_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/dataset_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/event_log_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/event_log_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/import_error_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/import_error_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/monitoring_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/monitoring_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/permission_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/permission_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/plugin_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/plugin_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/pool_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/pool_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/provider_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/provider_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/role_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/role_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/task_instance_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/task_instance_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/user_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/variable_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/variable_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api/x_com_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api/x_com_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/api_client.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/api_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/apis/__init__.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/configuration.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/configuration.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/exceptions.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/__init__.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/action.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/action.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/action_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/action_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/action_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/action_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/action_resource.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/action_resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/basic_dag_run.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/basic_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/class_reference.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/class_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/clear_dag_run.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/clear_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/clear_task_instances.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/clear_task_instances.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/collection_info.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/collection_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/color.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/color.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/config.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/config.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/config_option.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/config_option.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/config_section.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/config_section.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/connection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/connection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/connection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/connection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/connection_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/connection_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/connection_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/connection_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/connection_collection_item.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/connection_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/connection_test.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/cron_expression.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/cron_expression.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dag.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dag_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dag_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dag_detail.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_detail.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dag_detail_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dag_run.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dag_run_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_run_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dag_run_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_run_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dag_schedule_dataset_reference.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_schedule_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dag_state.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dag_warning.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_warning.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dag_warning_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_warning_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dag_warning_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dag_warning_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dataset.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dataset.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dataset_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dataset_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dataset_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dataset_event.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dataset_event.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dataset_event_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dataset_event_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/dataset_event_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/dataset_event_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/error.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/error.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/event_log.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/event_log.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/event_log_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/event_log_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/event_log_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/event_log_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/extra_link.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/extra_link.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/extra_link_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/extra_link_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/health_info.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/health_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/health_status.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/health_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/import_error.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/import_error.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/import_error_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/import_error_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/import_error_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/import_error_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/inline_response200.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/inline_response2001.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/job.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/job.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/list_dag_runs_form.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/list_dag_runs_form.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/list_task_instance_form.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/list_task_instance_form.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/metadatabase_status.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/metadatabase_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/plugin_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/plugin_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/plugin_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/plugin_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/plugin_collection_item.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/plugin_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/pool.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/pool.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/pool_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/pool_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/pool_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/pool_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/provider.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/provider.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/provider_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/provider_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/relative_delta.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/relative_delta.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/resource.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/role.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/role.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/role_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/role_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/role_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/role_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/schedule_interval.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/schedule_interval.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/scheduler_status.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/scheduler_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/set_dag_run_note.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/set_dag_run_note.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/set_task_instance_note.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/set_task_instance_note.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/sla_miss.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/sla_miss.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/tag.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/tag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/task.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/task.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/task_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/task_extra_links.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_extra_links.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/task_instance.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/task_instance_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_instance_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/task_instance_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_instance_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/task_instance_reference.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_instance_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/task_instance_reference_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_instance_reference_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/task_outlet_dataset_reference.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_outlet_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/task_state.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/task_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/time_delta.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/time_delta.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/trigger.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/trigger.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/trigger_rule.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/update_dag_run_state.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/update_dag_run_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/update_task_instance.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/update_task_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/update_task_instances_state.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/update_task_instances_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/user.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/user.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/user_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/user_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/user_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/user_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/user_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/user_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/user_collection_item.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/user_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/user_collection_item_roles.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/user_collection_item_roles.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/variable.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/variable.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/variable_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/variable_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/variable_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/variable_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/variable_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/variable_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/variable_collection_item.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/variable_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/version_info.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/version_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/weight_rule.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/weight_rule.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/x_com.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/x_com.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/x_com_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/x_com_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/x_com_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/x_com_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/x_com_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/x_com_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model/x_com_collection_item.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model/x_com_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/model_utils.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/models/__init__.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/client/rest.py` & `apache-airflow-client-2.6.1rc1/airflow_client/client/rest.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/__init__.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_action.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_action.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_action_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_action_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_action_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_action_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_action_resource.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_action_resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_basic_dag_run.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_basic_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_class_reference.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_class_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_clear_dag_run.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_clear_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_clear_task_instances.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_clear_task_instances.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_collection_info.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_collection_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_color.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_color.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_config.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_config.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_config_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_config_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_config_option.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_config_option.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_config_section.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_config_section.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_connection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_connection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_connection_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_connection_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_connection_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_connection_collection_item.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_connection_test.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_connection_test.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_cron_expression.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_cron_expression.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_detail.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_detail.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_detail_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_run.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_run_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_run_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_run_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_run_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_run_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_run_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_schedule_dataset_reference.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_schedule_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_state.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_warning.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_warning.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_warning_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_warning_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_warning_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_warning_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dag_warning_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dag_warning_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dataset.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dataset_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dataset_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dataset_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dataset_event.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset_event.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dataset_event_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset_event_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_dataset_event_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_dataset_event_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_error.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_error.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_event_log.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_event_log.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_event_log_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_event_log_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_event_log_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_event_log_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_event_log_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_event_log_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_extra_link.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_extra_link.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_extra_link_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_extra_link_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_health_info.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_health_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_health_status.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_health_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_import_error.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_import_error.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_import_error_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_import_error_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_import_error_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_import_error_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_import_error_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_import_error_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_inline_response200.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_inline_response2001.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_inline_response2001.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_job.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_job.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_list_dag_runs_form.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_list_dag_runs_form.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_list_task_instance_form.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_list_task_instance_form.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_metadatabase_status.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_metadatabase_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_monitoring_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_monitoring_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_permission_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_permission_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_plugin_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_plugin_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_plugin_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_plugin_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_plugin_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_plugin_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_plugin_collection_item.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_plugin_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_pool.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_pool.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_pool_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_pool_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_pool_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_pool_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_pool_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_pool_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_provider.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_provider.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_provider_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_provider_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_provider_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_provider_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_relative_delta.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_relative_delta.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_resource.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_role.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_role.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_role_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_role_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_role_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_role_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_role_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_role_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_schedule_interval.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_schedule_interval.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_scheduler_status.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_scheduler_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_set_dag_run_note.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_set_dag_run_note.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_set_task_instance_note.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_set_task_instance_note.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_sla_miss.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_sla_miss.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_tag.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_task.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_task.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_task_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_task_extra_links.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_extra_links.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_task_instance.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_task_instance_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_instance_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_task_instance_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_instance_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_task_instance_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_instance_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_task_instance_reference.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_instance_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_task_instance_reference_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_instance_reference_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_task_outlet_dataset_reference.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_outlet_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_task_state.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_task_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_time_delta.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_time_delta.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_trigger.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_trigger.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_trigger_rule.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_trigger_rule.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_update_dag_run_state.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_update_dag_run_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_update_task_instance.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_update_task_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_update_task_instances_state.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_update_task_instances_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_user.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_user.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_user_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_user_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_user_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_user_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_user_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_user_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_user_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_user_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_user_collection_item.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_user_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_user_collection_item_roles.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_user_collection_item_roles.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_variable.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_variable.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_variable_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_variable_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_variable_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_variable_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_variable_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_variable_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_variable_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_variable_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_variable_collection_item.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_variable_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_version_info.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_version_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_weight_rule.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_weight_rule.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_x_com.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_x_com.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_x_com_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_x_com_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_x_com_api.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_x_com_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_x_com_collection.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_x_com_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_x_com_collection_all_of.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_x_com_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/airflow_client/test/test_x_com_collection_item.py` & `apache-airflow-client-2.6.1rc1/airflow_client/test/test_x_com_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/apache_airflow_client.egg-info/PKG-INFO` & `apache-airflow-client-2.6.1rc1/apache_airflow_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-client
-Version: 2.6.1
+Version: 2.6.1rc1
 Summary: Apache Airflow API (Stable)
 Home-page: https://airflow.apache.org/
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Download-URL: https://archive.apache.org/dist/airflow/clients/python/2.6.1
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow/stable/stable-rest-api-ref.html
```

### Comparing `apache-airflow-client-2.6.1/apache_airflow_client.egg-info/SOURCES.txt` & `apache-airflow-client-2.6.1rc1/apache_airflow_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.1/setup.cfg` & `apache-airflow-client-2.6.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 python_requires = ~=3.7
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-client-2.6.1/setup.py` & `apache-airflow-client-2.6.1rc1/setup.py`

 * *Files identical despite different names*

