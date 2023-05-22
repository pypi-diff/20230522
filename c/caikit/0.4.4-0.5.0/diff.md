# Comparing `tmp/caikit-0.4.4.tar.gz` & `tmp/caikit-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.4.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caikit-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caikit-0.4.4.tar` & `caikit-0.5.0.tar`

### file list

```diff
@@ -1,320 +1,305 @@
--rw-r--r--   0        0        0       60 2023-05-18 22:23:26.587025 caikit-0.4.4/.coveragerc
--rw-r--r--   0        0        0      676 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/dependabot.yml
--rw-r--r--   0        0        0     1272 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1328 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      261 2023-05-18 22:23:26.587025 caikit-0.4.4/.gitignore
--rw-r--r--   0        0        0      324 2023-05-18 22:23:26.587025 caikit-0.4.4/.isort.cfg
--rw-r--r--   0        0        0      370 2023-05-18 22:23:26.587025 caikit-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-05-18 22:23:26.587025 caikit-0.4.4/.prettierignore
--rw-r--r--   0        0        0       12 2023-05-18 22:23:26.587025 caikit-0.4.4/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-05-18 22:23:26.587025 caikit-0.4.4/.pylintrc
--rw-r--r--   0        0        0       78 2023-05-18 22:23:26.587025 caikit-0.4.4/.whitesource
--rw-r--r--   0        0        0      368 2023-05-18 22:23:26.587025 caikit-0.4.4/CODEOWNERS
--rw-r--r--   0        0        0     7165 2023-05-18 22:23:26.587025 caikit-0.4.4/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-05-18 22:23:26.587025 caikit-0.4.4/LICENSE
--rw-r--r--   0        0        0     3626 2023-05-18 22:23:26.587025 caikit-0.4.4/README.md
--rw-r--r--   0        0        0      152 2023-05-18 22:23:26.587025 caikit-0.4.4/SECURITY.md
--rw-r--r--   0        0        0    44878 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit-overview.png
--rw-r--r--   0        0        0      419 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/config/__init__.py
--rw-r--r--   0        0        0     6052 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/config/config.py
--rw-r--r--   0        0        0     6554 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/config/config.yml
--rw-r--r--   0        0        0     1838 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0      974 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/blocks/__init__.py
--rw-r--r--   0        0        0     1586 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/blocks/base.py
--rw-r--r--   0        0        0     1026 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    35512 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     4050 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    13826 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     4858 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1564 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40248 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    21916 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/model_manager.py
--rw-r--r--   0        0        0    41505 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module.py
--rw-r--r--   0        0        0     6062 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_backend_config.py
--rw-r--r--   0        0        0      684 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     3399 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     4716 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     2769 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     6293 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_config.py
--rw-r--r--   0        0        0     6247 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_meta.py
--rw-r--r--   0        0        0    14929 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_type.py
--rw-r--r--   0        0        0      709 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/resources/__init__.py
--rw-r--r--   0        0        0     1246 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/resources/base.py
--rw-r--r--   0        0        0     5391 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/task.py
--rw-r--r--   0        0        0     1001 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    21366 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     4935 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1648 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32204 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0     1022 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/core/workflows/__init__.py
--rw-r--r--   0        0        0     9332 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/core/workflows/base.py
--rw-r--r--   0        0        0      530 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1431 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     1886 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1827 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    14200 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4659 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     5802 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12101 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4311 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1480 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    16693 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     3083 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5845 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    13914 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     7155 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0    12818 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/rpcs.py
--rw-r--r--   0        0        0      666 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10744 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4794 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8232 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/parsers.py
--rw-r--r--   0        0        0     2571 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     9473 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    15316 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5496 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1667 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6797 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    17900 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0      169 2023-05-18 22:23:26.599025 caikit-0.4.4/code-of-conduct.md
--rw-r--r--   0        0        0       68 2023-05-18 22:23:26.599025 caikit-0.4.4/docs-requirements.txt
--rw-r--r--   0        0        0      634 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/Makefile
--rw-r--r--   0        0        0     1610 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/adrs/010-data-model-definition.md
--rw-r--r--   0        0        0     2352 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/adrs/015-runtime-service-generation.md
--rw-r--r--   0        0        0     2581 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/adrs/018-shared-backends.md
--rw-r--r--   0        0        0     1223 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/adrs/019-loader-stack.md
--rw-r--r--   0        0        0      404 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/architecture_club/README.md
--rw-r--r--   0        0        0     2660 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/conf.py
--rw-r--r--   0        0        0      225 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/make.bat
--rw-r--r--   0        0        0      837 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     6095 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/README.md
--rw-r--r--   0        0        0     1425 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/client.py
--rw-r--r--   0        0        0      671 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/models/text_sentiment/config.yml
--rw-r--r--   0        0        0       72 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/requirements.txt
--rw-r--r--   0        0        0      961 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/start_runtime.py
--rw-r--r--   0        0        0      816 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/text_sentiment/__init__.py
--rw-r--r--   0        0        0      742 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/text_sentiment/config.yml
--rw-r--r--   0        0        0      661 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/text_sentiment/data_model/__init__.py
--rw-r--r--   0        0        0     1422 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/text_sentiment/data_model/classification.py
--rw-r--r--   0        0        0      643 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
--rw-r--r--   0        0        0     3061 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py
--rw-r--r--   0        0        0     1157 2023-05-18 22:23:30.587056 caikit-0.4.4/pyproject.toml
--rwxr-xr-x   0        0        0      639 2023-05-18 22:23:26.599025 caikit-0.4.4/scripts/check_deps.sh
--rwxr-xr-x   0        0        0      720 2023-05-18 22:23:26.599025 caikit-0.4.4/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-05-18 22:23:26.599025 caikit-0.4.4/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/__init__.py
--rw-r--r--   0        0        0     3572 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/base.py
--rw-r--r--   0        0        0        0 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/config/__init__.py
--rw-r--r--   0        0        0     5358 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/config/test_configs.py
--rw-r--r--   0        0        0     9171 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/blocks/__init__.py
--rw-r--r--   0        0        0    11661 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/blocks/test_base.py
--rw-r--r--   0        0        0        0 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     5033 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26454 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    16232 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    18410 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     5083 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/test_enums.py
--rw-r--r--   0        0        0     1104 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     4291 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/helpers.py
--rw-r--r--   0        0        0     2320 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0      521 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_imports.py
--rw-r--r--   0        0        0    21985 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_model_manager.py
--rw-r--r--   0        0        0    13348 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_module.py
--rw-r--r--   0        0        0     6950 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_module_backend_config.py
--rw-r--r--   0        0        0     8080 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_module_metadata.py
--rw-r--r--   0        0        0     3773 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_module_type.py
--rw-r--r--   0        0        0     1038 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     2456 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_task.py
--rw-r--r--   0        0        0     7967 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    18396 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4972 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/workflows/__init__.py
--rw-r--r--   0        0        0    14622 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/core/workflows/test_base.py
--rw-r--r--   0        0        0     6782 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      647 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      154 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/control_chars.jsonl
--rw-r--r--   0        0        0      106 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0     1016 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block.zip
--rw-r--r--   0        0        0      671 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block/data.pkl
--rw-r--r--   0        0        0      189 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block_backend/config.yml
--rw-r--r--   0        0        0      177 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block_foo/config.yml
--rw-r--r--   0        0        0      506 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block_no_nesting.zip
--rw-r--r--   0        0        0      566 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block_singleton/data.json
--rw-r--r--   0        0        0       14 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block_singleton/data.pkl
--rw-r--r--   0        0        0      222 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0      717 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_resource.zip
--rw-r--r--   0        0        0      230 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     1991 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_workflow.zip
--rw-r--r--   0        0        0      497 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_workflow/config.yml
--rw-r--r--   0        0        0      541 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_workflow/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_workflow/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_workflow/dummy_block/data.pkl
--rw-r--r--   0        0        0     3033 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      355 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      359 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      359 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_block/config.yml
--rw-r--r--   0        0        0      337 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      114 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/__init__.py
--rw-r--r--   0        0        0       88 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/other_task/__init__.py
--rw-r--r--   0        0        0     1875 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
--rw-r--r--   0        0        0      199 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
--rw-r--r--   0        0        0      646 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
--rw-r--r--   0        0        0     2456 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1306 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2713 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      410 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      157 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0        0 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/resources/__init__.py
--rw-r--r--   0        0        0       58 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/resources/sample_type/__init__.py
--rw-r--r--   0        0        0       74 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/workflows/__init__.py
--rw-r--r--   0        0        0       58 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
--rw-r--r--   0        0        0     1717 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
--rw-r--r--   0        0        0        0 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3843 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14146 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    10454 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    17908 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5303 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0     5398 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     8668 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0     3768 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18431 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     4065 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/test_primitives.py
--rw-r--r--   0        0        0     1716 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/test_rpcs.py
--rw-r--r--   0        0        0     1372 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     7848 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    15426 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3640 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7372 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4204 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    30097 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0    11070 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26122 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2758 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     2115 2023-05-18 22:23:26.607025 caikit-0.4.4/tox.ini
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 caikit-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-05-22 21:25:00.861991 caikit-0.5.0/.coveragerc
+-rw-r--r--   0        0        0      676 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1272 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1328 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      261 2023-05-22 21:25:00.861991 caikit-0.5.0/.gitignore
+-rw-r--r--   0        0        0      324 2023-05-22 21:25:00.861991 caikit-0.5.0/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-05-22 21:25:00.861991 caikit-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-05-22 21:25:00.861991 caikit-0.5.0/.prettierignore
+-rw-r--r--   0        0        0       12 2023-05-22 21:25:00.861991 caikit-0.5.0/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-05-22 21:25:00.861991 caikit-0.5.0/.pylintrc
+-rw-r--r--   0        0        0       78 2023-05-22 21:25:00.861991 caikit-0.5.0/.whitesource
+-rw-r--r--   0        0        0      368 2023-05-22 21:25:00.861991 caikit-0.5.0/CODEOWNERS
+-rw-r--r--   0        0        0     7165 2023-05-22 21:25:00.861991 caikit-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-05-22 21:25:00.861991 caikit-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3626 2023-05-22 21:25:00.861991 caikit-0.5.0/README.md
+-rw-r--r--   0        0        0      152 2023-05-22 21:25:00.861991 caikit-0.5.0/SECURITY.md
+-rw-r--r--   0        0        0    44878 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit-overview.png
+-rw-r--r--   0        0        0      427 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/config/__init__.py
+-rw-r--r--   0        0        0     6052 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/config/config.py
+-rw-r--r--   0        0        0     6488 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/config/config.yml
+-rw-r--r--   0        0        0     1615 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0     1027 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    35512 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2207 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     4050 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    14380 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     4858 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     1564 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40212 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    21296 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/model_manager.py
+-rw-r--r--   0        0        0      684 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2834 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     4718 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     2802 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     6002 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/module_backends/module_backend_config.py
+-rw-r--r--   0        0        0      742 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/__init__.py
+-rw-r--r--   0        0        0    30065 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/base.py
+-rw-r--r--   0        0        0     6247 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/config.py
+-rw-r--r--   0        0        0    10859 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/decorator.py
+-rw-r--r--   0        0        0     4151 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/loader.py
+-rw-r--r--   0        0        0     6013 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/meta.py
+-rw-r--r--   0        0        0    13024 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/saver.py
+-rw-r--r--   0        0        0     3895 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/registries.py
+-rw-r--r--   0        0        0     5358 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/task.py
+-rw-r--r--   0        0        0     1001 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    21366 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1648 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32206 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0      530 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     1886 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1827 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    14200 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    16502 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4659 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     5802 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12101 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4311 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1480 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    16699 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     3043 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/core_module_helpers.py
+-rw-r--r--   0        0        0     5838 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    13914 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     7155 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/primitives.py
+-rw-r--r--   0        0        0    12800 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/rpcs.py
+-rw-r--r--   0        0        0      666 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10747 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4794 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8225 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     2571 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     9476 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    15326 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5539 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1667 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6810 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    17892 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0      169 2023-05-22 21:25:00.869980 caikit-0.5.0/code-of-conduct.md
+-rw-r--r--   0        0        0       68 2023-05-22 21:25:00.869980 caikit-0.5.0/docs-requirements.txt
+-rw-r--r--   0        0        0      634 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0     1610 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/adrs/010-data-model-definition.md
+-rw-r--r--   0        0        0     2352 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/adrs/015-runtime-service-generation.md
+-rw-r--r--   0        0        0     2581 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/adrs/018-shared-backends.md
+-rw-r--r--   0        0        0     1223 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/adrs/019-loader-stack.md
+-rw-r--r--   0        0        0      404 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/architecture_club/README.md
+-rw-r--r--   0        0        0     2660 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0      225 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/make.bat
+-rw-r--r--   0        0        0      837 2023-05-22 21:25:00.869980 caikit-0.5.0/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     6095 2023-05-22 21:25:00.869980 caikit-0.5.0/examples/text-sentiment/README.md
+-rw-r--r--   0        0        0     1425 2023-05-22 21:25:00.869980 caikit-0.5.0/examples/text-sentiment/client.py
+-rw-r--r--   0        0        0      673 2023-05-22 21:25:00.869980 caikit-0.5.0/examples/text-sentiment/models/text_sentiment/config.yml
+-rw-r--r--   0        0        0       72 2023-05-22 21:25:00.869980 caikit-0.5.0/examples/text-sentiment/requirements.txt
+-rw-r--r--   0        0        0      961 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/start_runtime.py
+-rw-r--r--   0        0        0      816 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/text_sentiment/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/text_sentiment/config.yml
+-rw-r--r--   0        0        0      661 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/text_sentiment/data_model/__init__.py
+-rw-r--r--   0        0        0     1422 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/text_sentiment/data_model/classification.py
+-rw-r--r--   0        0        0      645 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
+-rw-r--r--   0        0        0     3067 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
+-rw-r--r--   0        0        0     1179 2023-05-22 21:25:04.013929 caikit-0.5.0/pyproject.toml
+-rwxr-xr-x   0        0        0      639 2023-05-22 21:25:00.873974 caikit-0.5.0/scripts/check_deps.sh
+-rwxr-xr-x   0        0        0      720 2023-05-22 21:25:00.873974 caikit-0.5.0/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-05-22 21:25:00.873974 caikit-0.5.0/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     3439 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/base.py
+-rw-r--r--   0        0        0        0 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/config/__init__.py
+-rw-r--r--   0        0        0     5358 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/config/test_configs.py
+-rw-r--r--   0        0        0     8956 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0        0 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     5033 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26459 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    16232 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    19538 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     5083 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/test_enums.py
+-rw-r--r--   0        0        0     1104 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     4357 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2320 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0     6922 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/module_backends/test_module_backend_config.py
+-rw-r--r--   0        0        0        0 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/modules/__init__.py
+-rw-r--r--   0        0        0    12293 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/modules/test_module.py
+-rw-r--r--   0        0        0     6274 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/modules/test_module_metadata.py
+-rw-r--r--   0        0        0      521 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/test_imports.py
+-rw-r--r--   0        0        0    21421 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0     1038 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     2460 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/test_task.py
+-rw-r--r--   0        0        0     7967 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    18396 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4997 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0     6782 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      647 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      154 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/control_chars.jsonl
+-rw-r--r--   0        0        0      106 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0      222 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0     1016 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module.zip
+-rw-r--r--   0        0        0      675 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module/config.yml
+-rw-r--r--   0        0        0      299 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module/data.json
+-rw-r--r--   0        0        0       14 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module/data.pkl
+-rw-r--r--   0        0        0      191 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module_backend/config.yml
+-rw-r--r--   0        0        0      179 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module_foo/config.yml
+-rw-r--r--   0        0        0      506 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module_no_nesting.zip
+-rw-r--r--   0        0        0      570 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module_singleton/data.pkl
+-rw-r--r--   0        0        0      230 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     3034 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      376 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      360 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      364 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      422 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     2080 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_pb2.py
+-rw-r--r--   0        0        0     2447 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2217 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
+-rw-r--r--   0        0        0     2602 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
+-rw-r--r--   0        0        0     5995 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0      416 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protos/caikit_runtime.proto
+-rw-r--r--   0        0        0      437 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/protos/caikit_runtime_train.proto
+-rw-r--r--   0        0        0       24 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      294 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      410 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      157 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0      156 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/__init__.py
+-rw-r--r--   0        0        0       89 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/other_task/__init__.py
+-rw-r--r--   0        0        0     1882 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
+-rw-r--r--   0        0        0      250 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/__init__.py
+-rw-r--r--   0        0        0     1720 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
+-rw-r--r--   0        0        0      651 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
+-rw-r--r--   0        0        0     2463 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1312 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2720 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      364 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_module/config.yml
+-rw-r--r--   0        0        0        0 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3845 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14141 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    10266 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    17911 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5303 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     5398 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8706 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0     3349 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18431 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     4065 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/test_primitives.py
+-rw-r--r--   0        0        0     1721 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/test_rpcs.py
+-rw-r--r--   0        0        0     1376 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     7859 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    15481 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     3640 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7372 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4204 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    30156 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0    11106 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26269 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2758 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3355 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     2115 2023-05-22 21:25:00.877969 caikit-0.5.0/tox.ini
+-rw-r--r--   0        0        0     4768 1970-01-01 00:00:00.000000 caikit-0.5.0/PKG-INFO
```

### Comparing `caikit-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.5.0/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/.github/workflows/build-library.yml` & `caikit-0.5.0/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/.github/workflows/lint-code.yml` & `caikit-0.5.0/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/.github/workflows/publish-library.yml` & `caikit-0.5.0/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/.pylintrc` & `caikit-0.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/CONTRIBUTING.md` & `caikit-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/LICENSE` & `caikit-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/README.md` & `caikit-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit-overview.png` & `caikit-0.5.0/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/config/__init__.py` & `caikit-0.5.0/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/config/config.py` & `caikit-0.5.0/caikit/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/config/config.yml` & `caikit-0.5.0/caikit/config/config.yml`

 * *Files 3% similar despite different names*

```diff
@@ -94,16 +94,14 @@
     server_shutdown_grace_period_seconds: 45
 
     compiled_proto_module_dir: unused
 
     # Configuration items for service generation
     service_generation:
         enabled: true
-        module_types:
-            included: ["blocks", "workflows"]
         module_guids:
             included: []
             excluded: []
         primitive_data_model_types: []
         task_types:
             included: []
             excluded: []
@@ -115,15 +113,15 @@
     # `collect_delay_s` value as a float number of seconds >= 0. This will indicate
     # the amount of time the batch should wait for more requests before running a
     # partial batch.
     batching:
         default:
             size: 0
             collect_delay_s: 0.0
-        fake_batch_block:
+        fake_batch_module:
             size: 10
 
     metering:
         # Switch off metering by default
         enabled: false
         # Directory to save metrics files
         log_dir: "metering_logs"
@@ -167,15 +165,15 @@
             categories_esa: 2.95
             concepts_alchemy: 13
             entities_alchemy-disambig: 13.76
             entity-mentions_bilstm: 1.44
             entity-mentions_rbr: 1.8
             sentiment_cnn: 2.73
             syntax_izumo: 43000
-            fake_block: 2
+            fake_module: 2
 
 ### Libraries configuration
 libraries:
     sample_lib:
         # Version override for dev running
         version: 1.2.3
         # Module path override if nested
```

### Comparing `caikit-0.4.4/caikit/core/__init__.py` & `caikit-0.5.0/caikit/core/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,25 +26,20 @@
 # Standard
 # We're filtering (most) warnings for now
 import warnings as _warnings
 
 _warnings.filterwarnings("ignore")
 
 # Local
-from . import blocks, data_model, module, module_config, resources, toolkit, workflows
-from .blocks.base import BlockBase, block
 from .data_model import DataObjectBase, dataobject
 from .model_manager import *
-from .module import *
-from .module_backend_config import configure as backend_configure
 from .module_backends import *
-from .module_config import ModuleConfig
-from .resources.base import ResourceBase, resource
+from .module_backends.module_backend_config import configure as backend_configure
+from .modules import ModuleBase, ModuleConfig, module
 from .task import TaskBase, task
 from .toolkit import *
-from .workflows.base import WorkflowBase, workflow
 
 # Configure the global model wrangling functions
 MODEL_MANAGER = ModelManager()
 extract = MODEL_MANAGER.extract
 load = MODEL_MANAGER.load
 resolve_and_load = MODEL_MANAGER.resolve_and_load
```

### Comparing `caikit-0.4.4/caikit/core/augmentors/__init__.py` & `caikit-0.5.0/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/augmentors/base.py` & `caikit-0.5.0/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.5.0/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.5.0/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/augmentors/schemes/base.py` & `caikit-0.5.0/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.5.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.5.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/blocks/__init__.py` & `caikit-0.5.0/caikit/interfaces/common/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,20 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-"""The `blocks` within the `caikit.core` library are essentially the conduits of algorithms.
-Each block follows sets of principles about how they work including `.__init__()`, `.load()`,
-`.run()`, `.save()`, and `.train()`. Blocks often require each other as inputs and support many
-models.
+"""This library defines the taxonomy of Data Model objects that are domain
+agnostic and should serve as utilities for other domains
 """
 
-#################
-## Core Blocks ##
-#################
-
 # Local
-from .base import BlockSaver, block
+from . import data_model
```

### Comparing `caikit-0.4.4/caikit/core/data_model/__init__.py` & `caikit-0.5.0/caikit/core/data_model/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Common data model containing all data structures that are passed in and out of blocks.
+"""Common data model containing all data structures that are passed in and out of modules.
 """
 
 # Local
 from . import base, data_backends, enums, producer, protobufs
 from .base import DataBase
 from .dataobject import (
     CAIKIT_DATA_MODEL,
```

### Comparing `caikit-0.4.4/caikit/core/data_model/base.py` & `caikit-0.5.0/caikit/core/data_model/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.5.0/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/data_model/data_backends/base.py` & `caikit-0.5.0/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.5.0/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/data_model/dataobject.py` & `caikit-0.5.0/caikit/core/data_model/dataobject.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 
 # Standard
 from enum import Enum
 from typing import Any, Callable, List, Type, Union, get_args, get_origin
 import dataclasses
 
 # Third Party
+from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal.enum_type_wrapper import EnumTypeWrapper
+import numpy as np
 
 # First Party
-from py_to_proto.dataclass_to_proto import DataclassConverter
+from py_to_proto.dataclass_to_proto import PY_TO_PROTO_TYPES, DataclassConverter
 import alog
 import py_to_proto
 
 # Local
 from ..toolkit.errors import error_handler
 from . import enums
 from .base import DataBase, _DataBaseMetaClass
@@ -200,16 +202,27 @@
     """
     for proto_class in _AUTO_GEN_PROTO_CLASSES:
         proto_class.write_proto_file(interfaces_dir)
 
 
 ## Implementation Details ######################################################
 
+DATAOBJECT_PY_TO_PROTO_TYPES = {
+    np.int32: _descriptor.FieldDescriptor.TYPE_INT32,
+    np.int64: _descriptor.FieldDescriptor.TYPE_INT64,
+    np.uint32: _descriptor.FieldDescriptor.TYPE_UINT32,
+    np.uint64: _descriptor.FieldDescriptor.TYPE_UINT64,
+    np.float32: _descriptor.FieldDescriptor.TYPE_FLOAT,
+    np.float64: _descriptor.FieldDescriptor.TYPE_DOUBLE,
+    **PY_TO_PROTO_TYPES,
+}
+
 
 def _dataobject_to_proto(*args, **kwargs):
+    kwargs.setdefault("type_mapping", DATAOBJECT_PY_TO_PROTO_TYPES)
     return _DataobjectConverter(*args, **kwargs).descriptor
 
 
 class _DataobjectConverter(DataclassConverter):
     """Augment the dataclass converter to be able to pull descriptors from
     existing data objects
     """
```

### Comparing `caikit-0.4.4/caikit/core/data_model/enums.py` & `caikit-0.5.0/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/data_model/producer.py` & `caikit-0.5.0/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.5.0/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/data_model/streams/__init__.py` & `caikit-0.5.0/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/data_model/streams/converter.py` & `caikit-0.5.0/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.5.0/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/data_model/streams/data_stream.py` & `caikit-0.5.0/caikit/core/data_model/streams/data_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Data streams for lazily loading, munging and passing data through multiple blocks or workflows.
+"""Data streams for lazily loading, munging and passing data through multiple modules.
 """
 
 # Standard
 from collections.abc import Iterable
 from glob import glob
 from typing import Dict, Generic, List, Tuple, TypeVar, Union
 import collections
@@ -51,15 +51,15 @@
 class DataStream(Generic[T]):
     """A data stream is a iterable container class that is reentrant in the sense that it can be
     iterated over multiple times.  The items produced by a data stream may be any python object
     and are called data items.  The data items produced by an iterator over a data stream are
     generated lazily (unless the `.eager` method is called) so that each data item in a series of
     data streams is produced as it is accessed.  This allows processing datasets that are too large
     to fit into memory.  A number of functional style methods are provided for manipulating and
-    munging data streams and the `.stream` method on blocks and workflows can also be used to
+    munging data streams and the `.stream` method on modules can also be used to
     process data streams.
 
     The `DataStream` class is really just a generic wrapper around functions that produce python
     iterators or generators.
     """
 
     def __init__(self, generator_func, *args, **kwargs):
@@ -82,15 +82,15 @@
                 These arguments are generally useful for passing arguments to an initial data loader
                 function (see `.from_csv` for an example).  In order to retain other variables in a
                 `generator_func` consider relying on closures instead of arguments.
 
         Notes:
             The constructor of `DataStream` is not usually invoked directly.  The typical use case
             is to construct a data stream using one of the `.from_` class methods or else from the
-            `.stream` method of a block or workflow or by extending the `DataStream` class.
+            `.stream` method of a module or by extending the `DataStream` class.
 
             Lexical closures, generators and iterators are all important to understand when writing
             a new `generator_func`.  Consider reviewing these topics before writing custom generator
             functions.
         """
         if not callable(generator_func):
             error(
```

### Comparing `caikit-0.4.4/caikit/core/data_model/streams/resolver.py` & `caikit-0.5.0/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/data_model/streams/validator.py` & `caikit-0.5.0/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/model_manager.py` & `caikit-0.5.0/caikit/core/model_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,45 +26,40 @@
 import tempfile
 import zipfile
 
 # First Party
 import alog
 
 # Local
-from . import module_backend_config
-from .module import (
-    _MODULE_TYPES,
-    MODULE_BACKEND_REGISTRY,
-    MODULE_REGISTRY,
-    ModuleBase,
-    ModuleConfig,
-)
-from .module_backends import backend_types
+from .module_backends import backend_types, module_backend_config
 from .module_backends.base import SharedLoadBackendBase
-from .module_type import SUPPORTED_LOAD_BACKENDS_VAR_NAME
+from .modules.base import ModuleBase
+from .modules.config import ModuleConfig
+from .modules.decorator import SUPPORTED_LOAD_BACKENDS_VAR_NAME
+from .registries import module_backend_registry, module_registry
 from .toolkit.errors import error_handler
 from caikit.config import get_config
 
 log = alog.use_channel("MDLMNG")
 error = error_handler.get(log)
 
 # restrict functions that are imported so we don't pollute the base module namespace
 __all__ = [
     "get_valid_module_ids",
     "ModelManager",
 ]
 
 
 def get_valid_module_ids():
-    """Get a dictionary mapping all module (block and workflow) IDs to the
-    string names of the implementing classes.
+    """Get a dictionary mapping all module IDs to the string names of the
+    implementing classes.
     """
     return {
         module_id: model_class.__name__
-        for module_id, model_class in MODULE_REGISTRY.items()
+        for module_id, model_class in module_registry().items()
     }
 
 
 class ModelManager:
     """Manage the models or resources for library."""
 
     def __init__(self):
@@ -90,15 +85,15 @@
                     4. A bytes object corresponding to a zip archive containing either a yaml
                        config file in the top level when extracted, or a directory containing a
                        yaml config file in the top level.
             load_singleton: bool (Defaults to False)
                 Indicates whether this model should be loaded as a singleton.
 
         Returns:
-            subclass of blocks.base.BlockBase
+            subclass of caikit.core.modules.ModuleBase
                 Model object that is loaded, configured, and ready for prediction.
         """
         error.type_check("<COR98255724E>", bool, load_singleton=load_singleton)
 
         # This allows a user to load their own model (e.g. model saved to disk)
         load_path = get_config().load_path
         if load_path is not None and isinstance(module_path, str):
@@ -135,15 +130,15 @@
             module_path:  str
                 Path to directory. At the top level of directory is `config.yml` which holds info
                 about the model.
             load_singleton: bool
                 Indicates whether this model should be loaded as a singleton.
 
         Returns:
-            subclass of blocks.base.BlockBase
+            subclass of caikit.core.modules.ModuleBase
                 Model object that is loaded, configured, and ready for prediction.
         """
         # Short-circuit the loading process if the path does not exist
         if not os.path.exists(module_path):
             raise FileNotFoundError(
                 errno.ENOENT, os.strerror(errno.ENOENT), module_path
             )
@@ -151,15 +146,15 @@
         # If this is a singleton load, the entire body of this function needs to
         # be locked to avoid concurrent loads on the same model. Otherwise, we
         # can freely load in parallel.
         with self.singleton_lock(load_singleton):
 
             # Using the module_path as a key, look for an instance preloaded in the
             # singleton cache if desired
-            # 🌶🌶🌶 This doesn't work for nested blocks
+            # 🌶🌶🌶 This doesn't work for nested modules
             # TODO: think about bringing back the `unique_hash` or `tracking_id`
             if singleton_entry := (
                 load_singleton and self.singleton_module_cache.get(module_path)
             ):
                 log.debug("Found %s in the singleton cache", module_path)
                 return singleton_entry
 
@@ -220,15 +215,15 @@
                 # model's module that works with this backend
                 else:
                     # If this is the first time parsing the module config, do so
                     if module_id is None:
                         log.debug2("Loading ModuleConfig from %s", module_path)
                         module_config = ModuleConfig.load(module_path)
                         module_id = module_config.module_id
-                        module_implementations = MODULE_BACKEND_REGISTRY.get(
+                        module_implementations = module_backend_registry().get(
                             module_id, {}
                         )
                         log.debug2(
                             "Number of available backend implementations for %s found: %d",
                             module_id,
                             len(module_implementations),
                         )
@@ -263,14 +258,15 @@
                             module_id,
                             load_backend.backend_type,
                             module_backend_impl.__name__,
                         )
                         loaded_model = module_backend_impl.load(
                             module_path,
                             *args,
+                            load_backend=load_backend,
                             **kwargs,
                         )
                         if loaded_model is not None:
                             log.debug2(
                                 "Successfully loaded %s with backend %s",
                                 module_path,
                                 load_backend.backend_type,
@@ -301,15 +297,15 @@
             module_path:  str
                 Path to directory. At the top level of directory is `config.yml` which holds info
                 about the model.
             load_singleton: bool
                 Indicates whether this model should be loaded as a singleton.
 
         Returns:
-            subclass of blocks.base.BlockBase
+            subclass of caikit.core.modules.ModuleBase
                 Model object that is loaded, configured, and ready for prediction.
         """
         with tempfile.TemporaryDirectory() as extract_path:
             with zipfile.ZipFile(module_path, "r") as zip_f:
                 zip_f.extractall(extract_path)
             # Depending on the way the zip archive is packaged, out temp directory may unpack
             # to files directly, or it may unpack to a (single) directory containing the files.
@@ -390,22 +386,22 @@
         return model_path
 
     def resolve_and_load(
         self, path_or_name_or_model_reference: Union[str, ModuleBase], **kwargs
     ):
         """Try our best to load a model, given a path or a name. Simply returns any loaded model
         passed in. This exists to ease the burden on workflow developers who need to accept
-        individual blocks in their API, where users may have references to custom models or may only
-        have the ability to give the name of a stock model.
+        individual modules in their API, where users may have references to custom models or may
+        only have the ability to give the name of a stock model.
 
         Args:
             path_or_name_or_model_reference (str, ModuleBase): Either a
                 - Path to a model on disk
                 - Name of a model that the catalog knows about
-                - Loaded module (e.g. block or workflow)
+                - Loaded module
             **kwargs: Any keyword arguments to pass along to ModelManager.load()
                       or ModelManager.download()
                 e.g. parent_dir
 
         Returns:
             A loaded module
 
@@ -489,27 +485,7 @@
         # Get list of backends that are supported for load
         # NOTE: since code in a module can change anytime, its support
         # for various backend might also change, in which case,
         # it would be better to keep the backend information in the model itself
         # If module_backend is None, then we will assume that this model is not loadable in
         # any other backend
         return getattr(backend_impl, SUPPORTED_LOAD_BACKENDS_VAR_NAME, [])
-
-    @classmethod
-    def get_module_class_from_config(cls, module_config):
-        """Utility function to fetch module class information
-        from ModuleConfig
-
-        Args:
-            module_config: caikit.core.module.ModuleConfig
-                Configuration for caikit.core module
-        Returns:
-            str: name of the module_class
-        """
-        module_class = ""
-        for module_type in _MODULE_TYPES:
-            module_class_name = "{}_class".format(module_type.lower())
-            if module_class_name in module_config:
-                module_class = module_config.get(module_class_name)
-                break
-
-        return module_class
```

### Comparing `caikit-0.4.4/caikit/core/module.py` & `caikit-0.5.0/caikit/core/modules/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,78 +8,50 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Shared functionality and interfaces used by *all* modules, i.e., all blocks and workflows.
+"""Shared functionality and interfaces used by *all* moduless.
 """
 
 # TODO: Review to see if the lines in this file can be reduced or
 # broken out into another file (e.g. Python sub-modules)
 # pylint: disable=too-many-lines
 
 # abstract methods may define arguments but not use them
 # pylint: disable=unused-argument
 
 # Standard
-from importlib import metadata
 from io import BytesIO
 from typing import Any, Dict, List, Union
 import collections
-import datetime
 import os
 import shutil
 import tempfile
 import time
 import types
-import uuid
 
 # First Party
 import alog
 
 # Local
-from .. import core
-from . import data_model as dm
-from .data_model import DataStream
-from .module_config import ModuleConfig
-from .module_meta import _ModuleBaseMeta
-from .toolkit import ObjectSerializer, fileio
-from .toolkit.errors import DataValidationError, error_handler
-from .toolkit.wip_decorator import TempDisableWIP, WipCategory, work_in_progress
-from caikit.config import get_config
+from ..data_model import DataBase, DataStream
+from ..toolkit import fileio
+from ..toolkit.errors import DataValidationError, error_handler
+from .meta import _ModuleBaseMeta
+from caikit import core
 
 log = alog.use_channel("MODULE")
 error = error_handler.get(log)
 
-# This file is `*` imported so we need to override what is exposed
-__all__ = [
-    "_MODULE_TYPES",
-    "MODULE_BACKEND_REGISTRY",
-    "MODULE_REGISTRY",
-    "ModuleBase",
-    "ModuleLoader",
-    "ModuleSaver",
-]
-
-# This private registry is used to define types of modules that have been
-# defined using the @module_type decorator. It is owned here along with the
-# other registries to avoid circular dependencies
-_MODULE_TYPES = []
-
-# Single base global registry of all modules
-MODULE_REGISTRY = {}
-
-# Global module backend registry dict
-MODULE_BACKEND_REGISTRY = {}
-
 
 class ModuleBase(metaclass=_ModuleBaseMeta):
-    """Abstract base class from which all Blocks and Workflows should inherit."""
+    """Abstract base class from which all modules should inherit."""
 
     def __init__(self):
         """Construct a new model."""
         # Set up an empty metadata dictionary, to be:
         # - populated with metadata from `config.yml` files on `load`, and
         # - saved back to `config.yml` files on `save`
         self._metadata = {}
@@ -87,15 +59,14 @@
         self._load_backend = None
 
     #############
     ## Utility ##
     #############
 
     @property
-    @work_in_progress(category=WipCategory.WIP)
     def metadata(self) -> Dict[str, Any]:
         """This module's metadata.
 
         Returns:
             Dict[str, Any]: A dictionary of this module's metadata
 
             TODO: Can this be a `ModuleConfig` object instead? (or aconfig.Config)?
@@ -121,15 +92,15 @@
     ###################
     ## Instantiation ##
     ###################
 
     @classmethod
     @alog.logged_function(log.debug)
     def bootstrap(cls, *args, **kwargs):
-        """Bootstrap a block. This method can be used to initialize the block
+        """Bootstrap a module. This method can be used to initialize the module
         from artifacts created outside of a particular caikit library
         """
         error(
             "<COR92634438E>",
             NotImplementedError("This is not available in this module."),
         )
 
@@ -342,15 +313,15 @@
             **kwargs:  dict
                 Will be passed to `self.run`.
 
         Returns:
             int, int, caikit.core.data_model.DataBase
                 The first return value is the total time spent in the `self.run` loop. The second
                 return value is the total number of calls to `self.run` were made.
-                The return value is the output of the block's run method
+                The return value is the output of the module's run method
 
         Notes:
             You can pass everything that should go to the run function normally using args/kwargs.
             Example: `model.timed_run("some example text", num_seconds=60)`
 
         By default it will run for greater than or equal to 120 seconds.
         """
@@ -392,26 +363,26 @@
                 Datastream to be lazily sequentially processed by the module under consideration.
             *args: Variable length argument list to be passed directly to run().
             **kwargs: Arbitrary keyword arguments to be passed directly to run().
         Returns:
             protobufs
                 A DataBase object.
         """
-        error.type_check("<COR98214589E>", dm.DataStream, data_stream=data_stream)
+        error.type_check("<COR98214589E>", DataStream, data_stream=data_stream)
         # Ensure that no args/kwargs are DataStreams, since these get passed to stream()
         run_argvals = list(args) + list(kwargs.values())
-        if any(isinstance(arg, dm.DataStream) for arg in run_argvals):
+        if any(isinstance(arg, DataStream) for arg in run_argvals):
             error(
                 "<COR28828273E>",
                 ValueError(
                     "Only one DataStream may be passed when invoking module stream()"
                 ),
             )
         # TODO: Add .run_batch() integration
-        return dm.DataStream(
+        return DataStream(
             lambda: (self.run(data_item, *args, **kwargs) for data_item in data_stream)
         )
 
     ##############
     ## Training ##
     ##############
 
@@ -436,30 +407,30 @@
             NotImplementedError("This is not available in this module."),
         )
 
     ################
     ## Evaluation ##
     ################
 
-    # will be used to evaluate blocks; defined in sub-classes
+    # will be used to evaluate modules; defined in sub-classes
     evaluation_type = None
     # first arg is "self", unfortunately; TODO: get rid of that somehow
     evaluator = None
 
     @staticmethod
     def find_label_func(*_args, **_kwargs):
-        """Function used to extract "label" from a prediction/result of a block's .run method.
+        """Function used to extract "label" from a prediction/result of a module's .run method.
         Define if you wish to have more specific evaluation metrics. Implemented in subclass.
         """
         raise NotImplementedError("Func not implemented")
 
     @staticmethod
     def find_label_data_func(*_args, **_kwargs):
         """Function used to extract data belonging to class "label" from a prediction/result
-        of a block's .run method. Define if you wish to have more specific evaluation metrics.
+        of a module's .run method. Define if you wish to have more specific evaluation metrics.
         Implemented in subclass.
         """
         raise NotImplementedError("Func not implemented")
 
     def evaluate_quality(
         self,
         dataset_path,
@@ -467,23 +438,23 @@
         preprocess_func=None,
         detailed_metrics=False,
         labels=None,
         partial_match_metrics=False,
         max_hierarchy_levels=3,
         **kwargs,
     ):
-        """Run quality evaluation for instance of block or workflow.
+        """Run quality evaluation for instance of module
 
         Args:
             dataset_path:  str
                 Path to where the input "gold set" dataset lives. Most often this is .json file.
             preprocess_func:  method
                 Function used as proxy for any preliminary steps that need to be taken to run the
                 model on the input text. This helper function ultimately leads to the input to this
-                block and may involve executing other blocks.
+                module and may involve executing other modules.
             detailed_metrics: boolean (Optional, defaults to False)
                 Only for 'keywords'. Include partial scores and scores over every text in document.
             labels:  list (Optional, defaults to None)
                 Optional list of class labels to evaluate quality on. By default evaluation is done
                 over all class labels. Using this, you can explicitly mention only a subset of
                 labels to include in the quality evaluation.
             partial_match_metrics: boolean (Optional, defaults to False)
@@ -491,19 +462,19 @@
             max_hierarchy_levels: int
                 Used in hierarchical multilabel multiclass evaluation only. The number of levels in
                 the hierarchy to run model evaluation on,
                 in addition to complete matches.
             *args, **kwargs:
                 Optional arguments which can be used by goldset/prediction set extraction.
                 keyword arguments:
-                `block_level`: str (Applicable to block_type relations)
-                    For any block that has pre processing steps in the
-                    middle of raw text and actual block input, use the input from gold standard
+                `block_level`: str
+                    For any module that has pre processing steps in the
+                    middle of raw text and actual module input, use the input from gold standard
                     labels instead of a pre-process function. Useful for measuring quality for the
-                    'block' alone (instead of the block + pre_process pipeline)
+                    'block' alone (instead of the module + pre_process pipeline)
         Returns:
             dict
                 Dictionary of results provided by the `self.evaluator.run` function, depending on
                 the associated `evaluation_type`. Reports things like precision, recall, and f1.
         """
         # 1) load dataset
         dataset = self._load_evaluation_dataset(dataset_path)
@@ -562,21 +533,21 @@
         # Throw if generators are passed - can't imagine any situation (for now) where this is
         # something that someone is doing on purpose, so we are a bit specific about this error.
         if isinstance(arg, types.GeneratorType):
             error(
                 "<COR28071103E>",
                 ValueError("Generator types are incompatible with .run_batch"),
             )
-        if isinstance(arg, dm.DataStream):
+        if isinstance(arg, DataStream):
             error(
                 "<COR75305604E>",
                 ValueError("Data streams are incompatible with .run_batch"),
             )
         if isinstance(arg, (tuple, list)):
-            return all(isinstance(obj, (str, dm.base.DataBase)) for obj in arg)
+            return all(isinstance(obj, (str, DataBase)) for obj in arg)
         return False
 
     def _validate_and_extract_batch_size(self, *args, **kwargs):
         """Check to ensure that there's at least one iterable whose length is well defined,
         i.e., no generators, and that if multiple iterable arg/kwarg values are provided,
         they are all the same length.
 
@@ -608,15 +579,15 @@
                 have been made on other expandable iterables yet.
         Returns:
             None | inferred batch size.
         """
         if self._is_expandable_iterable(val):
             iter_batch_size = len(val)
             # Set the batch size if it's not set already. Raise if we have conflicting iterator
-            # sizes. This will happen if the arg of a block run call has an iterable value. In
+            # sizes. This will happen if the arg of a module run call has an iterable value. In
             # such cases, the subclass should override run_batch.
             if current_batch_size is None:
                 return iter_batch_size
             if current_batch_size != iter_batch_size:
                 err_str = "Iterables of varying length may not be passed to default batch predict."
                 error("<COR98338604E>", ValueError(err_str))
         if current_batch_size:
@@ -696,15 +667,15 @@
 
         Args:
             dataset:  object
                 In-memory version of whatever is loaded from on-disk. May be json, txt, etc.
 
         Returns:
             list
-                List of labels in the format of the block_type that is being called.
+                List of labels in the format of the module_type that is being called.
         """
         error(
             "<COR01455940E>",
             NotImplementedError("This is not available in this module."),
         )
 
     def _extract_pred_set(self, dataset, *args, preprocess_func=None, **kwargs):
@@ -712,20 +683,20 @@
 
         Args:
             dataset:  object
                 In-memory version of whatever is loaded from on-disk. May be json, txt, etc.
             preprocess_func:  method
                 Function used as proxy for any preliminary steps that need to be taken to run the
                 model on the input text. This helper function ultimately leads to the input to this
-                block and may involve executing other blocks.
+                module and may involve executing other modules.
             *args, **kwargs: dict
                 Optional keyword arguments for prediction set extraction.
         Returns:
             list
-                List of labels in the format of the block_type that is being called.
+                List of labels in the format of the module_type that is being called.
         """
         error(
             "<COR95693719E>",
             NotImplementedError("This is not available in this module."),
         )
 
     @staticmethod
@@ -778,270 +749,7 @@
     def _generate_report(report, gold_set):
         """Generate the quality report output
         Args:
             report: dict
             gold_set: list(dict)
         """
         return report
-
-
-## ModuleLoader ################################################################
-
-
-class ModuleLoader:
-    def __init__(self, model_path):
-        """Construct a new module loader.
-
-        Args:
-            model_path:  str
-                The path to the directory where the model is to be loaded from.
-        """
-        self.model_path = os.path.normpath(model_path)
-        error.dir_check("<COR43014802E>", model_path)
-        self.config = ModuleConfig.load(model_path)
-
-    def load_arg(self, arg):
-        """Extract arg value from the loaded model's config"""
-        return getattr(self.config, arg)
-
-    def load_args(self, *args):
-        """Extract values from the loaded model's config"""
-        return tuple(getattr(self.config, arg) for arg in args)
-
-
-## ModuleSaver #################################################################
-
-
-class ModuleSaver:
-    """A module saver that provides common functionality used for saving modules and also a context
-    manager that cleans up gracefully in case an error is encountered during the save process.
-    """
-
-    SAVED_KEY_NAME = "saved"
-    CREATED_KEY_NAME = "created"
-    TRACKING_KEY_NAME = "tracking_id"
-    MODULE_VERSION_KEY_NAME = "version"
-
-    def __init__(self, module: ModuleBase, model_path):
-        """Construct a new module saver.
-
-        Args:
-            module:  caikit.core.module.Module
-                The instance of the module to be saved.
-            model_path:  str
-                The absolute path to the directory where the model will be saved.  If this directory
-                does not exist, it will be created.
-        """
-        self.model_path = os.path.normpath(model_path)
-
-        # Get possibly nested caikit library path
-        module_path = module.__module__
-        lib_name_generator = (
-            k
-            for k, v in get_config().libraries.items()
-            if module_path.startswith(v.module_path)
-        )
-        try:
-            self.library_name = next(lib_name_generator)
-        except StopIteration:
-            # This assumes no nested module path by default
-            self.library_name = module_path.split(".")[0]  # tests
-
-        try:
-            self.library_version = metadata.version(self.library_name)
-        except metadata.PackageNotFoundError:
-            log.debug("<COR25991305D>", "No library version found")
-            if (
-                self.library_name in get_config().libraries
-                and "version" in get_config().libraries[self.library_name]
-            ):
-                self.library_version = get_config().libraries[self.library_name].version
-            else:
-                self.library_version = "0.0.0"
-
-        self.config = {
-            self.library_name + "_version": self.library_version,
-            self.CREATED_KEY_NAME: str(datetime.datetime.now()),
-            self.SAVED_KEY_NAME: str(datetime.datetime.now()),
-            "name": module.MODULE_NAME,
-            self.TRACKING_KEY_NAME: str(uuid.uuid4()),
-        }
-
-        # Add the sub-type specific fields
-        for subtype in _MODULE_TYPES:
-            subtype_id = getattr(module, f"{subtype}_ID", None)
-            if subtype_id is not None:
-                self.config.update(
-                    {
-                        f"{subtype.lower()}_id": subtype_id,
-                        f"{subtype.lower()}_class": getattr(module, f"{subtype}_CLASS"),
-                        "version": getattr(module, f"{subtype}_VERSION"),
-                    }
-                )
-
-        # Temp disable wip for following invocation to not log warnings for downstream
-        # usage of ModuleSaver
-        with TempDisableWIP():
-            # Get metadata back about this module and add it to the config
-            stored_config = module.metadata
-        # Sanitize some things off of the config:
-        # Remove the old `saved` timestamp:
-        stored_config.pop(self.SAVED_KEY_NAME, None)
-        # Remove any reserved keys, these will be set by the `ModuleConfig` class
-        for key in ModuleConfig.reserved_keys:
-            if key in stored_config:
-                stored_config.pop(key)
-
-        # Run some extremely silly metadata sanitization stuff to _not_ save metadata that was
-        # explicitly removed from some certain modules
-        ModuleSaver._provide_backwards_compatibility(module, stored_config)
-
-        self.config.update(stored_config)
-
-    @staticmethod
-    def _provide_backwards_compatibility(
-        module: ModuleBase, stored_config: Dict[str, Any]
-    ) -> None:
-        """Updates the stored_config in-place to remove any metadata keys that some certain
-        existing models expect to _not_ exist"""
-
-        # BERT entity mentions blocks no longer save the "type_map.json" file
-        if module.MODULE_ID == "f7e4208f-daee-4c5d-8268-b010929dd247":
-            stored_config.pop("type_map_path", None)
-
-    def add_dir(self, relative_path, base_relative_path=""):
-        """Create a directory inside the `model_path` for this saver.
-
-        Args:
-            relative_path:  str
-                A path relative to this saver's `model_path` denoting the directory to create.
-            base_relative_path:  str
-                A path, relative to this saver's `model_path`, in which `relative_path` will be
-                created.
-
-        Returns:
-            str, str
-                A tuple containing both the `relative_path` and `absolute_path` to the
-                directory created.
-
-        Examples:
-            >>> with ModelSaver('/path/to/model') as saver:
-            >>>     rel_path, abs_path = saver.add_dir('word_embeddings', 'model_data')
-            >>> print(rel_path)
-            model_data/word_embeddings
-            >>> print(abs_path)
-            /path/to/model/model_data/word_embeddings
-        """
-        base_relative_path = os.path.normpath(base_relative_path)
-        relative_path = os.path.normpath(relative_path)
-
-        relative_path = os.path.join(base_relative_path, relative_path)
-        absolute_path = os.path.join(self.model_path, relative_path)
-
-        os.makedirs(absolute_path, exist_ok=True)
-
-        return relative_path, absolute_path
-
-    def copy_file(self, file_path, relative_path=""):
-        """Copy an external file into a subdirectory of the `model_path` for this saver.
-
-        Args:
-            file_path:  str
-                Absolute path to the external file to copy.
-            relative_path:  str
-                The relative path inside of `model_path` where the file will be copied to.
-                If set to the empty string (default) then the file will be placed directly in
-                the `model_path` directory.
-
-        Returns:
-            str, str
-                A tuple containing both the `relative_path` and `absolute_path` to the copied file.
-        """
-        file_path = os.path.normpath(file_path)
-
-        if not os.path.isfile(file_path):
-            error(
-                "<COR80954473E>",
-                FileNotFoundError(
-                    "Attempted to add `{}` but is not a regular file.".format(file_path)
-                ),
-            )
-
-        filename = os.path.basename(os.path.normpath(file_path))
-
-        relative_path, absolute_path = self.add_dir(relative_path)
-
-        relative_file_path = os.path.join(relative_path, filename)
-        absolute_file_path = os.path.join(absolute_path, filename)
-
-        shutil.copyfile(file_path, absolute_file_path)
-
-        return relative_file_path, absolute_file_path
-
-    def save_object(self, obj, filename, serializer, relative_path=""):
-        """Save a Python object using the provided ObjectSerializer.
-
-        Args:
-            obj:  any
-                The Python object to save
-            filename: str
-                The filename to use for the saved object
-            serializer: ObjectSerializer
-                An ObjectSerializer instance (e.g., YAMLSerializer) that should be used to serialize
-                the object
-            relative_path:  str
-                The relative path inside of `model_path` where the object will be saved
-        """
-        if not issubclass(serializer.__class__, ObjectSerializer):
-            error(
-                "<COR85655282E>",
-                TypeError(
-                    "`{}` does not extend `ObjectSerializer`".format(
-                        serializer.__class__.__name__
-                    )
-                ),
-            )
-
-        relative_path, absolute_path = self.add_dir(relative_path)
-
-        # Normalize any '././' structure that may come from relative paths
-        relative_file_path = os.path.normpath(os.path.join(relative_path, filename))
-        absolute_file_path = os.path.normpath(os.path.join(absolute_path, filename))
-
-        serializer.serialize(obj, absolute_file_path)
-
-        return relative_file_path, absolute_file_path
-
-    def update_config(self, additional_config):
-        """Add items to this saver's config dictionary.
-
-        Args:
-            additional_config:  dict
-                A dictionary of config options to add the this saver's configuration.
-
-        Notes:
-            The behavior of this method matches `dict.update` and is equivalent to calling
-            `saver.config.update`.  The `saver.config` dictionary may be accessed directly for
-            more sophisticated manipulation of the configuration.
-        """
-        self.config.update(additional_config)
-
-    def __enter__(self):
-        """Enter the module saver context.  This creates the `model_path` directory.  If this
-        context successfully exits, then the model configuration and all files it contains will
-        be written and saved to disk inside the `model_path` directory.  If any uncaught exceptions
-        are thrown inside this context, then `model_path` will be removed.
-        """
-        os.makedirs(self.model_path, exist_ok=True)
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        """Exit the module saver context. If this context successfully exits, then the model
-        configuration and all files it contains will be written and saved to disk inside the
-        `model_path` directory.  If any uncaught exceptions are thrown inside this context, then
-        `model_path` will be removed.
-        """
-        if exc_type is not None:
-            shutil.rmtree(self.model_path, ignore_errors=True)
-            return
-
-        ModuleConfig(self.config).save(self.model_path)
```

### Comparing `caikit-0.4.4/caikit/core/module_backend_config.py` & `caikit-0.5.0/caikit/core/module_backends/module_backend_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 from typing import List
 import copy
 
 # First Party
 import alog
 
 # Local
-from .module import MODULE_BACKEND_REGISTRY
-from .module_backends.backend_types import (
-    MODULE_BACKEND_CONFIG_FUNCTIONS,
-    MODULE_BACKEND_TYPES,
+from ..registries import (
+    module_backend_classes,
+    module_backend_registry,
+    module_backend_types,
 )
-from .module_backends.base import BackendBase
-from .toolkit.errors import error_handler
+from ..toolkit.errors import error_handler
+from .base import BackendBase
 from caikit.config import get_config
 
 log = alog.use_channel("CONF")
 error = error_handler.get(log)
 
 
 def start_backends() -> None:
@@ -80,27 +80,27 @@
                 "<COR48633635E>",
                 "type" in backend_config,
                 "All backend priority configs must have a 'type' field",
             )
             backend_type = backend_config.type
             error.value_check(
                 "<COR72281596E>",
-                backend_type in MODULE_BACKEND_TYPES,
+                backend_type in module_backend_types(),
                 "Invalid backend [{}] found at backend_priority index [{}]",
                 backend_type,
                 i,
             )
 
             log.debug("Configuring backend (%d)[%s]", i, backend_type)
             backend_instance_config = backend_config.get("config", {})
             log.debug3(
                 "Backend (%d)[%s] config: %s", i, backend_type, backend_instance_config
             )
 
-            backend_class = MODULE_BACKEND_CONFIG_FUNCTIONS.get(backend_type)
+            backend_class = module_backend_classes().get(backend_type)
             error.value_check(
                 "<COR64618509E>",
                 len(registry) == i,
                 "({})[{}] already configured",
                 i,
                 backend_type,
             )
@@ -148,15 +148,15 @@
             Name of the backend to select from registry
         backend_instance: object
             Initialized backend instance. This object should
             implement the `register_config` function which will be
             used to merge / iteratively configure the backend
     """
     # Go through all the modules registered with particular backend
-    for module_id, module_type_mapping in MODULE_BACKEND_REGISTRY.items():
+    for module_id, module_type_mapping in module_backend_registry().items():
         if backend in module_type_mapping:
             # check if it contains any special config
             config = module_type_mapping[backend].backend_config_override
             error.type_check("<COR61136899E>", dict, config=config)
             if len(config) != 0:
                 # TODO: Add a check here to see if the backend has already started
                 backend_instance.register_config(config)
```

### Comparing `caikit-0.4.4/caikit/core/module_backends/__init__.py` & `caikit-0.5.0/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/module_backends/backend_types.py` & `caikit-0.5.0/caikit/core/module_backends/backend_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,48 +13,28 @@
 # limitations under the License.
 
 """
 Shared registry of known backend types
 """
 
 # Standard
-from typing import Any, Dict, Optional, Type
+from typing import Optional, Type
 
 # First Party
 import alog
 
 # Local
+from ..registries import module_backend_classes, module_backend_types
 from ..toolkit.errors import error_handler
 from ..toolkit.wip_decorator import Action, WipCategory, work_in_progress
 from .base import BackendBase
 
 log = alog.use_channel("BCKENDTYP")
 error = error_handler.get(log)
 
-## Backend Type Extensible Enum ################################################
-
-
-class _AttrAccessDict(dict):
-    """Simple extension on a dict that allows attribute access in addition to
-    index lookup
-    """
-
-    def __getattr__(self, name: str) -> Any:
-        """Alias to index lookup"""
-        error.value_check(
-            "<COR85015051E>", name in self, "backend type {} not registered", name
-        )
-        return self[name]
-
-
-# "enum" holding known backend types. This is implemented as a dict so that it
-# can be extended as needed by downstream libraries.
-MODULE_BACKEND_TYPES = _AttrAccessDict()
-MODULE_BACKEND_CONFIG_FUNCTIONS: Dict[int, Type[BackendBase]] = {}
-
 
 ## Public ######################################################################
 
 
 @work_in_progress(action=Action.WARNING, category=WipCategory.BETA)
 def register_backend_type(config_class: Optional[Type[BackendBase]] = None):
     """Register a new module backend type by name. This will perform the
@@ -87,18 +67,20 @@
         "type_name must be fully UPPERCASE: {}",
         type_name,
     )
 
     # Add to the global registries
     # NOTE: This only contains a module name and does not contain an object of the backend module
     # The object of the "configured" backend module is generated using caikit.config.configure
-    if type_name not in MODULE_BACKEND_TYPES:
-        MODULE_BACKEND_TYPES[type_name] = type_name
-        MODULE_BACKEND_CONFIG_FUNCTIONS[type_name] = config_class
+    backend_types = module_backend_types()
+    backend_classes = module_backend_classes()
+    if type_name not in backend_types:
+        backend_types[type_name] = type_name
+        backend_classes[type_name] = config_class
 
 
 def __getattr__(name):
     """This module forwards attribute access to the MODULE_BACKEND_TYPES
     mapping
     """
     if not name.startswith("_"):
-        return getattr(MODULE_BACKEND_TYPES, name)
+        return getattr(module_backend_types(), name)
```

### Comparing `caikit-0.4.4/caikit/core/module_backends/base.py` & `caikit-0.5.0/caikit/core/module_backends/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from typing import Optional, Type
 import abc
 
 # First Party
 import aconfig
 
 # Local
-from ..module import ModuleBase
+from ..modules import ModuleBase
 
 
 class BackendBase(abc.ABC):
     """Interface for creating configuration setup for backends"""
 
     def __init__(self, config: Optional[aconfig.Config] = None) -> None:
         self.config = config or {}
@@ -46,15 +46,15 @@
     def is_started(self):
         return self._started
 
     @abc.abstractmethod
     def register_config(self, config):
         """Function to allow dynamic merging of configs.
         This can be useful, if there are explicit configurations
-        particular implementations (blocks) need to register before the starting the backend.
+        particular implementations (modules) need to register before the starting the backend.
         """
         # NOTE: This function should be implemented in such a way that it can be called multiple
         # times
 
     @abc.abstractmethod
     def start(self):
         """Function to start a distributed backend. This function
```

### Comparing `caikit-0.4.4/caikit/core/module_backends/local_backend.py` & `caikit-0.5.0/caikit/core/module_backends/local_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 # Third Party
 import yaml
 
 # First Party
 import alog
 
 # Local
-from ..module import MODULE_REGISTRY, ModuleBase
-from ..module_config import ModuleConfig
+from ..modules.base import ModuleBase
+from ..modules.config import ModuleConfig
+from ..registries import module_registry
 from ..toolkit.errors import error_handler
 from .backend_types import register_backend_type
 from .base import SharedLoadBackendBase, SharedTrainBackendBase
 
 log = alog.use_channel("LCLBKND")
 error = error_handler.get(log)
 
@@ -63,15 +64,15 @@
         """Look up the given module in the module registry and load it if found"""
         try:
             model_config = ModuleConfig.load(model_path)
         except (FileNotFoundError, KeyError, yaml.parser.ParserError):
             log.debug("Unable to load local model config from [%s]", model_path)
             return None
         module_id = model_config.module_id
-        module_class = MODULE_REGISTRY.get(module_id)
+        module_class = module_registry().get(module_id)
         if module_class is not None:
             return module_class.load(model_path, *args, **kwargs)
         log.warning(
             "<COR14661026W>",
             "Could not load MODULE_ID %s with %s",
             module_id,
             self.backend_type,
```

### Comparing `caikit-0.4.4/caikit/core/module_config.py` & `caikit-0.5.0/caikit/core/modules/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,45 +10,45 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
 import os
+import warnings
 
 # First Party
 import aconfig
 import alog
 
 # Local
-from . import toolkit
-from .toolkit.errors import error_handler
+from .. import toolkit
+from ..toolkit.errors import error_handler
 
-log = alog.use_channel("MODULE")
+log = alog.use_channel("MODULE_CFG")
 error = error_handler.get(log)
 
 
 class ModuleConfig(aconfig.Config):
-    """Config object used by all blocks for config loading, saving, etc."""
+    """Config object used by all modules for config loading, saving, etc."""
 
     # keys that are not allowed at the top-level module configuration (reserved for internal use)
-    reserved_keys = "module_id", "model_path"
+    reserved_keys = ["model_path"]
 
     def __init__(self, config_dict):
         """Construct a new module configuration object from a dictionary of config options.
 
         Args:
             config_dict:  dict
                 Dictionary or containing the module's configuration.
 
         Notes:
             The following keys are reserved and *must not* be specified at the top level of a
             configuration:
 
-            module_id - reserved for storing the block or workflow id
             model_path - reserved for storing the original location where the model was loaded from
         """
         super().__init__(config_dict, override_env_vars=False)
 
         # validate that reserved configuration items are not in the config_dict
         self_keys_lower = {key.lower() for key in self.keys()}
         for reserved_key in self.reserved_keys:
@@ -57,38 +57,34 @@
                     "<COR80419305E>",
                     KeyError(
                         "Do not add `{}` as top-level key in `config.yml`. "
                         "This is for internal use only.".format(reserved_key)
                     ),
                 )
 
-        # Alias from the subtype id to module_id
-        self.module_id = None
-        # 🌶️🌶️🌶️: Delayed import here to avoid circular dependency
-        # Needs a bit more ♻️ to be less 💩
-        # pylint: disable=import-outside-toplevel,no-name-in-module
-        # Local
-        from caikit.core import _MODULE_TYPES
-
-        for subtype in _MODULE_TYPES:
-            id_field = f"{subtype.lower()}_id"
-            subtype_id_val = getattr(self, id_field, None)
-            if subtype_id_val is not None:
-                error.type_check(
-                    "<COR80419079E>",
-                    str,
-                    **{id_field: subtype_id_val},
-                )
-                self.module_id = subtype_id_val
-                break
+        # 🌶️🌶️🌶️: Backwards compatibility for old-style `blocks`, `workflows`, and `resources`
+        if not self.module_id:  # pylint: disable=access-member-before-definition
+            warnings.warn(
+                "No module_id found in config. Re-save the block to use module_id",
+                DeprecationWarning,
+            )  # actual warning or just log.warning?
+            if self.block_id:
+                log.debug("Detected legacy block_id in config")
+                self.module_id = self.block_id
+            elif self.workflow_id:
+                log.debug("Detected legacy workflow_id in config")
+                self.module_id = self.block_id
+            elif self.resource_id:
+                log.debug("Detected legacy resource_id in config")
+                self.module_id = self.resource_id
+
         error.value_check(
             "<COR80418932E>",
-            self.module_id is not None,
-            "Please specify one of {} in model config.",
-            [f"{subtype.lower()}_id" for subtype in _MODULE_TYPES],
+            hasattr(self, "module_id"),
+            "Invalid model_config, module_id must be specified.",
         )
 
     @classmethod
     def load(cls, model_path):
         """Load a new module configuration from a directory on disk.
 
         Args:
```

### Comparing `caikit-0.4.4/caikit/core/module_meta.py` & `caikit-0.5.0/caikit/core/modules/meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,17 +68,16 @@
 # Standard
 import abc
 
 # First Party
 import alog
 
 # Local
-from .module_config import ModuleConfig
-from .toolkit import wip_decorator
-from .toolkit.errors import error_handler
+from .config import ModuleConfig
+from caikit.core.toolkit.errors import error_handler
 
 log = alog.use_channel("METADATA_INJECT")
 error = error_handler.get(log)
 
 
 class _ModuleBaseMeta(abc.ABCMeta):
     """This is the metaclass used by `caikit.core.ModuleBase`.
@@ -133,20 +132,17 @@
                         args,
                         kwargs,
                     )
 
                 # Call the original .load function to load the module
                 module = real_load.__func__(clz, *args, **kwargs)
 
-                # Compatibility issue: Some deprecated `blocks` returned tuples from load
-                # Temp disable wip for following invocation to not log warnings for downstream
-                # usage of _ModuleBaseMeta
-                with wip_decorator.TempDisableWIP():
-                    if hasattr(module, "metadata") and module_config:
-                        module.metadata.update(module_config)
+                # defer any "is this really a module" logic until after the load call
+                if hasattr(module, "metadata") and module_config:
+                    module.metadata.update(module_config)
 
                 return module
 
             attrs["load"] = classmethod(metadata_injecting_load)
 
         return super().__new__(mcs, name, bases, attrs)
```

### Comparing `caikit-0.4.4/caikit/core/resources/__init__.py` & `caikit-0.5.0/examples/text-sentiment/models/text_sentiment/config.yml`

 * *Files 19% similar despite different names*

```diff
@@ -8,13 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-"""Resource Base. All implementations of resource types are imported here.
-"""
-
-# Local
-from .base import ResourceSaver, resource
+module_id: 8f72161-c0e4-49b0-8fd0-7587b3017a35
+name: HuggingFaceSentimentModule
+version: 0.0.1
```

### Comparing `caikit-0.4.4/caikit/core/task.py` & `caikit-0.5.0/caikit/core/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # Standard
 from typing import Callable, Dict, List, Type, Union
 
 # First Party
 from alog import alog
 
 # Local
-from caikit.core.data_model import DataStream
-from caikit.core.data_model.base import DataBase
-from caikit.core.toolkit.errors import error_handler
+from .data_model import DataStream
+from .data_model.base import DataBase
+from .toolkit.errors import error_handler
 
 log = alog.use_channel("TASK_BASE")
 error = error_handler.get(log)
 
 ProtoableInputTypes = Type[Union[int, float, str, bytes, bool, DataBase]]
 ValidInputTypes = Union[
     ProtoableInputTypes, List[ProtoableInputTypes], DataStream[ProtoableInputTypes]
```

### Comparing `caikit-0.4.4/caikit/core/toolkit/__init__.py` & `caikit-0.5.0/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/toolkit/compatibility.py` & `caikit-0.5.0/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/toolkit/errors/__init__.py` & `caikit-0.5.0/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.5.0/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.5.0/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/toolkit/fileio.py` & `caikit-0.5.0/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/toolkit/isa.py` & `caikit-0.5.0/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/toolkit/logging.py` & `caikit-0.5.0/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.5.0/caikit/core/toolkit/quality_evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
                 # get per-class information if possible
                 all_labels = gold_labels.union(pred_labels)
 
             except NotImplementedError:
                 # If find_label_func raises NotImplementedError, we can't do label-based matching.
                 # In this case we need to fall back to set operations on the raw data tuples.
                 log.info(
-                    "INFO: find_label_func not implemented for this block type - falling back "
+                    "INFO: find_label_func not implemented for this module type - falling back "
                     "to tuple match!!"
                 )
                 use_labels_for_matching = False
 
             for label in all_labels:
                 # dictionary initizalization
                 if label not in per_class_confusion_matrix:
@@ -396,15 +396,15 @@
             per_class_confusion_matrix
         )
 
         # This section should be deprecated with future refactors
         if not use_labels_for_matching:
             log.warning(
                 "WARNING: Only Micro_avg metrics could be calculated based on the information "
-                "available for this block type."
+                "available for this module type."
             )
             calc_metrics.micro_metrics.precision = micro_precision
             calc_metrics.micro_metrics.recall = micro_recall
             calc_metrics.micro_metrics.f1 = micro_f1
             calc_metrics.micro_metrics.true_positive = overall_tp
             calc_metrics.micro_metrics.false_positive = overall_fp
             calc_metrics.micro_metrics.false_negative = overall_fn
```

### Comparing `caikit-0.4.4/caikit/core/toolkit/serializers.py` & `caikit-0.5.0/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/toolkit/wip_decorator.py` & `caikit-0.5.0/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/core/workflows/__init__.py` & `caikit-0.5.0/examples/text-sentiment/start_runtime.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,16 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# Standard
+from os import path
+import sys
 
-"""The `workflows` within the `caikit.core` library are essentially "super blocks" -- blocks
-that call other blocks and compose an execution graph that describes how the output of one
-block feeds into another block. Each `workflow` adheres to a contract that extends the contract
-of a block, offering `.__init__()`, `.load()`, `.run()`, `.save()`, and `.train()` methods.
-"""
+# First Party
+import alog
+
+sys.path.append(
+    path.abspath(path.join(path.dirname(__file__), "../"))
+)  # Here we assume that `start_runtime` file is at the same level of the `text_sentiment` package
 
 # Local
-from .base import WorkflowLoader, WorkflowSaver, workflow
+import text_sentiment
+
+alog.configure(default_level="debug")
+
+# Local
+from caikit.runtime import grpc_server
+
+grpc_server.main()
```

### Comparing `caikit-0.4.4/caikit/interfaces/__init__.py` & `caikit-0.5.0/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/interfaces/common/__init__.py` & `caikit-0.5.0/tests/runtime/generated/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+# Standard
+import os
+import sys
 
-"""This library defines the taxonomy of Data Model objects that are domain
-agnostic and should serve as utilities for other domains
-"""
-
-# Local
-from . import data_model
+# Allow generated _pb2 files in here to import each other
+script_loc = os.path.dirname(os.path.realpath(__file__))
+sys.path.insert(0, script_loc)
```

### Comparing `caikit-0.4.4/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.5.0/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/interfaces/common/data_model/producer.py` & `caikit-0.5.0/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/interfaces/runtime/__init__.py` & `caikit-0.5.0/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.5.0/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.5.0/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/__init__.py` & `caikit-0.5.0/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/dump_services.py` & `caikit-0.5.0/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/grpc_server.py` & `caikit-0.5.0/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/interceptors/__init__.py` & `caikit-0.5.0/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.5.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/metrics/__init__.py` & `caikit-0.5.0/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.5.0/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/model_management/__init__.py` & `caikit-0.5.0/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/model_management/batcher.py` & `caikit-0.5.0/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/model_management/loaded_model.py` & `caikit-0.5.0/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/model_management/model_loader.py` & `caikit-0.5.0/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/model_management/model_manager.py` & `caikit-0.5.0/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/model_management/model_sizer.py` & `caikit-0.5.0/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/model_management/training_manager.py` & `caikit-0.5.0/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/protobufs/__init__.py` & `caikit-0.5.0/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.5.0/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.5.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.5.0/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.5.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.5.0/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.5.0/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.5.0/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.5.0/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.5.0/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/service_factory.py` & `caikit-0.5.0/caikit/runtime/service_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # First Party
 from py_to_proto.json_to_service import json_to_service
 import aconfig
 import alog
 
 # Local
 from caikit import get_config
-from caikit.core.module import ModuleBase
+from caikit.core import ModuleBase
 from caikit.interfaces.runtime.data_model import (
     TrainingInfoRequest,
     TrainingInfoResponse,
 )
 from caikit.runtime import service_generation
 from caikit.runtime.service_generation.core_module_helpers import get_module_info
 from caikit.runtime.service_generation.rpcs import snake_to_upper_camel
@@ -230,15 +230,15 @@
     @staticmethod
     def _get_and_filter_modules(
         caikit_config: aconfig.Config, lib: str
     ) -> Set[Type[ModuleBase]]:
         clean_modules = set()
         modules = [
             module_class
-            for module_class in caikit.core.MODULE_REGISTRY.values()
+            for module_class in caikit.core.registries.module_registry().values()
             if module_class.__module__.partition(".")[0] == lib
         ]
         log.debug("Found all modules %s for library %s.", modules, lib)
 
         # Check config for any explicit inclusions
         included_task_types = (
             caikit_config.runtime.service_generation
```

### Comparing `caikit-0.4.4/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.5.0/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/service_generation/core_module_helpers.py` & `caikit-0.5.0/caikit/runtime/service_generation/core_module_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,21 +31,20 @@
     kind: str
     type: str
 
 
 def get_module_info(ck_module: Type[ModuleBase]) -> Optional[ModuleInfo]:
     """Determine the name for the module type for this Caikit Core Module. This
     is defined as the name string of the parent python module above the
-    immediate parent. This is done so that Modules of type block and workflow
-    can end up in the same `module type` if they implement the same logical
-    problem.
+    immediate parent. This is done so that Modules can end up in the same `module type`
+    if they implement the same logical problem.
 
     The logic here assumes one of several conventions is followed for the Module
     1. The Module is declared in a python module named
-        `<library>.<block/workflow>.<module type>`
+        `<library>.modules.<module type>`
     2. The module derives from a base class that itself derives from one of the
         known type-hierarchy derived from `ModuleBase`.
     """
     # NOTE: all of this assumes <library> has no .
     # Use the library name to qualify the module type in case there are
     # collisions across domains (e.g. classification in nlp and cv)
     py_mod_name_parts = ck_module.__module__.split(".")
```

### Comparing `caikit-0.4.4/caikit/runtime/service_generation/create_service.py` & `caikit-0.5.0/caikit/runtime/service_generation/create_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # Local
 from ... import get_config
 from .core_module_helpers import get_module_info
 from .primitives import is_primitive_method
 from .rpcs import CaikitRPCBase, ModuleClassTrainRPC, TaskPredictRPC
 from .signature_parsing.module_signature import CaikitCoreModuleMethodSignature
-from caikit.core.module import ModuleBase
+from caikit.core import ModuleBase
 
 log = alog.use_channel("CREATE-RPCS")
 
 ## Globals #####################################################################
 
 INFERENCE_FUNCTION_NAME = "run"
 TRAIN_FUNCTION_NAME = "train"
```

### Comparing `caikit-0.4.4/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.5.0/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/service_generation/primitives.py` & `caikit-0.5.0/caikit/runtime/service_generation/primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/service_generation/rpcs.py` & `caikit-0.5.0/caikit/runtime/service_generation/rpcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 # Local
 from . import primitives, type_helpers
 from .compatibility_checker import ApiFieldNames
 from .signature_parsing.module_signature import (
     CaikitCoreModuleMethodSignature,
     CustomSignature,
 )
+from caikit.core import ModuleBase
 from caikit.core.data_model.base import DataBase
 from caikit.core.data_model.dataobject import (
     DataObjectBase,
     _DataObjectBaseMetaClass,
     dataobject,
 )
-from caikit.core.module import ModuleBase
 from caikit.interfaces.runtime.data_model import ModelPointer, TrainingJob
 from caikit.runtime.service_generation.data_stream_source import make_data_stream_source
 
 log = alog.use_channel("RPC-SERIALIZERS")
 
 INDENT = "    "
 
@@ -164,17 +164,17 @@
             f"{module_split[1]}_{module_split[2]}_{self.clz.__name__}_Train"
         )
 
     def _module_class_to_req_name(self) -> str:
         """Helper function to convert from the name of a module to the name of the
         request RPC message
 
-        Example: self.clz._module__ = sample_lib.blocks.sample_task.sample_implementation
+        Example: self.clz._module__ = sample_lib.modules.sample_task.sample_implementation
 
-        return: BlocksSampleTaskSampleBlockTrainRequest
+        return: BlocksSampleTaskSampleModuleTrainRequest
 
         """
         module_split = self.clz.__module__.split(".")
         return snake_to_upper_camel(
             f"{module_split[1]}_{module_split[2]}_{self.clz.__name__}_TrainRequest"
         )
 
@@ -269,15 +269,15 @@
 
         # Create the rpc name based on the module type
         self.name = self._task_to_rpc_name()
 
     @property
     def module_list(self) -> List[Type[ModuleBase]]:
         """Returns the list of all caikit.core.modules that this RPC will be for. These should all
-        be of the same ai-problem, e.g. my_caikit_library.[blocks | workflows].classification
+        be of the same ai-problem, e.g. my_caikit_library.modules.classification
         """
         return self._module_list
 
     @property
     def request(self) -> "_RequestMessage":
         return self._req
```

### Comparing `caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/docstrings.py` & `caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/docstrings.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 def get_return_type(fn: Callable) -> Optional[Type]:
     """
     Grabs the return type off the docstring, if possible
     Args:
         fn: The function to get the return value of
-            e.g. my_caikit_library.blocks.classification.Transformer.run
+            e.g. my_caikit_library.modules.classification.Transformer.run
 
     Returns:
         The return type of `fn`, if it can be parsed from the docstring. Otherwise, None
     """
     try:
         docstring = docstring_parser.parse(fn.__doc__)
     except Exception as exc:
@@ -65,15 +65,15 @@
     """
     Checks if the `arg_name` param from `fn`s docstring is optional
     by checking if param description starts with "an optional"
     or "optional".
 
     Args:
         fn: The function to get the type of a parameter from
-            e.g.  my_caikit_library.blocks.classification.Transformer.run
+            e.g.  my_caikit_library.modules.classification.Transformer.run
         arg_name: The name of the parameter that we should try to get the type of
             e.g. "raw_document"
     """
     try:
         docstring = docstring_parser.parse(fn.__doc__)
     except Exception as exc:
         raise CaikitRuntimeException(
@@ -100,15 +100,15 @@
 
 
 def get_arg_type(fn: Callable, arg_name: str) -> Optional[Type]:
     """
     Grabs the type of the `arg_name` param from `fn`s docstring, if possible
     Args:
         fn: The function to get the type of a parameter from
-            e.g. my_caikit_library.blocks.classification.Transformer.run
+            e.g. my_caikit_library.modules.classification.Transformer.run
         arg_name: The name of the parameter that we should try to get the type of
             e.g. "raw_document"
     Returns:
         The return type of `fn`, if it can be parsed from the docstring. Otherwise, None
     """
 
     try:
```

### Comparing `caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/module_signature.py` & `caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/parsers.py` & `caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 import inspect
 
 # First Party
 import alog
 
 # Local
 from . import docstrings
+from caikit.core import ModuleBase
 from caikit.core.data_model.base import DataBase
-from caikit.core.module import ModuleBase
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 
 log = alog.use_channel("SIG-PARSING")
 
 # Constants ##################################
 KNOWN_ARG_TYPES = {
     "producer_id": "ProducerId",
```

### Comparing `caikit-0.4.4/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.5.0/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/servicers/__init__.py` & `caikit-0.5.0/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.5.0/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             "Constructed inference service for library: %s, version: %s",
             library,
             lib_version,
         )
         super()
 
     def Predict(self, request, context):
-        """Global predict RPC -- Mocks the invocation of a Caikit Library block.run()
+        """Global predict RPC -- Mocks the invocation of a Caikit Library module.run()
         method for a loaded Caikit Library model
 
         Args:
             request(object):
                 A deserialized RPC request message
             context(grpc.ServicerContext): Context object (contains request metadata, etc)
 
@@ -144,23 +144,23 @@
             with alog.ContextLog(log.debug, outer_scope_name):
                 # Make sure the request has a model before doing anything
                 model_id = get_metadata(context, self.MODEL_MESH_MODEL_ID_KEY)
                 # Retrieve the model from the model manager
                 log.debug("<RUN52259029D>", "Retrieving model '%s'", model_id)
                 model = self._model_manager.retrieve_model(model_id)
 
-                # Unmarshall the request object into the required block run argument(s)
+                # Unmarshall the request object into the required module run argument(s)
                 with PREDICT_FROM_PROTO_SUMMARY.labels(
                     grpc_request=desc_name, model_id=model_id
                 ).time():
                     caikit_library_request = build_caikit_library_request_dict(
                         request, model.run
                     )
 
-                # NB: we previously recorded the size of the request, and timed this block to
+                # NB: we previously recorded the size of the request, and timed this module to
                 # provide a rudimentary throughput metric of size / time
                 with alog.ContextLog(log.debug, inner_scope_name):
                     with PREDICT_CAIKIT_LIBRARY_SUMMARY.labels(
                         grpc_request=desc_name, model_id=model_id
                     ).time():
                         if self.use_abortable_threads:
                             work = AbortableAction(
```

### Comparing `caikit-0.4.4/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.5.0/caikit/runtime/servicers/global_train_servicer.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import grpc
 
 # First Party
 import alog
 
 # Local
 from caikit import get_config
-from caikit.core.module import ModuleBase
+from caikit.core import ModuleBase
 from caikit.interfaces.runtime.data_model import TrainingJob
 from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.model_management.training_manager import TrainingManager
 from caikit.runtime.service_factory import ServicePackage
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils.import_util import clean_lib_names, get_data_model
 from caikit.runtime.utils.servicer_util import (
@@ -95,44 +95,44 @@
             "Constructed train service for library: %s, version: %s",
             self.library,
             lib_version,
         )
         super()
 
     def Train(self, request, *_, **__) -> TrainingJob:
-        """Global predict RPC -- Mocks the invocation of a Caikit Library block.train()
+        """Global predict RPC -- Mocks the invocation of a Caikit Library module.train()
         method for a loaded Caikit Library model
         Args:
             request(object):
                 A deserialized RPC request message
             context(grpc.ServicerContext): Context object (contains request metadata, etc)
         Returns:
             caikit.interfaces.runtime.data_model.TrainingJob:
                 A TrainingJob data model response object
         """
         desc_name = request.DESCRIPTOR.name
         outer_scope_name = "GlobalTrainServicer.Train:%s" % desc_name
 
         try:
             with alog.ContextLog(log.debug, outer_scope_name):
-                # BlocksSampleTaskSampleBlockTrainRequest
-                # getattr(importlib.import_module("sample_lib.blocks.sample_task"), "SampleBlock")
+                # BlocksSampleTaskSampleModuleTrainRequest
+                # getattr(importlib.import_module("sample_lib.modules.sample_task"), "SampleModule")
                 # TODO: fixme - temporary workaround for now
                 desc_name = desc_name.replace("TrainRequest", "")
                 split = re.split("(?<=.)(?=[A-Z])", desc_name)
                 model = None
                 try:
                     model = getattr(
                         importlib.import_module(
                             f"{self.library}.{split[0].lower()}.{split[1].lower()}"
                         ),
                         f"{''.join(split[2:])}",
                     )
                 except Exception:  # pylint: disable=broad-exception-caught
-                    for mod in caikit.core.MODULE_REGISTRY.values():
+                    for mod in caikit.core.registries.module_registry().values():
                         module_split = mod.__module__.split(".")
                         train_request_for_mod = snake_to_upper_camel(
                             f"{module_split[1]}_{module_split[2]}_{mod.__name__}"
                         )
                         if train_request_for_mod == desc_name:
                             model = mod
                             break
```

### Comparing `caikit-0.4.4/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.5.0/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.5.0/caikit/runtime/servicers/model_train_servicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,17 @@
         log.info("<RUN02584562I>", "Calling ModelTrainServicer.Run!")
         log.debug("<RUN91039903D>", "ProcessRequest: %s", request)
 
         try:
             request_dict = request.request_dict
 
             # get the model to train
-            train_module = caikit.core.MODULE_REGISTRY.get(request_dict["train_module"])
+            train_module = caikit.core.registries.module_registry().get(
+                request_dict["train_module"]
+            )
             log.debug("<RUN76043064D>", "train_module: %s", train_module)
             if train_module is None:
                 raise CaikitRuntimeException(
                     grpc.StatusCode.INVALID_ARGUMENT,
                     "Model Train not able to parse module for this Train Request",
                 )
```

### Comparing `caikit-0.4.4/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.5.0/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/types/__init__.py` & `caikit-0.5.0/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/types/aborted_exception.py` & `caikit-0.5.0/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.5.0/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.5.0/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/utils/__init__.py` & `caikit-0.5.0/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/utils/import_util.py` & `caikit-0.5.0/caikit/runtime/utils/import_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 def get_data_model(config: aconfig.Config = None) -> UnifiedDataModel:
     """
     Get the data model from the Caikit library of interest. This is accomplished
     via dynamic import on the caikit_library's environment variable.
 
     NOTE: This function also has the side-effect of importing each of the
         caikit_library libraries for the first time, causing their modules to
-        be registered with the caikit.core MODULE_REGISTRY. It is a critical
+        be registered with the caikit.core module registry. It is a critical
         step in initializing the set of modules that can be loaded by this
         running server instance.
 
     Args:
         config(aconfig.Config): caikit configuration
 
     Returns:
@@ -104,15 +104,15 @@
         cdm = _get_cdm_from_lib(lib_name, cdm)
 
     # Check module registry to get base modules
     # NOTE: Following is done after previous for-loop, since we need to import
     # all the libraries which will register all the modules and that happens
     # in get_dynamic_module above
     base_lib_names = set()
-    for module_class in caikit.core.MODULE_REGISTRY.values():
+    for module_class in caikit.core.registries.module_registry().values():
         lib_name = module_class.__module__.partition(".")[0]
         if lib_name not in lib_names:
             # This module is from a library not mentioned
             # in lib_names. Consider this as a base library, like caikit.core
             base_lib_names.add(lib_name)
 
     # Get data model from lib_names
```

### Comparing `caikit-0.4.4/caikit/runtime/utils/servicer_util.py` & `caikit-0.5.0/caikit/runtime/utils/servicer_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
                     field.type,
                 )
 
         # Now we do something similar for the output RPC message, verifying
         # that we can construct an object of the Caikit Library CDM that matches
         # the specified field type, and that said Caikit Library object has a
         # to_proto method defined. No need to check for proto primitives here since
-        # all Caikit library blocks/workflows should return well formed "predict" messages
+        # all Caikit library modules should return well formed "predict" messages
         # from the data model.
         output_class = method.output_type.name
         caikit_Library_class = validate_caikit_library_class_exists(cdm, output_class)
         validate_caikit_library_class_method_exists(caikit_Library_class, "to_proto")
 
 
 def build_caikit_library_request_dict(
@@ -371,15 +371,15 @@
                             caikit_library_class = getattr(cdm, class_name)
                             # Use the Caikit Library CDM class's from_proto
                             # method to turn our protobufs field message into an
                             # instance of the Caikit Library CDM class
                             instance = caikit_library_class.from_proto(field_value)
                             # Add to the request dictionary, using the message
                             # field's name as the key (since, by convention, the
-                            # argument name to the block run function will be
+                            # argument name to the module run function will be
                             # the same as the field name)
                             caikit_library_request_dict[field.name] = instance
 
         log.debug2(
             "caikit_library_request_dict returned is: %s", caikit_library_request_dict
         )
```

### Comparing `caikit-0.4.4/caikit/runtime/work_management/__init__.py` & `caikit-0.5.0/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/work_management/abortable_action.py` & `caikit-0.5.0/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/work_management/call_aborter.py` & `caikit-0.5.0/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.5.0/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/docs/Makefile` & `caikit-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/docs/adrs/010-data-model-definition.md` & `caikit-0.5.0/docs/adrs/010-data-model-definition.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/docs/adrs/015-runtime-service-generation.md` & `caikit-0.5.0/docs/adrs/015-runtime-service-generation.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/docs/adrs/018-shared-backends.md` & `caikit-0.5.0/docs/adrs/018-shared-backends.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/docs/adrs/019-loader-stack.md` & `caikit-0.5.0/docs/adrs/019-loader-stack.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/docs/architecture_club/04-25-23.md` & `caikit-0.5.0/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/docs/conf.py` & `caikit-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/docs/make.bat` & `caikit-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/examples/start_runtime_with_sample_lib.py` & `caikit-0.5.0/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/examples/text-sentiment/README.md` & `caikit-0.5.0/examples/text-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/examples/text-sentiment/client.py` & `caikit-0.5.0/examples/text-sentiment/client.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/examples/text-sentiment/models/text_sentiment/config.yml` & `caikit-0.5.0/examples/text-sentiment/text_sentiment/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,10 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-block_id: 8f72161-c0e4-49b0-8fd0-7587b3017a35
-name: HuggingFaceSentimentBlock
-version: 0.0.1
+# Standard
+import os
+
+# Local
+from . import data_model, runtime_model
+import caikit
+
+# Give the path to the `config.yml`
+CONFIG_PATH = os.path.realpath(os.path.join(os.path.dirname(__file__), "config.yml"))
+
+caikit.configure(CONFIG_PATH)
```

### Comparing `caikit-0.4.4/examples/text-sentiment/start_runtime.py` & `caikit-0.5.0/tests/core/test_no_write_permissions.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,28 +7,22 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""RQA has a build that does not get write permissions, so a whole bunch of things can fail
 
+We want to make sure that at least `import caikit.core` does not barf, which it will if we aren't
+careful
+"""
 # Standard
-from os import path
-import sys
+from unittest.mock import patch
 
-# First Party
-import alog
+with patch("os.makedirs") as makedirs:
+    makedirs.side_effect = PermissionError("No files for you")
 
-sys.path.append(
-    path.abspath(path.join(path.dirname(__file__), "../"))
-)  # Here we assume that `start_runtime` file is at the same level of the `text_sentiment` package
-
-# Local
-import text_sentiment
-
-alog.configure(default_level="debug")
-
-# Local
-from caikit.runtime import grpc_server
-
-grpc_server.main()
+    # Make sure importing does not fail
+    # pylint: disable=unused-import
+    # Local
+    import caikit.core
```

### Comparing `caikit-0.4.4/examples/text-sentiment/text_sentiment/__init__.py` & `caikit-0.5.0/examples/text-sentiment/text_sentiment/config.yml`

 * *Files 18% similar despite different names*

```diff
@@ -8,18 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# Standard
-import os
-
-# Local
-from . import data_model, runtime_model
-import caikit
-
-# Give the path to the `config.yml`
-CONFIG_PATH = os.path.realpath(os.path.join(os.path.dirname(__file__), "config.yml"))
-
-caikit.configure(CONFIG_PATH)
+runtime:
+    library: text_sentiment
+    service_generation:
+        primitive_data_model_types:
+            - "text_sentiment.data_model.classification.TextInput"
```

### Comparing `caikit-0.4.4/examples/text-sentiment/text_sentiment/config.yml` & `caikit-0.5.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,13 +7,10 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-runtime:
-    library: text_sentiment
-    service_generation:
-        primitive_data_model_types:
-            - "text_sentiment.data_model.classification.TextInput"
+# # Local
+# Local
+from .hf_module import HuggingFaceSentimentModule
```

### Comparing `caikit-0.4.4/examples/text-sentiment/text_sentiment/data_model/__init__.py` & `caikit-0.5.0/examples/text-sentiment/text_sentiment/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/examples/text-sentiment/text_sentiment/data_model/classification.py` & `caikit-0.5.0/examples/text-sentiment/text_sentiment/data_model/classification.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/examples/text-sentiment/text_sentiment/runtime_model/__init__.py` & `caikit-0.5.0/tests/runtime/metrics/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,10 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# # Local
-# Local
-from .hf_block import HuggingFaceSentimentBlock
```

### Comparing `caikit-0.4.4/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py` & `caikit-0.5.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 # Standard
 import os
 
 # Third Party
 from transformers import pipeline
 
 # Local
-from caikit.core import BlockBase, ModuleLoader, ModuleSaver, block
+from caikit.core import ModuleBase, ModuleLoader, ModuleSaver, module
 from text_sentiment.data_model.classification import (
     ClassificationPrediction,
     ClassInfo,
     TextInput,
 )
 
 
-@block("8f72161-c0e4-49b0-8fd0-7587b3017a35", "HuggingFaceSentimentBlock", "0.0.1")
-class HuggingFaceSentimentBlock(BlockBase):
+@module("8f72161-c0e4-49b0-8fd0-7587b3017a35", "HuggingFaceSentimentModule", "0.0.1")
+class HuggingFaceSentimentModule(ModuleBase):
     """Class to wrap sentiment analysis pipeline from HuggingFace"""
 
     def __init__(self, model_path) -> None:
         super().__init__()
         loader = ModuleLoader(model_path)
         config = loader.config
         model = pipeline(model=config.hf_artifact_path, task="sentiment-analysis")
```

### Comparing `caikit-0.4.4/pyproject.toml` & `caikit-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.4.4"
+version = "0.5.0"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
@@ -17,22 +17,23 @@
     "alchemy-config>=1.1.1,<2.0.0",
     "alchemy-logging>=1.0.4,<2.0.0",
     "anytree>=2.7.0,<3.0",
     "docstring-parser>=0.14.1,<0.16.0",
     "grpcio-health-checking>=1.35.0,<2.0",
     "grpcio>=1.35.0,<2.0",
     "ijson>=3.1.4,<3.3.0",
+    "import-tracker>=3.1.5,<4",
     "munch>=2.5.0,<4.0",
-    "protobuf>=3.19.0,<5",
+    "numpy>=1.20,<2",
     "prometheus_client>=0.12.0,<1.0",
+    "protobuf>=3.19.0,<5",
     "py-grpc-prometheus>=0.7.0,<0.8",
+    "py-to-proto>=0.2.0,<0.3.0",
     "PyYAML>=6.0,<7.0",
     "requests>=2.26.0,<3.0",
     "semver>=2.13.0,<4.0",
     "six>=1.16.0,<2.0.0",
     "tqdm>=4.59.0,<5.0.0",
-    "py-to-proto>=0.2.0,<0.3.0",
-    "import-tracker>=3.1.5,<4",
 ]
 
 [project.urls]
 Source = "https://github.com/caikit/caikit"
```

### Comparing `caikit-0.4.4/scripts/check_deps.sh` & `caikit-0.5.0/scripts/check_deps.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/scripts/fmt.sh` & `caikit-0.5.0/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/__init__.py` & `caikit-0.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/base.py` & `caikit-0.5.0/tests/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,17 +25,15 @@
 
 class TestCaseBase(unittest.TestCase):
     """Parent class for all specific test classes in Caikit Core."""
 
     # common reference to the place where we put our fixtures, because a ton of tests use this
     fixtures_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "fixtures")
     # Other things that we use often
-    block_fixtures_dir = os.path.join(fixtures_dir, "blocks")
-    resource_fixtures_dir = os.path.join(fixtures_dir, "resources")
-    workflow_fixtures_dir = os.path.join(fixtures_dir, "workflows")
+    modules_fixtures_dir = os.path.join(fixtures_dir, "modules")
     toolkit_fixtures_dir = os.path.join(fixtures_dir, "toolkit")
 
     def __init__(self, *args, **kwargs):
         # initialize parent class
         super().__init__(*args, **kwargs)
 
     def _compare_seqs(self, obj_seq1, obj_seq2, properties):
```

### Comparing `caikit-0.4.4/tests/config/test_configs.py` & `caikit-0.5.0/tests/config/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/conftest.py` & `caikit-0.5.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -261,26 +261,16 @@
 
 @pytest.fixture
 def fixtures_dir():
     yield os.path.join(os.path.dirname(os.path.realpath(__file__)), "fixtures")
 
 
 @pytest.fixture
-def block_fixtures_dir(fixtures_dir):
-    yield os.path.join(fixtures_dir, "blocks")
-
-
-@pytest.fixture
-def resource_fixtures_dir(fixtures_dir):
-    yield os.path.join(fixtures_dir, "resources")
-
-
-@pytest.fixture
-def workflow_fixtures_dir(fixtures_dir):
-    yield os.path.join(fixtures_dir, "workflows")
+def modules_fixtures_dir(fixtures_dir):
+    yield os.path.join(fixtures_dir, "modules")
 
 
 @pytest.fixture
 def toolkit_fixtures_dir(fixtures_dir):
     yield os.path.join(fixtures_dir, "toolkit")
```

### Comparing `caikit-0.4.4/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.5.0/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.5.0/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/blocks/__init__.py` & `caikit-0.5.0/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.5.0/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/data_model/streams/test_converter.py` & `caikit-0.5.0/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.5.0/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.5.0/tests/core/data_model/streams/test_data_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 # Standard
 import os
 
 # Local
 from caikit.core import data_model as core_dm
 from caikit.core.augmentors import AugmentorBase
-from sample_lib.blocks.sample_task.sample_implementation import SampleBlock
 from sample_lib.data_model.sample import SampleInputType, SampleOutputType
+from sample_lib.modules.sample_task.sample_implementation import SampleModule
 
 # Unit Test Infrastructure
 from tests.base import TestCaseBase
 import caikit.core
 
 
 def build_test_augmentor(produces_none):
@@ -493,37 +493,37 @@
             self.assertEqual(data_item, count * 2 + 1)
 
     def test_dummy_stream(self):
         """Verify that we can use streams to generate dummy predictions."""
         text_stream = self.csv_data_stream[0]
         self.validate_data_stream(text_stream, 3, str)
 
-        dummy_model = caikit.core.load(os.path.join(self.fixtures_dir, "dummy_block"))
+        dummy_model = caikit.core.load(os.path.join(self.fixtures_dir, "dummy_module"))
         # Map to data stream of SampleInputType for model
         sample_type_data_stream = text_stream.map(
             lambda text: SampleInputType(name=text)
         )
         dummy_stream = dummy_model.stream(sample_type_data_stream)
         self.validate_data_stream(dummy_stream, 3, SampleOutputType)
 
     def test_only_one_stream_allowed(self):  # , mock_run):
         """Verify that we can't call module.stream() with multiple DataStream args."""
         text_stream = self.csv_data_stream[0]
         self.validate_data_stream(text_stream, 3, str)
 
-        dummy_model = caikit.core.load(os.path.join(self.fixtures_dir, "dummy_block"))
+        dummy_model = caikit.core.load(os.path.join(self.fixtures_dir, "dummy_module"))
         with self.assertRaises(ValueError):
             # NOTE: Even though this is too many args for .run() to handle, it's okay; this
             # will fail before it gets to .run(). In the event that .run() is called with the
             # wrong number of positional arguments, it'll throw a TypeError, which fails this test.
             dummy_model.stream(text_stream, text_stream)
 
     def test_pipe_stream(self):
         """Verify that we can use streams to generate dummy predictions using `|` syntax."""
-        dummy_model = caikit.core.load(os.path.join(self.fixtures_dir, "dummy_block"))
+        dummy_model = caikit.core.load(os.path.join(self.fixtures_dir, "dummy_module"))
 
         dummy_stream = self.sample_type_data_stream | dummy_model
         self.validate_data_stream(dummy_stream, 7, SampleOutputType)
 
     ### generic file loader tests
 
     def test_from_file_can_handle_a_json_file(self):
```

### Comparing `caikit-0.4.4/tests/core/data_model/streams/test_resolver.py` & `caikit-0.5.0/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/data_model/streams/test_validator.py` & `caikit-0.5.0/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/data_model/test_base.py` & `caikit-0.5.0/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/data_model/test_dataobject.py` & `caikit-0.5.0/tests/core/data_model/test_dataobject.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 from typing import List, Optional, Union
 import copy
 import json
 import os
 import tempfile
 
 # Third Party
+from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool, message
+import numpy as np
 import pytest
 
 # First Party
 from py_to_proto.dataclass_to_proto import Annotated, FieldNumber, OneofField
 
 # Local
 from caikit.core import (  # NOTE: Imported from the top to validate
@@ -646,7 +648,46 @@
     assert json.loads(inst.to_json())["foo"] == FooEnum.FOO.name
 
     # Create an instance with an integer value
     inst = Foo(foo=FooEnum.FOO.value)
     assert inst.to_proto().foo == FooEnum.FOO.value
     assert inst.to_dict()["foo"] == FooEnum.FOO.name
     assert json.loads(inst.to_json())["foo"] == FooEnum.FOO.name
+
+
+def test_np_dtypes():
+    """Make sure that numpy dtype types can be used in dataobjects"""
+
+    @dataobject
+    class Foo(DataObjectBase):
+        int32: np.int32
+        int64: np.int64
+        uint32: np.uint32
+        uint64: np.uint64
+        float32: np.float32
+        float64: np.float64
+
+    descriptor = Foo._proto_class.DESCRIPTOR
+    assert (
+        descriptor.fields_by_name["int32"].type
+        == _descriptor.FieldDescriptor.TYPE_INT32
+    )
+    assert (
+        descriptor.fields_by_name["int64"].type
+        == _descriptor.FieldDescriptor.TYPE_INT64
+    )
+    assert (
+        descriptor.fields_by_name["uint32"].type
+        == _descriptor.FieldDescriptor.TYPE_UINT32
+    )
+    assert (
+        descriptor.fields_by_name["uint64"].type
+        == _descriptor.FieldDescriptor.TYPE_UINT64
+    )
+    assert (
+        descriptor.fields_by_name["float32"].type
+        == _descriptor.FieldDescriptor.TYPE_FLOAT
+    )
+    assert (
+        descriptor.fields_by_name["float64"].type
+        == _descriptor.FieldDescriptor.TYPE_DOUBLE
+    )
```

### Comparing `caikit-0.4.4/tests/core/data_model/test_enums.py` & `caikit-0.5.0/tests/core/data_model/test_enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/data_model/test_producer.py` & `caikit-0.5.0/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/helpers.py` & `caikit-0.5.0/tests/core/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,24 +17,30 @@
 import copy
 
 # Third Party
 import pytest
 
 # Local
 from caikit.core import LocalBackend
-from caikit.core.module import MODULE_BACKEND_REGISTRY, MODULE_REGISTRY, ModuleBase
-from caikit.core.module_backend_config import (
-    _CONFIGURED_LOAD_BACKENDS,
-    _CONFIGURED_TRAIN_BACKENDS,
-)
 from caikit.core.module_backends import BackendBase, backend_types
 
 # Add mock backend
 # This is set in the base test config's load_priority list
 from caikit.core.module_backends.base import SharedLoadBackendBase
+from caikit.core.module_backends.module_backend_config import (
+    _CONFIGURED_LOAD_BACKENDS,
+    _CONFIGURED_TRAIN_BACKENDS,
+)
+from caikit.core.modules.base import ModuleBase
+from caikit.core.registries import (
+    module_backend_classes,
+    module_backend_registry,
+    module_backend_types,
+    module_registry,
+)
 
 
 class MockBackend(BackendBase):
     backend_type = "MOCK"
 
     def __init__(self, config=...) -> None:
         super().__init__(config)
@@ -79,43 +85,41 @@
 
 backend_types.register_backend_type(TestLoader)
 
 
 @pytest.fixture
 def reset_backend_types():
     """Fixture that will reset the backend types if a test modifies them"""
-    base_backend_types = {
-        key: val for key, val in backend_types.MODULE_BACKEND_TYPES.items()
-    }
-    base_backend_fns = {
-        key: val for key, val in backend_types.MODULE_BACKEND_CONFIG_FUNCTIONS.items()
-    }
+    base_backend_types = {key: val for key, val in module_backend_types().items()}
+    base_backend_classes = {key: val for key, val in module_backend_classes().items()}
     yield
-    backend_types.MODULE_BACKEND_TYPES.clear()
-    backend_types.MODULE_BACKEND_TYPES.update(base_backend_types)
-    backend_types.MODULE_BACKEND_CONFIG_FUNCTIONS.clear()
-    backend_types.MODULE_BACKEND_CONFIG_FUNCTIONS.update(base_backend_fns)
+    module_backend_types().clear()
+    module_backend_types().update(base_backend_types)
+    module_backend_classes().clear()
+    module_backend_classes().update(base_backend_classes)
 
 
 @pytest.fixture
 def reset_module_backend_registry():
     """Fixture that will reset the module distribution registry if a test modifies them"""
-    module_registry = {key: val for key, val in MODULE_BACKEND_REGISTRY.items()}
+    orig_module_backend_registry = {
+        key: val for key, val in module_backend_registry().items()
+    }
     yield
-    MODULE_BACKEND_REGISTRY.clear()
-    MODULE_BACKEND_REGISTRY.update(module_registry)
+    module_backend_registry().clear()
+    module_backend_registry().update(orig_module_backend_registry)
 
 
 @pytest.fixture
 def reset_module_registry():
     """Fixture that will reset caikit.core module registry if a test modifies it"""
-    module_registry = {key: val for key, val in MODULE_REGISTRY.items()}
+    orig_module_registry = {key: val for key, val in module_registry().items()}
     yield
-    MODULE_REGISTRY.clear()
-    MODULE_REGISTRY.update(module_registry)
+    module_registry().clear()
+    module_registry().update(orig_module_registry)
 
 
 @pytest.fixture
 def reset_configured_backends():
     """Fixture that will reset the configured backends"""
     load_backends_list = copy.copy(_CONFIGURED_LOAD_BACKENDS)
     train_backends_list = copy.copy(_CONFIGURED_TRAIN_BACKENDS)
```

### Comparing `caikit-0.4.4/tests/core/module_backends/test_backend_types.py` & `caikit-0.5.0/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/test_imports.py` & `caikit-0.5.0/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/test_model_manager.py` & `caikit-0.5.0/tests/core/test_model_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,30 @@
 # limitations under the License.
 """Tests for the model manager, which corrals catalogs to resolve models from names,
 and download and load them.
 """
 
 # Standard
 from contextlib import contextmanager
+from unittest import mock
+from unittest.mock import MagicMock
 import os
 import tempfile
 import uuid
 
 # Local
-from caikit.core.module_backend_config import configure, configured_load_backends
-from caikit.core.module_backends import LocalBackend
-from caikit.core.module_backends.base import SharedLoadBackendBase
+from caikit.core.module_backends import module_backend_config
+from caikit.core.module_backends.module_backend_config import (
+    configure,
+    configured_load_backends,
+)
+from sample_lib.data_model import SampleTask
 
 # Unit Test Infrastructure
-from sample_lib.blocks.sample_task import SampleBlock
-from sample_lib.data_model import SampleTask
+from sample_lib.modules.sample_task import SampleModule
 from tests.base import TestCaseBase
 from tests.conftest import temp_config
 
 # NOTE: We do need to import `reset_backend_types` and `reset_module_distribution_registry` for `reset_globals` to work
 from tests.core.helpers import *
 import caikit.core
 
@@ -41,55 +45,47 @@
     """This test class tries to mock out the catalogs and direct download calls to reduce network
     overhead.
     """
 
     @classmethod
     def setUpClass(cls) -> None:
         # Test fixtures that can be directly loaded
-        cls.model_path = os.path.join(cls.fixtures_dir, "dummy_block")
+        cls.model_path = os.path.join(cls.fixtures_dir, "dummy_module")
         # This model has no unique hash set in its config; we use it as a nonsingleton model too
         cls.non_singleton_model_path = cls.model_path
         cls.singleton_model_path = os.path.join(
-            cls.fixtures_dir, "dummy_block_singleton"
+            cls.fixtures_dir, "dummy_module_singleton"
         )
 
         cls.resource_path = os.path.join(cls.fixtures_dir, "dummy_resource")
 
         # Binary buffers of zip archives, for mocking downloads
-        cls.block_zip_path = os.path.join(cls.fixtures_dir, "dummy_block.zip")
-        with open(cls.block_zip_path, "rb") as f:
-            cls.block_archive_buffer = f.read()
-
-        zipfile = os.path.join(cls.fixtures_dir, "dummy_workflow.zip")
-        with open(zipfile, "rb") as f:
-            cls.workflow_archive_buffer = f.read()
-
-        zipfile = os.path.join(cls.fixtures_dir, "dummy_resource.zip")
-        with open(zipfile, "rb") as f:
-            cls.resource_archive_buffer = f.read()
+        cls.module_zip_path = os.path.join(cls.fixtures_dir, "dummy_module.zip")
+        with open(cls.module_zip_path, "rb") as f:
+            cls.module_archive_buffer = f.read()
 
     @pytest.fixture
     def global_load_path(self):
         """Set load_path prior to importing caikit.core."""
         # Set test load path
         test_load_path = os.path.join(self.fixtures_dir, "models")
 
         with temp_config({"load_path": test_load_path}):
             yield
 
-    def test_load_can_return_a_block(self):
+    def test_load_can_return_a_module(self):
         model = caikit.core.load(self.model_path)
-        self.assertIsInstance(model, caikit.core.BlockBase)
+        self.assertIsInstance(model, caikit.core.ModuleBase)
 
-    def test_load_can_load_a_block_as_a_singleton(self):
+    def test_load_can_load_a_module_as_a_singleton(self):
         model1 = caikit.core.load(self.singleton_model_path, load_singleton=True)
         model2 = caikit.core.load(self.singleton_model_path, load_singleton=True)
         assert model1 is model2
 
-    def test_load_can_load_a_block_with_singleton_disabled(self):
+    def test_load_can_load_a_module_with_singleton_disabled(self):
         model1 = caikit.core.load(self.singleton_model_path, load_singleton=True)
         model2 = caikit.core.load(self.singleton_model_path, load_singleton=False)
         assert model1 is not model2
 
     def test_singleton_cache_can_be_cleared(self):
         model = caikit.core.load(self.singleton_model_path, load_singleton=True)
         self.assertGreater(
@@ -108,15 +104,15 @@
     def test_load_raises_on_bad_paths(self):
         with self.assertRaises(FileNotFoundError):
             caikit.core.load("bad/path/to/model")
 
     def test_extract(self):
         with tempfile.TemporaryDirectory() as tempdir:
             extract_path = caikit.core.extract(
-                self.block_zip_path, tempdir, force_overwrite=True
+                self.module_zip_path, tempdir, force_overwrite=True
             )
             self.assertEqual(extract_path, tempdir)
             self.assertTrue(os.path.isdir(extract_path))
             # load shouldn't barf
             caikit.core.load(extract_path)
 
     def test_resolve_and_load_can_load_a_model_from_a_path(self):
@@ -137,116 +133,106 @@
         with self.assertRaises(TypeError):
             caikit.core.resolve_and_load(["test", "not", "a", "module"])
         with self.assertRaises(TypeError):
             caikit.core.resolve_and_load({"this dict is": "not a module"})
 
     def test_load_model_with_artifacts_from_zip_str(self):
         """Test that we can load a model archive [extracts to temp_dir/...] with artifacts."""
-        model = caikit.core.load(self.block_zip_path)
-        self.assertIsInstance(model, caikit.core.BlockBase)
+        model = caikit.core.load(self.module_zip_path)
+        self.assertIsInstance(model, caikit.core.ModuleBase)
 
     def test_load_model_with_artifacts_from_bytes(self):
         """Test that we can load a bytes object as a model, even if it has artifacts."""
-        model_bytes = caikit.core.load(self.block_zip_path).as_bytes()
+        model_bytes = caikit.core.load(self.module_zip_path).as_bytes()
         model = caikit.core.load(model_bytes)
-        self.assertIsInstance(model, caikit.core.BlockBase)
+        self.assertIsInstance(model, caikit.core.ModuleBase)
 
     def test_load_model_with_artifacts_from_file_like(self):
         """Test that we can load a file-like object as a model, even if it has artifacts."""
-        model_bytesio = caikit.core.load(self.block_zip_path).as_file_like_object()
+        model_bytesio = caikit.core.load(self.module_zip_path).as_file_like_object()
         model = caikit.core.load(model_bytesio)
-        self.assertIsInstance(model, caikit.core.BlockBase)
+        self.assertIsInstance(model, caikit.core.ModuleBase)
 
     def test_load_model_with_no_nesting(self):
         """Test that we can load a zip even if it unzips directly into the extraction archive."""
-        model_path = os.path.join(self.fixtures_dir, "dummy_block_no_nesting.zip")
+        model_path = os.path.join(self.fixtures_dir, "dummy_module_no_nesting.zip")
         model = caikit.core.load(model_path)
-        self.assertIsInstance(model, caikit.core.BlockBase)
+        self.assertIsInstance(model, caikit.core.ModuleBase)
 
     def test_load_invalid_zip_file(self):
         """Test that loading a zip archive not containing a model fails gracefully."""
         model_path = os.path.join(self.fixtures_dir, "invalid.zip")
         with self.assertRaises(FileNotFoundError):
             caikit.core.load(model_path)
 
     @pytest.mark.usefixtures("global_load_path")
     def test_load_path(self):
         """Test that loading a model from a path defined in the load_path config variable works."""
         model = caikit.core.load("foo")
-        self.assertIsInstance(model, caikit.core.BlockBase)
-
-    def test_import_block_registry(self):
-        """Make sure that the BLOCK_REGISTRY can be imported from model_manager"""
-        # pylint: disable = import-outside-toplevel,no-name-in-module,unused-import
-        from caikit.core.model_manager import BLOCK_REGISTRY  # isort: skip
-
-    def test_import_workflow_registry(self):
-        """Make sure that the WORKFLOW_REGISTRY can be imported from model_manager"""
-        # pylint: disable = import-outside-toplevel,no-name-in-module,unused-import
-        from caikit.core.model_manager import WORKFLOW_REGISTRY  # isort: skip
+        self.assertIsInstance(model, caikit.core.ModuleBase)
 
-    def test_import_resource_registry(self):
-        """Make sure that the RESOURCE_REGISTRY can be imported from model_manager"""
+    def test_import_module_registry(self):
+        """Make sure that the module registry can be imported from model_manager"""
         # pylint: disable = import-outside-toplevel,no-name-in-module,unused-import
-        from caikit.core.model_manager import RESOURCE_REGISTRY  # isort: skip
+        from caikit.core.model_manager import module_registry  # isort: skip
 
 
 # Pytest tests #########################################################
 
 # Setup #########################################################################
 
 DUMMY_MODULE_ID = "foo"
 
 TEST_DATA_PATH = os.path.join("tests", "fixtures")
-DUMMY_LOCAL_MODEL_NAME = "dummy_block_foo"
-DUMMY_BACKEND_MODEL_NAME = "dummy_block_backend"
+DUMMY_LOCAL_MODEL_NAME = "dummy_module_foo"
+DUMMY_BACKEND_MODEL_NAME = "dummy_module_backend"
 CONFIG_FILE_NAME = "config.yml"
 
 
 def setup_saved_model(mock_backend_class):
     """Fixture to create and cleanup a dummy loadable model"""
 
     backend_types.register_backend_type(LocalBackend)
 
-    @caikit.core.blocks.block(
+    @caikit.core.modules.module(
         id=DUMMY_MODULE_ID, name="dummy base", version="0.0.1", task=SampleTask
     )
-    class DummyFoo(caikit.core.blocks.base.BlockBase):
+    class DummyFoo(caikit.core.ModuleBase):
         @classmethod
         def load(cls, *args, **kwargs):
             return cls()
 
     # Register backend type
     backend_types.register_backend_type(mock_backend_class)
 
-    @caikit.core.blocks.block(base_module=DummyFoo, backend_type=backend_types.MOCK)
-    class DummyBar(caikit.core.blocks.base.BlockBase):
+    @caikit.core.modules.module(base_module=DummyFoo, backend_type=backend_types.MOCK)
+    class DummyBar(caikit.core.ModuleBase):
         SUPPORTED_LOAD_BACKENDS = [backend_types.MOCK, backend_types.LOCAL]
 
         @classmethod
         def load(self, *args, **kwargs):
             return DummyBar()
 
     return DummyFoo, DummyBar
 
 
-@caikit.core.blocks.block(
+@caikit.core.modules.module(
     id="non-distributed", name="non distributed mod", version="0.0.1", task=SampleTask
 )
-class NonDistributedBlock(caikit.core.blocks.base.BlockBase):
+class NonDistributedModule(caikit.core.ModuleBase):
     @classmethod
     def load(cls, *args, **kwargs):
         return cls()
 
     def save(self, model_path):
-        block_saver = caikit.core.blocks.BlockSaver(
+        module_saver = caikit.core.modules.ModuleSaver(
             self,
             model_path=model_path,
         )
-        with block_saver:
+        with module_saver:
             pass
 
 
 @contextmanager
 def temp_saved_model(model):
     """Temporarily save the model and yield its path"""
     with tempfile.TemporaryDirectory() as model_path:
@@ -369,40 +355,22 @@
 
         dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_LOCAL_MODEL_NAME)
         _ = caikit.core.load(dummy_model_path, load_singleton=True)
 
         assert len(caikit.core.MODEL_MANAGER.get_singleton_model_cache_info()) == 2
 
 
-def test_get_module_class():
-    """Test to verify get_module_class function can return appropriate module class"""
-    # Block
-    config = {"block_id": "foo", "block_class": "Foo"}
-    module_config = caikit.core.module.ModuleConfig(config)
-    assert caikit.core.ModelManager.get_module_class_from_config(module_config) == "Foo"
-
-    # Workflow
-    config = {"workflow_id": "foo", "workflow_class": "Foo"}
-    module_config = caikit.core.module.ModuleConfig(config)
-    assert caikit.core.ModelManager.get_module_class_from_config(module_config) == "Foo"
-
-    # Resource
-    config = {"resource_id": "foo", "resource_class": "Foo"}
-    module_config = caikit.core.module.ModuleConfig(config)
-    assert caikit.core.ModelManager.get_module_class_from_config(module_config) == "Foo"
-
-
 def test_fall_back_to_local(reset_globals):
     """Make sure that if LOCAL is enabled and a given module doesn't have any
     registered backends, the default caikit.core.load is used.
     """
-    with temp_saved_model(NonDistributedBlock()) as model_path:
+    with temp_saved_model(NonDistributedModule()) as model_path:
         model = caikit.core.load(model_path)
 
-    assert isinstance(model, NonDistributedBlock)
+    assert isinstance(model, NonDistributedModule)
 
 
 def test_load_fails_on_no_supported_backend(reset_globals):
     """Make sure if a given module doesn't have any registered backends,
     loading fails.
     """
     _ = setup_saved_model(MockBackend)
@@ -412,15 +380,15 @@
             "module_backends": {
                 "load_priority": [{"type": backend_types.MOCK}],
                 "train_priority": [],
             },
         }
     ):
         configure()
-        with temp_saved_model(NonDistributedBlock()) as model_path:
+        with temp_saved_model(NonDistributedModule()) as model_path:
             with pytest.raises(ValueError):
                 caikit.core.load(model_path)
 
 
 def test_preferred_backend_enabled(reset_globals):
     """Make sure that for a model artifact saved with a local backend can be
     loaded with an enabled non-local backend if given as a preferred_backend.
@@ -436,14 +404,42 @@
         configure()
 
         dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_LOCAL_MODEL_NAME)
         model = caikit.core.load(dummy_model_path)
         assert isinstance(model, DummyBar)
 
 
+def test_module_backend_instance_is_passed_to_load_classmethod(reset_globals):
+    """When an alternate module implementation is loaded via a backend, the concrete
+    instance of the module backend is passed to .load via the load_backend kwarg.
+    """
+    _, DummyBar = setup_saved_model(MockBackend)
+    with temp_config(
+        {
+            "module_backends": {
+                "load_priority": [{"type": backend_types.MOCK}],
+            }
+        }
+    ):
+        configure()
+        with mock.patch.object(DummyBar, "load", MagicMock()) as mock_load:
+            mock_load.return_value = DummyBar()
+            dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_LOCAL_MODEL_NAME)
+            model = caikit.core.load(dummy_model_path)
+
+            load_backends = module_backend_config.configured_load_backends()
+            expected_load_backend = [
+                be for be in load_backends if be.backend_type == backend_types.MOCK
+            ][0]
+
+            mock_load.assert_called_with(
+                dummy_model_path, **{"load_backend": expected_load_backend}
+            )
+
+
 def test_preferred_backend_disabled(reset_globals):
     """Make sure that for a model artifact saved with a local backend loads as
     local even with a preferred_backend when the preferred backend is disabled.
     """
     DummyFoo, DummyBar = setup_saved_model(MockBackend)
     with temp_config(
         {
@@ -476,16 +472,16 @@
             pass
 
         def stop(self):
             pass
 
     backend_types.register_backend_type(MockBackend2)
 
-    @caikit.core.blocks.block(base_module=DummyFoo, backend_type=backend_types.MOCK2)
-    class DummyBaz(caikit.core.blocks.base.BlockBase):
+    @caikit.core.modules.module(base_module=DummyFoo, backend_type=backend_types.MOCK2)
+    class DummyBaz(caikit.core.ModuleBase):
         SUPPORTED_LOAD_BACKENDS = [backend_types.MOCK, backend_types.MOCK2]
 
         @classmethod
         def load(self, *args, **kwargs):
             return DummyBaz()
 
     with temp_config(
@@ -503,16 +499,16 @@
 
 
 def test_load_must_return_model():
     """Make sure that the return type of load is checked to be an instance of
     ModuleBase, and will raise TypeError if it is not.
     """
 
-    @caikit.core.block("00110203-baad-beef-0809-0a0b0c0d0e0f", "FunkyBlock", "0.0.1")
-    class _FunkyModel(SampleBlock):
+    @caikit.core.module("00110203-baad-beef-0809-0a0b0c0d0e0f", "FunkyModule", "0.0.1")
+    class _FunkyModel(SampleModule):
         @classmethod
         def load(cls, model_path):
             return (super().load(model_path), "something else")
 
     model = _FunkyModel()
     with tempfile.TemporaryDirectory() as tempdir:
         # NOTE: the module will get detected as tests since _FunkyModel is defined here
@@ -588,23 +584,23 @@
             pass
 
         def register_config(self, config):
             pass
 
         def load(self, model_path, *args, **kwargs):
             """This load function doesn't read from model_path, so it definitely does not read the config.yml file"""
-            return SampleBlock()
+            return SampleModule()
 
     backend_types.register_backend_type(NoYamlLoader)
 
     with temp_config(
         {
             "module_backends": {
                 "load_priority": [
                     {"type": NoYamlLoader.backend_type},
                 ]
             }
         }
     ):
         configure()
         model = caikit.core.load(tmpdir)
-        assert isinstance(model, SampleBlock)
+        assert isinstance(model, SampleModule)
```

### Comparing `caikit-0.4.4/tests/core/test_module.py` & `caikit-0.5.0/tests/core/modules/test_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,37 +9,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
-import abc
 import io
 import os
 import tempfile
-import uuid
-
-# Third Party
-import pytest
 
 # First Party
 import aconfig
 
 # Local
-from caikit.core import ModuleConfig, module
-from caikit.core.module_backend_config import configured_load_backends
-from caikit.core.module_backends import backend_types
-from caikit.core.module_type import SUPPORTED_LOAD_BACKENDS_VAR_NAME
+from caikit.core import ModuleConfig
+from caikit.core.module_backends.module_backend_config import configured_load_backends
+from caikit.core.modules.decorator import SUPPORTED_LOAD_BACKENDS_VAR_NAME
+from caikit.core.registries import module_backend_registry
 
 # pylint: disable=import-error
 from sample_lib.data_model.sample import SampleInputType, SampleTask
 
 # Unit Test Infrastructure
-from tests.conftest import fixtures_dir, temp_config
+from tests.conftest import temp_config
 
 # NOTE: We do need to import `reset_backend_types` and `reset_module_distribution_registry` for `reset_globals` to work
 from tests.core.helpers import *
 import caikit.core
 
 ## Helpers #####################################################################
 
@@ -47,40 +42,40 @@
 @pytest.fixture
 def base_module_instance():
     return caikit.core.ModuleBase()
 
 
 @pytest.fixture
 def model_path(fixtures_dir):
-    yield os.path.join(fixtures_dir, "dummy_block")
+    yield os.path.join(fixtures_dir, "dummy_module")
 
 
 @pytest.fixture
 def model_config(model_path):
     yield ModuleConfig.load(model_path)
 
 
 DUMMY_MODULE_ID = "foo"
 
 
 def configure_alternate_backend_impl():
     """Function to register a new backend type and register a module implementation
     of existing caikit.core module"""
 
-    @caikit.core.blocks.block(
+    @caikit.core.modules.module(
         id=DUMMY_MODULE_ID, name="dummy base", version="0.0.1", task=SampleTask
     )
-    class DummyFoo(caikit.core.blocks.base.BlockBase):
+    class DummyFoo(caikit.core.ModuleBase):
         pass
 
     # Register backend type
     backend_types.register_backend_type(MockBackend)
 
-    @caikit.core.blocks.block(base_module=DummyFoo, backend_type=backend_types.MOCK)
-    class DummyBar(caikit.core.blocks.base.BlockBase):
+    @caikit.core.modules.module(base_module=DummyFoo, backend_type=backend_types.MOCK)
+    class DummyBar(caikit.core.ModuleBase):
         def test_fetching_backend(self):
             return [
                 backend
                 for backend in configured_load_backends()
                 if backend.backend_type == backend_types.MOCK
             ][0]
 
@@ -88,15 +83,15 @@
 
 
 ## ModuleBase ##################################################################
 
 
 def test_load_evaluation_dataset(fixtures_dir):
     assert isinstance(
-        module.ModuleBase._load_evaluation_dataset(
+        ModuleBase._load_evaluation_dataset(
             os.path.join(fixtures_dir, "dummy_dataset.json")
         ),
         list,
     )
 
 
 def test_init_available():
@@ -118,15 +113,15 @@
 def test_save_not_implemented(base_module_instance):
     with pytest.raises(NotImplementedError):
         base_module_instance.save("dummy_path")
 
 
 def test_train_not_implemented():
     with pytest.raises(NotImplementedError):
-        caikit.core.BlockBase.train()
+        caikit.core.ModuleBase.train()
 
 
 def test_run_batch_keyword_only(model_path):
     """Make sure that calling run_batch without any positional args is safe"""
     dummy_model = caikit.core.load(model_path)
     dummy_model.run(sample_input=SampleInputType(name="Gabe"))
     dummy_model.run_batch(sample_input=[SampleInputType(name="Gabe")])
@@ -139,81 +134,50 @@
     assert isinstance(model_config, ModuleConfig)
     assert isinstance(model_config, aconfig.Config)
 
 
 def test_init_and_members():
     config = ModuleConfig(
         {
-            "block_id": "123",
-            "block_class": "caikit.core.blocks.dummy.Dummy",
+            "module_id": "123",
+            "module_class": "caikit.core.modules.dummy.Dummy",
             "name": "Dummy Block",
             "string": "hello",
             "integer": 1,
             "float": 0.5,
             "nested": {
                 "string": "world",
                 "integer": 2,
                 "float": -0.123,
             },
         }
     )
 
-    assert config.block_id == "123"
-    assert config.block_class == "caikit.core.blocks.dummy.Dummy"
+    assert config.module_id == "123"
+    assert config.module_class == "caikit.core.modules.dummy.Dummy"
     assert isinstance(config.string, str)
     assert config.string == "hello"
     assert isinstance(config.integer, int)
     assert config.integer == 1
     assert isinstance(config.float, float)
     assert config.float == 0.5
     assert isinstance(config.nested, dict)
     assert config.nested.string == "world"
     assert config.nested.integer == 2
     assert config.nested.float == -0.123
 
 
-def test_block_config_has_module_id(model_config):
-    assert model_config.module_id is not None
-    assert model_config.module_id == model_config.block_id
-
-
-def test_workflow_config_has_module_id():
-    config = ModuleConfig(
-        {
-            "workflow_id": "123",
-            "workflow_class": "caikit.core.workflows.dummy.Dummy",
-            "name": "Dummy Workflow",
-        }
-    )
-
-    assert config.module_id is not None
-    assert config.module_id == config.workflow_id
-
-
-def test_resource_config_has_module_id():
-    config = ModuleConfig(
-        {
-            "resource_id": "r123",
-            "resource_class": "caikit.core.resources.dummy.Dummy",
-            "name": "Dummy Resource",
-        }
-    )
-
-    assert config.module_id is not None
-    assert config.module_id == config.resource_id
-
-
 def test_reserved_keys():
-    for reserved_key in ("module_id", "model_path"):
+    for reserved_key in ("model_path",):
         with pytest.raises(KeyError):
             ModuleConfig(
                 {
                     reserved_key: "x",
-                    "block_class": "caikit.core.blocks.dummy.Dummy",
-                    "name": "Dummy Workflow",
+                    "module_class": "caikit.core.modules.dummy.Dummy",
+                    "name": "Dummy Module",
                 }
             )
 
 
 def test_no_config_yaml():
     with pytest.raises(FileNotFoundError):
         with tempfile.TemporaryDirectory() as tempd:
@@ -256,33 +220,34 @@
 
 
 def test_load_file_like_conversion_and_back(model_path):
     """Test that we can load a model, export to a file-like object, and reload the model."""
     dummy_model = caikit.core.load(model_path)
     file_like = dummy_model.as_file_like_object()
     reloaded_model = caikit.core.load(file_like)
-    assert isinstance(reloaded_model, caikit.core.BlockBase)
+    assert isinstance(reloaded_model, caikit.core.ModuleBase)
 
 
 def test_load_bytes_conversion_and_back(model_path):
     """Test that we can load a model, export to a bytes object, and reload the model."""
     dummy_model = caikit.core.load(model_path)
     bytes_like = dummy_model.as_bytes()
     reloaded_model = caikit.core.load(bytes_like)
-    assert isinstance(reloaded_model, caikit.core.BlockBase)
+    assert isinstance(reloaded_model, caikit.core.ModuleBase)
 
 
 ## Non-Local Backends ##########################################################
 
 
 def test_can_get_module_id(reset_globals):
     """Test we can get registered module from registry"""
     _, DummyBar = configure_alternate_backend_impl()
     assert (
-        caikit.core.MODULE_BACKEND_REGISTRY.get(DUMMY_MODULE_ID)
+        module_backend_registry()
+        .get(DUMMY_MODULE_ID)
         .get(MockBackend.backend_type)
         .impl_class
         == DummyBar
     )
 
 
 def test_module_id_registration_for_backend(reset_globals):
@@ -290,67 +255,65 @@
     DummyFoo, DummyBar = configure_alternate_backend_impl()
     assert DummyBar.MODULE_ID == DummyFoo.MODULE_ID
 
 
 def test_module_registry_for_backend_type(reset_globals):
     """Test backend is properly registered in the module registry"""
     _ = configure_alternate_backend_impl()
-    assert DUMMY_MODULE_ID in MODULE_BACKEND_REGISTRY
-    assert MockBackend.backend_type in MODULE_BACKEND_REGISTRY[DUMMY_MODULE_ID]
+    assert DUMMY_MODULE_ID in module_backend_registry()
+    assert MockBackend.backend_type in module_backend_registry()[DUMMY_MODULE_ID]
 
 
 def test_duplicate_registration_raises(reset_globals):
     """Test duplicate registration of same backend for same module raises"""
     DummyFoo, _ = configure_alternate_backend_impl()
     with pytest.raises(AssertionError):
 
-        @caikit.core.blocks.block(base_module=DummyFoo, backend_type=backend_types.MOCK)
-        class DummyBat(caikit.core.blocks.base.BlockBase):
+        @caikit.core.modules.module(
+            base_module=DummyFoo, backend_type=backend_types.MOCK
+        )
+        class DummyBat(caikit.core.ModuleBase):
             pass
 
 
 def test_backend_impl_inheritance_error(reset_globals):
     """Test creating a backend implementation of a module
     which inherits from base module raises"""
     DummyFoo, DummyBar = configure_alternate_backend_impl()
     with pytest.raises(TypeError):
 
-        @caikit.core.blocks.block(backend_type=backend_types.MOCK)
+        @caikit.core.modules.module(backend_type=backend_types.MOCK)
         class DummyBat(DummyFoo):
             pass
 
 
 def test_class_attributes(reset_globals):
     """Test that the wrapped class has the correct attributes set"""
     DummyFoo, DummyBar = configure_alternate_backend_impl()
 
     # Make sure all of the right class attrs are set
     assert DummyBar.BACKEND_TYPE == backend_types.MOCK
     assert DummyBar.MODULE_ID == DummyFoo.MODULE_ID
     assert DummyBar.MODULE_NAME
     assert DummyBar.MODULE_VERSION
     assert DummyBar.MODULE_CLASS
-    assert DummyBar.BLOCK_ID == DummyFoo.BLOCK_ID
-    assert DummyBar.BLOCK_NAME
-    assert DummyBar.BLOCK_VERSION
-    assert DummyBar.BLOCK_CLASS
     assert DummyBar.PRODUCER_ID
 
     # No configured modules before configure
     assert not configured_load_backends()
 
     # Configure and make sure it can be fetched by the class
     with temp_config(
         {
             "module_backends": {
                 "load_priority": [{"type": backend_types.MOCK}],
             }
         }
     ):
-        caikit.core.module_backend_config.configure()
+        caikit.core.module_backends.module_backend_config.configure()
         assert DummyBar.BACKEND_TYPE == backend_types.MOCK
 
         # Make sure an instance can fetch via get_backend()
         inst = DummyBar()
         assert inst.test_fetching_backend().backend_type == backend_types.MOCK
 
 
@@ -362,62 +325,62 @@
     assert DummyBar.SUPPORTED_LOAD_BACKENDS[0] == backend_types.MOCK
 
 
 def test_override_load_supported_backend(reset_globals):
     """Test if the class can successfully define its own backends
     that it supports load from"""
 
-    @caikit.core.blocks.block(
+    @caikit.core.modules.module(
         id=DUMMY_MODULE_ID, name="dummy base", version="0.0.1", task=SampleTask
     )
-    class DummyFoo(caikit.core.blocks.base.BlockBase):
+    class DummyFoo(caikit.core.ModuleBase):
         pass
 
     class BazBackend(BackendBase):
         backend_type = "BAZ"
 
     class FooBackend(BackendBase):
         backend_type = "FOO"
 
     backend_types.register_backend_type(BazBackend)
     backend_types.register_backend_type(FooBackend)
 
     supported_backends = [backend_types.BAZ, backend_types.FOO]
 
-    @caikit.core.blocks.block(base_module=DummyFoo, backend_type=backend_types.BAZ)
-    class DummyBaz(caikit.core.blocks.base.BlockBase):
+    @caikit.core.modules.module(base_module=DummyFoo, backend_type=backend_types.BAZ)
+    class DummyBaz(caikit.core.ModuleBase):
         SUPPORTED_LOAD_BACKENDS = supported_backends
 
     assert hasattr(DummyBaz, SUPPORTED_LOAD_BACKENDS_VAR_NAME)
     assert DummyBaz.SUPPORTED_LOAD_BACKENDS == supported_backends
 
 
 def test_base_module_in_decorator(reset_globals):
     """Test multiple backend implementation of a module doesn't override base module
-    from MODULE_REGISTRY"""
+    from module registry"""
 
     class BazBackend(BackendBase):
         backend_type = "BAZ"
 
     class FooBackend(BackendBase):
         backend_type = "FOO"
 
     backend_types.register_backend_type(BazBackend)
     backend_types.register_backend_type(FooBackend)
 
-    @caikit.core.blocks.block(
+    @caikit.core.modules.module(
         id=DUMMY_MODULE_ID, name="dummy base", version="0.0.1", task=SampleTask
     )
-    class DummyLocal(caikit.core.blocks.base.BlockBase):
+    class DummyLocal(caikit.core.ModuleBase):
         pass
 
-    @caikit.core.blocks.block(backend_type=backend_types.BAZ, base_module=DummyLocal)
-    class DummyBaz(caikit.core.blocks.base.BlockBase):
+    @caikit.core.modules.module(backend_type=backend_types.BAZ, base_module=DummyLocal)
+    class DummyBaz(caikit.core.ModuleBase):
         pass
 
-    @caikit.core.blocks.block(
+    @caikit.core.modules.module(
         backend_type=backend_types.FOO, base_module=DummyLocal.MODULE_ID
     )
-    class DummyFoo(caikit.core.blocks.base.BlockBase):
+    class DummyFoo(caikit.core.ModuleBase):
         pass
 
-    assert DummyLocal in list(caikit.core.MODULE_REGISTRY.values())
+    assert DummyLocal in list(module_registry().values())
```

### Comparing `caikit-0.4.4/tests/core/test_module_backend_config.py` & `caikit-0.5.0/tests/core/module_backends/test_module_backend_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,22 +13,21 @@
 # limitations under the License.
 
 """
 Tests for the backend configuration framework
 """
 
 # Local
-from caikit.core.blocks import base, block
-from caikit.core.module_backend_config import (
+from caikit.core.module_backends.module_backend_config import (
     configure,
     configured_load_backends,
     configured_train_backends,
     start_backends,
 )
-from caikit.core.module_backends import backend_types
+from caikit.core.modules import base, module
 from sample_lib.data_model import SampleTask
 from tests.conftest import temp_config
 from tests.core.helpers import *
 
 # Setup #########################################################################
 
 foo_cfg = {"mock": 1}
@@ -189,38 +188,38 @@
 
 
 def test_multiple_module_same_backend_configures(reset_globals):
     """Test to check if multiple modules for same backend
     can override backend configurations"""
     # Register backend type
 
-    @block(id="foo", name="dummy base", version="0.0.1", task=SampleTask)
-    class DummyFoo(base.BlockBase):
+    @module(id="foo", name="dummy base", version="0.0.1", task=SampleTask)
+    class DummyFoo(base.ModuleBase):
         pass
 
     # Create dummy classes
-    @block(
+    @module(
         base_module=DummyFoo,
         backend_type=backend_types.MOCK,
         backend_config_override={"bar1": 1},
     )
-    class DummyBar(base.BlockBase):
+    class DummyBar(base.ModuleBase):
         pass
 
-    @block(id="foo2", name="dummy base", version="0.0.1", task=SampleTask)
-    class DummyFoo2(base.BlockBase):
+    @module(id="foo2", name="dummy base", version="0.0.1", task=SampleTask)
+    class DummyFoo2(base.ModuleBase):
         pass
 
     # Create dummy classes
-    @block(
+    @module(
         base_module=DummyFoo2,
         backend_type=backend_types.MOCK,
         backend_config_override={"bar2": 2},
     )
-    class DummyBar(base.BlockBase):
+    class DummyBar(base.ModuleBase):
         pass
 
     # Initiate configuration
 
     with temp_config(
         {
             "module_backends": {
```

### Comparing `caikit-0.4.4/tests/core/test_module_metadata.py` & `caikit-0.5.0/tests/core/modules/test_module_metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,19 +25,18 @@
 # Third Party
 import pytest
 
 # Local
 from caikit.core import toolkit
 
 # pylint: disable=import-error
-from sample_lib.blocks.sample_task import SampleBlock
+from sample_lib.data_model import SampleTask
 
 # pylint: disable=import-error
-from sample_lib.data_model import SampleTask
-from sample_lib.workflows.sample_task import SampleWorkflow
+from sample_lib.modules.sample_task import SampleModule
 
 # Unit Test Infrastructure
 from tests.base import TestCaseBase
 import caikit.core
 
 # scratch:
 # - might want to support like a `saved` date?
@@ -69,22 +68,22 @@
 def fixtures_dir():
     return TestCaseBase.fixtures_dir
 
 
 @pytest.fixture
 # pylint: disable=redefined-outer-name
 def sample_model_path(fixtures_dir):
-    return os.path.join(fixtures_dir, "sample_block")
+    return os.path.join(fixtures_dir, "sample_module")
 
 
 # pylint: disable=redefined-outer-name
-def test_block_metadata_is_persisted(sample_model_path):
+def test_module_metadata_is_persisted(sample_model_path):
     """Make sure that if you load and then re-save any model, the metadata in the config.yml is
     persisted."""
-    # Get the block metadata:
+    # Get the module metadata:
     initial_metadata = _load_model_metadata(sample_model_path)
     model = caikit.core.load(sample_model_path)
 
     with tempfile.TemporaryDirectory() as tempdir:
         model.save(tempdir)
         resaved_metadata = _load_model_metadata(tempdir)
 
@@ -96,15 +95,15 @@
 
 
 # pylint: disable=redefined-outer-name
 def test_loaded_modules_have_metadata(sample_model_path):
     """Make sure a model has metadata after being loaded"""
     expected_metadata = _load_model_metadata(sample_model_path)
     model_loaded_with_core = caikit.core.load(sample_model_path)
-    model_directly_loaded = SampleBlock.load(sample_model_path)
+    model_directly_loaded = SampleModule.load(sample_model_path)
 
     # TODO: figure out "module_id" and "model_path" as well...
 
     _check_dicts_equal(
         expected_metadata,
         model_loaded_with_core.metadata,
         {"module_id", "model_path"},
@@ -112,37 +111,37 @@
     _check_dicts_equal(
         expected_metadata,
         model_directly_loaded.metadata,
         {"module_id", "model_path"},
     )
 
 
-def test_block_has_saved_field():
+def test_module_has_saved_field():
     """Make sure that if you load a model and then save it multiple times,
     the "saved" field should track each timestamp when you save, and should be different
     """
     with tempfile.TemporaryDirectory() as tempdir:
-        model1 = SampleBlock()
+        model1 = SampleModule()
         path1 = os.path.join(tempdir, "test1")
         model1.save(path1)
         resaved_metadata1 = _load_model_metadata(path1)
 
         model2 = caikit.core.load(path1)
         path2 = os.path.join(tempdir, "test1")
         model2.save(path2)
         resaved_metadata2 = _load_model_metadata(path2)
 
     assert "saved" in resaved_metadata1
     assert "saved" in resaved_metadata2
     assert resaved_metadata1["saved"] != resaved_metadata2["saved"]
 
 
-def test_block_has_tracking_id_field():
+def test_module_has_tracking_id_field():
     with tempfile.TemporaryDirectory() as tempdir:
-        model1 = SampleBlock()
+        model1 = SampleModule()
         path1 = os.path.join(tempdir, "test1")
         model1.save(path1)
         resaved_metadata1 = _load_model_metadata(path1)
 
         model2 = caikit.core.load(path1)
         path2 = os.path.join(tempdir, "test1")
         model2.save(path2)
@@ -150,79 +149,38 @@
 
     assert "tracking_id" in resaved_metadata1
     assert "tracking_id" in resaved_metadata2
     assert resaved_metadata1["tracking_id"] == resaved_metadata2["tracking_id"]
 
 
 # pylint: disable=redefined-outer-name
-def test_block_metadata_is_saved_into_a_workflow(sample_model_path):
-    """Make sure that if you load a model and then re-package it as part of yet another model
-    (in this case a block is packaged inside a workflow), the metadata of the original model is
-    persisted"""
-    # Get the block metadata:
-    initial_metadata = _load_model_metadata(sample_model_path)
-    model = caikit.core.load(sample_model_path)
-
-    # Create a new workflow containing our block
-    workflow = SampleWorkflow(model)
-
-    with tempfile.TemporaryDirectory() as tempdir:
-        workflow.save(tempdir)
-        # The block's .yaml should live under workflow_root/dummy_model/config.yml
-        resaved_metadata = _load_model_metadata(os.path.join(tempdir, "dummy_model"))
-
-    # assert resaved_metadata == initial_metadata
-    fields_to_not_check = {"saved", "SampleBlock_version", "train"}
-    _check_dicts_equal(resaved_metadata, initial_metadata, fields_to_not_check)
-
-
-# pylint: disable=redefined-outer-name
 def test_load_can_be_called_directly_with_non_standard_kwargs(sample_model_path):
     initial_metadata = _load_model_metadata(sample_model_path)
     # note that
     # - no positional arguments given
     # - path is `model_path` not `module_path`
-    model = SampleBlock.load(foo="bar", test_kw="arg", model_path=sample_model_path)
+    model = SampleModule.load(foo="bar", test_kw="arg", model_path=sample_model_path)
 
     assert len(model.metadata) > 0
     _check_dicts_equal(initial_metadata, model.metadata, {"module_id", "model_path"})
 
     # Write a class that doesn't have a `xxx_path` arg for load
-    @caikit.core.block(
-        "00110203-0809-beef-baad-0a0b0c0d0e0f", "FunkyBlock", "0.0.1", SampleTask
+    @caikit.core.module(
+        "00110203-0809-beef-baad-0a0b0c0d0e0f", "FunkyModule", "0.0.1", SampleTask
     )
-    class _FunkyModel(SampleBlock):
+    class _FunkyModel(SampleModule):
         @classmethod
         def load(cls, some_really_odd_param_name):
             return super().load(some_really_odd_param_name)
 
     # check this doesn't raise
     # (it won't extract metadata though...)
     _FunkyModel.load(some_really_odd_param_name=sample_model_path)
 
 
 # pylint: disable=redefined-outer-name
 def test_parent_class_loads_work(sample_model_path):
-    """This test ensures that our metadata injector works on blocks that inherit from other
+    """This test ensures that our metadata injector works on modules that inherit from other
     classes"""
-    model = SampleBlock.load(sample_model_path)
-
-    assert isinstance(model, SampleBlock)
-
+    model = SampleModule.load(sample_model_path)
 
-def test_workflows_save_correct_module_paths():
-    with tempfile.TemporaryDirectory() as tempdir:
-        SampleWorkflow(SampleBlock()).save(tempdir)
-        workflow = caikit.core.load(tempdir)
-
-    # Should only be the path to the one block
-    assert len(workflow.metadata["module_paths"]) == 1
-    # Add a fake module path
-    module_paths = workflow.metadata["module_paths"]
-    module_paths["some_module"] = "some_path"
-    assert len(workflow.metadata["module_paths"]) == 2
-
-    # Assert that re-loading works fine and fake path not in new model's metadata
-    with tempfile.TemporaryDirectory() as tempdir:
-        workflow.save(tempdir)
-        reloaded_workflow = caikit.core.load(tempdir)
-    assert len(reloaded_workflow.metadata["module_paths"]) == 1
+    assert isinstance(model, SampleModule)
```

### Comparing `caikit-0.4.4/tests/core/test_task.py` & `caikit-0.5.0/tests/core/test_task.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import uuid
 
 # Third Party
 import pytest
 
 # Local
 from caikit.core import TaskBase, task
-from sample_lib import SampleBlock
+from sample_lib import SampleModule
 from sample_lib.data_model.sample import SampleInputType, SampleOutputType, SampleTask
 import caikit.core
 
 
 def test_task_decorator_has_required_inputs_and_output_type():
     @task(
         required_parameters={"sample_input": SampleInputType},
@@ -47,42 +47,42 @@
             output_type=str,
         )
         class SampleTask(TaskBase):
             pass
 
 
 def test_task_is_set_on_module_classes():
-    assert hasattr(SampleBlock, "TASK_CLASS")
-    assert SampleBlock.TASK_CLASS == SampleTask
+    assert hasattr(SampleModule, "TASK_CLASS")
+    assert SampleModule.TASK_CLASS == SampleTask
 
 
-def test_task_can_be_inferred_from_parent_block():
-    @caikit.core.blocks.block(id="foobar", name="Stuff", version="0.0.1")
-    class Stuff(SampleBlock):
+def test_task_can_be_inferred_from_parent_module():
+    @caikit.core.modules.module(id="foobar", name="Stuff", version="0.0.1")
+    class Stuff(SampleModule):
         pass
 
-    assert Stuff.TASK_CLASS == SampleBlock.TASK_CLASS
+    assert Stuff.TASK_CLASS == SampleModule.TASK_CLASS
 
 
-def test_task_cannot_conflict_with_parent_block():
+def test_task_cannot_conflict_with_parent_module():
     @task(
         required_parameters={"foo": SampleInputType},
         output_type=SampleOutputType,
     )
     class SomeTask(TaskBase):
         pass
 
     with pytest.raises(TypeError, match="but superclass has"):
 
-        @caikit.core.blocks.block(
+        @caikit.core.modules.module(
             id=str(uuid.uuid4()), name="Stuff", version="0.0.1", task=SomeTask
         )
-        class Stuff(SampleBlock):
+        class Stuff(SampleModule):
             pass
 
 
-def test_task_is_not_required_for_blocks():
-    @caikit.core.blocks.block(id=str(uuid.uuid4()), name="Stuff", version="0.0.1")
-    class Stuff(caikit.core.blocks.base.BlockBase):
+def test_task_is_not_required_for_modules():
+    @caikit.core.modules.module(id=str(uuid.uuid4()), name="Stuff", version="0.0.1")
+    class Stuff(caikit.core.ModuleBase):
         pass
 
     assert Stuff.TASK_CLASS is None
```

### Comparing `caikit-0.4.4/tests/core/toolkit/test_compatibility.py` & `caikit-0.5.0/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/toolkit/test_error_handler.py` & `caikit-0.5.0/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/toolkit/test_fileio.py` & `caikit-0.5.0/tests/core/toolkit/test_fileio.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,19 +23,21 @@
 # Unit Test Infrastructure
 from tests.base import TestCaseBase
 
 
 class TestFeatureExtractor(TestCaseBase):
     def setUp(self):
         self.yaml_filename = os.path.join(
-            self.fixtures_dir, "dummy_block", "config.yml"
+            self.fixtures_dir, "dummy_module", "config.yml"
+        )
+        self.json_filename = os.path.join(
+            self.fixtures_dir, "dummy_module", "data.json"
         )
-        self.json_filename = os.path.join(self.fixtures_dir, "dummy_block", "data.json")
         self.pickle_filename = os.path.join(
-            self.fixtures_dir, "dummy_block", "data.pkl"
+            self.fixtures_dir, "dummy_module", "data.pkl"
         )
         self.csv_filename = os.path.join(self.fixtures_dir, "sample.csv")
 
     def test_load_yaml(self):
         yaml_dict = toolkit.load_yaml(self.yaml_filename)
         self.assertIsInstance(yaml_dict, dict)
         self.assertEqual(yaml_dict["train"]["batch_size"], 64)
```

### Comparing `caikit-0.4.4/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.5.0/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/toolkit/test_serializers.py` & `caikit-0.5.0/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.5.0/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/core/workflows/__init__.py` & `caikit-0.5.0/tests/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/data_model_helpers.py` & `caikit-0.5.0/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/fixtures/config/config.yml` & `caikit-0.5.0/tests/fixtures/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.5.0/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/fixtures/dummy_block.zip` & `caikit-0.5.0/tests/fixtures/dummy_module.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/fixtures/dummy_block/config.yml` & `caikit-0.5.0/tests/fixtures/dummy_module/config.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # a dummy configuration yaml
 # note: this config is not actually loadable since there is no DummyBlock
 #   but we *can* use it to create a config object for testing
-block_id: "00110203-0405-0607-0809-0a0b02dd0e0f"
-block_class: "sample_lib.blocks.sample_task.sample_implementation.SampleBlock"
+module_id: "00110203-0405-0607-0809-0a0b02dd0e0f"
+module_class: "sample_lib.modules.sample_task.sample_implementation.SampleModule"
 name: "Dummy config file."
 version: "4.0.2"
 description': "dummy model for testing"
 
 created: "2022-11-03 21:55:38.496338"
 
 tracking_id: ba67469f-281d-4250-915c-00111e0327a5
```

### Comparing `caikit-0.4.4/tests/fixtures/dummy_block_singleton/config.yml` & `caikit-0.5.0/tests/fixtures/dummy_module_singleton/config.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # a dummy configuration yaml
 # note: this config is not actually loadable since there is no DummyBlock
 #   but we *can* use it to create a config object for testing
-block_id: "00110203-0405-0607-0809-0a0b02dd0e0f"
-block_class: "sample_lib.blocks.sample_task.sample_implementation.SampleBlock"
+module_id: "00110203-0405-0607-0809-0a0b02dd0e0f"
+module_class: "sample_lib.modules.sample_task.sample_implementation.SampleModule"
 name: "Dummy config file."
 version: "4.0.2"
 
 train:
     batch_size: 64
     learning_rate: 0.0015
     optim_method: "Rprop"
```

### Comparing `caikit-0.4.4/tests/fixtures/fixtures.py` & `caikit-0.5.0/tests/fixtures/fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,8 +88,8 @@
 
     @staticmethod
     def get_invalid_model_archive_path():
         return os.path.join(os.path.dirname(__file__), "models", "bad_archive.zip")
 
     @staticmethod
     def get_good_model_type():
-        return "fake_block"
+        return "fake_module"
```

### Comparing `caikit-0.4.4/tests/fixtures/invalid.zip` & `caikit-0.5.0/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/fixtures/linux.txt` & `caikit-0.5.0/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/fixtures/primitive_party.proto` & `caikit-0.5.0/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_pb2.py` & `caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py` & `caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_train_pb2.py` & `caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_train_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py` & `caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.5.0/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py` & `caikit-0.5.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
-A sample block for sample things!
+A sample module for sample things!
 """
 # Standard
 from typing import Union
 
 # Local
 from ...data_model.sample import OtherOutputType, OtherTask, SampleInputType
 from caikit.core.data_model import DataStream
-from caikit.core.module import ModuleLoader, ModuleSaver
+from caikit.core.modules import ModuleLoader, ModuleSaver
 import caikit.core
 
 
-@caikit.core.block(
-    "33221100-0405-0607-0809-0a0b02dd0e0f", "OtherBlock", "0.0.1", OtherTask
+@caikit.core.module(
+    "33221100-0405-0607-0809-0a0b02dd0e0f", "OtherModule", "0.0.1", OtherTask
 )
-class OtherBlock(caikit.core.BlockBase):
+class OtherModule(caikit.core.ModuleBase):
     def __init__(self, batch_size=64, learning_rate=0.0015):
         super().__init__()
         self.batch_size = batch_size
         self.learning_rate = learning_rate
 
     def run(
         self, sample_input: Union[SampleInputType, str]
@@ -48,13 +48,13 @@
 
     @classmethod
     def train(
         cls,
         training_data: DataStream[int],
         sample_input: Union[SampleInputType, str],
         batch_size: int = 64,
-    ) -> "OtherBlock":
+    ) -> "OtherModule":
         """Sample training method that produces a trained model"""
         # Barf if we were incorrectly passed data not in datastream format
         assert type(training_data) == DataStream
         assert batch_size > 0
         return cls(batch_size=batch_size)
```

### Comparing `caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py` & `caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
-A hypothetical inner block that transforms some output type rather than taking domain input
+A hypothetical inner module that transforms some output type rather than taking domain input
 """
 # Local
 from ...data_model.sample import SampleOutputType, SampleTask
 import caikit.core
 
 
-@caikit.core.block(
-    "00110203-baad-beef-0809-0a0b02dd0e0f", "SampleBlock", "0.0.1", SampleTask
+@caikit.core.module(
+    "00110203-baad-beef-0809-0a0b02dd0e0f", "SampleModule", "0.0.1", SampleTask
 )
-class InnerBlock(caikit.core.BlockBase):
+class InnerModule(caikit.core.ModuleBase):
     def __init__(self, batch_size=64, learning_rate=0.0015):
         super().__init__()
         self.batch_size = batch_size
         self.learning_rate = learning_rate
 
     def run(self, some_input: SampleOutputType) -> SampleOutputType:
         return SampleOutputType(f"nested greeting: {some_input.greeting}")
```

### Comparing `caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py` & `caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
-A sample block for sample things!
+A sample module for sample things!
 """
 # Standard
 from typing import List, Optional
 
 # Local
 from ...data_model.sample import (
     SampleInputType,
     SampleOutputType,
     SampleTask,
     SampleTrainingType,
 )
 from caikit.core.data_model import DataStream
-from caikit.core.module import ModuleLoader, ModuleSaver
+from caikit.core.modules import ModuleLoader, ModuleSaver
 import caikit.core
 
 
-@caikit.core.block(
-    "00af2203-0405-0607-0263-0a0b02dd0c2f", "ListBlock", "0.0.1", SampleTask
+@caikit.core.module(
+    "00af2203-0405-0607-0263-0a0b02dd0c2f", "ListModule", "0.0.1", SampleTask
 )
-class ListBlock(caikit.core.BlockBase):
+class ListModule(caikit.core.ModuleBase):
     POISON_PILL_NAME = "Bob Marley"
 
     def __init__(self, batch_size=64, learning_rate=0.0015):
         super().__init__()
         self.batch_size = batch_size
         self.learning_rate = learning_rate
 
@@ -66,15 +66,15 @@
 
     @classmethod
     def train(
         cls,
         training_data: DataStream[SampleTrainingType],
         batch_size: int = 64,
         poison_pills: Optional[List[str]] = None,
-    ) -> "ListBlock":
+    ) -> "ListModule":
         """Sample training method that produces a trained model"""
         # Barf if we were incorrectly passed data not in datastream format
         poison_pills = (
             poison_pills if poison_pills is not None else [cls.POISON_PILL_NAME]
         )
         assert isinstance(training_data, DataStream)
         assert len(poison_pills) > 0
```

### Comparing `caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py` & `caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-A block meant to flex a bit of the protobufs primitive support
+A module meant to flex a bit of the protobufs primitive support
 """
 # Standard
 from typing import List
 
 # Local
 from ...data_model.sample import SampleOutputType, SampleTask
-from caikit.core.module import ModuleSaver
+from caikit.core.modules import ModuleSaver
 import caikit.core
 
 
-@caikit.core.block(
-    "00112233-0405-0607-0809-0a0b02dd0e0f", "SampleBlock", "0.0.1", SampleTask
+@caikit.core.module(
+    "00112233-0405-0607-0809-0a0b02dd0e0f", "SampleModule", "0.0.1", SampleTask
 )
-class SamplePrimitiveBlock(caikit.core.BlockBase):
+class SamplePrimitiveModule(caikit.core.ModuleBase):
     def __init__(self):
         super().__init__()
 
     @classmethod
     def load(cls, model_path, **kwargs):
         return cls()
```

### Comparing `caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py` & `caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
-A sample block for sample things!
+A sample module for sample things!
 """
 # Standard
 import os
 
 # Local
 from ...data_model.sample import (
     SampleInputType,
     SampleOutputType,
     SampleTask,
     SampleTrainingType,
 )
 from caikit.core.data_model import DataStream
-from caikit.core.module import ModuleLoader, ModuleSaver
+from caikit.core.modules import ModuleLoader, ModuleSaver
 import caikit.core
 
 
-@caikit.core.block(
-    "00110203-0405-0607-0809-0a0b02dd0e0f", "SampleBlock", "0.0.1", SampleTask
+@caikit.core.module(
+    "00110203-0405-0607-0809-0a0b02dd0e0f", "SampleModule", "0.0.1", SampleTask
 )
-class SampleBlock(caikit.core.BlockBase):
+class SampleModule(caikit.core.ModuleBase):
     POISON_PILL_NAME = "Bob Marley"
     POISON_PILL_BATCH_SIZE = 999
 
     def __init__(self, batch_size=64, learning_rate=0.0015):
         super().__init__()
         self.batch_size = batch_size
         self.learning_rate = learning_rate
@@ -67,15 +67,15 @@
 
     @classmethod
     def train(
         cls,
         training_data: DataStream[SampleTrainingType],
         batch_size: int = 64,
         oom_exit: bool = False,
-    ) -> "SampleBlock":
+    ) -> "SampleModule":
         """Sample training method that produces a trained model"""
 
         if oom_exit:
             # exit with OOM code. Note _exit method is used to exit the
             # process with specified status without calling cleanup handlers
             # to replicate OOM scenario
             os._exit(137)
```

### Comparing `caikit-0.4.4/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.5.0/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py` & `caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,40 +8,41 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # Local
-from ...blocks.sample_task.sample_implementation import SampleBlock
 from ...data_model import SampleInputType, SampleOutputType, SampleTask
-from caikit.core.workflows import WorkflowLoader, WorkflowSaver
-import caikit.core
+from ...modules.sample_task.sample_implementation import SampleModule
+from caikit.core.modules import ModuleLoader, ModuleSaver
+import caikit
 
 
-@caikit.core.workflow(
-    "A34E68FA-E5E6-41BD-BAAE-77A880EB6877", "SampleWorkflow", "0.0.1", SampleTask
+@caikit.module(
+    "A34E68FA-E5E6-41BD-BAAE-77A880EB6877", "CompositeModule", "0.0.1", SampleTask
 )
-class SampleWorkflow(caikit.core.WorkflowBase):
-    def __init__(self, sample_block: SampleBlock = SampleBlock()):
+class CompositeModule(caikit.core.ModuleBase):
+    def __init__(self, sample_block: SampleModule = SampleModule()):
         super().__init__()
         self.block = sample_block
 
     def run(self, sample_input: SampleInputType) -> SampleOutputType:
         """Runs the inner block"""
         return self.block.run(sample_input)
 
     @classmethod
-    def _load(cls, workflow_loader: WorkflowLoader):
-        return SampleWorkflow(workflow_loader.load_module("dummy_model"))
+    def load(cls, model_path: str):
+        loader = ModuleLoader(model_path)
+        return CompositeModule(loader.load_module("dummy_model"))
 
     def save(self, model_path):
-        saver = WorkflowSaver(
+        saver = ModuleSaver(
             module=self,
             model_path=model_path,
         )
         with saver:
             saver.save_module(self.block, "dummy_model")
 
     @classmethod
-    def train(cls, sample_block: SampleBlock) -> "SampleWorkflow":
+    def train(cls, sample_block: SampleModule) -> "CompositeModule":
         return cls(sample_block)
```

### Comparing `caikit-0.4.4/tests/runtime/generated/__init__.py` & `caikit-0.5.0/tests/runtime/servicers/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# Standard
-import os
-import sys
-
-# Allow generated _pb2 files in here to import each other
-script_loc = os.path.dirname(os.path.realpath(__file__))
-sys.path.insert(0, script_loc)
```

### Comparing `caikit-0.4.4/tests/runtime/metrics/__init__.py` & `caikit-0.5.0/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.5.0/tests/runtime/metrics/test_rpc_meter.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 class TestRPCMeter(unittest.TestCase):
     """This test suite tests the RPCMeter class which is using for RPC metering"""
 
     def setUp(self):
         """This method runs before each test begins to run"""
         self.rpc_meter = RPCMeter()
         # Note: These are not real classes in sample_lib
-        self.another_widget_type = "<class 'sample_lib.blocks.sample_task.sample_implementation.AnotherWidget'>"
-        self.another_fidget_type = "<class 'sample_lib.blocks.sample_task.sample_implementation.AnotherFidget'>"
+        self.another_widget_type = "<class 'sample_lib.modules.sample_task.sample_implementation.AnotherWidget'>"
+        self.another_fidget_type = "<class 'sample_lib.modules.sample_task.sample_implementation.AnotherFidget'>"
 
     def test_update_metrics(self):
         pool = ThreadPool(1000)
         inputs = [self.another_widget_type for i in range(500)]
         inputs.extend([self.another_fidget_type for i in range(500)])
         pool.map(self.rpc_meter.update_metrics, inputs)
```

### Comparing `caikit-0.4.4/tests/runtime/model_management/__init__.py` & `caikit-0.5.0/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/runtime/model_management/test_batcher.py` & `caikit-0.5.0/tests/runtime/model_management/test_batcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,46 +43,46 @@
         "fixtures",
         "models",
         "foo_archive.zip",
     )
 )
 
 
-@caikit.core.block(
-    "7464f684-58e3-4e99-9a58-1c5bc085472b", "slow sample block", "0.0.1", SampleTask
+@caikit.core.module(
+    "7464f684-58e3-4e99-9a58-1c5bc085472b", "slow sample module", "0.0.1", SampleTask
 )
-class SlowSampleBlock(caikit.core.blocks.base.BlockBase):
-    """This block is just a wrapper around another module that will inject a
+class SlowSampleModule(caikit.core.ModuleBase):
+    """This module is just a wrapper around another module that will inject a
     sleep
     """
 
     def __init__(self, model, sleep_time_s=0.1):
         self._model = model
         self._sleep_time_s = sleep_time_s
         self.batches = []
         self.batches_lock = threading.Lock()
 
     def run(self, *args, **kwargs):
-        log.debug("Starting slow block")
+        log.debug("Starting slow module")
         time.sleep(self._sleep_time_s)
         return self._model.run(*args, **kwargs)
 
     def run_batch(self, *args, **kwargs):
         with self.batches_lock:
             self.batches.append((args, kwargs))
         return self._model.run_batch(*args, **kwargs)
 
 
-@caikit.core.block(
+@caikit.core.module(
     "19b126aa-b55b-4349-94f1-d676f3e12c9b",
     "Really silly bunch of bobs!",
     "0.0.1",
     SampleTask,
 )
-class StubBlock(caikit.core.blocks.base.BlockBase):
+class StubModule(caikit.core.ModuleBase):
     # NOTE: The initial implementation had "num_bobs" which expected an int.
     #   This led to the discovery of the fact that lists of ints are not
     #   considered "expandable iterables" in the default run_batch impl.
     def __init__(self):
         super().__init__()
         self.reqs = []
 
@@ -175,15 +175,15 @@
     standard_res = model.run(producer_id=prod_id)
     wrapped_res = wrapped_model.run(producer_id=prod_id)
     assert standard_res.to_dict() == wrapped_res.to_dict()
 
 
 def test_multi_request_batch():
     """Make sure that batches of size > 1 can be run"""
-    model = SlowSampleBlock(caikit.core.load(DUMMY_MODEL))
+    model = SlowSampleModule(caikit.core.load(DUMMY_MODEL))
     batch_size = 10
     wrapped_model = Batcher("test-model", model, batch_size)
     threads = {str(i): ModelRunThread(wrapped_model, i) for i in range(2 * batch_size)}
 
     for thread in threads.values():
         thread.start()
 
@@ -198,15 +198,15 @@
     assert model.batches
     assert any(len(batch) > 1 for batch in model.batches)
 
 
 def test_stop_in_flight_batch():
     """Make sure that setting the stop event will preempt running a batch"""
     model_delay = 0.001
-    model = SlowSampleBlock(caikit.core.load(DUMMY_MODEL), model_delay)
+    model = SlowSampleModule(caikit.core.load(DUMMY_MODEL), model_delay)
     batch_size = 10
     wrapped_model = Batcher("test-model", model, batch_size, model_delay * 2)
     threads = {str(i): ModelRunThread(wrapped_model, i) for i in range(2 * batch_size)}
 
     for thread in threads.values():
         thread.start()
 
@@ -267,15 +267,15 @@
     with pytest.raises(RuntimeError):
         wrapped_model.run(producer_id=prod_id)
 
 
 def test_different_kwargs():
     """Make sure that calls with ragged kwargs are batched correctly"""
 
-    model = StubBlock()
+    model = StubModule()
     batch_size = 5
     wrapped_model = Batcher("stub-model", model, batch_size)
     threads = {
         i: (
             ModelRunThread(wrapped_model, i, {"bobs_name": "Bob"})
             if i % 2
             else ModelRunThread(
@@ -302,15 +302,15 @@
 
 def test_invalid_req_after_valid_req():
     """Make sure that in a batch, if a request is processed with a missing
     required keyword arg after a request that has it, the valid request is
     processed and the invalid request is rejected.
     """
 
-    model = SlowSampleBlock(StubBlock())
+    model = SlowSampleModule(StubModule())
     batch_size = 5
     wrapped_model = Batcher("stub-model", model, batch_size)
     threads = {
         i: (
             ModelRunThread(wrapped_model, i, {"bobs_name": "Bob", "last_name": str(i)})
             if i < 2
             else ModelRunThread(wrapped_model, i, {})
@@ -336,15 +336,15 @@
 
 def test_valid_req_after_invalid_req():
     """Make sure that in a batch, if a request is processed that adds new
     keyword args which previous requests didn't have that also don't have
     defaults, the previous invalid requests are rejected.
     """
 
-    model = SlowSampleBlock(StubBlock())
+    model = SlowSampleModule(StubModule())
     batch_size = 5
     wrapped_model = Batcher("stub-model", model, batch_size)
     threads = {
         i: (
             ModelRunThread(wrapped_model, i, {"bobs_name": "Bob", "last_name": str(i)})
             if i >= 2
             else ModelRunThread(wrapped_model, i, {})
@@ -368,15 +368,15 @@
             assert isinstance(thread.response, RuntimeError)
 
 
 def test_batch_collect_delay():
     """Make sure that with the batch delay, multiple sequential calls end up in
     the same batchg even when not presented concurrently
     """
-    model = SlowSampleBlock(StubBlock())
+    model = SlowSampleModule(StubModule())
     batch_size = 5
     batch_collect_delay = 0.01
     wrapped_model = Batcher("stub-model", model, batch_size, batch_collect_delay)
 
     # Start one thread, wait for less than the collect delay, then start another
     th1 = ModelRunThread(wrapped_model, 0, {"bobs_name": "Bob"})
     th1.start()
@@ -399,15 +399,15 @@
     """There's a subtle race condition that can heppen when handling a request
     where the event is created, stop is called and completes, _then_ the request
     gets added to the queue and will never be pulled out by stop() if it has
     finished. To avoid orphaned requests in the queue, we ensure that the event
     is somewhere that stop() can find it by putting it in a member dict on
     creation. This tests ensures that the race is mitigated.
     """
-    wrapped_model = Batcher("stub-model", StubBlock(), 10)
+    wrapped_model = Batcher("stub-model", StubModule(), 10)
 
     # Patch the batcher's run function to wait on an intentional condition after
     # creating the event
     blocked_queue = BlockedSimpleQueue()
     wrapped_model._input_q = blocked_queue
 
     # Create a thread that will add a request. When run, this will create the
```

### Comparing `caikit-0.4.4/tests/runtime/model_management/test_model_loader.py` & `caikit-0.5.0/tests/runtime/model_management/test_model_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 # Third Party
 import grpc
 import pytest
 
 # Local
 from caikit.config import get_config
 from caikit.core import ModuleConfig
-from caikit.core.blocks import base, block
 from caikit.core.module_backends import backend_types
+from caikit.core.modules import base, module
 from caikit.runtime.model_management.batcher import Batcher
 from caikit.runtime.model_management.model_loader import ModelLoader
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from sample_lib.blocks.sample_task import SampleBlock
 from sample_lib.data_model import SampleInputType, SampleOutputType
+from sample_lib.modules.sample_task import SampleModule
 from tests.conftest import random_test_id, temp_config
 from tests.core.helpers import MockBackend
 from tests.fixtures import Fixtures
-import caikit.core.blocks
+import caikit.core
 
 ## Helpers #####################################################################
 
 
 @contextmanager
 def temp_model_loader():
     """Temporarily reset the ModelLoader singleton"""
@@ -61,15 +61,15 @@
     model_id = "happy_load_test"
     loaded_model = model_loader.load_model(
         model_id=model_id,
         local_model_path=Fixtures.get_good_model_path(),
         model_type=Fixtures.get_good_model_type(),
     )
     assert loaded_model.module() is not None
-    assert isinstance(loaded_model.module(), base.BlockBase)
+    assert isinstance(loaded_model.module(), base.ModuleBase)
     assert model_id == loaded_model.id()
     assert Fixtures.get_good_model_type() == loaded_model.type()
     assert Fixtures.get_good_model_path() == loaded_model.path()
 
     # Models are not sized by the loader
     assert loaded_model.size() == 0
 
@@ -79,15 +79,15 @@
     model_id = "happy_load_test"
     loaded_model = model_loader.load_model(
         model_id=model_id,
         local_model_path=Fixtures.get_good_model_archive_path(),
         model_type=Fixtures.get_good_model_type(),
     )
     assert loaded_model.module() is not None
-    assert isinstance(loaded_model.module(), base.BlockBase)
+    assert isinstance(loaded_model.module(), base.ModuleBase)
 
 
 def test_load_model_error_not_found_response(model_loader):
     """Test load model's model does not exist error response"""
     model_id = random_test_id()
     with pytest.raises(CaikitRuntimeException) as context:
         model_loader.load_model(
@@ -163,18 +163,18 @@
 def test_with_batching(model_loader):
     """Make sure that loading with batching configuration correctly wraps a
     Batcher around the model.
     """
     model = model_loader.load_model(
         "load_with_batch",
         Fixtures.get_good_model_path(),
-        model_type="fake_batch_block",
+        model_type="fake_batch_module",
     ).module()
     assert isinstance(model, Batcher)
-    assert model._batch_size == get_config().runtime.batching.fake_batch_block.size
+    assert model._batch_size == get_config().runtime.batching.fake_batch_module.size
 
     # Make sure another model loads without batching
     model = model_loader.load_model(
         "load_without_batch",
         Fixtures.get_good_model_path(),
         model_type=Fixtures.get_good_model_type(),
     ).module()
@@ -221,66 +221,66 @@
             model._batch_collect_delay_s
             == getattr(cfg.runtime.batching, model_type).collect_delay_s
         )
 
 
 def test_load_distributed_impl():
     """Make sure that when configured, an alternate distributed
-    implementation of a block can be loaded
+    implementation of a module can be loaded
     """
 
-    reg_copy = copy.deepcopy(caikit.core.module.MODULE_REGISTRY)
-    backend_registry_copy = copy.deepcopy(caikit.core.module.MODULE_BACKEND_REGISTRY)
+    reg_copy = copy.deepcopy(caikit.core.registries.module_registry())
+    backend_registry_copy = copy.deepcopy(
+        caikit.core.registries.module_backend_registry()
+    )
     # 🌶️🌶️🌶️: the MODULE_BACKEND_REGISTRY can't be easily patched since two separate modules hold
-    # an imported reference to it and one edits it (module_type.py) while the other reads it
+    # an imported reference to it and one edits it (decorator.py) while the other reads it
     # (model_manager.py)
 
-    with mock.patch.object(caikit.core.module, "MODULE_REGISTRY", reg_copy):
+    with mock.patch.object(caikit.core.registries, "MODULE_REGISTRY", reg_copy):
         with mock.patch.object(
-            caikit.core.module_type, "MODULE_BACKEND_REGISTRY", backend_registry_copy
+            caikit.core.registries,
+            "MODULE_BACKEND_REGISTRY",
+            backend_registry_copy,
         ):
-            with mock.patch.object(
-                caikit.core.model_manager,
-                "MODULE_BACKEND_REGISTRY",
-                backend_registry_copy,
-            ):
-
-                @block(
-                    base_module=SampleBlock,
-                    backend_type=backend_types.MOCK,
-                    backend_config_override={"bar1": 1},
-                )
-                class DistributedGadget(caikit.core.blocks.base.BlockBase):
-                    """An alternate implementation of a Gadget"""
-
-                    SUPPORTED_LOAD_BACKENDS = [
-                        MockBackend.backend_type,
-                        backend_types.LOCAL,
-                    ]
-
-                    def __init__(self, bar):
-                        self.bar = bar
-
-                    def run(self, sample_input: SampleInputType) -> SampleOutputType:
-                        return SampleOutputType(
-                            greeting=f"hello distributed {sample_input.name}"
-                        )
-
-                    @classmethod
-                    def load(cls, model_load_path) -> "DistributedGadget":
-                        config = ModuleConfig.load(model_load_path)
-                        return cls(bar=config.bar)
-
-                with tempfile.TemporaryDirectory() as model_path:
-                    # Create and save the model directly with the local impl
-                    SampleBlock().save(model_path)
-
-                    model_type = "gadget"
-
-                    with temp_model_loader() as model_loader:
-                        # Load the distributed version
-                        model = model_loader.load_model(
-                            random_test_id(),
-                            model_path,
-                            model_type=model_type,
-                        ).module()
-                        assert isinstance(model, DistributedGadget)
+
+            @module(
+                base_module=SampleModule,
+                backend_type=backend_types.MOCK,
+                backend_config_override={"bar1": 1},
+            )
+            class DistributedGadget(caikit.core.ModuleBase):
+                """An alternate implementation of a Gadget"""
+
+                SUPPORTED_LOAD_BACKENDS = [
+                    MockBackend.backend_type,
+                    backend_types.LOCAL,
+                ]
+
+                def __init__(self, bar):
+                    self.bar = bar
+
+                def run(self, sample_input: SampleInputType) -> SampleOutputType:
+                    return SampleOutputType(
+                        greeting=f"hello distributed {sample_input.name}"
+                    )
+
+                @classmethod
+                def load(cls, model_load_path, **kwargs) -> "DistributedGadget":
+                    # NOTE: kwargs needed here for load_backend
+                    config = ModuleConfig.load(model_load_path)
+                    return cls(bar=config.bar)
+
+            with tempfile.TemporaryDirectory() as model_path:
+                # Create and save the model directly with the local impl
+                SampleModule().save(model_path)
+
+                model_type = "gadget"
+
+                with temp_model_loader() as model_loader:
+                    # Load the distributed version
+                    model = model_loader.load_model(
+                        random_test_id(),
+                        model_path,
+                        model_type=model_type,
+                    ).module()
+                    assert isinstance(model, DistributedGadget)
```

### Comparing `caikit-0.4.4/tests/runtime/model_management/test_model_manager.py` & `caikit-0.5.0/tests/runtime/model_management/test_model_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import unittest
 
 # Third Party
 import grpc
 
 # Local
 from caikit import get_config
-from caikit.core.blocks.base import BlockBase
+from caikit.core.modules import ModuleBase
 from caikit.runtime.model_management.loaded_model import LoadedModel
 from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils.import_util import get_dynamic_module
 from tests.conftest import random_test_id, temp_config
 from tests.fixtures import Fixtures
 
@@ -210,15 +210,15 @@
         model_id = random_test_id()
         Fixtures.load_model(
             model_id=model_id,
             local_model_path=Fixtures.get_good_model_path(),
             model_type=Fixtures.get_good_model_type(),
         )
         model = self.model_manager.retrieve_model(model_id)
-        self.assertIsInstance(model, BlockBase)
+        self.assertIsInstance(model, ModuleBase)
         self.assertEqual(len(self.model_manager.loaded_models), 1)
 
     def test_retrieve_model_raises_error_for_not_found_model(self):
         """Test that gRPC NOT_FOUND exception raised when non-existent model retrieved"""
         with self.assertRaises(CaikitRuntimeException) as context:
             self.model_manager.retrieve_model("not-found")
         self.assertEqual(context.exception.status_code, grpc.StatusCode.NOT_FOUND)
@@ -335,31 +335,31 @@
                 self.model_manager.load_model(
                     random_test_id(), ANY_MODEL_PATH, ANY_MODEL_TYPE
                 )
 
             self.assertEqual(context.exception.status_code, grpc.StatusCode.NOT_FOUND)
             self.assertEqual(len(self.model_manager.loaded_models), 0)
 
-    def test_retrieve_model_returns_the_block_from_the_model_loader(self):
+    def test_retrieve_model_returns_the_module_from_the_model_loader(self):
         """Test that a loaded model can be retrieved"""
         model_id = random_test_id()
-        expected_block = "this is definitely a stub block"
+        expected_module = "this is definitely a stub module"
         mock_sizer = MagicMock()
         mock_loader = MagicMock()
 
         with patch.object(self.model_manager, "model_loader", mock_loader):
             with patch.object(self.model_manager, "model_sizer", mock_sizer):
                 mock_sizer.get_model_size.return_value = 1
                 mock_loader.load_model.return_value = (
-                    LoadedModel.Builder().module(expected_block).build()
+                    LoadedModel.Builder().module(expected_module).build()
                 )
                 self.model_manager.load_model(model_id, ANY_MODEL_PATH, ANY_MODEL_TYPE)
 
                 model = self.model_manager.retrieve_model(model_id)
-                self.assertEqual(expected_block, model)
+                self.assertEqual(expected_module, model)
 
     def test_get_model_size_returns_size_from_model_sizer(self):
         """Test that loading a model stores the size from the ModelSizer"""
         mock_loader = MagicMock()
         mock_sizer = MagicMock()
         expected_model_size = 1234
         model_id = random_test_id()
```

### Comparing `caikit-0.4.4/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.5.0/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/runtime/model_management/test_training_manager.py` & `caikit-0.5.0/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/runtime/service_generation/signature_parsing/test_docstrings.py` & `caikit-0.5.0/tests/runtime/service_generation/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/runtime/service_generation/signature_parsing/test_parsers.py` & `caikit-0.5.0/tests/runtime/service_generation/signature_parsing/test_parsers.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,98 +63,98 @@
 
 def test_get_output_type_name():
 
     # Test that if there's no function signature, use docstring to deduct output type
     empty_sign = inspect.Signature(return_annotation=inspect.Signature.empty)
     assert (
         get_output_type_name(
-            module_class=sample_lib.blocks.sample_task.SampleBlock,
+            module_class=sample_lib.modules.sample_task.SampleModule,
             fn_signature=empty_sign,
-            fn=sample_lib.blocks.sample_task.SampleBlock.run,
+            fn=sample_lib.modules.sample_task.SampleModule.run,
         )
         == sample_lib.data_model.SampleOutputType
     )
 
     # Test that we use type annotation to deduct output type
-    inner_block_run_method_ptr = getattr(
-        sample_lib.blocks.sample_task.InnerBlock, "run"
+    inner_module_run_method_ptr = getattr(
+        sample_lib.modules.sample_task.InnerModule, "run"
     )
-    fn_sign = inspect.signature(inner_block_run_method_ptr)
+    fn_sign = inspect.signature(inner_module_run_method_ptr)
     assert (
         get_output_type_name(
-            module_class=sample_lib.blocks.sample_task.InnerBlock,
+            module_class=sample_lib.modules.sample_task.InnerModule,
             fn_signature=fn_sign,
-            fn=sample_lib.blocks.sample_task.InnerBlock.run,
+            fn=sample_lib.modules.sample_task.InnerModule.run,
         )
         == sample_lib.data_model.SampleOutputType
     )
 
     # Test that we use type annotation to deduct output type is return annotation is a string
-    def _run(self, some_input: str) -> "InnerBlock":
+    def _run(self, some_input: str) -> "InnerModule":
         pass
 
     fn_sign = inspect.signature(_run)
     assert (
         get_output_type_name(
-            module_class=sample_lib.blocks.sample_task.InnerBlock,
+            module_class=sample_lib.modules.sample_task.InnerModule,
             fn_signature=fn_sign,
-            fn=sample_lib.blocks.sample_task.InnerBlock.run,
+            fn=sample_lib.modules.sample_task.InnerModule.run,
         )
-        == sample_lib.blocks.sample_task.InnerBlock
+        == sample_lib.modules.sample_task.InnerModule
     )
 
     # Test that we return None if type annotation as a string that doesn't match module class name
-    def _run2(self, some_input: str) -> "AStringThatsNotInnerBlock":
+    def _run2(self, some_input: str) -> "AStringThatsNotInnerModule":
         pass
 
     fn_sign = inspect.signature(_run2)
     assert (
         get_output_type_name(
-            module_class=sample_lib.blocks.sample_task.InnerBlock,
+            module_class=sample_lib.modules.sample_task.InnerModule,
             fn_signature=fn_sign,
-            fn=sample_lib.blocks.sample_task.InnerBlock.run,
+            fn=sample_lib.modules.sample_task.InnerModule.run,
         )
         == None
     )
 
     # User doesn't provide any type annotation or docstring, return None
     assert (
         get_output_type_name(
-            module_class=sample_lib.blocks.sample_task.InnerBlock,
+            module_class=sample_lib.modules.sample_task.InnerModule,
             fn_signature=empty_sign,
-            fn=sample_lib.blocks.sample_task.InnerBlock.run,
+            fn=sample_lib.modules.sample_task.InnerModule.run,
         )
         == None
     )
 
     # Test that if a ParseError was raised with docstring.parsers, we have no idea the type and return None
     with patch("docstring_parser.parse", side_effect=ParseError("mocked error")):
         assert (
             get_output_type_name(
-                module_class=sample_lib.blocks.sample_task.InnerBlock,
+                module_class=sample_lib.modules.sample_task.InnerModule,
                 fn_signature=empty_sign,
-                fn=sample_lib.blocks.sample_task.InnerBlock.run,
+                fn=sample_lib.modules.sample_task.InnerModule.run,
             )
             == None
         )
 
 
-def test_get_argument_types_with_real_block():
-    """Quick check that we get the right type for our sample block"""
+def test_get_argument_types_with_real_module():
+    """Quick check that we get the right type for our sample module"""
     assert (
-        get_argument_types(sample_lib.blocks.sample_task.SampleBlock.run)[
+        get_argument_types(sample_lib.modules.sample_task.SampleModule.run)[
             "sample_input"
         ]
         == sample_lib.data_model.SampleInputType
     )
 
     # Test that if a ParseError was raised with docstring.parsers, we could still parse from type annotation
     with patch("docstring_parser.parse", side_effect=ParseError("mocked error")):
         assert (
-            get_argument_types(sample_lib.blocks.sample_task.SampleBlock.run)[
+            get_argument_types(sample_lib.modules.sample_task.SampleModule.run)[
                 "sample_input"
             ]
             == sample_lib.data_model.SampleInputType
         )
 
     # Test that if a ParseError was raised with docstring.parsers, but no type annotation provided, we cannot deduct type and return None
     def run_fn(some_input: str, some_input_2):
```

### Comparing `caikit-0.4.4/tests/runtime/service_generation/test_create_service.py` & `caikit-0.5.0/tests/runtime/service_generation/test_create_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     create_inference_rpcs,
     create_training_rpcs,
 )
 import sample_lib
 
 ## Setup ########################################################################
 
-widget_class = sample_lib.blocks.sample_task.SampleBlock
-untrainable_module_class = sample_lib.blocks.sample_task.SamplePrimitiveBlock
+widget_class = sample_lib.modules.sample_task.SampleModule
+untrainable_module_class = sample_lib.modules.sample_task.SamplePrimitiveModule
 
 ## Tests ########################################################################
 
 ### create_inference_rpcs tests #################################################
 
 
 def test_create_inference_rpcs_for_module_with_no_run_function():
@@ -42,50 +42,38 @@
     rpcs = create_inference_rpcs([widget_class])
     assert len(rpcs) == 1
     assert widget_class in rpcs[0].module_list
 
 
 def test_create_inference_rpcs_for_multiple_modules_of_same_type():
     module_list = [
-        sample_lib.blocks.sample_task.SampleBlock,
-        sample_lib.blocks.sample_task.SamplePrimitiveBlock,
-        sample_lib.blocks.other_task.OtherBlock,
+        sample_lib.modules.sample_task.SampleModule,
+        sample_lib.modules.sample_task.SamplePrimitiveModule,
+        sample_lib.modules.other_task.OtherModule,
     ]
     rpcs = create_inference_rpcs(module_list)
 
     # only 2 RPCs, Widget and Gadget because SampleWidget and AnotherWidget are of the same module type Widget
     assert len(rpcs) == 2
-    assert sample_lib.blocks.sample_task.SampleBlock in rpcs[0].module_list
-    assert sample_lib.blocks.sample_task.SamplePrimitiveBlock in rpcs[0].module_list
-    assert sample_lib.blocks.other_task.OtherBlock in rpcs[1].module_list
-
-
-def test_create_inference_rpcs_with_block_and_workflow():
-    module_list = [
-        sample_lib.blocks.sample_task.SampleBlock,
-        sample_lib.workflows.sample_task.SampleWorkflow,
-    ]
-    rpcs = create_inference_rpcs(module_list)
-    # only 1 RPC
-    assert len(rpcs) == 1
-    assert sample_lib.blocks.sample_task.SampleBlock in rpcs[0].module_list
-    assert sample_lib.workflows.sample_task.SampleWorkflow in rpcs[0].module_list
+    assert sample_lib.modules.sample_task.SampleModule in rpcs[0].module_list
+    assert sample_lib.modules.sample_task.SamplePrimitiveModule in rpcs[0].module_list
+    assert sample_lib.modules.other_task.OtherModule in rpcs[1].module_list
 
 
 def test_create_inference_rpcs_remove_non_primitive_modules():
     # NOTE: This requires Gadget to be in config since other modules do not have methods - TODO fix?
     module_list = [
-        sample_lib.blocks.sample_task.SampleBlock,  # is a primitive module
-        sample_lib.blocks.sample_task.InnerBlock,  # not a primitive module
+        sample_lib.modules.sample_task.SampleModule,  # is a primitive module
+        sample_lib.modules.sample_task.InnerModule,  # not a primitive module
     ]
     rpcs = create_inference_rpcs(module_list)
 
     # only 1 RPC, fidget is not valid
     assert len(rpcs) == 1
-    assert sample_lib.blocks.sample_task.SampleBlock in rpcs[0].module_list
+    assert sample_lib.modules.sample_task.SampleModule in rpcs[0].module_list
 
 
 ### create_training_rpcs tests #################################################
 
 
 def test_create_inference_rpcs_for_module_with_no_train_function():
     class Foo:
```

### Comparing `caikit-0.4.4/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.5.0/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/runtime/service_generation/test_primitives.py` & `caikit-0.5.0/tests/runtime/service_generation/test_primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/runtime/service_generation/test_rpcs.py` & `caikit-0.5.0/tests/runtime/service_generation/test_rpcs.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 """Tests for the rpc objects that hold our in-memory representation of
 what an RPC for a service looks like"""
 # Standard
 import uuid
 
 # Local
-from caikit.core import BlockBase, TaskBase
+from caikit.core import ModuleBase, TaskBase
 from caikit.runtime.service_generation.rpcs import TaskPredictRPC
 from caikit.runtime.service_generation.signature_parsing import (
     CaikitCoreModuleMethodSignature,
 )
 from sample_lib.data_model import SampleOutputType, SampleTask
 import caikit.core
 
@@ -30,22 +30,22 @@
 def test_task_inference_rpc_with_all_optional_params():
     @caikit.core.task(
         required_parameters={"str_val": str}, output_type=SampleOutputType
     )
     class TestTask(TaskBase):
         pass
 
-    @caikit.core.block(
+    @caikit.core.module(
         id=str(uuid.uuid4()), name="testest", version="9.9.9", task=SampleTask
     )
-    class TestBlock(BlockBase):
+    class TestModule(ModuleBase):
         def run(self, str_val="I have a default"):
             pass
 
     rpc = TaskPredictRPC(
         task=("foo", "bar"),
-        method_signatures=[CaikitCoreModuleMethodSignature(TestBlock, "run")],
+        method_signatures=[CaikitCoreModuleMethodSignature(TestModule, "run")],
         primitive_data_model_types=[],
     )
 
     data_model = rpc.create_request_data_model(package_name="blah")
     assert data_model is not None
```

### Comparing `caikit-0.4.4/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.5.0/tests/runtime/service_generation/test_type_helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,9 +31,9 @@
     assert has_data_stream(Union[List[DataStream[int]], str])
 
     assert get_data_stream_type(Optional[DataStream[int]]) == DataStream[int]
     assert get_data_stream_type(Union[List[DataStream[str]], int]) == DataStream[str]
 
 
 def test_model_type_helpers():
-    assert is_model_type(sample_lib.blocks.sample_task.SampleBlock)
-    assert is_model_type(Union[str, sample_lib.blocks.sample_task.SampleBlock])
+    assert is_model_type(sample_lib.modules.sample_task.SampleModule)
+    assert is_model_type(Union[str, sample_lib.modules.sample_task.SampleModule])
```

### Comparing `caikit-0.4.4/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.5.0/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,46 +23,46 @@
 # Third Party
 import grpc
 import pytest
 
 # Local
 from caikit.runtime.servicers.global_predict_servicer import GlobalPredictServicer
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from sample_lib.blocks.sample_task import SampleBlock
 from sample_lib.data_model import SampleInputType, SampleOutputType
+from sample_lib.modules.sample_task import SampleModule
 from tests.fixtures import Fixtures
 import sample_lib
 
 HAPPY_PATH_INPUT = SampleInputType(name="Gabe").to_proto()
 HAPPY_PATH_RESPONSE = SampleOutputType(greeting="Hello Gabe").to_proto()
 
 
-def test_calling_predict_should_raise_if_block_raises(
+def test_calling_predict_should_raise_if_module_raises(
     sample_inference_service, sample_predict_servicer, loaded_model_id
 ):
     with pytest.raises(CaikitRuntimeException) as context:
-        # SampleBlocks will raise a RuntimeError if the throw flag is set
+        # SampleModules will raise a RuntimeError if the throw flag is set
         request = sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT, throw=True
         )
         sample_predict_servicer.Predict(
             request, Fixtures.build_context(loaded_model_id)
         )
     assert context.value.status_code == grpc.StatusCode.INTERNAL
     assert "Unhandled exception during prediction" in context.value.message
 
 
 def test_invalid_input_to_a_valid_caikit_core_class_method_raises(
     loaded_model_id, sample_inference_service, sample_predict_servicer
 ):
-    """Test that a caikit.core block that gets an unexpected input value errors in an expected way"""
+    """Test that a caikit.core module that gets an unexpected input value errors in an expected way"""
     with pytest.raises(CaikitRuntimeException) as context:
-        # SampleBlocks will raise a ValueError if the poison pill name is given
+        # SampleModules will raise a ValueError if the poison pill name is given
         request = sample_inference_service.messages.SampleTaskRequest(
-            sample_input=SampleInputType(name=SampleBlock.POISON_PILL_NAME).to_proto(),
+            sample_input=SampleInputType(name=SampleModule.POISON_PILL_NAME).to_proto(),
         )
         sample_predict_servicer.Predict(
             request, Fixtures.build_context(loaded_model_id)
         )
     assert context.value.status_code == grpc.StatusCode.INVALID_ARGUMENT
     assert "problem with your input" in context.value.message
 
@@ -163,15 +163,15 @@
             "batch_size",
             "model_type_counters",
             "container_id",
         ]
         assert data[0]["batch_size"] == 20
         assert len(data[0]["model_type_counters"]) == 1
         assert data[0]["model_type_counters"] == {
-            "<class 'sample_lib.blocks.sample_task.sample_implementation.SampleBlock'>": 20
+            "<class 'sample_lib.modules.sample_task.sample_implementation.SampleModule'>": 20
         }
     finally:
         sample_predict_servicer.rpc_meter.end_writer_thread()
 
 
 def test_metering_write_to_metrics_file_twice(
     sample_inference_service, loaded_model_id
@@ -209,11 +209,11 @@
             "batch_size",
             "model_type_counters",
             "container_id",
         ]
         assert data[0]["batch_size"] == 1
         assert len(data[0]["model_type_counters"]) == 1
         assert data[0]["model_type_counters"] == {
-            "<class 'sample_lib.blocks.sample_task.sample_implementation.SampleBlock'>": 1
+            "<class 'sample_lib.modules.sample_task.sample_implementation.SampleModule'>": 1
         }
     finally:
         sample_predict_servicer.rpc_meter.end_writer_thread()
```

### Comparing `caikit-0.4.4/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.5.0/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 
 # Third Party
 import pytest
 
 # Local
 from caikit.runtime.servicers.global_train_servicer import GlobalTrainServicer
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from sample_lib.blocks.sample_task.sample_implementation import SampleBlock
 from sample_lib.data_model.sample import (
     OtherOutputType,
     SampleInputType,
     SampleOutputType,
     SampleTrainingType,
 )
+from sample_lib.modules.sample_task.sample_implementation import SampleModule
 from tests.conftest import random_test_id, temp_config
 from tests.fixtures import Fixtures
 import caikit.core
 
 ## Helpers #####################################################################
 
 
@@ -84,15 +84,15 @@
     """
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
     model_name = random_test_id()
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name=model_name,
             batch_size=42,
             training_data=training_data,
         )
     )
 
     training_response = sample_train_servicer.Train(train_request)
@@ -101,16 +101,16 @@
     assert isinstance(training_response.training_id, str)
 
     result = sample_train_servicer.training_map.get(
         training_response.training_id
     ).result()
     assert result.batch_size == 42
     assert (
-        result.BLOCK_CLASS
-        == "sample_lib.blocks.sample_task.sample_implementation.SampleBlock"
+        result.MODULE_CLASS
+        == "sample_lib.modules.sample_task.sample_implementation.SampleModule"
     )
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     inference_response = sample_predict_servicer.Predict(
@@ -136,33 +136,35 @@
     """Global train of TrainRequest returns a training job with the correct
     model name, and some training id for a basic train function that doesn't
     require any loaded model
     """
     batch_size = 42
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceInt
     training_data = stream_type(jsondata=stream_type.JsonData(data=[1])).to_proto()
-    train_request = sample_train_service.messages.BlocksOtherTaskOtherBlockTrainRequest(
-        model_name="Other block Training",
-        training_data=training_data,
-        sample_input=SampleInputType(name="Gabe").to_proto(),
-        batch_size=batch_size,
+    train_request = (
+        sample_train_service.messages.ModulesOtherTaskOtherModuleTrainRequest(
+            model_name="Other module Training",
+            training_data=training_data,
+            sample_input=SampleInputType(name="Gabe").to_proto(),
+            batch_size=batch_size,
+        )
     )
 
     training_response = sample_train_servicer.Train(train_request)
-    assert training_response.model_name == "Other block Training"
+    assert training_response.model_name == "Other module Training"
     assert training_response.training_id is not None
     assert isinstance(training_response.training_id, str)
 
     result = sample_train_servicer.training_map.get(
         training_response.training_id
     ).result()
     assert result.batch_size == batch_size
     assert (
-        result.BLOCK_CLASS
-        == "sample_lib.blocks.other_task.other_implementation.OtherBlock"
+        result.MODULE_CLASS
+        == "sample_lib.modules.other_task.other_implementation.OtherModule"
     )
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     inference_response = sample_predict_servicer.Predict(
@@ -188,15 +190,15 @@
 ):
     """Global train of TrainRequest returns a training job with the correct model name, and some training id for a train function that requires another loaded model"""
     sample_model = caikit.interfaces.runtime.data_model.ModelPointer(
         model_id=loaded_model_id
     ).to_proto()
 
     training_request = (
-        sample_train_service.messages.WorkflowsSampleTaskSampleWorkflowTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskCompositeModuleTrainRequest(
             model_name="AnotherWidget_Training",
             sample_block=sample_model,
         )
     )
 
     training_response = sample_train_servicer.Train(training_request)
 
@@ -205,16 +207,16 @@
     assert isinstance(training_response.training_id, str)
 
     training_result = sample_train_servicer.training_map.get(
         training_response.training_id
     ).result()
 
     assert (
-        training_result.WORKFLOW_CLASS
-        == "sample_lib.workflows.sample_task.sample_implementation.SampleWorkflow"
+        training_result.MODULE_CLASS
+        == "sample_lib.modules.sample_task.composite_module.CompositeModule"
     )
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     # make sure the trained model can run inference
@@ -237,25 +239,25 @@
 ):
     """Check if run_train_job works as expected for syncronous requests"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name=random_test_id(),
             batch_size=42,
             training_data=training_data,
         )
     )
     servicer = GlobalTrainServicer(training_service=sample_train_service)
     with TemporaryDirectory() as tmp_dir:
         training_response = servicer.run_training_job(
             train_request,
-            SampleBlock,
+            SampleModule,
             training_id="dummy-training-id",
             training_output_dir=tmp_dir,
             wait=True,
         )
 
         assert training_response.training_id == "dummy-training-id"
 
@@ -276,28 +278,28 @@
 def test_run_train_job_works_with_no_autoload(sample_train_service):
     """Check if run_train_job works with no auto-load doesn't load model"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name=str(uuid.uuid4()),
             batch_size=42,
             training_data=training_data,
         )
     )
     servicer = GlobalTrainServicer(training_service=sample_train_service)
     servicer.auto_load_trained_model = False
     init_loaded_models_count = len(servicer._model_manager.loaded_models)
 
     with TemporaryDirectory() as tmp_dir:
         training_response = servicer.run_training_job(
             train_request,
-            SampleBlock,
+            SampleModule,
             training_id="dummy-training-id",
             training_output_dir=tmp_dir,
             wait=True,
         )
         assert training_response.training_id == "dummy-training-id"
         assert init_loaded_models_count == len(servicer._model_manager.loaded_models)
 
@@ -305,28 +307,28 @@
 def test_run_train_job_works_with_autoload(sample_train_service):
     """Check if run_train_job works with auto-load loading the model"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name=str(uuid.uuid4()),
             batch_size=42,
             training_data=training_data,
         )
     )
     servicer = GlobalTrainServicer(training_service=sample_train_service)
     servicer.auto_load_trained_model = True
     init_loaded_models_count = len(servicer._model_manager.loaded_models)
 
     with TemporaryDirectory() as tmp_dir:
         training_response = servicer.run_training_job(
             train_request,
-            SampleBlock,
+            SampleModule,
             training_id="dummy-training-id-2",
             training_output_dir=tmp_dir,
             wait=True,
         )
         assert training_response.training_id == "dummy-training-id-2"
         assert init_loaded_models_count < len(servicer._model_manager.loaded_models)
 
@@ -342,36 +344,36 @@
     """Global train of TrainRequest raises when calling a train function that requires another loaded model, but model is not loaded"""
     model_id = random_test_id()
 
     sample_model = caikit.interfaces.runtime.data_model.ModelPointer(
         model_id=model_id
     ).to_proto()
     request = (
-        sample_train_service.messages.WorkflowsSampleTaskSampleWorkflowTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskCompositeModuleTrainRequest(
             model_name="AnotherWidget_Training",
             sample_block=sample_model,
         )
     )
 
     with pytest.raises(CaikitRuntimeException) as context:
         sample_train_servicer.Train(request)
 
     assert f"Model '{model_id}' not loaded" == context.value.message
 
 
 def test_global_train_Edge_Case_Widget_should_raise_when_error_surfaces_from_block(
     sample_train_service, sample_train_servicer
 ):
-    """Test that if a block raises a ValueError, we should surface it to the user in a helpful way"""
+    """Test that if a module raises a ValueError, we should surface it to the user in a helpful way"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name=random_test_id(),
             batch_size=999,
             training_data=training_data,
         )
     )
     with pytest.raises(CaikitRuntimeException) as context:
         training_response = sample_train_servicer.Train(train_request)
@@ -382,21 +384,21 @@
 
     assert f"This may be a problem with your input" in str(context.value.message)
 
 
 def test_global_train_returns_exit_code_with_oom(
     sample_train_service, sample_train_servicer
 ):
-    """Test that if block goes into OOM we are able to surface error code"""
+    """Test that if module goes into OOM we are able to surface error code"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name=random_test_id(),
             batch_size=42,
             training_data=training_data,
             oom_exit=True,
         )
     )
```

### Comparing `caikit-0.4.4/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.5.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.5.0/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.5.0/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/runtime/test_grpc_server.py` & `caikit-0.5.0/tests/runtime/test_grpc_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,37 +134,37 @@
     )
     assert response.status == TrainingStatus.COMPLETED.value
 
     # Make sure we wait for training to finish
     result = TrainingManager.get_instance().training_futures[training_id].result()
 
     assert (
-        result.BLOCK_CLASS
-        == "sample_lib.blocks.sample_task.sample_implementation.SampleBlock"
+        result.MODULE_CLASS
+        == "sample_lib.modules.sample_task.sample_implementation.SampleModule"
     )
     # Fields with defaults have expected values
     assert result.batch_size == 64
     assert result.learning_rate == 0.0015
 
 
-def test_predict_fake_block_ok_response(
+def test_predict_fake_module_ok_response(
     loaded_model_id, runtime_grpc_server, sample_inference_service
 ):
     """Test RPC CaikitRuntime.WidgetPredict successful response"""
     stub = sample_inference_service.stub_class(runtime_grpc_server.make_local_channel())
     predict_request = sample_inference_service.messages.SampleTaskRequest(
         sample_input=HAPPY_PATH_INPUT
     )
     actual_response = stub.SampleTaskPredict(
         predict_request, metadata=[("mm-model-id", loaded_model_id)]
     )
     assert actual_response == HAPPY_PATH_RESPONSE
 
 
-def test_predict_fake_block_error_response(
+def test_predict_fake_module_error_response(
     runtime_grpc_server, sample_inference_service
 ):
     """Test RPC CaikitRuntime.WidgetPredict error response"""
     with pytest.raises(grpc.RpcError) as context:
         stub = sample_inference_service.stub_class(
             runtime_grpc_server.make_local_channel()
         )
@@ -174,34 +174,34 @@
         stub.SampleTaskPredict(
             predict_request, metadata=[("mm-model-id", "random_model_id")]
         )
     assert context.value.code() == grpc.StatusCode.NOT_FOUND
 
 
 ####### End-to-end tests for train a model and then predict with it
-def test_train_fake_block_ok_response_and_can_predict_with_trained_model(
+def test_train_fake_module_ok_response_and_can_predict_with_trained_model(
     train_stub,
     inference_stub,
     sample_train_service,
     sample_inference_service,
 ):
-    """Test RPC CaikitRuntime.BlocksSampleTaskSampleBlockTrain successful response"""
+    """Test RPC CaikitRuntime.ModulesSampleTaskSampleModuleTrain successful response"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(
             data=[SampleTrainingType(1), SampleTrainingType(2)]
         )
     ).to_proto()
     model_name = random_test_id()
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name=model_name, training_data=training_data
         )
     )
-    actual_response = train_stub.BlocksSampleTaskSampleBlockTrain(train_request)
+    actual_response = train_stub.ModulesSampleTaskSampleModuleTrain(train_request)
     is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name)
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     # make sure the trained model can run inference
@@ -210,32 +210,32 @@
     )
     inference_response = inference_stub.SampleTaskPredict(
         predict_request, metadata=[("mm-model-id", actual_response.model_name)]
     )
     assert inference_response == HAPPY_PATH_RESPONSE
 
 
-def test_train_fake_block_ok_response_with_loaded_model_can_predict_with_trained_model(
+def test_train_fake_module_ok_response_with_loaded_model_can_predict_with_trained_model(
     loaded_model_id,
     train_stub,
     inference_stub,
     sample_train_service,
     sample_inference_service,
 ):
     """Test RPC CaikitRuntime.WorkflowsSampleTaskSampleWorkflowTrain successful response with a loaded model"""
     sample_model = caikit.interfaces.runtime.data_model.ModelPointer(
         model_id=loaded_model_id
     ).to_proto()
     model_name = random_test_id()
     train_request = (
-        sample_train_service.messages.WorkflowsSampleTaskSampleWorkflowTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskCompositeModuleTrainRequest(
             model_name=model_name, sample_block=sample_model
         )
     )
-    actual_response = train_stub.WorkflowsSampleTaskSampleWorkflowTrain(train_request)
+    actual_response = train_stub.ModulesSampleTaskCompositeModuleTrain(train_request)
     is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name)
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     # make sure the trained model can run inference
@@ -244,36 +244,38 @@
     )
     inference_response = inference_stub.SampleTaskPredict(
         predict_request, metadata=[("mm-model-id", actual_response.model_name)]
     )
     assert inference_response == HAPPY_PATH_RESPONSE
 
 
-def test_train_fake_block_does_not_change_another_instance_model_of_block(
+def test_train_fake_module_does_not_change_another_instance_model_of_block(
     other_loaded_model_id,
     sample_int_file,
     train_stub,
     inference_stub,
     sample_train_service,
     sample_inference_service,
 ):
-    """This test: original "stock" OtherBlock model has batch size 42 (see fixtures/models/bar.yml),
-    we then train a custom OtherBlock model with batch size 100,
+    """This test: original "stock" OtherModule model has batch size 42 (see fixtures/models/bar.yml),
+    we then train a custom OtherModule model with batch size 100,
     then we make a predict to each, they should have the correct batch size"""
 
-    # Train an OtherBlock with batch size 100
+    # Train an OtherModule with batch size 100
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceInt
     training_data = stream_type(
         file=stream_type.File(filename=sample_int_file)
     ).to_proto()
 
-    train_request = sample_train_service.messages.BlocksOtherTaskOtherBlockTrainRequest(
-        model_name="Bar Training", batch_size=100, training_data=training_data
+    train_request = (
+        sample_train_service.messages.ModulesOtherTaskOtherModuleTrainRequest(
+            model_name="Bar Training", batch_size=100, training_data=training_data
+        )
     )
-    actual_response = train_stub.BlocksOtherTaskOtherBlockTrain(train_request)
+    actual_response = train_stub.ModulesOtherTaskOtherModuleTrain(train_request)
     is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, "Bar Training")
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     # make sure the trained model can run inference, and the batch size 100 was used
@@ -284,45 +286,45 @@
         predict_request, metadata=[("mm-model-id", actual_response.model_name)]
     )
     expected_trained_inference_response = OtherOutputType(
         farewell="goodbye: Gabe 100 times"
     ).to_proto()
     assert trained_inference_response == expected_trained_inference_response
 
-    # make sure the previously loaded OtherBlock model still has batch size 42
+    # make sure the previously loaded OtherModule model still has batch size 42
     original_inference_response = inference_stub.OtherTaskPredict(
         predict_request, metadata=[("mm-model-id", other_loaded_model_id)]
     )
     expected_original_inference_response = OtherOutputType(
         farewell="goodbye: Gabe 42 times"
     ).to_proto()
     assert original_inference_response == expected_original_inference_response
 
 
 ##### Test different datastream types #####
-def test_train_fake_block_ok_response_with_datastream_jsondata(
+def test_train_fake_module_ok_response_with_datastream_jsondata(
     train_stub, inference_stub, sample_train_service, sample_inference_service
 ):
-    """Test RPC CaikitRuntime.BlocksSampleTaskSampleBlockTrainRequest successful response with training data json type"""
+    """Test RPC CaikitRuntime.ModulesSampleTaskSampleModuleTrainRequest successful response with training data json type"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(
             data=[SampleTrainingType(1), SampleTrainingType(2)]
         )
     ).to_proto()
     model_name = random_test_id()
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name=model_name,
             batch_size=42,
             training_data=training_data,
         )
     )
 
-    actual_response = train_stub.BlocksSampleTaskSampleBlockTrain(train_request)
+    actual_response = train_stub.ModulesSampleTaskSampleModuleTrain(train_request)
     is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name)
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     # make sure the trained model can run inference
@@ -331,35 +333,35 @@
     )
     inference_response = inference_stub.SampleTaskPredict(
         predict_request, metadata=[("mm-model-id", actual_response.model_name)]
     )
     assert inference_response == HAPPY_PATH_RESPONSE
 
 
-def test_train_fake_block_ok_response_with_datastream_csv_file(
+def test_train_fake_module_ok_response_with_datastream_csv_file(
     train_stub,
     inference_stub,
     sample_train_service,
     sample_inference_service,
     sample_csv_file,
 ):
-    """Test RPC CaikitRuntime.BlocksSampleTaskSampleBlockTrainRequest successful response with training data file type"""
+    """Test RPC CaikitRuntime.ModulesSampleTaskSampleModuleTrainRequest successful response with training data file type"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         file=stream_type.File(filename=sample_csv_file)
     ).to_proto()
     model_name = random_test_id()
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name=model_name,
             training_data=training_data,
         )
     )
 
-    actual_response = train_stub.BlocksSampleTaskSampleBlockTrain(train_request)
+    actual_response = train_stub.ModulesSampleTaskSampleModuleTrain(train_request)
     is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name)
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     # make sure the trained model can run inference
@@ -369,29 +371,29 @@
     inference_response = inference_stub.SampleTaskPredict(
         predict_request, metadata=[("mm-model-id", actual_response.model_name)]
     )
     assert inference_response == HAPPY_PATH_RESPONSE
 
 
 #### Error cases for train tests #####
-def test_train_fake_block_error_response_with_unloaded_model(
+def test_train_fake_module_error_response_with_unloaded_model(
     train_stub, sample_train_service
 ):
     """Test RPC CaikitRuntime.WorkflowsSampleTaskSampleWorkflowTrain error response because sample model is not loaded"""
     with pytest.raises(grpc.RpcError) as context:
         sample_model = caikit.interfaces.runtime.data_model.ModelPointer(
             model_id=random_test_id()
         ).to_proto()
 
         train_request = (
-            sample_train_service.messages.WorkflowsSampleTaskSampleWorkflowTrainRequest(
+            sample_train_service.messages.ModulesSampleTaskCompositeModuleTrainRequest(
                 model_name=random_test_id(), sample_block=sample_model
             )
         )
-        train_stub.WorkflowsSampleTaskSampleWorkflowTrain(train_request)
+        train_stub.ModulesSampleTaskCompositeModuleTrain(train_request)
     assert context.value.code() == grpc.StatusCode.NOT_FOUND
 
 
 #### ModelRuntime tests ####
 def test_load_model_ok_response(runtime_grpc_server):
     """Test load model's successful response"""
     stub = model_runtime_pb2_grpc.ModelRuntimeStub(
@@ -724,15 +726,15 @@
                 "batch_size",
                 "model_type_counters",
                 "container_id",
             ]
             assert data[0]["batch_size"] == 1
             assert len(data[0]["model_type_counters"]) == 1
             assert data[0]["model_type_counters"] == {
-                "<class 'sample_lib.blocks.sample_task.sample_implementation.SampleBlock'>": 1
+                "<class 'sample_lib.modules.sample_task.sample_implementation.SampleModule'>": 1
             }
 
 
 def test_out_of_range_port(sample_inference_service):
     """Test that the server can use a port outside of the default 8888-9000
     range
     """
```

### Comparing `caikit-0.4.4/tests/runtime/test_service_factory.py` & `caikit-0.5.0/tests/runtime/test_service_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
 
 # Local
 import sample_lib
 
 MODULE_LIST = [
     module_class
-    for module_class in caikit.core.MODULE_REGISTRY.values()
+    for module_class in caikit.core.registries.module_registry().values()
     if module_class.__module__.partition(".")[0] == "sample_lib"
 ]
 
 ### Test ServicePackageFactory._get_and_filter_modules function
 def test_get_and_filter_modules_respects_excluded_task_type():
     with temp_config(
         {
@@ -204,71 +204,71 @@
         }
     ) as cfg:
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
         assert "sample_task" not in str(clean_modules)
 
 
 def test_get_and_filter_modules_respects_excluded_modules():
-    assert "InnerBlock" in str(MODULE_LIST)
+    assert "InnerModule" in str(MODULE_LIST)
     with temp_config(
         {
             "runtime": {
                 "service_generation": {
                     "module_guids": {
                         "excluded": ["00110203-baad-beef-0809-0a0b02dd0e0f"]
                     }
                 }
             }
-        }  # excluding InnerBlock
+        }  # excluding InnerModule
     ) as cfg:
 
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
-        assert "InnerBlock" not in str(clean_modules)
+        assert "InnerModule" not in str(clean_modules)
 
 
 def test_get_and_filter_modules_respects_excluded_modules_and_excluded_task_type():
-    assert "InnerBlock" in str(MODULE_LIST)
+    assert "InnerModule" in str(MODULE_LIST)
     with temp_config(
         {
             "runtime": {
                 "service_generation": {
                     "module_guids": {
                         "excluded": ["00110203-baad-beef-0809-0a0b02dd0e0f"]
                     },
                     "task_types": {"excluded": ["other_task"]},
                 }
             }
-        }  # excluding InnerBlock and OtherBlock
+        }  # excluding InnerModule and OtherModule
     ) as cfg:
 
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
-        assert "InnerBlock" not in str(clean_modules)
-        assert "OtherBlock" not in str(clean_modules)
+        assert "InnerModule" not in str(clean_modules)
+        assert "OtherModule" not in str(clean_modules)
         assert "other_task" not in str(clean_modules)
 
 
 def test_get_and_filter_modules_respects_included_modules_and_included_task_types():
     with temp_config(
         {
             "runtime": {
                 "service_generation": {
                     "module_guids": {
                         "included": ["00110203-baad-beef-0809-0a0b02dd0e0f"]
                     },
                     "task_types": {"included": ["other_task"]},
                 }
             }
-        }  # only want InnerBlock and OtherBlock
+        }  # only want InnerModule and OtherModule
     ) as cfg:
 
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
         assert len(clean_modules) == 2
-        assert "InnerBlock" in str(clean_modules)
-        assert "OtherBlock" in str(clean_modules)
-        assert "ListBlock" not in str(clean_modules)
+        assert "InnerModule" in str(clean_modules)
+        assert "OtherModule" in str(clean_modules)
+        assert "ListModule" not in str(clean_modules)
 
 
 def test_get_and_filter_modules_respects_included_modules():
     with temp_config(
         {
             "runtime": {
                 "service_generation": {
@@ -276,50 +276,50 @@
                         "included": [
                             "00110203-baad-beef-0809-0a0b02dd0e0f",
                             "00af2203-0405-0607-0263-0a0b02dd0c2f",
                         ]
                     },
                 }
             }
-        }  # only want InnerBlock and ListBlock
+        }  # only want InnerModule and ListModule
     ) as cfg:
 
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
         assert len(clean_modules) == 2
-        assert "InnerBlock" in str(clean_modules)
-        assert "ListBlock" in str(clean_modules)
-        assert "OtherBlock" not in str(clean_modules)
+        assert "InnerModule" in str(clean_modules)
+        assert "ListModule" in str(clean_modules)
+        assert "OtherModule" not in str(clean_modules)
 
 
 def test_get_and_filter_modules_respects_included_task_types():
     with temp_config(
         {
             "runtime": {
                 "service_generation": {
                     "task_types": {"included": ["sample_task"]},
                 }
             }
         }  # only want sample_task which has 6 modules
     ) as cfg:
 
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
-        assert "InnerBlock" in str(clean_modules)
-        assert "OtherBlock" not in str(clean_modules)
+        assert "InnerModule" in str(clean_modules)
+        assert "OtherModule" not in str(clean_modules)
 
 
 def test_get_and_filter_modules_respects_included_task_types_and_excluded_modules():
     with temp_config(
         {
             "runtime": {
                 "service_generation": {
                     "task_types": {"included": ["sample_task"]},
                     "module_guids": {
                         "excluded": ["00af2203-0405-0607-0263-0a0b02dd0c2f"]
                     },
                 }
             }
-        }  # only want sample_task but not ListBlock
+        }  # only want sample_task but not ListModule
     ) as cfg:
 
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
-        assert "InnerBlock" in str(clean_modules)
-        assert "ListBlock" not in str(clean_modules)
+        assert "InnerModule" in str(clean_modules)
+        assert "ListModule" not in str(clean_modules)
```

### Comparing `caikit-0.4.4/tests/runtime/utils/test_import_util.py` & `caikit-0.5.0/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/runtime/utils/test_servicer_util.py` & `caikit-0.5.0/tests/runtime/utils/test_servicer_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -211,53 +211,53 @@
 
 HAPPY_PATH_INPUT = SampleInputType(name="Gabe").to_proto()
 
 
 def test_global_predict_build_caikit_library_request_dict_creates_caikit_core_run_kwargs(
     sample_inference_service,
 ):
-    """Test that build_caikit_library_request_dict creates block run kwargs from RPC msg"""
+    """Test that build_caikit_library_request_dict creates module run kwargs from RPC msg"""
     request_dict = build_caikit_library_request_dict(
         sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT
         ),
-        sample_lib.blocks.sample_task.SampleBlock().run,
+        sample_lib.modules.sample_task.SampleModule().run,
     )
 
     # No self or "throw", throw was not set and the throw parameter contains a default value
     expected_arguments = {"sample_input"}
 
     assert expected_arguments == set(request_dict.keys())
     assert isinstance(request_dict["sample_input"], SampleInputType)
 
 
 def test_global_predict_build_caikit_library_request_dict_strips_invalid_run_kwargs_from_request(
     sample_inference_service,
 ):
     """Global predict build_caikit_library_request_dict strips invalid run kwargs from request"""
-    # Sample block doesn't take the `int_type` or `bool_type` params
+    # Sample module doesn't take the `int_type` or `bool_type` params
     request_dict = build_caikit_library_request_dict(
         sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT, int_type=5, bool_type=True
         ),
-        sample_lib.blocks.sample_task.SampleBlock().run,
+        sample_lib.modules.sample_task.SampleModule().run,
     )
 
     expected_arguments = {"sample_input"}
     assert expected_arguments == set(request_dict.keys())
     assert "int_type" not in request_dict.keys()
 
 
 def test_global_predict_build_caikit_library_request_dict_strips_empty_list_from_request(
     sample_inference_service,
 ):
     """Global predict build_caikit_library_request_dict strips empty list from request"""
     request_dict = build_caikit_library_request_dict(
         sample_inference_service.messages.SampleTaskRequest(int_type=5, list_type=[]),
-        sample_lib.blocks.sample_task.SamplePrimitiveBlock().run,
+        sample_lib.modules.sample_task.SamplePrimitiveModule().run,
     )
 
     assert "list_type" not in request_dict.keys()
     assert "int_type" in request_dict.keys()
 
 
 def test_global_predict_build_caikit_library_request_dict_works_for_non_optional_primitives():
@@ -336,25 +336,25 @@
     # self.assertTrue("repeated_message_field" in caikit.core_request)
     # self.assertIsInstance(caikit.core_request["repeated_message_field"], list)
 
 
 def test_global_train_build_caikit_library_request_dict_creates_caikit_core_run_kwargs_not_fail_when_optional_proto_field_not_exist(
     sample_train_service,
 ):
-    """Global train build_caikit_library_request_dict creates block run kwargs from RPC msg
+    """Global train build_caikit_library_request_dict creates module run kwargs from RPC msg
     and if not passed in request, it creates the fields with default values"""
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name=random_test_id()  # not having batch_size, and training_data
         )
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
-        sample_lib.blocks.sample_task.SampleBlock().train,
+        sample_lib.modules.sample_task.SampleModule().train,
     )
 
     expected_arguments = {"training_data"}
 
     # assert that even though not passed in, caikit.core_request now has training_data
     # because empty stream types get an empty steam initialized
     # TODO: will need additional tests for list arguments
@@ -369,22 +369,22 @@
 ):
     """Global train build_caikit_library_request_dict strips empty list from request"""
     # NOTE: not sure this test is relevant anymore, since nothing effectively gets removed?
     # the datastream is empty but it's not removed from request, which is expected
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(jsondata=stream_type.JsonData(data=[])).to_proto()
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name=random_test_id(), training_data=training_data
         )
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
-        sample_lib.blocks.sample_task.SampleBlock().train,
+        sample_lib.modules.sample_task.SampleModule().train,
     )
 
     # model_name is not expected to be passed through
     expected_arguments = {"training_data"}
 
     assert expected_arguments == set(caikit.core_request.keys())
 
@@ -392,23 +392,25 @@
 def test_global_train_build_caikit_library_request_dict_works_for_repeated_fields(
     sample_train_service,
 ):
     """Global train build_caikit_library_request_dict works for repeated fields"""
 
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(jsondata=stream_type.JsonData(data=[])).to_proto()
-    train_request = sample_train_service.messages.BlocksSampleTaskListBlockTrainRequest(
-        model_name=random_test_id(),
-        training_data=training_data,
-        poison_pills=["Bob Marley", "Bunny Livingston"],
+    train_request = (
+        sample_train_service.messages.ModulesSampleTaskListModuleTrainRequest(
+            model_name=random_test_id(),
+            training_data=training_data,
+            poison_pills=["Bob Marley", "Bunny Livingston"],
+        )
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
-        sample_lib.blocks.sample_task.ListBlock().train,
+        sample_lib.modules.sample_task.ListModule().train,
     )
 
     # model_name is not expected to be passed through
     expected_arguments = {"training_data", "poison_pills"}
 
     assert expected_arguments == set(caikit.core_request.keys())
     assert len(caikit.core_request.keys()) == 2
@@ -420,24 +422,26 @@
     sample_train_service,
 ):
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceInt
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[100, 120])
     ).to_proto()
 
-    train_request = sample_train_service.messages.BlocksOtherTaskOtherBlockTrainRequest(
-        model_name="Bar Training", batch_size=100, training_data=training_data
+    train_request = (
+        sample_train_service.messages.ModulesOtherTaskOtherModuleTrainRequest(
+            model_name="Bar Training", batch_size=100, training_data=training_data
+        )
     )
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
-        sample_lib.blocks.other_task.OtherBlock().train,
+        sample_lib.modules.other_task.OtherModule().train,
     )
 
     expected_arguments = set(
-        sample_lib.blocks.other_task.OtherBlock().train.__code__.co_varnames
+        sample_lib.modules.other_task.OtherModule().train.__code__.co_varnames
     )
     expected_arguments.remove("cls")
 
     assert expected_arguments == set(caikit.core_request.keys())
 
 
 def test_global_train_build_caikit_library_request_dict_ok_with_data_stream_file_type_csv(
@@ -446,23 +450,23 @@
     """Global train build_caikit_library_request_dict works for csv training data file"""
 
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         file=stream_type.File(filename=sample_csv_file)
     ).to_proto()
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name=random_test_id(),
             training_data=training_data,
         )
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
-        sample_lib.blocks.sample_task.SampleBlock().train,
+        sample_lib.modules.sample_task.SampleModule().train,
     )
 
     # model_name is not expected to be passed through
     expected_arguments = {"training_data"}
 
     assert expected_arguments == set(caikit.core_request.keys())
 
@@ -471,23 +475,25 @@
     sample_train_service, sample_csv_file, sample_json_file
 ):
     """Global train build_caikit_library_request_dict works for list of data files"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         listoffiles=stream_type.ListOfFiles(files=[sample_csv_file, sample_json_file])
     ).to_proto()
-    train_request = sample_train_service.messages.BlocksSampleTaskListBlockTrainRequest(
-        model_name=random_test_id(),
-        training_data=training_data,
-        poison_pills=["Bob Marley", "Bunny Livingston"],
+    train_request = (
+        sample_train_service.messages.ModulesSampleTaskListModuleTrainRequest(
+            model_name=random_test_id(),
+            training_data=training_data,
+            poison_pills=["Bob Marley", "Bunny Livingston"],
+        )
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
-        sample_lib.blocks.sample_task.ListBlock().train,
+        sample_lib.modules.sample_task.ListModule().train,
     )
 
     # model_name is not expected to be passed through
     expected_arguments = {"training_data", "poison_pills"}
 
     assert expected_arguments == set(caikit.core_request.keys())
     assert len(caikit.core_request.keys()) == 2
@@ -510,48 +516,48 @@
         stream_type = (
             caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
         )
         training_data = stream_type(
             directory=stream_type.Directory(dirname=tempdir, extension="json")
         ).to_proto()
         train_request = (
-            sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+            sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
                 model_name=random_test_id(),
                 training_data=training_data,
             )
         )
 
         # no error because at least 1 json file exists within the provided dir
         caikit.core_request = build_caikit_library_request_dict(
             train_request,
-            sample_lib.blocks.sample_task.SampleBlock().train,
+            sample_lib.modules.sample_task.SampleModule().train,
         )
 
 
 # ---------------- Error tests for build_caikit_library_request_dict --------------------
 
 
 def test_build_caikit_library_request_dict_raises_invalid_data_stream_source_file(
     sample_train_service,
 ):
     """Global train build_caikit_library_request_dict works for repeated fields"""
 
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(file=stream_type.File(filename="abc.blah")).to_proto()
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name=random_test_id(),
             training_data=training_data,
         )
     )
 
     with pytest.raises(CaikitRuntimeException) as e:
         caikit.core_request = build_caikit_library_request_dict(
             train_request,
-            sample_lib.blocks.sample_task.SampleBlock().train,
+            sample_lib.modules.sample_task.SampleModule().train,
         )
 
     assert "Invalid .blah data source file" in e.value.message
 
 
 def test_build_caikit_library_request_dict_raises_invalid_data_stream_source_file_ext(
     sample_train_service,
@@ -562,24 +568,24 @@
         handle.flush()
         fname = handle.name
         stream_type = (
             caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
         )
         training_data = stream_type(file=stream_type.File(filename=fname)).to_proto()
         train_request = (
-            sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+            sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
                 model_name="Foo Bar Training",
                 training_data=training_data,
             )
         )
 
         with pytest.raises(CaikitRuntimeException) as e:
             caikit.core_request = build_caikit_library_request_dict(
                 train_request,
-                sample_lib.blocks.sample_task.SampleBlock().train,
+                sample_lib.modules.sample_task.SampleModule().train,
             )
 
         assert "Extension not supported" in e.value.message
 
 
 def test_build_caikit_library_request_dict_raises_when_data_stream_file_passes_as_dir(
     sample_train_service, sample_csv_file
@@ -587,24 +593,24 @@
     """Global train build_caikit_library_request_dict raises for a file passed as directory"""
 
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         directory=stream_type.Directory(dirname=sample_csv_file)
     ).to_proto()
     train_request = (
-        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
             model_name="Foo Bar Training",
             training_data=training_data,
         )
     )
 
     with pytest.raises(CaikitRuntimeException) as e:
         caikit.core_request = build_caikit_library_request_dict(
             train_request,
-            sample_lib.blocks.sample_task.SampleBlock().train,
+            sample_lib.modules.sample_task.SampleModule().train,
         )
 
     assert "Invalid json directory source file" in e.value.message
 
 
 def test_build_caikit_library_request_dict_raises_when_data_stream_directory_passed_with_nonsupported_extension(
     sample_train_service,
@@ -619,24 +625,24 @@
         stream_type = (
             caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
         )
         training_data = stream_type(
             directory=stream_type.Directory(dirname=tempdir, extension="txt")
         ).to_proto()
         train_request = (
-            sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+            sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
                 model_name=random_test_id(),
                 training_data=training_data,
             )
         )
 
         with pytest.raises(CaikitRuntimeException) as e:
             caikit.core_request = build_caikit_library_request_dict(
                 train_request,
-                sample_lib.blocks.sample_task.SampleBlock().train,
+                sample_lib.modules.sample_task.SampleModule().train,
             )
 
         # TODO: change this message once it's implemented
         assert "Extension not supported!" in e.value.message
 
 
 def test_build_caikit_library_request_dict_raises_when_data_stream_directory_passed_with_incorrect_extension(
@@ -652,20 +658,20 @@
         stream_type = (
             caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
         )
         training_data = stream_type(
             directory=stream_type.Directory(dirname=tempdir, extension="json")
         ).to_proto()
         train_request = (
-            sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+            sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
                 model_name=random_test_id(),
                 training_data=training_data,
             )
         )
 
         with pytest.raises(CaikitRuntimeException) as e:
             caikit.core_request = build_caikit_library_request_dict(
                 train_request,
-                sample_lib.blocks.sample_task.SampleBlock().train,
+                sample_lib.modules.sample_task.SampleModule().train,
             )
 
         assert "contains no source files with extension" in e.value.message
```

### Comparing `caikit-0.4.4/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.5.0/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.5.0/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.5.0/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/tox.ini` & `caikit-0.5.0/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-0.4.4/PKG-INFO` & `caikit-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.4.4
+Version: 0.5.0
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.1.1,<2.0.0
 Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
 Requires-Dist: docstring-parser>=0.14.1,<0.16.0
 Requires-Dist: grpcio-health-checking>=1.35.0,<2.0
 Requires-Dist: grpcio>=1.35.0,<2.0
 Requires-Dist: ijson>=3.1.4,<3.3.0
+Requires-Dist: import-tracker>=3.1.5,<4
 Requires-Dist: munch>=2.5.0,<4.0
-Requires-Dist: protobuf>=3.19.0,<5
+Requires-Dist: numpy>=1.20,<2
 Requires-Dist: prometheus_client>=0.12.0,<1.0
+Requires-Dist: protobuf>=3.19.0,<5
 Requires-Dist: py-grpc-prometheus>=0.7.0,<0.8
+Requires-Dist: py-to-proto>=0.2.0,<0.3.0
 Requires-Dist: PyYAML>=6.0,<7.0
 Requires-Dist: requests>=2.26.0,<3.0
 Requires-Dist: semver>=2.13.0,<4.0
 Requires-Dist: six>=1.16.0,<2.0.0
 Requires-Dist: tqdm>=4.59.0,<5.0.0
-Requires-Dist: py-to-proto>=0.2.0,<0.3.0
-Requires-Dist: import-tracker>=3.1.5,<4
 Project-URL: Source, https://github.com/caikit/caikit
 
 # Caikit
 
 Caikit is an AI toolkit that enables users to manage models through a set of developer friendly APIs. It provides a consistent format for creating and using AI models against a wide variety of data domains and tasks.
 
 ![Caikit Overview](https://raw.githubusercontent.com/caikit/caikit/main/caikit-overview.png)
```

