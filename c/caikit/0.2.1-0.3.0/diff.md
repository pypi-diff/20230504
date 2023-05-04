# Comparing `tmp/caikit-0.2.1.tar.gz` & `tmp/caikit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.2.1.tar", last modified: Fri Apr 28 16:00:43 2023, max compression
+gzip compressed data, was "caikit-0.3.0.tar", last modified: Thu May  4 18:10:02 2023, max compression
```

## Comparing `caikit-0.2.1.tar` & `caikit-0.3.0.tar`

### file list

```diff
@@ -1,293 +1,305 @@
--rw-r--r--   0        0        0       60 2023-04-28 16:00:36.056088 caikit-0.2.1/.coveragerc
--rw-r--r--   0        0        0      676 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1272 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1141 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      212 2023-04-28 16:00:36.056088 caikit-0.2.1/.gitignore
--rw-r--r--   0        0        0      310 2023-04-28 16:00:36.056088 caikit-0.2.1/.isort.cfg
--rw-r--r--   0        0        0      370 2023-04-28 16:00:36.056088 caikit-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-04-28 16:00:36.056088 caikit-0.2.1/.prettierignore
--rw-r--r--   0        0        0       12 2023-04-28 16:00:36.056088 caikit-0.2.1/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-04-28 16:00:36.056088 caikit-0.2.1/.pylintrc
--rw-r--r--   0        0        0       78 2023-04-28 16:00:36.056088 caikit-0.2.1/.whitesource
--rw-r--r--   0        0        0     3358 2023-04-28 16:00:36.056088 caikit-0.2.1/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      336 2023-04-28 16:00:36.056088 caikit-0.2.1/CODEOWNERS
--rw-r--r--   0        0        0     7094 2023-04-28 16:00:36.056088 caikit-0.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-04-28 16:00:36.056088 caikit-0.2.1/LICENSE
--rw-r--r--   0        0        0     3757 2023-04-28 16:00:36.056088 caikit-0.2.1/README.md
--rw-r--r--   0        0        0    44878 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit-overview.png
--rw-r--r--   0        0        0      419 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/config/__init__.py
--rw-r--r--   0        0        0     5392 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/config/config.py
--rw-r--r--   0        0        0     6140 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/config/config.yml
--rw-r--r--   0        0        0     1770 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0      974 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/blocks/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/blocks/base.py
--rw-r--r--   0        0        0      962 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    29207 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     3962 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    13676 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     5340 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1471 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40187 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    20457 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/model_manager.py
--rw-r--r--   0        0        0    52621 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module.py
--rw-r--r--   0        0        0     6735 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_backend_config.py
--rw-r--r--   0        0        0      684 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     3399 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     1786 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     1493 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     5500 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_config.py
--rw-r--r--   0        0        0     6247 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_meta.py
--rw-r--r--   0        0        0      709 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/resources/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/resources/base.py
--rw-r--r--   0        0        0     1001 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    18059 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     4935 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1648 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32204 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0     1022 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/workflows/__init__.py
--rw-r--r--   0        0        0     9298 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/workflows/base.py
--rw-r--r--   0        0        0      530 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1377 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     2070 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1716 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    13996 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4659 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0     2370 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/metrics/throughput.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     6047 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12101 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4311 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1587 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    20071 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     3083 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5791 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    12221 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     7155 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0    10693 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/serializers.py
--rw-r--r--   0        0        0      666 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10744 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4911 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8181 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/parsers.py
--rw-r--r--   0        0        0     2571 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0    11938 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    15316 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5496 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1579 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6665 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    17900 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0     3693 2023-04-28 16:00:36.064088 caikit-0.2.1/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-04-28 16:00:36.064088 caikit-0.2.1/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-04-28 16:00:36.064088 caikit-0.2.1/docs/architecture_club/README.md
--rw-r--r--   0        0        0      837 2023-04-28 16:00:36.064088 caikit-0.2.1/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     1155 2023-04-28 16:00:39.252073 caikit-0.2.1/pyproject.toml
--rwxr-xr-x   0        0        0      720 2023-04-28 16:00:36.064088 caikit-0.2.1/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-04-28 16:00:36.064088 caikit-0.2.1/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     3572 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/base.py
--rw-r--r--   0        0        0        0 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/config/__init__.py
--rw-r--r--   0        0        0     4345 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/config/test_configs.py
--rw-r--r--   0        0        0     8462 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/blocks/__init__.py
--rw-r--r--   0        0        0    11631 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/blocks/test_base.py
--rw-r--r--   0        0        0        0 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     4559 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26013 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    13070 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    13533 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     1104 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     2909 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/helpers.py
--rw-r--r--   0        0        0     2320 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0      521 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/test_imports.py
--rw-r--r--   0        0        0    19262 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/test_model_manager.py
--rw-r--r--   0        0        0    17485 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/test_module.py
--rw-r--r--   0        0        0     5581 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/test_module_backend_config.py
--rw-r--r--   0        0        0     8529 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/test_module_metadata.py
--rw-r--r--   0        0        0     1038 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     7967 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    15068 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4972 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/workflows/__init__.py
--rw-r--r--   0        0        0    14580 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/workflows/test_base.py
--rw-r--r--   0        0        0     5655 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      498 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      106 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0     1016 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block.zip
--rw-r--r--   0        0        0      671 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block/data.pkl
--rw-r--r--   0        0        0      189 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block_backend/config.yml
--rw-r--r--   0        0        0      177 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block_foo/config.yml
--rw-r--r--   0        0        0      506 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block_no_nesting.zip
--rw-r--r--   0        0        0      566 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block_singleton/data.json
--rw-r--r--   0        0        0       14 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block_singleton/data.pkl
--rw-r--r--   0        0        0      222 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0      717 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_resource.zip
--rw-r--r--   0        0        0      230 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     1991 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_workflow.zip
--rw-r--r--   0        0        0      497 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_workflow/config.yml
--rw-r--r--   0        0        0      541 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_workflow/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_workflow/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_workflow/dummy_block/data.pkl
--rw-r--r--   0        0        0     3033 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      355 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      359 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      359 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_block/config.yml
--rw-r--r--   0        0        0      337 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      114 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/__init__.py
--rw-r--r--   0        0        0       88 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/other_task/__init__.py
--rw-r--r--   0        0        0     1847 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
--rw-r--r--   0        0        0      199 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
--rw-r--r--   0        0        0      616 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
--rw-r--r--   0        0        0     2283 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1276 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2662 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      410 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      141 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0      859 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0        0 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/resources/__init__.py
--rw-r--r--   0        0        0       58 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/resources/sample_type/__init__.py
--rw-r--r--   0        0        0       74 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/workflows/__init__.py
--rw-r--r--   0        0        0       58 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
--rw-r--r--   0        0        0     1687 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
--rw-r--r--   0        0        0        0 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3843 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0     6402 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/metrics/test_throughput.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14115 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    11607 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    18018 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5373 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0     5398 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     8595 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0     3768 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18336 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     4065 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/test_primitives.py
--rw-r--r--   0        0        0     1372 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     7923 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    15695 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3640 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7372 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4180 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    30069 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0    10935 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26086 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2807 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     1133 2023-04-28 16:00:36.072088 caikit-0.2.1/tox.ini
--rw-r--r--   0        0        0     4867 1970-01-01 00:00:00.000000 caikit-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-05-04 18:09:51.665948 caikit-0.3.0/.coveragerc
+-rw-r--r--   0        0        0      676 2023-05-04 18:09:51.665948 caikit-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-05-04 18:09:51.665948 caikit-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-05-04 18:09:51.665948 caikit-0.3.0/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-05-04 18:09:51.665948 caikit-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1272 2023-05-04 18:09:51.665948 caikit-0.3.0/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1141 2023-05-04 18:09:51.665948 caikit-0.3.0/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-05-04 18:09:51.665948 caikit-0.3.0/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      212 2023-05-04 18:09:51.665948 caikit-0.3.0/.gitignore
+-rw-r--r--   0        0        0      324 2023-05-04 18:09:51.665948 caikit-0.3.0/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-05-04 18:09:51.665948 caikit-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-05-04 18:09:51.665948 caikit-0.3.0/.prettierignore
+-rw-r--r--   0        0        0       12 2023-05-04 18:09:51.665948 caikit-0.3.0/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-05-04 18:09:51.665948 caikit-0.3.0/.pylintrc
+-rw-r--r--   0        0        0       78 2023-05-04 18:09:51.665948 caikit-0.3.0/.whitesource
+-rw-r--r--   0        0        0      336 2023-05-04 18:09:51.665948 caikit-0.3.0/CODEOWNERS
+-rw-r--r--   0        0        0     7165 2023-05-04 18:09:51.665948 caikit-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-05-04 18:09:51.665948 caikit-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3626 2023-05-04 18:09:51.665948 caikit-0.3.0/README.md
+-rw-r--r--   0        0        0      152 2023-05-04 18:09:51.665948 caikit-0.3.0/SECURITY.md
+-rw-r--r--   0        0        0    44878 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit-overview.png
+-rw-r--r--   0        0        0      419 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/config/__init__.py
+-rw-r--r--   0        0        0     5392 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/config/config.py
+-rw-r--r--   0        0        0     6140 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/config/config.yml
+-rw-r--r--   0        0        0     1786 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0      974 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/blocks/__init__.py
+-rw-r--r--   0        0        0     1552 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/blocks/base.py
+-rw-r--r--   0        0        0      999 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    28381 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2207 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     3962 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    12394 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     4736 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     1564 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40181 2023-05-04 18:09:51.665948 caikit-0.3.0/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    20457 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/model_manager.py
+-rw-r--r--   0        0        0    52621 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/module.py
+-rw-r--r--   0        0        0     6735 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/module_backend_config.py
+-rw-r--r--   0        0        0      684 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     3399 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     1786 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     1493 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     5500 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/module_config.py
+-rw-r--r--   0        0        0     6247 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/module_meta.py
+-rw-r--r--   0        0        0      709 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/resources/__init__.py
+-rw-r--r--   0        0        0     1212 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/resources/base.py
+-rw-r--r--   0        0        0     1001 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    18059 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1648 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32204 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0     1022 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/workflows/__init__.py
+-rw-r--r--   0        0        0     9298 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/core/workflows/base.py
+-rw-r--r--   0        0        0      530 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     1886 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    14200 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    16502 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4659 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     6047 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12101 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4311 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1480 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    20581 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     3083 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/service_generation/core_module_helpers.py
+-rw-r--r--   0        0        0     5791 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    13249 2023-05-04 18:09:51.669948 caikit-0.3.0/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     7155 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/service_generation/primitives.py
+-rw-r--r--   0        0        0    10710 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/service_generation/serializers.py
+-rw-r--r--   0        0        0      666 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10744 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/service_generation/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4794 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/service_generation/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8232 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/service_generation/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     2571 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     9473 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    15316 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5496 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1667 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6797 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    17900 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-05-04 18:09:51.673948 caikit-0.3.0/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0      169 2023-05-04 18:09:51.673948 caikit-0.3.0/code-of-conduct.md
+-rw-r--r--   0        0        0     1610 2023-05-04 18:09:51.673948 caikit-0.3.0/docs/adrs/010-data-model-definition.md
+-rw-r--r--   0        0        0     2352 2023-05-04 18:09:51.673948 caikit-0.3.0/docs/adrs/015-runtime-service-generation.md
+-rw-r--r--   0        0        0      181 2023-05-04 18:09:51.673948 caikit-0.3.0/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-05-04 18:09:51.673948 caikit-0.3.0/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-05-04 18:09:51.673948 caikit-0.3.0/docs/architecture_club/README.md
+-rw-r--r--   0        0        0      837 2023-05-04 18:09:51.673948 caikit-0.3.0/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     6095 2023-05-04 18:09:51.673948 caikit-0.3.0/examples/text-sentiment/README.md
+-rw-r--r--   0        0        0     1425 2023-05-04 18:09:51.673948 caikit-0.3.0/examples/text-sentiment/client.py
+-rw-r--r--   0        0        0      671 2023-05-04 18:09:51.673948 caikit-0.3.0/examples/text-sentiment/models/text_sentiment/config.yml
+-rw-r--r--   0        0        0       72 2023-05-04 18:09:51.673948 caikit-0.3.0/examples/text-sentiment/requirements.txt
+-rw-r--r--   0        0        0      961 2023-05-04 18:09:51.673948 caikit-0.3.0/examples/text-sentiment/start_runtime.py
+-rw-r--r--   0        0        0      816 2023-05-04 18:09:51.673948 caikit-0.3.0/examples/text-sentiment/text_sentiment/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-04 18:09:51.673948 caikit-0.3.0/examples/text-sentiment/text_sentiment/config.yml
+-rw-r--r--   0        0        0      661 2023-05-04 18:09:51.673948 caikit-0.3.0/examples/text-sentiment/text_sentiment/data_model/__init__.py
+-rw-r--r--   0        0        0     1372 2023-05-04 18:09:51.673948 caikit-0.3.0/examples/text-sentiment/text_sentiment/data_model/classification.py
+-rw-r--r--   0        0        0      643 2023-05-04 18:09:51.673948 caikit-0.3.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
+-rw-r--r--   0        0        0     3061 2023-05-04 18:09:51.673948 caikit-0.3.0/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py
+-rw-r--r--   0        0        0     1157 2023-05-04 18:09:58.482194 caikit-0.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0      720 2023-05-04 18:09:51.673948 caikit-0.3.0/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-05-04 18:09:51.673948 caikit-0.3.0/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3572 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/base.py
+-rw-r--r--   0        0        0        0 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/config/__init__.py
+-rw-r--r--   0        0        0     4345 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/config/test_configs.py
+-rw-r--r--   0        0        0     8462 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/blocks/__init__.py
+-rw-r--r--   0        0        0    11631 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/blocks/test_base.py
+-rw-r--r--   0        0        0        0 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     4559 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26013 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    13147 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    19079 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     1104 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     2909 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/helpers.py
+-rw-r--r--   0        0        0     2320 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0      521 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/test_imports.py
+-rw-r--r--   0        0        0    19262 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0    17485 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/test_module.py
+-rw-r--r--   0        0        0     5581 2023-05-04 18:09:51.673948 caikit-0.3.0/tests/core/test_module_backend_config.py
+-rw-r--r--   0        0        0     8529 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/core/test_module_metadata.py
+-rw-r--r--   0        0        0     1038 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     7967 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    15068 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4972 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/core/workflows/__init__.py
+-rw-r--r--   0        0        0    14580 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/core/workflows/test_base.py
+-rw-r--r--   0        0        0     5542 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      498 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      106 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0     1016 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_block.zip
+-rw-r--r--   0        0        0      671 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_block/data.pkl
+-rw-r--r--   0        0        0      189 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_block_backend/config.yml
+-rw-r--r--   0        0        0      177 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_block_foo/config.yml
+-rw-r--r--   0        0        0      506 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_block_no_nesting.zip
+-rw-r--r--   0        0        0      566 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_block_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_block_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_block_singleton/data.pkl
+-rw-r--r--   0        0        0      222 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0      717 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_resource.zip
+-rw-r--r--   0        0        0      230 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     1991 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_workflow.zip
+-rw-r--r--   0        0        0      497 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_workflow/config.yml
+-rw-r--r--   0        0        0      541 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_workflow/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_workflow/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/dummy_workflow/dummy_block/data.pkl
+-rw-r--r--   0        0        0     3033 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      376 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      355 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      359 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      422 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     2080 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/protobufs/caikit_runtime_pb2.py
+-rw-r--r--   0        0        0     2447 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2217 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
+-rw-r--r--   0        0        0     2602 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
+-rw-r--r--   0        0        0     5995 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0      416 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/protos/caikit_runtime.proto
+-rw-r--r--   0        0        0      437 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/protos/caikit_runtime_train.proto
+-rw-r--r--   0        0        0       24 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      359 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_block/config.yml
+-rw-r--r--   0        0        0      337 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      114 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/blocks/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/blocks/other_task/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
+-rw-r--r--   0        0        0      199 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
+-rw-r--r--   0        0        0      616 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
+-rw-r--r--   0        0        0     2405 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1276 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2662 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      410 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      141 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0      892 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0        0 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/resources/__init__.py
+-rw-r--r--   0        0        0       58 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/resources/sample_type/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/workflows/__init__.py
+-rw-r--r--   0        0        0       58 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
+-rw-r--r--   0        0        0     1687 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3843 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14115 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    11607 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    18018 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5373 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     5398 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/service_generation/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8668 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/service_generation/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0     3768 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18431 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     4065 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/service_generation/test_primitives.py
+-rw-r--r--   0        0        0     1372 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.677948 caikit-0.3.0/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     7923 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    15695 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     3640 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7372 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4204 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    30081 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0    10935 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26086 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2807 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3355 2023-05-04 18:09:51.681948 caikit-0.3.0/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     1133 2023-05-04 18:09:51.681948 caikit-0.3.0/tox.ini
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 caikit-0.3.0/PKG-INFO
```

### Comparing `caikit-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.3.0/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/.github/workflows/build-library.yml` & `caikit-0.3.0/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/.github/workflows/lint-code.yml` & `caikit-0.3.0/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/.github/workflows/publish-library.yml` & `caikit-0.3.0/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/.pylintrc` & `caikit-0.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/CONTRIBUTING.md` & `caikit-0.3.0/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Contributing
 
 👍🎉 First off, thank you for taking the time to contribute! 🎉👍
 
-The following is a set of guidelines for contributing. These are just guidelines, not rules. Use your best judgment, and feel free to propose changes to this document in a pull request. Please [read community contribution guide](TODO) for general practices for the Caikit community.
+The following is a set of guidelines for contributing. These are just guidelines, not rules. Use your best judgment, and feel free to propose changes to this document in a pull request. Please read the [community contribution guide](https://github.com/caikit/community/blob/main/CONTRIBUTING.md) first for general practices for the Caikit community.
 
 ## What Should I Know Before I Get Started?
 
 ### Code of Conduct
 
-This project adheres to the [Contributor Covenant](./CODE-OF-CONDUCT.md). By participating, you are expected to uphold this code.
+This project adheres to the [Contributor Covenant](./code-of-conduct.md). By participating, you are expected to uphold this code.
 
-Please report unacceptable behavior to one of the [Code Owners](./OWNERS).
+Please report unacceptable behavior to one of the [Code Owners](./CODEOWNERS).
 
 ### How Do I Start Contributing?
 
 The below workflow is designed to help you begin your first contribution journey. It will guide you through creating and picking up issues, working through them, having your work reviewed, and then merging.
 
 Help on open source projects is always welcome and there is always something that can be improved. For example, documentation (like the text you are reading now) can always use improvement, code can always be clarified, variables or functions can always be renamed or commented on, and there is always a need for more test coverage. If you see something that you think should be fixed, take ownership! Here is how you get started:
 
@@ -22,15 +22,15 @@
 
 When contributing, it's useful to start by looking at [issues](https://github.com/caikit/caikit/issues). After picking up an issue, writing code, or updating a document, make a pull request and your work will be reviewed and merged. If you're adding a new feature or find a bug, it's best to [write an issue](https://github.com/caikit/caikit/issues/new?assignees=&labels=&template=feature_request.md&title=) first to discuss it with maintainers.
 
 To contribute to this repo, you'll use the Fork and Pull model common in many open source repositories. For details on this process, check out [The GitHub Workflow
 Guide](https://github.com/kubernetes/community/blob/master/contributors/guide/github-workflow.md)
 from Kubernetes.
 
-When your contribution is ready, you can create a pull request. Pull requests are often referred to as "PR". In general, we follow the standard [github pull request](https://help.github.com/en/articles/about-pull-requests) process. Follow the template to provide details about your pull request to the maintainers.
+When your contribution is ready, you can create a pull request. Pull requests are often referred to as "PR". In general, we follow the standard [GitHub pull request](https://help.github.com/en/articles/about-pull-requests) process. Follow the template to provide details about your pull request to the maintainers.
 
 Before sending pull requests, make sure your changes pass formatting, linting and unit tests.
 
 #### Code Review
 
 Once you've [created a pull request](#how-can-i-contribute), maintainers will review your code and may make suggestions to fix before merging. It will be easier for your pull request to receive reviews if you consider the criteria the reviewers follow while working. Remember to:
```

### Comparing `caikit-0.2.1/LICENSE` & `caikit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/README.md` & `caikit-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -31,22 +31,14 @@
   - They bring data and tuning params to a pre-existing model architecture and create a new concrete model using APIs provided by Caikit
   - Examples of model authors are machine learning engineers, data scientists, and AI developers
 - AI Model Operator:
   - Model operators use an existing AI model to perform a specific function within the context of an application
   - They take trained models, deploy them, and then infer the models in applications through APIs provided by Caikit
   - Examples of operators are cloud and embedded application developers whose applications need analysis of unstructured data
 
-## AI Model Operator Quick Start
+## AI Model Operator Example
 
-**UNDER CONSTRUCTION**
-
-At this point, Caikit does not publish any pre-defined task implementations that can be readily consumed. Stay tuned!
-
-## AI Model Author Quick Start
-
-**UNDER CONSTRUCTION**
-
-We're getting a slim example ready, so stay tuned!
+Check out the [Text Sentiment example](examples/text-sentiment/) to understand how to load and infer a model using Caikit.
 
 ## Code of conduct
 
 Participation in the Caikit community is governed by the [Code of Conduct](CODE-OF-CONDUCT.md).
```

### Comparing `caikit-0.2.1/caikit-overview.png` & `caikit-0.3.0/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/config/__init__.py` & `caikit-0.3.0/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/config/config.py` & `caikit-0.3.0/caikit/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/config/config.yml` & `caikit-0.3.0/caikit/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/__init__.py` & `caikit-0.3.0/caikit/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 _warnings.filterwarnings("ignore")
 
 # Local
 # must import toolkit first since we need alog to be set up before it is used
 from . import blocks, data_model, module, module_config, resources, toolkit, workflows
 from .blocks.base import BlockBase, block
-from .data_model import dataobject
+from .data_model import DataObjectBase, dataobject
 from .model_manager import *
 from .module import *
 from .module_backend_config import configure as backend_configure
 from .module_backends import *
 from .module_config import ModuleConfig
 from .resources.base import ResourceBase, resource
 from .toolkit import *
```

### Comparing `caikit-0.2.1/caikit/core/augmentors/__init__.py` & `caikit-0.3.0/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/augmentors/base.py` & `caikit-0.3.0/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.3.0/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.3.0/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/augmentors/schemes/base.py` & `caikit-0.3.0/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.3.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.3.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/blocks/__init__.py` & `caikit-0.3.0/caikit/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/blocks/base.py` & `caikit-0.3.0/caikit/core/blocks/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/data_model/__init__.py` & `caikit-0.3.0/caikit/core/data_model/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,12 +14,17 @@
 
 
 """Common data model containing all data structures that are passed in and out of blocks.
 """
 
 # Local
 from . import base, data_backends, enums, producer, protobufs
-from .dataobject import CAIKIT_DATA_MODEL, dataobject, render_dataobject_protos
+from .dataobject import (
+    CAIKIT_DATA_MODEL,
+    DataObjectBase,
+    dataobject,
+    render_dataobject_protos,
+)
 from .enums import *
 from .producer import PACKAGE_COMMON, ProducerId
 from .streams import data_stream
 from .streams.data_stream import *
```

### Comparing `caikit-0.2.1/caikit/core/data_model/base.py` & `caikit-0.3.0/caikit/core/data_model/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 # metaclass-generated field members cannot be detected by pylint
 # pylint: disable=no-member
 
 # Standard
 from typing import Optional, Type, Union
 import base64
-import importlib
 import json
 
 # Third Party
 from google.protobuf import json_format
 from google.protobuf.descriptor import Descriptor
 from google.protobuf.message import Message as ProtoMessageType
 
@@ -50,213 +49,204 @@
     class_registry = {}
 
     # This sentinel value is used to determine whether a given attribute is
     # present on a class without doing `getattr` twice in the case where the
     # attribute does exist.
     _MISSING_ATTRIBUTE = "missing attribute"
 
+    # Special attribute used to communicate that the proto fields are forward
+    # declared and will be populated after the metaclass has completed
+    # construction.
+    _FWD_DECL_FIELDS = "__fwd_decl_fields__"
+
     def __new__(mcs, name, bases, attrs):
         """When constructing a new data model class, we set the 'fields' class variable from the
         protobufs descriptor and then set the '__slots__' magic class attribute to fields.  This
         provides two benefits: (a) performance is improved since the classes only need to know
         about these attributes (b) it helps to enforce that all member variables in these classes
         are described in the protobufs.
 
         Note:  If you want to add a variable for internal use that is not described in the
         protobufs, it can be named in the tuple class variable _private_slots and will
         automatically be added to __slots__.
         """
-        # get all fields in protobufs with same name as class,
+        # Get all fields in protobufs with same name as class,
         # except for DataBase, which has no matching protobufs
         fields = ()
 
-        # protobufs fields can be divided into these categories, which are used to automatically
+        # Protobufs fields can be divided into these categories, which are used to automatically
         # determine appropriate behavior in a number of methods
         fields_enum_map = {}
         fields_enum_rev = {}
         _fields_message = ()
         _fields_message_repeated = ()
         _fields_enum = ()
         _fields_enum_repeated = ()
         _fields_primitive = ()
         _fields_primitive_repeated = ()
         _fields_map = ()
         proto_class = None
         full_name = name
-        if name != "DataBase":
-            # Look for the proto class. There are two places it could be:
-            #
-            # 1. The "protobufs" module in caikit.core (injected via
-            #   import_protobufs)
-            # 2. The "protobufs" module in the derived library.
-            #
-            # The second option is primarily needed when using import_tracker on
-            # a caikit.core derived library. The side-effects of
-            # import_protobufs break the import_tracker mechanism, so this
-            # fallback avoids the reliance on side-effects.
+        if name not in ["DataBase", "DataObjectBase"]:
+            # Look for a precompiled proto class and if found, parse its
+            # descriptor
             proto_class = attrs.get("_proto_class")
-            if proto_class is None:
-                parent_mod = attrs.get("__module__")
-                log.debug3(
-                    "No proto class found in central registry for [%s]. Looking in [%s]",
-                    name,
-                    parent_mod,
+            if proto_class is not None:
+                fields = tuple(proto_class.DESCRIPTOR.fields_by_name)
+
+            # Otherwise, we need to get the fields from a "special" attribute
+            else:
+                fields = attrs.pop(mcs._FWD_DECL_FIELDS, None)
+                log.debug4(
+                    "Using dataclass forward declaration fields %s for %s", fields, name
                 )
-                if parent_mod is not None:
-                    parent_mod_name = parent_mod.rpartition(".")[0]
-                    if not parent_mod_name:
-                        log.debug3(
-                            "No parent module for data model declared outside library"
-                        )
-                    else:
-                        parent_mod_protos_name = ".".join(
-                            [parent_mod_name, "protobufs"]
-                        )
-                        try:
-                            parent_mod_protos = importlib.import_module(
-                                parent_mod_protos_name
-                            )
-                            proto_class = getattr(parent_mod_protos, name, None)
-                        except ImportError:
-                            log.debug3(
-                                "Could not find a protobufs module in [%s]: %s",
-                                parent_mod,
-                                parent_mod_protos_name,
-                            )
-
-            if proto_class is None:
-                raise AttributeError(
-                    f"Failed to find {name} in caikit.core.data_model.protobufs or derived "
-                    f"library protobufs"
+                error.value_check(
+                    "<COR49310991E>",
+                    fields is not None,
+                    name,
+                    msg="No proto class found for {}",
                 )
 
-            # all fields
-            fields += tuple(proto_class.DESCRIPTOR.fields_by_name)
-
-            # all fields of type map
-            _fields_map = tuple(
-                field.name
-                for field in proto_class.DESCRIPTOR.fields
-                if field.message_type and field.message_type.GetOptions().map_entry
-            )
-
-            # map from all enum fields to their enum classes
-            # note: enums are also primitives, these overlap
-            fields_enum_map = {
-                field.name: getattr(enums, field.enum_type.name)
-                for field in proto_class.DESCRIPTOR.fields
-                if field.enum_type is not None
-            }
-
-            fields_enum_rev = {
-                field.name: getattr(enums, field.enum_type.name + "Rev")
-                for field in proto_class.DESCRIPTOR.fields
-                if field.enum_type is not None
-            }
-
-            # all repeated fields
-            fields_repeated = tuple(
-                field.name
-                for field in proto_class.DESCRIPTOR.fields
-                if field.label == field.LABEL_REPEATED
-            )
-
-            # all messages, repeated or not
-            _fields_message_all = tuple(
-                field.name
-                for field in proto_class.DESCRIPTOR.fields
-                if field.type == field.TYPE_MESSAGE
-            )
-
-            # all enums, repeated or not
-            _fields_enum_all = tuple(
-                field.name
-                for field in proto_class.DESCRIPTOR.fields
-                if field.enum_type is not None
-            )
-
-            # all primitives, repeated or not
-            _fields_primitive_all = (
-                frozenset(fields)
-                .difference(_fields_map)
-                .difference(_fields_message_all)
-                .difference(_fields_enum_all)
-            )
-
-            # messages that are not repeated
-            _fields_message = frozenset(_fields_message_all).difference(fields_repeated)
-
-            # messages that are repeated
-            _fields_message_repeated = frozenset(fields_repeated).intersection(
-                _fields_message_all
-            )
-
-            _fields_enum = frozenset(_fields_enum_all).difference(fields_repeated)
-
-            _fields_enum_repeated = frozenset(_fields_enum_all).intersection(
-                fields_repeated
-            )
-
-            # primitives that are not repeated
-            _fields_primitive = frozenset(_fields_primitive_all).difference(
-                fields_repeated
-            )
-
-            # primitives that are repeated
-            _fields_primitive_repeated = frozenset(fields_repeated).intersection(
-                _fields_primitive_all
-            )
-
-            # use the fully qualified protobuf name to avoid conflicts with
-            # nested messages that have matching names
-            full_name = proto_class.DESCRIPTOR.full_name
-
-        # look if any private slots are declared as class variables
+        # Look if any private slots are declared as class variables
         private_slots = attrs.setdefault("_private_slots", ())
 
-        # class slots are fields + private slots, this prevents other
+        # Class slots are fields + private slots, this prevents other
         # member attributes from being set and also improves performance
         attrs["__slots__"] = tuple(
             [f"_{field}" for field in fields] + list(private_slots) + ["_backend"]
         )
 
-        # add properties that use the underlying backend
-        for field in fields:
-            attrs[field] = mcs._make_property_getter(field)
-
-        # If there is not already an __init__ function defined, make one
-        current_init = attrs.get("__init__")
-        if current_init is None or current_init is DataBase.__init__:
-            attrs["__init__"] = mcs._make_init(fields)
-
-        # set fields class variable for reference
+        # Set fields class variable for reference
         # these are valuable for validating attributes and
         # also for recursively converting to and from protobufs
         attrs["full_name"] = full_name
         attrs["fields"] = fields
         attrs["fields_enum_map"] = fields_enum_map
         attrs["fields_enum_rev"] = fields_enum_rev
+        attrs["_fields_map"] = _fields_map
         attrs["_fields_message"] = _fields_message
         attrs["_fields_message_repeated"] = _fields_message_repeated
         attrs["_fields_enum"] = _fields_enum
         attrs["_fields_enum_repeated"] = _fields_enum_repeated
         attrs["_fields_primitive"] = _fields_primitive
         attrs["_fields_primitive_repeated"] = _fields_primitive_repeated
-        attrs["_fields_map"] = _fields_map
         attrs["_proto_class"] = proto_class
+
         instance = super().__new__(mcs, name, bases, attrs)
 
-        # Update the global class and proto registries
-        if name != "DataBase":
-            mcs.class_registry[full_name] = instance
+        # If there's a valid proto class, perform proto descriptor parsing
+        if proto_class is not None:
+            mcs.parse_proto_descriptor(instance)
 
         # Return the constructed class instance
         return instance
 
     @classmethod
+    def parse_proto_descriptor(mcs, cls):
+        """Encapsulate the logic for parsing the protobuf descriptor here. This
+        allows the parsing to be done as a post-process after metaclass
+        initialization
+        """
+
+        # use the fully qualified protobuf name to avoid conflicts with
+        # nested messages that have matching names
+        cls.full_name = cls._proto_class.DESCRIPTOR.full_name
+
+        # all fields
+        cls.fields = tuple(cls._proto_class.DESCRIPTOR.fields_by_name)
+
+        # map from all enum fields to their enum classes
+        # note: enums are also primitives, these overlap
+        cls.fields_enum_map = {
+            field.name: getattr(enums, field.enum_type.name)
+            for field in cls._proto_class.DESCRIPTOR.fields
+            if field.enum_type is not None
+        }
+
+        cls.fields_enum_rev = {
+            field.name: getattr(enums, field.enum_type.name + "Rev")
+            for field in cls._proto_class.DESCRIPTOR.fields
+            if field.enum_type is not None
+        }
+
+        # all repeated fields
+        fields_repeated = tuple(
+            field.name
+            for field in cls._proto_class.DESCRIPTOR.fields
+            if field.label == field.LABEL_REPEATED
+        )
+
+        # all messages, repeated or not
+        _fields_message_all = tuple(
+            field.name
+            for field in cls._proto_class.DESCRIPTOR.fields
+            if field.type == field.TYPE_MESSAGE
+        )
+
+        # all enums, repeated or not
+        _fields_enum_all = tuple(
+            field.name
+            for field in cls._proto_class.DESCRIPTOR.fields
+            if field.enum_type is not None
+        )
+
+        # all fields of type map
+        cls._fields_map = tuple(
+            field.name
+            for field in cls._proto_class.DESCRIPTOR.fields
+            if field.message_type and field.message_type.GetOptions().map_entry
+        )
+
+        # all primitives, repeated or not
+        _fields_primitive_all = (
+            frozenset(cls.fields)
+            .difference(cls._fields_map)
+            .difference(_fields_message_all)
+            .difference(_fields_enum_all)
+        )
+
+        # messages that are not repeated
+        cls._fields_message = frozenset(_fields_message_all).difference(fields_repeated)
+
+        # messages that are repeated
+        cls._fields_message_repeated = frozenset(fields_repeated).intersection(
+            _fields_message_all
+        )
+
+        cls._fields_enum = frozenset(_fields_enum_all).difference(fields_repeated)
+
+        cls._fields_enum_repeated = frozenset(_fields_enum_all).intersection(
+            fields_repeated
+        )
+
+        # primitives that are not repeated
+        cls._fields_primitive = frozenset(_fields_primitive_all).difference(
+            fields_repeated
+        )
+
+        # primitives that are repeated
+        cls._fields_primitive_repeated = frozenset(fields_repeated).intersection(
+            _fields_primitive_all
+        )
+
+        # Update the global class and proto registries
+        # NOTE: Explicitly not respecting metaclass inheritance so single
+        #   registry shared for all
+        _DataBaseMetaClass.class_registry[cls.full_name] = cls
+
+        # Add properties that use the underlying backend
+        for field in cls.fields:
+            setattr(cls, field, mcs._make_property_getter(field))
+
+        # If there is not already an __init__ function defined, make one
+        current_init = cls.__init__
+        if current_init is None or current_init is DataBase.__init__:
+            setattr(cls, "__init__", mcs._make_init(cls.fields))
+
+    @classmethod
     def _make_property_getter(mcs, field):
         """This helper creates an @property attribute getter for the given field
 
         NOTE: This needs to live as a standalone function in order for the given
             field name to be properly bound to the closure for the attrs
         """
         private_name = f"_{field}"
@@ -301,33 +291,33 @@
             num_kwargs = len(kwargs)
             num_fields = len(fields)
             used_fields = []
 
             if num_args + num_kwargs > num_fields:
                 error(
                     "<COR71444420E>",
-                    ValueError(f"Too many arguments given. Args are: {fields}"),
+                    TypeError(f"Too many arguments given. Args are: {fields}"),
                 )
 
             if num_args > 0:  # Do a quick check for performance reason
                 for i, field_val in enumerate(args):
                     field_name = fields[i]
                     setattr(self, field_name, field_val)
                     used_fields.append(field_name)
 
             if num_kwargs > 0:  # Do a quick check for performance reason
                 for field_name, field_val in kwargs.items():
                     if field_name not in fields:
                         error(
-                            "<COR71444421E>", ValueError(f"Unknown field {field_name}")
+                            "<COR71444421E>", TypeError(f"Unknown field {field_name}")
                         )
                     elif field_name in used_fields:
                         error(
                             "<COR71444422E>",
-                            ValueError(f"Got multiple values for field {field_name}"),
+                            TypeError(f"Got multiple values for field {field_name}"),
                         )
                     setattr(self, field_name, field_val)
                     used_fields.append(field_name)
 
             # Default all unspecified fields to None
             if num_fields > 0:  # Do a quick check for performance reason
                 for field_name in fields:
@@ -577,15 +567,15 @@
                 subproto = getattr(proto, field)
                 for key, value in attr.items():
                     # If our values aren't primitives, the subproto will have a DESCRIPTOR;
                     # in this case we need to fill down recursively, i.e., this is a
                     # protobufs message map container
                     if hasattr(subproto[key], "DESCRIPTOR"):
                         value.fill_proto(subproto[key])
-                    # Otherwise we have a protobufs scala map container, and we can set the
+                    # Otherwise we have a protobufs scalar map container, and we can set the
                     # primitive value like a normal dictionary.
                     else:
                         subproto[key] = value
             elif (
                 field in self._fields_primitive_repeated
                 or field in self._fields_enum_repeated
             ):
```

### Comparing `caikit-0.2.1/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.3.0/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/data_model/data_backends/base.py` & `caikit-0.3.0/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.3.0/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/data_model/dataobject.py` & `caikit-0.3.0/caikit/core/data_model/dataobject.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,210 +14,201 @@
 
 """This module defines the @schema decorator which can be used to declare data
 model objects inline without manually defining the protobufs representation
 """
 
 
 # Standard
-from datetime import datetime
-from functools import update_wrapper
-from types import ModuleType
-from typing import Callable, Dict, List, Type, Union
-import importlib
-import sys
-import types
-import typing
+from enum import Enum
+from typing import Any, Callable, List, Type, Union, get_args, get_origin
+import dataclasses
 
 # Third Party
-from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal.enum_type_wrapper import EnumTypeWrapper
 
 # First Party
-from jtd_to_proto.jtd_to_proto import JTD_TO_PROTO_TYPES
-from jtd_to_proto.validation import is_valid_jtd
+from py_to_proto.dataclass_to_proto import DataclassConverter
 import alog
-import jtd_to_proto
+import py_to_proto
 
 # Local
 from ..toolkit.errors import error_handler
 from . import enums
 from .base import DataBase, _DataBaseMetaClass
-from .streams.data_stream import DataStream
 
 ## Globals #####################################################################
 
 log = alog.use_channel("SCHEMA")
 error = error_handler.get(log)
 
-# Type defs for input schemas to a dataobject
-_SCHEMA_VALUE_TYPE = Union[str, "_SCHEMA_VALUE_TYPE", Type[DataBase]]
-_SCHEMA_DEF_TYPE = Dict[str, _SCHEMA_VALUE_TYPE]
+# Common package prefix
+CAIKIT_DATA_MODEL = "caikit_data_model"
 
 # Registry of auto-generated protos so that they can be rendered to .proto
 _AUTO_GEN_PROTO_CLASSES = []
 
-# Reserved keywords in JTD
-_JTD_KEYWORDS = [
-    "elements",
-    "type",
-    "properties",
-    "enum",
-    "values",
-    "optionalProperties",
-    "additionalProperties",
-    "discriminator",
-]
-
-# Type defs for schemas passed to jtd_to_proto
-_JTD_VALUE_TYPE = Union[str, "_JTD_VALUE_TYPE", _descriptor.Descriptor]
-_JTD_DEF_TYPE = Dict[str, _JTD_VALUE_TYPE]
-
-# Python type -> jtd name
-_NATIVE_TYPE_TO_JTD = {
-    str: "string",
-    int: "int64",
-    float: "float64",
-    bytes: "bytes",
-    bool: "boolean",
-    datetime: "timestamp",
-}
+# Special attribute used to indicate which defaults are user provided
+_USER_DEFINED_DEFAULTS = "__user_defined_defaults__"
 
 ## Public ######################################################################
 
-# Common package prefix
-CAIKIT_DATA_MODEL = "caikit_data_model"
+
+class _DataObjectBaseMetaClass(_DataBaseMetaClass):
+    """This metaclass is used for the DataObject base class so that all data
+    objects can delay the creation of their proto class until after the
+    metaclass has been instantiated.
+    """
+
+    def __new__(mcs, name, bases, attrs):
+        """When instantiating a new DataObject class, the proto class will not
+        yet have been generated, but the set of fields will be known since the
+        class will be the raw input representation of a @dataclass
+        """
+
+        # Get the annotations that will go into the dataclass
+        if name != "DataObjectBase":
+            raw_field_names = attrs.get("__annotations__")
+            if raw_field_names is None:
+                raise TypeError(
+                    "All DataObjectBase classes must follow dataclass syntax"
+                )
+
+            # TODO: Sort out oneof field names
+            field_names = list(raw_field_names.keys())
+
+            # Add the forward declaration
+            attrs[_DataBaseMetaClass._FWD_DECL_FIELDS] = field_names
+
+        # Delegate to the base metaclass
+        return super().__new__(mcs, name, bases, attrs)
+
+
+class DataObjectBase(DataBase, metaclass=_DataObjectBaseMetaClass):
+    """A DataObject is a data model class that is backed by a @dataclass.
+
+    Data model classes that use the @dataobject decorator must derive from this
+    base class.
+    """
 
 
-def dataobject(
-    schema: _SCHEMA_DEF_TYPE,
-    package: str = CAIKIT_DATA_MODEL,
-) -> Callable[[Type], Type[DataBase]]:
-    """The @schema decorator can be used to define a Data Model object's schema
-    inline with the definition of the python class rather than needing to bind
-    to a pre-compiled protobufs class. For example:
-
-    @dataobject(
-        package="foo.bar",
-        schema={"foo": str, "bar": int},
-    )
-    class MyDataObject:
+def dataobject(*args, **kwargs) -> Callable[[Type], Type[DataBase]]:
+    """The @dataobject decorator can be used to define a Data Model object's
+    schema inline with the definition of the python class rather than needing to
+    bind to a pre-compiled protobufs class. For example:
+
+    @dataobject("foo.bar")
+    @dataclass
+    class MyDataObject(DataObjectBase):
         '''My Custom Data Object'''
+        foo: str
+        bar: int
 
     NOTE: The wrapped class must NOT inherit directly from DataBase. That
         inheritance will be added by this decorator, but if it is written
         directly, the metaclass that links protobufs to the class will be called
         before this decorator can auto-gen the protobufs class.
 
     Args:
-        schema:  _SCHEMA_DEF_TYPE
-            The full schema definition dict
         package:  str
             The package name to use for the generated protobufs class
 
     Returns:
         decorator:  Callable[[Type], Type[DataBase]]
             The decorator function that will wrap the given class
     """
 
     def decorator(cls: Type) -> Type[DataBase]:
         # Make sure that the wrapped class does NOT inherit from DataBase
         error.value_check(
             "<COR95184230E>",
-            not issubclass(cls, DataBase),
-            "{} should not directly inherit from DataBase when using @schema",
+            issubclass(cls, (DataObjectBase, Enum)),
             cls.__name__,
+            msg="{} must inherit from DataObjectBase/Enum when using @dataobject",
         )
 
-        # Create the message class from the schema
-        jtd_def = _to_jtd_schema(schema)
-        log.debug3("JTD Def for %s: %s", cls.__name__, jtd_def)
-        proto_class = jtd_to_proto.descriptor_to_message_class(
-            jtd_to_proto.jtd_to_proto(
+        # Add the package to the kwargs
+        kwargs.setdefault("package", package)
+
+        # If there's a schema in the keyword args, use jtd_to_proto
+        schema = kwargs.pop("schema", None)
+        if schema is not None:
+            log.debug("Using JTD To Proto")
+            kwargs.setdefault("validate_jtd", True)
+            descriptor = py_to_proto.jtd_to_proto(
                 name=cls.__name__,
-                package=package,
-                jtd_def=jtd_def,
+                jtd_def=schema,
+                **kwargs,
             )
-        )
-        # pylint: disable=unused-variable,global-variable-not-assigned
-        global _AUTO_GEN_PROTO_CLASSES
+        # If it's already a dataclass, convert it directly
+        else:
+            log.debug("Using dataclass/enum to proto on dataclass")
+
+            # If it's not an enum, fill in any missing field defaults as None
+            # and make sure it's a dataclass
+            if not issubclass(cls, Enum):
+                log.debug2("Wrapping data class %s", cls)
+                user_defined_defaults = {}
+                for annotation in getattr(cls, "__annotations__", {}):
+                    user_defined_default = getattr(cls, annotation, dataclasses.MISSING)
+                    if user_defined_default == dataclasses.MISSING:
+                        log.debug3("Filling in None default for %s.%s", cls, annotation)
+                        setattr(cls, annotation, None)
+                    else:
+                        user_defined_defaults[annotation] = user_defined_default
+                # If the current __init__ is auto-generated by dataclass, remove
+                # it so that a new one is created with the new defaults. This is
+                # a little hard to detect across different python versions, so
+                # the most reliable way is to assume that the only place
+                # __annotations__ are added to the __init__ function itself are
+                # in dataclass. If cls is either not a dataclass or is a
+                # dataclass with a non-default __init__, there will not be
+                # annotations
+                if getattr(cls.__init__, "__annotations__", None):
+                    log.debug3("Resetting default dataclass init")
+                    delattr(cls, "__init__")
+                cls = dataclasses.dataclass(cls)
+                setattr(cls, _USER_DEFINED_DEFAULTS, user_defined_defaults)
+
+            descriptor = _dataobject_to_proto(dataclass_=cls, **kwargs)
+
+        # Create the message class from the dataclass
+        proto_class = py_to_proto.descriptor_to_message_class(descriptor)
         _AUTO_GEN_PROTO_CLASSES.append(proto_class)
 
         # Add enums to the global enums module
         for enum_class in _get_all_enums(proto_class):
             log.debug2("Importing enum [%s]", enum_class.DESCRIPTOR.name)
             enums.import_enum(enum_class)
 
         # Declare the merged class that binds DataBase to the wrapped class with
         # this generated proto class
         if isinstance(proto_class, type):
-            wrapper_class = _make_data_model_class(proto_class, cls)
+            setattr(cls, "_proto_class", proto_class)
+            cls = _make_data_model_class(proto_class, cls)
         else:
-            ck_enum = enums.EnumBase(proto_class)
+            enums.import_enum(proto_class, cls)
+            setattr(cls, "_proto_enum", proto_class)
 
-            # Handling enums with the @dataobject decorator is quite tricky
-            # because unlike a message which is represented as a `class` in
-            # python, an enum is represented as an INSTANCE of a `class`. This
-            # means that the naive implementation of this decorator would apply
-            # to a `class`, but return an object that is NOT a `class` (e.g.
-            # isinstance(MyEnum, type) == False). This is bad for two distinct
-            # reasons:
-            #
-            # 1. It's confusing to see code written with a decorator around a
-            #   `class` and have the resulting thing NOT be a class
-            # 2. It makes it harder to add additional functionality to the Enum
-            #   by defining custom methods on your "enum class"
-            #
-            # To get around this, we need to "bind" the instance of the EnumBase
-            # to a net-new `class`! This class will function as a singleton
-            # wrapper around the EnumBase instance, but will allow the decorator
-            # to return a true `class` and allow user-defined methods on that
-            # class to persist through the decorator.
-            # pylint: disable=unused-variable
-            class EnumBindingMeta(type):
-                def __new__(mcs, name, bases, attrs):
-                    attrs.update(vars(ck_enum))
-                    for method in ["toYAML", "toJSON", "toDict"]:
-                        attrs[method] = getattr(ck_enum, method)
-                    attrs["_proto_enum"] = proto_class
-                    attrs["_singleton_inst"] = ck_enum
-                    bases = tuple(list(bases) + [_EnumBaseSentinel])
-                    return super().__new__(mcs, name, bases, attrs)
-
-                def __call__(cls):
-                    return ck_enum
-
-                def __str__(cls):
-                    return ck_enum.__str__()
-
-                def __repr__(cls):
-                    return ck_enum.__repr__()
-
-            class _Dummy(cls, metaclass=EnumBindingMeta):
-                pass
-
-            update_wrapper(_Dummy, cls, updated=())
-            wrapper_class = _Dummy
-
-        # Attach the proto class to the protobufs module
-        parent_mod_name = getattr(cls, "__module__", "").rpartition(".")[0]
-        log.debug2("Parent mod name: %s", parent_mod_name)
-        if parent_mod_name:
-            proto_mod_name = ".".join([parent_mod_name, "protobufs"])
-            try:
-                proto_mod = importlib.import_module(proto_mod_name)
-            except ImportError:
-                log.debug("Creating new protobufs module: %s", proto_mod_name)
-                proto_mod = ModuleType(proto_mod_name)
-                sys.modules[proto_mod_name] = proto_mod
-            setattr(proto_mod, cls.__name__, proto_class)
-
-        # Return the merged data class
-        return wrapper_class
+        # Return the decorated class
+        return cls
 
+    # If called without the function invocation, fill in the default argument
+    if args and callable(args[0]):
+        assert not kwargs, "This shouldn't happen!"
+        package = CAIKIT_DATA_MODEL
+        return decorator(args[0])
+
+    # Pull the package as an arg or a keyword arg
+    if args:
+        package = args[0]
+        if "package" in kwargs:
+            raise TypeError("Got multiple values for argument 'package'")
+    else:
+        package = kwargs.get("package", CAIKIT_DATA_MODEL)
     return decorator
 
 
 def render_dataobject_protos(interfaces_dir: str):
     """Write out protobufs files for all proto classes generated from dataobjects
     to the target interfaces directory
 
@@ -228,97 +219,63 @@
     for proto_class in _AUTO_GEN_PROTO_CLASSES:
         proto_class.write_proto_file(interfaces_dir)
 
 
 ## Implementation Details ######################################################
 
 
-class _EnumBaseSentinel:
-    """This base class is used to provide a common base class for enum warpper
-    classes so that they can be identified generically
-    """
+def _dataobject_to_proto(*args, **kwargs):
+    return _DataobjectConverter(*args, **kwargs).descriptor
 
 
-# pylint: disable=too-many-return-statements
-def _to_jtd_schema(
-    input_schema: _SCHEMA_DEF_TYPE, is_inside_properties_dict: bool = False
-) -> _JTD_DEF_TYPE:
-    """Recursive helper that will convert an input schema to a fully fleshed out
-    JTD schema
+class _DataobjectConverter(DataclassConverter):
+    """Augment the dataclass converter to be able to pull descriptors from
+    existing data objects
     """
-    try:
-        # Unwrap optional to base type if applicable
-        input_schema = _unwrap_optional_type(input_schema)
-
-        # If it's a reference to an EnumBase, de-alias to that enum's EnumDescriptor
-        # NOTE: This must come before the check for dict since EnumBase instances
-        #   are themselves dicts
-        if isinstance(input_schema, enums.EnumBase) or (
-            isinstance(input_schema, type)
-            and issubclass(input_schema, _EnumBaseSentinel)
-        ):
-            return {"type": input_schema._proto_enum.DESCRIPTOR}
-
-        if isinstance(input_schema, dict):
-            # If this dict is already a JTD schema, return it as is
-            if is_valid_jtd(input_schema, valid_types=JTD_TO_PROTO_TYPES.keys()):
-                return input_schema
-
-            # If the dict is structured as a JTD element already, recurse on the
-            # values
-            if any(keyword in input_schema for keyword in _JTD_KEYWORDS):
-                return {
-                    k: _to_jtd_schema(v, "properties" in k.lower())
-                    for k, v in input_schema.items()
-                }
-
-            # If not, assume it's a flat properties dict
-            # Check to make sure we don't re-wrap *properties
-            translated_dict = {k: _to_jtd_schema(v) for k, v in input_schema.items()}
-            return (
-                {"properties": translated_dict}
-                if not is_inside_properties_dict
-                else translated_dict
-            )
 
-        # If it's a reference to another data model object, de-alias to that
-        # object's underlying proto descriptor
-        if isinstance(input_schema, type) and issubclass(input_schema, DataBase):
-            return {"type": input_schema.get_proto_class().DESCRIPTOR}
-
-        # If it's a native type, wrap it as a "type" element
-        if input_schema in _NATIVE_TYPE_TO_JTD:
-            return {"type": _NATIVE_TYPE_TO_JTD[input_schema]}
-
-        # If it's a list or data stream, wrap it with "elements":
-        if typing.get_origin(input_schema) in [list, DataStream]:
-            # type_ could be caikit.core.data_model.streams.data_stream.DataStream[int]
-            return {"elements": _to_jtd_schema(typing.get_args(input_schema)[0])}
-
-        # All other cases are invalid!
-        raise ValueError(f"Invalid input schema: {input_schema}")
-
-    except ValueError:
-        log.error("Invalid schema: %s", input_schema)
-        raise
-
-
-def _unwrap_optional_type(type_: typing.Any) -> typing.Any:
-    """Unwrap an Optional[T] type, or return the type as-is if it is not an optional
-    NB: Optional[T] is expressed as Union[T, None]
-    This function checks for Unions of [T, None] and returns T, or raises if the union
-    contains more types, as those need to be handled differently (and are not yet supported)
-    """
-    if typing.get_origin(type_) != Union:
-        return type_
-    possible_types = set(typing.get_args(type_))
-    possible_types.discard(type(None))
-    if len(possible_types) == 1:
-        return list(possible_types)[0]
-    raise ValueError(f"Invalid input schema, cannot handle unions yet: {type_}")
+    def get_concrete_type(self, entry: Any) -> Any:
+        """Also include data model classes and enums as concrete types"""
+        unwrapped = self._resolve_wrapped_type(entry)
+        if (
+            isinstance(unwrapped, type)
+            and issubclass(unwrapped, DataBase)
+            and unwrapped._proto_class is not None
+        ) or hasattr(unwrapped, "_proto_enum"):
+            return entry
+        return super().get_concrete_type(entry)
+
+    def get_descriptor(self, entry: Any) -> Any:
+        """Unpack data model classes and enums to their descriptors"""
+        entry = self._resolve_wrapped_type(entry)
+        if isinstance(entry, type) and issubclass(entry, DataBase):
+            return entry._proto_class.DESCRIPTOR
+        proto_enum = getattr(entry, "_proto_enum", None)
+        if proto_enum is not None:
+            return proto_enum.DESCRIPTOR
+        return super().get_descriptor(entry)
+
+    def get_optional_field_names(self, entry: Any) -> List[str]:
+        """Get the names of any fields which are optional. This will be any
+        field that has a user-defined default or is marked as Optional[]
+        """
+        optional_fields = list(getattr(entry, _USER_DEFINED_DEFAULTS, {}))
+        for field_name, field in entry.__dataclass_fields__.items():
+            if (
+                field_name not in optional_fields
+                and self._is_python_optional(field.type) is not None
+            ):
+                optional_fields.append(field_name)
+        return optional_fields
+
+    @staticmethod
+    def _is_python_optional(entry: Any) -> Any:
+        """Detect if this type is a python optional"""
+        if get_origin(entry) is Union:
+            args = get_args(entry)
+            return type(None) in args
 
 
 def _get_all_enums(
     proto_class: Union[_message.Message, EnumTypeWrapper],
 ) -> List[EnumTypeWrapper]:
     """Given a generated proto class, recursively extract all enums"""
     all_enums = []
@@ -331,35 +288,36 @@
             all_enums.extend(
                 _get_all_enums(getattr(proto_class, nested_proto_descriptor.name))
             )
 
     return all_enums
 
 
-def _make_data_model_class(proto_class, wrapped_cls):
-    wrapper_cls = _DataBaseMetaClass(
-        wrapped_cls.__name__,
-        tuple([DataBase, wrapped_cls]),
-        {"_proto_class": proto_class, **wrapped_cls.__dict__},
-    )
-    update_wrapper(wrapper_cls, wrapped_cls, updated=())
+def _make_data_model_class(proto_class, cls):
+    if issubclass(cls, DataObjectBase):
+        _DataBaseMetaClass.parse_proto_descriptor(cls)
 
     # Recursively make all nested message wrappers
     for nested_message_descriptor in proto_class.DESCRIPTOR.nested_types:
         nested_message_name = nested_message_descriptor.name
         nested_proto_class = getattr(proto_class, nested_message_name)
         setattr(
-            wrapper_cls,
+            cls,
             nested_message_name,
             _make_data_model_class(
                 nested_proto_class,
-                types.new_class(nested_message_name),
+                _DataBaseMetaClass.__new__(
+                    _DataBaseMetaClass,
+                    name=nested_message_name,
+                    bases=(DataBase,),
+                    attrs={"_proto_class": getattr(proto_class, nested_message_name)},
+                ),
             ),
         )
     for nested_enum_descriptor in proto_class.DESCRIPTOR.enum_types:
         setattr(
-            wrapper_cls,
+            cls,
             nested_enum_descriptor.name,
             getattr(enums, nested_enum_descriptor.name),
         )
 
-    return wrapper_cls
+    return cls
```

### Comparing `caikit-0.2.1/caikit/core/data_model/producer.py` & `caikit-0.3.0/caikit/core/data_model/producer.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,33 +12,35 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Common data model objects used to identify the producer of a given output
 """
 
 # Local
-from .dataobject import CAIKIT_DATA_MODEL, dataobject
+from .dataobject import CAIKIT_DATA_MODEL, DataObjectBase, dataobject
 
 PACKAGE_COMMON = f"{CAIKIT_DATA_MODEL}.common"
 
 
-@dataobject(
-    {"name": str, "version": str},
-    package=PACKAGE_COMMON,
-)
-class ProducerId:
+@dataobject(PACKAGE_COMMON)
+class ProducerId(DataObjectBase):
     """Information about a data structure and the module that produced it."""
 
+    name: str
+    version: str
+
     def __add__(self, other):
         """Add two producer ids."""
         return ProducerId(name=" & ".join([self.name, other.name]), version="0.0.0")
 
     @classmethod
     def from_proto(cls, proto):
         """Overloaded implementation for efficiency vs base introspection"""
         return cls(proto.name, proto.version)
 
     def fill_proto(self, proto):
         """Overloaded implementation for efficiency vs base introspection"""
-        proto.name = self.name
-        proto.version = self.version
+        if self.name is not None:
+            proto.name = self.name
+        if self.version is not None:
+            proto.version = self.version
         return proto
```

### Comparing `caikit-0.2.1/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.3.0/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/data_model/streams/__init__.py` & `caikit-0.3.0/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/data_model/streams/converter.py` & `caikit-0.3.0/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.3.0/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/data_model/streams/data_stream.py` & `caikit-0.3.0/caikit/core/data_model/streams/data_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         Examples:
             For a JSON lines file that looks like:
                 {"name": "Gilbert", "wins": [["straight", "7♣"], ["one pair", "10♥"]]}
                 {"name": "Alexa", "wins": [["two pair", "4♠"], ["two pair", "9♠"]]}
                 {"name": "May", "wins": []}
                 {"name": "Deloise", "wins": [["three of a kind", "5♣"]]}
 
-            >>> jsonl_data_stream = DataStream.from_jsonl_array('sample.jsonl')
+            >>> jsonl_data_stream = DataStream.from_jsonl('sample.jsonl')
             >>> for data_item in jsonl_data_stream:
             >>>     print(data_item)
             {'name': 'Gilbert', 'wins': [['straight', '7♣'], ['one pair', '10♥']]}
             {'name': 'Alexa', 'wins': [['two pair', '4♠'], ['two pair', '9♠']]}
             {'name': 'May', 'wins': []}
             {'name': 'Deloise', 'wins': [['three of a kind', '5♣']]}
```

### Comparing `caikit-0.2.1/caikit/core/data_model/streams/resolver.py` & `caikit-0.3.0/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/data_model/streams/validator.py` & `caikit-0.3.0/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/model_manager.py` & `caikit-0.3.0/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/module.py` & `caikit-0.3.0/caikit/core/module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/module_backend_config.py` & `caikit-0.3.0/caikit/core/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/module_backends/__init__.py` & `caikit-0.3.0/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/module_backends/backend_types.py` & `caikit-0.3.0/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/module_backends/base.py` & `caikit-0.3.0/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/module_backends/local_backend.py` & `caikit-0.3.0/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/module_config.py` & `caikit-0.3.0/caikit/core/module_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/module_meta.py` & `caikit-0.3.0/caikit/core/module_meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/resources/__init__.py` & `caikit-0.3.0/caikit/core/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/resources/base.py` & `caikit-0.3.0/caikit/core/resources/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/toolkit/__init__.py` & `caikit-0.3.0/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/toolkit/compatibility.py` & `caikit-0.3.0/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/toolkit/errors/__init__.py` & `caikit-0.3.0/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.3.0/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.3.0/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/toolkit/fileio.py` & `caikit-0.3.0/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/toolkit/isa.py` & `caikit-0.3.0/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/toolkit/logging.py` & `caikit-0.3.0/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.3.0/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/toolkit/serializers.py` & `caikit-0.3.0/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/toolkit/wip_decorator.py` & `caikit-0.3.0/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/workflows/__init__.py` & `caikit-0.3.0/caikit/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/core/workflows/base.py` & `caikit-0.3.0/caikit/core/workflows/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/interfaces/__init__.py` & `caikit-0.3.0/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/interfaces/common/__init__.py` & `caikit-0.3.0/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.3.0/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/interfaces/common/data_model/producer.py` & `caikit-0.3.0/caikit/interfaces/common/data_model/producer.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,35 +8,42 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# Standard
+from typing import List
+
 # First Party
 import alog
 
 # Local
-from caikit.core.data_model import PACKAGE_COMMON, ProducerId, dataobject
+from caikit.core.data_model import (
+    PACKAGE_COMMON,
+    DataObjectBase,
+    ProducerId,
+    dataobject,
+)
 from caikit.core.toolkit.errors import error_handler
 
 log = alog.use_channel("DATAM")
 error = error_handler.get(log)
 
 
-@dataobject(
-    package=PACKAGE_COMMON,
-    schema={"producers": {"elements": ProducerId}},
-)
-class ProducerPriority:
+@dataobject(PACKAGE_COMMON)
+class ProducerPriority(DataObjectBase):
     """An ordered list of ProducerId structures in descending order of priority.
     This is used when handling conflicts between multiple producers of the same
     data structure.
     """
 
+    elements: List[ProducerId]
+
     def __init__(self, producers):
         """Construct a new ProducerPriority
 
         Args:
             producers:  list(ProducerId)
         """
         error.type_check_all("<COR01353088E>", ProducerId, producers=producers)
```

### Comparing `caikit-0.2.1/caikit/interfaces/runtime/__init__.py` & `caikit-0.3.0/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.3.0/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.3.0/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,75 +8,61 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# Standard
+from enum import Enum
+
 # First Party
 import alog
 
 # Local
+from caikit.core.data_model import DataObjectBase, dataobject
 from caikit.core.toolkit.wip_decorator import Action, WipCategory, work_in_progress
-import caikit.core
 
 log = alog.use_channel("MDLOPS")
 
+RUNTIME_PACKAGE = "caikit_data_model.runtime"
+
 
 @work_in_progress(action=Action.WARNING, category=WipCategory.BETA)
-@caikit.core.dataobject(
-    schema={"training_id": str},
-    package="caikit_data_model.runtime",
-)
-class TrainingInfoRequest:
-    pass
+@dataobject(RUNTIME_PACKAGE)
+class TrainingInfoRequest(DataObjectBase):
+    training_id: str
 
 
 @work_in_progress(action=Action.WARNING, category=WipCategory.BETA)
-@caikit.core.dataobject(
-    schema={"training_id": str, "model_name": str},
-    package="caikit_data_model.runtime",
-)
-class TrainingJob:
-    pass
+@dataobject(RUNTIME_PACKAGE)
+class TrainingJob(DataObjectBase):
+    training_id: str
+    model_name: str
 
 
 @work_in_progress(action=Action.WARNING, category=WipCategory.BETA)
-@caikit.core.dataobject(
-    schema={"model_id": str},
-    package="caikit_data_model.runtime",
-)
-class ModelPointer:
-    pass
+@dataobject(RUNTIME_PACKAGE)
+class ModelPointer(DataObjectBase):
+    model_id: str
 
 
 @work_in_progress(action=Action.WARNING, category=WipCategory.BETA)
-@caikit.core.dataobject(
-    {
-        "enum": [
-            "NOT_STARTED",
-            "HALTED",
-            "FAILED",
-            "DOWNLOADING",
-            "PROCESSING",
-            "STORING",
-            "COMPLETED",
-        ]
-    }
-)
-class TrainingStatus:
-    pass
+@dataobject(RUNTIME_PACKAGE)
+class TrainingStatus(Enum):
+    NOT_STARTED = 0
+    HALTED = 1
+    FAILED = 2
+    DOWNLOADING = 3
+    PROCESSING = 4
+    STORING = 5
+    COMPLETED = 6
 
 
 @work_in_progress(action=Action.WARNING, category=WipCategory.BETA)
-@caikit.core.dataobject(
-    schema={
-        "training_id": str,
-        "status": TrainingStatus,
-        "submission_timestamp": str,
-        "completion_timestamp": str,
-        "error_code": str,
-    },
-    package="caikit_data_model.runtime",
-)
-class TrainingInfoResponse:
-    pass
+@dataobject(RUNTIME_PACKAGE)
+class TrainingInfoResponse(DataObjectBase):
+    training_id: str
+    status: TrainingStatus
+    submission_timestamp: str
+    completion_timestamp: str
+    error_code: str
```

### Comparing `caikit-0.2.1/caikit/runtime/__init__.py` & `caikit-0.3.0/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/dump_services.py` & `caikit-0.3.0/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/grpc_server.py` & `caikit-0.3.0/caikit/runtime/grpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,29 +144,32 @@
         health_servicer = health.HealthServicer(
             experimental_non_blocking=True,
             experimental_thread_pool=futures.ThreadPoolExecutor(max_workers=1),
         )
         health_pb2_grpc.add_HealthServicer_to_server(health_servicer, self.server)
 
         # Listen on a unix socket as well for model mesh.
-        try:
-            self.server.add_insecure_port(
-                f"unix://{self.config.runtime.unix_socket_path}"
-            )
-            log.info(
-                "<RUN10001011I>",
-                "Caikit Runtime is communicating through address: unix://%s",
-                self.config.runtime.unix_socket_path,
-            )
-        except RuntimeError:
-            log.info(
-                "<RUN10001100I>",
-                "Binding failed for: unix://%s",
-                self.config.runtime.unix_socket_path,
-            )
+        if self.config.runtime.unix_socket_path and os.path.exists(
+            self.config.runtime.unix_socket_path
+        ):
+            try:
+                self.server.add_insecure_port(
+                    f"unix://{self.config.runtime.unix_socket_path}"
+                )
+                log.info(
+                    "<RUN10001011I>",
+                    "Caikit Runtime is communicating through address: unix://%s",
+                    self.config.runtime.unix_socket_path,
+                )
+            except RuntimeError:
+                log.info(
+                    "<RUN10001100I>",
+                    "Binding failed for: unix://%s",
+                    self.config.runtime.unix_socket_path,
+                )
 
         # Pull TLS config from app config, unless an explicit override was passed
         self.tls_config = (
             tls_config_override if tls_config_override else self.config.runtime.tls
         )
 
         if (
@@ -220,15 +223,15 @@
             self.port,
             self.config.runtime.server_thread_pool_size,
         )
 
         if blocking:
             self.server.wait_for_termination(None)
 
-    def interrupt(self, signal_):
+    def interrupt(self, signal_, _stack_frame):
         """Interrupt the server. Implements the interface for Python signal.signal
 
         Reference: https://docs.python.org/3/library/signal.html#signal.signal
         """
         log.info(
             "<RUN81000120I>",
             "Caikit Runtime received interrupt signal %s, shutting down",
@@ -351,15 +354,15 @@
         training_service: Optional[
             ServicePackage
         ] = ServicePackageFactory.get_service_package(
             ServicePackageFactory.ServiceType.TRAINING,
             service_source,
         )
     except CaikitRuntimeException as e:
-        log.error("Cannot stand up training service, disabling training: %s", e)
+        log.warning("Cannot stand up training service, disabling training: %s", e)
         training_service = None
 
     server = RuntimeGRPCServer(
         inference_service=inference_service,
         training_service=training_service,
         handle_terminations=handle_terminations,
     )
```

### Comparing `caikit-0.2.1/caikit/runtime/interceptors/__init__.py` & `caikit-0.3.0/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.3.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/metrics/__init__.py` & `caikit-0.3.0/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.3.0/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/model_management/__init__.py` & `caikit-0.3.0/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/model_management/batcher.py` & `caikit-0.3.0/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/model_management/loaded_model.py` & `caikit-0.3.0/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/model_management/model_loader.py` & `caikit-0.3.0/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/model_management/model_manager.py` & `caikit-0.3.0/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/model_management/model_sizer.py` & `caikit-0.3.0/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/model_management/training_manager.py` & `caikit-0.3.0/caikit/runtime/model_management/training_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,14 @@
 # Third Party
 import grpc
 
 # Local
 from caikit.interfaces.runtime.data_model import TrainingStatus
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 
-#
-# @dataclasses.dataclass
-# class TrainingStuff:
-#     status: TrainingStatus
-#     exception: Exception
-
 
 class TrainingManager:
     __instance: "TrainingManager" = None
 
     training_futures: Dict[str, Future]
 
     def __init__(self):
```

### Comparing `caikit-0.2.1/caikit/runtime/protobufs/__init__.py` & `caikit-0.3.0/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.3.0/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.3.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.3.0/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.3.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.3.0/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.3.0/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.3.0/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.3.0/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.3.0/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/service_factory.py` & `caikit-0.3.0/caikit/runtime/service_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,37 +11,46 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module is responsible for creating service objects for the runtime to consume"""
 # Standard
 from enum import Enum
 from types import ModuleType
-from typing import Callable, Dict, List, Set, Type
+from typing import Callable, Dict, List, Optional, Set, Type
+import copy
 import dataclasses
 import inspect
 
 # Third Party
 import google.protobuf.descriptor
 import google.protobuf.service
 import grpc
 
 # First Party
-from jtd_to_proto.json_to_service import (
+from py_to_proto.dataclass_to_proto import (  # NOTE: Imported from here for compatibility
+    Annotated,
+    FieldNumber,
+)
+from py_to_proto.json_to_service import (
     json_to_service,
     service_descriptor_to_client_stub,
     service_descriptor_to_server_registration_function,
     service_descriptor_to_service,
 )
 import aconfig
 import alog
 
 # Local
 from caikit import get_config
-from caikit.core import dataobject
 from caikit.core.data_model.base import DataBase
+from caikit.core.data_model.dataobject import (
+    DataObjectBase,
+    _DataObjectBaseMetaClass,
+    dataobject,
+)
 from caikit.core.module import ModuleBase
 from caikit.interfaces.runtime.data_model import (
     TrainingInfoRequest,
     TrainingInfoResponse,
 )
 from caikit.runtime import service_generation
 from caikit.runtime.service_generation.core_module_helpers import get_module_info
@@ -321,37 +330,40 @@
     ) -> List[Type[DataBase]]:
         """Dynamically create data model classes for the inputs to these RPCs"""
         data_model_classes = []
         for task in rpcs_list:
             properties = {
                 # triple e.g. ('caikit.interfaces.common.ProducerPriority', 'producer_id', 1)
                 # This does not take care of nested descriptors
-                triple[1]: triple[0]
+                triple[1]: Annotated[triple[0], FieldNumber(triple[2])]
                 for triple in task.request.triples
-                if triple[1] not in task.request.default_set
+                if triple[1] not in task.request.default_map
             }
             optional_properties = {
-                triple[1]: triple[0]
+                triple[1]: Annotated[Optional[triple[0]], FieldNumber(triple[2])]
                 for triple in task.request.triples
-                if triple[1] in task.request.default_set
-            }
-            schema = {
-                "properties": properties,
-                "optionalProperties": optional_properties,
+                if triple[1] in task.request.default_map
             }
+            attrs = copy.copy(task.request.default_map)
+            attrs["__annotations__"] = {**properties, **optional_properties}
 
-            if not schema:
-                # hacky hack hack: make sure we actually have a schema to generate
+            if not properties and optional_properties:
+                log.warning(
+                    "No arguments found for request %s. Cannot generate rpc",
+                    task.request.name,
+                )
                 continue
 
-            decorator = dataobject(
-                schema=schema,
-                package=package_name,
+            decorator = dataobject(package=package_name)
+            cls_ = _DataObjectBaseMetaClass.__new__(
+                _DataObjectBaseMetaClass,
+                name=task.request.name,
+                bases=(DataObjectBase,),
+                attrs=attrs,
             )
-            cls_ = type(task.request.name, (object,), {})
             decorated_cls = decorator(cls_)
             data_model_classes.append(decorated_cls)
 
         return data_model_classes
 
     @staticmethod
     def _create_service_json(
```

### Comparing `caikit-0.2.1/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.3.0/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/service_generation/core_module_helpers.py` & `caikit-0.3.0/caikit/runtime/service_generation/core_module_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/service_generation/create_service.py` & `caikit-0.3.0/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.3.0/caikit/runtime/service_generation/data_stream_source.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,39 +9,53 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
+from datetime import datetime
 from glob import glob
 from typing import Any, Optional, Type
 import os
 import sys
 
 # Third Party
 from google.protobuf.message import Message as ProtoMessageType
 import grpc
 
 # First Party
 import alog
 
 # Local
-from caikit.core.data_model import dataobject
 from caikit.core.data_model.base import DataBase
-from caikit.core.data_model.dataobject import _NATIVE_TYPE_TO_JTD
+from caikit.core.data_model.dataobject import (
+    DataObjectBase,
+    _DataObjectBaseMetaClass,
+    dataobject,
+)
 from caikit.core.data_model.streams.data_stream import DataStream
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 import caikit
 
 # This global holds the mapping of element types to their respective
 # DataStreamSource wrappers so that the same message is not recreated
 # unnecessarily
 _DATA_STREAM_SOURCE_TYPES = {}
 
+# Python type -> jtd name
+_NATIVE_TYPE_TO_JTD = {
+    str: "string",
+    int: "int64",
+    float: "float64",
+    bytes: "bytes",
+    bool: "boolean",
+    datetime: "timestamp",
+}
+
 log = alog.use_channel("DSTRM-SRC")
 
 
 class DataStreamSourceBase(DataStream):
     """This base class acts as a sentinel so that dynamically generated data
     stream source classes can be identified programmatically.
     """
@@ -204,67 +218,81 @@
         log.debug("Creating DataStreamSource[%s] -> %s", data_element_type, cls_name)
         element_type = (
             data_element_type.get_proto_class().DESCRIPTOR
             if isinstance(data_element_type, type)
             and issubclass(data_element_type, DataBase)
             else _NATIVE_TYPE_TO_JTD[data_element_type]
         )
-        data_object = dataobject(
-            schema={
-                "properties": {
-                    "data_stream": {
-                        "discriminator": "data_reference_type",
-                        "mapping": {
-                            "JsonData": {
-                                "properties": {
-                                    "data": {
-                                        "elements": {"type": element_type},
-                                    },
+        schema = {
+            "properties": {
+                "data_stream": {
+                    "discriminator": "data_reference_type",
+                    "mapping": {
+                        "JsonData": {
+                            "properties": {
+                                "data": {
+                                    "elements": {"type": element_type},
                                 },
                             },
-                            "File": {"properties": {"filename": {"type": "string"}}},
-                            "ListOfFiles": {
-                                "properties": {
-                                    "files": {
-                                        "elements": {"type": "string"},
-                                    },
+                        },
+                        "File": {"properties": {"filename": {"type": "string"}}},
+                        "ListOfFiles": {
+                            "properties": {
+                                "files": {
+                                    "elements": {"type": "string"},
                                 },
                             },
-                            "Directory": {
-                                "properties": {
-                                    "dirname": {"type": "string"},
-                                    "extension": {"type": "string"},
-                                }
-                            },
                         },
-                    }
+                        "Directory": {
+                            "properties": {
+                                "dirname": {"type": "string"},
+                                "extension": {"type": "string"},
+                            }
+                        },
+                    },
                 }
-            },
-            package="caikit_data_model.runtime",
-        )(
-            type(
-                cls_name,
-                (DataStreamSourceBase,),
-                {"ELEMENT_TYPE": data_element_type},
+            }
+        }
+        # TODO: Once full oneof support is implemented, this can move to using
+        #   the proper @dataclass style. In the meantime, the "schema" version
+        #   that uses JTD is still supported so that this oneof can be
+        #   dynamically declared. In order to make this work, the
+        #   _DataObjectBaseMetaClass needs to pre-know the right set of field
+        #   names for the oneof fields as if this were a dataclass. The values
+        #   of these annotations are unused since this will never be made into a
+        #   true @dataclass.
+        annotations = {
+            name.lower(): None
+            for name in schema["properties"]["data_stream"]["mapping"]
+        }
+        data_object = dataobject(schema=schema, package="caikit_data_model.runtime",)(
+            _DataObjectBaseMetaClass.__new__(
+                _DataObjectBaseMetaClass,
+                name=cls_name,
+                bases=(DataObjectBase, DataStreamSourceBase),
+                attrs={
+                    "ELEMENT_TYPE": data_element_type,
+                    "__annotations__": annotations,
+                },
             )
         )
         setattr(
             caikit.interfaces.common.data_model,
             cls_name,
             data_object,
         )
         setattr(
-            sys.modules[__name__],
+            sys.modules[data_object.__module__],
             cls_name,
             data_object,
         )
 
         # Add an init that sequences the initialization so that
         # DataStreamSourceBase is initialized after DataBase
-        orig_init = data_object.__init__
+        orig_init = _DataObjectBaseMetaClass._make_init(data_object.fields)
 
         def __init__(self, *args, **kwargs):
             orig_init(self, *args, **kwargs)
             DataStreamSourceBase.__init__(self)
 
         setattr(data_object, "__init__", __init__)
```

### Comparing `caikit-0.2.1/caikit/runtime/service_generation/primitives.py` & `caikit-0.3.0/caikit/runtime/service_generation/primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/service_generation/serializers.py` & `caikit-0.3.0/caikit/runtime/service_generation/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """
 This package has classes that will serialize a python interface to a protocol buffer interface.
 
 Typically used for `caikit.core.module`s that expose .train and .run functions.
 """
 # Standard
-from typing import Dict, List, Optional, Set, Tuple, Type, get_args
+from typing import Any, Dict, List, Optional, Tuple, Type, get_args
 import abc
 
 # First Party
 import alog
 
 # Local
 from . import primitives, type_helpers
@@ -180,15 +180,15 @@
         """
         self.task = task
         self._module_list = [method.module for method in method_signatures]
         self._method_signatures = method_signatures
 
         # Aggregate the argument signature types into a single parameters_dict
         parameters_dict = {}
-        default_parameters = set()
+        default_parameters = {}
         for method in method_signatures:
             default_parameters.update(method.default_parameters)
             primitive_arg_dict = primitives.to_primitive_signature(
                 method.parameters, primitive_data_model_types
             )
             for arg_name, arg_type in primitive_arg_dict.items():
                 current_val = parameters_dict.get(arg_name, arg_type)
@@ -244,21 +244,23 @@
 
 class _RequestMessage:
     """Helper class to create the input request message that wraps up the inputs
     for a given function. The request Contains N named data-model or primitive
     objects.
     """
 
-    def __init__(self, msg_name: str, params: Dict[str, Type], default_set: Set[str]):
+    def __init__(
+        self, msg_name: str, params: Dict[str, Type], default_map: Dict[str, Any]
+    ):
         """Initialize with the module class and the parsed parameters to the run
         function.
         """
         self.name = msg_name
         self.triples = []
-        self.default_set = default_set
+        self.default_map = default_map
 
         existing_fields = ApiFieldNames.get_fields_for_message(self.name)
 
         if len(existing_fields) > 0:
             last_used_number = max(existing_fields.values())
         else:
             last_used_number = 0
```

### Comparing `caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.3.0/caikit/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/docstrings.py` & `caikit-0.3.0/caikit/runtime/service_generation/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/module_signature.py` & `caikit-0.3.0/caikit/runtime/service_generation/signature_parsing/module_signature.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 name, return type and input parameters.
 
 This encapsulates a lot of custom logic used to parse input/output parameters, especially when it
 comes to the caikit core common data model.
 """
 
 # Standard
-from typing import Dict, Optional, Set, Type
+from typing import Any, Dict, Optional, Type
 import inspect
 
 # First Party
 import alog
 
 # Local
 from . import parsers
@@ -47,40 +47,37 @@
     through a list of candidate ways to determine the signature in order least-
     hacky to most-hacky:
 
     1. Look for a known type mapping based on the name of the argument
     2. Look for python type annotations
     3. Look for a default value and check its type
     4. Parse the docstring
-
-    Return types can also be inferred as "{module_type}Prediction" if the type cannot be
-    determined any other way.
     """
 
     def __init__(self, caikit_core_module: Type[ModuleBase], method_name: str):
         self._module = caikit_core_module
         self._method_name = method_name
 
         try:
             self._method_pointer = getattr(self._module, self._method_name)
-            self._default_set = parsers.get_args_with_defaults(self._method_pointer)
+            self._default_map = parsers.get_args_with_defaults(self._method_pointer)
             method_signature = inspect.signature(self._method_pointer)
             self._return_type = parsers.get_output_type_name(
                 self._module, method_signature, self._method_pointer
             )
 
             self._parameters = parsers.get_argument_types(self._method_pointer)
         except AttributeError:
             log.warning(
                 "Could not find method [%s] in this module",
                 self.method_name,
             )
             self._return_type = None
             self._parameters = None
-            self._default_set = set()
+            self._default_map = {}
 
     @property
     def module(self) -> Type[ModuleBase]:
         """The concrete caikit.core.ModuleBase type"""
         return self._module
 
     @property
@@ -96,17 +93,17 @@
     @property
     def parameters(self) -> Optional[Dict[str, Type]]:
         """A dictionary of the parameter names to their types, or None if the method does not
         exist"""
         return self._parameters
 
     @property
-    def default_parameters(self) -> Set[str]:
+    def default_parameters(self) -> Dict[str, Any]:
         """A set of all parameter names which have default values"""
-        return self._default_set
+        return self._default_map
 
 
 class CustomSignature(CaikitCoreModuleMethodSignature):
     """(TBD on new class)? Need something to hold an intentionally mutated representation of a
     method signature. This represents the extra indirection that lives in the runtime, between the
     service API and the actual method. For example: .train functions return a fully constructed
     module, but the runtime will invoke .train asynchronously and instead return some handle that
```

### Comparing `caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/parsers.py` & `caikit-0.3.0/caikit/runtime/service_generation/signature_parsing/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Contains functions that attempt to parse the I/O types of member methods on `caikit.core.module`s
 """
 # Standard
-from typing import Callable, Dict, List, Optional, Set, Type
+from typing import Any, Callable, Dict, List, Optional, Type
 import inspect
 
 # First Party
 import alog
 
 # Local
 from . import docstrings
@@ -91,26 +91,28 @@
     return {
         name: _get_argument_type(param, module_method)
         for name, param in method_signature.parameters.items()
         if name not in ["self", "args", "kwargs", "_", "__"]
     }
 
 
-def get_args_with_defaults(module_method: Callable) -> Set[str]:
-    """Get the names of all arguments that have a default value supplied.
+def get_args_with_defaults(module_method: Callable) -> Dict[str, Any]:
+    """Get the the mapping of all argument names that have defaults to their
+    default values.
+
     Args:
         module_method (Callable): A pointer to a method
 
     Returns:
-        Set[str]: A set of all parameter names which have a default value.
+        Dict[str: Any]: A set of all parameter names which have a default value.
             Empty if none have defaults or no parameters exist.
     """
     method_signature = inspect.signature(module_method)
     return {
-        param.name
+        param.name: param.default
         for param in method_signature.parameters.values()
         if param.default != inspect.Parameter.empty
     }
 
 
 # pylint: disable=too-many-return-statements
 @alog.logged_function(log.debug2)
```

### Comparing `caikit-0.2.1/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.3.0/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/servicers/__init__.py` & `caikit-0.3.0/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.3.0/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,31 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # Standard
 from importlib.metadata import version
-from typing import Type
 import traceback
 
 # Third Party
 from google.protobuf.descriptor import FieldDescriptor
 from grpc import StatusCode
 from prometheus_client import Counter, Summary
-import grpc
 
 # First Party
 import alog
 
 # Local
 from caikit import get_config
-from caikit.core import ModuleBase
 from caikit.runtime.metrics.rpc_meter import RPCMeter
-from caikit.runtime.metrics.throughput import Throughput
 from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.service_factory import ServicePackage
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils.import_util import clean_lib_names
 from caikit.runtime.utils.servicer_util import (
     build_caikit_library_request_dict,
     build_proto_response,
@@ -49,34 +45,24 @@
     ["grpc_request", "code", "model_id"],
 )
 PREDICT_FROM_PROTO_SUMMARY = Summary(
     "predict_from_proto_duration_seconds",
     "Histogram of predict request unmarshalling duration (in seconds)",
     ["grpc_request", "model_id"],
 )
-PREDICT_caikit_library_SUMMARY = Summary(
+PREDICT_CAIKIT_LIBRARY_SUMMARY = Summary(
     "predict_caikit_library_duration_seconds",
     "Histogram of predict Caikit Library run duration (in seconds)",
     ["grpc_request", "model_id"],
 )
 PREDICT_TO_PROTO_SUMMARY = Summary(
     "predict_to_proto_duration_seconds",
     "Histogram of predict response marshalling duration (in seconds)",
     ["grpc_request", "model_id"],
 )
-INPUT_SIZE_SUMMARY = Summary(
-    "input_code_points",
-    "Size of original text input in code points",
-    ["grpc_request", "model_id"],
-)
-THROUGHPUT_ESTIMATE_SUMMARY = Throughput(
-    "throughput_kilocodepoints_per_second",
-    "An estimate of per-model throughput",
-    ["grpc_request", "model_id"],
-)
 
 log = alog.use_channel("GP-SERVICR-I")
 
 # Protobuf non primitives
 # Ref: https://developers.google.com/protocol-buffers/docs/reference/cpp/google.protobuf.descriptor
 NON_PRIMITIVE_TYPES = [FieldDescriptor.TYPE_MESSAGE, FieldDescriptor.TYPE_ENUM]
 
@@ -166,35 +152,29 @@
                 with PREDICT_FROM_PROTO_SUMMARY.labels(
                     grpc_request=desc_name, model_id=model_id
                 ).time():
                     caikit_library_request = build_caikit_library_request_dict(
                         request, model.run
                     )
 
-                input_size_kchar = self.get_input_kchar(context)
-                INPUT_SIZE_SUMMARY.labels(
-                    grpc_request=desc_name, model_id=model_id
-                ).observe(input_size_kchar)
-
+                # NB: we previously recorded the size of the request, and timed this block to
+                # provide a rudimentary throughput metric of size / time
                 with alog.ContextLog(log.debug, inner_scope_name):
-                    with THROUGHPUT_ESTIMATE_SUMMARY.input_size(
-                        input_size_kchar
-                    ).labels(grpc_request=desc_name, model_id=model_id).time():
-                        with PREDICT_caikit_library_SUMMARY.labels(
-                            grpc_request=desc_name, model_id=model_id
-                        ).time():
-                            if self.use_abortable_threads:
-                                work = AbortableAction(
-                                    CallAborter(context),
-                                    model.run,
-                                    **caikit_library_request,
-                                )
-                                response = work.do()
-                            else:
-                                response = model.run(**caikit_library_request)
+                    with PREDICT_CAIKIT_LIBRARY_SUMMARY.labels(
+                        grpc_request=desc_name, model_id=model_id
+                    ).time():
+                        if self.use_abortable_threads:
+                            work = AbortableAction(
+                                CallAborter(context),
+                                model.run,
+                                **caikit_library_request,
+                            )
+                            response = work.do()
+                        else:
+                            response = model.run(**caikit_library_request)
 
                 # Marshall the response to the necessary return type
                 with PREDICT_TO_PROTO_SUMMARY.labels(
                     grpc_request=desc_name, model_id=model_id
                 ).time():
                     response_proto = build_proto_response(response)
 
@@ -249,46 +229,7 @@
             log.warning(log_dict)
             PREDICT_RPC_COUNTER.labels(
                 grpc_request=desc_name, code=StatusCode.INTERNAL.name, model_id=model_id
             ).inc()
             raise CaikitRuntimeException(
                 StatusCode.INTERNAL, "Unhandled exception during prediction"
             ) from e
-
-    def get_input_kchar(self, context):
-        input_size = get_metadata(context, self.INPUT_SIZE_KEY, required=False)
-        if input_size is not None:
-            try:
-                input_size_int = int(input_size)
-                return input_size_int / 1000.0
-            except ArithmeticError:
-                pass
-        return 0
-
-    @staticmethod
-    def _raise_on_wrong_rpc(
-        desc_name: str, response_type: Type, model_id: str, model: Type[ModuleBase]
-    ) -> None:
-        """
-        Raise if a model was used for the wrong RPC. This relies on our RPC naming conventions, and
-        protects us from failing to serialize the response later in the grpc server layer.
-        (If there's a better way to check whether response.to_proto() matches the current RPC spec,
-        maybe we should do that instead...)
-
-        Args:
-            desc_name (str): The name of the RPC that was called
-            response_type (Type): type(model.run())
-            model_id (str): the ID of the model that was used
-            model (Type[ModuleBase]): the actual model used
-
-        Returns:
-            None
-        """
-        expected_response_type_name = desc_name.replace("Request", "Prediction")
-        response_class_name = response_type.__name__
-        if expected_response_type_name != response_class_name:
-            log.error("Cannot return type %s from request %s", response_type, desc_name)
-            raise CaikitRuntimeException(
-                grpc.StatusCode.INVALID_ARGUMENT,
-                f"Wrong return type from model {model_id}. Expected type {expected_response_type_name} "  # pylint: disable=line-too-long
-                f"but found type {response_type}. Model is type: {type(model)}",
-            )
```

### Comparing `caikit-0.2.1/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.3.0/caikit/runtime/servicers/global_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.3.0/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.3.0/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.3.0/caikit/runtime/servicers/training_management_servicer.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,9 +36,12 @@
         self.training_manager = TrainingManager.get_instance()
 
     def GetTrainingStatus(self, request, context):  # pylint: disable=unused-argument
         """Missing associated documentation comment in .proto file."""
         training_info = TrainingInfoRequest.from_proto(request)
 
         return TrainingInfoResponse(
-            status=self.training_manager.get_training_status(training_info.training_id)
+            training_id=training_info.training_id,
+            status=self.training_manager.get_training_status(
+                training_info.training_id
+            ).value,
         ).to_proto()
```

### Comparing `caikit-0.2.1/caikit/runtime/types/__init__.py` & `caikit-0.3.0/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/types/aborted_exception.py` & `caikit-0.3.0/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.3.0/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.3.0/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/utils/__init__.py` & `caikit-0.3.0/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/utils/import_util.py` & `caikit-0.3.0/caikit/runtime/utils/import_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,17 @@
     else:
         module_path = module_name
     log.info("<RUN11997772I>", "Loading service module: %s", module_path)
     # Try to find the spec for the module that we're interested in.
     spec = importlib.util.find_spec(module_path)
     if not spec:
         message = "Unable to find spec for module: %s" % (module_path)
-        log.error("<RUN11991313E>", message)
+        # TODO: figure out the better way of doing this
+        # https://github.com/caikit/caikit/pull/85#discussion_r1182890609
+        log.warning("<RUN11991313W>", message)
         raise CaikitRuntimeException(StatusCode.NOT_FOUND, message)
     # Found spec - import the library
     if module_dir:
         return importlib.import_module(module_path)
 
     return importlib.import_module(module_path, "*")
```

### Comparing `caikit-0.2.1/caikit/runtime/utils/servicer_util.py` & `caikit-0.3.0/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/work_management/__init__.py` & `caikit-0.3.0/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/work_management/abortable_action.py` & `caikit-0.3.0/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/work_management/call_aborter.py` & `caikit-0.3.0/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.3.0/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/docs/architecture_club/04-25-23.md` & `caikit-0.3.0/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/examples/start_runtime_with_sample_lib.py` & `caikit-0.3.0/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/pyproject.toml` & `caikit-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.2.1"
+version = "0.3.0"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
@@ -19,20 +19,20 @@
     "anytree>=2.7.0,<3.0",
     "docstring-parser>=0.14.1,<0.15.0",
     "grpcio-health-checking>=1.35.0,<2.0",
     "grpcio>=1.35.0,<2.0",
     "ijson>=3.1.4,<3.3.0",
     "munch>=2.5.0,<3.0",
     "protobuf>=3.19.0,<5",
-    "prometheus_client==0.12.0",
+    "prometheus_client>=0.12.0,<1.0",
     "py-grpc-prometheus>=0.7.0,<0.8",
     "PyYAML>=6.0,<7.0",
     "requests>=2.26.0,<3.0",
     "semver>=2.13.0,<4.0",
     "six>=1.16.0,<2.0.0",
     "tqdm>=4.59.0,<5.0.0",
-    "jtd-to-proto>=0.12.1,<0.13.0",
+    "py-to-proto>=0.1.2,<0.2.0",
     "import-tracker>=3.1.5,<4",
 ]
 
 [project.urls]
 Source = "https://github.com/caikit/caikit"
```

### Comparing `caikit-0.2.1/scripts/fmt.sh` & `caikit-0.3.0/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/__init__.py` & `caikit-0.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/base.py` & `caikit-0.3.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/config/test_configs.py` & `caikit-0.3.0/tests/config/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/conftest.py` & `caikit-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.3.0/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.3.0/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/blocks/__init__.py` & `caikit-0.3.0/tests/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/blocks/test_base.py` & `caikit-0.3.0/tests/core/blocks/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.3.0/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/data_model/streams/test_converter.py` & `caikit-0.3.0/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.3.0/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.3.0/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/data_model/streams/test_resolver.py` & `caikit-0.3.0/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/data_model/streams/test_validator.py` & `caikit-0.3.0/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/data_model/test_base.py` & `caikit-0.3.0/tests/core/data_model/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
                     class Object(base.DataBase):
                         def __init__(self, foo):
                             self.foo = foo
                     """
                 )
             )
 
-        # Make sure an AttributeError is raised when the import is tried
-        with pytest.raises(AttributeError):
+        # Make sure an ValueError is raised when the import is tried
+        with pytest.raises(ValueError):
             importlib.import_module(".".join([mod_name, "object"]))
 
 
 def test_derived_class_no_proto_mod():
     """Test that an appropriate error is raised when the derived library does
     not have a protobufs directory
     """
@@ -106,16 +106,16 @@
                     class Object(base.DataBase):
                         def __init__(self, foo):
                             self.foo = foo
                     """
                 )
             )
 
-        # Make sure an AttributeError is raised when the import is tried
-        with pytest.raises(AttributeError):
+        # Make sure an ValueError is raised when the import is tried
+        with pytest.raises(ValueError):
             importlib.import_module(".".join([mod_name, "object"]))
 
 
 def test_derived_class_no_import_side_effects():
     """Test that a library which does not use the import side effects can still
     safely create a derived data model class
     """
@@ -140,16 +140,18 @@
             )
 
         # Add a derived data model class file
         with open(os.path.join(mod_dir, "object.py"), "w", encoding="utf-8") as handle:
             handle.write(
                 justify_script_string(
                     """
+                    from . import protobufs
                     from caikit.core.data_model import base
                     class Object(base.DataBase):
+                        _proto_class = protobufs.Object
                         def __init__(self, foo):
                             self.foo = foo
                     """
                 )
             )
 
         # Make sure the import succeeds and that the data model class has the
@@ -264,41 +266,41 @@
         # Single kwarg, other unset
         msg = dm.ThingOne(foo=1)
         assert msg.foo == 1
         assert msg.bar is None
 
 
 def test_default_init_invalid_args():
-    """Make sure that a ValueError is raised if the default __init__ is given
+    """Make sure that a TypeError is raised if the default __init__ is given
     various combinations of incorrect arguments
     """
     with temp_data_model(
         make_proto_def(
             {
                 "ThingOne": {
                     "foo": int,
                     "bar": int,
                 }
             }
         )
     ) as dm:
         # Too many arguments
-        with pytest.raises(ValueError):
+        with pytest.raises(TypeError):
             dm.ThingOne(1, 2, 3, 4)
 
         # Too many args + kwargs
-        with pytest.raises(ValueError):
+        with pytest.raises(TypeError):
             dm.ThingOne(1, 2, baz=3)
 
         # Bad kwarg name
-        with pytest.raises(ValueError):
+        with pytest.raises(TypeError):
             dm.ThingOne(1, baz=3)
 
         # Multiple values
-        with pytest.raises(ValueError):
+        with pytest.raises(TypeError):
             dm.ThingOne(1, foo=3)
 
 
 ############################
 ## get_field_message_type ##
 ############################
 
@@ -378,15 +380,15 @@
 
 def test_primitive_maps_are_serializable():
     """Ensure that we correctly handle primitive values for de/serialization."""
     with temp_data_model(
         make_proto_def(
             {
                 "MapParty": {
-                    "mobject": '{"values": str}',
+                    "mobject": "Dict[str, str]",
                 },
             }
         )
     ) as dm:
         msg = dm.MapParty({"foo": "bar"})
         # Make sure we can proto and back
         recon_msg = dm.MapParty.from_proto(msg.to_proto())
@@ -403,15 +405,15 @@
     with temp_data_model(
         make_proto_def(
             {
                 "ComplexType": {
                     "foo": int,
                 },
                 "MapParty": {
-                    "mobject": '{"values": ComplexType}',
+                    "mobject": "Dict[str, ComplexType]",
                 },
             }
         )
     ) as dm:
         nested_msg = dm.ComplexType(100)
         msg = dm.MapParty({"foo": nested_msg})
         # Make sure we can proto and back
```

### Comparing `caikit-0.2.1/tests/core/data_model/test_producer.py` & `caikit-0.3.0/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/helpers.py` & `caikit-0.3.0/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/module_backends/test_backend_types.py` & `caikit-0.3.0/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/test_imports.py` & `caikit-0.3.0/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/test_model_manager.py` & `caikit-0.3.0/tests/core/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/test_module.py` & `caikit-0.3.0/tests/core/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/test_module_backend_config.py` & `caikit-0.3.0/tests/core/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/test_module_metadata.py` & `caikit-0.3.0/tests/core/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/test_no_write_permissions.py` & `caikit-0.3.0/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/toolkit/test_compatibility.py` & `caikit-0.3.0/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/toolkit/test_error_handler.py` & `caikit-0.3.0/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/toolkit/test_fileio.py` & `caikit-0.3.0/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.3.0/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/toolkit/test_serializers.py` & `caikit-0.3.0/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.3.0/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/workflows/__init__.py` & `caikit-0.3.0/tests/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/core/workflows/test_base.py` & `caikit-0.3.0/tests/core/workflows/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/data_model_helpers.py` & `caikit-0.3.0/tests/data_model_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -139,34 +139,32 @@
 def _get_proto_val_name(field_val) -> str:
     if isinstance(field_val, str):
         return field_val
     if isinstance(field_val, type):
         return field_val.__name__
     if isinstance(field_val, list):
         assert len(field_val) == 1
-        return f"""{{"elements": {_get_proto_val_name(field_val[0])}}}"""
+        return f"List[{_get_proto_val_name(field_val[0])}]"
     raise RuntimeError(f"Invalid field type specifier: {field_val}")
 
 
 def make_proto_def(message_specs: Dict[str, dict], pkg_suffix: str = None) -> str:
     """Helper for writing a syntatically correct protobufs file"""
     if pkg_suffix is None:
         pkg_suffix = _random_package_suffix()
     package_name = f"{caikit.core.data_model.CAIKIT_DATA_MODEL}.{pkg_suffix}"
-    # pylint: disable=f-string-without-interpolation
     out = justify_script_string(
-        f"""
-        import caikit.core
+        """
+        from typing import Dict, List
+        from caikit.core.data_model import DataObjectBase, dataobject
 
         """
     )
     for message_name, message_spec in message_specs.items():
-        # pylint: disable=f-string-without-interpolation
-        msg_str = f"""\n@caikit.core.dataobject(schema={{"""
-        schema_fields = [
-            f'"{field_name}": {_get_proto_val_name(field_val)}'
-            for field_name, field_val in message_spec.items()
-        ]
-        msg_str += ", ".join(schema_fields)
-        msg_str += f'}}, package="{package_name}")\nclass {message_name}: pass\n\n'
+        msg_str = (
+            f'\n@dataobject("{package_name}")\nclass {message_name}(DataObjectBase):\n'
+        )
+        for field_name, field_type in message_spec.items():
+            msg_str += f"    {field_name}: {_get_proto_val_name(field_type)}\n"
+        msg_str += "\n"
         out += msg_str
     return out
```

### Comparing `caikit-0.2.1/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.3.0/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/dummy_block.zip` & `caikit-0.3.0/tests/fixtures/dummy_block.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/dummy_block/config.yml` & `caikit-0.3.0/tests/fixtures/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/dummy_block_singleton/config.yml` & `caikit-0.3.0/tests/fixtures/dummy_block_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/dummy_resource.zip` & `caikit-0.3.0/tests/fixtures/dummy_resource.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/dummy_workflow.zip` & `caikit-0.3.0/tests/fixtures/dummy_workflow.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/dummy_workflow/dummy_block/config.yml` & `caikit-0.3.0/tests/fixtures/dummy_workflow/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/fixtures.py` & `caikit-0.3.0/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/invalid.zip` & `caikit-0.3.0/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/linux.txt` & `caikit-0.3.0/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/primitive_party.proto` & `caikit-0.3.0/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_pb2.py` & `caikit-0.3.0/tests/fixtures/protobufs/caikit_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py` & `caikit-0.3.0/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_train_pb2.py` & `caikit-0.3.0/tests/fixtures/protobufs/caikit_runtime_train_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py` & `caikit-0.3.0/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.3.0/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py` & `caikit-0.3.0/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py` & `caikit-0.3.0/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py` & `caikit-0.3.0/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A sample block for sample things!
 """
 # Standard
-from typing import List
+from typing import List, Optional
 
 # Local
 from ...data_model.sample import SampleInputType, SampleOutputType, SampleTrainingType
 from caikit.core.data_model import DataStream
 from caikit.core.module import ModuleLoader, ModuleSaver
 import caikit.core
 
@@ -58,14 +58,17 @@
             module_saver.update_config(config_options)
 
     @classmethod
     def train(
         cls,
         training_data: DataStream[SampleTrainingType],
         batch_size: int = 64,
-        poison_pills: List[str] = [POISON_PILL_NAME],
+        poison_pills: Optional[List[str]] = None,
     ) -> "ListBlock":
         """Sample training method that produces a trained model"""
         # Barf if we were incorrectly passed data not in datastream format
+        poison_pills = (
+            poison_pills if poison_pills is not None else [cls.POISON_PILL_NAME]
+        )
         assert isinstance(training_data, DataStream)
         assert len(poison_pills) > 0
         return cls(batch_size=batch_size)
```

### Comparing `caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py` & `caikit-0.3.0/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py` & `caikit-0.3.0/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.3.0/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 """
 Dummy data model object for testing
 """
 
 # Local
-import caikit.core
+from caikit.core.data_model import DataObjectBase, dataobject
 
 
-@caikit.core.dataobject({"name": str}, package="caikit_data_model.sample_lib")
-class SampleInputType:
+@dataobject(package="caikit_data_model.sample_lib")
+class SampleInputType(DataObjectBase):
     """A sample `domain primitive` input type for this library.
     The analog to a `Raw Document` for the `Natural Language Processing` domain."""
 
+    name: str
 
-@caikit.core.dataobject(
-    schema={"greeting": str}, package="caikit_data_model.sample_lib"
-)
-class SampleOutputType:
+
+@dataobject(package="caikit_data_model.sample_lib")
+class SampleOutputType(DataObjectBase):
     """A simple return type for the `sample_task` task"""
 
+    greeting: str
+
 
-@caikit.core.dataobject(
-    schema={"farewell": str}, package="caikit_data_model.sample_lib"
-)
-class OtherOutputType:
+@dataobject(package="caikit_data_model.sample_lib")
+class OtherOutputType(DataObjectBase):
     """A simple return type for the `other_task` task"""
 
+    farewell: str
 
-@caikit.core.dataobject({"number": int}, package="caikit_data_model.sample_lib")
-class SampleTrainingType:
+
+@dataobject(package="caikit_data_model.sample_lib")
+class SampleTrainingType(DataObjectBase):
     """A sample `training data` type for the `sample_task` task."""
+
+    number: int
```

### Comparing `caikit-0.2.1/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py` & `caikit-0.3.0/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/generated/__init__.py` & `caikit-0.3.0/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/metrics/__init__.py` & `caikit-0.3.0/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.3.0/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/model_management/__init__.py` & `caikit-0.3.0/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/model_management/test_batcher.py` & `caikit-0.3.0/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/model_management/test_model_loader.py` & `caikit-0.3.0/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/model_management/test_model_manager.py` & `caikit-0.3.0/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.3.0/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/model_management/test_training_manager.py` & `caikit-0.3.0/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.3.0/tests/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/service_generation/signature_parsing/test_docstrings.py` & `caikit-0.3.0/tests/runtime/service_generation/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/service_generation/signature_parsing/test_parsers.py` & `caikit-0.3.0/tests/runtime/service_generation/signature_parsing/test_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,15 +258,21 @@
     """Check that we get arguments with any default value supplied"""
 
     def _run(
         a, b: bool, c: int = None, d: str = None, e: int = 5, f: float = 0.5, g=None
     ):
         pass
 
-    assert get_args_with_defaults(_run) == {"c", "d", "e", "f", "g"}
+    assert get_args_with_defaults(_run) == {
+        "c": None,
+        "d": None,
+        "e": 5,
+        "f": 0.5,
+        "g": None,
+    }
 
 
 def test_get_args_with_known_args():
     """Check that we get arguments with a known arg type supplied"""
 
     def _run(producer_id):
         pass
```

### Comparing `caikit-0.2.1/tests/runtime/service_generation/test_create_service.py` & `caikit-0.3.0/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.3.0/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Standard
+from dataclasses import dataclass
 from typing import List
 import json
 import os
 import pickle
 import tempfile
 
 # Third Party
 import pytest
 
 # Local
+from caikit.core.data_model import DataObjectBase, dataobject
 from caikit.core.data_model.streams.data_stream import DataStream
 from caikit.runtime.service_generation.data_stream_source import (
     DataStreamSourceBase,
     _make_data_stream_source_type_name,
     get_data_stream_source,
     make_data_stream_source,
 )
@@ -178,17 +180,18 @@
 
 
 def test_pickle_round_trip_data_model():
     """Make sure that a source wrapping a data model object can be round-tripped
     cleanly with pickle
     """
 
-    @caikit.core.dataobject({"foo": int, "bar": str})
-    class Foo:
-        pass
+    @dataobject
+    class Foo(DataObjectBase):
+        foo: int
+        bar: str
 
     stream_type = make_data_stream_source(Foo)
     inst = stream_type(
         jsondata=stream_type.JsonData(data=[Foo(1, "two"), Foo(2, "three")])
     )
     round_trip = pickle.loads(pickle.dumps(inst))
     assert round_trip.to_dict() == inst.to_dict()
```

### Comparing `caikit-0.2.1/tests/runtime/service_generation/test_primitives.py` & `caikit-0.3.0/tests/runtime/service_generation/test_primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.3.0/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/servicers/__init__.py` & `caikit-0.3.0/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.3.0/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.3.0/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.3.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.3.0/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.3.0/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,23 +57,23 @@
     # Create a future and set it in the training manager
     future = training_pool.submit(_train, wait_event=event)
     training_manager.training_futures[training_id] = future
 
     # send a request, check it's processing
     request = TrainingInfoRequest(training_id=training_id).to_proto()
     response = training_management_servicer.GetTrainingStatus(request, context=None)
-    assert response.status == TrainingStatus.PROCESSING
+    assert response.status == TrainingStatus.PROCESSING.value
 
     event.set()
     future.result()
 
     # Ensure it's now done
     request = TrainingInfoRequest(training_id=training_id).to_proto()
     response = training_management_servicer.GetTrainingStatus(request, context=None)
-    assert response.status == TrainingStatus.COMPLETED
+    assert response.status == TrainingStatus.COMPLETED.value
 
 
 def test_training_complete_status(training_management_servicer, training_pool):
     training_id = str(uuid.uuid4())
     training_manager = TrainingManager.get_instance()
 
     # Create a future and set it in the training manager
@@ -83,15 +83,15 @@
     future.result()
 
     # send a request
     request = TrainingInfoRequest(training_id=training_id).to_proto()
     response = training_management_servicer.GetTrainingStatus(request, context=None)
 
     assert re.match("<class '.*TrainingInfoResponse'>", str(type(response)))
-    assert response.status == TrainingStatus.COMPLETED
+    assert response.status == TrainingStatus.COMPLETED.value
 
 
 def test_training_status_incorrect_id(training_management_servicer):
     # send a request with a training id that doesn't exist
     request = TrainingInfoRequest(training_id="some_random_id").to_proto()
     with pytest.raises(CaikitRuntimeException) as context:
         training_management_servicer.GetTrainingStatus(request, context=None)
@@ -111,8 +111,8 @@
     future = training_pool.submit(_train, raise_=True)
     training_manager.training_futures[training_id] = future
 
     # send a request
     request = TrainingInfoRequest(training_id=training_id).to_proto()
     response = training_management_servicer.GetTrainingStatus(request, context=None)
 
-    assert response.status == TrainingStatus.FAILED
+    assert response.status == TrainingStatus.FAILED.value
```

### Comparing `caikit-0.2.1/tests/runtime/test_grpc_server.py` & `caikit-0.3.0/tests/runtime/test_grpc_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         runtime_grpc_server.make_local_channel()
     )
 
     # MT training is sync, so it should be COMPLETE immediately
     response: TrainingInfoResponse = TrainingInfoResponse.from_proto(
         training_management_stub.GetTrainingStatus(training_info_request)
     )
-    assert response.status == TrainingStatus.COMPLETED
+    assert response.status == TrainingStatus.COMPLETED.value
 
     # Make sure we wait for training to finish
     result = TrainingManager.get_instance().training_futures[training_id].result()
 
     assert (
         result.BLOCK_CLASS
         == "sample_lib.blocks.sample_task.sample_implementation.SampleBlock"
@@ -708,15 +708,15 @@
             sample_input=HAPPY_PATH_INPUT
         )
         _ = stub.SampleTaskPredict(
             predict_request, metadata=[("mm-model-id", loaded_model_id)]
         )
 
         # Interrupt server
-        server.interrupt(None)
+        server.interrupt(None, None)
 
         # Assertions on the created metrics file
         with open(server._global_predict_servicer.rpc_meter.file_path) as f:
             data = [json.loads(line) for line in f]
 
             assert len(data) == 1
             assert list(data[0].keys()) == [
```

### Comparing `caikit-0.2.1/tests/runtime/test_service_factory.py` & `caikit-0.3.0/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/utils/__init__.py` & `caikit-0.3.0/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/utils/test_import_util.py` & `caikit-0.3.0/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/utils/test_servicer_util.py` & `caikit-0.3.0/tests/runtime/utils/test_servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/work_management/__init__.py` & `caikit-0.3.0/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.3.0/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.3.0/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.3.0/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/tox.ini` & `caikit-0.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-0.2.1/PKG-INFO` & `caikit-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.2.1
+Version: 0.3.0
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.1.1,<2.0.0
 Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
 Requires-Dist: docstring-parser>=0.14.1,<0.15.0
 Requires-Dist: grpcio-health-checking>=1.35.0,<2.0
 Requires-Dist: grpcio>=1.35.0,<2.0
 Requires-Dist: ijson>=3.1.4,<3.3.0
 Requires-Dist: munch>=2.5.0,<3.0
 Requires-Dist: protobuf>=3.19.0,<5
-Requires-Dist: prometheus_client==0.12.0
+Requires-Dist: prometheus_client>=0.12.0,<1.0
 Requires-Dist: py-grpc-prometheus>=0.7.0,<0.8
 Requires-Dist: PyYAML>=6.0,<7.0
 Requires-Dist: requests>=2.26.0,<3.0
 Requires-Dist: semver>=2.13.0,<4.0
 Requires-Dist: six>=1.16.0,<2.0.0
 Requires-Dist: tqdm>=4.59.0,<5.0.0
-Requires-Dist: jtd-to-proto>=0.12.1,<0.13.0
+Requires-Dist: py-to-proto>=0.1.2,<0.2.0
 Requires-Dist: import-tracker>=3.1.5,<4
 Project-URL: Source, https://github.com/caikit/caikit
 
 # Caikit
 
 Caikit is an AI toolkit that enables users to manage models through a set of developer friendly APIs. It provides a consistent format for creating and using AI models against a wide variety of data domains and tasks.
 
@@ -58,23 +58,15 @@
   - They bring data and tuning params to a pre-existing model architecture and create a new concrete model using APIs provided by Caikit
   - Examples of model authors are machine learning engineers, data scientists, and AI developers
 - AI Model Operator:
   - Model operators use an existing AI model to perform a specific function within the context of an application
   - They take trained models, deploy them, and then infer the models in applications through APIs provided by Caikit
   - Examples of operators are cloud and embedded application developers whose applications need analysis of unstructured data
 
-## AI Model Operator Quick Start
+## AI Model Operator Example
 
-**UNDER CONSTRUCTION**
-
-At this point, Caikit does not publish any pre-defined task implementations that can be readily consumed. Stay tuned!
-
-## AI Model Author Quick Start
-
-**UNDER CONSTRUCTION**
-
-We're getting a slim example ready, so stay tuned!
+Check out the [Text Sentiment example](examples/text-sentiment/) to understand how to load and infer a model using Caikit.
 
 ## Code of conduct
 
 Participation in the Caikit community is governed by the [Code of Conduct](CODE-OF-CONDUCT.md).
```

