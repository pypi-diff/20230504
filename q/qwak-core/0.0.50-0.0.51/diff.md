# Comparing `tmp/qwak_core-0.0.50.tar.gz` & `tmp/qwak_core-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.50.tar", max compression
+gzip compressed data, was "qwak_core-0.0.51.tar", max compression
```

## Comparing `qwak_core-0.0.50.tar` & `qwak_core-0.0.51.tar`

### file list

```diff
@@ -1,567 +1,570 @@
--rw-r--r--   0        0        0      264 2023-05-03 15:38:01.521046 qwak_core-0.0.50/README.md
--rw-r--r--   0        0        0        0 2023-05-03 15:39:37.137487 qwak_core-0.0.50/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-03 15:39:37.161487 qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-03 15:39:18.697405 qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.161487 qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-03 15:39:37.157487 qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-03 15:39:18.357404 qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.157487 qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-03 15:39:37.157487 qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-03 15:39:18.525404 qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.157487 qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-03 15:39:37.149487 qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-03 15:39:17.861401 qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-03 15:39:37.149487 qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-03 15:39:37.153487 qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-03 15:39:18.029402 qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.153487 qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-03 15:39:37.153487 qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-03 15:39:18.193403 qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.153487 qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-03 15:39:37.137487 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-03 15:39:17.693401 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-03 15:39:37.141487 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-03 15:39:37.141487 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-03 15:39:18.865406 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.141487 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-03 15:39:37.145487 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-03 15:39:19.201407 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.145487 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-03 15:39:37.145487 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-03 15:39:19.369408 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-03 15:39:37.149487 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-03 15:39:37.141487 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-03 15:39:19.033407 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.145487 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-03 15:39:37.149487 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-03 15:39:19.537409 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.149487 qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-03 15:39:37.185487 qwak_core-0.0.50/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-03 15:39:21.905419 qwak_core-0.0.50/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.185487 qwak_core-0.0.50/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-03 15:39:37.189487 qwak_core-0.0.50/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-03 15:39:22.073420 qwak_core-0.0.50/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-03 15:39:37.189487 qwak_core-0.0.50/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-03 15:39:37.249488 qwak_core-0.0.50/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-03 15:39:26.789441 qwak_core-0.0.50/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.249488 qwak_core-0.0.50/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-03 15:39:37.249488 qwak_core-0.0.50/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-03 15:39:26.957441 qwak_core-0.0.50/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-03 15:39:37.249488 qwak_core-0.0.50/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-03 15:39:37.253488 qwak_core-0.0.50/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-03 15:39:27.813445 qwak_core-0.0.50/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-03 15:39:37.253488 qwak_core-0.0.50/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-03 15:39:37.253488 qwak_core-0.0.50/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-03 15:39:27.641444 qwak_core-0.0.50/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.253488 qwak_core-0.0.50/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-05-03 15:39:37.257488 qwak_core-0.0.50/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-05-03 15:39:27.981446 qwak_core-0.0.50/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.257488 qwak_core-0.0.50/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-03 15:39:37.257488 qwak_core-0.0.50/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-03 15:39:28.149447 qwak_core-0.0.50/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-03 15:39:37.257488 qwak_core-0.0.50/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    11441 2023-05-03 15:39:37.313488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    17892 2023-05-03 15:39:32.981468 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.313488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-05-03 15:39:37.309488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-05-03 15:39:32.645467 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.309488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-03 15:39:37.309488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-03 15:39:32.813468 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.313488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-03 15:39:37.305488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-03 15:39:32.297465 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-03 15:39:37.305488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-03 15:39:37.305488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-03 15:39:32.473466 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.309488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-03 15:39:37.317488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-03 15:39:33.481470 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.321488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-03 15:39:37.317488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-03 15:39:33.317470 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.317488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-03 15:39:37.313488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-03 15:39:33.149469 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.317488 qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-03 15:39:37.353488 qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-03 15:39:36.561484 qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.353488 qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-03 15:39:37.349488 qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-03 15:39:36.205483 qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.349488 qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    37419 2023-05-03 15:39:37.353488 qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    48027 2023-05-03 15:39:36.393484 qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-03 15:39:37.353488 qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-03 15:39:37.281488 qwak_core-0.0.50/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-03 15:39:29.885454 qwak_core-0.0.50/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-03 15:39:37.281488 qwak_core-0.0.50/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-03 15:39:37.281488 qwak_core-0.0.50/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-03 15:39:29.713453 qwak_core-0.0.50/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.281488 qwak_core-0.0.50/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-03 15:39:37.273488 qwak_core-0.0.50/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-03 15:39:29.369452 qwak_core-0.0.50/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.273488 qwak_core-0.0.50/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-03 15:39:37.273488 qwak_core-0.0.50/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-03 15:39:29.541453 qwak_core-0.0.50/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.273488 qwak_core-0.0.50/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-03 15:39:37.277488 qwak_core-0.0.50/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-03 15:39:30.057455 qwak_core-0.0.50/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-03 15:39:37.277488 qwak_core-0.0.50/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-03 15:39:37.277488 qwak_core-0.0.50/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-03 15:39:30.425457 qwak_core-0.0.50/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-03 15:39:37.277488 qwak_core-0.0.50/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-03 15:39:37.289488 qwak_core-0.0.50/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-03 15:39:30.777458 qwak_core-0.0.50/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.289488 qwak_core-0.0.50/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-03 15:39:37.289488 qwak_core-0.0.50/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-03 15:39:30.945459 qwak_core-0.0.50/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-03 15:39:37.289488 qwak_core-0.0.50/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-03 15:39:37.265488 qwak_core-0.0.50/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-03 15:39:28.849450 qwak_core-0.0.50/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.265488 qwak_core-0.0.50/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-03 15:39:37.269488 qwak_core-0.0.50/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-03 15:39:29.017450 qwak_core-0.0.50/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-03 15:39:37.269488 qwak_core-0.0.50/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-03 15:39:37.261488 qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-03 15:39:28.505448 qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.261488 qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-05-03 15:39:37.261488 qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-05-03 15:39:28.329447 qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.261488 qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-03 15:39:37.265488 qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-03 15:39:28.681449 qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-03 15:39:37.265488 qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-03 15:39:37.177487 qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-03 15:39:21.053415 qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.177487 qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-03 15:39:37.177487 qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-03 15:39:21.225416 qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.181487 qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-03 15:39:37.181487 qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-03 15:39:21.397417 qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-03 15:39:37.181487 qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-03 15:39:37.229488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-03 15:39:25.749436 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.233488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-03 15:39:37.229488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-03 15:39:25.581435 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-03 15:39:37.229488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-03 15:39:37.213487 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-03 15:39:24.229429 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.213487 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-03 15:39:37.209488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-03 15:39:24.061429 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.213487 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-03 15:39:37.205487 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-03 15:39:23.537426 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.205487 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-05-03 15:39:37.209488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-05-03 15:39:23.893428 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-05-03 15:39:37.209488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-03 15:39:37.213487 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-03 15:39:24.401430 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.217487 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-03 15:39:37.217487 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-03 15:39:24.569431 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-03 15:39:37.217487 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    24876 2023-05-03 15:39:37.205487 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    36861 2023-05-03 15:39:23.717427 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.209488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-03 15:39:37.217487 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-03 15:39:24.737432 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.221488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-03 15:39:37.233488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-03 15:39:36.729485 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.233488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-03 15:39:37.233488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-03 15:39:36.901486 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-03 15:39:37.237488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-03 15:39:37.237488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-03 15:39:26.253438 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.237488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-03 15:39:37.237488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-03 15:39:26.453439 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-03 15:39:37.241488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-03 15:39:37.241488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-03 15:39:26.621440 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.241488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-03 15:39:37.245488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-03 15:39:27.297443 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.245488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-03 15:39:37.241488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-03 15:39:27.129442 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-03 15:39:37.245488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-03 15:39:37.245488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-03 15:39:27.469444 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.249488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-03 15:39:37.221488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-03 15:39:24.905432 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.221488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-03 15:39:37.221488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-03 15:39:25.073433 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.225488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-03 15:39:37.225488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-03 15:39:25.245434 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-03 15:39:37.225488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-03 15:39:37.225488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-03 15:39:25.413435 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.229488 qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-03 15:39:37.321488 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-03 15:39:33.649471 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.321488 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-03 15:39:37.321488 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-03 15:39:33.817472 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-03 15:39:37.325488 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-03 15:39:37.325488 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-03 15:39:33.985473 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.325488 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-03 15:39:37.325488 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-03 15:39:34.157474 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-03 15:39:37.325488 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-03 15:39:37.329488 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-03 15:39:34.333474 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-03 15:39:37.329488 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-03 15:39:37.329488 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-03 15:39:34.501475 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.329488 qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-03 15:39:37.293488 qwak_core-0.0.50/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-03 15:39:31.113460 qwak_core-0.0.50/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.293488 qwak_core-0.0.50/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-03 15:39:37.293488 qwak_core-0.0.50/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-03 15:39:31.281461 qwak_core-0.0.50/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-03 15:39:37.293488 qwak_core-0.0.50/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-03 15:39:37.193488 qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-03 15:39:22.853423 qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.193488 qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-03 15:39:37.193488 qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-03 15:39:23.021424 qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.197487 qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-03 15:39:37.197487 qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-03 15:39:23.193425 qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-03 15:39:37.201487 qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-03 15:39:37.201487 qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-03 15:39:23.361426 qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.205487 qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-03 15:39:37.269488 qwak_core-0.0.50/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-03 15:39:29.185451 qwak_core-0.0.50/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-03 15:39:37.269488 qwak_core-0.0.50/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-03 15:39:37.333488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-03 15:39:34.669476 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.333488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-03 15:39:37.333488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-03 15:39:34.833477 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.333488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-03 15:39:37.337488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-03 15:39:35.005478 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.337488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-03 15:39:37.337488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-03 15:39:35.177478 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.337488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-03 15:39:37.341488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-03 15:39:35.353479 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.341488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-03 15:39:37.341488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-03 15:39:35.537480 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-03 15:39:37.341488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-03 15:39:37.345488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-03 15:39:35.705481 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.345488 qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-03 15:39:37.297488 qwak_core-0.0.50/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-03 15:39:31.621462 qwak_core-0.0.50/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.297488 qwak_core-0.0.50/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-03 15:39:37.301488 qwak_core-0.0.50/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-03 15:39:32.125464 qwak_core-0.0.50/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.305488 qwak_core-0.0.50/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-03 15:39:37.301488 qwak_core-0.0.50/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-03 15:39:31.789463 qwak_core-0.0.50/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-03 15:39:37.301488 qwak_core-0.0.50/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-05-03 15:39:37.301488 qwak_core-0.0.50/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-05-03 15:39:31.957464 qwak_core-0.0.50/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.301488 qwak_core-0.0.50/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-03 15:39:37.285488 qwak_core-0.0.50/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-03 15:39:30.609457 qwak_core-0.0.50/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-03 15:39:37.285488 qwak_core-0.0.50/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-03 15:39:37.173487 qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-03 15:39:22.469422 qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-03 15:39:37.173487 qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-03 15:39:37.169487 qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-03 15:39:22.265421 qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.173487 qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-03 15:39:37.173487 qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-03 15:39:22.673423 qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-03 15:39:37.177487 qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-03 15:39:37.285488 qwak_core-0.0.50/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-03 15:39:30.237456 qwak_core-0.0.50/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-03 15:39:37.285488 qwak_core-0.0.50/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-03 15:39:37.297488 qwak_core-0.0.50/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-03 15:39:31.449461 qwak_core-0.0.50/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-03 15:39:37.297488 qwak_core-0.0.50/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-03 15:39:37.169487 qwak_core-0.0.50/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-03 15:39:20.381413 qwak_core-0.0.50/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.169487 qwak_core-0.0.50/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-03 15:39:37.165487 qwak_core-0.0.50/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-03 15:39:20.213412 qwak_core-0.0.50/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-03 15:39:37.169487 qwak_core-0.0.50/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-03 15:39:37.161487 qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-03 15:39:19.705410 qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.161487 qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-03 15:39:37.161487 qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-03 15:39:19.873410 qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.165487 qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-03 15:39:37.165487 qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-03 15:39:20.041411 qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-03 15:39:37.165487 qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-03 15:39:37.349488 qwak_core-0.0.50/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-03 15:39:36.041482 qwak_core-0.0.50/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-03 15:39:37.349488 qwak_core-0.0.50/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-03 15:39:37.345488 qwak_core-0.0.50/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-03 15:39:35.873481 qwak_core-0.0.50/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.345488 qwak_core-0.0.50/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0     4083 2023-05-03 15:39:37.181487 qwak_core-0.0.50/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0     4036 2023-05-03 15:39:21.565418 qwak_core-0.0.50/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.185487 qwak_core-0.0.50/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-03 15:39:37.185487 qwak_core-0.0.50/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-03 15:39:21.733419 qwak_core-0.0.50/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:39:37.185487 qwak_core-0.0.50/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-03 15:39:38.493493 qwak_core-0.0.50/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-03 15:39:38.493493 qwak_core-0.0.50/qwak/__init__.py
--rw-r--r--   0        0        0     1204 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    32539 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.521046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9480 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6071 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-03 15:38:01.525046 qwak_core-0.0.50/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-03 15:38:01.529046 qwak_core-0.0.50/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.50/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.50/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-04 10:31:55.182051 qwak_core-0.0.51/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 10:33:36.606639 qwak_core-0.0.51/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-04 10:33:36.630639 qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-04 10:33:15.310514 qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.634639 qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-04 10:33:36.626639 qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-04 10:33:14.914512 qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.630639 qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-04 10:33:36.630639 qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-04 10:33:15.114513 qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.630639 qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-04 10:33:36.622639 qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-04 10:33:14.318509 qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-04 10:33:36.622639 qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-04 10:33:36.622639 qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-04 10:33:14.514510 qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.626639 qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-04 10:33:36.626639 qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-04 10:33:14.714511 qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.626639 qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-04 10:33:36.606639 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-04 10:33:14.122507 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-04 10:33:36.610639 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-04 10:33:36.610639 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-04 10:33:15.514515 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.610639 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-04 10:33:36.614639 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-04 10:33:15.914518 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.614639 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-04 10:33:36.618639 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-04 10:33:16.110519 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-04 10:33:36.618639 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-04 10:33:36.610639 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-04 10:33:15.714517 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.614639 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-04 10:33:36.618639 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-04 10:33:16.302520 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.618639 qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-04 10:33:36.662639 qwak_core-0.0.51/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-04 10:33:19.002536 qwak_core-0.0.51/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.666639 qwak_core-0.0.51/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-04 10:33:36.666639 qwak_core-0.0.51/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-04 10:33:19.206537 qwak_core-0.0.51/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-04 10:33:36.666639 qwak_core-0.0.51/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-04 10:33:36.742640 qwak_core-0.0.51/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-04 10:33:24.766569 qwak_core-0.0.51/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.742640 qwak_core-0.0.51/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-04 10:33:36.746640 qwak_core-0.0.51/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-04 10:33:24.958571 qwak_core-0.0.51/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-04 10:33:36.746640 qwak_core-0.0.51/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-04 10:33:36.750640 qwak_core-0.0.51/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-04 10:33:25.918576 qwak_core-0.0.51/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-04 10:33:36.750640 qwak_core-0.0.51/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-04 10:33:36.746640 qwak_core-0.0.51/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-04 10:33:25.730575 qwak_core-0.0.51/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.746640 qwak_core-0.0.51/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-05-04 10:33:36.750640 qwak_core-0.0.51/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-05-04 10:33:26.110577 qwak_core-0.0.51/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.754640 qwak_core-0.0.51/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-04 10:33:36.754640 qwak_core-0.0.51/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-04 10:33:26.306578 qwak_core-0.0.51/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-04 10:33:36.754640 qwak_core-0.0.51/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11441 2023-05-04 10:33:36.818640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    17892 2023-05-04 10:33:31.786611 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.818640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-05-04 10:33:36.814640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-05-04 10:33:31.398609 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.814640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-04 10:33:36.814640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-04 10:33:31.590610 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.818640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-04 10:33:36.810640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-04 10:33:31.014606 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-04 10:33:36.810640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-04 10:33:36.810640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-04 10:33:31.210607 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.810640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-04 10:33:36.826640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-04 10:33:32.354614 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.826640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-04 10:33:36.822640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-04 10:33:32.166613 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.822640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-04 10:33:36.818640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-04 10:33:31.974612 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.822640 qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-04 10:33:36.866641 qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-04 10:33:35.926635 qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.866641 qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-04 10:33:36.862640 qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-04 10:33:35.518633 qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.862640 qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    37419 2023-05-04 10:33:36.862640 qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    48027 2023-05-04 10:33:35.726634 qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-04 10:33:36.862640 qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-05-04 10:33:36.782640 qwak_core-0.0.51/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-05-04 10:33:28.246590 qwak_core-0.0.51/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-05-04 10:33:36.782640 qwak_core-0.0.51/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-04 10:33:36.778640 qwak_core-0.0.51/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-04 10:33:28.054589 qwak_core-0.0.51/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.778640 qwak_core-0.0.51/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-04 10:33:36.770640 qwak_core-0.0.51/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-04 10:33:27.674587 qwak_core-0.0.51/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.770640 qwak_core-0.0.51/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-04 10:33:36.770640 qwak_core-0.0.51/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-04 10:33:27.862588 qwak_core-0.0.51/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.774640 qwak_core-0.0.51/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-04 10:33:36.774640 qwak_core-0.0.51/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-04 10:33:28.438591 qwak_core-0.0.51/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-04 10:33:36.774640 qwak_core-0.0.51/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-04 10:33:36.778640 qwak_core-0.0.51/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-04 10:33:28.854593 qwak_core-0.0.51/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-04 10:33:36.778640 qwak_core-0.0.51/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-04 10:33:36.786640 qwak_core-0.0.51/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-04 10:33:29.262596 qwak_core-0.0.51/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.790640 qwak_core-0.0.51/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-04 10:33:36.790640 qwak_core-0.0.51/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-04 10:33:29.462597 qwak_core-0.0.51/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-04 10:33:36.790640 qwak_core-0.0.51/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-04 10:33:36.762640 qwak_core-0.0.51/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-04 10:33:27.102583 qwak_core-0.0.51/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.762640 qwak_core-0.0.51/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-04 10:33:36.766640 qwak_core-0.0.51/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-04 10:33:27.290584 qwak_core-0.0.51/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-04 10:33:36.766640 qwak_core-0.0.51/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-04 10:33:36.758640 qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-04 10:33:26.706581 qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.758640 qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    42956 2023-05-04 10:33:36.754640 qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    62847 2023-05-04 10:33:26.514580 qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.758640 qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-04 10:33:36.762640 qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-04 10:33:26.910582 qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-04 10:33:36.762640 qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-04 10:33:36.650639 qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-04 10:33:18.054530 qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.654639 qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-04 10:33:36.654639 qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-04 10:33:18.246532 qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.654639 qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-04 10:33:36.658639 qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-04 10:33:18.438533 qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-04 10:33:36.658639 qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-04 10:33:36.722640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-04 10:33:23.602563 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.722640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-04 10:33:36.718640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-04 10:33:23.406561 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-04 10:33:36.722640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-04 10:33:36.698639 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-04 10:33:21.650551 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.702640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-04 10:33:36.698639 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-04 10:33:21.458550 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.698639 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-04 10:33:36.690640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-04 10:33:20.838547 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.690640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-05-04 10:33:36.694640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-05-04 10:33:21.262549 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-05-04 10:33:36.694640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-04 10:33:36.702640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-04 10:33:21.842553 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.702640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-04 10:33:36.702640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-04 10:33:22.034554 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-04 10:33:36.706640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25213 2023-05-04 10:33:36.690640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37366 2023-05-04 10:33:21.046548 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.694640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-04 10:33:36.706640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-04 10:33:22.222555 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.706640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     5958 2023-05-04 10:33:36.710640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py
+-rw-r--r--   0        0        0     6232 2023-05-04 10:33:22.414556 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.710640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-04 10:33:36.726640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-04 10:33:36.118636 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.726640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-04 10:33:36.726640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-04 10:33:36.322637 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-04 10:33:36.726640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-04 10:33:36.730640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-04 10:33:24.194566 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.730640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-04 10:33:36.730640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-04 10:33:24.386567 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-04 10:33:36.730640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-04 10:33:36.734640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-04 10:33:24.578568 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.734640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-04 10:33:36.738640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-04 10:33:25.350573 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.738640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-04 10:33:36.734640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-04 10:33:25.154572 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-04 10:33:36.738640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-04 10:33:36.738640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-04 10:33:25.538574 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.742640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-04 10:33:36.710640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-04 10:33:22.610557 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.710640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-04 10:33:36.714640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-04 10:33:22.806558 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.714640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-04 10:33:36.714640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-04 10:33:23.006559 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-04 10:33:36.718640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-04 10:33:36.718640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-04 10:33:23.206560 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.718640 qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-04 10:33:36.826640 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-04 10:33:32.546615 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.826640 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-04 10:33:36.830640 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-04 10:33:32.734616 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-04 10:33:36.830640 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-04 10:33:36.830640 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-04 10:33:32.930617 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.834640 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-04 10:33:36.834640 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-04 10:33:33.130619 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-04 10:33:36.834640 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-04 10:33:36.834640 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-04 10:33:33.330620 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-04 10:33:36.838640 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-04 10:33:36.838640 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-04 10:33:33.522621 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.838640 qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-04 10:33:36.794640 qwak_core-0.0.51/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-04 10:33:29.654598 qwak_core-0.0.51/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.794640 qwak_core-0.0.51/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-04 10:33:36.794640 qwak_core-0.0.51/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-04 10:33:29.858599 qwak_core-0.0.51/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-04 10:33:36.794640 qwak_core-0.0.51/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-04 10:33:36.670639 qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-04 10:33:20.050542 qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.670639 qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-04 10:33:36.674640 qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-04 10:33:20.238543 qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.678640 qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-04 10:33:36.678640 qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-04 10:33:20.430544 qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-04 10:33:36.682639 qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-04 10:33:36.686640 qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-04 10:33:20.638545 qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.690640 qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-04 10:33:36.766640 qwak_core-0.0.51/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-04 10:33:27.482585 qwak_core-0.0.51/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-04 10:33:36.770640 qwak_core-0.0.51/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-04 10:33:36.838640 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-04 10:33:33.714622 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.842640 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-04 10:33:36.842640 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-04 10:33:33.910623 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.842640 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-04 10:33:36.846640 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-04 10:33:34.110624 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.846640 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-04 10:33:36.846640 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-04 10:33:34.306625 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.846640 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-04 10:33:36.850640 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-04 10:33:34.506627 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.850640 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-04 10:33:36.850640 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-04 10:33:34.718628 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-04 10:33:36.854641 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-04 10:33:36.854641 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-04 10:33:34.914629 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.854641 qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-04 10:33:36.798640 qwak_core-0.0.51/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-04 10:33:30.242602 qwak_core-0.0.51/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.802640 qwak_core-0.0.51/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-04 10:33:36.806640 qwak_core-0.0.51/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-04 10:33:30.818605 qwak_core-0.0.51/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.806640 qwak_core-0.0.51/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-04 10:33:36.802640 qwak_core-0.0.51/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-04 10:33:30.438603 qwak_core-0.0.51/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-04 10:33:36.802640 qwak_core-0.0.51/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-05-04 10:33:36.806640 qwak_core-0.0.51/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-05-04 10:33:30.630604 qwak_core-0.0.51/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.806640 qwak_core-0.0.51/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-04 10:33:36.786640 qwak_core-0.0.51/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-04 10:33:29.062595 qwak_core-0.0.51/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-04 10:33:36.786640 qwak_core-0.0.51/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-04 10:33:36.646639 qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-04 10:33:19.642540 qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-04 10:33:36.650639 qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-04 10:33:36.646639 qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-04 10:33:19.418538 qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.646639 qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-04 10:33:36.650639 qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-04 10:33:19.854541 qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-04 10:33:36.650639 qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-04 10:33:36.782640 qwak_core-0.0.51/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-04 10:33:28.642592 qwak_core-0.0.51/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-04 10:33:36.786640 qwak_core-0.0.51/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-04 10:33:36.798640 qwak_core-0.0.51/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-04 10:33:30.050600 qwak_core-0.0.51/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-04 10:33:36.798640 qwak_core-0.0.51/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-04 10:33:36.642639 qwak_core-0.0.51/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-04 10:33:17.262526 qwak_core-0.0.51/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.646639 qwak_core-0.0.51/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-04 10:33:36.642639 qwak_core-0.0.51/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-04 10:33:17.074525 qwak_core-0.0.51/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-04 10:33:36.642639 qwak_core-0.0.51/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-04 10:33:36.634639 qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-04 10:33:16.494521 qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.634639 qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-04 10:33:36.638639 qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-04 10:33:16.686522 qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.638639 qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-04 10:33:36.638639 qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-04 10:33:16.882524 qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-04 10:33:36.638639 qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-04 10:33:36.858641 qwak_core-0.0.51/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-04 10:33:35.318632 qwak_core-0.0.51/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-04 10:33:36.858641 qwak_core-0.0.51/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-04 10:33:36.854641 qwak_core-0.0.51/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-04 10:33:35.114630 qwak_core-0.0.51/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.858641 qwak_core-0.0.51/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0     4083 2023-05-04 10:33:36.658639 qwak_core-0.0.51/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0     4036 2023-05-04 10:33:18.626534 qwak_core-0.0.51/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.658639 qwak_core-0.0.51/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-04 10:33:36.662639 qwak_core-0.0.51/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-04 10:33:18.810535 qwak_core-0.0.51/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-04 10:33:36.662639 qwak_core-0.0.51/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-04 10:33:39.094654 qwak_core-0.0.51/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-04 10:33:39.094654 qwak_core-0.0.51/qwak/__init__.py
+-rw-r--r--   0        0        0     1204 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    32539 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.186051 qwak_core-0.0.51/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9480 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6071 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-04 10:31:55.190051 qwak_core-0.0.51/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-04 10:31:55.194051 qwak_core-0.0.51/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.51/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.51/PKG-INFO
```

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from _qwak_proto.qwak.feature_store.sources import batch_pb2 as qwak_dot_feature__store_dot_sources_dot_batch__pb2
 from _qwak_proto.qwak.feature_store.sources import streaming_pb2 as qwak_dot_feature__store_dot_sources_dot_streaming__pb2
 from _qwak_proto.qwak.feature_store.features import execution_pb2 as qwak_dot_feature__store_dot_features_dot_execution__pb2
 from _qwak_proto.qwak.feature_store.features import aggregation_pb2 as qwak_dot_feature__store_dot_features_dot_aggregation__pb2
 from _qwak_proto.qwak.feature_store.features import monitoring_pb2 as qwak_dot_feature__store_dot_features_dot_monitoring__pb2
+from _qwak_proto.qwak.feature_store.features import real_time_feature_set_type_pb2 as qwak_dot_feature__store_dot_features_dot_real__time__feature__set__type__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3qwak/feature_store/features/feature_set_types.proto\x12\x1bqwak.feature.store.features\x1a\x1fgoogle/protobuf/timestamp.proto\x1a&qwak/feature_store/sources/batch.proto\x1a*qwak/feature_store/sources/streaming.proto\x1a+qwak/feature_store/features/execution.proto\x1a-qwak/feature_store/features/aggregation.proto\x1a,qwak/feature_store/features/monitoring.proto\"\x9f\x04\n\x0e\x46\x65\x61tureSetType\x12I\n\x11\x62\x61tch_feature_set\x18\x05 \x01(\x0b\x32,.qwak.feature.store.features.BatchFeatureSetH\x00\x12Q\n\x16on_the_fly_feature_set\x18\x06 \x01(\x0b\x32/.qwak.feature.store.features.OnTheFlyFeatureSetH\x00\x12Q\n\x15streaming_feature_set\x18\x07 \x01(\x0b\x32\x30.qwak.feature.store.features.StreamingFeatureSetH\x00\x12V\n\x18streaming_feature_set_v1\x18\x08 \x01(\x0b\x32\x32.qwak.feature.store.features.StreamingFeatureSetV1H\x00\x12N\n\x14\x62\x61tch_feature_set_v1\x18\t \x01(\x0b\x32..qwak.feature.store.features.BatchFeatureSetV1H\x00\x12h\n!streaming_aggregation_feature_set\x18\n \x01(\x0b\x32;.qwak.feature.store.features.StreamingAggregationFeatureSetH\x00\x42\n\n\x08set_type\"\x9d\x03\n\x0f\x42\x61tchFeatureSet\x12\x19\n\x11scheduling_policy\x18\x01 \x01(\t\x12\x41\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\'.qwak.feature.store.sources.BatchSourceB\x02\x18\x01\x12\x37\n\x08\x62\x61\x63kfill\x18\x03 \x01(\x0b\x32%.qwak.feature.store.features.Backfill\x12\x37\n\x08\x66unction\x18\x04 \x01(\x0b\x32%.qwak.feature.store.features.Function\x12U\n\x19\x66\x65\x61ture_set_batch_sources\x18\x05 \x03(\x0b\x32\x32.qwak.feature.store.features.FeatureSetBatchSource\x12\x63\n\x19monitoring_configurations\x18\x06 \x01(\x0b\x32@.qwak.feature.store.features.monitoring.MonitoringConfigurations\"\xe5\x04\n\x11\x42\x61tchFeatureSetV1\x12\x19\n\x11scheduling_policy\x18\x01 \x01(\t\x12\x37\n\x08\x62\x61\x63kfill\x18\x02 \x01(\x0b\x32%.qwak.feature.store.features.Backfill\x12;\n\x08\x66unction\x18\x03 \x01(\x0b\x32%.qwak.feature.store.features.FunctionB\x02\x18\x01\x12U\n\x19\x66\x65\x61ture_set_batch_sources\x18\x04 \x03(\x0b\x32\x32.qwak.feature.store.features.FeatureSetBatchSource\x12L\n\x0e\x65xecution_spec\x18\x05 \x01(\x0b\x32\x34.qwak.feature.store.features.execution.ExecutionSpec\x12\x14\n\x0coffline_sink\x18\x06 \x01(\x08\x12\x13\n\x0bonline_sink\x18\x07 \x01(\x08\x12\x63\n\x19monitoring_configurations\x18\x08 \x01(\x0b\x32@.qwak.feature.store.features.monitoring.MonitoringConfigurations\x12\x1d\n\x15timestamp_column_name\x18\t \x01(\t\x12\x43\n\x0etransformation\x18\n \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12&\n\x1eqwak_internal_protocol_version\x18\x0b \x01(\x05\"\x9d\x01\n\x15\x46\x65\x61tureSetBatchSource\x12<\n\x0b\x64\x61ta_source\x18\x01 \x01(\x0b\x32\'.qwak.feature.store.sources.BatchSource\x12\x46\n\x0bread_policy\x18\x02 \x01(\x0b\x32\x31.qwak.feature.store.features.DataSourceReadPolicy\"X\n\x13StreamingFeatureSet\x12\x41\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32+.qwak.feature.store.sources.StreamingSource\"\x81\x03\n\x15StreamingFeatureSetV1\x12\x41\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32+.qwak.feature.store.sources.StreamingSource\x12\x43\n\x0etransformation\x18\x02 \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12U\n\x0e\x65xecution_spec\x18\x03 \x01(\x0b\x32=.qwak.feature.store.features.execution.StreamingExecutionSpec\x12\x1d\n\x15timestamp_column_name\x18\x04 \x01(\t\x12\x1f\n\x17online_trigger_interval\x18\x05 \x01(\x05\x12!\n\x19offline_scheduling_policy\x18\x06 \x01(\t\x12&\n\x1eqwak_internal_protocol_version\x18\x07 \x01(\x05\"\x97\x04\n\x1eStreamingAggregationFeatureSet\x12\x41\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32+.qwak.feature.store.sources.StreamingSource\x12\x43\n\x0etransformation\x18\x02 \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12U\n\x0e\x65xecution_spec\x18\x03 \x01(\x0b\x32=.qwak.feature.store.features.execution.StreamingExecutionSpec\x12\x1d\n\x15timestamp_column_name\x18\x04 \x01(\t\x12\x1f\n\x17online_trigger_interval\x18\x05 \x01(\x05\x12$\n\x1c\x63ompaction_scheduling_policy\x18\x06 \x01(\t\x12\x46\n\x10\x61ggregation_spec\x18\x07 \x01(\x0b\x32,.qwak.feature.store.features.AggregationSpec\x12@\n\rbackfill_spec\x18\x08 \x01(\x0b\x32).qwak.feature.store.features.BackfillSpec\x12&\n\x1eqwak_internal_protocol_version\x18\t \x01(\x05\"\xc3\x01\n\x1b\x42\x61\x63kfillBatchDataSourceSpec\x12<\n\x0b\x64\x61ta_source\x18\x01 \x01(\x0b\x32\'.qwak.feature.store.sources.BatchSource\x12\x33\n\x0fstart_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"|\n\x16\x42\x61\x63kfillDataSourceSpec\x12Z\n\x16\x62\x61tch_data_source_spec\x18\x01 \x01(\x0b\x32\x38.qwak.feature.store.features.BackfillBatchDataSourceSpecH\x00\x42\x06\n\x04type\"\xe1\x02\n\x0c\x42\x61\x63kfillSpec\x12T\n\x0e\x65xecution_spec\x18\x01 \x01(\x0b\x32<.qwak.feature.store.features.execution.BackfillExecutionSpec\x12\x33\n\x0fstart_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\x0etransformation\x18\x04 \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12N\n\x11\x64\x61ta_source_specs\x18\x05 \x03(\x0b\x32\x33.qwak.feature.store.features.BackfillDataSourceSpec\"\x9f\x01\n\x0f\x41ggregationSpec\x12O\n\x0c\x61ggregations\x18\x01 \x03(\x0b\x32\x39.qwak.feature.store.features.aggregation.AggregationField\x12\x15\n\rslide_seconds\x18\x02 \x01(\x05\x12$\n\x1c\x61llowed_late_arrival_seconds\x18\x03 \x01(\x05\"\x9f\x02\n\x0eTransformation\x12L\n\x12udf_transformation\x18\x01 \x01(\x0b\x32..qwak.feature.store.features.UdfTransformationH\x00\x12L\n\x12sql_transformation\x18\x02 \x01(\x0b\x32..qwak.feature.store.features.SqlTransformationH\x00\x12R\n\x15koalas_transformation\x18\x03 \x01(\x0b\x32\x31.qwak.feature.store.features.KoalasTransformationH\x00\x12\x15\n\rartifact_path\x18\x04 \x01(\tB\x06\n\x04type\"*\n\x11UdfTransformation\x12\x15\n\rfunction_name\x18\x01 \x01(\t\"8\n\x11SqlTransformation\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x16\n\x0e\x66unction_names\x18\x02 \x03(\t\"-\n\x14KoalasTransformation\x12\x15\n\rfunction_name\x18\x01 \x01(\t\"f\n\x12OnTheFlyFeatureSet\x12:\n\x08\x66unction\x18\x01 \x01(\x0b\x32(.qwak.feature.store.features.UdfFunction\x12\x14\n\x0crequirements\x18\x02 \x01(\x0c\"\x96\x01\n\x08\x46unction\x12@\n\x0csql_function\x18\x01 \x01(\x0b\x32(.qwak.feature.store.features.SqlFunctionH\x00\x12@\n\x0cudf_function\x18\x02 \x01(\x0b\x32(.qwak.feature.store.features.UdfFunctionH\x00\x42\x06\n\x04type\"\xb5\x01\n\x08\x42\x61\x63kfill\x12.\n\nstart_date\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\rfillup_method\x18\x02 \x01(\x0e\x32\x32.qwak.feature.store.features.Backfill.FillUpMethod\".\n\x0c\x46illUpMethod\x12\x10\n\x0c\x41S_SCHEDULED\x10\x00\x12\x0c\n\x08SNAPSHOT\x10\x01\"\x1a\n\x0bSqlFunction\x12\x0b\n\x03sql\x18\x01 \x01(\t\"\x1b\n\x0bUdfFunction\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x0c\"\t\n\x07NewOnly\"\xa0\x01\n\tTimeFrame\x12\x0f\n\x07minutes\x18\x01 \x01(\x05\x12\x37\n\x07vanilla\x18\x02 \x01(\x0b\x32$.qwak.feature.store.features.VanillaH\x00\x12?\n\x0b\x61ggregation\x18\x03 \x01(\x0b\x32(.qwak.feature.store.features.AggregationH\x00\x42\x08\n\x06\x66lavor\"k\n\x0b\x41ggregation\x12T\n\x16\x61ggregation_population\x18\x01 \x01(\x0b\x32\x32.qwak.feature.store.features.AggregationPopulationH\x00\x42\x06\n\x04type\"\x17\n\x15\x41ggregationPopulation\"\x1c\n\x1aPopulationTimeframeNewOnly\"j\n\x13PopulationTimeframe\x12K\n\x08new_only\x18\x01 \x01(\x0b\x32\x37.qwak.feature.store.features.PopulationTimeframeNewOnlyH\x00\x42\x06\n\x04type\"\t\n\x07Vanilla\"\x9f\x01\n\x08\x46ullRead\x12\x37\n\x07\x64\x65\x66\x61ult\x18\x01 \x01(\x0b\x32$.qwak.feature.store.features.VanillaH\x00\x12P\n\x14population_timeframe\x18\x02 \x01(\x0b\x32\x30.qwak.feature.store.features.PopulationTimeframeH\x00\x42\x08\n\x06\x66lavor\"\xd2\x01\n\x14\x44\x61taSourceReadPolicy\x12\x38\n\x08new_only\x18\x01 \x01(\x0b\x32$.qwak.feature.store.features.NewOnlyH\x00\x12<\n\ntime_frame\x18\x02 \x01(\x0b\x32&.qwak.feature.store.features.TimeFrameH\x00\x12:\n\tfull_read\x18\x03 \x01(\x0b\x32%.qwak.feature.store.features.FullReadH\x00\x42\x06\n\x04typeB[\n&com.qwak.ai.feature.store.features.apiP\x01Z/qwak/featurestore/features;featurestorefeaturesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3qwak/feature_store/features/feature_set_types.proto\x12\x1bqwak.feature.store.features\x1a\x1fgoogle/protobuf/timestamp.proto\x1a&qwak/feature_store/sources/batch.proto\x1a*qwak/feature_store/sources/streaming.proto\x1a+qwak/feature_store/features/execution.proto\x1a-qwak/feature_store/features/aggregation.proto\x1a,qwak/feature_store/features/monitoring.proto\x1a<qwak/feature_store/features/real_time_feature_set_type.proto\"\xf1\x04\n\x0e\x46\x65\x61tureSetType\x12I\n\x11\x62\x61tch_feature_set\x18\x05 \x01(\x0b\x32,.qwak.feature.store.features.BatchFeatureSetH\x00\x12Q\n\x16on_the_fly_feature_set\x18\x06 \x01(\x0b\x32/.qwak.feature.store.features.OnTheFlyFeatureSetH\x00\x12Q\n\x15streaming_feature_set\x18\x07 \x01(\x0b\x32\x30.qwak.feature.store.features.StreamingFeatureSetH\x00\x12V\n\x18streaming_feature_set_v1\x18\x08 \x01(\x0b\x32\x32.qwak.feature.store.features.StreamingFeatureSetV1H\x00\x12N\n\x14\x62\x61tch_feature_set_v1\x18\t \x01(\x0b\x32..qwak.feature.store.features.BatchFeatureSetV1H\x00\x12h\n!streaming_aggregation_feature_set\x18\n \x01(\x0b\x32;.qwak.feature.store.features.StreamingAggregationFeatureSetH\x00\x12P\n\x15real_time_feature_set\x18\x0b \x01(\x0b\x32/.qwak.feature.store.features.RealTimeFeatureSetH\x00\x42\n\n\x08set_type\"\x9d\x03\n\x0f\x42\x61tchFeatureSet\x12\x19\n\x11scheduling_policy\x18\x01 \x01(\t\x12\x41\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\'.qwak.feature.store.sources.BatchSourceB\x02\x18\x01\x12\x37\n\x08\x62\x61\x63kfill\x18\x03 \x01(\x0b\x32%.qwak.feature.store.features.Backfill\x12\x37\n\x08\x66unction\x18\x04 \x01(\x0b\x32%.qwak.feature.store.features.Function\x12U\n\x19\x66\x65\x61ture_set_batch_sources\x18\x05 \x03(\x0b\x32\x32.qwak.feature.store.features.FeatureSetBatchSource\x12\x63\n\x19monitoring_configurations\x18\x06 \x01(\x0b\x32@.qwak.feature.store.features.monitoring.MonitoringConfigurations\"\xe5\x04\n\x11\x42\x61tchFeatureSetV1\x12\x19\n\x11scheduling_policy\x18\x01 \x01(\t\x12\x37\n\x08\x62\x61\x63kfill\x18\x02 \x01(\x0b\x32%.qwak.feature.store.features.Backfill\x12;\n\x08\x66unction\x18\x03 \x01(\x0b\x32%.qwak.feature.store.features.FunctionB\x02\x18\x01\x12U\n\x19\x66\x65\x61ture_set_batch_sources\x18\x04 \x03(\x0b\x32\x32.qwak.feature.store.features.FeatureSetBatchSource\x12L\n\x0e\x65xecution_spec\x18\x05 \x01(\x0b\x32\x34.qwak.feature.store.features.execution.ExecutionSpec\x12\x14\n\x0coffline_sink\x18\x06 \x01(\x08\x12\x13\n\x0bonline_sink\x18\x07 \x01(\x08\x12\x63\n\x19monitoring_configurations\x18\x08 \x01(\x0b\x32@.qwak.feature.store.features.monitoring.MonitoringConfigurations\x12\x1d\n\x15timestamp_column_name\x18\t \x01(\t\x12\x43\n\x0etransformation\x18\n \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12&\n\x1eqwak_internal_protocol_version\x18\x0b \x01(\x05\"\x9d\x01\n\x15\x46\x65\x61tureSetBatchSource\x12<\n\x0b\x64\x61ta_source\x18\x01 \x01(\x0b\x32\'.qwak.feature.store.sources.BatchSource\x12\x46\n\x0bread_policy\x18\x02 \x01(\x0b\x32\x31.qwak.feature.store.features.DataSourceReadPolicy\"X\n\x13StreamingFeatureSet\x12\x41\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32+.qwak.feature.store.sources.StreamingSource\"\x81\x03\n\x15StreamingFeatureSetV1\x12\x41\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32+.qwak.feature.store.sources.StreamingSource\x12\x43\n\x0etransformation\x18\x02 \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12U\n\x0e\x65xecution_spec\x18\x03 \x01(\x0b\x32=.qwak.feature.store.features.execution.StreamingExecutionSpec\x12\x1d\n\x15timestamp_column_name\x18\x04 \x01(\t\x12\x1f\n\x17online_trigger_interval\x18\x05 \x01(\x05\x12!\n\x19offline_scheduling_policy\x18\x06 \x01(\t\x12&\n\x1eqwak_internal_protocol_version\x18\x07 \x01(\x05\"\x97\x04\n\x1eStreamingAggregationFeatureSet\x12\x41\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32+.qwak.feature.store.sources.StreamingSource\x12\x43\n\x0etransformation\x18\x02 \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12U\n\x0e\x65xecution_spec\x18\x03 \x01(\x0b\x32=.qwak.feature.store.features.execution.StreamingExecutionSpec\x12\x1d\n\x15timestamp_column_name\x18\x04 \x01(\t\x12\x1f\n\x17online_trigger_interval\x18\x05 \x01(\x05\x12$\n\x1c\x63ompaction_scheduling_policy\x18\x06 \x01(\t\x12\x46\n\x10\x61ggregation_spec\x18\x07 \x01(\x0b\x32,.qwak.feature.store.features.AggregationSpec\x12@\n\rbackfill_spec\x18\x08 \x01(\x0b\x32).qwak.feature.store.features.BackfillSpec\x12&\n\x1eqwak_internal_protocol_version\x18\t \x01(\x05\"\xc3\x01\n\x1b\x42\x61\x63kfillBatchDataSourceSpec\x12<\n\x0b\x64\x61ta_source\x18\x01 \x01(\x0b\x32\'.qwak.feature.store.sources.BatchSource\x12\x33\n\x0fstart_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"|\n\x16\x42\x61\x63kfillDataSourceSpec\x12Z\n\x16\x62\x61tch_data_source_spec\x18\x01 \x01(\x0b\x32\x38.qwak.feature.store.features.BackfillBatchDataSourceSpecH\x00\x42\x06\n\x04type\"\xe1\x02\n\x0c\x42\x61\x63kfillSpec\x12T\n\x0e\x65xecution_spec\x18\x01 \x01(\x0b\x32<.qwak.feature.store.features.execution.BackfillExecutionSpec\x12\x33\n\x0fstart_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\x0etransformation\x18\x04 \x01(\x0b\x32+.qwak.feature.store.features.Transformation\x12N\n\x11\x64\x61ta_source_specs\x18\x05 \x03(\x0b\x32\x33.qwak.feature.store.features.BackfillDataSourceSpec\"\x9f\x01\n\x0f\x41ggregationSpec\x12O\n\x0c\x61ggregations\x18\x01 \x03(\x0b\x32\x39.qwak.feature.store.features.aggregation.AggregationField\x12\x15\n\rslide_seconds\x18\x02 \x01(\x05\x12$\n\x1c\x61llowed_late_arrival_seconds\x18\x03 \x01(\x05\"\x9f\x02\n\x0eTransformation\x12L\n\x12udf_transformation\x18\x01 \x01(\x0b\x32..qwak.feature.store.features.UdfTransformationH\x00\x12L\n\x12sql_transformation\x18\x02 \x01(\x0b\x32..qwak.feature.store.features.SqlTransformationH\x00\x12R\n\x15koalas_transformation\x18\x03 \x01(\x0b\x32\x31.qwak.feature.store.features.KoalasTransformationH\x00\x12\x15\n\rartifact_path\x18\x04 \x01(\tB\x06\n\x04type\"*\n\x11UdfTransformation\x12\x15\n\rfunction_name\x18\x01 \x01(\t\"8\n\x11SqlTransformation\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x16\n\x0e\x66unction_names\x18\x02 \x03(\t\"-\n\x14KoalasTransformation\x12\x15\n\rfunction_name\x18\x01 \x01(\t\"f\n\x12OnTheFlyFeatureSet\x12:\n\x08\x66unction\x18\x01 \x01(\x0b\x32(.qwak.feature.store.features.UdfFunction\x12\x14\n\x0crequirements\x18\x02 \x01(\x0c\"\x96\x01\n\x08\x46unction\x12@\n\x0csql_function\x18\x01 \x01(\x0b\x32(.qwak.feature.store.features.SqlFunctionH\x00\x12@\n\x0cudf_function\x18\x02 \x01(\x0b\x32(.qwak.feature.store.features.UdfFunctionH\x00\x42\x06\n\x04type\"\xb5\x01\n\x08\x42\x61\x63kfill\x12.\n\nstart_date\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\rfillup_method\x18\x02 \x01(\x0e\x32\x32.qwak.feature.store.features.Backfill.FillUpMethod\".\n\x0c\x46illUpMethod\x12\x10\n\x0c\x41S_SCHEDULED\x10\x00\x12\x0c\n\x08SNAPSHOT\x10\x01\"\x1a\n\x0bSqlFunction\x12\x0b\n\x03sql\x18\x01 \x01(\t\"\x1b\n\x0bUdfFunction\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x0c\"\t\n\x07NewOnly\"\xa0\x01\n\tTimeFrame\x12\x0f\n\x07minutes\x18\x01 \x01(\x05\x12\x37\n\x07vanilla\x18\x02 \x01(\x0b\x32$.qwak.feature.store.features.VanillaH\x00\x12?\n\x0b\x61ggregation\x18\x03 \x01(\x0b\x32(.qwak.feature.store.features.AggregationH\x00\x42\x08\n\x06\x66lavor\"k\n\x0b\x41ggregation\x12T\n\x16\x61ggregation_population\x18\x01 \x01(\x0b\x32\x32.qwak.feature.store.features.AggregationPopulationH\x00\x42\x06\n\x04type\"\x17\n\x15\x41ggregationPopulation\"\x1c\n\x1aPopulationTimeframeNewOnly\"j\n\x13PopulationTimeframe\x12K\n\x08new_only\x18\x01 \x01(\x0b\x32\x37.qwak.feature.store.features.PopulationTimeframeNewOnlyH\x00\x42\x06\n\x04type\"\t\n\x07Vanilla\"\x9f\x01\n\x08\x46ullRead\x12\x37\n\x07\x64\x65\x66\x61ult\x18\x01 \x01(\x0b\x32$.qwak.feature.store.features.VanillaH\x00\x12P\n\x14population_timeframe\x18\x02 \x01(\x0b\x32\x30.qwak.feature.store.features.PopulationTimeframeH\x00\x42\x08\n\x06\x66lavor\"\xd2\x01\n\x14\x44\x61taSourceReadPolicy\x12\x38\n\x08new_only\x18\x01 \x01(\x0b\x32$.qwak.feature.store.features.NewOnlyH\x00\x12<\n\ntime_frame\x18\x02 \x01(\x0b\x32&.qwak.feature.store.features.TimeFrameH\x00\x12:\n\tfull_read\x18\x03 \x01(\x0b\x32%.qwak.feature.store.features.FullReadH\x00\x42\x06\n\x04typeB[\n&com.qwak.ai.feature.store.features.apiP\x01Z/qwak/featurestore/features;featurestorefeaturesb\x06proto3')
 
 
 
 _FEATURESETTYPE = DESCRIPTOR.message_types_by_name['FeatureSetType']
 _BATCHFEATURESET = DESCRIPTOR.message_types_by_name['BatchFeatureSet']
 _BATCHFEATURESETV1 = DESCRIPTOR.message_types_by_name['BatchFeatureSetV1']
 _FEATURESETBATCHSOURCE = DESCRIPTOR.message_types_by_name['FeatureSetBatchSource']
@@ -261,68 +262,68 @@
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n&com.qwak.ai.feature.store.features.apiP\001Z/qwak/featurestore/features;featurestorefeatures'
   _BATCHFEATURESET.fields_by_name['data_sources']._options = None
   _BATCHFEATURESET.fields_by_name['data_sources']._serialized_options = b'\030\001'
   _BATCHFEATURESETV1.fields_by_name['function']._options = None
   _BATCHFEATURESETV1.fields_by_name['function']._serialized_options = b'\030\001'
-  _FEATURESETTYPE._serialized_start=340
-  _FEATURESETTYPE._serialized_end=883
-  _BATCHFEATURESET._serialized_start=886
-  _BATCHFEATURESET._serialized_end=1299
-  _BATCHFEATURESETV1._serialized_start=1302
-  _BATCHFEATURESETV1._serialized_end=1915
-  _FEATURESETBATCHSOURCE._serialized_start=1918
-  _FEATURESETBATCHSOURCE._serialized_end=2075
-  _STREAMINGFEATURESET._serialized_start=2077
-  _STREAMINGFEATURESET._serialized_end=2165
-  _STREAMINGFEATURESETV1._serialized_start=2168
-  _STREAMINGFEATURESETV1._serialized_end=2553
-  _STREAMINGAGGREGATIONFEATURESET._serialized_start=2556
-  _STREAMINGAGGREGATIONFEATURESET._serialized_end=3091
-  _BACKFILLBATCHDATASOURCESPEC._serialized_start=3094
-  _BACKFILLBATCHDATASOURCESPEC._serialized_end=3289
-  _BACKFILLDATASOURCESPEC._serialized_start=3291
-  _BACKFILLDATASOURCESPEC._serialized_end=3415
-  _BACKFILLSPEC._serialized_start=3418
-  _BACKFILLSPEC._serialized_end=3771
-  _AGGREGATIONSPEC._serialized_start=3774
-  _AGGREGATIONSPEC._serialized_end=3933
-  _TRANSFORMATION._serialized_start=3936
-  _TRANSFORMATION._serialized_end=4223
-  _UDFTRANSFORMATION._serialized_start=4225
-  _UDFTRANSFORMATION._serialized_end=4267
-  _SQLTRANSFORMATION._serialized_start=4269
-  _SQLTRANSFORMATION._serialized_end=4325
-  _KOALASTRANSFORMATION._serialized_start=4327
-  _KOALASTRANSFORMATION._serialized_end=4372
-  _ONTHEFLYFEATURESET._serialized_start=4374
-  _ONTHEFLYFEATURESET._serialized_end=4476
-  _FUNCTION._serialized_start=4479
-  _FUNCTION._serialized_end=4629
-  _BACKFILL._serialized_start=4632
-  _BACKFILL._serialized_end=4813
-  _BACKFILL_FILLUPMETHOD._serialized_start=4767
-  _BACKFILL_FILLUPMETHOD._serialized_end=4813
-  _SQLFUNCTION._serialized_start=4815
-  _SQLFUNCTION._serialized_end=4841
-  _UDFFUNCTION._serialized_start=4843
-  _UDFFUNCTION._serialized_end=4870
-  _NEWONLY._serialized_start=4872
-  _NEWONLY._serialized_end=4881
-  _TIMEFRAME._serialized_start=4884
-  _TIMEFRAME._serialized_end=5044
-  _AGGREGATION._serialized_start=5046
-  _AGGREGATION._serialized_end=5153
-  _AGGREGATIONPOPULATION._serialized_start=5155
-  _AGGREGATIONPOPULATION._serialized_end=5178
-  _POPULATIONTIMEFRAMENEWONLY._serialized_start=5180
-  _POPULATIONTIMEFRAMENEWONLY._serialized_end=5208
-  _POPULATIONTIMEFRAME._serialized_start=5210
-  _POPULATIONTIMEFRAME._serialized_end=5316
-  _VANILLA._serialized_start=5318
-  _VANILLA._serialized_end=5327
-  _FULLREAD._serialized_start=5330
-  _FULLREAD._serialized_end=5489
-  _DATASOURCEREADPOLICY._serialized_start=5492
-  _DATASOURCEREADPOLICY._serialized_end=5702
+  _FEATURESETTYPE._serialized_start=402
+  _FEATURESETTYPE._serialized_end=1027
+  _BATCHFEATURESET._serialized_start=1030
+  _BATCHFEATURESET._serialized_end=1443
+  _BATCHFEATURESETV1._serialized_start=1446
+  _BATCHFEATURESETV1._serialized_end=2059
+  _FEATURESETBATCHSOURCE._serialized_start=2062
+  _FEATURESETBATCHSOURCE._serialized_end=2219
+  _STREAMINGFEATURESET._serialized_start=2221
+  _STREAMINGFEATURESET._serialized_end=2309
+  _STREAMINGFEATURESETV1._serialized_start=2312
+  _STREAMINGFEATURESETV1._serialized_end=2697
+  _STREAMINGAGGREGATIONFEATURESET._serialized_start=2700
+  _STREAMINGAGGREGATIONFEATURESET._serialized_end=3235
+  _BACKFILLBATCHDATASOURCESPEC._serialized_start=3238
+  _BACKFILLBATCHDATASOURCESPEC._serialized_end=3433
+  _BACKFILLDATASOURCESPEC._serialized_start=3435
+  _BACKFILLDATASOURCESPEC._serialized_end=3559
+  _BACKFILLSPEC._serialized_start=3562
+  _BACKFILLSPEC._serialized_end=3915
+  _AGGREGATIONSPEC._serialized_start=3918
+  _AGGREGATIONSPEC._serialized_end=4077
+  _TRANSFORMATION._serialized_start=4080
+  _TRANSFORMATION._serialized_end=4367
+  _UDFTRANSFORMATION._serialized_start=4369
+  _UDFTRANSFORMATION._serialized_end=4411
+  _SQLTRANSFORMATION._serialized_start=4413
+  _SQLTRANSFORMATION._serialized_end=4469
+  _KOALASTRANSFORMATION._serialized_start=4471
+  _KOALASTRANSFORMATION._serialized_end=4516
+  _ONTHEFLYFEATURESET._serialized_start=4518
+  _ONTHEFLYFEATURESET._serialized_end=4620
+  _FUNCTION._serialized_start=4623
+  _FUNCTION._serialized_end=4773
+  _BACKFILL._serialized_start=4776
+  _BACKFILL._serialized_end=4957
+  _BACKFILL_FILLUPMETHOD._serialized_start=4911
+  _BACKFILL_FILLUPMETHOD._serialized_end=4957
+  _SQLFUNCTION._serialized_start=4959
+  _SQLFUNCTION._serialized_end=4985
+  _UDFFUNCTION._serialized_start=4987
+  _UDFFUNCTION._serialized_end=5014
+  _NEWONLY._serialized_start=5016
+  _NEWONLY._serialized_end=5025
+  _TIMEFRAME._serialized_start=5028
+  _TIMEFRAME._serialized_end=5188
+  _AGGREGATION._serialized_start=5190
+  _AGGREGATION._serialized_end=5297
+  _AGGREGATIONPOPULATION._serialized_start=5299
+  _AGGREGATIONPOPULATION._serialized_end=5322
+  _POPULATIONTIMEFRAMENEWONLY._serialized_start=5324
+  _POPULATIONTIMEFRAMENEWONLY._serialized_end=5352
+  _POPULATIONTIMEFRAME._serialized_start=5354
+  _POPULATIONTIMEFRAME._serialized_end=5460
+  _VANILLA._serialized_start=5462
+  _VANILLA._serialized_end=5471
+  _FULLREAD._serialized_start=5474
+  _FULLREAD._serialized_end=5633
+  _DATASOURCEREADPOLICY._serialized_start=5636
+  _DATASOURCEREADPOLICY._serialized_end=5846
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
 import qwak.feature_store.features.aggregation_pb2
 import qwak.feature_store.features.execution_pb2
 import qwak.feature_store.features.monitoring_pb2
+import qwak.feature_store.features.real_time_feature_set_type_pb2
 import qwak.feature_store.sources.batch_pb2
 import qwak.feature_store.sources.streaming_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
@@ -29,39 +30,43 @@
 
     BATCH_FEATURE_SET_FIELD_NUMBER: builtins.int
     ON_THE_FLY_FEATURE_SET_FIELD_NUMBER: builtins.int
     STREAMING_FEATURE_SET_FIELD_NUMBER: builtins.int
     STREAMING_FEATURE_SET_V1_FIELD_NUMBER: builtins.int
     BATCH_FEATURE_SET_V1_FIELD_NUMBER: builtins.int
     STREAMING_AGGREGATION_FEATURE_SET_FIELD_NUMBER: builtins.int
+    REAL_TIME_FEATURE_SET_FIELD_NUMBER: builtins.int
     @property
     def batch_feature_set(self) -> global___BatchFeatureSet: ...
     @property
     def on_the_fly_feature_set(self) -> global___OnTheFlyFeatureSet: ...
     @property
     def streaming_feature_set(self) -> global___StreamingFeatureSet: ...
     @property
     def streaming_feature_set_v1(self) -> global___StreamingFeatureSetV1: ...
     @property
     def batch_feature_set_v1(self) -> global___BatchFeatureSetV1: ...
     @property
     def streaming_aggregation_feature_set(self) -> global___StreamingAggregationFeatureSet: ...
+    @property
+    def real_time_feature_set(self) -> qwak.feature_store.features.real_time_feature_set_type_pb2.RealTimeFeatureSet: ...
     def __init__(
         self,
         *,
         batch_feature_set: global___BatchFeatureSet | None = ...,
         on_the_fly_feature_set: global___OnTheFlyFeatureSet | None = ...,
         streaming_feature_set: global___StreamingFeatureSet | None = ...,
         streaming_feature_set_v1: global___StreamingFeatureSetV1 | None = ...,
         batch_feature_set_v1: global___BatchFeatureSetV1 | None = ...,
         streaming_aggregation_feature_set: global___StreamingAggregationFeatureSet | None = ...,
+        real_time_feature_set: qwak.feature_store.features.real_time_feature_set_type_pb2.RealTimeFeatureSet | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["batch_feature_set", b"batch_feature_set", "batch_feature_set_v1", b"batch_feature_set_v1", "on_the_fly_feature_set", b"on_the_fly_feature_set", "set_type", b"set_type", "streaming_aggregation_feature_set", b"streaming_aggregation_feature_set", "streaming_feature_set", b"streaming_feature_set", "streaming_feature_set_v1", b"streaming_feature_set_v1"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["batch_feature_set", b"batch_feature_set", "batch_feature_set_v1", b"batch_feature_set_v1", "on_the_fly_feature_set", b"on_the_fly_feature_set", "set_type", b"set_type", "streaming_aggregation_feature_set", b"streaming_aggregation_feature_set", "streaming_feature_set", b"streaming_feature_set", "streaming_feature_set_v1", b"streaming_feature_set_v1"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["set_type", b"set_type"]) -> typing_extensions.Literal["batch_feature_set", "on_the_fly_feature_set", "streaming_feature_set", "streaming_feature_set_v1", "batch_feature_set_v1", "streaming_aggregation_feature_set"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["batch_feature_set", b"batch_feature_set", "batch_feature_set_v1", b"batch_feature_set_v1", "on_the_fly_feature_set", b"on_the_fly_feature_set", "real_time_feature_set", b"real_time_feature_set", "set_type", b"set_type", "streaming_aggregation_feature_set", b"streaming_aggregation_feature_set", "streaming_feature_set", b"streaming_feature_set", "streaming_feature_set_v1", b"streaming_feature_set_v1"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["batch_feature_set", b"batch_feature_set", "batch_feature_set_v1", b"batch_feature_set_v1", "on_the_fly_feature_set", b"on_the_fly_feature_set", "real_time_feature_set", b"real_time_feature_set", "set_type", b"set_type", "streaming_aggregation_feature_set", b"streaming_aggregation_feature_set", "streaming_feature_set", b"streaming_feature_set", "streaming_feature_set_v1", b"streaming_feature_set_v1"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["set_type", b"set_type"]) -> typing_extensions.Literal["batch_feature_set", "on_the_fly_feature_set", "streaming_feature_set", "streaming_feature_set_v1", "batch_feature_set_v1", "streaming_aggregation_feature_set", "real_time_feature_set"] | None: ...
 
 global___FeatureSetType = FeatureSetType
 
 class BatchFeatureSet(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SCHEDULING_POLICY_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.51/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.51/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.51/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/pyproject.toml` & `qwak_core-0.0.51/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.50"
+version = "0.0.51"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.50/qwak/automations/__init__.py` & `qwak_core-0.0.51/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/automations/automation_executions.py` & `qwak_core-0.0.51/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/automations/automations.py` & `qwak_core-0.0.51/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.51/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.51/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.51/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.51/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.51/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/alert_management/client.py` & `qwak_core-0.0.51/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/analytics/client.py` & `qwak_core-0.0.51/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/audience/client.py` & `qwak_core-0.0.51/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/automation_management/client.py` & `qwak_core-0.0.51/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.51/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.51/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.51/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.51/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/build_management/client.py` & `qwak_core-0.0.51/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.51/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.51/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/deployment/client.py` & `qwak_core-0.0.51/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.51/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.51/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.51/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.51/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.51/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/logging_client/client.py` & `qwak_core-0.0.51/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/model_management/client.py` & `qwak_core-0.0.51/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/project/client.py` & `qwak_core-0.0.51/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/secret_service/client.py` & `qwak_core-0.0.51/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.51/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.51/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.51/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.51/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.51/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.51/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.51/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.51/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.51/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.51/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.51/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.51/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.51/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.51/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.51/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/offline/client.py` & `qwak_core-0.0.51/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/feature_store/online/client.py` & `qwak_core-0.0.51/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/inner/const.py` & `qwak_core-0.0.51/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.51/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.51/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.51/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.51/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/inner/singleton_meta.py` & `qwak_core-0.0.51/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/inner/tool/auth.py` & `qwak_core-0.0.51/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.51/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.51/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.51/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.51/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/adapters/__init__.py` & `qwak_core-0.0.51/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.51/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.51/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.51/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.51/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.51/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/base.py` & `qwak_core-0.0.51/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/decorators/api.py` & `qwak_core-0.0.51/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.51/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/experiment_tracking.py` & `qwak_core-0.0.51/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/schema.py` & `qwak_core-0.0.51/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/schema_entities.py` & `qwak_core-0.0.51/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.51/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.51/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.51/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.51/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.51/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.51/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.51/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.51/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.51/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.51/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.51/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.51/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.51/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.51/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.51/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.51/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.51/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.51/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.51/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/qwak_client/client.py` & `qwak_core-0.0.51/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.51/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/qwak_client/models/model.py` & `qwak_core-0.0.51/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.51/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.51/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/tools/logger/logger.py` & `qwak_core-0.0.51/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak/tools/logger/logging.yml` & `qwak_core-0.0.51/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.51/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/qwak_services_mock/services_mock.py` & `qwak_core-0.0.51/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.50/setup.py` & `qwak_core-0.0.51/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.50',
+    'version': '0.0.51',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.50/PKG-INFO` & `qwak_core-0.0.51/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.50
+Version: 0.0.51
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

