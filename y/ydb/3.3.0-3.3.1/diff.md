# Comparing `tmp/ydb-3.3.0.tar.gz` & `tmp/ydb-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydb-3.3.0.tar", last modified: Fri Apr 14 17:36:18 2023, max compression
+gzip compressed data, was "ydb-3.3.1.tar", last modified: Thu May  4 14:04:41 2023, max compression
```

## Comparing `ydb-3.3.0.tar` & `ydb-3.3.1.tar`

### file list

```diff
@@ -1,272 +1,272 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.365202 ydb-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-14 17:36:08.000000 ydb-3.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-14 17:36:08.000000 ydb-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 17:36:08.000000 ydb-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-14 17:36:18.365202 ydb-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-14 17:36:08.000000 ydb-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 17:36:08.000000 ydb-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 17:36:08.000000 ydb-3.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:36:18.365202 ydb-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 17:36:11.000000 ydb-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.313202 ydb-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.313202 ydb-3.3.0/tests/aio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_async_iter_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_session_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/session_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.313202 ydb-3.3.0/tests/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/ssl/test_ssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.313202 ydb-3.3.0/tests/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/table/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/table/test_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/test_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.317202 ydb-3.3.0/tests/topics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/topics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/topics/test_control_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/topics/test_topic_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/topics/test_topic_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.321202 ydb-3.3.0/ydb/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.325202 ydb-3.3.0/ydb/_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.325202 ydb-3.3.0/ydb/_grpc/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.325202 ydb-3.3.0/ydb/_grpc/grpcwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/grpcwrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/grpcwrapper/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    42486 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_topic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.329202 ydb-3.3.0/ydb/_grpc/v3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.341202 ydb-3.3.0/ydb/_grpc/v3/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.341202 ydb-3.3.0/ydb/_grpc/v3/protos/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/annotations/validation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/annotations/validation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    83179 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_cms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_cms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   121326 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_coordination_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_coordination_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_export_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_export_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_formats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_formats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_import_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_import_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_issue_message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    72285 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29771 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_query_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    40278 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_scheme_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_scheme_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_scripting_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_scripting_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_status_codes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   332647 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_table_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_table_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   234296 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    52587 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_auth_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_cms_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_coordination_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_discovery_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_export_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_import_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_operation_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_scheme_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_scripting_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_table_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_topic_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.349202 ydb-3.3.0/ydb/_grpc/v4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.357202 ydb-3.3.0/ydb/_grpc/v4/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.357202 ydb-3.3.0/ydb/_grpc/v4/protos/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/annotations/validation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/annotations/validation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_cms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_cms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_coordination_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_coordination_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_export_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_export_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_formats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_formats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_import_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_import_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_issue_message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_query_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_scheme_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_scheme_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_scripting_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_scripting_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_status_codes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    46408 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_table_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_table_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    34953 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_auth_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_cms_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_coordination_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_discovery_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_export_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_import_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_operation_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_scheme_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_scripting_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_table_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_topic_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_session_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_sp_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.357202 ydb-3.3.0/ydb/_topic_common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_common/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_common/common_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_common/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.361202 ydb-3.3.0/ydb/_topic_reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/datatypes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/topic_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/topic_reader_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    46855 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/topic_reader_asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/topic_reader_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.361202 ydb-3.3.0/ydb/_topic_writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_writer/topic_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23235 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_writer/topic_writer_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_writer/topic_writer_asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_writer/topic_writer_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_writer/topic_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_tx_ctx_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_utilities_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.365202 ydb-3.3.0/ydb/aio/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/auth_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.365202 ydb-3.3.0/ydb/dbapi/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/dbapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/dbapi/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/dbapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)   285865 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/default_pem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/global_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.365202 ydb-3.3.0/ydb/iam/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/iam/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/import_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/scheme_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.365202 ydb-3.3.0/ydb/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/sqlalchemy/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    82321 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/types.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 17:36:11.000000 ydb-3.3.0/ydb/ydb_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.365202 ydb-3.3.0/ydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-14 17:36:18.000000 ydb-3.3.0/ydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-14 17:36:18.000000 ydb-3.3.0/ydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:36:18.000000 ydb-3.3.0/ydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-14 17:36:18.000000 ydb-3.3.0/ydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 17:36:18.000000 ydb-3.3.0/ydb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.092745 ydb-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-04 14:04:29.000000 ydb-3.3.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-04 14:04:29.000000 ydb-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 14:04:29.000000 ydb-3.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-04 14:04:41.092745 ydb-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-04 14:04:29.000000 ydb-3.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 14:04:29.000000 ydb-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-04 14:04:29.000000 ydb-3.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:04:41.092745 ydb-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-04 14:04:34.000000 ydb-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.052744 ydb-3.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.052744 ydb-3.3.1/tests/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/aio/test_async_iter_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/aio/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/aio/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/aio/test_session_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/aio/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/aio/test_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/aio/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/session_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.052744 ydb-3.3.1/tests/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/ssl/test_ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.052744 ydb-3.3.1/tests/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/table/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/table/test_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/test_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.052744 ydb-3.3.1/tests/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/topics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/topics/test_control_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/topics/test_topic_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-04 14:04:29.000000 ydb-3.3.1/tests/topics/test_topic_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.056744 ydb-3.3.1/ydb/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.056744 ydb-3.3.1/ydb/_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.056744 ydb-3.3.1/ydb/_grpc/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.060744 ydb-3.3.1/ydb/_grpc/grpcwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/grpcwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/grpcwrapper/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/grpcwrapper/ydb_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42486 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/grpcwrapper/ydb_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/grpcwrapper/ydb_topic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.064744 ydb-3.3.1/ydb/_grpc/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.068745 ydb-3.3.1/ydb/_grpc/v3/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.072744 ydb-3.3.1/ydb/_grpc/v3/protos/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/annotations/validation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/annotations/validation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83179 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_cms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_cms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121326 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_coordination_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_coordination_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_export_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_export_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_formats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_formats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_import_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_import_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_issue_message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72285 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29771 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_query_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40278 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_scheme_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_scheme_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_scripting_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_scripting_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_status_codes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   332647 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_table_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_table_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234296 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52587 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/protos/ydb_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_auth_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_cms_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_coordination_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_discovery_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_export_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_import_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_operation_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_scheme_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_scripting_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_table_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_topic_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.076745 ydb-3.3.1/ydb/_grpc/v4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.084745 ydb-3.3.1/ydb/_grpc/v4/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.084745 ydb-3.3.1/ydb/_grpc/v4/protos/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/annotations/validation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/annotations/validation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_cms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_cms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_coordination_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_coordination_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_export_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_export_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_formats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_formats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_import_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_import_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_issue_message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_query_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_scheme_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_scheme_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_scripting_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_scripting_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_status_codes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46408 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_table_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_table_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34953 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/protos/ydb_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_auth_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_cms_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_coordination_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_discovery_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_export_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_import_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_operation_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_scheme_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_scripting_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_table_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_topic_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_session_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_sp_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.084745 ydb-3.3.1/ydb/_topic_common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_common/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_common/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.088745 ydb-3.3.1/ydb/_topic_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_reader/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_reader/datatypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_reader/topic_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_reader/topic_reader_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46855 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_reader/topic_reader_asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_reader/topic_reader_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.088745 ydb-3.3.1/ydb/_topic_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_writer/topic_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23235 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_writer/topic_writer_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_writer/topic_writer_asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_writer/topic_writer_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_topic_writer/topic_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_tx_ctx_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/_utilities_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.088745 ydb-3.3.1/ydb/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/aio/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/aio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/aio/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/aio/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/aio/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/aio/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/aio/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/aio/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/aio/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/auth_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.092745 ydb-3.3.1/ydb/dbapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/dbapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/dbapi/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/dbapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   285865 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/default_pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.092745 ydb-3.3.1/ydb/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/iam/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/import_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/scheme_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.092745 ydb-3.3.1/ydb/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/sqlalchemy/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82321 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-04 14:04:29.000000 ydb-3.3.1/ydb/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 14:04:34.000000 ydb-3.3.1/ydb/ydb_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:41.092745 ydb-3.3.1/ydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-04 14:04:41.000000 ydb-3.3.1/ydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-05-04 14:04:41.000000 ydb-3.3.1/ydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:04:41.000000 ydb-3.3.1/ydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 14:04:41.000000 ydb-3.3.1/ydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 14:04:41.000000 ydb-3.3.1/ydb.egg-info/top_level.txt
```

### Comparing `ydb-3.3.0/LICENSE` & `ydb-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/PKG-INFO` & `ydb-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydb
-Version: 3.3.0
+Version: 3.3.1
 Summary: YDB Python SDK
 Home-page: http://github.com/ydb-platform/ydb-python-sdk
 Author: Yandex LLC
 Author-email: ydb@yandex-team.ru
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ydb-3.3.0/README.md` & `ydb-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/setup.py` & `ydb-3.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     for line in r.readlines():
         line = line.strip()
         if line != "":
             requirements.append(line)
 
 setuptools.setup(
     name="ydb",
-    version="3.3.0",  # AUTOVERSION
+    version="3.3.1",  # AUTOVERSION
     description="YDB Python SDK",
     author="Yandex LLC",
     author_email="ydb@yandex-team.ru",
     url="http://github.com/ydb-platform/ydb-python-sdk",
     license="Apache 2.0",
     package_dir={"": "."},
     long_description=long_description,
```

### Comparing `ydb-3.3.0/tests/aio/test_async_iter_stream.py` & `ydb-3.3.1/tests/aio/test_async_iter_stream.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/tests/aio/test_connection.py` & `ydb-3.3.1/tests/aio/test_connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/tests/aio/test_connection_pool.py` & `ydb-3.3.1/tests/aio/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/tests/aio/test_session_pool.py` & `ydb-3.3.1/tests/aio/test_session_pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/tests/aio/test_tx.py` & `ydb-3.3.1/tests/aio/test_tx.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/tests/aio/test_types.py` & `ydb-3.3.1/tests/aio/test_types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/tests/conftest.py` & `ydb-3.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/tests/session_pool.py` & `ydb-3.3.1/tests/session_pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/tests/table/table_test.py` & `ydb-3.3.1/tests/table/table_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/tests/table/test_tx.py` & `ydb-3.3.1/tests/table/test_tx.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/tests/test_errors.py` & `ydb-3.3.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/tests/topics/test_control_plane.py` & `ydb-3.3.1/tests/topics/test_control_plane.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/tests/topics/test_topic_reader.py` & `ydb-3.3.1/tests/topics/test_topic_reader.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/tests/topics/test_topic_writer.py` & `ydb-3.3.1/tests/topics/test_topic_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from __future__ import annotations
+from typing import List
+
 import pytest
 
 import ydb.aio
 
 
 @pytest.mark.asyncio
 class TestTopicWriterAsyncIO:
@@ -192,7 +195,20 @@
         ],
     )
     def test_write_encoded(self, driver_sync: ydb.Driver, topic_path: str, codec):
         with driver_sync.topic_client.writer(topic_path, codec=codec) as writer:
             writer.write("a" * 1000)
             writer.write("b" * 1000)
             writer.write("c" * 1000)
+
+    def test_start_many_sync_writers_in_parallel(self, driver_sync: ydb.Driver, topic_path):
+        target_count = 100
+        writers = []  # type: List[ydb.TopicWriter]
+        for i in range(target_count):
+            writer = driver_sync.topic_client.writer(topic_path)
+            writers.append(writer)
+
+        for i, writer in enumerate(writers):
+            writer.write(str(i))
+
+        for writer in writers:
+            writer.close()
```

### Comparing `ydb-3.3.0/ydb/__init__.py` & `ydb-3.3.1/ydb/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_apis.py` & `ydb-3.3.1/ydb/_apis.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_errors.py` & `ydb-3.3.1/ydb/_errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/common/__init__.py` & `ydb-3.3.1/ydb/_grpc/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/grpcwrapper/common_utils.py` & `ydb-3.3.1/ydb/_grpc/grpcwrapper/common_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import abc
 import asyncio
+import concurrent.futures
 import contextvars
 import datetime
 import functools
 import typing
 from typing import (
     Optional,
     Any,
@@ -107,27 +108,28 @@
     def __next__(self):
         item = asyncio.run_coroutine_threadsafe(self._queue.get(), self._loop).result()
         if item is _stop_grpc_connection_marker:
             raise StopIteration()
         return item
 
 
-class SyncIteratorToAsyncIterator:
-    def __init__(self, sync_iterator: Iterator):
+class SyncToAsyncIterator:
+    def __init__(self, sync_iterator: Iterator, executor: concurrent.futures.Executor):
         self._sync_iterator = sync_iterator
+        self._executor = executor
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
         try:
-            res = await to_thread(self._sync_iterator.__next__)
+            res = await to_thread(self._sync_iterator.__next__, executor=self._executor)
             return res
-        except StopAsyncIteration:
-            raise StopIteration()
+        except StopIteration:
+            raise StopAsyncIteration()
 
 
 class IGrpcWrapperAsyncIO(abc.ABC):
     @abc.abstractmethod
     async def receive(self) -> Any:
         ...
 
@@ -145,53 +147,61 @@
 
 class GrpcWrapperAsyncIO(IGrpcWrapperAsyncIO):
     from_client_grpc: asyncio.Queue
     from_server_grpc: AsyncIterator
     convert_server_grpc_to_wrapper: Callable[[Any], Any]
     _connection_state: str
     _stream_call: Optional[Union[grpc.aio.StreamStreamCall, "grpc._channel._MultiThreadedRendezvous"]]
+    _wait_executor: Optional[concurrent.futures.ThreadPoolExecutor]
 
     def __init__(self, convert_server_grpc_to_wrapper):
         self.from_client_grpc = asyncio.Queue()
         self.convert_server_grpc_to_wrapper = convert_server_grpc_to_wrapper
         self._connection_state = "new"
         self._stream_call = None
+        self._wait_executor = None
+
+    def __del__(self):
+        self._clean_executor(wait=False)
 
     async def start(self, driver: SupportedDriverType, stub, method):
         if asyncio.iscoroutinefunction(driver.__call__):
             await self._start_asyncio_driver(driver, stub, method)
         else:
             await self._start_sync_driver(driver, stub, method)
         self._connection_state = "started"
 
     def close(self):
         self.from_client_grpc.put_nowait(_stop_grpc_connection_marker)
         if self._stream_call:
             self._stream_call.cancel()
 
+        self._clean_executor(wait=True)
+
+    def _clean_executor(self, wait: bool):
+        if self._wait_executor:
+            self._wait_executor.shutdown(wait)
+
     async def _start_asyncio_driver(self, driver: ydb.aio.Driver, stub, method):
         requests_iterator = QueueToIteratorAsyncIO(self.from_client_grpc)
         stream_call = await driver(
             requests_iterator,
             stub,
             method,
         )
         self._stream_call = stream_call
         self.from_server_grpc = stream_call.__aiter__()
 
     async def _start_sync_driver(self, driver: ydb.Driver, stub, method):
         requests_iterator = AsyncQueueToSyncIteratorAsyncIO(self.from_client_grpc)
-        stream_call = await to_thread(
-            driver,
-            requests_iterator,
-            stub,
-            method,
-        )
+        self._wait_executor = concurrent.futures.ThreadPoolExecutor(max_workers=1)
+
+        stream_call = await to_thread(driver, requests_iterator, stub, method, executor=self._wait_executor)
         self._stream_call = stream_call
-        self.from_server_grpc = SyncIteratorToAsyncIterator(stream_call.__iter__())
+        self.from_server_grpc = SyncToAsyncIterator(stream_call.__iter__(), self._wait_executor)
 
     async def receive(self) -> Any:
         # todo handle grpc exceptions and convert it to internal exceptions
         try:
             grpc_message = await self.from_server_grpc.__anext__()
         except grpc.RpcError as e:
             raise connection._rpc_error_handler(self._connection_state, e)
@@ -251,15 +261,15 @@
 
     if asyncio.iscoroutinefunction(callback):
         return loop.create_task(callback())
     else:
         return loop.run_in_executor(None, callback)
 
 
-async def to_thread(func, /, *args, **kwargs):
+async def to_thread(func, *args, executor: Optional[concurrent.futures.Executor], **kwargs):
     """Asynchronously run function *func* in a separate thread.
 
     Any *args and **kwargs supplied for this function are directly passed
     to *func*. Also, the current :class:`contextvars.Context` is propagated,
     allowing context variables from the main thread to be accessed in the
     separate thread.
 
@@ -267,15 +277,15 @@
 
     copy to_thread from 3.10
     """
 
     loop = asyncio.get_running_loop()
     ctx = contextvars.copy_context()
     func_call = functools.partial(ctx.run, func, *args, **kwargs)
-    return await loop.run_in_executor(None, func_call)
+    return await loop.run_in_executor(executor, func_call)
 
 
 def proto_duration_from_timedelta(t: Optional[datetime.timedelta]) -> Optional[ProtoDuration]:
     if t is None:
         return None
 
     res = ProtoDuration()
```

### Comparing `ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_scheme.py` & `ydb-3.3.1/ydb/_grpc/grpcwrapper/ydb_scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_topic.py` & `ydb-3.3.1/ydb/_grpc/grpcwrapper/ydb_topic.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py` & `ydb-3.3.1/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_topic_test.py` & `ydb-3.3.1/ydb/_grpc/grpcwrapper/ydb_topic_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/annotations/validation_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/annotations/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_auth_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_auth_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_cms_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_cms_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_common_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_common_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_coordination_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_coordination_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_discovery_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_discovery_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_export_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_export_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_formats_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_formats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_import_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_import_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_operation_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_scheme_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_scheme_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_scripting_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_scripting_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_table_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_table_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_topic_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_topic_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_value_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/protos/ydb_value_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_auth_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_auth_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_cms_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_cms_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_coordination_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_coordination_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_discovery_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_discovery_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_export_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_export_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_import_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_import_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_operation_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_operation_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_scheme_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_scheme_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_scripting_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_scripting_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_table_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_table_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_topic_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_topic_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/annotations/validation_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/annotations/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_auth_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_auth_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_cms_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_cms_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_common_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_common_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_coordination_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_coordination_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_discovery_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_discovery_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_export_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_export_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_formats_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_formats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_import_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_import_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_operation_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_scheme_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_scheme_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_scripting_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_scripting_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_table_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_table_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_topic_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_topic_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_value_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/protos/ydb_value_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_auth_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_auth_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_cms_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_cms_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_coordination_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_coordination_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_discovery_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_discovery_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_export_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_export_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_import_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_import_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_operation_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_operation_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_scheme_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_scheme_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_scripting_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_scripting_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_table_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_table_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_topic_v1_pb2.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_topic_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py` & `ydb-3.3.1/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_session_impl.py` & `ydb-3.3.1/ydb/_session_impl.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_sp_impl.py` & `ydb-3.3.1/ydb/_sp_impl.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_common/common.py` & `ydb-3.3.1/ydb/_topic_common/common.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_common/common_test.py` & `ydb-3.3.1/ydb/_topic_common/common_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_common/test_helpers.py` & `ydb-3.3.1/ydb/_topic_common/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_reader/datatypes.py` & `ydb-3.3.1/ydb/_topic_reader/datatypes.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_reader/datatypes_test.py` & `ydb-3.3.1/ydb/_topic_reader/datatypes_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_reader/topic_reader.py` & `ydb-3.3.1/ydb/_topic_reader/topic_reader.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_reader/topic_reader_asyncio.py` & `ydb-3.3.1/ydb/_topic_reader/topic_reader_asyncio.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_reader/topic_reader_asyncio_test.py` & `ydb-3.3.1/ydb/_topic_reader/topic_reader_asyncio_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_reader/topic_reader_sync.py` & `ydb-3.3.1/ydb/_topic_reader/topic_reader_sync.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_writer/topic_writer.py` & `ydb-3.3.1/ydb/_topic_writer/topic_writer.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_writer/topic_writer_asyncio.py` & `ydb-3.3.1/ydb/_topic_writer/topic_writer_asyncio.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_writer/topic_writer_asyncio_test.py` & `ydb-3.3.1/ydb/_topic_writer/topic_writer_asyncio_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_writer/topic_writer_sync.py` & `ydb-3.3.1/ydb/_topic_writer/topic_writer_sync.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_topic_writer/topic_writer_test.py` & `ydb-3.3.1/ydb/_topic_writer/topic_writer_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_tx_ctx_impl.py` & `ydb-3.3.1/ydb/_tx_ctx_impl.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/_utilities.py` & `ydb-3.3.1/ydb/_utilities.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/aio/connection.py` & `ydb-3.3.1/ydb/aio/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/aio/credentials.py` & `ydb-3.3.1/ydb/aio/credentials.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/aio/driver.py` & `ydb-3.3.1/ydb/aio/driver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/aio/iam.py` & `ydb-3.3.1/ydb/aio/iam.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/aio/pool.py` & `ydb-3.3.1/ydb/aio/pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/aio/resolver.py` & `ydb-3.3.1/ydb/aio/resolver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/aio/scheme.py` & `ydb-3.3.1/ydb/aio/scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/aio/table.py` & `ydb-3.3.1/ydb/aio/table.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/connection.py` & `ydb-3.3.1/ydb/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/convert.py` & `ydb-3.3.1/ydb/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,16 @@
     "decimal_type": _pb_to_decimal,
     "optional_type": _pb_to_optional,
     "list_type": _pb_to_list,
     "tuple_type": _pb_to_tuple,
     "dict_type": _pb_to_dict,
     "struct_type": _pb_to_struct,
     "void_type": _pb_to_void,
+    "empty_list_type": _pb_to_list,
+    "empty_dict_type": _pb_to_dict,
 }
 
 
 def _to_native_value(type_pb, value_pb, table_client_settings=None):
     return _to_native_map.get(type_pb.WhichOneof("type"))(type_pb, value_pb, table_client_settings)
 
 
@@ -291,15 +293,15 @@
         self.rows = rows
         self.truncated = truncated
         self.snapshot = snapshot
 
     @classmethod
     def from_message(cls, message, table_client_settings=None, snapshot=None):
         rows = []
-        # prepare columnn parsers before actuall parsing
+        # prepare column parsers before actuall parsing
         column_parsers = []
         if len(message.rows) > 0:
             for column in message.columns:
                 column_parsers.append(_unwrap_optionality(column))
 
         for row_proto in message.rows:
             row = _Row(message.columns)
```

### Comparing `ydb-3.3.0/ydb/credentials.py` & `ydb-3.3.1/ydb/credentials.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/dbapi/__init__.py` & `ydb-3.3.1/ydb/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/dbapi/connection.py` & `ydb-3.3.1/ydb/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/dbapi/cursor.py` & `ydb-3.3.1/ydb/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/dbapi/errors.py` & `ydb-3.3.1/ydb/dbapi/errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/default_pem.py` & `ydb-3.3.1/ydb/default_pem.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/driver.py` & `ydb-3.3.1/ydb/driver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/export.py` & `ydb-3.3.1/ydb/export.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/global_settings.py` & `ydb-3.3.1/ydb/global_settings.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/iam/auth.py` & `ydb-3.3.1/ydb/iam/auth.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/import_client.py` & `ydb-3.3.1/ydb/import_client.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/interceptor.py` & `ydb-3.3.1/ydb/interceptor.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/issues.py` & `ydb-3.3.1/ydb/issues.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/operation.py` & `ydb-3.3.1/ydb/operation.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/pool.py` & `ydb-3.3.1/ydb/pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/resolver.py` & `ydb-3.3.1/ydb/resolver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/scheme.py` & `ydb-3.3.1/ydb/scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/scheme_test.py` & `ydb-3.3.1/ydb/scheme_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/scripting.py` & `ydb-3.3.1/ydb/scripting.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/settings.py` & `ydb-3.3.1/ydb/settings.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/sqlalchemy/__init__.py` & `ydb-3.3.1/ydb/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/sqlalchemy/types.py` & `ydb-3.3.1/ydb/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/table.py` & `ydb-3.3.1/ydb/table.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/table_test.py` & `ydb-3.3.1/ydb/table_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/topic.py` & `ydb-3.3.1/ydb/topic.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/tracing.py` & `ydb-3.3.1/ydb/tracing.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb/types.py` & `ydb-3.3.1/ydb/types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.0/ydb.egg-info/PKG-INFO` & `ydb-3.3.1/ydb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydb
-Version: 3.3.0
+Version: 3.3.1
 Summary: YDB Python SDK
 Home-page: http://github.com/ydb-platform/ydb-python-sdk
 Author: Yandex LLC
 Author-email: ydb@yandex-team.ru
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ydb-3.3.0/ydb.egg-info/SOURCES.txt` & `ydb-3.3.1/ydb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

