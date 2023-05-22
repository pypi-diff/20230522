# Comparing `tmp/qwak_core-0.0.69.tar.gz` & `tmp/qwak_core-0.0.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.69.tar", max compression
+gzip compressed data, was "qwak_core-0.0.70.tar", max compression
```

## Comparing `qwak_core-0.0.69.tar` & `qwak_core-0.0.70.tar`

### file list

```diff
@@ -1,582 +1,582 @@
--rw-r--r--   0        0        0      264 2023-05-21 15:32:09.852429 qwak_core-0.0.69/README.md
--rw-r--r--   0        0        0        0 2023-05-21 15:34:00.853152 qwak_core-0.0.69/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-21 15:34:00.881152 qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-21 15:33:38.193006 qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.881152 qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-21 15:34:00.877153 qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-21 15:33:37.785004 qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.877153 qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-21 15:34:00.877153 qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-21 15:33:37.989005 qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.877153 qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-21 15:34:00.869152 qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-21 15:33:37.185000 qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-21 15:34:00.869152 qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-21 15:34:00.873153 qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-21 15:33:37.385001 qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.873153 qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-21 15:34:00.873153 qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-21 15:33:37.581002 qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.873153 qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-21 15:34:00.857152 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-21 15:33:36.956998 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-21 15:34:00.857152 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-21 15:34:00.857152 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-21 15:33:38.389007 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.857152 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-21 15:34:00.861153 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-21 15:33:38.805010 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.865152 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-21 15:34:00.865152 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-21 15:33:39.001011 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-21 15:34:00.865152 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-21 15:34:00.861153 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-21 15:33:38.613009 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.861153 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-21 15:34:00.865152 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-21 15:33:39.197013 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.869152 qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-21 15:34:00.913153 qwak_core-0.0.69/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-21 15:33:41.949030 qwak_core-0.0.69/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.913153 qwak_core-0.0.69/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-21 15:34:00.917153 qwak_core-0.0.69/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-21 15:33:42.153032 qwak_core-0.0.69/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-21 15:34:00.917153 qwak_core-0.0.69/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-21 15:34:01.049154 qwak_core-0.0.69/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-21 15:33:48.209071 qwak_core-0.0.69/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.049154 qwak_core-0.0.69/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-21 15:34:01.049154 qwak_core-0.0.69/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-21 15:33:48.401072 qwak_core-0.0.69/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-21 15:34:01.053154 qwak_core-0.0.69/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-21 15:34:01.057154 qwak_core-0.0.69/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-21 15:33:49.413078 qwak_core-0.0.69/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-21 15:34:01.057154 qwak_core-0.0.69/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-21 15:34:01.053154 qwak_core-0.0.69/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-21 15:33:49.209077 qwak_core-0.0.69/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.053154 qwak_core-0.0.69/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-05-21 15:34:01.057154 qwak_core-0.0.69/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-05-21 15:33:49.613080 qwak_core-0.0.69/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.057154 qwak_core-0.0.69/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-21 15:34:01.061154 qwak_core-0.0.69/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-21 15:33:49.813081 qwak_core-0.0.69/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-21 15:34:01.061154 qwak_core-0.0.69/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-21 15:34:01.157154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-21 15:33:58.237136 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.157154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-05-21 15:34:01.153154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-05-21 15:33:57.849133 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.153154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-21 15:34:01.153154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-21 15:33:58.041134 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.153154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-21 15:34:01.145154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-21 15:33:57.445130 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-21 15:34:01.149154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-21 15:34:01.149154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-21 15:33:57.641132 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.149154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-21 15:34:01.161154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-21 15:33:58.793139 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.165154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-21 15:34:01.161154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-21 15:33:58.609138 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.161154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-21 15:34:01.157154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-21 15:33:58.421137 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.157154 qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-21 15:34:01.145154 qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-21 15:33:57.237129 qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.145154 qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-21 15:34:01.141154 qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-21 15:33:56.821126 qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.141154 qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-21 15:34:01.141154 qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-21 15:33:57.037128 qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-21 15:34:01.145154 qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-21 15:34:01.089154 qwak_core-0.0.69/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-21 15:33:51.845094 qwak_core-0.0.69/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-21 15:34:01.089154 qwak_core-0.0.69/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-21 15:34:01.085154 qwak_core-0.0.69/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-21 15:33:51.637093 qwak_core-0.0.69/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.085154 qwak_core-0.0.69/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-21 15:34:01.077154 qwak_core-0.0.69/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-21 15:33:51.237090 qwak_core-0.0.69/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.077154 qwak_core-0.0.69/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-21 15:34:01.077154 qwak_core-0.0.69/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-21 15:33:51.433091 qwak_core-0.0.69/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.081154 qwak_core-0.0.69/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-21 15:34:01.081154 qwak_core-0.0.69/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-21 15:33:52.057096 qwak_core-0.0.69/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-21 15:34:01.081154 qwak_core-0.0.69/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-21 15:34:01.081154 qwak_core-0.0.69/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-21 15:33:52.505098 qwak_core-0.0.69/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-21 15:34:01.085154 qwak_core-0.0.69/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-21 15:34:01.093154 qwak_core-0.0.69/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-21 15:33:52.933101 qwak_core-0.0.69/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.097154 qwak_core-0.0.69/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-21 15:34:01.097154 qwak_core-0.0.69/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-21 15:33:53.129103 qwak_core-0.0.69/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-21 15:34:01.097154 qwak_core-0.0.69/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-21 15:34:01.069154 qwak_core-0.0.69/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-21 15:33:50.633086 qwak_core-0.0.69/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.069154 qwak_core-0.0.69/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-21 15:34:01.073154 qwak_core-0.0.69/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-21 15:33:50.833088 qwak_core-0.0.69/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-21 15:34:01.073154 qwak_core-0.0.69/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-21 15:34:01.065154 qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-21 15:33:50.221084 qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.065154 qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-21 15:34:01.061154 qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-21 15:33:50.021082 qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.065154 qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-21 15:34:01.065154 qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-21 15:33:50.433085 qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-21 15:34:01.069154 qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-21 15:34:00.901153 qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-21 15:33:40.945024 qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.901153 qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-21 15:34:00.905153 qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-21 15:33:41.137025 qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.905153 qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-21 15:34:00.905153 qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-21 15:33:41.345027 qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-21 15:34:00.909153 qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-21 15:34:01.029153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-21 15:33:46.981063 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.029153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-21 15:34:01.025153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-21 15:33:46.773062 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-21 15:34:01.025153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-21 15:34:01.005153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-21 15:33:44.769049 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.005153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-21 15:34:01.001153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-21 15:33:44.553047 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.005153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-21 15:34:00.997153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-21 15:33:43.853043 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.997153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-21 15:34:01.001153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-21 15:33:44.333046 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-21 15:34:01.001153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-21 15:34:01.009153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-21 15:33:45.021050 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.009153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-21 15:34:01.009153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-21 15:33:45.237052 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-21 15:34:01.009153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25222 2023-05-21 15:34:00.997153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37429 2023-05-21 15:33:44.105044 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.001153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-21 15:34:01.013153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-21 15:33:45.441053 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.013153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     7284 2023-05-21 15:34:01.013153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0     8518 2023-05-21 15:33:45.649054 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.017153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-21 15:34:01.029153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-21 15:34:00.209148 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.033154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-21 15:34:01.033154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-21 15:34:00.441150 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-21 15:34:01.033154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-21 15:34:01.033154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-21 15:33:47.585067 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.037154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-21 15:34:01.037154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-21 15:33:47.821068 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-21 15:34:01.037154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-21 15:34:01.041154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-21 15:33:48.013069 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.041154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-21 15:34:01.045154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-21 15:33:48.809074 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.045154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-21 15:34:01.041154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-21 15:33:48.601073 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-21 15:34:01.041154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-21 15:34:01.045154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-21 15:33:49.005076 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.045154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-21 15:34:01.017153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-21 15:33:45.865056 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.017153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-21 15:34:01.017153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-21 15:33:46.077057 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.021154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-21 15:34:01.021154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-21 15:33:46.293058 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-21 15:34:01.021154 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-21 15:34:01.025153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-21 15:33:46.545060 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.025153 qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-21 15:34:01.165154 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-21 15:33:58.993140 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.165154 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-21 15:34:01.165154 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-21 15:33:59.189142 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-21 15:34:01.169155 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-21 15:34:01.169155 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-21 15:33:59.385143 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.169155 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-21 15:34:01.173154 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-21 15:33:59.597144 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-21 15:34:01.173154 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-21 15:34:01.173154 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-21 15:33:59.805146 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-21 15:34:01.173154 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-21 15:34:01.177154 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-21 15:33:59.997147 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.177154 qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-21 15:34:01.097154 qwak_core-0.0.69/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-21 15:33:53.317104 qwak_core-0.0.69/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.101154 qwak_core-0.0.69/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-21 15:34:01.101154 qwak_core-0.0.69/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-21 15:33:53.509105 qwak_core-0.0.69/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-21 15:34:01.101154 qwak_core-0.0.69/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-21 15:34:00.941153 qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-21 15:33:42.993037 qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.953153 qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-21 15:34:00.965153 qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-21 15:33:43.197039 qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.969153 qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-21 15:34:00.981153 qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-21 15:33:43.413040 qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-21 15:34:00.985153 qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-21 15:34:00.989153 qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-21 15:33:43.621041 qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.993153 qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-21 15:34:01.073154 qwak_core-0.0.69/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-21 15:33:51.033089 qwak_core-0.0.69/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-21 15:34:01.073154 qwak_core-0.0.69/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-05-21 15:34:01.105154 qwak_core-0.0.69/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-05-21 15:33:53.705106 qwak_core-0.0.69/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.105154 qwak_core-0.0.69/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-05-21 15:34:01.105154 qwak_core-0.0.69/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-05-21 15:33:53.897107 qwak_core-0.0.69/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-05-21 15:34:01.105154 qwak_core-0.0.69/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-21 15:34:01.121154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-21 15:33:55.053115 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.121154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-21 15:34:01.121154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-21 15:33:55.249116 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.121154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-21 15:34:01.125154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-21 15:33:55.441117 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.125154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-21 15:34:01.125154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-21 15:33:55.633119 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.125154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-21 15:34:01.129154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-21 15:33:55.825120 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.129154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-21 15:34:01.129154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-21 15:33:56.033121 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-21 15:34:01.133154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-21 15:34:01.133154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-21 15:33:56.229122 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.133154 qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-21 15:34:01.109154 qwak_core-0.0.69/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-21 15:33:54.265110 qwak_core-0.0.69/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.113154 qwak_core-0.0.69/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-21 15:34:01.117154 qwak_core-0.0.69/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-21 15:33:54.857114 qwak_core-0.0.69/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.117154 qwak_core-0.0.69/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-21 15:34:01.113154 qwak_core-0.0.69/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-21 15:33:54.453111 qwak_core-0.0.69/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-21 15:34:01.113154 qwak_core-0.0.69/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-05-21 15:34:01.113154 qwak_core-0.0.69/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-05-21 15:33:54.645112 qwak_core-0.0.69/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.117154 qwak_core-0.0.69/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-21 15:34:01.093154 qwak_core-0.0.69/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-21 15:33:52.713100 qwak_core-0.0.69/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-21 15:34:01.093154 qwak_core-0.0.69/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-21 15:34:00.897153 qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-21 15:33:42.545034 qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-21 15:34:00.897153 qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-21 15:34:00.893153 qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-21 15:33:42.349033 qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.897153 qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-21 15:34:00.901153 qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-21 15:33:42.765036 qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-21 15:34:00.901153 qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-21 15:34:01.089154 qwak_core-0.0.69/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-21 15:33:52.289097 qwak_core-0.0.69/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-21 15:34:01.089154 qwak_core-0.0.69/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-21 15:34:01.109154 qwak_core-0.0.69/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-21 15:33:54.081109 qwak_core-0.0.69/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-21 15:34:01.109154 qwak_core-0.0.69/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-21 15:34:00.893153 qwak_core-0.0.69/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-21 15:33:40.177019 qwak_core-0.0.69/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.893153 qwak_core-0.0.69/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-21 15:34:00.889153 qwak_core-0.0.69/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-21 15:33:39.985018 qwak_core-0.0.69/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-21 15:34:00.889153 qwak_core-0.0.69/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-21 15:34:00.881152 qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-21 15:33:39.393014 qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.885153 qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-21 15:34:00.885153 qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-21 15:33:39.585015 qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.885153 qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-21 15:34:00.889153 qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-21 15:33:39.781016 qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-21 15:34:00.889153 qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-21 15:34:01.137154 qwak_core-0.0.69/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-21 15:33:56.629125 qwak_core-0.0.69/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-21 15:34:01.137154 qwak_core-0.0.69/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-21 15:34:01.137154 qwak_core-0.0.69/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-21 15:33:56.429124 qwak_core-0.0.69/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:01.137154 qwak_core-0.0.69/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-21 15:34:00.909153 qwak_core-0.0.69/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    15881 2023-05-21 15:33:41.545028 qwak_core-0.0.69/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.909153 qwak_core-0.0.69/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-21 15:34:00.909153 qwak_core-0.0.69/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-21 15:33:41.753029 qwak_core-0.0.69/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 15:34:00.913153 qwak_core-0.0.69/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-21 15:34:08.873204 qwak_core-0.0.69/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-21 15:34:08.873204 qwak_core-0.0.69/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14847 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-21 15:32:09.856429 qwak_core-0.0.69/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-21 15:32:09.860429 qwak_core-0.0.69/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-21 15:32:09.864429 qwak_core-0.0.69/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.69/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.69/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-22 10:47:44.669654 qwak_core-0.0.70/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 10:49:54.866586 qwak_core-0.0.70/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-22 10:49:54.898586 qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-22 10:49:27.026383 qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.898586 qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-22 10:49:54.890586 qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-22 10:49:26.494379 qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.894586 qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-22 10:49:54.894586 qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-22 10:49:26.762381 qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.894586 qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-22 10:49:54.882586 qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-22 10:49:25.802374 qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-22 10:49:54.886586 qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-22 10:49:54.886586 qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-22 10:49:26.034375 qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.886586 qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-22 10:49:54.890586 qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-22 10:49:26.266377 qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.890586 qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-22 10:49:54.866586 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-22 10:49:25.570372 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-22 10:49:54.870586 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-22 10:49:54.870586 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-22 10:49:27.302385 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.870586 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-22 10:49:54.874586 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-22 10:49:27.786388 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.878586 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-22 10:49:54.878586 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-22 10:49:28.022390 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-22 10:49:54.878586 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-22 10:49:54.874586 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-22 10:49:27.538386 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.874586 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-22 10:49:54.882586 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-22 10:49:28.254392 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.882586 qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-22 10:49:54.934586 qwak_core-0.0.70/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-22 10:49:31.534416 qwak_core-0.0.70/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.934586 qwak_core-0.0.70/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-22 10:49:54.938586 qwak_core-0.0.70/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-22 10:49:31.778417 qwak_core-0.0.70/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-22 10:49:54.938586 qwak_core-0.0.70/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-22 10:49:55.022587 qwak_core-0.0.70/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-22 10:49:39.302472 qwak_core-0.0.70/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.022587 qwak_core-0.0.70/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-22 10:49:55.026587 qwak_core-0.0.70/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-22 10:49:39.550474 qwak_core-0.0.70/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-22 10:49:55.026587 qwak_core-0.0.70/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-22 10:49:55.030587 qwak_core-0.0.70/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-22 10:49:40.746483 qwak_core-0.0.70/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-22 10:49:55.030587 qwak_core-0.0.70/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-22 10:49:55.026587 qwak_core-0.0.70/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-22 10:49:40.494481 qwak_core-0.0.70/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.030587 qwak_core-0.0.70/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-05-22 10:49:55.034587 qwak_core-0.0.70/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-05-22 10:49:40.974485 qwak_core-0.0.70/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.034587 qwak_core-0.0.70/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-22 10:49:55.034587 qwak_core-0.0.70/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-22 10:49:41.210486 qwak_core-0.0.70/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-22 10:49:55.038587 qwak_core-0.0.70/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-22 10:49:55.150588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-22 10:49:51.726563 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.150588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-05-22 10:49:55.146588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-05-22 10:49:51.214559 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.146588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-22 10:49:55.146588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-22 10:49:51.458561 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.146588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-22 10:49:55.138588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-22 10:49:50.686555 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-22 10:49:55.142588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-22 10:49:55.142588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-22 10:49:50.942557 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.142588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-22 10:49:55.158588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-22 10:49:52.462568 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.158588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-22 10:49:55.154588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-22 10:49:52.218567 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.154588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-22 10:49:55.150588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-22 10:49:51.970565 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.154588 qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-22 10:49:55.138588 qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-22 10:49:50.434554 qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.138588 qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-22 10:49:55.130588 qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-22 10:49:49.830549 qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.130588 qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-22 10:49:55.134588 qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-22 10:49:50.122551 qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-22 10:49:55.134588 qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-05-22 10:49:55.070587 qwak_core-0.0.70/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-05-22 10:49:43.654504 qwak_core-0.0.70/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-05-22 10:49:55.070587 qwak_core-0.0.70/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-22 10:49:55.066587 qwak_core-0.0.70/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-22 10:49:43.414502 qwak_core-0.0.70/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.066587 qwak_core-0.0.70/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-22 10:49:55.054587 qwak_core-0.0.70/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-22 10:49:42.922499 qwak_core-0.0.70/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.058587 qwak_core-0.0.70/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-22 10:49:55.058587 qwak_core-0.0.70/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-22 10:49:43.162500 qwak_core-0.0.70/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.058587 qwak_core-0.0.70/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-22 10:49:55.062587 qwak_core-0.0.70/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-22 10:49:43.898506 qwak_core-0.0.70/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-22 10:49:55.062587 qwak_core-0.0.70/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-22 10:49:55.062587 qwak_core-0.0.70/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-22 10:49:44.402510 qwak_core-0.0.70/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-22 10:49:55.066587 qwak_core-0.0.70/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-22 10:49:55.078587 qwak_core-0.0.70/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-22 10:49:44.898513 qwak_core-0.0.70/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.078587 qwak_core-0.0.70/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-22 10:49:55.078587 qwak_core-0.0.70/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-22 10:49:45.126515 qwak_core-0.0.70/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-22 10:49:55.082588 qwak_core-0.0.70/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-22 10:49:55.046587 qwak_core-0.0.70/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-22 10:49:42.210494 qwak_core-0.0.70/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.050587 qwak_core-0.0.70/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-22 10:49:55.050587 qwak_core-0.0.70/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-22 10:49:42.446495 qwak_core-0.0.70/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-22 10:49:55.050587 qwak_core-0.0.70/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-22 10:49:55.042587 qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-22 10:49:41.706490 qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.042587 qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-22 10:49:55.038587 qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-22 10:49:41.470488 qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.038587 qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-22 10:49:55.046587 qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-22 10:49:41.978492 qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-22 10:49:55.046587 qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-22 10:49:54.922586 qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-22 10:49:30.346407 qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.922586 qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-22 10:49:54.922586 qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-22 10:49:30.578409 qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.926586 qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-22 10:49:54.926586 qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-22 10:49:30.826410 qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-22 10:49:54.926586 qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-22 10:49:54.998587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-22 10:49:37.870462 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.998587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-22 10:49:54.994587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-22 10:49:37.630460 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-22 10:49:54.998587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-22 10:49:54.970587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-22 10:49:35.246443 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.970587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-22 10:49:54.966587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-22 10:49:34.974441 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.970587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-22 10:49:54.958587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-22 10:49:34.146435 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.962586 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-22 10:49:54.966587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-22 10:49:34.694439 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-22 10:49:54.966587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-22 10:49:54.974587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-22 10:49:35.494444 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.974587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-22 10:49:54.974587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-22 10:49:35.754446 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-22 10:49:54.978587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25222 2023-05-22 10:49:54.962586 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37429 2023-05-22 10:49:34.414437 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.962586 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-22 10:49:54.978587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-22 10:49:36.002448 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.978587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     7284 2023-05-22 10:49:54.982587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0     8518 2023-05-22 10:49:36.274450 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.982587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-22 10:49:55.002587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-22 10:49:54.266582 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.002587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-22 10:49:55.002587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-22 10:49:54.522583 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-22 10:49:55.006587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-22 10:49:55.006587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-22 10:49:38.590467 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.006587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-22 10:49:55.010587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-22 10:49:38.826469 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-22 10:49:55.010587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-22 10:49:55.010587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-22 10:49:39.058471 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.014587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-22 10:49:55.018587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-22 10:49:40.030478 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.018587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-22 10:49:55.014587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-22 10:49:39.790476 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-22 10:49:55.014587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-22 10:49:55.018587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-22 10:49:40.262479 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.022587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-22 10:49:54.986587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-22 10:49:36.566452 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.986587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-22 10:49:54.986587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-22 10:49:36.846454 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.990587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-22 10:49:54.990587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-22 10:49:37.138457 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-22 10:49:54.990587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-22 10:49:54.994587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-22 10:49:37.390458 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.994587 qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-22 10:49:55.158588 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-22 10:49:52.702570 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.162588 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-22 10:49:55.162588 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-22 10:49:52.962572 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-22 10:49:55.162588 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-22 10:49:55.166588 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-22 10:49:53.222574 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.166588 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-22 10:49:55.166588 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-22 10:49:53.486576 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-22 10:49:55.170588 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-22 10:49:55.170588 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-22 10:49:53.762578 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-22 10:49:55.170588 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-22 10:49:55.174588 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-22 10:49:54.014580 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.174588 qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-22 10:49:55.082588 qwak_core-0.0.70/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-22 10:49:45.378517 qwak_core-0.0.70/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.082588 qwak_core-0.0.70/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-22 10:49:55.086588 qwak_core-0.0.70/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-22 10:49:45.610519 qwak_core-0.0.70/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-22 10:49:55.086588 qwak_core-0.0.70/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-22 10:49:54.942587 qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-22 10:49:33.038426 qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.946586 qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-22 10:49:54.946586 qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-22 10:49:33.290428 qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.950586 qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-22 10:49:54.950586 qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-22 10:49:33.574431 qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-22 10:49:54.954587 qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-22 10:49:54.954587 qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-22 10:49:33.846433 qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.958587 qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-22 10:49:55.054587 qwak_core-0.0.70/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-22 10:49:42.682497 qwak_core-0.0.70/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-22 10:49:55.054587 qwak_core-0.0.70/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-05-22 10:49:55.086588 qwak_core-0.0.70/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-05-22 10:49:45.858520 qwak_core-0.0.70/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.090587 qwak_core-0.0.70/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-05-22 10:49:55.090587 qwak_core-0.0.70/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-05-22 10:49:46.098522 qwak_core-0.0.70/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-05-22 10:49:55.090587 qwak_core-0.0.70/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-22 10:49:55.106588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-22 10:49:47.558533 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.106588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-22 10:49:55.110588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-22 10:49:47.798534 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.110588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-22 10:49:55.110588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-22 10:49:48.054536 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.114588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-22 10:49:55.114588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-22 10:49:48.286538 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.114588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-22 10:49:55.118588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-22 10:49:48.542540 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.118588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-22 10:49:55.118588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-22 10:49:48.802542 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-22 10:49:55.122588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-22 10:49:55.122588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-22 10:49:49.042544 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.122588 qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-22 10:49:55.094588 qwak_core-0.0.70/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-22 10:49:46.578525 qwak_core-0.0.70/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.098588 qwak_core-0.0.70/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-22 10:49:55.102588 qwak_core-0.0.70/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-22 10:49:47.318531 qwak_core-0.0.70/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.106588 qwak_core-0.0.70/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-22 10:49:55.098588 qwak_core-0.0.70/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-22 10:49:46.830527 qwak_core-0.0.70/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-22 10:49:55.098588 qwak_core-0.0.70/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-05-22 10:49:55.102588 qwak_core-0.0.70/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-05-22 10:49:47.062529 qwak_core-0.0.70/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.102588 qwak_core-0.0.70/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-22 10:49:55.074587 qwak_core-0.0.70/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-22 10:49:44.654512 qwak_core-0.0.70/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-22 10:49:55.078587 qwak_core-0.0.70/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-22 10:49:54.914586 qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-22 10:49:32.418422 qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-22 10:49:54.918586 qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-22 10:49:54.914586 qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-22 10:49:32.106420 qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.914586 qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-22 10:49:54.918586 qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-22 10:49:32.750424 qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-22 10:49:54.918586 qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-22 10:49:55.070587 qwak_core-0.0.70/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-22 10:49:44.142508 qwak_core-0.0.70/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-22 10:49:55.074587 qwak_core-0.0.70/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-22 10:49:55.094588 qwak_core-0.0.70/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-22 10:49:46.334524 qwak_core-0.0.70/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-22 10:49:55.094588 qwak_core-0.0.70/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-22 10:49:54.910586 qwak_core-0.0.70/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-22 10:49:29.418400 qwak_core-0.0.70/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.910586 qwak_core-0.0.70/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-22 10:49:54.906586 qwak_core-0.0.70/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-22 10:49:29.190399 qwak_core-0.0.70/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-22 10:49:54.910586 qwak_core-0.0.70/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-22 10:49:54.898586 qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-22 10:49:28.482393 qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.902586 qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-22 10:49:54.902586 qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-22 10:49:28.714395 qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.902586 qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-22 10:49:54.906586 qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-22 10:49:28.954397 qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-22 10:49:54.906586 qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-22 10:49:55.126588 qwak_core-0.0.70/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-22 10:49:49.574547 qwak_core-0.0.70/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-22 10:49:55.130588 qwak_core-0.0.70/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-22 10:49:55.126588 qwak_core-0.0.70/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-22 10:49:49.302545 qwak_core-0.0.70/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:55.126588 qwak_core-0.0.70/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-22 10:49:54.930586 qwak_core-0.0.70/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    15881 2023-05-22 10:49:31.062412 qwak_core-0.0.70/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.930586 qwak_core-0.0.70/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-22 10:49:54.930586 qwak_core-0.0.70/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-22 10:49:31.294414 qwak_core-0.0.70/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 10:49:54.934586 qwak_core-0.0.70/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-22 10:49:58.118610 qwak_core-0.0.70/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-22 10:49:58.118610 qwak_core-0.0.70/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-22 10:47:44.669654 qwak_core-0.0.70/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14847 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-22 10:47:44.673654 qwak_core-0.0.70/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-22 10:47:44.677654 qwak_core-0.0.70/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-22 10:47:44.681654 qwak_core-0.0.70/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.70/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.70/PKG-INFO
```

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dqwak/logging/log_source.proto\x12\x14qwak.logging.service\"\xed\x03\n\tLogSource\x12\x41\n\rmodel_runtime\x18\x01 \x01(\x0b\x32(.qwak.logging.service.ModelRuntimeSourceH\x00\x12?\n\x0cremote_build\x18\x02 \x01(\x0b\x32\'.qwak.logging.service.RemoteBuildSourceH\x00\x12M\n\x13inference_execution\x18\x03 \x01(\x0b\x32..qwak.logging.service.InferenceExecutionSourceH\x00\x12P\n\x15streaming_feature_set\x18\x04 \x01(\x0b\x32/.qwak.logging.service.StreamingFeatureSetSourceH\x00\x12g\n!streaming_aggregation_feature_set\x18\x05 \x01(\x0b\x32:.qwak.logging.service.StreamingAggregationFeatureSetSourceH\x00\x12H\n\x11\x62\x61tch_feature_set\x18\x06 \x01(\x0b\x32+.qwak.logging.service.BatchFeatureSetSourceH\x00\x42\x08\n\x06source\"8\n\x11RemoteBuildSource\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x11\n\tphase_ids\x18\x02 \x03(\t\"N\n\x12ModelRuntimeSource\x12\x17\n\rdeployment_id\x18\x01 \x01(\tH\x00\x12\x12\n\x08\x62uild_id\x18\x02 \x01(\tH\x00\x42\x0b\n\tsearch_by\"`\n\x18InferenceExecutionSource\x12\x1a\n\x10inference_job_id\x18\x01 \x01(\tH\x00\x12\x1b\n\x11inference_task_id\x18\x02 \x01(\tH\x00\x42\x0b\n\tsearch_by\"\xbf\x01\n\x19StreamingFeatureSetSource\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x34\n\x07offline\x18\x03 \x01(\x0b\x32!.qwak.logging.service.OfflineTypeH\x00\x12\x32\n\x06online\x18\x04 \x01(\x0b\x32 .qwak.logging.service.OnlineTypeH\x00\x42\x06\n\x04type\"W\n\x15\x42\x61tchFeatureSetSource\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x17\n\x0f\x66\x65\x61tureset_name\x18\x02 \x01(\t\x12\x0e\n\x06run_id\x18\x03 \x01(\t\"\xdb\x01\n$StreamingAggregationFeatureSetSource\x12\x37\n\trow_level\x18\x01 \x01(\x0b\x32\".qwak.logging.service.RowLevelTypeH\x00\x12:\n\ncompaction\x18\x02 \x01(\x0b\x32$.qwak.logging.service.CompactionTypeH\x00\x12\x36\n\x08\x62\x61\x63kfill\x18\x03 \x01(\x0b\x32\".qwak.logging.service.BackfillTypeH\x00\x42\x06\n\x04type\">\n\nOnlineType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\"O\n\x0bOfflineType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x0e\n\x06run_id\x18\x03 \x01(\t\"@\n\x0cRowLevelType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\"R\n\x0e\x43ompactionType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x0e\n\x06run_id\x18\x03 \x01(\t\"@\n\x0c\x42\x61\x63kfillType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\tB\"\n\x1e\x63om.qwak.ai.logging.reader.apiP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dqwak/logging/log_source.proto\x12\x14qwak.logging.service\"\xca\x04\n\tLogSource\x12\x41\n\rmodel_runtime\x18\x01 \x01(\x0b\x32(.qwak.logging.service.ModelRuntimeSourceH\x00\x12?\n\x0cremote_build\x18\x02 \x01(\x0b\x32\'.qwak.logging.service.RemoteBuildSourceH\x00\x12M\n\x13inference_execution\x18\x03 \x01(\x0b\x32..qwak.logging.service.InferenceExecutionSourceH\x00\x12P\n\x15streaming_feature_set\x18\x04 \x01(\x0b\x32/.qwak.logging.service.StreamingFeatureSetSourceH\x00\x12g\n!streaming_aggregation_feature_set\x18\x05 \x01(\x0b\x32:.qwak.logging.service.StreamingAggregationFeatureSetSourceH\x00\x12H\n\x11\x62\x61tch_feature_set\x18\x06 \x01(\x0b\x32+.qwak.logging.service.BatchFeatureSetSourceH\x00\x12[\n\x1breal_time_feature_extractor\x18\x07 \x01(\x0b\x32\x34.qwak.logging.service.RealTimeFeatureExtractorSourceH\x00\x42\x08\n\x06source\"8\n\x11RemoteBuildSource\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x11\n\tphase_ids\x18\x02 \x03(\t\"N\n\x12ModelRuntimeSource\x12\x17\n\rdeployment_id\x18\x01 \x01(\tH\x00\x12\x12\n\x08\x62uild_id\x18\x02 \x01(\tH\x00\x42\x0b\n\tsearch_by\"`\n\x18InferenceExecutionSource\x12\x1a\n\x10inference_job_id\x18\x01 \x01(\tH\x00\x12\x1b\n\x11inference_task_id\x18\x02 \x01(\tH\x00\x42\x0b\n\tsearch_by\"\xbf\x01\n\x19StreamingFeatureSetSource\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x34\n\x07offline\x18\x03 \x01(\x0b\x32!.qwak.logging.service.OfflineTypeH\x00\x12\x32\n\x06online\x18\x04 \x01(\x0b\x32 .qwak.logging.service.OnlineTypeH\x00\x42\x06\n\x04type\"W\n\x15\x42\x61tchFeatureSetSource\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x17\n\x0f\x66\x65\x61tureset_name\x18\x02 \x01(\t\x12\x0e\n\x06run_id\x18\x03 \x01(\t\"\xdb\x01\n$StreamingAggregationFeatureSetSource\x12\x37\n\trow_level\x18\x01 \x01(\x0b\x32\".qwak.logging.service.RowLevelTypeH\x00\x12:\n\ncompaction\x18\x02 \x01(\x0b\x32$.qwak.logging.service.CompactionTypeH\x00\x12\x36\n\x08\x62\x61\x63kfill\x18\x03 \x01(\x0b\x32\".qwak.logging.service.BackfillTypeH\x00\x42\x06\n\x04type\">\n\nOnlineType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\"O\n\x0bOfflineType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x0e\n\x06run_id\x18\x03 \x01(\t\"@\n\x0cRowLevelType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\"R\n\x0e\x43ompactionType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x0e\n\x06run_id\x18\x03 \x01(\t\"@\n\x0c\x42\x61\x63kfillType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\"H\n\x1eRealTimeFeatureExtractorSource\x12&\n\x1ereal_time_feature_extractor_id\x18\x01 \x01(\tB\"\n\x1e\x63om.qwak.ai.logging.reader.apiP\x01\x62\x06proto3')
 
 
 
 _LOGSOURCE = DESCRIPTOR.message_types_by_name['LogSource']
 _REMOTEBUILDSOURCE = DESCRIPTOR.message_types_by_name['RemoteBuildSource']
 _MODELRUNTIMESOURCE = DESCRIPTOR.message_types_by_name['ModelRuntimeSource']
 _INFERENCEEXECUTIONSOURCE = DESCRIPTOR.message_types_by_name['InferenceExecutionSource']
@@ -26,14 +26,15 @@
 _BATCHFEATURESETSOURCE = DESCRIPTOR.message_types_by_name['BatchFeatureSetSource']
 _STREAMINGAGGREGATIONFEATURESETSOURCE = DESCRIPTOR.message_types_by_name['StreamingAggregationFeatureSetSource']
 _ONLINETYPE = DESCRIPTOR.message_types_by_name['OnlineType']
 _OFFLINETYPE = DESCRIPTOR.message_types_by_name['OfflineType']
 _ROWLEVELTYPE = DESCRIPTOR.message_types_by_name['RowLevelType']
 _COMPACTIONTYPE = DESCRIPTOR.message_types_by_name['CompactionType']
 _BACKFILLTYPE = DESCRIPTOR.message_types_by_name['BackfillType']
+_REALTIMEFEATUREEXTRACTORSOURCE = DESCRIPTOR.message_types_by_name['RealTimeFeatureExtractorSource']
 LogSource = _reflection.GeneratedProtocolMessageType('LogSource', (_message.Message,), {
   'DESCRIPTOR' : _LOGSOURCE,
   '__module__' : 'qwak.logging.log_source_pb2'
   # @@protoc_insertion_point(class_scope:qwak.logging.service.LogSource)
   })
 _sym_db.RegisterMessage(LogSource)
 
@@ -110,36 +111,45 @@
 BackfillType = _reflection.GeneratedProtocolMessageType('BackfillType', (_message.Message,), {
   'DESCRIPTOR' : _BACKFILLTYPE,
   '__module__' : 'qwak.logging.log_source_pb2'
   # @@protoc_insertion_point(class_scope:qwak.logging.service.BackfillType)
   })
 _sym_db.RegisterMessage(BackfillType)
 
+RealTimeFeatureExtractorSource = _reflection.GeneratedProtocolMessageType('RealTimeFeatureExtractorSource', (_message.Message,), {
+  'DESCRIPTOR' : _REALTIMEFEATUREEXTRACTORSOURCE,
+  '__module__' : 'qwak.logging.log_source_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.logging.service.RealTimeFeatureExtractorSource)
+  })
+_sym_db.RegisterMessage(RealTimeFeatureExtractorSource)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.qwak.ai.logging.reader.apiP\001'
   _LOGSOURCE._serialized_start=56
-  _LOGSOURCE._serialized_end=549
-  _REMOTEBUILDSOURCE._serialized_start=551
-  _REMOTEBUILDSOURCE._serialized_end=607
-  _MODELRUNTIMESOURCE._serialized_start=609
-  _MODELRUNTIMESOURCE._serialized_end=687
-  _INFERENCEEXECUTIONSOURCE._serialized_start=689
-  _INFERENCEEXECUTIONSOURCE._serialized_end=785
-  _STREAMINGFEATURESETSOURCE._serialized_start=788
-  _STREAMINGFEATURESETSOURCE._serialized_end=979
-  _BATCHFEATURESETSOURCE._serialized_start=981
-  _BATCHFEATURESETSOURCE._serialized_end=1068
-  _STREAMINGAGGREGATIONFEATURESETSOURCE._serialized_start=1071
-  _STREAMINGAGGREGATIONFEATURESETSOURCE._serialized_end=1290
-  _ONLINETYPE._serialized_start=1292
-  _ONLINETYPE._serialized_end=1354
-  _OFFLINETYPE._serialized_start=1356
-  _OFFLINETYPE._serialized_end=1435
-  _ROWLEVELTYPE._serialized_start=1437
-  _ROWLEVELTYPE._serialized_end=1501
-  _COMPACTIONTYPE._serialized_start=1503
-  _COMPACTIONTYPE._serialized_end=1585
-  _BACKFILLTYPE._serialized_start=1587
-  _BACKFILLTYPE._serialized_end=1651
+  _LOGSOURCE._serialized_end=642
+  _REMOTEBUILDSOURCE._serialized_start=644
+  _REMOTEBUILDSOURCE._serialized_end=700
+  _MODELRUNTIMESOURCE._serialized_start=702
+  _MODELRUNTIMESOURCE._serialized_end=780
+  _INFERENCEEXECUTIONSOURCE._serialized_start=782
+  _INFERENCEEXECUTIONSOURCE._serialized_end=878
+  _STREAMINGFEATURESETSOURCE._serialized_start=881
+  _STREAMINGFEATURESETSOURCE._serialized_end=1072
+  _BATCHFEATURESETSOURCE._serialized_start=1074
+  _BATCHFEATURESETSOURCE._serialized_end=1161
+  _STREAMINGAGGREGATIONFEATURESETSOURCE._serialized_start=1164
+  _STREAMINGAGGREGATIONFEATURESETSOURCE._serialized_end=1383
+  _ONLINETYPE._serialized_start=1385
+  _ONLINETYPE._serialized_end=1447
+  _OFFLINETYPE._serialized_start=1449
+  _OFFLINETYPE._serialized_end=1528
+  _ROWLEVELTYPE._serialized_start=1530
+  _ROWLEVELTYPE._serialized_end=1594
+  _COMPACTIONTYPE._serialized_start=1596
+  _COMPACTIONTYPE._serialized_end=1678
+  _BACKFILLTYPE._serialized_start=1680
+  _BACKFILLTYPE._serialized_end=1744
+  _REALTIMEFEATUREEXTRACTORSOURCE._serialized_start=1746
+  _REALTIMEFEATUREEXTRACTORSOURCE._serialized_end=1818
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -23,39 +23,43 @@
 
     MODEL_RUNTIME_FIELD_NUMBER: builtins.int
     REMOTE_BUILD_FIELD_NUMBER: builtins.int
     INFERENCE_EXECUTION_FIELD_NUMBER: builtins.int
     STREAMING_FEATURE_SET_FIELD_NUMBER: builtins.int
     STREAMING_AGGREGATION_FEATURE_SET_FIELD_NUMBER: builtins.int
     BATCH_FEATURE_SET_FIELD_NUMBER: builtins.int
+    REAL_TIME_FEATURE_EXTRACTOR_FIELD_NUMBER: builtins.int
     @property
     def model_runtime(self) -> global___ModelRuntimeSource: ...
     @property
     def remote_build(self) -> global___RemoteBuildSource: ...
     @property
     def inference_execution(self) -> global___InferenceExecutionSource: ...
     @property
     def streaming_feature_set(self) -> global___StreamingFeatureSetSource: ...
     @property
     def streaming_aggregation_feature_set(self) -> global___StreamingAggregationFeatureSetSource: ...
     @property
     def batch_feature_set(self) -> global___BatchFeatureSetSource: ...
+    @property
+    def real_time_feature_extractor(self) -> global___RealTimeFeatureExtractorSource: ...
     def __init__(
         self,
         *,
         model_runtime: global___ModelRuntimeSource | None = ...,
         remote_build: global___RemoteBuildSource | None = ...,
         inference_execution: global___InferenceExecutionSource | None = ...,
         streaming_feature_set: global___StreamingFeatureSetSource | None = ...,
         streaming_aggregation_feature_set: global___StreamingAggregationFeatureSetSource | None = ...,
         batch_feature_set: global___BatchFeatureSetSource | None = ...,
+        real_time_feature_extractor: global___RealTimeFeatureExtractorSource | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["batch_feature_set", b"batch_feature_set", "inference_execution", b"inference_execution", "model_runtime", b"model_runtime", "remote_build", b"remote_build", "source", b"source", "streaming_aggregation_feature_set", b"streaming_aggregation_feature_set", "streaming_feature_set", b"streaming_feature_set"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["batch_feature_set", b"batch_feature_set", "inference_execution", b"inference_execution", "model_runtime", b"model_runtime", "remote_build", b"remote_build", "source", b"source", "streaming_aggregation_feature_set", b"streaming_aggregation_feature_set", "streaming_feature_set", b"streaming_feature_set"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["source", b"source"]) -> typing_extensions.Literal["model_runtime", "remote_build", "inference_execution", "streaming_feature_set", "streaming_aggregation_feature_set", "batch_feature_set"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["batch_feature_set", b"batch_feature_set", "inference_execution", b"inference_execution", "model_runtime", b"model_runtime", "real_time_feature_extractor", b"real_time_feature_extractor", "remote_build", b"remote_build", "source", b"source", "streaming_aggregation_feature_set", b"streaming_aggregation_feature_set", "streaming_feature_set", b"streaming_feature_set"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["batch_feature_set", b"batch_feature_set", "inference_execution", b"inference_execution", "model_runtime", b"model_runtime", "real_time_feature_extractor", b"real_time_feature_extractor", "remote_build", b"remote_build", "source", b"source", "streaming_aggregation_feature_set", b"streaming_aggregation_feature_set", "streaming_feature_set", b"streaming_feature_set"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["source", b"source"]) -> typing_extensions.Literal["model_runtime", "remote_build", "inference_execution", "streaming_feature_set", "streaming_aggregation_feature_set", "batch_feature_set", "real_time_feature_extractor"] | None: ...
 
 global___LogSource = LogSource
 
 class RemoteBuildSource(google.protobuf.message.Message):
     """Represent a "remote build source" """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -296,7 +300,22 @@
         *,
         feature_set_id: builtins.str = ...,
         feature_set_name: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["feature_set_id", b"feature_set_id", "feature_set_name", b"feature_set_name"]) -> None: ...
 
 global___BackfillType = BackfillType
+
+class RealTimeFeatureExtractorSource(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    REAL_TIME_FEATURE_EXTRACTOR_ID_FIELD_NUMBER: builtins.int
+    real_time_feature_extractor_id: builtins.str
+    """Filter by the real-time feature extractor id"""
+    def __init__(
+        self,
+        *,
+        real_time_feature_extractor_id: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["real_time_feature_extractor_id", b"real_time_feature_extractor_id"]) -> None: ...
+
+global___RealTimeFeatureExtractorSource = RealTimeFeatureExtractorSource
```

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.70/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.70/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.70/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/pyproject.toml` & `qwak_core-0.0.70/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.69"
+version = "0.0.70"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.69/qwak/automations/__init__.py` & `qwak_core-0.0.70/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/automations/automation_executions.py` & `qwak_core-0.0.70/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/automations/automations.py` & `qwak_core-0.0.70/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.70/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.70/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/automations/common.py` & `qwak_core-0.0.70/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.70/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.70/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.70/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.70/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.70/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/alert_management/client.py` & `qwak_core-0.0.70/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/analytics/client.py` & `qwak_core-0.0.70/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/audience/client.py` & `qwak_core-0.0.70/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/automation_management/client.py` & `qwak_core-0.0.70/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.70/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.70/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.70/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.70/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/build_management/client.py` & `qwak_core-0.0.70/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.70/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.70/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/deployment/client.py` & `qwak_core-0.0.70/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.70/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.70/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.70/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.70/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/instance_template/client.py` & `qwak_core-0.0.70/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.70/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/logging_client/client.py` & `qwak_core-0.0.70/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/model_management/client.py` & `qwak_core-0.0.70/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/project/client.py` & `qwak_core-0.0.70/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/secret_service/client.py` & `qwak_core-0.0.70/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.70/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.70/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.70/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.70/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.70/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.70/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.70/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.70/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.70/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.70/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.70/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.70/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.70/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.70/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.70/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/offline/client.py` & `qwak_core-0.0.70/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/feature_store/online/client.py` & `qwak_core-0.0.70/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/inner/const.py` & `qwak_core-0.0.70/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.70/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.70/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.70/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.70/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/inner/singleton_meta.py` & `qwak_core-0.0.70/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/inner/tool/auth.py` & `qwak_core-0.0.70/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.70/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.70/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.70/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.70/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/adapters/__init__.py` & `qwak_core-0.0.70/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.70/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.70/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.70/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.70/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.70/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/base.py` & `qwak_core-0.0.70/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/decorators/api.py` & `qwak_core-0.0.70/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.70/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/experiment_tracking.py` & `qwak_core-0.0.70/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/schema.py` & `qwak_core-0.0.70/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/schema_entities.py` & `qwak_core-0.0.70/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.70/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.70/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.70/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.70/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.70/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.70/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.70/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.70/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.70/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.70/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.70/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.70/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.70/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.70/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.70/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.70/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.70/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.70/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.70/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/qwak_client/client.py` & `qwak_core-0.0.70/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.70/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/qwak_client/models/model.py` & `qwak_core-0.0.70/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.70/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.70/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/tools/logger/logger.py` & `qwak_core-0.0.70/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak/tools/logger/logging.yml` & `qwak_core-0.0.70/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.70/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/qwak_services_mock/services_mock.py` & `qwak_core-0.0.70/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.69/setup.py` & `qwak_core-0.0.70/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.69',
+    'version': '0.0.70',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.69/PKG-INFO` & `qwak_core-0.0.70/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.69
+Version: 0.0.70
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

