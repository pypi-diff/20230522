# Comparing `tmp/aws-parallelcluster-3.6.0.tar.gz` & `tmp/aws-parallelcluster-3.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-parallelcluster-3.6.0.tar", last modified: Mon May 22 15:44:11 2023, max compression
+gzip compressed data, was "aws-parallelcluster-3.6.0b1.tar", last modified: Thu Apr 27 20:58:59 2023, max compression
```

## Comparing `aws-parallelcluster-3.6.0.tar` & `aws-parallelcluster-3.6.0b1.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.129563 aws-parallelcluster-3.6.0/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      114 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/MANIFEST.in
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1850 2023-05-22 15:44:11.129563 aws-parallelcluster-3.6.0/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      787 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/README
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       38 2023-05-22 15:44:11.129563 aws-parallelcluster-3.6.0/setup.cfg
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3443 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/setup.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.093563 aws-parallelcluster-3.6.0/src/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.093563 aws-parallelcluster-3.6.0/src/aws_parallelcluster.egg-info/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1850 2023-05-22 15:44:11.000000 aws-parallelcluster-3.6.0/src/aws_parallelcluster.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10677 2023-05-22 15:44:11.000000 aws-parallelcluster-3.6.0/src/aws_parallelcluster.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-05-22 15:44:11.000000 aws-parallelcluster-3.6.0/src/aws_parallelcluster.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      147 2023-05-22 15:44:11.000000 aws-parallelcluster-3.6.0/src/aws_parallelcluster.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-05-22 15:44:11.000000 aws-parallelcluster-3.6.0/src/aws_parallelcluster.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      641 2023-05-22 15:44:11.000000 aws-parallelcluster-3.6.0/src/aws_parallelcluster.egg-info/requires.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       36 2023-05-22 15:44:11.000000 aws-parallelcluster-3.6.0/src/aws_parallelcluster.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.093563 aws-parallelcluster-3.6.0/src/pcluster/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      559 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.097563 aws-parallelcluster-3.6.0/src/pcluster/api/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.097563 aws-parallelcluster-3.6.0/src/pcluster/api/awslambda/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/awslambda/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2659 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/awslambda/entrypoint.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11252 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/awslambda/serverless_wsgi.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.097563 aws-parallelcluster-3.6.0/src/pcluster/api/controllers/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      548 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/controllers/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4019 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/controllers/cluster_compute_fleet_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4192 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/controllers/cluster_instances_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7167 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/controllers/cluster_logs_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    19236 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/controllers/cluster_operations_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7697 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/controllers/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6289 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/controllers/image_logs_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    15354 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/controllers/image_operations_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4143 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/converters.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1536 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/encoder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5812 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/errors.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7657 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/flask_app.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.109563 aws-parallelcluster-3.6.0/src/pcluster/api/models/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6121 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4682 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/ami_info.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2128 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2428 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/base_model_.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3757 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/build_image_bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3652 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/build_image_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3639 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/build_image_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3369 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/change.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1717 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/cloud_formation_resource_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1775 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/cloud_formation_stack_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2103 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/cluster_configuration_structure.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9207 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/cluster_info_summary.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8637 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/cluster_instance.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2106 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/cluster_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1879 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/cluster_status_filtering_option.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1630 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/compute_fleet_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4053 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/config_validation_message.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2106 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/conflict_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3813 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3875 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/create_cluster_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3751 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/create_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2302 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/delete_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2220 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/delete_image_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3397 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/describe_cluster_instances_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    17460 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/describe_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3802 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/describe_compute_fleet_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    19464 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/describe_image_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4859 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/dryrun_operation_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6209 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/ec2_ami_info.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2185 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/ec2_ami_info_summary.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1488 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/ec2_ami_state.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6566 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/ec2_instance.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2451 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/failure.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3660 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/get_cluster_log_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2791 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/get_cluster_stack_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3618 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/get_image_log_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2759 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/get_image_stack_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1576 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/image_build_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1678 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/image_builder_image_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2053 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/image_configuration_structure.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8609 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/image_info_summary.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1615 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/image_status_filtering_option.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1484 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/instance_state.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2183 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/internal_service_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2161 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/limit_exceeded_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3024 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/list_cluster_log_streams_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3200 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/list_clusters_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2992 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/list_image_log_streams_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3108 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/list_images_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2315 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/list_official_images_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2373 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/log_event.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8592 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/log_stream.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2418 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/metadata.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1348 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/node_type.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2106 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/not_found_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1532 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/requested_compute_fleet_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2656 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/scheduler.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12343 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/stack_event.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2286 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/tag.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2172 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/unauthorized_client_error_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6155 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2594 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/update_cluster_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4944 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/update_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2377 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/update_compute_fleet_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3274 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/update_compute_fleet_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4087 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/update_error.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1394 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/models/validation_level.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.109563 aws-parallelcluster-3.6.0/src/pcluster/api/openapi/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/openapi/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)   114697 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/openapi/openapi.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1388 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/typing_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8594 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/api/util.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.113563 aws-parallelcluster-3.6.0/src/pcluster/aws/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5634 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/aws_api.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    15716 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/aws_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5430 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/batch.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7832 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/cfn.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8480 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2234 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/dynamo.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    21619 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/ec2.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3313 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/efs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3795 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/fsx.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1351 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/iam.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      949 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/imagebuilder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      907 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/kms.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5687 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/logs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1801 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/resource_groups.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2097 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/route53.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7491 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/s3.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2656 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/s3_resource.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1067 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/secretsmanager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1003 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/ssm.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      959 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/aws/sts.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.113563 aws-parallelcluster-3.6.0/src/pcluster/cli/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.113563 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4361 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/cluster_logs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      975 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/commands.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5361 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/common.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.117563 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/configure/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/configure/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1486 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/configure/command.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    20483 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/configure/easyconfig.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10146 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/configure/networking.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5959 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/configure/subnet_computation.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8348 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/configure/utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6742 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/dcv_connect.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      896 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/dcv_util.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3571 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/image_logs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3968 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/ssh.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1434 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/commands/version.py
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)    11369 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/entrypoint.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1116 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/exceptions.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3002 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/logger.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4586 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/middleware.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7601 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/cli/model.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.117563 aws-parallelcluster-3.6.0/src/pcluster/config/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/config/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)   134123 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/config/cluster_config.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    16981 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/config/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12981 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/config/config_patch.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11611 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/config/imagebuilder_config.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    21758 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/config/update_policy.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11434 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/constants.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2624 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/imagebuilder_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2364 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/launch_template_utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.117563 aws-parallelcluster-3.6.0/src/pcluster/lib/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      963 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/lib/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3558 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/lib/lib.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.117563 aws-parallelcluster-3.6.0/src/pcluster/models/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/models/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    58732 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/models/cluster.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12099 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/models/cluster_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    13929 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/models/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12602 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/models/compute_fleet_status_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    35260 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/models/imagebuilder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5037 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/models/imagebuilder_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    16902 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/models/s3_bucket.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.117563 aws-parallelcluster-3.6.0/src/pcluster/networking/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      559 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/networking/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3769 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/networking/vpc_factory.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.093563 aws-parallelcluster-3.6.0/src/pcluster/resources/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.089563 aws-parallelcluster-3.6.0/src/pcluster/resources/batch/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.117563 aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.117563 aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/alinux2/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1816 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/alinux2/Dockerfile
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     1139 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/build-docker-images.sh
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      535 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/buildspec.yml
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.121563 aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/scripts/
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     1599 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/scripts/entrypoint.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     5466 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     1954 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     2882 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/scripts/mount_efs.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     2457 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)      856 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/upload-docker-images.sh
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.121563 aws-parallelcluster-3.6.0/src/pcluster/resources/compute_node/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10447 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/compute_node/user_data.sh
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.089563 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.121563 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7610 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.121563 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10142 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       96 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/NOTICE
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       81 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2701 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    13195 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1842 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3545 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3369 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2763 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.121563 aws-parallelcluster-3.6.0/src/pcluster/resources/head_node/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6660 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/head_node/user_data.sh
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.121563 aws-parallelcluster-3.6.0/src/pcluster/resources/imagebuilder/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1919 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/imagebuilder/custom_script.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10585 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/imagebuilder/parallelcluster.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8732 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12214 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    15874 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7391 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/resources/imagebuilder/update_and_reboot.yaml
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.125563 aws-parallelcluster-3.6.0/src/pcluster/schemas/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/schemas/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    86365 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/schemas/cluster_schema.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10601 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/schemas/common_schema.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7968 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/schemas/imagebuilder_schema.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.125563 aws-parallelcluster-3.6.0/src/pcluster/templates/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/templates/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    38565 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/templates/awsbatch_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5999 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/templates/cdk_artifacts_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3232 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/templates/cdk_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    40959 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/templates/cdk_builder_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    62313 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/templates/cluster_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5807 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/templates/compute_fleet_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    36443 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/templates/cw_dashboard_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    44224 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/templates/imagebuilder_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      682 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/templates/import_cdk.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    17210 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/templates/queues_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    13562 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/templates/slurm_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    19351 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.129563 aws-parallelcluster-3.6.0/src/pcluster/validators/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8763 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/awsbatch_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    64756 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/cluster_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5233 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3528 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/database_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7602 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/directory_service_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12873 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/ebs_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    25736 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/ec2_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1212 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/efs_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1202 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/feature_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9186 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/fsx_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4000 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/iam_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2361 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/imagebuilder_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12556 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/instances_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1414 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/kms_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1858 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/monitoring_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9209 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/networking_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6760 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/s3_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7690 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/scheduler_plugin_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5195 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/slurm_settings_validator.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4081 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/tags_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      825 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster/validators/utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:44:11.129563 aws-parallelcluster-3.6.0/src/pcluster3_config_converter/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster3_config_converter/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    52964 2023-05-22 12:18:56.000000 aws-parallelcluster-3.6.0/src/pcluster3_config_converter/pcluster3_config_converter.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.624519 aws-parallelcluster-3.6.0b1/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      114 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/MANIFEST.in
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1852 2023-04-27 20:58:59.624519 aws-parallelcluster-3.6.0b1/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      787 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/README
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       38 2023-04-27 20:58:59.624519 aws-parallelcluster-3.6.0b1/setup.cfg
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3447 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/setup.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.584519 aws-parallelcluster-3.6.0b1/src/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.584519 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1852 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10682 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      147 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      803 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       36 2023-04-27 20:58:59.000000 aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.584519 aws-parallelcluster-3.6.0b1/src/pcluster/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      559 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.588519 aws-parallelcluster-3.6.0b1/src/pcluster/api/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.588519 aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2659 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/entrypoint.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11252 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/serverless_wsgi.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.588519 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      548 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4019 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_compute_fleet_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4192 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_instances_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7167 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_logs_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    19236 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_operations_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7697 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6289 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/image_logs_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    15354 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/image_operations_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4143 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/converters.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1536 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/encoder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5812 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/errors.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7657 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/flask_app.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.600519 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6121 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4682 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ami_info.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2128 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2428 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/base_model_.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3757 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/build_image_bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3652 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/build_image_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3639 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/build_image_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3369 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/change.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1717 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cloud_formation_resource_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1775 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cloud_formation_stack_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2103 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_configuration_structure.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9207 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_info_summary.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8637 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_instance.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2106 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1879 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_status_filtering_option.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1630 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/compute_fleet_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4053 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/config_validation_message.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2106 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/conflict_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3813 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3875 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/create_cluster_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3751 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/create_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2302 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/delete_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2220 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/delete_image_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3397 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_cluster_instances_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    17460 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3802 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_compute_fleet_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    19464 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_image_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4859 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/dryrun_operation_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6209 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_ami_info.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2185 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_ami_info_summary.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1488 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_ami_state.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6566 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_instance.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2451 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/failure.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3660 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_cluster_log_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2791 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_cluster_stack_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3618 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_image_log_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2759 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_image_stack_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1576 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_build_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1678 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_builder_image_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2053 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_configuration_structure.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8609 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_info_summary.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1615 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_status_filtering_option.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1484 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/instance_state.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2183 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/internal_service_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2161 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/limit_exceeded_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3024 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_cluster_log_streams_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3200 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_clusters_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2992 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_image_log_streams_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3108 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_images_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2315 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_official_images_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2373 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/log_event.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8592 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/log_stream.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2418 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/metadata.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1348 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/node_type.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2106 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/not_found_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1532 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/requested_compute_fleet_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2656 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/scheduler.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12343 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/stack_event.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2286 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/tag.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2172 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/unauthorized_client_error_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6155 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2594 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_cluster_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4944 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2377 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_compute_fleet_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3274 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_compute_fleet_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4087 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_error.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1394 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/models/validation_level.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.600519 aws-parallelcluster-3.6.0b1/src/pcluster/api/openapi/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/openapi/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)   114697 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/openapi/openapi.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1388 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/typing_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8594 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/api/util.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.604519 aws-parallelcluster-3.6.0b1/src/pcluster/aws/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5634 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/aws_api.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    15716 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/aws_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5430 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/batch.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7832 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/cfn.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8480 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2234 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/dynamo.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    21619 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/ec2.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3313 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/efs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3795 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/fsx.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1351 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/iam.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      949 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/imagebuilder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      907 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/kms.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5687 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/logs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1801 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/resource_groups.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2097 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/route53.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7491 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/s3.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2656 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/s3_resource.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1067 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/secretsmanager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1003 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/ssm.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      959 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/aws/sts.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.604519 aws-parallelcluster-3.6.0b1/src/pcluster/cli/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.608519 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4361 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/cluster_logs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      975 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/commands.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5361 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/common.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.608519 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1486 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/command.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    20572 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/easyconfig.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10146 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/networking.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5959 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/subnet_computation.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8348 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6742 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/dcv_connect.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      896 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/dcv_util.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3571 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/image_logs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3968 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/ssh.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1434 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/version.py
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)    10935 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/entrypoint.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1116 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/exceptions.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3002 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/logger.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4586 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/middleware.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7601 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/cli/model.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.608519 aws-parallelcluster-3.6.0b1/src/pcluster/config/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/config/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)   133673 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/config/cluster_config.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    16981 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/config/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12981 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/config/config_patch.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11611 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/config/imagebuilder_config.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    21758 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/config/update_policy.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11490 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/constants.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2624 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/imagebuilder_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2364 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/launch_template_utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.608519 aws-parallelcluster-3.6.0b1/src/pcluster/lib/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      963 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/lib/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3558 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/lib/lib.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.608519 aws-parallelcluster-3.6.0b1/src/pcluster/models/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    58732 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/cluster.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12099 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/cluster_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    13929 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12602 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/compute_fleet_status_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    35260 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/imagebuilder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5037 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/imagebuilder_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    16902 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/models/s3_bucket.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/networking/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      559 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/networking/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3769 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/networking/vpc_factory.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.584519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.584519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/alinux2/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1816 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/alinux2/Dockerfile
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     1139 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/build-docker-images.sh
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      535 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/buildspec.yml
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     1599 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/entrypoint.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     5466 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     1954 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     2882 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/mount_efs.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)     2457 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (1000)      856 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/upload-docker-images.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/compute_node/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10447 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/compute_node/user_data.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.584519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7610 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10142 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       96 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/NOTICE
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       81 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2701 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    13195 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1842 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3545 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3369 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2763 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.612519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/head_node/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6660 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/head_node/user_data.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.616519 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1919 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/custom_script.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10585 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8732 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12214 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    16131 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6319 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/update_and_reboot.yaml
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.616519 aws-parallelcluster-3.6.0b1/src/pcluster/schemas/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/schemas/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    86365 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/schemas/cluster_schema.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10452 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/schemas/common_schema.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7968 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/schemas/imagebuilder_schema.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.616519 aws-parallelcluster-3.6.0b1/src/pcluster/templates/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    38565 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/awsbatch_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5999 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/cdk_artifacts_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3115 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/cdk_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    40959 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/cdk_builder_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    62422 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/cluster_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    10026 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/compute_fleet_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    35904 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/cw_dashboard_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    44224 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/imagebuilder_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      682 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/import_cdk.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    17214 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/queue_group_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    13562 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/templates/slurm_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    18843 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.620519 aws-parallelcluster-3.6.0b1/src/pcluster/validators/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     8763 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/awsbatch_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    64756 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/cluster_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5233 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3528 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/database_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7577 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/directory_service_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12873 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/ebs_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    25736 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/ec2_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1212 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/efs_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1739 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/feature_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9186 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/fsx_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4000 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/iam_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2361 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/imagebuilder_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    12556 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/instances_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1414 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/kms_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1858 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/monitoring_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9209 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/networking_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6760 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/s3_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     7690 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/scheduler_plugin_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5195 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/slurm_settings_validator.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4081 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/tags_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      825 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster/validators/utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:58:59.620519 aws-parallelcluster-3.6.0b1/src/pcluster3_config_converter/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster3_config_converter/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    52964 2023-04-27 19:15:10.000000 aws-parallelcluster-3.6.0b1/src/pcluster3_config_converter/pcluster3_config_converter.py
```

### Comparing `aws-parallelcluster-3.6.0/PKG-INFO` & `aws-parallelcluster-3.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster
-Version: 3.6.0
+Version: 3.6.0b1
 Summary: AWS ParallelCluster is an AWS supported Open Source cluster management tool to deploy and manage HPC clusters in the AWS cloud.
 Home-page: https://github.com/aws/aws-parallelcluster
 Author: Amazon Web Services
 License: Apache License 2.0
 Project-URL: Changelog, https://github.com/aws/aws-parallelcluster/blob/develop/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/aws/aws-parallelcluster/issues
 Project-URL: Documentation, https://docs.aws.amazon.com/parallelcluster/
```

### Comparing `aws-parallelcluster-3.6.0/README` & `aws-parallelcluster-3.6.0b1/README`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/setup.py` & `aws-parallelcluster-3.6.0b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 def readme():
     """Read the README file and use it as long description."""
     with open(os.path.join(os.path.dirname(__file__), "README"), encoding="utf-8") as f:
         return f.read()
 
 
-VERSION = "3.6.0"
-CDK_VERSION = "1.164"
+VERSION = "3.6.0b1"
+CDK_VERSION = "1.137,!=1.153.0"
 REQUIRES = [
     "setuptools",
     "boto3>=1.16.14",
     "tabulate>=0.8.8,<=0.8.10",
     "PyYAML~=5.3",
     "jinja2~=3.0",
     "marshmallow~=3.10",
@@ -44,15 +44,15 @@
     "aws-cdk.aws-logs~=" + CDK_VERSION,
     "aws-cdk.aws-route53~=" + CDK_VERSION,
     "aws-cdk.aws-ssm~=" + CDK_VERSION,
     "aws-cdk.aws-sqs~=" + CDK_VERSION,
     "aws-cdk.aws-cloudformation~=" + CDK_VERSION,
     "werkzeug~=2.0",
     "connexion~=2.13.0",
-    "flask>=2.2.5,==2.2.*",
+    "flask~=2.2.0",
     "jmespath~=0.10",
 ]
 
 LAMBDA_REQUIRES = [
     "aws-lambda-powertools~=1.14",
 ]
```

### Comparing `aws-parallelcluster-3.6.0/src/aws_parallelcluster.egg-info/PKG-INFO` & `aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster
-Version: 3.6.0
+Version: 3.6.0b1
 Summary: AWS ParallelCluster is an AWS supported Open Source cluster management tool to deploy and manage HPC clusters in the AWS cloud.
 Home-page: https://github.com/aws/aws-parallelcluster
 Author: Amazon Web Services
 License: Apache License 2.0
 Project-URL: Changelog, https://github.com/aws/aws-parallelcluster/blob/develop/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/aws/aws-parallelcluster/issues
 Project-URL: Documentation, https://docs.aws.amazon.com/parallelcluster/
```

### Comparing `aws-parallelcluster-3.6.0/src/aws_parallelcluster.egg-info/SOURCES.txt` & `aws-parallelcluster-3.6.0b1/src/aws_parallelcluster.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 src/pcluster/templates/cdk_builder.py
 src/pcluster/templates/cdk_builder_utils.py
 src/pcluster/templates/cluster_stack.py
 src/pcluster/templates/compute_fleet_stack.py
 src/pcluster/templates/cw_dashboard_builder.py
 src/pcluster/templates/imagebuilder_stack.py
 src/pcluster/templates/import_cdk.py
-src/pcluster/templates/queues_stack.py
+src/pcluster/templates/queue_group_stack.py
 src/pcluster/templates/slurm_builder.py
 src/pcluster/validators/__init__.py
 src/pcluster/validators/awsbatch_validators.py
 src/pcluster/validators/cluster_validators.py
 src/pcluster/validators/common.py
 src/pcluster/validators/database_validators.py
 src/pcluster/validators/directory_service_validators.py
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/awslambda/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/awslambda/entrypoint.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/entrypoint.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/awslambda/serverless_wsgi.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/awslambda/serverless_wsgi.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/controllers/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/controllers/cluster_compute_fleet_controller.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_compute_fleet_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/controllers/cluster_instances_controller.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_instances_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/controllers/cluster_logs_controller.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_logs_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/controllers/cluster_operations_controller.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/cluster_operations_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/controllers/common.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/controllers/image_logs_controller.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/image_logs_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/controllers/image_operations_controller.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/controllers/image_operations_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/converters.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/converters.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/encoder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/encoder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/errors.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/errors.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/flask_app.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/flask_app.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/ami_info.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ami_info.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/bad_request_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/base_model_.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/build_image_bad_request_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/build_image_bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/build_image_request_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/build_image_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/build_image_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/build_image_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/change.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/change.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/cloud_formation_resource_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cloud_formation_resource_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/cloud_formation_stack_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cloud_formation_stack_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/cluster_configuration_structure.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_configuration_structure.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/cluster_info_summary.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_info_summary.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/cluster_instance.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_instance.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/cluster_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/cluster_status_filtering_option.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/cluster_status_filtering_option.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/compute_fleet_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/compute_fleet_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/config_validation_message.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/config_validation_message.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/conflict_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/conflict_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/create_cluster_request_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/create_cluster_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/create_cluster_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/create_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/delete_cluster_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/delete_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/delete_image_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/delete_image_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/describe_cluster_instances_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_cluster_instances_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/describe_cluster_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/describe_compute_fleet_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_compute_fleet_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/describe_image_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/describe_image_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/dryrun_operation_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/dryrun_operation_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/ec2_ami_info.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_ami_info.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/ec2_ami_info_summary.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_ami_info_summary.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/ec2_ami_state.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_ami_state.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/ec2_instance.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/ec2_instance.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/failure.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/failure.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/get_cluster_log_events_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_cluster_log_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/get_cluster_stack_events_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_cluster_stack_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/get_image_log_events_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_image_log_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/get_image_stack_events_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/get_image_stack_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/image_build_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_build_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/image_builder_image_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_builder_image_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/image_configuration_structure.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_configuration_structure.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/image_info_summary.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_info_summary.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/image_status_filtering_option.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/image_status_filtering_option.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/instance_state.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/instance_state.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/internal_service_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/internal_service_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/limit_exceeded_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/limit_exceeded_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/list_cluster_log_streams_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_cluster_log_streams_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/list_clusters_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_clusters_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/list_image_log_streams_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_image_log_streams_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/list_images_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_images_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/list_official_images_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/list_official_images_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/log_event.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/log_event.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/log_stream.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/log_stream.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/metadata.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/metadata.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/node_type.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/node_type.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/not_found_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/not_found_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/requested_compute_fleet_status.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/requested_compute_fleet_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/scheduler.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/scheduler.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/stack_event.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/stack_event.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/tag.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/tag.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/unauthorized_client_error_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/unauthorized_client_error_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/update_cluster_request_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_cluster_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/update_cluster_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/update_compute_fleet_request_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_compute_fleet_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/update_compute_fleet_response_content.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_compute_fleet_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/update_error.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/update_error.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/models/validation_level.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/models/validation_level.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/openapi/openapi.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/openapi/openapi.yaml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/typing_utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/typing_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/api/util.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/api/util.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/aws_api.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/aws_api.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/aws_resources.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/aws_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/batch.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/batch.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/cfn.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/cfn.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/common.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/dynamo.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/dynamo.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/ec2.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/ec2.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/efs.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/efs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/fsx.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/fsx.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/iam.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/iam.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/imagebuilder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/imagebuilder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/kms.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/kms.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/logs.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/logs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/resource_groups.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/resource_groups.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/route53.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/route53.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/s3.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/s3.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/s3_resource.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/s3_resource.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/secretsmanager.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/ssm.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/aws/sts.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/aws/sts.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/cluster_logs.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/cluster_logs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/commands.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/commands.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/common.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/configure/command.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/command.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/configure/easyconfig.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/easyconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     placement_group_exists,
     prompt,
     prompt_iterable,
 )
 from pcluster.constants import (
     DEFAULT_MAX_COUNT,
     DEFAULT_MIN_COUNT,
+    MAX_COMPUTE_RESOURCES_PER_QUEUE,
     MAX_NUMBER_OF_COMPUTE_RESOURCES_PER_CLUSTER,
     MAX_NUMBER_OF_QUEUES,
     SUPPORTED_SCHEDULERS,
 )
 from pcluster.utils import error, get_supported_os_for_scheduler
 from pcluster.validators.cluster_validators import NameValidator
 
@@ -191,20 +192,21 @@
                 f"Error: The name {queue_name} cannot be used for multiple queues. Please insert a different queue "
                 "name."
             )
 
         if scheduler == "awsbatch":
             number_of_compute_resources = 1
         else:
-            crs_per_queue_limit = MAX_NUMBER_OF_COMPUTE_RESOURCES_PER_CLUSTER // number_of_queues
-
+            queue_limit = min(
+                (MAX_NUMBER_OF_COMPUTE_RESOURCES_PER_CLUSTER / number_of_queues), MAX_COMPUTE_RESOURCES_PER_QUEUE
+            )
             number_of_compute_resources = int(
                 prompt(
                     f"Number of compute resources for {queue_name}",
-                    validator=lambda x, q=crs_per_queue_limit: str(x).isdigit() and 1 <= int(x) <= q,
+                    validator=lambda x, q=queue_limit: str(x).isdigit() and 1 <= int(x) <= q,
                     default_value=1,
                 )
             )
         compute_resources = []
         efa_enabled_in_queue = False
         for compute_resource_index in range(number_of_compute_resources):
             efa_enabled_in_compute_resource = False
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/configure/networking.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/networking.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/configure/subnet_computation.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/subnet_computation.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/configure/utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/configure/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/dcv_connect.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/dcv_connect.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/dcv_util.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/dcv_util.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/image_logs.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/image_logs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/ssh.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/ssh.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/commands/version.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/entrypoint.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/entrypoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,34 +19,29 @@
 import re
 import sys
 from functools import partial
 
 import argparse
 from botocore.exceptions import NoCredentialsError  # TODO: remove
 
-# Suppress JSII warnings for Node version
-os.environ["JSII_SILENCE_WARNING_KNOWN_BROKEN_NODE_VERSION"] = "1"
-os.environ["JSII_SILENCE_WARNING_UNTESTED_NODE_VERSION"] = "1"
-os.environ["JSII_SILENCE_WARNING_DEPRECATED_NODE_VERSION"] = "1"
-
 # Controllers
-import pcluster.api.controllers.cluster_compute_fleet_controller  # noqa: E402
-import pcluster.api.controllers.cluster_instances_controller  # noqa: E402
-import pcluster.api.controllers.cluster_operations_controller  # noqa: E402
-import pcluster.api.controllers.image_operations_controller  # noqa: E402
-import pcluster.api.errors  # noqa: E402
-import pcluster.cli.commands.commands as cli_commands  # noqa: E402
-import pcluster.cli.logger as pcluster_logging  # noqa: E402
-import pcluster.cli.model  # noqa: E402
-from pcluster.api import encoder  # noqa: E402
-from pcluster.cli.commands.common import CliCommand, exit_msg, to_bool, to_int, to_number  # noqa: E402
-from pcluster.cli.exceptions import APIOperationException, ParameterException  # noqa: E402
-from pcluster.cli.logger import redirect_stdouterr_to_logger  # noqa: E402
-from pcluster.cli.middleware import add_additional_args, middleware_hooks  # noqa: E402
-from pcluster.utils import to_camel_case, to_snake_case  # noqa: E402
+import pcluster.api.controllers.cluster_compute_fleet_controller
+import pcluster.api.controllers.cluster_instances_controller
+import pcluster.api.controllers.cluster_operations_controller
+import pcluster.api.controllers.image_operations_controller
+import pcluster.api.errors
+import pcluster.cli.commands.commands as cli_commands
+import pcluster.cli.logger as pcluster_logging
+import pcluster.cli.model
+from pcluster.api import encoder
+from pcluster.cli.commands.common import CliCommand, exit_msg, to_bool, to_int, to_number
+from pcluster.cli.exceptions import APIOperationException, ParameterException
+from pcluster.cli.logger import redirect_stdouterr_to_logger
+from pcluster.cli.middleware import add_additional_args, middleware_hooks
+from pcluster.utils import to_camel_case, to_snake_case
 
 LOGGER = logging.getLogger(__name__)
 
 
 def re_validator(rexp_str, param, in_str):
     """Take a string and validate the input format."""
     rexp = re.compile(rexp_str)
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/exceptions.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/logger.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/logger.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/middleware.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/middleware.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/cli/model.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/cli/model.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/config/cluster_config.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/config/cluster_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -3090,25 +3090,14 @@
         for queue in self.scheduling.queues:
             for compute_resource in queue.compute_resources:
                 for instance_type in compute_resource.instance_types:
                     instance_type_info = compute_resource.instance_type_info_map[instance_type]
                     result[instance_type] = instance_type_info.instance_type_data
         return result
 
-    @property
-    def has_gpu_health_checks_enabled(self):
-        """Return True if an queue or compute resources has GPU health checking enabled."""
-        for queue in self.scheduling.queues:
-            if queue.health_checks.gpu.enabled:
-                return True
-            for compute_resource in queue.compute_resources:
-                if compute_resource.health_checks.gpu.enabled:
-                    return True
-        return False
-
     def _register_validators(self, context: ValidatorContext = None):
         super()._register_validators(context)
         self._register_validator(
             MixedSecurityGroupOverwriteValidator,
             head_node_security_groups=self.head_node.networking.security_groups,
             queues=self.scheduling.queues,
         )
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/config/common.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/config/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/config/config_patch.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/config/config_patch.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/config/imagebuilder_config.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/config/imagebuilder_config.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/config/update_policy.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/config/update_policy.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/constants.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,27 +92,28 @@
 }
 EBS_VOLUME_SIZE_DEFAULT = 35
 EBS_VOLUME_TYPE_DEFAULT = "gp3"
 EBS_VOLUME_TYPE_DEFAULT_US_ISO = "gp2"
 
 DEFAULT_MAX_COUNT = 10
 DEFAULT_MIN_COUNT = 0
-MAX_NUMBER_OF_QUEUES = 50
+MAX_NUMBER_OF_QUEUES = 100
 SCHEDULER_PLUGIN_MAX_NUMBER_OF_QUEUES = 10
 SCHEDULER_PLUGIN_MAX_NUMBER_OF_COMPUTE_RESOURCES = 5
-# Allow for flexibility in how compute resources are distributed in the cluster
-MAX_NUMBER_OF_COMPUTE_RESOURCES_PER_CLUSTER = MAX_COMPUTE_RESOURCES_PER_QUEUE = 50
+MAX_NUMBER_OF_COMPUTE_RESOURCES_PER_CLUSTER = 150  # Based on API timeout limitations
+MAX_COMPUTE_RESOURCES_PER_DEPLOYMENT_WAVE = 150  # Maximum compute resources that can be deployed at the same time
+MAX_COMPUTE_RESOURCES_PER_QUEUE = 40  # Ensures that each queue will share the same stack as its compute resources
 
 MAX_EBS_COUNT = 5
 MAX_NEW_STORAGE_COUNT = {"efs": 1, "fsx": 1, "raid": 1}
 MAX_EXISTING_STORAGE_COUNT = {"efs": 20, "fsx": 20, "raid": 0}
 
 COOKBOOK_PACKAGES_VERSIONS = {
-    "parallelcluster": "3.6.0",
-    "cookbook": "aws-parallelcluster-cookbook-3.6.0",
+    "parallelcluster": "3.6.0b1",
+    "cookbook": "aws-parallelcluster-cookbook-3.6.0b1",
     "chef": "17.2.29",
     "berkshelf": "7.2.0",
     "ami": "dev",
 }
 
 CW_DASHBOARD_ENABLED_DEFAULT = True
 CW_LOGS_ENABLED_DEFAULT = True
@@ -239,25 +240,23 @@
 
     BATCH = "AWS Batch scheduler"
     DCV = "NICE DCV"
     FSX_LUSTRE = "FSx Lustre"
     FSX_ONTAP = "FSx ONTAP"
     FSX_OPENZFS = "FSx OpenZfs"
     SLURM_DATABASE = "SLURM Database"
-    CLUSTER_HEALTH_METRICS = "Cluster Health Metrics"
 
 
 UNSUPPORTED_FEATURES_MAP = {
     Feature.BATCH: ["ap-northeast-3", "us-iso"],
     Feature.DCV: ["us-iso"],
     Feature.FSX_LUSTRE: ["us-iso"],
     Feature.FSX_ONTAP: ["us-iso"],
     Feature.FSX_OPENZFS: ["us-iso"],
     Feature.SLURM_DATABASE: ["us-iso"],
-    Feature.CLUSTER_HEALTH_METRICS: ["us-iso"],
 }
 
 
 # Operations support
 # By default, all operations are considered supported.
 # To mark an operation as unsupported for certain regions,
 # add the entry to the map below by region prefixes.
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/imagebuilder_utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/imagebuilder_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/launch_template_utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/launch_template_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/lib/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/lib/lib.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/lib/lib.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/models/cluster.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/cluster.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/models/cluster_resources.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/cluster_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/models/common.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/models/compute_fleet_status_manager.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/compute_fleet_status_manager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/models/imagebuilder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/imagebuilder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/models/imagebuilder_resources.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/imagebuilder_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/models/s3_bucket.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/models/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/networking/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/networking/vpc_factory.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/networking/vpc_factory.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/alinux2/Dockerfile` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/alinux2/Dockerfile`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/build-docker-images.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/build-docker-images.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/buildspec.yml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/buildspec.yml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/scripts/entrypoint.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/scripts/mount_efs.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/mount_efs.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/batch/docker/upload-docker-images.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/batch/docker/upload-docker-images.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/compute_node/user_data.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/compute_node/user_data.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/head_node/user_data.sh` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/head_node/user_data.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/imagebuilder/custom_script.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/custom_script.yaml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/imagebuilder/parallelcluster.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster.yaml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -102,31 +102,31 @@
       ### conditions ###
       - name: IntelMPISupported
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
-              [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} != 'arm64' ]] && echo "true" || echo "false"
+              [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} != 'arm64' && {{ validate.OperatingSystemName.outputs.stdout }} != 'rhel8' ]] && echo "true" || echo "false"
 
       - name: ArmPLSupported
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
-              [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} == 'arm64' ]] && echo "true" || echo "false"
+              [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} == 'arm64' && {{ validate.OperatingSystemName.outputs.stdout }} != 'rhel8' ]] && echo "true" || echo "false"
 
       - name: FabricManagerSupported
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
-              [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} == 'arm64' ]] && echo "false" || echo "true"
+              [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} == 'arm64' || {{ validate.OperatingSystemName.outputs.stdout }} == 'rhel8' ]] && echo "false" || echo "true"
 
       - name: LustreSupported
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
@@ -161,15 +161,15 @@
 
       - name: CudaVersion
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
-              PATTERN=$(jq '.default.cluster.nvidia.cuda.version' {{ CookbookDefaultFile }})
+              PATTERN=$(jq '.default.cluster.nvidia.cuda_version' {{ CookbookDefaultFile }})
               VERSION=$(echo ${PATTERN} | tr -d '\n' | cut -d = -f 2 | xargs)
               echo ${VERSION}
 
       - name: CudaSamplesSrcDir
         action: ExecuteBash
         inputs:
           commands:
@@ -266,15 +266,15 @@
                 if [ ${PLATFORM} == RHEL ]; then
                   rpm -qa | grep libfabric && rpm -qa | grep efa-
                   [[ $? -ne 0 ]] && echo "Check efa rpm failed" && exit 1
 
                   echo "Checking Intel MPI 20xx installed and module available..."
                   unset MODULEPATH
                   source /etc/profile.d/modules.sh
-                  (module avail intelmpi)2>&1 | grep "/opt/intel/mpi/20.*/modulefiles"
+                  (module avail intelmpi)2>&1 | grep "/opt/intel/mpi/20.*/modulefiles/"
                   [[ $? -ne 0 ]] && echo "Check Intel MPI failed" && exit 1
                 else
                   dpkg -l | grep libfabric && modinfo efa | grep efa && [ -d /opt/amazon/efa ]
                   [[ $? -ne 0 ]] && echo "Check efa deb failed" && exit 1
                 fi
               fi
               echo "EFA test passed"
@@ -283,15 +283,15 @@
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -vx
               PLATFORM='{{ validate.PlatformName.outputs.stdout }}'
 
-              if [[ {{ validate.NvidiaEnabled.outputs.stdout }} == 'no' ]]; then
+              if [[ {{ validate.NvidiaEnabled.outputs.stdout }} == 'no' || {{ validate.OperatingSystemName.outputs.stdout }} == 'rhel8' ]]; then
                 echo "Nvidia recipe not enabled, skipping." && exit 0
               fi
               if [ {{ validate.HasGPU.outputs.stdout }} == "false" ]; then
                 echo "No GPU detected, skipping." && exit 0
               fi
 
               driver_ver="{{ validate.NvidiaDriverVersion.outputs.stdout }}"
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/resources/imagebuilder/update_and_reboot.yaml` & `aws-parallelcluster-3.6.0b1/src/pcluster/resources/imagebuilder/update_and_reboot.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -124,33 +124,15 @@
           commands:
             - |
               set -v
               OS='{{ build.OperatingSystemName.outputs.stdout }}'
               PLATFORM='{{ build.PlatformName.outputs.stdout }}'
 
               if [[ ${!PLATFORM} == RHEL ]]; then
-                yum -y update
-              
-                if [[ ${!OS} != "rhel8" ]]; then
-                  package-cleanup -y --oldkernels --count=1
-                else
-                  # package-cleanup has changed in RHEL8 and it works differently
-                  # RHEL8 keeps at least 2 kernel for fallback reason https://access.redhat.com/solutions/1227
-                  # The kernel cleanup should be performed manually
-              
-                  # get the default kernel for the next boot
-                  LAST_KERNEL_VERSION=$(grubby --default-kernel | sed -e "s/.*-\(4.18.0-.*\).$(uname -m)/\1/g")
-                  
-                  # get all the installed kernel versions except the one for the next boot
-                  KERNEL_VERSIONS_CLEANUP=$(rpm -q --qf "%{VERSION}-%{RELEASE}\n" kernel | grep -v "$LAST_KERNEL_VERSION")
-                  for VERSION in $KERNEL_VERSIONS_CLEANUP; do
-                    echo "Removing kernel-$VERSION kernel-core-$VERSION kernel-modules-$VERSION"
-                    rpm -e kernel-$VERSION kernel-core-$VERSION kernel-modules-$VERSION;
-                  done
-                fi
+                yum -y update && package-cleanup -y --oldkernels --count=1
                 yum -y install kernel-devel
               elif [[ ${!PLATFORM} == DEBIAN ]]; then
                 while [ ! -f /var/lib/cloud/instance/boot-finished ]; do echo 'Waiting for cloud-init...'; sleep 1; done
                 flock $(apt-config shell StateDir Dir::State/d | sed -r "s/.*'(.*)\/?'$/\1/")/daily_lock systemctl disable --now apt-daily.timer apt-daily.service apt-daily-upgrade.timer apt-daily-upgrade.service
                 sed "/Update-Package-Lists/s/\"1\"/\"0\"/; /Unattended-Upgrade/s/\"1\"/\"0\"/;" /etc/apt/apt.conf.d/20auto-upgrades > "/etc/apt/apt.conf.d/51pcluster-unattended-upgrades"
                 DEBIAN_FRONTEND=noninteractive apt-get -y update && DEBIAN_FRONTEND=noninteractive apt-get -y -o Dpkg::Options::="--force-confdef" -o Dpkg::Options::="--force-confold" --with-new-pkgs upgrade && apt-get --purge autoremove -y
                 apt-get -y install linux-aws linux-headers-aws linux-image-aws
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/schemas/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/schemas/cluster_schema.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/schemas/cluster_schema.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/schemas/common_schema.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/schemas/common_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,26 +57,23 @@
     """
     if tags:
         for tag in tags:
             if isinstance(tag, BaseTag):
                 tag_key = tag.key
             else:
                 tag_key = tag.get("key", "")
-            if tag_key.startswith(PCLUSTER_PREFIX) and not tag_key == "parallelcluster:custom_resource":
+            if tag_key.startswith(PCLUSTER_PREFIX):
                 raise ValidationError(message=f"The tag key prefix '{PCLUSTER_PREFIX}' is reserved and cannot be used.")
 
 
 def validate_no_duplicate_tag(tags):
     """Validate there is no duplicate tag keys in the same tag section."""
     all_tags = set()
     for tag in tags:
-        if isinstance(tag, BaseTag):
-            tag_key = tag.key
-        else:
-            tag_key = tag.get("key", "")
+        tag_key = tag.key
         if tag_key in all_tags:
             raise ValidationError(
                 f"Duplicate tag key ({tag_key}) detected. Tags keys should be unique within the Tags section."
             )
         all_tags.add(tag_key)
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/schemas/imagebuilder_schema.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/schemas/imagebuilder_schema.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/templates/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/templates/awsbatch_builder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/awsbatch_builder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/templates/cdk_artifacts_manager.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/cdk_artifacts_manager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/templates/cdk_builder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/cdk_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import logging
 import os
 import tempfile
 
 from pcluster.config.cluster_config import BaseClusterConfig
 from pcluster.config.imagebuilder_config import ImageBuilderConfig
 from pcluster.models.s3_bucket import S3Bucket
+from pcluster.templates.cdk_artifacts_manager import CDKArtifactsManager
 from pcluster.utils import load_yaml_dict
 
 LOGGER = logging.getLogger(__name__)
 
 
 class CDKTemplateBuilder:
     """Create the template, starting from the given resources."""
@@ -30,16 +31,14 @@
     def build_cluster_template(
         cluster_config: BaseClusterConfig, bucket: S3Bucket, stack_name: str, log_group_name: str = None
     ):
         """Build template for the given cluster and return as output in Yaml format."""
         LOGGER.info("Importing CDK...")
         from aws_cdk.core import App  # pylint: disable=C0415
 
-        # CDK import must be inside the redirect_stdouterr_to_logger contextmanager
-        from pcluster.templates.cdk_artifacts_manager import CDKArtifactsManager  # pylint: disable=C0415
         from pcluster.templates.cluster_stack import ClusterCdkStack  # pylint: disable=C0415
 
         LOGGER.info("CDK import completed successfully")
         LOGGER.info("Starting CDK template generation...")
         with tempfile.TemporaryDirectory() as cloud_assembly_dir:
             output_file = str(stack_name)
             app = App(outdir=str(cloud_assembly_dir))
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/templates/cdk_builder_utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/cdk_builder_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/templates/cluster_stack.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/cluster_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -778,14 +778,15 @@
 
         return fsx_id
 
     def _add_efs_storage(self, id: str, shared_efs: SharedEfs):
         """Add specific Cfn Resources to map the EFS storage."""
         # EFS FileSystem
         efs_id = shared_efs.file_system_id
+        new_file_system = efs_id is None
         deletion_policy = convert_deletion_policy(shared_efs.deletion_policy)
         if not efs_id and shared_efs.mount_dir:
             efs_resource = efs.CfnFileSystem(
                 self.stack,
                 id,
                 encrypted=shared_efs.encrypted,
                 kms_key_id=shared_efs.kms_key_id,
@@ -793,68 +794,73 @@
                 provisioned_throughput_in_mibps=shared_efs.provisioned_throughput,
                 throughput_mode=shared_efs.throughput_mode,
             )
             efs_resource.tags.set_tag(key="Name", value=shared_efs.name)
             efs_resource.cfn_options.deletion_policy = efs_resource.cfn_options.update_replace_policy = deletion_policy
             efs_id = efs_resource.ref
 
-            # Create Mount Targets
-            checked_availability_zones = []
+        checked_availability_zones = []
 
-            # Mount Targets for Compute Fleet
-            compute_subnet_ids = self.config.compute_subnet_ids
-            file_system_security_groups = [self._add_storage_security_group(id, shared_efs)]
-
-            for subnet_id in compute_subnet_ids:
-                self._add_efs_mount_target(
-                    id,
-                    efs_id,
-                    file_system_security_groups,
-                    subnet_id,
-                    checked_availability_zones,
-                    deletion_policy,
-                )
+        # Mount Targets for Compute Fleet
+        compute_subnet_ids = self.config.compute_subnet_ids
+        file_system_security_groups = [self._add_storage_security_group(id, shared_efs)]
 
-            # Mount Target for Head Node
+        for subnet_id in compute_subnet_ids:
             self._add_efs_mount_target(
                 id,
                 efs_id,
                 file_system_security_groups,
-                self.config.head_node.networking.subnet_id,
+                subnet_id,
                 checked_availability_zones,
+                new_file_system,
                 deletion_policy,
             )
 
+        # Mount Target for Head Node
+        self._add_efs_mount_target(
+            id,
+            efs_id,
+            file_system_security_groups,
+            self.config.head_node.networking.subnet_id,
+            checked_availability_zones,
+            new_file_system,
+            deletion_policy,
+        )
+
         self.shared_storage_attributes[SharedStorageType.EFS]["EncryptionInTransits"].append(
             shared_efs.encryption_in_transit
         )
         self.shared_storage_attributes[SharedStorageType.EFS]["IamAuthorizations"].append(shared_efs.iam_authorization)
 
         return efs_id
 
     def _add_efs_mount_target(
         self,
         efs_cfn_resource_id,
         file_system_id,
         security_groups,
         subnet_id,
         checked_availability_zones,
+        new_file_system,
         deletion_policy,
     ):
         """Create a EFS Mount Point for the file system, if not already available on the same AZ."""
         availability_zone = AWSApi.instance().ec2.get_subnet_avail_zone(subnet_id)
         if availability_zone not in checked_availability_zones:
-            efs_resource = efs.CfnMountTarget(
-                self.stack,
-                "{0}MT{1}".format(efs_cfn_resource_id, availability_zone),
-                file_system_id=file_system_id,
-                security_groups=[sg.ref for sg in security_groups],
-                subnet_id=subnet_id,
-            )
-            efs_resource.cfn_options.deletion_policy = efs_resource.cfn_options.update_replace_policy = deletion_policy
+            if new_file_system:
+                efs_resource = efs.CfnMountTarget(
+                    self.stack,
+                    "{0}MT{1}".format(efs_cfn_resource_id, availability_zone),
+                    file_system_id=file_system_id,
+                    security_groups=[sg.ref for sg in security_groups],
+                    subnet_id=subnet_id,
+                )
+                efs_resource.cfn_options.deletion_policy = (
+                    efs_resource.cfn_options.update_replace_policy
+                ) = deletion_policy
             checked_availability_zones.append(availability_zone)
 
     def _add_raid_volume(self, id_prefix: str, shared_ebs: SharedEbs):
         """Add specific Cfn Resources to map the RAID EBS storage."""
         ebs_ids = []
         for index in range(shared_ebs.raid.number_of_volumes):
             ebs_ids.append(StorageInfo(self._add_cfn_volume(f"{id_prefix}Volume{index}", shared_ebs), shared_ebs))
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/templates/cw_dashboard_builder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/cw_dashboard_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 
 from aws_cdk import aws_cloudwatch as cloudwatch
 from aws_cdk import aws_ec2 as ec2
 from aws_cdk import aws_logs as logs
 from aws_cdk.core import Construct, Duration, Stack
 
 from pcluster.config.cluster_config import BaseClusterConfig, SharedFsxLustre, SharedStorageType
-from pcluster.constants import Feature
-from pcluster.utils import is_feature_supported
 
 MAX_WIDTH = 24
 
 
 class Coord:
     """Create coordinates for locating cloudwatch graphs."""
 
@@ -145,15 +143,15 @@
 
         # Add FSx metrics graphs
         if len(self.shared_storage_infos[SharedStorageType.FSX]) > 0:
             self._add_fsx_metrics_graphs()
 
         # Head Node logs add custom metrics if cw_log and metrics are enabled
         if self.config.is_cw_logging_enabled:
-            if self.config.scheduling.scheduler == "slurm" and is_feature_supported(Feature.CLUSTER_HEALTH_METRICS):
+            if self.config.scheduling.scheduler == "slurm":
                 self._add_custom_health_metrics()
             self._add_cw_log()
 
     def _update_coord(self, d_x, d_y):
         """Calculate coordinates for the new graph."""
         self.coord.x_value = self.coord.x_value + d_x
         x_value = self.coord.x_value + d_x
@@ -330,31 +328,22 @@
                 metric_value=metric_value,
             ),
             _CustomMetricFilter(
                 metric_name="NoCorrespondingInstanceErrors",
                 filter_pattern=_generate_metric_filter_pattern("invalid-backing-instance-count"),
                 metric_value=metric_value,
             ),
+            # Use text matching here because it comes from slurmctld.log
             _CustomMetricFilter(
                 metric_name="SlurmNodeNotRespondingErrors",
                 filter_pattern=_generate_metric_filter_pattern("node-not-responding-down-count"),
                 metric_value=metric_value,
             ),
         ]
 
-        if self.config.has_gpu_health_checks_enabled:
-            compute_node_events.append(
-                _CustomMetricFilter(
-                    metric_name="GpuHealthCheckFailures",
-                    filter_pattern='{ $.event-type = "compute-node-health-check" && $.scheduler = "slurm" && '
-                    '$.detail.health-check-name = "Gpu" && $.detail.health-check-result != 0 }',
-                    metric_value="1",
-                )
-            )
-
         cluster_health_metrics = [
             _HealthMetric(
                 "Instance Provisioning Errors",
                 jobs_not_starting_errors,
                 left_y_axis=cloudwatch.YAxisProps(min=0.0),
             ),
             _HealthMetric(
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/templates/imagebuilder_stack.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/imagebuilder_stack.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/templates/import_cdk.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/import_cdk.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/templates/queues_stack.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/queue_group_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     scheduler_is_slurm,
     to_comma_separated_string,
 )
 from pcluster.templates.slurm_builder import SlurmConstruct
 from pcluster.utils import get_attr, get_http_tokens_setting
 
 
-class QueuesStack(NestedStack):
+class QueueGroupStack(NestedStack):
     """Stack encapsulating a set of queues and the associated resources."""
 
     def __init__(
         self,
         scope: Construct,
         id: str,
         queues: List[SlurmQueue],
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/templates/slurm_builder.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/templates/slurm_builder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,15 @@
 import pkg_resources
 import yaml
 from yaml import SafeLoader
 from yaml.constructor import ConstructorError
 from yaml.resolver import BaseResolver
 
 from pcluster.aws.common import get_region
-from pcluster.constants import (
-    SUPPORTED_OSES_FOR_ARCHITECTURE,
-    SUPPORTED_OSES_FOR_SCHEDULER,
-    UNSUPPORTED_FEATURES_MAP,
-    Feature,
-)
+from pcluster.constants import SUPPORTED_OSES_FOR_ARCHITECTURE, SUPPORTED_OSES_FOR_SCHEDULER
 
 LOGGER = logging.getLogger(__name__)
 
 DEFAULT_PARTITION = "aws"
 PARTITION_MAP = {
     "cn-": "aws-cn",
     "us-gov-": "aws-us-gov",
@@ -168,25 +163,14 @@
 
 
 def get_supported_os_for_architecture(architecture):
     """Return list of supported OSes for the specified architecture."""
     return SUPPORTED_OSES_FOR_ARCHITECTURE.get(architecture, [])
 
 
-def is_feature_supported(feature: Feature, region: str = None):
-    """
-    Check if a feature is supported for the given region.
-
-    If region is None, consider the region set in the environment.
-    """
-    _region = get_region() if region is None else region
-    prefixes_of_unsupported_regions = UNSUPPORTED_FEATURES_MAP.get(feature, [])
-    return all(not _region.startswith(region_prefix) for region_prefix in prefixes_of_unsupported_regions)
-
-
 def to_utc_datetime(time_in, default_timezone=datetime.timezone.utc) -> datetime.datetime:
     """
     Convert a given string, datetime or int into utc datetime.
 
     :param time_in: Time in a format that may be parsed, integers are assumed to
     be timestamps in UTC timezone.
     :param default_timezone: Timezone to assum in the event that the time is
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/awsbatch_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/awsbatch_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/cluster_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/cluster_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/common.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/database_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/database_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/directory_service_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/directory_service_validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 from urllib.parse import urlparse
 
+from aws_cdk.core import Arn, ArnFormat
+
 from pcluster.aws.aws_api import AWSApi
 from pcluster.aws.common import AWSClientError
 from pcluster.constants import DIRECTORY_SERVICE_RESERVED_SETTINGS
 from pcluster.validators.common import FailureLevel, Validator
 
 
 class DomainAddrValidator(Validator):
@@ -78,24 +80,20 @@
 
         In particular, the ARN should be one of the following resources:
          1. a readable secret in AWS Secrets Manager, which is supported in all regions but us-isob-east-1.
          2. a readable parameter in SSM Parameter Store, which is supported only in us-isob-east-1.
         """
         try:
             # We only require the secret to exist; we do not validate its content.
-            arn_components = password_secret_arn.split(":")
-            service = arn_components[2]
-            resource = arn_components[5]
-            if service == "ssm":
-                resource = arn_components[5].split("/")[0]
-
+            arn_components = Arn.split(password_secret_arn, ArnFormat.COLON_RESOURCE_NAME)
+            service, resource = arn_components.service, arn_components.resource
             if service == "secretsmanager" and resource == "secret" and region != "us-isob-east-1":
                 AWSApi.instance().secretsmanager.describe_secret(password_secret_arn)
             elif service == "ssm" and resource == "parameter" and region == "us-isob-east-1":
-                parameter_name = arn_components[5].split("/")[1]
+                parameter_name = arn_components.resource_name
                 AWSApi.instance().ssm.get_parameter(parameter_name)
             else:
                 self._add_failure(
                     f"The secret {password_secret_arn} is not supported in region {region}.", FailureLevel.ERROR
                 )
         except AWSClientError as e:
             if e.error_code in ("ResourceNotFoundExceptionSecrets", "ParameterNotFound"):
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/ebs_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/ebs_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/ec2_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/ec2_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/efs_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/efs_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/feature_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/feature_validators.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,29 @@
 #
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # This module contains all the classes representing the Resources objects.
 # These objects are obtained from the configuration file through a conversion based on the Schema classes.
-from pcluster import utils
-from pcluster.constants import Feature
+from pcluster.aws.common import get_region
+from pcluster.constants import UNSUPPORTED_FEATURES_MAP, Feature
 from pcluster.validators.common import FailureLevel, Validator
 
 
 class FeatureRegionValidator(Validator):
     """Validate if a feature is supported in the given region."""
 
     def _validate(self, feature: Feature, region: str):
-        if not utils.is_feature_supported(feature, region):
+        if not self._is_feature_supported(feature, region):
             self._add_failure(f"{feature.value} is not supported in region '{region}'.", FailureLevel.ERROR)
+
+    @staticmethod
+    def _is_feature_supported(feature: Feature, region: str):
+        """
+        Check if a feature is supported for the given region.
+
+        If region is None, consider the region set in the environment.
+        """
+        _region = get_region() if region is None else region
+        prefixes_of_unsupported_regions = UNSUPPORTED_FEATURES_MAP.get(feature, [])
+        return all(not _region.startswith(region_prefix) for region_prefix in prefixes_of_unsupported_regions)
```

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/fsx_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/fsx_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/iam_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/iam_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/imagebuilder_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/imagebuilder_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/instances_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/instances_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/kms_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/kms_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/monitoring_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/monitoring_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/networking_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/networking_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/s3_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/s3_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/scheduler_plugin_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/scheduler_plugin_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/slurm_settings_validator.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/slurm_settings_validator.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/tags_validators.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/tags_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster/validators/utils.py` & `aws-parallelcluster-3.6.0b1/src/pcluster/validators/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster3_config_converter/__init__.py` & `aws-parallelcluster-3.6.0b1/src/pcluster3_config_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.0/src/pcluster3_config_converter/pcluster3_config_converter.py` & `aws-parallelcluster-3.6.0b1/src/pcluster3_config_converter/pcluster3_config_converter.py`

 * *Files identical despite different names*

