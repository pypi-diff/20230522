# Comparing `tmp/wds-client-0.2.84.tar.gz` & `tmp/wds-client-0.2.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wds-client-0.2.84.tar", last modified: Wed May 17 15:12:33 2023, max compression
+gzip compressed data, was "wds-client-0.2.85.tar", last modified: Mon May 22 18:53:17 2023, max compression
```

## Comparing `wds-client-0.2.84.tar` & `wds-client-0.2.85.tar`

### file list

```diff
@@ -1,82 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:33.224681 wds-client-0.2.84/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-17 15:12:33.224681 wds-client-0.2.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-05-17 15:10:55.000000 wds-client-0.2.84/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 15:12:33.224681 wds-client-0.2.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-17 15:10:55.000000 wds-client-0.2.84/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:33.216681 wds-client-0.2.84/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_db_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_inline_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_instances_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_record_attribute_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_record_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_records_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_search_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_version_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:33.216681 wds-client-0.2.84/wds_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:33.220681 wds-client-0.2.84/wds_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api/general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17329 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api/instances_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    61562 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api/records_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api/schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26217 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:33.224681 wds-client-0.2.84/wds_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/db_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/record_attribute_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/record_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/search_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/version_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:33.216681 wds-client-0.2.84/wds_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-17 15:12:33.000000 wds-client-0.2.84/wds_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-17 15:12:33.000000 wds-client-0.2.84/wds_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:12:33.000000 wds-client-0.2.84/wds_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 15:12:33.000000 wds-client-0.2.84/wds_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 15:12:33.000000 wds-client-0.2.84/wds_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:53:17.627516 wds-client-0.2.85/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 18:53:17.627516 wds-client-0.2.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-05-22 18:51:32.000000 wds-client-0.2.85/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 18:53:17.627516 wds-client-0.2.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-22 18:51:32.000000 wds-client-0.2.85/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:53:17.615516 wds-client-0.2.85/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_db_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_db_validationcomponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_db_validationcomponent_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_disk_space_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_disk_space_component_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_record_attribute_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-22 18:51:31.000000 wds-client-0.2.85/test/test_record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_record_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_request_body_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_search_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_stack_trace_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-22 18:51:32.000000 wds-client-0.2.85/test/test_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:53:17.619516 wds-client-0.2.85/wds_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:53:17.619516 wds-client-0.2.85/wds_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/api/general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17329 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/api/instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61562 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/api/records_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/api/schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/api/snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26217 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:53:17.627516 wds-client-0.2.85/wds_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/db_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/db_validationcomponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/db_validationcomponent_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/disk_space_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/disk_space_component_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/record_attribute_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-22 18:51:31.000000 wds-client-0.2.85/wds_client/models/record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/models/record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/models/record_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/models/record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/models/request_body_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/models/search_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/models/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/models/search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/models/stack_trace_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/models/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/models/tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/models/version_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-22 18:51:32.000000 wds-client-0.2.85/wds_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:53:17.619516 wds-client-0.2.85/wds_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 18:53:17.000000 wds-client-0.2.85/wds_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-22 18:53:17.000000 wds-client-0.2.85/wds_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:53:17.000000 wds-client-0.2.85/wds_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-22 18:53:17.000000 wds-client-0.2.85/wds_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 18:53:17.000000 wds-client-0.2.85/wds_client.egg-info/top_level.txt
```

### Comparing `wds-client-0.2.84/README.md` & `wds-client-0.2.85/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This page lists current APIs.
 As of v0.2, all APIs are subject to change without notice.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v0.2
-- Package version: 0.2.84
+- Package version: 0.2.85
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -108,14 +108,18 @@
  - [BatchRecordRequest](docs/BatchRecordRequest.md)
  - [BatchResponse](docs/BatchResponse.md)
  - [Build](docs/Build.md)
  - [Commit](docs/Commit.md)
  - [Component](docs/Component.md)
  - [Components](docs/Components.md)
  - [DbComponent](docs/DbComponent.md)
+ - [DbValidationcomponent](docs/DbValidationcomponent.md)
+ - [DbValidationcomponentDetails](docs/DbValidationcomponentDetails.md)
+ - [DiskSpaceComponent](docs/DiskSpaceComponent.md)
+ - [DiskSpaceComponentDetails](docs/DiskSpaceComponentDetails.md)
  - [ErrorResponse](docs/ErrorResponse.md)
  - [Git](docs/Git.md)
  - [InlineObject](docs/InlineObject.md)
  - [RecordAttributeDefinition](docs/RecordAttributeDefinition.md)
  - [RecordQueryResponse](docs/RecordQueryResponse.md)
  - [RecordRequest](docs/RecordRequest.md)
  - [RecordResponse](docs/RecordResponse.md)
```

### Comparing `wds-client-0.2.84/setup.py` & `wds-client-0.2.85/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "wds-client"
-VERSION = "0.2.84"
+VERSION = "0.2.85"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `wds-client-0.2.84/test/test_attribute_schema.py` & `wds-client-0.2.85/test/test_attribute_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_batch_operation.py` & `wds-client-0.2.85/test/test_batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_batch_record_request.py` & `wds-client-0.2.85/test/test_batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_batch_response.py` & `wds-client-0.2.85/test/test_batch_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_build.py` & `wds-client-0.2.85/test/test_build.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_commit.py` & `wds-client-0.2.85/test/test_commit.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_component.py` & `wds-client-0.2.85/test/test_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_components.py` & `wds-client-0.2.85/test/test_db_validationcomponent.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,52 +12,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.components import Components  # noqa: E501
+from wds_client.models.db_validationcomponent import DbValidationcomponent  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestComponents(unittest.TestCase):
-    """Components unit test stubs"""
+class TestDbValidationcomponent(unittest.TestCase):
+    """DbValidationcomponent unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test Components
+        """Test DbValidationcomponent
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.components.Components()  # noqa: E501
+        # model = wds_client.models.db_validationcomponent.DbValidationcomponent()  # noqa: E501
         if include_optional :
-            return Components(
-                db = wds_client.models.db_component.dbComponent(
-                    status = '0', 
-                    components = '0', ), 
-                disk_space = wds_client.models.component.component(
-                    status = '0', 
-                    details = '0', ), 
-                ping = wds_client.models.component.component(
-                    status = '0', 
-                    details = '0', ), 
-                permissions = wds_client.models.component.component(
-                    status = '0', 
-                    details = '0', )
+            return DbValidationcomponent(
+                status = '0', 
+                components = wds_client.models.db_validationcomponent_details.dbValidationcomponentDetails(
+                    database = '0', 
+                    validation_query = '0', )
             )
         else :
-            return Components(
+            return DbValidationcomponent(
         )
 
-    def testComponents(self):
-        """Test Components"""
+    def testDbValidationcomponent(self):
+        """Test DbValidationcomponent"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.84/test/test_db_component.py` & `wds-client-0.2.85/test/test_db_component.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,15 +33,17 @@
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = wds_client.models.db_component.DbComponent()  # noqa: E501
         if include_optional :
             return DbComponent(
                 status = '0', 
-                components = '0'
+                components = wds_client.models.component.component(
+                    status = '0', 
+                    details = '0', )
             )
         else :
             return DbComponent(
         )
 
     def testDbComponent(self):
         """Test DbComponent"""
```

### Comparing `wds-client-0.2.84/test/test_error_response.py` & `wds-client-0.2.85/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_general_wds_information_api.py` & `wds-client-0.2.85/test/test_general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_git.py` & `wds-client-0.2.85/test/test_git.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_inline_object.py` & `wds-client-0.2.85/test/test_inline_object.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_instances_api.py` & `wds-client-0.2.85/test/test_instances_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_record_attribute_definition.py` & `wds-client-0.2.85/test/test_record_attribute_definition.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_record_query_response.py` & `wds-client-0.2.85/test/test_record_query_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_record_request.py` & `wds-client-0.2.85/test/test_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_record_response.py` & `wds-client-0.2.85/test/test_record_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_record_type_schema.py` & `wds-client-0.2.85/test/test_record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_records_api.py` & `wds-client-0.2.85/test/test_records_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_request_body_search.py` & `wds-client-0.2.85/test/test_request_body_search.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_schema_api.py` & `wds-client-0.2.85/test/test_schema_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_search_operator.py` & `wds-client-0.2.85/test/test_search_operator.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_search_request.py` & `wds-client-0.2.85/test/test_search_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_search_sort_direction.py` & `wds-client-0.2.85/test/test_search_sort_direction.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_snapshots_api.py` & `wds-client-0.2.85/test/test_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_stack_trace_element.py` & `wds-client-0.2.85/test/test_stack_trace_element.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_status_response.py` & `wds-client-0.2.85/test/test_status_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,24 +36,27 @@
         # model = wds_client.models.status_response.StatusResponse()  # noqa: E501
         if include_optional :
             return StatusResponse(
                 status = '0', 
                 components = wds_client.models.components.components(
                     db = wds_client.models.db_component.dbComponent(
                         status = '0', ), 
-                    disk_space = wds_client.models.component.component(
+                    disk_space = wds_client.models.disk_space_component.diskSpaceComponent(
                         status = '0', 
-                        details = '0', ), 
+                        details = wds_client.models.disk_space_component_details.diskSpaceComponentDetails(
+                            total = '0', 
+                            free = null, 
+                            threshold = null, 
+                            exists = True, ), ), 
                     ping = wds_client.models.component.component(
-                        status = '0', 
-                        details = '0', ), 
-                    permissions = wds_client.models.component.component(
-                        status = '0', 
-                        details = '0', ), ), 
-                groups = '0'
+                        status = '0', ), 
+                    main_db = wds_client.models.db_validationcomponent.dbValidationcomponent(
+                        status = '0', ), 
+                    streaming_ds = wds_client.models.db_validationcomponent.dbValidationcomponent(
+                        status = '0', ), )
             )
         else :
             return StatusResponse(
         )
 
     def testStatusResponse(self):
         """Test StatusResponse"""
```

### Comparing `wds-client-0.2.84/test/test_tsv_upload_response.py` & `wds-client-0.2.85/test/test_tsv_upload_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/test/test_version_response.py` & `wds-client-0.2.85/test/test_version_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/__init__.py` & `wds-client-0.2.85/wds_client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.2.84"
+__version__ = "0.2.85"
 
 # import apis into sdk package
 from wds_client.api.general_wds_information_api import GeneralWDSInformationApi
 from wds_client.api.instances_api import InstancesApi
 from wds_client.api.records_api import RecordsApi
 from wds_client.api.schema_api import SchemaApi
 from wds_client.api.snapshots_api import SnapshotsApi
@@ -37,14 +37,18 @@
 from wds_client.models.batch_record_request import BatchRecordRequest
 from wds_client.models.batch_response import BatchResponse
 from wds_client.models.build import Build
 from wds_client.models.commit import Commit
 from wds_client.models.component import Component
 from wds_client.models.components import Components
 from wds_client.models.db_component import DbComponent
+from wds_client.models.db_validationcomponent import DbValidationcomponent
+from wds_client.models.db_validationcomponent_details import DbValidationcomponentDetails
+from wds_client.models.disk_space_component import DiskSpaceComponent
+from wds_client.models.disk_space_component_details import DiskSpaceComponentDetails
 from wds_client.models.error_response import ErrorResponse
 from wds_client.models.git import Git
 from wds_client.models.inline_object import InlineObject
 from wds_client.models.record_attribute_definition import RecordAttributeDefinition
 from wds_client.models.record_query_response import RecordQueryResponse
 from wds_client.models.record_request import RecordRequest
 from wds_client.models.record_response import RecordResponse
```

### Comparing `wds-client-0.2.84/wds_client/api/general_wds_information_api.py` & `wds-client-0.2.85/wds_client/api/general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/api/instances_api.py` & `wds-client-0.2.85/wds_client/api/instances_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/api/records_api.py` & `wds-client-0.2.85/wds_client/api/records_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/api/schema_api.py` & `wds-client-0.2.85/wds_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/api/snapshots_api.py` & `wds-client-0.2.85/wds_client/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/api_client.py` & `wds-client-0.2.85/wds_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.2.84/python'
+        self.user_agent = 'OpenAPI-Generator/0.2.85/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `wds-client-0.2.84/wds_client/configuration.py` & `wds-client-0.2.85/wds_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v0.2\n"\
-               "SDK Package Version: 0.2.84".\
+               "SDK Package Version: 0.2.85".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `wds-client-0.2.84/wds_client/exceptions.py` & `wds-client-0.2.85/wds_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/__init__.py` & `wds-client-0.2.85/wds_client/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 from wds_client.models.batch_record_request import BatchRecordRequest
 from wds_client.models.batch_response import BatchResponse
 from wds_client.models.build import Build
 from wds_client.models.commit import Commit
 from wds_client.models.component import Component
 from wds_client.models.components import Components
 from wds_client.models.db_component import DbComponent
+from wds_client.models.db_validationcomponent import DbValidationcomponent
+from wds_client.models.db_validationcomponent_details import DbValidationcomponentDetails
+from wds_client.models.disk_space_component import DiskSpaceComponent
+from wds_client.models.disk_space_component_details import DiskSpaceComponentDetails
 from wds_client.models.error_response import ErrorResponse
 from wds_client.models.git import Git
 from wds_client.models.inline_object import InlineObject
 from wds_client.models.record_attribute_definition import RecordAttributeDefinition
 from wds_client.models.record_query_response import RecordQueryResponse
 from wds_client.models.record_request import RecordRequest
 from wds_client.models.record_response import RecordResponse
```

### Comparing `wds-client-0.2.84/wds_client/models/attribute_schema.py` & `wds-client-0.2.85/wds_client/models/attribute_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/batch_operation.py` & `wds-client-0.2.85/wds_client/models/batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/batch_record_request.py` & `wds-client-0.2.85/wds_client/models/batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/batch_response.py` & `wds-client-0.2.85/wds_client/models/batch_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/build.py` & `wds-client-0.2.85/wds_client/models/build.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/commit.py` & `wds-client-0.2.85/wds_client/models/commit.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/component.py` & `wds-client-0.2.85/wds_client/models/component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/components.py` & `wds-client-0.2.85/wds_client/models/components.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,46 +30,51 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'db': 'DbComponent',
-        'disk_space': 'Component',
+        'disk_space': 'DiskSpaceComponent',
         'ping': 'Component',
-        'permissions': 'Component'
+        'main_db': 'DbValidationcomponent',
+        'streaming_ds': 'DbValidationcomponent'
     }
 
     attribute_map = {
         'db': 'db',
         'disk_space': 'diskSpace',
         'ping': 'ping',
-        'permissions': 'Permissions'
+        'main_db': 'mainDb',
+        'streaming_ds': 'streamingDs'
     }
 
-    def __init__(self, db=None, disk_space=None, ping=None, permissions=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, db=None, disk_space=None, ping=None, main_db=None, streaming_ds=None, local_vars_configuration=None):  # noqa: E501
         """Components - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._db = None
         self._disk_space = None
         self._ping = None
-        self._permissions = None
+        self._main_db = None
+        self._streaming_ds = None
         self.discriminator = None
 
         if db is not None:
             self.db = db
         if disk_space is not None:
             self.disk_space = disk_space
         if ping is not None:
             self.ping = ping
-        if permissions is not None:
-            self.permissions = permissions
+        if main_db is not None:
+            self.main_db = main_db
+        if streaming_ds is not None:
+            self.streaming_ds = streaming_ds
 
     @property
     def db(self):
         """Gets the db of this Components.  # noqa: E501
 
 
         :return: The db of this Components.  # noqa: E501
@@ -90,25 +95,25 @@
 
     @property
     def disk_space(self):
         """Gets the disk_space of this Components.  # noqa: E501
 
 
         :return: The disk_space of this Components.  # noqa: E501
-        :rtype: Component
+        :rtype: DiskSpaceComponent
         """
         return self._disk_space
 
     @disk_space.setter
     def disk_space(self, disk_space):
         """Sets the disk_space of this Components.
 
 
         :param disk_space: The disk_space of this Components.  # noqa: E501
-        :type: Component
+        :type: DiskSpaceComponent
         """
 
         self._disk_space = disk_space
 
     @property
     def ping(self):
         """Gets the ping of this Components.  # noqa: E501
@@ -127,33 +132,54 @@
         :param ping: The ping of this Components.  # noqa: E501
         :type: Component
         """
 
         self._ping = ping
 
     @property
-    def permissions(self):
-        """Gets the permissions of this Components.  # noqa: E501
+    def main_db(self):
+        """Gets the main_db of this Components.  # noqa: E501
 
 
-        :return: The permissions of this Components.  # noqa: E501
-        :rtype: Component
+        :return: The main_db of this Components.  # noqa: E501
+        :rtype: DbValidationcomponent
         """
-        return self._permissions
+        return self._main_db
 
-    @permissions.setter
-    def permissions(self, permissions):
-        """Sets the permissions of this Components.
+    @main_db.setter
+    def main_db(self, main_db):
+        """Sets the main_db of this Components.
 
 
-        :param permissions: The permissions of this Components.  # noqa: E501
-        :type: Component
+        :param main_db: The main_db of this Components.  # noqa: E501
+        :type: DbValidationcomponent
+        """
+
+        self._main_db = main_db
+
+    @property
+    def streaming_ds(self):
+        """Gets the streaming_ds of this Components.  # noqa: E501
+
+
+        :return: The streaming_ds of this Components.  # noqa: E501
+        :rtype: DbValidationcomponent
+        """
+        return self._streaming_ds
+
+    @streaming_ds.setter
+    def streaming_ds(self, streaming_ds):
+        """Sets the streaming_ds of this Components.
+
+
+        :param streaming_ds: The streaming_ds of this Components.  # noqa: E501
+        :type: DbValidationcomponent
         """
 
-        self._permissions = permissions
+        self._streaming_ds = streaming_ds
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
```

### Comparing `wds-client-0.2.84/wds_client/models/db_component.py` & `wds-client-0.2.85/wds_client/models/db_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'status': 'str',
-        'components': 'str'
+        'components': 'Component'
     }
 
     attribute_map = {
         'status': 'status',
         'components': 'components'
     }
 
@@ -80,25 +80,25 @@
 
     @property
     def components(self):
         """Gets the components of this DbComponent.  # noqa: E501
 
 
         :return: The components of this DbComponent.  # noqa: E501
-        :rtype: str
+        :rtype: Component
         """
         return self._components
 
     @components.setter
     def components(self, components):
         """Sets the components of this DbComponent.
 
 
         :param components: The components of this DbComponent.  # noqa: E501
-        :type: str
+        :type: Component
         """
 
         self._components = components
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `wds-client-0.2.84/wds_client/models/error_response.py` & `wds-client-0.2.85/wds_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/git.py` & `wds-client-0.2.85/wds_client/models/git.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/inline_object.py` & `wds-client-0.2.85/wds_client/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/record_attribute_definition.py` & `wds-client-0.2.85/wds_client/models/record_attribute_definition.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/record_query_response.py` & `wds-client-0.2.85/wds_client/models/record_query_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/record_request.py` & `wds-client-0.2.85/wds_client/models/record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/record_response.py` & `wds-client-0.2.85/wds_client/models/record_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/record_type_schema.py` & `wds-client-0.2.85/wds_client/models/record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/request_body_search.py` & `wds-client-0.2.85/wds_client/models/request_body_search.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/search_operator.py` & `wds-client-0.2.85/wds_client/models/search_operator.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/search_request.py` & `wds-client-0.2.85/wds_client/models/search_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/search_sort_direction.py` & `wds-client-0.2.85/wds_client/models/search_sort_direction.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/stack_trace_element.py` & `wds-client-0.2.85/wds_client/models/stack_trace_element.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/status_response.py` & `wds-client-0.2.85/wds_client/models/status_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,41 +30,36 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'status': 'str',
-        'components': 'Components',
-        'groups': 'str'
+        'components': 'Components'
     }
 
     attribute_map = {
         'status': 'status',
-        'components': 'components',
-        'groups': 'groups'
+        'components': 'components'
     }
 
-    def __init__(self, status=None, components=None, groups=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, status=None, components=None, local_vars_configuration=None):  # noqa: E501
         """StatusResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._status = None
         self._components = None
-        self._groups = None
         self.discriminator = None
 
         if status is not None:
             self.status = status
         if components is not None:
             self.components = components
-        if groups is not None:
-            self.groups = groups
 
     @property
     def status(self):
         """Gets the status of this StatusResponse.  # noqa: E501
 
 
         :return: The status of this StatusResponse.  # noqa: E501
@@ -100,35 +95,14 @@
 
         :param components: The components of this StatusResponse.  # noqa: E501
         :type: Components
         """
 
         self._components = components
 
-    @property
-    def groups(self):
-        """Gets the groups of this StatusResponse.  # noqa: E501
-
-
-        :return: The groups of this StatusResponse.  # noqa: E501
-        :rtype: str
-        """
-        return self._groups
-
-    @groups.setter
-    def groups(self, groups):
-        """Sets the groups of this StatusResponse.
-
-
-        :param groups: The groups of this StatusResponse.  # noqa: E501
-        :type: str
-        """
-
-        self._groups = groups
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `wds-client-0.2.84/wds_client/models/tsv_upload_response.py` & `wds-client-0.2.85/wds_client/models/tsv_upload_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/models/version_response.py` & `wds-client-0.2.85/wds_client/models/version_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client/rest.py` & `wds-client-0.2.85/wds_client/rest.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.84/wds_client.egg-info/SOURCES.txt` & `wds-client-0.2.85/wds_client.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 test/test_batch_record_request.py
 test/test_batch_response.py
 test/test_build.py
 test/test_commit.py
 test/test_component.py
 test/test_components.py
 test/test_db_component.py
+test/test_db_validationcomponent.py
+test/test_db_validationcomponent_details.py
+test/test_disk_space_component.py
+test/test_disk_space_component_details.py
 test/test_error_response.py
 test/test_general_wds_information_api.py
 test/test_git.py
 test/test_inline_object.py
 test/test_instances_api.py
 test/test_record_attribute_definition.py
 test/test_record_query_response.py
@@ -53,14 +57,18 @@
 wds_client/models/batch_record_request.py
 wds_client/models/batch_response.py
 wds_client/models/build.py
 wds_client/models/commit.py
 wds_client/models/component.py
 wds_client/models/components.py
 wds_client/models/db_component.py
+wds_client/models/db_validationcomponent.py
+wds_client/models/db_validationcomponent_details.py
+wds_client/models/disk_space_component.py
+wds_client/models/disk_space_component_details.py
 wds_client/models/error_response.py
 wds_client/models/git.py
 wds_client/models/inline_object.py
 wds_client/models/record_attribute_definition.py
 wds_client/models/record_query_response.py
 wds_client/models/record_request.py
 wds_client/models/record_response.py
```

