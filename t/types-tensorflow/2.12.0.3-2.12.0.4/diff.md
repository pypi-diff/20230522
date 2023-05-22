# Comparing `tmp/types-tensorflow-2.12.0.3.tar.gz` & `tmp/types-tensorflow-2.12.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tensorflow-2.12.0.3.tar", last modified: Wed May 10 15:23:36 2023, max compression
+gzip compressed data, was "types-tensorflow-2.12.0.4.tar", last modified: Mon May 22 15:15:42 2023, max compression
```

## Comparing `types-tensorflow-2.12.0.3.tar` & `types-tensorflow-2.12.0.4.tar`

### file list

```diff
@@ -1,139 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-10 15:23:35.000000 types-tensorflow-2.12.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:23:35.000000 types-tensorflow-2.12.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-10 15:23:35.000000 types-tensorflow-2.12.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.270543 types-tensorflow-2.12.0.3/tensorflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-10 15:23:35.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/_aliases.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.266543 types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.270543 types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/xla/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.270543 types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/xla/service/
--rw-r--r--   0 runner    (1001) docker     (123)    78294 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    78920 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.270543 types-tensorflow-2.12.0.3/tensorflow-stubs/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.270543 types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/example_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/feature_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.274543 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/api_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/attr_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22095 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23251 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/full_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/log_memory_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/node_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/op_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/reader_base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/step_stats_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/summary_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/variable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.278544 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    77923 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26277 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/debug_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28896 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27624 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/saver_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.278544 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    51042 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.278544 types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/test_log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/dtypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.278544 types-tensorflow-2.12.0.3/tensorflow-stubs/feature_column/
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.278544 types-tensorflow-2.12.0.3/tensorflow-stubs/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/io/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/io/gfile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/activations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/constraints.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/initializers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/layers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/schedules.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/regularizers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/math.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/python/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/python/feature_column/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/python/trackable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/trackable/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/trackable/autotrackable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/trackable/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/sparse.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.270543 types-tensorflow-2.12.0.3/tensorflow-stubs/tsl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/tsl/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/types_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-10 15:23:36.000000 types-tensorflow-2.12.0.3/types_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-05-10 15:23:36.000000 types-tensorflow-2.12.0.3/types_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:23:36.000000 types-tensorflow-2.12.0.3/types_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 15:23:36.000000 types-tensorflow-2.12.0.3/types_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 15:23:36.000000 types-tensorflow-2.12.0.3/types_tensorflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-22 15:15:41.000000 types-tensorflow-2.12.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 15:15:41.000000 types-tensorflow-2.12.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-22 15:15:41.000000 types-tensorflow-2.12.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.404107 types-tensorflow-2.12.0.4/tensorflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-22 15:15:41.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/_aliases.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.400107 types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.404107 types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/xla/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.404107 types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/xla/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    78294 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    78920 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.400107 types-tensorflow-2.12.0.4/tensorflow-stubs/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.404107 types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/example_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/feature_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.408107 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/api_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/attr_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22095 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23251 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/full_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/log_memory_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/node_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/op_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/reader_base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/step_stats_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/summary_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/variable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    77923 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26277 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/debug_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28896 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27624 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/saver_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    51042 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/test_log_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/data/experimental.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/dtypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/experimental/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/io/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/io/gfile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/activations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/initializers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/layers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/schedules.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/regularizers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/math.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/python/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/python/trackable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/trackable/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/trackable/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/trackable/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/sparse.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.404107 types-tensorflow-2.12.0.4/tensorflow-stubs/tsl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/tsl/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/types_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-22 15:15:42.000000 types-tensorflow-2.12.0.4/types_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-22 15:15:42.000000 types-tensorflow-2.12.0.4/types_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:15:42.000000 types-tensorflow-2.12.0.4/types_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 15:15:42.000000 types-tensorflow-2.12.0.4/types_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 15:15:42.000000 types-tensorflow-2.12.0.4/types_tensorflow.egg-info/top_level.txt
```

### Comparing `types-tensorflow-2.12.0.3/CHANGELOG.md` & `types-tensorflow-2.12.0.4/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 2.12.0.4 (2023-05-22)
+
+Add core tensorflow.data stubs (#10122)
+
+Co-authored-by: Mehdi Drissi <mdrissi@snapchat.com>
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
+
 ## 2.12.0.3 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 2.12.0.2 (2023-04-27)
 
 tensorflow: feature columns (#10052)
```

### Comparing `types-tensorflow-2.12.0.3/PKG-INFO` & `types-tensorflow-2.12.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.12.0.3
+Version: 2.12.0.4
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `510547ef3c07502faec40cc4c070e2c0dcda7f93`.
```

### Comparing `types-tensorflow-2.12.0.3/setup.py` & `types-tensorflow-2.12.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `510547ef3c07502faec40cc4c070e2c0dcda7f93`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.12.0.3",
+      version="2.12.0.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-protobuf', 'numpy>=1.20'],
       packages=['tensorflow-stubs'],
-      package_data={'tensorflow-stubs': ['__init__.pyi', '_aliases.pyi', 'compiler/xla/service/hlo_pb2.pyi', 'compiler/xla/xla_data_pb2.pyi', 'core/example/example_parser_configuration_pb2.pyi', 'core/example/example_pb2.pyi', 'core/example/feature_pb2.pyi', 'core/framework/allocation_description_pb2.pyi', 'core/framework/api_def_pb2.pyi', 'core/framework/attr_value_pb2.pyi', 'core/framework/cost_graph_pb2.pyi', 'core/framework/dataset_metadata_pb2.pyi', 'core/framework/dataset_options_pb2.pyi', 'core/framework/device_attributes_pb2.pyi', 'core/framework/full_type_pb2.pyi', 'core/framework/function_pb2.pyi', 'core/framework/graph_pb2.pyi', 'core/framework/graph_transfer_info_pb2.pyi', 'core/framework/kernel_def_pb2.pyi', 'core/framework/log_memory_pb2.pyi', 'core/framework/model_pb2.pyi', 'core/framework/node_def_pb2.pyi', 'core/framework/op_def_pb2.pyi', 'core/framework/reader_base_pb2.pyi', 'core/framework/resource_handle_pb2.pyi', 'core/framework/step_stats_pb2.pyi', 'core/framework/summary_pb2.pyi', 'core/framework/tensor_description_pb2.pyi', 'core/framework/tensor_pb2.pyi', 'core/framework/tensor_shape_pb2.pyi', 'core/framework/tensor_slice_pb2.pyi', 'core/framework/types_pb2.pyi', 'core/framework/variable_pb2.pyi', 'core/framework/versions_pb2.pyi', 'core/protobuf/bfc_memory_map_pb2.pyi', 'core/protobuf/cluster_pb2.pyi', 'core/protobuf/composite_tensor_variant_pb2.pyi', 'core/protobuf/config_pb2.pyi', 'core/protobuf/control_flow_pb2.pyi', 'core/protobuf/coordination_config_pb2.pyi', 'core/protobuf/core_platform_payloads_pb2.pyi', 'core/protobuf/data_service_pb2.pyi', 'core/protobuf/debug_event_pb2.pyi', 'core/protobuf/debug_pb2.pyi', 'core/protobuf/device_filters_pb2.pyi', 'core/protobuf/device_properties_pb2.pyi', 'core/protobuf/distributed_runtime_payloads_pb2.pyi', 'core/protobuf/error_codes_pb2.pyi', 'core/protobuf/fingerprint_pb2.pyi', 'core/protobuf/graph_debug_info_pb2.pyi', 'core/protobuf/meta_graph_pb2.pyi', 'core/protobuf/named_tensor_pb2.pyi', 'core/protobuf/queue_runner_pb2.pyi', 'core/protobuf/remote_tensor_handle_pb2.pyi', 'core/protobuf/rewriter_config_pb2.pyi', 'core/protobuf/saved_model_pb2.pyi', 'core/protobuf/saved_object_graph_pb2.pyi', 'core/protobuf/saver_pb2.pyi', 'core/protobuf/service_config_pb2.pyi', 'core/protobuf/snapshot_pb2.pyi', 'core/protobuf/struct_pb2.pyi', 'core/protobuf/tensor_bundle_pb2.pyi', 'core/protobuf/tensorflow_server_pb2.pyi', 'core/protobuf/tpu/compilation_result_pb2.pyi', 'core/protobuf/tpu/dynamic_padding_pb2.pyi', 'core/protobuf/tpu/optimization_parameters_pb2.pyi', 'core/protobuf/tpu/topology_pb2.pyi', 'core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi', 'core/protobuf/trackable_object_graph_pb2.pyi', 'core/protobuf/transport_options_pb2.pyi', 'core/protobuf/verifier_config_pb2.pyi', 'core/util/event_pb2.pyi', 'core/util/memmapped_file_system_pb2.pyi', 'core/util/saved_tensor_slice_pb2.pyi', 'core/util/test_log_pb2.pyi', 'dtypes.pyi', 'feature_column/__init__.pyi', 'initializers.pyi', 'io/__init__.pyi', 'io/gfile.pyi', 'keras/__init__.pyi', 'keras/activations.pyi', 'keras/constraints.pyi', 'keras/initializers.pyi', 'keras/layers.pyi', 'keras/optimizers/__init__.pyi', 'keras/optimizers/legacy/__init__.pyi', 'keras/optimizers/schedules.pyi', 'keras/regularizers.pyi', 'math.pyi', 'python/__init__.pyi', 'python/feature_column/__init__.pyi', 'python/feature_column/feature_column_v2.pyi', 'python/feature_column/sequence_feature_column.pyi', 'python/keras/__init__.pyi', 'python/keras/protobuf/projector_config_pb2.pyi', 'python/keras/protobuf/saved_metadata_pb2.pyi', 'python/keras/protobuf/versions_pb2.pyi', 'python/trackable/__init__.pyi', 'python/trackable/autotrackable.pyi', 'python/trackable/base.pyi', 'sparse.pyi', 'tsl/protobuf/error_codes_pb2.pyi', 'tsl/protobuf/histogram_pb2.pyi', 'METADATA.toml']},
+      package_data={'tensorflow-stubs': ['__init__.pyi', '_aliases.pyi', 'compiler/xla/service/hlo_pb2.pyi', 'compiler/xla/xla_data_pb2.pyi', 'core/example/example_parser_configuration_pb2.pyi', 'core/example/example_pb2.pyi', 'core/example/feature_pb2.pyi', 'core/framework/allocation_description_pb2.pyi', 'core/framework/api_def_pb2.pyi', 'core/framework/attr_value_pb2.pyi', 'core/framework/cost_graph_pb2.pyi', 'core/framework/dataset_metadata_pb2.pyi', 'core/framework/dataset_options_pb2.pyi', 'core/framework/device_attributes_pb2.pyi', 'core/framework/full_type_pb2.pyi', 'core/framework/function_pb2.pyi', 'core/framework/graph_pb2.pyi', 'core/framework/graph_transfer_info_pb2.pyi', 'core/framework/kernel_def_pb2.pyi', 'core/framework/log_memory_pb2.pyi', 'core/framework/model_pb2.pyi', 'core/framework/node_def_pb2.pyi', 'core/framework/op_def_pb2.pyi', 'core/framework/reader_base_pb2.pyi', 'core/framework/resource_handle_pb2.pyi', 'core/framework/step_stats_pb2.pyi', 'core/framework/summary_pb2.pyi', 'core/framework/tensor_description_pb2.pyi', 'core/framework/tensor_pb2.pyi', 'core/framework/tensor_shape_pb2.pyi', 'core/framework/tensor_slice_pb2.pyi', 'core/framework/types_pb2.pyi', 'core/framework/variable_pb2.pyi', 'core/framework/versions_pb2.pyi', 'core/protobuf/__init__.pyi', 'core/protobuf/bfc_memory_map_pb2.pyi', 'core/protobuf/cluster_pb2.pyi', 'core/protobuf/composite_tensor_variant_pb2.pyi', 'core/protobuf/config_pb2.pyi', 'core/protobuf/control_flow_pb2.pyi', 'core/protobuf/coordination_config_pb2.pyi', 'core/protobuf/core_platform_payloads_pb2.pyi', 'core/protobuf/data_service_pb2.pyi', 'core/protobuf/debug_event_pb2.pyi', 'core/protobuf/debug_pb2.pyi', 'core/protobuf/device_filters_pb2.pyi', 'core/protobuf/device_properties_pb2.pyi', 'core/protobuf/distributed_runtime_payloads_pb2.pyi', 'core/protobuf/error_codes_pb2.pyi', 'core/protobuf/fingerprint_pb2.pyi', 'core/protobuf/graph_debug_info_pb2.pyi', 'core/protobuf/meta_graph_pb2.pyi', 'core/protobuf/named_tensor_pb2.pyi', 'core/protobuf/queue_runner_pb2.pyi', 'core/protobuf/remote_tensor_handle_pb2.pyi', 'core/protobuf/rewriter_config_pb2.pyi', 'core/protobuf/saved_model_pb2.pyi', 'core/protobuf/saved_object_graph_pb2.pyi', 'core/protobuf/saver_pb2.pyi', 'core/protobuf/service_config_pb2.pyi', 'core/protobuf/snapshot_pb2.pyi', 'core/protobuf/struct_pb2.pyi', 'core/protobuf/tensor_bundle_pb2.pyi', 'core/protobuf/tensorflow_server_pb2.pyi', 'core/protobuf/tpu/compilation_result_pb2.pyi', 'core/protobuf/tpu/dynamic_padding_pb2.pyi', 'core/protobuf/tpu/optimization_parameters_pb2.pyi', 'core/protobuf/tpu/topology_pb2.pyi', 'core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi', 'core/protobuf/trackable_object_graph_pb2.pyi', 'core/protobuf/transport_options_pb2.pyi', 'core/protobuf/verifier_config_pb2.pyi', 'core/util/event_pb2.pyi', 'core/util/memmapped_file_system_pb2.pyi', 'core/util/saved_tensor_slice_pb2.pyi', 'core/util/test_log_pb2.pyi', 'data/__init__.pyi', 'data/experimental.pyi', 'dtypes.pyi', 'experimental/__init__.pyi', 'feature_column/__init__.pyi', 'initializers.pyi', 'io/__init__.pyi', 'io/gfile.pyi', 'keras/__init__.pyi', 'keras/activations.pyi', 'keras/constraints.pyi', 'keras/initializers.pyi', 'keras/layers.pyi', 'keras/optimizers/__init__.pyi', 'keras/optimizers/legacy/__init__.pyi', 'keras/optimizers/schedules.pyi', 'keras/regularizers.pyi', 'math.pyi', 'python/__init__.pyi', 'python/feature_column/__init__.pyi', 'python/feature_column/feature_column_v2.pyi', 'python/feature_column/sequence_feature_column.pyi', 'python/keras/__init__.pyi', 'python/keras/protobuf/projector_config_pb2.pyi', 'python/keras/protobuf/saved_metadata_pb2.pyi', 'python/keras/protobuf/versions_pb2.pyi', 'python/trackable/__init__.pyi', 'python/trackable/autotrackable.pyi', 'python/trackable/base.pyi', 'sparse.pyi', 'tsl/protobuf/error_codes_pb2.pyi', 'tsl/protobuf/histogram_pb2.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/__init__.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 from _typeshed import Incomplete, Unused
-from abc import ABCMeta
+from abc import ABC, ABCMeta, abstractmethod
 from builtins import bool as _bool
 from collections.abc import Callable, Generator, Iterable, Iterator, Mapping, Sequence
 from contextlib import contextmanager
 from enum import Enum
 from types import TracebackType
-from typing import Any, NoReturn, TypeVar, overload
+from typing import Any, Generic, NoReturn, TypeVar, overload
 from typing_extensions import ParamSpec, Self, TypeAlias
 
 import numpy
-from tensorflow import feature_column as feature_column, initializers as initializers, io as io, keras as keras, math as math
+from google.protobuf.message import Message
+from tensorflow import (
+    data as data,
+    experimental as experimental,
+    feature_column as feature_column,
+    initializers as initializers,
+    io as io,
+    keras as keras,
+    math as math,
+)
 from tensorflow._aliases import ContainerGradients, ContainerTensors, ContainerTensorsLike, Gradients, TensorLike
+from tensorflow.core.protobuf import struct_pb2
 
 # Explicit import of DType is covered by the wildcard, but
 # is necessary to avoid a crash in pytype.
 from tensorflow.dtypes import *
 from tensorflow.dtypes import DType as DType
 
 # Most tf.math functions are exported as tf, but sadly not all are.
@@ -328,8 +338,70 @@
     @contextmanager
     def stop_recording(self) -> Generator[None, None, None]: ...
     def reset(self) -> None: ...
     def watch(self, tensor: ContainerTensorsLike) -> None: ...
     def watched_variables(self) -> tuple[Variable, ...]: ...
     def __getattr__(self, name: str) -> Incomplete: ...
 
+_SpecProto = TypeVar("_SpecProto", bound=Message)
+
+class TypeSpec(Generic[_SpecProto], ABC):
+    @property
+    @abstractmethod
+    def value_type(self) -> Any: ...
+    def experimental_as_proto(self) -> _SpecProto: ...
+    @classmethod
+    def experimental_from_proto(cls, proto: _SpecProto) -> Self: ...
+    @classmethod
+    def experimental_type_proto(cls) -> type[_SpecProto]: ...
+    def is_compatible_with(self, spec_or_value: Self | _TensorCompatible | SparseTensor | RaggedTensor) -> _bool: ...
+    # Incomplete as tf.types is not yet covered.
+    def is_subtype_of(self, other: Incomplete) -> _bool: ...
+    def most_specific_common_supertype(self, others: Sequence[Incomplete]) -> Self | None: ...
+    def most_specific_compatible_type(self, other: Self) -> Self: ...
+
+class TensorSpec(TypeSpec[struct_pb2.TensorSpecProto]):
+    def __init__(self, shape: _ShapeLike, dtype: _DTypeLike = ..., name: str | None = None) -> None: ...
+    @property
+    def value_type(self) -> Tensor: ...
+    @property
+    def shape(self) -> TensorShape: ...
+    @property
+    def dtype(self) -> DType: ...
+    @property
+    def name(self) -> str | None: ...
+    @classmethod
+    def from_spec(cls, spec: TypeSpec[Any], name: str | None = None) -> Self: ...
+    @classmethod
+    def from_tensor(cls, tensor: Tensor, name: str | None = None) -> Self: ...
+    def is_compatible_with(self, spec_or_tensor: Self | _TensorCompatible) -> _bool: ...  # type: ignore[override]
+
+class SparseTensorSpec(TypeSpec[struct_pb2.TypeSpecProto]):
+    def __init__(self, shape: _ShapeLike | None = None, dtype: _DTypeLike = ...) -> None: ...
+    @property
+    def value_type(self) -> SparseTensor: ...
+    @property
+    def shape(self) -> TensorShape: ...
+    @property
+    def dtype(self) -> DType: ...
+    @classmethod
+    def from_value(cls, value: SparseTensor) -> Self: ...
+
+class RaggedTensorSpec(TypeSpec[struct_pb2.TypeSpecProto]):
+    def __init__(
+        self,
+        shape: _ShapeLike | None = None,
+        dtype: _DTypeLike = ...,
+        ragged_rank: int | None = None,
+        row_splits_dtype: _DTypeLike = ...,
+        flat_values_spec: TypeSpec[Any] | None = None,
+    ) -> None: ...
+    @property
+    def value_type(self) -> RaggedTensor: ...
+    @property
+    def shape(self) -> TensorShape: ...
+    @property
+    def dtype(self) -> DType: ...
+    @classmethod
+    def from_value(cls, value: RaggedTensor) -> Self: ...
+
 def __getattr__(name: str) -> Incomplete: ...
```

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/_aliases.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/_aliases.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/example_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/example_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/feature_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/feature_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/allocation_description_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/allocation_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/api_def_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/api_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/attr_value_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/attr_value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/cost_graph_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/cost_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/dataset_options_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/dataset_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/device_attributes_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/device_attributes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/full_type_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/full_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/function_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/graph_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/kernel_def_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/kernel_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/log_memory_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/log_memory_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/model_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/node_def_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/node_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/op_def_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/op_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/reader_base_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/reader_base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/resource_handle_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/resource_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/step_stats_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/step_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/summary_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/summary_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_description_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/types_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/variable_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/variable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/versions_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/cluster_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/config_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/data_service_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/data_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/debug_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/debug_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/saver_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/saver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/service_config_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/service_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/struct_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/struct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/event_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/test_log_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/test_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/dtypes.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/feature_column/__init__.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/feature_column/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/io/__init__.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/io/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from tensorflow import _DTypeLike, _ShapeLike, _TensorCompatible
 from tensorflow._aliases import TensorLike
 from tensorflow.io import gfile as gfile
 
 _FeatureSpecs: TypeAlias = Mapping[str, FixedLenFeature | FixedLenSequenceFeature | VarLenFeature | RaggedFeature | SparseFeature]
 
-_CompressionTypes: TypeAlias = Literal["ZLIB", "GZIP", "", 0, 1, 2] | None
+_CompressionTypes: TypeAlias = Literal["ZLIB", "GZIP", "AUTO", "", 0, 1, 2] | None
 _CompressionLevels: TypeAlias = Literal[0, 1, 2, 3, 4, 5, 6, 7, 8, 9] | None
 _MemoryLevels: TypeAlias = Literal[1, 2, 3, 4, 5, 6, 7, 8, 9] | None
 
 class TFRecordOptions:
     compression_type: _CompressionTypes | TFRecordOptions
     flush_mode: int | None  # The exact values allowed comes from zlib
     input_buffer_size: int | None
```

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/io/gfile.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/io/gfile.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/keras/constraints.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/keras/constraints.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/keras/initializers.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/keras/initializers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/keras/layers.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/keras/layers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/schedules.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/schedules.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/keras/regularizers.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/keras/regularizers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/math.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/math.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/python/feature_column/feature_column_v2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/python/feature_column/feature_column_v2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/sparse.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/sparse.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi` & `types-tensorflow-2.12.0.4/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.3/types_tensorflow.egg-info/PKG-INFO` & `types-tensorflow-2.12.0.4/types_tensorflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.12.0.3
+Version: 2.12.0.4
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `510547ef3c07502faec40cc4c070e2c0dcda7f93`.
```

### Comparing `types-tensorflow-2.12.0.3/types_tensorflow.egg-info/SOURCES.txt` & `types-tensorflow-2.12.0.4/types_tensorflow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 tensorflow-stubs/core/framework/tensor_description_pb2.pyi
 tensorflow-stubs/core/framework/tensor_pb2.pyi
 tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
 tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
 tensorflow-stubs/core/framework/types_pb2.pyi
 tensorflow-stubs/core/framework/variable_pb2.pyi
 tensorflow-stubs/core/framework/versions_pb2.pyi
+tensorflow-stubs/core/protobuf/__init__.pyi
 tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
 tensorflow-stubs/core/protobuf/cluster_pb2.pyi
 tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
 tensorflow-stubs/core/protobuf/config_pb2.pyi
 tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
 tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi
 tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
@@ -77,14 +78,17 @@
 tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
 tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
 tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
 tensorflow-stubs/core/util/event_pb2.pyi
 tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
 tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
 tensorflow-stubs/core/util/test_log_pb2.pyi
+tensorflow-stubs/data/__init__.pyi
+tensorflow-stubs/data/experimental.pyi
+tensorflow-stubs/experimental/__init__.pyi
 tensorflow-stubs/feature_column/__init__.pyi
 tensorflow-stubs/io/__init__.pyi
 tensorflow-stubs/io/gfile.pyi
 tensorflow-stubs/keras/__init__.pyi
 tensorflow-stubs/keras/activations.pyi
 tensorflow-stubs/keras/constraints.pyi
 tensorflow-stubs/keras/initializers.pyi
```

