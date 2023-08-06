# Comparing `tmp/qwak_core-0.0.98.tar.gz` & `tmp/qwak_core-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.98.tar", max compression
+gzip compressed data, was "qwak_core-0.0.99.tar", max compression
```

## Comparing `qwak_core-0.0.98.tar` & `qwak_core-0.0.99.tar`

### file list

```diff
@@ -1,588 +1,588 @@
--rw-r--r--   0        0        0      264 2023-06-05 11:45:12.282585 qwak_core-0.0.98/README.md
--rw-r--r--   0        0        0        0 2023-06-05 11:46:49.483904 qwak_core-0.0.98/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-06-05 11:46:49.507904 qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-06-05 11:46:30.203628 qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.507904 qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-06-05 11:46:49.503904 qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-06-05 11:46:29.871624 qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.503904 qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-06-05 11:46:49.503904 qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-06-05 11:46:30.035626 qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.503904 qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-06-05 11:46:49.495904 qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-06-05 11:46:29.371616 qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-06-05 11:46:49.495904 qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-06-05 11:46:49.499904 qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-06-05 11:46:29.535619 qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.499904 qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4901 2023-06-05 11:46:49.499904 qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5995 2023-06-05 11:46:29.703621 qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.499904 qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-06-05 11:46:49.483904 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-06-05 11:46:29.203614 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-06-05 11:46:49.487904 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5707 2023-06-05 11:46:49.487904 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8170 2023-06-05 11:46:30.371631 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.487904 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-06-05 11:46:49.491904 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-06-05 11:46:30.707636 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.491904 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-06-05 11:46:49.491904 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-06-05 11:46:30.875638 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-06-05 11:46:49.495904 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-06-05 11:46:49.487904 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-06-05 11:46:30.539633 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.491904 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-06-05 11:46:49.495904 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-06-05 11:46:31.051641 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.495904 qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-06-05 11:46:49.531904 qwak_core-0.0.98/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-06-05 11:46:33.431675 qwak_core-0.0.98/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.531904 qwak_core-0.0.98/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-06-05 11:46:49.535905 qwak_core-0.0.98/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-06-05 11:46:33.611677 qwak_core-0.0.98/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-06-05 11:46:49.535905 qwak_core-0.0.98/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-06-05 11:46:49.599905 qwak_core-0.0.98/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-06-05 11:46:38.831748 qwak_core-0.0.98/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.599905 qwak_core-0.0.98/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-06-05 11:46:49.599905 qwak_core-0.0.98/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-06-05 11:46:38.995750 qwak_core-0.0.98/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-06-05 11:46:49.599905 qwak_core-0.0.98/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-06-05 11:46:49.603905 qwak_core-0.0.98/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-06-05 11:46:39.847761 qwak_core-0.0.98/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-06-05 11:46:49.603905 qwak_core-0.0.98/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-06-05 11:46:49.603905 qwak_core-0.0.98/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-06-05 11:46:39.675759 qwak_core-0.0.98/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.603905 qwak_core-0.0.98/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-06-05 11:46:49.607905 qwak_core-0.0.98/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-06-05 11:46:40.011763 qwak_core-0.0.98/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.607905 qwak_core-0.0.98/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-06-05 11:46:49.607905 qwak_core-0.0.98/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-06-05 11:46:40.183766 qwak_core-0.0.98/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-06-05 11:46:49.607905 qwak_core-0.0.98/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-06-05 11:46:49.691907 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-06-05 11:46:47.383875 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.691907 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-06-05 11:46:49.687907 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-06-05 11:46:47.039871 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.687907 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-06-05 11:46:49.687907 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-06-05 11:46:47.207873 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.687907 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-06-05 11:46:49.683906 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-06-05 11:46:46.699866 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-06-05 11:46:49.683906 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-06-05 11:46:49.683906 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-06-05 11:46:46.875868 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.687907 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-06-05 11:46:49.695906 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-06-05 11:46:47.883882 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.695906 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-06-05 11:46:49.695906 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-06-05 11:46:47.715880 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.695906 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-06-05 11:46:49.691907 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-06-05 11:46:47.551877 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.695906 qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10989 2023-06-05 11:46:49.679906 qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    15193 2023-06-05 11:46:46.523863 qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.683906 qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-06-05 11:46:49.675906 qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-06-05 11:46:46.171859 qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.675906 qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    44118 2023-06-05 11:46:49.679906 qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    58049 2023-06-05 11:46:46.355861 qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-06-05 11:46:49.679906 qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    20255 2023-06-05 11:46:49.631906 qwak_core-0.0.98/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    17495 2023-06-05 11:46:41.899793 qwak_core-0.0.98/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    20359 2023-06-05 11:46:49.631906 qwak_core-0.0.98/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-06-05 11:46:49.631906 qwak_core-0.0.98/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-06-05 11:46:41.731790 qwak_core-0.0.98/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.631906 qwak_core-0.0.98/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    13611 2023-06-05 11:46:49.623906 qwak_core-0.0.98/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    21063 2023-06-05 11:46:41.391785 qwak_core-0.0.98/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.623906 qwak_core-0.0.98/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-06-05 11:46:49.623906 qwak_core-0.0.98/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-06-05 11:46:41.559787 qwak_core-0.0.98/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.623906 qwak_core-0.0.98/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-06-05 11:46:49.627906 qwak_core-0.0.98/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-06-05 11:46:42.071796 qwak_core-0.0.98/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-06-05 11:46:49.627906 qwak_core-0.0.98/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38290 2023-06-05 11:46:49.627906 qwak_core-0.0.98/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52702 2023-06-05 11:46:42.439802 qwak_core-0.0.98/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-06-05 11:46:49.627906 qwak_core-0.0.98/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-06-05 11:46:49.639906 qwak_core-0.0.98/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-06-05 11:46:42.791808 qwak_core-0.0.98/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.639906 qwak_core-0.0.98/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-06-05 11:46:49.639906 qwak_core-0.0.98/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-06-05 11:46:42.963811 qwak_core-0.0.98/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-06-05 11:46:49.639906 qwak_core-0.0.98/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-06-05 11:46:49.615906 qwak_core-0.0.98/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-06-05 11:46:40.883776 qwak_core-0.0.98/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.615906 qwak_core-0.0.98/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-06-05 11:46:49.619906 qwak_core-0.0.98/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-06-05 11:46:41.051779 qwak_core-0.0.98/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-06-05 11:46:49.619906 qwak_core-0.0.98/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-06-05 11:46:49.611905 qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-06-05 11:46:40.531771 qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.611905 qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-06-05 11:46:49.611905 qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-06-05 11:46:40.359768 qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.611905 qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-06-05 11:46:49.615906 qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-06-05 11:46:40.715773 qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-06-05 11:46:49.615906 qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-06-05 11:46:49.523904 qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-06-05 11:46:32.579663 qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.523904 qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-06-05 11:46:49.523904 qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-06-05 11:46:32.747665 qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.527904 qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-06-05 11:46:49.527904 qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-06-05 11:46:32.915668 qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-06-05 11:46:49.527904 qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-06-05 11:46:49.579905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-06-05 11:46:37.823734 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.583905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-06-05 11:46:49.579905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-06-05 11:46:37.655732 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-06-05 11:46:49.579905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2023-06-05 11:46:49.559905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2023-06-05 11:46:35.807707 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.559905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2023-06-05 11:46:49.555905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2023-06-05 11:46:35.635705 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.555905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-06-05 11:46:49.551905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-06-05 11:46:35.095697 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.551905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-06-05 11:46:49.555905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-06-05 11:46:35.455702 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-06-05 11:46:49.555905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-06-05 11:46:49.559905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-06-05 11:46:35.975709 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.559905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-06-05 11:46:49.563905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-06-05 11:46:36.143711 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-06-05 11:46:49.563905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25269 2023-06-05 11:46:49.551905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37664 2023-06-05 11:46:35.275700 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.551905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-06-05 11:46:49.563905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-06-05 11:46:36.307714 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.563905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    10202 2023-06-05 11:46:49.567905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py
--rw-r--r--   0        0        0    16565 2023-06-05 11:46:36.647718 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.567905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2_grpc.py
--rw-r--r--   0        0        0     3559 2023-06-05 11:46:49.567905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py
--rw-r--r--   0        0        0     1759 2023-06-05 11:46:36.815720 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi
--rw-r--r--   0        0        0     3608 2023-06-05 11:46:49.571905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0    10604 2023-06-05 11:46:49.567905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    13410 2023-06-05 11:46:36.479716 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.567905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-06-05 11:46:49.583905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-06-05 11:46:49.067898 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.583905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-06-05 11:46:49.583905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-06-05 11:46:49.239900 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-06-05 11:46:49.587905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-06-05 11:46:49.587905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-06-05 11:46:38.327741 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.587905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-06-05 11:46:49.587905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-06-05 11:46:38.495743 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-06-05 11:46:49.591905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-06-05 11:46:49.591905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-06-05 11:46:38.659745 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.591905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-06-05 11:46:49.595905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-06-05 11:46:39.339754 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.595905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-06-05 11:46:49.591905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-06-05 11:46:39.167752 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-06-05 11:46:49.595905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-06-05 11:46:49.595905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-06-05 11:46:39.507757 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.595905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-06-05 11:46:49.571905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-06-05 11:46:36.983723 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.571905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-06-05 11:46:49.571905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-06-05 11:46:37.151725 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.575905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-06-05 11:46:49.575905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-06-05 11:46:37.323727 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-06-05 11:46:49.575905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-06-05 11:46:49.575905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-06-05 11:46:37.491730 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.579905 qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-06-05 11:46:49.699907 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-06-05 11:46:48.051884 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.699907 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-06-05 11:46:49.699907 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-06-05 11:46:48.215886 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-06-05 11:46:49.699907 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-06-05 11:46:49.703907 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-06-05 11:46:48.383889 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.703907 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-06-05 11:46:49.703907 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-06-05 11:46:48.555891 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-06-05 11:46:49.703907 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-06-05 11:46:49.707907 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-06-05 11:46:48.735894 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-06-05 11:46:49.707907 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-06-05 11:46:49.707907 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-06-05 11:46:48.899896 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.707907 qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-06-05 11:46:49.639906 qwak_core-0.0.98/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-06-05 11:46:43.127814 qwak_core-0.0.98/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.643906 qwak_core-0.0.98/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-06-05 11:46:49.643906 qwak_core-0.0.98/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-06-05 11:46:43.295816 qwak_core-0.0.98/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-06-05 11:46:49.643906 qwak_core-0.0.98/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-06-05 11:46:49.535905 qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-06-05 11:46:34.395688 qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.539904 qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-06-05 11:46:49.539904 qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-06-05 11:46:34.567690 qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.543905 qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-06-05 11:46:49.543905 qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-06-05 11:46:34.731692 qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-06-05 11:46:49.543905 qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-06-05 11:46:49.547905 qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-06-05 11:46:34.899695 qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.547905 qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-06-05 11:46:49.619906 qwak_core-0.0.98/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-06-05 11:46:41.219782 qwak_core-0.0.98/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-06-05 11:46:49.619906 qwak_core-0.0.98/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-06-05 11:46:49.643906 qwak_core-0.0.98/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-06-05 11:46:43.459819 qwak_core-0.0.98/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.647906 qwak_core-0.0.98/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-06-05 11:46:49.647906 qwak_core-0.0.98/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-06-05 11:46:43.627822 qwak_core-0.0.98/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-06-05 11:46:49.647906 qwak_core-0.0.98/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-06-05 11:46:49.659906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-06-05 11:46:44.631838 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.659906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-06-05 11:46:49.659906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-06-05 11:46:44.795840 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.663906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-06-05 11:46:49.663906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-06-05 11:46:44.967842 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.663906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-06-05 11:46:49.663906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-06-05 11:46:45.135845 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.663906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-06-05 11:46:49.667906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-06-05 11:46:45.315847 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.667906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-06-05 11:46:49.667906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-06-05 11:46:45.503850 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-06-05 11:46:49.671906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-06-05 11:46:49.671906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-06-05 11:46:45.667852 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.671906 qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-06-05 11:46:49.651906 qwak_core-0.0.98/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-06-05 11:46:43.963827 qwak_core-0.0.98/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.651906 qwak_core-0.0.98/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-06-05 11:46:49.655906 qwak_core-0.0.98/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-06-05 11:46:44.463835 qwak_core-0.0.98/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.659906 qwak_core-0.0.98/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-06-05 11:46:49.651906 qwak_core-0.0.98/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-06-05 11:46:44.131830 qwak_core-0.0.98/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-06-05 11:46:49.655906 qwak_core-0.0.98/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-06-05 11:46:49.655906 qwak_core-0.0.98/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-06-05 11:46:44.299833 qwak_core-0.0.98/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.655906 qwak_core-0.0.98/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-06-05 11:46:49.635906 qwak_core-0.0.98/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-06-05 11:46:42.623805 qwak_core-0.0.98/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-06-05 11:46:49.635906 qwak_core-0.0.98/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-06-05 11:46:49.519904 qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-06-05 11:46:34.003682 qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-06-05 11:46:49.519904 qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-06-05 11:46:49.515904 qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-06-05 11:46:33.799680 qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.519904 qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-06-05 11:46:49.519904 qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-06-05 11:46:34.207685 qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-06-05 11:46:49.523904 qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-06-05 11:46:49.635906 qwak_core-0.0.98/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-06-05 11:46:42.251799 qwak_core-0.0.98/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-06-05 11:46:49.635906 qwak_core-0.0.98/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-06-05 11:46:49.647906 qwak_core-0.0.98/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-06-05 11:46:43.791825 qwak_core-0.0.98/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-06-05 11:46:49.651906 qwak_core-0.0.98/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-06-05 11:46:49.515904 qwak_core-0.0.98/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-06-05 11:46:31.899653 qwak_core-0.0.98/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.515904 qwak_core-0.0.98/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-06-05 11:46:49.511904 qwak_core-0.0.98/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-06-05 11:46:31.731650 qwak_core-0.0.98/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-06-05 11:46:49.515904 qwak_core-0.0.98/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-06-05 11:46:49.507904 qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-06-05 11:46:31.223643 qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.507904 qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-06-05 11:46:49.507904 qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-06-05 11:46:31.391646 qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.511904 qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-06-05 11:46:49.511904 qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-06-05 11:46:31.559648 qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-06-05 11:46:49.511904 qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-06-05 11:46:49.675906 qwak_core-0.0.98/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-06-05 11:46:46.003856 qwak_core-0.0.98/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-06-05 11:46:49.675906 qwak_core-0.0.98/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-06-05 11:46:49.671906 qwak_core-0.0.98/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-06-05 11:46:45.839854 qwak_core-0.0.98/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.671906 qwak_core-0.0.98/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    10961 2023-06-05 11:46:49.527904 qwak_core-0.0.98/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    14256 2023-06-05 11:46:33.087670 qwak_core-0.0.98/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.527904 qwak_core-0.0.98/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3072 2023-06-05 11:46:49.531904 qwak_core-0.0.98/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2663 2023-06-05 11:46:33.259672 qwak_core-0.0.98/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-05 11:46:49.531904 qwak_core-0.0.98/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-06-05 11:46:50.891923 qwak_core-0.0.98/pyproject.toml
--rw-r--r--   0        0        0      447 2023-06-05 11:46:50.891923 qwak_core-0.0.98/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    19458 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6370 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    15319 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-06-05 11:45:12.286585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-06-05 11:45:12.290585 qwak_core-0.0.98/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-06-05 11:45:12.294585 qwak_core-0.0.98/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.98/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.98/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-06-05 12:49:37.240028 qwak_core-0.0.99/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 12:51:30.848461 qwak_core-0.0.99/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-06-05 12:51:30.872461 qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-06-05 12:51:08.332371 qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.876461 qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-06-05 12:51:30.868461 qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-06-05 12:51:07.964369 qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.868461 qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-06-05 12:51:30.872461 qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-06-05 12:51:08.148370 qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.872461 qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-06-05 12:51:30.860461 qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-06-05 12:51:07.392367 qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-06-05 12:51:30.864461 qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-06-05 12:51:30.864461 qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-06-05 12:51:07.576368 qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.864461 qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4901 2023-06-05 12:51:30.864461 qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5995 2023-06-05 12:51:07.764369 qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.868461 qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-06-05 12:51:30.848461 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-06-05 12:51:07.212366 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-06-05 12:51:30.848461 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5707 2023-06-05 12:51:30.848461 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8170 2023-06-05 12:51:08.524372 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.852461 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-06-05 12:51:30.856461 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-06-05 12:51:08.928373 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.856461 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-06-05 12:51:30.856461 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-06-05 12:51:09.124374 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-06-05 12:51:30.856461 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-06-05 12:51:30.852461 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-06-05 12:51:08.736373 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.852461 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-06-05 12:51:30.860461 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-06-05 12:51:09.316375 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.860461 qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-06-05 12:51:30.904461 qwak_core-0.0.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-06-05 12:51:12.036386 qwak_core-0.0.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.904461 qwak_core-0.0.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-06-05 12:51:30.904461 qwak_core-0.0.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-06-05 12:51:12.232386 qwak_core-0.0.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-06-05 12:51:30.908461 qwak_core-0.0.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-06-05 12:51:30.976462 qwak_core-0.0.99/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-06-05 12:51:18.116410 qwak_core-0.0.99/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.980461 qwak_core-0.0.99/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-06-05 12:51:30.980461 qwak_core-0.0.99/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-06-05 12:51:18.308411 qwak_core-0.0.99/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-06-05 12:51:30.980461 qwak_core-0.0.99/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-06-05 12:51:30.984461 qwak_core-0.0.99/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-06-05 12:51:19.272415 qwak_core-0.0.99/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-06-05 12:51:30.984461 qwak_core-0.0.99/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-06-05 12:51:30.980461 qwak_core-0.0.99/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-06-05 12:51:19.076414 qwak_core-0.0.99/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.984461 qwak_core-0.0.99/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-06-05 12:51:30.984461 qwak_core-0.0.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-06-05 12:51:19.464415 qwak_core-0.0.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.988461 qwak_core-0.0.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-06-05 12:51:30.988461 qwak_core-0.0.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-06-05 12:51:19.652416 qwak_core-0.0.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-06-05 12:51:30.988461 qwak_core-0.0.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-06-05 12:51:31.084462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-06-05 12:51:28.436451 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.084462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-06-05 12:51:31.080462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-06-05 12:51:28.036450 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.080462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-06-05 12:51:31.080462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-06-05 12:51:28.240450 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.084462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-06-05 12:51:31.076462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-06-05 12:51:27.636448 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-06-05 12:51:31.076462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-06-05 12:51:31.076462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-06-05 12:51:27.836449 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.080462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-06-05 12:51:31.092462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-06-05 12:51:29.000454 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.092462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-06-05 12:51:31.088462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-06-05 12:51:28.812453 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.088462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-06-05 12:51:31.084462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-06-05 12:51:28.628452 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.088462 qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10989 2023-06-05 12:51:31.068462 qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    15193 2023-06-05 12:51:27.424447 qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.072462 qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-06-05 12:51:31.064462 qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-06-05 12:51:27.024446 qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.068462 qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    44118 2023-06-05 12:51:31.068462 qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    58049 2023-06-05 12:51:27.232447 qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-06-05 12:51:31.068462 qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20255 2023-06-05 12:51:31.016461 qwak_core-0.0.99/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    17495 2023-06-05 12:51:21.640424 qwak_core-0.0.99/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-06-05 12:51:31.016461 qwak_core-0.0.99/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-06-05 12:51:31.012462 qwak_core-0.0.99/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-06-05 12:51:21.448423 qwak_core-0.0.99/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.012462 qwak_core-0.0.99/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    13611 2023-06-05 12:51:31.004462 qwak_core-0.0.99/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    21063 2023-06-05 12:51:21.068422 qwak_core-0.0.99/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.004462 qwak_core-0.0.99/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-06-05 12:51:31.004462 qwak_core-0.0.99/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-06-05 12:51:21.252422 qwak_core-0.0.99/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.008462 qwak_core-0.0.99/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-06-05 12:51:31.008462 qwak_core-0.0.99/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-06-05 12:51:21.848425 qwak_core-0.0.99/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-06-05 12:51:31.008462 qwak_core-0.0.99/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38290 2023-06-05 12:51:31.012462 qwak_core-0.0.99/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52702 2023-06-05 12:51:22.312427 qwak_core-0.0.99/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-06-05 12:51:31.012462 qwak_core-0.0.99/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-06-05 12:51:31.020462 qwak_core-0.0.99/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-06-05 12:51:22.748428 qwak_core-0.0.99/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.024462 qwak_core-0.0.99/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-06-05 12:51:31.024462 qwak_core-0.0.99/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-06-05 12:51:22.976429 qwak_core-0.0.99/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-06-05 12:51:31.024462 qwak_core-0.0.99/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-06-05 12:51:30.996461 qwak_core-0.0.99/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-06-05 12:51:20.484419 qwak_core-0.0.99/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.996461 qwak_core-0.0.99/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-06-05 12:51:31.000461 qwak_core-0.0.99/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-06-05 12:51:20.676420 qwak_core-0.0.99/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-06-05 12:51:31.000461 qwak_core-0.0.99/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-06-05 12:51:30.992462 qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-06-05 12:51:20.056418 qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.992462 qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-06-05 12:51:30.992462 qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-06-05 12:51:19.860417 qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.992462 qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-06-05 12:51:30.996461 qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-06-05 12:51:20.288419 qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-06-05 12:51:30.996461 qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-06-05 12:51:30.892461 qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-06-05 12:51:11.060382 qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.892461 qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-06-05 12:51:30.896461 qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-06-05 12:51:11.252383 qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.896461 qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-06-05 12:51:30.896461 qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-06-05 12:51:11.452383 qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-06-05 12:51:30.900461 qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-06-05 12:51:30.956461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-06-05 12:51:16.972405 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.960461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-06-05 12:51:30.956461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-06-05 12:51:16.780405 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-06-05 12:51:30.956461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2023-06-05 12:51:30.932461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2023-06-05 12:51:14.564396 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.932461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0    13825 2023-06-05 12:51:30.944461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/deployment_pb2.py
+-rw-r--r--   0        0        0    19227 2023-06-05 12:51:15.540400 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.944461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     3307 2023-06-05 12:51:30.944461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py
+-rw-r--r--   0        0        0     1637 2023-06-05 12:51:15.732401 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0     3293 2023-06-05 12:51:30.944461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2023-06-05 12:51:30.928461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2023-06-05 12:51:14.372395 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.932461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-06-05 12:51:30.924461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-06-05 12:51:13.768393 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.924461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-06-05 12:51:30.928461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-06-05 12:51:14.180394 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-06-05 12:51:30.928461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-06-05 12:51:30.932461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-06-05 12:51:14.756397 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.936461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-06-05 12:51:30.936461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-06-05 12:51:14.944397 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-06-05 12:51:30.936461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25269 2023-06-05 12:51:30.924461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37664 2023-06-05 12:51:13.972393 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.928461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-06-05 12:51:30.940461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-06-05 12:51:15.144398 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.940461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    10504 2023-06-05 12:51:30.940461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    13308 2023-06-05 12:51:15.344399 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.940461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-06-05 12:51:30.960461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-06-05 12:51:30.364459 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.960461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-06-05 12:51:30.960461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-06-05 12:51:30.560460 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-06-05 12:51:30.964461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-06-05 12:51:30.964461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-06-05 12:51:17.540408 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.964461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-06-05 12:51:30.968461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-06-05 12:51:17.732408 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-06-05 12:51:30.968461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-06-05 12:51:30.968461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-06-05 12:51:17.924409 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.968461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-06-05 12:51:30.972461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-06-05 12:51:18.696412 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.972461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-06-05 12:51:30.972461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-06-05 12:51:18.500412 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-06-05 12:51:30.972461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-06-05 12:51:30.976462 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-06-05 12:51:18.884413 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.976462 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-06-05 12:51:30.948461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-06-05 12:51:15.988402 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.948461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-06-05 12:51:30.948461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-06-05 12:51:16.204402 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.948461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-06-05 12:51:30.952461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-06-05 12:51:16.396403 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-06-05 12:51:30.952461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-06-05 12:51:30.952461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-06-05 12:51:16.588404 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.956461 qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-06-05 12:51:31.092462 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-06-05 12:51:29.188454 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.092462 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-06-05 12:51:31.096462 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-06-05 12:51:29.376455 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-06-05 12:51:31.096462 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-06-05 12:51:31.096462 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-06-05 12:51:29.580456 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.096462 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-06-05 12:51:31.100462 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-06-05 12:51:29.780457 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-06-05 12:51:31.100462 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-06-05 12:51:31.100462 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-06-05 12:51:29.988458 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-06-05 12:51:31.104462 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-06-05 12:51:31.104462 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-06-05 12:51:30.176458 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.104462 qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-06-05 12:51:31.024462 qwak_core-0.0.99/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-06-05 12:51:23.200430 qwak_core-0.0.99/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.028462 qwak_core-0.0.99/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-06-05 12:51:31.028462 qwak_core-0.0.99/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-06-05 12:51:23.416431 qwak_core-0.0.99/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-06-05 12:51:31.028462 qwak_core-0.0.99/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-06-05 12:51:30.908461 qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-06-05 12:51:13.008390 qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.912461 qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-06-05 12:51:30.912461 qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-06-05 12:51:13.192390 qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.916461 qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-06-05 12:51:30.916461 qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-06-05 12:51:13.384391 qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-06-05 12:51:30.920461 qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-06-05 12:51:30.920461 qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-06-05 12:51:13.572392 qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.920461 qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-06-05 12:51:31.000461 qwak_core-0.0.99/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-06-05 12:51:20.868421 qwak_core-0.0.99/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-06-05 12:51:31.004462 qwak_core-0.0.99/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-06-05 12:51:31.032462 qwak_core-0.0.99/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-06-05 12:51:23.628432 qwak_core-0.0.99/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.032462 qwak_core-0.0.99/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-06-05 12:51:31.032462 qwak_core-0.0.99/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-06-05 12:51:23.836433 qwak_core-0.0.99/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-06-05 12:51:31.032462 qwak_core-0.0.99/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-06-05 12:51:31.044462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-06-05 12:51:25.132438 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.048462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-06-05 12:51:31.048462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-06-05 12:51:25.336439 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.048462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-06-05 12:51:31.048462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-06-05 12:51:25.564440 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.052462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-06-05 12:51:31.052462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-06-05 12:51:25.788441 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.052462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-06-05 12:51:31.052462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-06-05 12:51:26.008442 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.056462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-06-05 12:51:31.056462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-06-05 12:51:26.236442 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-06-05 12:51:31.056462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-06-05 12:51:31.060462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-06-05 12:51:26.440443 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.060462 qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-06-05 12:51:31.036462 qwak_core-0.0.99/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-06-05 12:51:24.248434 qwak_core-0.0.99/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.036462 qwak_core-0.0.99/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-06-05 12:51:31.044462 qwak_core-0.0.99/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-06-05 12:51:24.904437 qwak_core-0.0.99/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.044462 qwak_core-0.0.99/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-06-05 12:51:31.040462 qwak_core-0.0.99/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-06-05 12:51:24.480435 qwak_core-0.0.99/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-06-05 12:51:31.040462 qwak_core-0.0.99/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-06-05 12:51:31.040462 qwak_core-0.0.99/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-06-05 12:51:24.696436 qwak_core-0.0.99/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.040462 qwak_core-0.0.99/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-06-05 12:51:31.020462 qwak_core-0.0.99/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-06-05 12:51:22.536428 qwak_core-0.0.99/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-06-05 12:51:31.020462 qwak_core-0.0.99/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-06-05 12:51:30.888461 qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-06-05 12:51:12.620388 qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-06-05 12:51:30.888461 qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-06-05 12:51:30.888461 qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-06-05 12:51:12.432387 qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.888461 qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-06-05 12:51:30.892461 qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-06-05 12:51:12.812389 qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-06-05 12:51:30.892461 qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-06-05 12:51:31.016461 qwak_core-0.0.99/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-06-05 12:51:22.084426 qwak_core-0.0.99/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-06-05 12:51:31.020462 qwak_core-0.0.99/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-06-05 12:51:31.036462 qwak_core-0.0.99/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-06-05 12:51:24.044434 qwak_core-0.0.99/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-06-05 12:51:31.036462 qwak_core-0.0.99/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-06-05 12:51:30.884461 qwak_core-0.0.99/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-06-05 12:51:10.296379 qwak_core-0.0.99/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.884461 qwak_core-0.0.99/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-06-05 12:51:30.880461 qwak_core-0.0.99/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-06-05 12:51:10.100378 qwak_core-0.0.99/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-06-05 12:51:30.884461 qwak_core-0.0.99/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-06-05 12:51:30.876461 qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-06-05 12:51:09.516376 qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.876461 qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-06-05 12:51:30.876461 qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-06-05 12:51:09.708376 qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.880461 qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-06-05 12:51:30.880461 qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-06-05 12:51:09.900377 qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-06-05 12:51:30.880461 qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-06-05 12:51:31.064462 qwak_core-0.0.99/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-06-05 12:51:26.832445 qwak_core-0.0.99/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-06-05 12:51:31.064462 qwak_core-0.0.99/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-06-05 12:51:31.060462 qwak_core-0.0.99/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-06-05 12:51:26.644444 qwak_core-0.0.99/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:31.060462 qwak_core-0.0.99/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    10961 2023-06-05 12:51:30.900461 qwak_core-0.0.99/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    14256 2023-06-05 12:51:11.652384 qwak_core-0.0.99/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.900461 qwak_core-0.0.99/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3072 2023-06-05 12:51:30.900461 qwak_core-0.0.99/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2663 2023-06-05 12:51:11.844385 qwak_core-0.0.99/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 12:51:30.904461 qwak_core-0.0.99/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-06-05 12:51:32.504468 qwak_core-0.0.99/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-06-05 12:51:32.504468 qwak_core-0.0.99/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    19458 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6370 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    15319 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.240028 qwak_core-0.0.99/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.244028 qwak_core-0.0.99/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-06-05 12:49:37.248028 qwak_core-0.0.99/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.99/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.99/PKG-INFO
```

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,134 +1,169 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: qwak/feature_store/features/real_time_feature_extractor_deployment.proto
+# source: qwak/feature_store/jobs/v1/job_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from _qwak_proto.qwak.feature_store.jobs.v1 import job_pb2 as qwak_dot_feature__store_dot_jobs_dot_v1_dot_job__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHqwak/feature_store/features/real_time_feature_extractor_deployment.proto\x12\x1bqwak.feature.store.features\x1a\x1fgoogle/protobuf/timestamp.proto\"\xde\x02\n\x18\x45xtractorDeploymentBrief\x12\x15\n\rdeployment_id\x18\x01 \x01(\t\x12\x46\n\x06status\x18\x02 \x01(\x0e\x32\x36.qwak.feature.store.features.ExtractorDeploymentStatus\x12\x13\n\x0b\x64\x65ployed_by\x18\x03 \x01(\t\x12\x1b\n\x13\x66\x61ilure_reason_code\x18\x04 \x01(\t\x12\x17\n\x0f\x66\x61ilure_message\x18\x05 \x01(\t\x12\x19\n\x11technical_details\x18\x06 \x01(\t\x12\x38\n\x14\x64\x65ployment_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x65xtractor_id\x18\x08 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\t \x01(\t\x12\x15\n\rfeatureset_id\x18\n \x01(\t\"\xfe\x01\n\"KubernetesExtractorDeploymentState\x12\x1f\n\x17\x65xtractor_deployment_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xtractor_id\x18\x02 \x01(\t\x12\x15\n\rfeatureset_id\x18\x03 \x01(\t\x12\x46\n\x06status\x18\x04 \x01(\x0e\x32\x36.qwak.feature.store.features.ExtractorDeploymentStatus\x12\x42\n\x0estatus_details\x18\x05 \x01(\x0b\x32*.qwak.feature.store.features.StatusDetails\"\xa1\x02\n\rStatusDetails\x12S\n\x16pending_status_details\x18\x01 \x01(\x0b\x32\x31.qwak.feature.store.features.PendingStatusDetailsH\x00\x12V\n\x16success_status_details\x18\x02 \x01(\x0b\x32\x34.qwak.feature.store.features.SuccessfulStatusDetailsH\x00\x12Q\n\x15\x66\x61iled_status_details\x18\x03 \x01(\x0b\x32\x30.qwak.feature.store.features.FailedStatusDetailsH\x00\x42\x10\n\x0estatus_details\"\x9e\x01\n\x14PendingStatusDetails\x12\x42\n\x0cold_instance\x18\x01 \x01(\x0b\x32,.qwak.feature.store.features.InstanceDetails\x12\x42\n\x0cnew_instance\x18\x02 \x01(\x0b\x32,.qwak.feature.store.features.InstanceDetails\"a\n\x17SuccessfulStatusDetails\x12\x46\n\x10running_instance\x18\x01 \x01(\x0b\x32,.qwak.feature.store.features.InstanceDetails\"\xe6\x01\n\x13\x46\x61iledStatusDetails\x12\x44\n\x0f\x66\x61ilure_details\x18\x01 \x01(\x0b\x32+.qwak.feature.store.features.FailureDetails\x12\x42\n\x0cold_instance\x18\x02 \x01(\x0b\x32,.qwak.feature.store.features.InstanceDetails\x12\x45\n\x0f\x66\x61iled_instance\x18\x03 \x01(\x0b\x32,.qwak.feature.store.features.InstanceDetails\"\x92\x01\n\x0e\x46\x61ilureDetails\x12`\n\x1e\x64\x65ployment_failure_reason_code\x18\x01 \x01(\x0e\x32\x38.qwak.feature.store.features.DeploymentFailureReasonCode\x12\x1e\n\x16\x66\x61ilure_reason_details\x18\x02 \x01(\t\"Z\n\x0fInstanceDetails\x12\x15\n\rdeployment_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xtractor_id\x18\x02 \x01(\t\x12\x1a\n\x12\x61vailable_replicas\x18\x03 \x01(\x05*\xa7\x02\n\x19\x45xtractorDeploymentStatus\x12\x16\n\x12INVALID_DEPLOYMENT\x10\x00\x12\x19\n\x15INITIATING_DEPLOYMENT\x10\x01\x12 \n\x1c\x46\x41ILED_INITIATING_DEPLOYMENT\x10\x02\x12\x16\n\x12PENDING_DEPLOYMENT\x10\x03\x12\x19\n\x15SUCCESSFUL_DEPLOYMENT\x10\x04\x12\x15\n\x11\x46\x41ILED_DEPLOYMENT\x10\x05\x12\x1b\n\x17INITIATING_UNDEPLOYMENT\x10\x06\x12\x18\n\x14PENDING_UNDEPLOYMENT\x10\x07\x12\x1b\n\x17SUCCESSFUL_UNDEPLOYMENT\x10\x08\x12\x17\n\x13\x46\x41ILED_UNDEPLOYMENT\x10\t*\x97\x02\n\x1b\x44\x65ploymentFailureReasonCode\x12\x18\n\x14INVALID_FAILURE_CODE\x10\x00\x12\x12\n\x0eUNKNOWN_REASON\x10\x01\x12\x1e\n\x1aNO_REPLICA_SETS_PODS_FOUND\x10\x02\x12!\n\x1d\x45XTRACTOR_CONTAINER_NOT_FOUND\x10\x03\x12\x11\n\rUNSCHEDULABLE\x10\x04\x12\x1a\n\x16\x44OCKER_IMAGE_NOT_FOUND\x10\x05\x12\x19\n\x15MEMORY_LIMIT_EXCEEDED\x10\x06\x12\x0e\n\nCRASH_LOOP\x10\x07\x12-\n)CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON\x10\x08\x42[\n&com.qwak.ai.feature.store.features.apiP\x01Z/qwak/featurestore/features;featurestorefeaturesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,qwak/feature_store/jobs/v1/job_service.proto\x12\x1aqwak.feature.store.jobs.v1\x1a$qwak/feature_store/jobs/v1/job.proto\"b\n!DeleteFeaturesetJobByJobIdRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x02 \x01(\t\x12\x0e\n\x06job_id\x18\x03 \x01(\t\"F\n\"DeleteFeaturesetJobByJobIdResponse\x12 \n\x18\x64\x65leted_job_record_count\x18\x01 \x01(\x05\"L\n\x0f\x41pplyJobRequest\x12\x39\n\njob_record\x18\x01 \x01(\x0b\x32%.qwak.feature.store.jobs.v1.JobRecord\":\n\x10\x41pplyJobResponse\x12\x16\n\x0ejob_running_id\x18\x01 \x01(\x03\x12\x0e\n\x06job_id\x18\x02 \x01(\t\"F\n\x15InitPaginationRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x02 \x01(\t\"Q\n\x16InitPaginationResponse\x12\x14\n\x0crecord_count\x18\x01 \x01(\x03\x12!\n\x19pagination_session_max_id\x18\x02 \x01(\x03\"\x8b\x01\n\x0fListJobsRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x02 \x01(\t\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\x13\n\x0bpage_number\x18\x04 \x01(\x05\x12!\n\x19pagination_session_max_id\x18\x05 \x01(\x03\"G\n\x10ListJobsResponse\x12\x33\n\x04jobs\x18\x01 \x03(\x0b\x32%.qwak.feature.store.jobs.v1.JobRecord\"N\n\x1dGetLatestSuccessfulJobRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x02 \x01(\t\"D\n\x13GetLatestJobRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x02 \x01(\t\"J\n\x14GetLatestJobResponse\x12\x32\n\x03job\x18\x01 \x01(\x0b\x32%.qwak.feature.store.jobs.v1.JobRecord\"c\n\x1eGetLatestSuccessfulJobResponse\x12\x32\n\x03job\x18\x01 \x01(\x0b\x32%.qwak.feature.store.jobs.v1.JobRecord\x12\r\n\x05\x66ound\x18\x02 \x01(\x08\"L\n\x1b\x44\x65leteFeaturesetJobsRequest\x12\x15\n\rfeatureset_id\x18\x01 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x02 \x01(\t\"A\n\x1c\x44\x65leteFeaturesetJobsResponse\x12!\n\x19\x64\x65leted_job_records_count\x18\x01 \x01(\x05\x32\x82\x07\n\nJobService\x12\x65\n\x08\x41pplyJob\x12+.qwak.feature.store.jobs.v1.ApplyJobRequest\x1a,.qwak.feature.store.jobs.v1.ApplyJobResponse\x12w\n\x0eInitPagination\x12\x31.qwak.feature.store.jobs.v1.InitPaginationRequest\x1a\x32.qwak.feature.store.jobs.v1.InitPaginationResponse\x12\x65\n\x08ListJobs\x12+.qwak.feature.store.jobs.v1.ListJobsRequest\x1a,.qwak.feature.store.jobs.v1.ListJobsResponse\x12\x8f\x01\n\x16GetLatestSuccessfulJob\x12\x39.qwak.feature.store.jobs.v1.GetLatestSuccessfulJobRequest\x1a:.qwak.feature.store.jobs.v1.GetLatestSuccessfulJobResponse\x12q\n\x0cGetLatestJob\x12/.qwak.feature.store.jobs.v1.GetLatestJobRequest\x1a\x30.qwak.feature.store.jobs.v1.GetLatestJobResponse\x12\x89\x01\n\x14\x44\x65leteFeaturesetJobs\x12\x37.qwak.feature.store.jobs.v1.DeleteFeaturesetJobsRequest\x1a\x38.qwak.feature.store.jobs.v1.DeleteFeaturesetJobsResponse\x12\x9b\x01\n\x1a\x44\x65leteFeaturesetJobByJobId\x12=.qwak.feature.store.jobs.v1.DeleteFeaturesetJobByJobIdRequest\x1a>.qwak.feature.store.jobs.v1.DeleteFeaturesetJobByJobIdResponseB=\n%com.qwak.ai.feature.store.jobs.v1.apiP\x01Z\x12qwak/fsjobs;fsjobsb\x06proto3')
 
-_EXTRACTORDEPLOYMENTSTATUS = DESCRIPTOR.enum_types_by_name['ExtractorDeploymentStatus']
-ExtractorDeploymentStatus = enum_type_wrapper.EnumTypeWrapper(_EXTRACTORDEPLOYMENTSTATUS)
-_DEPLOYMENTFAILUREREASONCODE = DESCRIPTOR.enum_types_by_name['DeploymentFailureReasonCode']
-DeploymentFailureReasonCode = enum_type_wrapper.EnumTypeWrapper(_DEPLOYMENTFAILUREREASONCODE)
-INVALID_DEPLOYMENT = 0
-INITIATING_DEPLOYMENT = 1
-FAILED_INITIATING_DEPLOYMENT = 2
-PENDING_DEPLOYMENT = 3
-SUCCESSFUL_DEPLOYMENT = 4
-FAILED_DEPLOYMENT = 5
-INITIATING_UNDEPLOYMENT = 6
-PENDING_UNDEPLOYMENT = 7
-SUCCESSFUL_UNDEPLOYMENT = 8
-FAILED_UNDEPLOYMENT = 9
-INVALID_FAILURE_CODE = 0
-UNKNOWN_REASON = 1
-NO_REPLICA_SETS_PODS_FOUND = 2
-EXTRACTOR_CONTAINER_NOT_FOUND = 3
-UNSCHEDULABLE = 4
-DOCKER_IMAGE_NOT_FOUND = 5
-MEMORY_LIMIT_EXCEEDED = 6
-CRASH_LOOP = 7
-CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON = 8
-
-
-_EXTRACTORDEPLOYMENTBRIEF = DESCRIPTOR.message_types_by_name['ExtractorDeploymentBrief']
-_KUBERNETESEXTRACTORDEPLOYMENTSTATE = DESCRIPTOR.message_types_by_name['KubernetesExtractorDeploymentState']
-_STATUSDETAILS = DESCRIPTOR.message_types_by_name['StatusDetails']
-_PENDINGSTATUSDETAILS = DESCRIPTOR.message_types_by_name['PendingStatusDetails']
-_SUCCESSFULSTATUSDETAILS = DESCRIPTOR.message_types_by_name['SuccessfulStatusDetails']
-_FAILEDSTATUSDETAILS = DESCRIPTOR.message_types_by_name['FailedStatusDetails']
-_FAILUREDETAILS = DESCRIPTOR.message_types_by_name['FailureDetails']
-_INSTANCEDETAILS = DESCRIPTOR.message_types_by_name['InstanceDetails']
-ExtractorDeploymentBrief = _reflection.GeneratedProtocolMessageType('ExtractorDeploymentBrief', (_message.Message,), {
-  'DESCRIPTOR' : _EXTRACTORDEPLOYMENTBRIEF,
-  '__module__' : 'qwak.feature_store.features.real_time_feature_extractor_deployment_pb2'
-  # @@protoc_insertion_point(class_scope:qwak.feature.store.features.ExtractorDeploymentBrief)
-  })
-_sym_db.RegisterMessage(ExtractorDeploymentBrief)
-
-KubernetesExtractorDeploymentState = _reflection.GeneratedProtocolMessageType('KubernetesExtractorDeploymentState', (_message.Message,), {
-  'DESCRIPTOR' : _KUBERNETESEXTRACTORDEPLOYMENTSTATE,
-  '__module__' : 'qwak.feature_store.features.real_time_feature_extractor_deployment_pb2'
-  # @@protoc_insertion_point(class_scope:qwak.feature.store.features.KubernetesExtractorDeploymentState)
-  })
-_sym_db.RegisterMessage(KubernetesExtractorDeploymentState)
-
-StatusDetails = _reflection.GeneratedProtocolMessageType('StatusDetails', (_message.Message,), {
-  'DESCRIPTOR' : _STATUSDETAILS,
-  '__module__' : 'qwak.feature_store.features.real_time_feature_extractor_deployment_pb2'
-  # @@protoc_insertion_point(class_scope:qwak.feature.store.features.StatusDetails)
-  })
-_sym_db.RegisterMessage(StatusDetails)
-
-PendingStatusDetails = _reflection.GeneratedProtocolMessageType('PendingStatusDetails', (_message.Message,), {
-  'DESCRIPTOR' : _PENDINGSTATUSDETAILS,
-  '__module__' : 'qwak.feature_store.features.real_time_feature_extractor_deployment_pb2'
-  # @@protoc_insertion_point(class_scope:qwak.feature.store.features.PendingStatusDetails)
-  })
-_sym_db.RegisterMessage(PendingStatusDetails)
-
-SuccessfulStatusDetails = _reflection.GeneratedProtocolMessageType('SuccessfulStatusDetails', (_message.Message,), {
-  'DESCRIPTOR' : _SUCCESSFULSTATUSDETAILS,
-  '__module__' : 'qwak.feature_store.features.real_time_feature_extractor_deployment_pb2'
-  # @@protoc_insertion_point(class_scope:qwak.feature.store.features.SuccessfulStatusDetails)
-  })
-_sym_db.RegisterMessage(SuccessfulStatusDetails)
-
-FailedStatusDetails = _reflection.GeneratedProtocolMessageType('FailedStatusDetails', (_message.Message,), {
-  'DESCRIPTOR' : _FAILEDSTATUSDETAILS,
-  '__module__' : 'qwak.feature_store.features.real_time_feature_extractor_deployment_pb2'
-  # @@protoc_insertion_point(class_scope:qwak.feature.store.features.FailedStatusDetails)
-  })
-_sym_db.RegisterMessage(FailedStatusDetails)
-
-FailureDetails = _reflection.GeneratedProtocolMessageType('FailureDetails', (_message.Message,), {
-  'DESCRIPTOR' : _FAILUREDETAILS,
-  '__module__' : 'qwak.feature_store.features.real_time_feature_extractor_deployment_pb2'
-  # @@protoc_insertion_point(class_scope:qwak.feature.store.features.FailureDetails)
-  })
-_sym_db.RegisterMessage(FailureDetails)
-
-InstanceDetails = _reflection.GeneratedProtocolMessageType('InstanceDetails', (_message.Message,), {
-  'DESCRIPTOR' : _INSTANCEDETAILS,
-  '__module__' : 'qwak.feature_store.features.real_time_feature_extractor_deployment_pb2'
-  # @@protoc_insertion_point(class_scope:qwak.feature.store.features.InstanceDetails)
+
+
+_DELETEFEATURESETJOBBYJOBIDREQUEST = DESCRIPTOR.message_types_by_name['DeleteFeaturesetJobByJobIdRequest']
+_DELETEFEATURESETJOBBYJOBIDRESPONSE = DESCRIPTOR.message_types_by_name['DeleteFeaturesetJobByJobIdResponse']
+_APPLYJOBREQUEST = DESCRIPTOR.message_types_by_name['ApplyJobRequest']
+_APPLYJOBRESPONSE = DESCRIPTOR.message_types_by_name['ApplyJobResponse']
+_INITPAGINATIONREQUEST = DESCRIPTOR.message_types_by_name['InitPaginationRequest']
+_INITPAGINATIONRESPONSE = DESCRIPTOR.message_types_by_name['InitPaginationResponse']
+_LISTJOBSREQUEST = DESCRIPTOR.message_types_by_name['ListJobsRequest']
+_LISTJOBSRESPONSE = DESCRIPTOR.message_types_by_name['ListJobsResponse']
+_GETLATESTSUCCESSFULJOBREQUEST = DESCRIPTOR.message_types_by_name['GetLatestSuccessfulJobRequest']
+_GETLATESTJOBREQUEST = DESCRIPTOR.message_types_by_name['GetLatestJobRequest']
+_GETLATESTJOBRESPONSE = DESCRIPTOR.message_types_by_name['GetLatestJobResponse']
+_GETLATESTSUCCESSFULJOBRESPONSE = DESCRIPTOR.message_types_by_name['GetLatestSuccessfulJobResponse']
+_DELETEFEATURESETJOBSREQUEST = DESCRIPTOR.message_types_by_name['DeleteFeaturesetJobsRequest']
+_DELETEFEATURESETJOBSRESPONSE = DESCRIPTOR.message_types_by_name['DeleteFeaturesetJobsResponse']
+DeleteFeaturesetJobByJobIdRequest = _reflection.GeneratedProtocolMessageType('DeleteFeaturesetJobByJobIdRequest', (_message.Message,), {
+  'DESCRIPTOR' : _DELETEFEATURESETJOBBYJOBIDREQUEST,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.DeleteFeaturesetJobByJobIdRequest)
+  })
+_sym_db.RegisterMessage(DeleteFeaturesetJobByJobIdRequest)
+
+DeleteFeaturesetJobByJobIdResponse = _reflection.GeneratedProtocolMessageType('DeleteFeaturesetJobByJobIdResponse', (_message.Message,), {
+  'DESCRIPTOR' : _DELETEFEATURESETJOBBYJOBIDRESPONSE,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.DeleteFeaturesetJobByJobIdResponse)
+  })
+_sym_db.RegisterMessage(DeleteFeaturesetJobByJobIdResponse)
+
+ApplyJobRequest = _reflection.GeneratedProtocolMessageType('ApplyJobRequest', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYJOBREQUEST,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.ApplyJobRequest)
+  })
+_sym_db.RegisterMessage(ApplyJobRequest)
+
+ApplyJobResponse = _reflection.GeneratedProtocolMessageType('ApplyJobResponse', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYJOBRESPONSE,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.ApplyJobResponse)
+  })
+_sym_db.RegisterMessage(ApplyJobResponse)
+
+InitPaginationRequest = _reflection.GeneratedProtocolMessageType('InitPaginationRequest', (_message.Message,), {
+  'DESCRIPTOR' : _INITPAGINATIONREQUEST,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.InitPaginationRequest)
+  })
+_sym_db.RegisterMessage(InitPaginationRequest)
+
+InitPaginationResponse = _reflection.GeneratedProtocolMessageType('InitPaginationResponse', (_message.Message,), {
+  'DESCRIPTOR' : _INITPAGINATIONRESPONSE,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.InitPaginationResponse)
+  })
+_sym_db.RegisterMessage(InitPaginationResponse)
+
+ListJobsRequest = _reflection.GeneratedProtocolMessageType('ListJobsRequest', (_message.Message,), {
+  'DESCRIPTOR' : _LISTJOBSREQUEST,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.ListJobsRequest)
+  })
+_sym_db.RegisterMessage(ListJobsRequest)
+
+ListJobsResponse = _reflection.GeneratedProtocolMessageType('ListJobsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _LISTJOBSRESPONSE,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.ListJobsResponse)
+  })
+_sym_db.RegisterMessage(ListJobsResponse)
+
+GetLatestSuccessfulJobRequest = _reflection.GeneratedProtocolMessageType('GetLatestSuccessfulJobRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETLATESTSUCCESSFULJOBREQUEST,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.GetLatestSuccessfulJobRequest)
+  })
+_sym_db.RegisterMessage(GetLatestSuccessfulJobRequest)
+
+GetLatestJobRequest = _reflection.GeneratedProtocolMessageType('GetLatestJobRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETLATESTJOBREQUEST,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.GetLatestJobRequest)
+  })
+_sym_db.RegisterMessage(GetLatestJobRequest)
+
+GetLatestJobResponse = _reflection.GeneratedProtocolMessageType('GetLatestJobResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETLATESTJOBRESPONSE,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.GetLatestJobResponse)
+  })
+_sym_db.RegisterMessage(GetLatestJobResponse)
+
+GetLatestSuccessfulJobResponse = _reflection.GeneratedProtocolMessageType('GetLatestSuccessfulJobResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETLATESTSUCCESSFULJOBRESPONSE,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.GetLatestSuccessfulJobResponse)
+  })
+_sym_db.RegisterMessage(GetLatestSuccessfulJobResponse)
+
+DeleteFeaturesetJobsRequest = _reflection.GeneratedProtocolMessageType('DeleteFeaturesetJobsRequest', (_message.Message,), {
+  'DESCRIPTOR' : _DELETEFEATURESETJOBSREQUEST,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.DeleteFeaturesetJobsRequest)
+  })
+_sym_db.RegisterMessage(DeleteFeaturesetJobsRequest)
+
+DeleteFeaturesetJobsResponse = _reflection.GeneratedProtocolMessageType('DeleteFeaturesetJobsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _DELETEFEATURESETJOBSRESPONSE,
+  '__module__' : 'qwak.feature_store.jobs.v1.job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.jobs.v1.DeleteFeaturesetJobsResponse)
   })
-_sym_db.RegisterMessage(InstanceDetails)
+_sym_db.RegisterMessage(DeleteFeaturesetJobsResponse)
 
+_JOBSERVICE = DESCRIPTOR.services_by_name['JobService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n&com.qwak.ai.feature.store.features.apiP\001Z/qwak/featurestore/features;featurestorefeatures'
-  _EXTRACTORDEPLOYMENTSTATUS._serialized_start=1775
-  _EXTRACTORDEPLOYMENTSTATUS._serialized_end=2070
-  _DEPLOYMENTFAILUREREASONCODE._serialized_start=2073
-  _DEPLOYMENTFAILUREREASONCODE._serialized_end=2352
-  _EXTRACTORDEPLOYMENTBRIEF._serialized_start=139
-  _EXTRACTORDEPLOYMENTBRIEF._serialized_end=489
-  _KUBERNETESEXTRACTORDEPLOYMENTSTATE._serialized_start=492
-  _KUBERNETESEXTRACTORDEPLOYMENTSTATE._serialized_end=746
-  _STATUSDETAILS._serialized_start=749
-  _STATUSDETAILS._serialized_end=1038
-  _PENDINGSTATUSDETAILS._serialized_start=1041
-  _PENDINGSTATUSDETAILS._serialized_end=1199
-  _SUCCESSFULSTATUSDETAILS._serialized_start=1201
-  _SUCCESSFULSTATUSDETAILS._serialized_end=1298
-  _FAILEDSTATUSDETAILS._serialized_start=1301
-  _FAILEDSTATUSDETAILS._serialized_end=1531
-  _FAILUREDETAILS._serialized_start=1534
-  _FAILUREDETAILS._serialized_end=1680
-  _INSTANCEDETAILS._serialized_start=1682
-  _INSTANCEDETAILS._serialized_end=1772
+  DESCRIPTOR._serialized_options = b'\n%com.qwak.ai.feature.store.jobs.v1.apiP\001Z\022qwak/fsjobs;fsjobs'
+  _DELETEFEATURESETJOBBYJOBIDREQUEST._serialized_start=114
+  _DELETEFEATURESETJOBBYJOBIDREQUEST._serialized_end=212
+  _DELETEFEATURESETJOBBYJOBIDRESPONSE._serialized_start=214
+  _DELETEFEATURESETJOBBYJOBIDRESPONSE._serialized_end=284
+  _APPLYJOBREQUEST._serialized_start=286
+  _APPLYJOBREQUEST._serialized_end=362
+  _APPLYJOBRESPONSE._serialized_start=364
+  _APPLYJOBRESPONSE._serialized_end=422
+  _INITPAGINATIONREQUEST._serialized_start=424
+  _INITPAGINATIONREQUEST._serialized_end=494
+  _INITPAGINATIONRESPONSE._serialized_start=496
+  _INITPAGINATIONRESPONSE._serialized_end=577
+  _LISTJOBSREQUEST._serialized_start=580
+  _LISTJOBSREQUEST._serialized_end=719
+  _LISTJOBSRESPONSE._serialized_start=721
+  _LISTJOBSRESPONSE._serialized_end=792
+  _GETLATESTSUCCESSFULJOBREQUEST._serialized_start=794
+  _GETLATESTSUCCESSFULJOBREQUEST._serialized_end=872
+  _GETLATESTJOBREQUEST._serialized_start=874
+  _GETLATESTJOBREQUEST._serialized_end=942
+  _GETLATESTJOBRESPONSE._serialized_start=944
+  _GETLATESTJOBRESPONSE._serialized_end=1018
+  _GETLATESTSUCCESSFULJOBRESPONSE._serialized_start=1020
+  _GETLATESTSUCCESSFULJOBRESPONSE._serialized_end=1119
+  _DELETEFEATURESETJOBSREQUEST._serialized_start=1121
+  _DELETEFEATURESETJOBSREQUEST._serialized_end=1197
+  _DELETEFEATURESETJOBSRESPONSE._serialized_start=1199
+  _DELETEFEATURESETJOBSRESPONSE._serialized_end=1264
+  _JOBSERVICE._serialized_start=1267
+  _JOBSERVICE._serialized_end=2165
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -2,90 +2,104 @@
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
-import google.protobuf.timestamp_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class _ExtractorDeploymentStatus:
+class _DeploymentUpdateRequestStatus:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _ExtractorDeploymentStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ExtractorDeploymentStatus.ValueType], builtins.type):  # noqa: F821
+class _DeploymentUpdateRequestStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_DeploymentUpdateRequestStatus.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
-    INVALID_DEPLOYMENT: _ExtractorDeploymentStatus.ValueType  # 0
-    """Invalid deployment status"""
-    INITIATING_DEPLOYMENT: _ExtractorDeploymentStatus.ValueType  # 1
-    """Deployment is initiating"""
-    FAILED_INITIATING_DEPLOYMENT: _ExtractorDeploymentStatus.ValueType  # 2
-    """Failed to initiate a deployment process"""
-    PENDING_DEPLOYMENT: _ExtractorDeploymentStatus.ValueType  # 3
-    """Deployment is in progress"""
-    SUCCESSFUL_DEPLOYMENT: _ExtractorDeploymentStatus.ValueType  # 4
-    """Deployment has finished successfully"""
-    FAILED_DEPLOYMENT: _ExtractorDeploymentStatus.ValueType  # 5
-    """Deployment has failed"""
-    INITIATING_UNDEPLOYMENT: _ExtractorDeploymentStatus.ValueType  # 6
-    """Undeployment is initiating"""
-    PENDING_UNDEPLOYMENT: _ExtractorDeploymentStatus.ValueType  # 7
-    """Undeployment is in progress"""
-    SUCCESSFUL_UNDEPLOYMENT: _ExtractorDeploymentStatus.ValueType  # 8
-    """Extractor is undeployed"""
-    FAILED_UNDEPLOYMENT: _ExtractorDeploymentStatus.ValueType  # 9
-    """Undeployment has failed"""
-
-class ExtractorDeploymentStatus(_ExtractorDeploymentStatus, metaclass=_ExtractorDeploymentStatusEnumTypeWrapper): ...
-
-INVALID_DEPLOYMENT: ExtractorDeploymentStatus.ValueType  # 0
-"""Invalid deployment status"""
-INITIATING_DEPLOYMENT: ExtractorDeploymentStatus.ValueType  # 1
-"""Deployment is initiating"""
-FAILED_INITIATING_DEPLOYMENT: ExtractorDeploymentStatus.ValueType  # 2
-"""Failed to initiate a deployment process"""
-PENDING_DEPLOYMENT: ExtractorDeploymentStatus.ValueType  # 3
-"""Deployment is in progress"""
-SUCCESSFUL_DEPLOYMENT: ExtractorDeploymentStatus.ValueType  # 4
-"""Deployment has finished successfully"""
-FAILED_DEPLOYMENT: ExtractorDeploymentStatus.ValueType  # 5
-"""Deployment has failed"""
-INITIATING_UNDEPLOYMENT: ExtractorDeploymentStatus.ValueType  # 6
-"""Undeployment is initiating"""
-PENDING_UNDEPLOYMENT: ExtractorDeploymentStatus.ValueType  # 7
-"""Undeployment is in progress"""
-SUCCESSFUL_UNDEPLOYMENT: ExtractorDeploymentStatus.ValueType  # 8
-"""Extractor is undeployed"""
-FAILED_UNDEPLOYMENT: ExtractorDeploymentStatus.ValueType  # 9
-"""Undeployment has failed"""
-global___ExtractorDeploymentStatus = ExtractorDeploymentStatus
+    DEPLOYMENT_UPDATE_REQUEST_INVALID_STATUS: _DeploymentUpdateRequestStatus.ValueType  # 0
+    """Invalid proto status"""
+    INVALID_DEPLOYMENT_UPDATE_REQUEST: _DeploymentUpdateRequestStatus.ValueType  # 1
+    """Invalid deployment update request status"""
+    INITIATING_DEPLOYMENT_UPDATE_REQUEST: _DeploymentUpdateRequestStatus.ValueType  # 2
+    """Deployment update request is initiating"""
+    FAILED_INITIATING_DEPLOYMENT_UPDATE_REQUEST: _DeploymentUpdateRequestStatus.ValueType  # 3
+    """Failed to initiate a deployment update request process"""
+    PENDING_DEPLOYMENT_UPDATE_REQUEST: _DeploymentUpdateRequestStatus.ValueType  # 4
+    """Deployment update request is in progress"""
+    SUCCESSFUL_DEPLOYMENT_UPDATE_REQUEST: _DeploymentUpdateRequestStatus.ValueType  # 5
+    """Deployment update request has finished successfully"""
+
+class DeploymentUpdateRequestStatus(_DeploymentUpdateRequestStatus, metaclass=_DeploymentUpdateRequestStatusEnumTypeWrapper): ...
+
+DEPLOYMENT_UPDATE_REQUEST_INVALID_STATUS: DeploymentUpdateRequestStatus.ValueType  # 0
+"""Invalid proto status"""
+INVALID_DEPLOYMENT_UPDATE_REQUEST: DeploymentUpdateRequestStatus.ValueType  # 1
+"""Invalid deployment update request status"""
+INITIATING_DEPLOYMENT_UPDATE_REQUEST: DeploymentUpdateRequestStatus.ValueType  # 2
+"""Deployment update request is initiating"""
+FAILED_INITIATING_DEPLOYMENT_UPDATE_REQUEST: DeploymentUpdateRequestStatus.ValueType  # 3
+"""Failed to initiate a deployment update request process"""
+PENDING_DEPLOYMENT_UPDATE_REQUEST: DeploymentUpdateRequestStatus.ValueType  # 4
+"""Deployment update request is in progress"""
+SUCCESSFUL_DEPLOYMENT_UPDATE_REQUEST: DeploymentUpdateRequestStatus.ValueType  # 5
+"""Deployment update request has finished successfully"""
+global___DeploymentUpdateRequestStatus = DeploymentUpdateRequestStatus
+
+class _DeploymentStatus:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _DeploymentStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_DeploymentStatus.ValueType], builtins.type):  # noqa: F821
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    DEPLOYMENT_INVALID_STATUS: _DeploymentStatus.ValueType  # 0
+    """Invalid proto status"""
+    DEPLOYMENT_RUNNING: _DeploymentStatus.ValueType  # 1
+    """DEPLOYMENT IS IN RUNNING STATE"""
+    DEPLOYMENT_UPDATE_IN_PROGRESS: _DeploymentStatus.ValueType  # 2
+    """DEPLOYMENT UPDATE REQUEST IS IN PROGRESS"""
+    DEPLOYMENT_UNDEPLOYED: _DeploymentStatus.ValueType  # 3
+    """DEPLOYMENT WAS DELETED"""
+    DEPLOYMENT_FAILED: _DeploymentStatus.ValueType  # 4
+    """DEPLOYMENT IS FAILING"""
+
+class DeploymentStatus(_DeploymentStatus, metaclass=_DeploymentStatusEnumTypeWrapper): ...
+
+DEPLOYMENT_INVALID_STATUS: DeploymentStatus.ValueType  # 0
+"""Invalid proto status"""
+DEPLOYMENT_RUNNING: DeploymentStatus.ValueType  # 1
+"""DEPLOYMENT IS IN RUNNING STATE"""
+DEPLOYMENT_UPDATE_IN_PROGRESS: DeploymentStatus.ValueType  # 2
+"""DEPLOYMENT UPDATE REQUEST IS IN PROGRESS"""
+DEPLOYMENT_UNDEPLOYED: DeploymentStatus.ValueType  # 3
+"""DEPLOYMENT WAS DELETED"""
+DEPLOYMENT_FAILED: DeploymentStatus.ValueType  # 4
+"""DEPLOYMENT IS FAILING"""
+global___DeploymentStatus = DeploymentStatus
 
 class _DeploymentFailureReasonCode:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _DeploymentFailureReasonCodeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_DeploymentFailureReasonCode.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     INVALID_FAILURE_CODE: _DeploymentFailureReasonCode.ValueType  # 0
     """Invalid failure reason"""
     UNKNOWN_REASON: _DeploymentFailureReasonCode.ValueType  # 1
     """Unknown failure reason"""
     NO_REPLICA_SETS_PODS_FOUND: _DeploymentFailureReasonCode.ValueType  # 2
     """No replica sets pods found reason"""
-    EXTRACTOR_CONTAINER_NOT_FOUND: _DeploymentFailureReasonCode.ValueType  # 3
-    """Extractor container not found reason"""
+    CONTAINER_NOT_FOUND: _DeploymentFailureReasonCode.ValueType  # 3
+    """Container not found reason"""
     UNSCHEDULABLE: _DeploymentFailureReasonCode.ValueType  # 4
     """Unschedulable reason"""
     DOCKER_IMAGE_NOT_FOUND: _DeploymentFailureReasonCode.ValueType  # 5
     """Docker image not found reason"""
     MEMORY_LIMIT_EXCEEDED: _DeploymentFailureReasonCode.ValueType  # 6
     """Memory limit exceeded reason"""
     CRASH_LOOP: _DeploymentFailureReasonCode.ValueType  # 7
@@ -97,196 +111,210 @@
 
 INVALID_FAILURE_CODE: DeploymentFailureReasonCode.ValueType  # 0
 """Invalid failure reason"""
 UNKNOWN_REASON: DeploymentFailureReasonCode.ValueType  # 1
 """Unknown failure reason"""
 NO_REPLICA_SETS_PODS_FOUND: DeploymentFailureReasonCode.ValueType  # 2
 """No replica sets pods found reason"""
-EXTRACTOR_CONTAINER_NOT_FOUND: DeploymentFailureReasonCode.ValueType  # 3
-"""Extractor container not found reason"""
+CONTAINER_NOT_FOUND: DeploymentFailureReasonCode.ValueType  # 3
+"""Container not found reason"""
 UNSCHEDULABLE: DeploymentFailureReasonCode.ValueType  # 4
 """Unschedulable reason"""
 DOCKER_IMAGE_NOT_FOUND: DeploymentFailureReasonCode.ValueType  # 5
 """Docker image not found reason"""
 MEMORY_LIMIT_EXCEEDED: DeploymentFailureReasonCode.ValueType  # 6
 """Memory limit exceeded reason"""
 CRASH_LOOP: DeploymentFailureReasonCode.ValueType  # 7
 """Crash loop reason"""
 CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON: DeploymentFailureReasonCode.ValueType  # 8
 """Container fail to load for unknown reason"""
 global___DeploymentFailureReasonCode = DeploymentFailureReasonCode
 
-class ExtractorDeploymentBrief(google.protobuf.message.Message):
+class DeploymentUpdateRequestState(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DEPLOYMENT_ID_FIELD_NUMBER: builtins.int
-    STATUS_FIELD_NUMBER: builtins.int
-    DEPLOYED_BY_FIELD_NUMBER: builtins.int
-    FAILURE_REASON_CODE_FIELD_NUMBER: builtins.int
-    FAILURE_MESSAGE_FIELD_NUMBER: builtins.int
-    TECHNICAL_DETAILS_FIELD_NUMBER: builtins.int
-    DEPLOYMENT_TIMESTAMP_FIELD_NUMBER: builtins.int
-    EXTRACTOR_ID_FIELD_NUMBER: builtins.int
-    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
-    FEATURESET_ID_FIELD_NUMBER: builtins.int
-    deployment_id: builtins.str
-    """The id of the current deployment"""
-    status: global___ExtractorDeploymentStatus.ValueType
-    """The extractor deployment status"""
-    deployed_by: builtins.str
-    """The user id that did the deployment"""
-    failure_reason_code: builtins.str
-    """The failure reason code if deployment failed"""
-    failure_message: builtins.str
-    """User friendly message about the failure if deployment failed"""
-    technical_details: builtins.str
-    """Technical Details about the failure details."""
+    INVALID_REQUEST_TYPE_FIELD_NUMBER: builtins.int
+    UPDATE_REQUEST_TYPE_FIELD_NUMBER: builtins.int
+    UNDEPLOY_REQUEST_TYPE_FIELD_NUMBER: builtins.int
+    DEPLOYMENT_UPDATE_REQUEST_STATUS_FIELD_NUMBER: builtins.int
     @property
-    def deployment_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
-        """The deployment date"""
-    extractor_id: builtins.str
-    """the deployed extractor id"""
-    environment_id: builtins.str
-    """The extractor deployment environment id"""
-    featureset_id: builtins.str
-    """The extractor deployment featureset id"""
+    def invalid_request_type(self) -> global___DeploymentInvalidRequestType: ...
+    @property
+    def update_request_type(self) -> global___DeploymentUpdateRequestType: ...
+    @property
+    def undeploy_request_type(self) -> global___DeploymentUndeployRequestType: ...
+    deployment_update_request_status: global___DeploymentUpdateRequestStatus.ValueType
     def __init__(
         self,
         *,
-        deployment_id: builtins.str = ...,
-        status: global___ExtractorDeploymentStatus.ValueType = ...,
-        deployed_by: builtins.str = ...,
-        failure_reason_code: builtins.str = ...,
-        failure_message: builtins.str = ...,
-        technical_details: builtins.str = ...,
-        deployment_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
-        extractor_id: builtins.str = ...,
-        environment_id: builtins.str = ...,
-        featureset_id: builtins.str = ...,
+        invalid_request_type: global___DeploymentInvalidRequestType | None = ...,
+        update_request_type: global___DeploymentUpdateRequestType | None = ...,
+        undeploy_request_type: global___DeploymentUndeployRequestType | None = ...,
+        deployment_update_request_status: global___DeploymentUpdateRequestStatus.ValueType = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["invalid_request_type", b"invalid_request_type", "type", b"type", "undeploy_request_type", b"undeploy_request_type", "update_request_type", b"update_request_type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["deployment_update_request_status", b"deployment_update_request_status", "invalid_request_type", b"invalid_request_type", "type", b"type", "undeploy_request_type", b"undeploy_request_type", "update_request_type", b"update_request_type"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["invalid_request_type", "update_request_type", "undeploy_request_type"] | None: ...
+
+global___DeploymentUpdateRequestState = DeploymentUpdateRequestState
+
+class DeploymentInvalidRequestType(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___DeploymentInvalidRequestType = DeploymentInvalidRequestType
+
+class DeploymentUpdateRequestType(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___DeploymentUpdateRequestType = DeploymentUpdateRequestType
+
+class DeploymentUndeployRequestType(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___DeploymentUndeployRequestType = DeploymentUndeployRequestType
+
+class DeploymentState(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    EXTRACTOR_IDENTIFIER_FIELD_NUMBER: builtins.int
+    STATUS_DETAILS_FIELD_NUMBER: builtins.int
+    @property
+    def extractor_identifier(self) -> global___ExtractorDeploymentIdentifier: ...
+    @property
+    def status_details(self) -> global___DeploymentStatusDetails:
+        """Deployment status details of the current state"""
+    def __init__(
+        self,
+        *,
+        extractor_identifier: global___ExtractorDeploymentIdentifier | None = ...,
+        status_details: global___DeploymentStatusDetails | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["deployment_timestamp", b"deployment_timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["deployed_by", b"deployed_by", "deployment_id", b"deployment_id", "deployment_timestamp", b"deployment_timestamp", "environment_id", b"environment_id", "extractor_id", b"extractor_id", "failure_message", b"failure_message", "failure_reason_code", b"failure_reason_code", "featureset_id", b"featureset_id", "status", b"status", "technical_details", b"technical_details"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["extractor_identifier", b"extractor_identifier", "identifier_type", b"identifier_type", "status_details", b"status_details"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["extractor_identifier", b"extractor_identifier", "identifier_type", b"identifier_type", "status_details", b"status_details"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["identifier_type", b"identifier_type"]) -> typing_extensions.Literal["extractor_identifier"] | None: ...
 
-global___ExtractorDeploymentBrief = ExtractorDeploymentBrief
+global___DeploymentState = DeploymentState
 
-class KubernetesExtractorDeploymentState(google.protobuf.message.Message):
+class ExtractorDeploymentIdentifier(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EXTRACTOR_DEPLOYMENT_ID_FIELD_NUMBER: builtins.int
     EXTRACTOR_ID_FIELD_NUMBER: builtins.int
     FEATURESET_ID_FIELD_NUMBER: builtins.int
-    STATUS_FIELD_NUMBER: builtins.int
-    STATUS_DETAILS_FIELD_NUMBER: builtins.int
     extractor_deployment_id: builtins.str
     """The ID of the current deployment"""
     extractor_id: builtins.str
     """The ID of the extractor to deploy"""
     featureset_id: builtins.str
     """The ID of the featureset to which the extractor belongs"""
-    status: global___ExtractorDeploymentStatus.ValueType
-    """The extractor deployment status"""
-    @property
-    def status_details(self) -> global___StatusDetails:
-        """Status details of the Kubernetes current state"""
     def __init__(
         self,
         *,
         extractor_deployment_id: builtins.str = ...,
         extractor_id: builtins.str = ...,
         featureset_id: builtins.str = ...,
-        status: global___ExtractorDeploymentStatus.ValueType = ...,
-        status_details: global___StatusDetails | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["status_details", b"status_details"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["extractor_deployment_id", b"extractor_deployment_id", "extractor_id", b"extractor_id", "featureset_id", b"featureset_id", "status", b"status", "status_details", b"status_details"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["extractor_deployment_id", b"extractor_deployment_id", "extractor_id", b"extractor_id", "featureset_id", b"featureset_id"]) -> None: ...
 
-global___KubernetesExtractorDeploymentState = KubernetesExtractorDeploymentState
+global___ExtractorDeploymentIdentifier = ExtractorDeploymentIdentifier
 
-class StatusDetails(google.protobuf.message.Message):
+class DeploymentStatusDetails(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PENDING_STATUS_DETAILS_FIELD_NUMBER: builtins.int
-    SUCCESS_STATUS_DETAILS_FIELD_NUMBER: builtins.int
+    UPDATE_IN_PROGRESS_STATUS_DETAILS_FIELD_NUMBER: builtins.int
+    RUNNING_STATUS_DETAILS_FIELD_NUMBER: builtins.int
     FAILED_STATUS_DETAILS_FIELD_NUMBER: builtins.int
     @property
-    def pending_status_details(self) -> global___PendingStatusDetails:
-        """Detailed information about the Kubernetes, pending status"""
+    def update_in_progress_status_details(self) -> global___UpdateInProgressStatusDetails:
+        """Detailed information about the update in progress status"""
     @property
-    def success_status_details(self) -> global___SuccessfulStatusDetails:
-        """Detailed information about the Kubernetes successful status"""
+    def running_status_details(self) -> global___RunningStatusDetails:
+        """Detailed information about the active running deployment stats"""
     @property
     def failed_status_details(self) -> global___FailedStatusDetails:
-        """Detailed information about the Kubernetes failed status"""
+        """Detailed information about the failed deployment"""
     def __init__(
         self,
         *,
-        pending_status_details: global___PendingStatusDetails | None = ...,
-        success_status_details: global___SuccessfulStatusDetails | None = ...,
+        update_in_progress_status_details: global___UpdateInProgressStatusDetails | None = ...,
+        running_status_details: global___RunningStatusDetails | None = ...,
         failed_status_details: global___FailedStatusDetails | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["failed_status_details", b"failed_status_details", "pending_status_details", b"pending_status_details", "status_details", b"status_details", "success_status_details", b"success_status_details"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["failed_status_details", b"failed_status_details", "pending_status_details", b"pending_status_details", "status_details", b"status_details", "success_status_details", b"success_status_details"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["status_details", b"status_details"]) -> typing_extensions.Literal["pending_status_details", "success_status_details", "failed_status_details"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["failed_status_details", b"failed_status_details", "running_status_details", b"running_status_details", "status_details", b"status_details", "update_in_progress_status_details", b"update_in_progress_status_details"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["failed_status_details", b"failed_status_details", "running_status_details", b"running_status_details", "status_details", b"status_details", "update_in_progress_status_details", b"update_in_progress_status_details"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["status_details", b"status_details"]) -> typing_extensions.Literal["update_in_progress_status_details", "running_status_details", "failed_status_details"] | None: ...
 
-global___StatusDetails = StatusDetails
+global___DeploymentStatusDetails = DeploymentStatusDetails
 
-class PendingStatusDetails(google.protobuf.message.Message):
+class UpdateInProgressStatusDetails(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OLD_INSTANCE_FIELD_NUMBER: builtins.int
     NEW_INSTANCE_FIELD_NUMBER: builtins.int
     @property
     def old_instance(self) -> global___InstanceDetails:
-        """Detailed information about the Kubernetes old instance"""
+        """Detailed information about the old instance"""
     @property
     def new_instance(self) -> global___InstanceDetails:
-        """Detailed information about the Kubernetes new instance"""
+        """Detailed information about the new instance"""
     def __init__(
         self,
         *,
         old_instance: global___InstanceDetails | None = ...,
         new_instance: global___InstanceDetails | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["new_instance", b"new_instance", "old_instance", b"old_instance"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["new_instance", b"new_instance", "old_instance", b"old_instance"]) -> None: ...
 
-global___PendingStatusDetails = PendingStatusDetails
+global___UpdateInProgressStatusDetails = UpdateInProgressStatusDetails
 
-class SuccessfulStatusDetails(google.protobuf.message.Message):
+class RunningStatusDetails(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RUNNING_INSTANCE_FIELD_NUMBER: builtins.int
     @property
     def running_instance(self) -> global___InstanceDetails:
-        """Detailed information about the Kubernetes running instance"""
+        """Detailed information about the running instance"""
     def __init__(
         self,
         *,
         running_instance: global___InstanceDetails | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["running_instance", b"running_instance"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["running_instance", b"running_instance"]) -> None: ...
 
-global___SuccessfulStatusDetails = SuccessfulStatusDetails
+global___RunningStatusDetails = RunningStatusDetails
 
 class FailedStatusDetails(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FAILURE_DETAILS_FIELD_NUMBER: builtins.int
     OLD_INSTANCE_FIELD_NUMBER: builtins.int
     FAILED_INSTANCE_FIELD_NUMBER: builtins.int
     @property
     def failure_details(self) -> global___FailureDetails:
-        """Detailed information about the Kubernetes failure status"""
+        """Detailed information about the failure status"""
     @property
     def old_instance(self) -> global___InstanceDetails:
-        """Detailed information about the Kubernetes old instance"""
+        """Detailed information about the previous deployment instance"""
     @property
     def failed_instance(self) -> global___InstanceDetails:
-        """Detailed information about the Kubernetes failed instance"""
+        """Detailed information about the failed instance"""
     def __init__(
         self,
         *,
         failure_details: global___FailureDetails | None = ...,
         old_instance: global___InstanceDetails | None = ...,
         failed_instance: global___InstanceDetails | None = ...,
     ) -> None: ...
@@ -313,26 +341,39 @@
     def ClearField(self, field_name: typing_extensions.Literal["deployment_failure_reason_code", b"deployment_failure_reason_code", "failure_reason_details", b"failure_reason_details"]) -> None: ...
 
 global___FailureDetails = FailureDetails
 
 class InstanceDetails(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DEPLOYMENT_ID_FIELD_NUMBER: builtins.int
-    EXTRACTOR_ID_FIELD_NUMBER: builtins.int
+    EXTRACTOR_IDENTIFIER_FIELD_NUMBER: builtins.int
     AVAILABLE_REPLICAS_FIELD_NUMBER: builtins.int
-    deployment_id: builtins.str
-    """The deployment ID"""
-    extractor_id: builtins.str
-    """Build ID to deploy"""
+    @property
+    def extractor_identifier(self) -> global___ExtractorInstanceIdentifier: ...
     available_replicas: builtins.int
     """Available replicas"""
     def __init__(
         self,
         *,
-        deployment_id: builtins.str = ...,
-        extractor_id: builtins.str = ...,
+        extractor_identifier: global___ExtractorInstanceIdentifier | None = ...,
         available_replicas: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["available_replicas", b"available_replicas", "deployment_id", b"deployment_id", "extractor_id", b"extractor_id"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["extractor_identifier", b"extractor_identifier", "identifier_type", b"identifier_type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["available_replicas", b"available_replicas", "extractor_identifier", b"extractor_identifier", "identifier_type", b"identifier_type"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["identifier_type", b"identifier_type"]) -> typing_extensions.Literal["extractor_identifier"] | None: ...
 
 global___InstanceDetails = InstanceDetails
+
+class ExtractorInstanceIdentifier(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    EXTRACTOR_DEPLOYMENT_UPDATE_REQUEST_ID_FIELD_NUMBER: builtins.int
+    extractor_deployment_update_request_id: builtins.str
+    """The ID of the current deployment"""
+    def __init__(
+        self,
+        *,
+        extractor_deployment_update_request_id: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["extractor_deployment_update_request_id", b"extractor_deployment_update_request_id"]) -> None: ...
+
+global___ExtractorInstanceIdentifier = ExtractorInstanceIdentifier
```

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: qwak/feature_store/features/real_time_feature_extractor_deployment_service.proto
+# source: qwak/feature_store/features/deployment_service.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from _qwak_proto.qwak.feature_store.features import real_time_feature_extractor_deployment_pb2 as qwak_dot_feature__store_dot_features_dot_real__time__feature__extractor__deployment__pb2
+from _qwak_proto.qwak.feature_store.features import deployment_pb2 as qwak_dot_feature__store_dot_features_dot_deployment__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nPqwak/feature_store/features/real_time_feature_extractor_deployment_service.proto\x12\x1bqwak.feature.store.features\x1aHqwak/feature_store/features/real_time_feature_extractor_deployment.proto\"\x9a\x01\n%PushEnvironmentDeploymentStateRequest\x12\x16\n\x0e\x65nvironment_id\x18\x01 \x01(\t\x12Y\n\x10\x64\x65ployment_state\x18\x02 \x03(\x0b\x32?.qwak.feature.store.features.KubernetesExtractorDeploymentState\"(\n&PushEnvironmentDeploymentStateResponse2\xd2\x01\n$ExtractorDeploymentManagementService\x12\xa9\x01\n\x1ePushEnvironmentDeploymentState\x12\x42.qwak.feature.store.features.PushEnvironmentDeploymentStateRequest\x1a\x43.qwak.feature.store.features.PushEnvironmentDeploymentStateResponseB]\n(com.qwak.ai.feature.store.management.apiP\x01Z/qwak/featurestore/features;featurestorefeaturesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n4qwak/feature_store/features/deployment_service.proto\x12\x1bqwak.feature.store.features\x1a,qwak/feature_store/features/deployment.proto\"\x87\x01\n%PushEnvironmentDeploymentStateRequest\x12\x16\n\x0e\x65nvironment_id\x18\x01 \x01(\t\x12\x46\n\x10\x64\x65ployment_state\x18\x02 \x03(\x0b\x32,.qwak.feature.store.features.DeploymentState\"(\n&PushEnvironmentDeploymentStateResponse2\xc9\x01\n\x1b\x44\x65ploymentManagementService\x12\xa9\x01\n\x1ePushEnvironmentDeploymentState\x12\x42.qwak.feature.store.features.PushEnvironmentDeploymentStateRequest\x1a\x43.qwak.feature.store.features.PushEnvironmentDeploymentStateResponseB]\n(com.qwak.ai.feature.store.management.apiP\x01Z/qwak/featurestore/features;featurestorefeaturesb\x06proto3')
 
 
 
 _PUSHENVIRONMENTDEPLOYMENTSTATEREQUEST = DESCRIPTOR.message_types_by_name['PushEnvironmentDeploymentStateRequest']
 _PUSHENVIRONMENTDEPLOYMENTSTATERESPONSE = DESCRIPTOR.message_types_by_name['PushEnvironmentDeploymentStateResponse']
 PushEnvironmentDeploymentStateRequest = _reflection.GeneratedProtocolMessageType('PushEnvironmentDeploymentStateRequest', (_message.Message,), {
   'DESCRIPTOR' : _PUSHENVIRONMENTDEPLOYMENTSTATEREQUEST,
-  '__module__' : 'qwak.feature_store.features.real_time_feature_extractor_deployment_service_pb2'
+  '__module__' : 'qwak.feature_store.features.deployment_service_pb2'
   # @@protoc_insertion_point(class_scope:qwak.feature.store.features.PushEnvironmentDeploymentStateRequest)
   })
 _sym_db.RegisterMessage(PushEnvironmentDeploymentStateRequest)
 
 PushEnvironmentDeploymentStateResponse = _reflection.GeneratedProtocolMessageType('PushEnvironmentDeploymentStateResponse', (_message.Message,), {
   'DESCRIPTOR' : _PUSHENVIRONMENTDEPLOYMENTSTATERESPONSE,
-  '__module__' : 'qwak.feature_store.features.real_time_feature_extractor_deployment_service_pb2'
+  '__module__' : 'qwak.feature_store.features.deployment_service_pb2'
   # @@protoc_insertion_point(class_scope:qwak.feature.store.features.PushEnvironmentDeploymentStateResponse)
   })
 _sym_db.RegisterMessage(PushEnvironmentDeploymentStateResponse)
 
-_EXTRACTORDEPLOYMENTMANAGEMENTSERVICE = DESCRIPTOR.services_by_name['ExtractorDeploymentManagementService']
+_DEPLOYMENTMANAGEMENTSERVICE = DESCRIPTOR.services_by_name['DeploymentManagementService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n(com.qwak.ai.feature.store.management.apiP\001Z/qwak/featurestore/features;featurestorefeatures'
-  _PUSHENVIRONMENTDEPLOYMENTSTATEREQUEST._serialized_start=188
-  _PUSHENVIRONMENTDEPLOYMENTSTATEREQUEST._serialized_end=342
-  _PUSHENVIRONMENTDEPLOYMENTSTATERESPONSE._serialized_start=344
-  _PUSHENVIRONMENTDEPLOYMENTSTATERESPONSE._serialized_end=384
-  _EXTRACTORDEPLOYMENTMANAGEMENTSERVICE._serialized_start=387
-  _EXTRACTORDEPLOYMENTMANAGEMENTSERVICE._serialized_end=597
+  _PUSHENVIRONMENTDEPLOYMENTSTATEREQUEST._serialized_start=132
+  _PUSHENVIRONMENTDEPLOYMENTSTATEREQUEST._serialized_end=267
+  _PUSHENVIRONMENTDEPLOYMENTSTATERESPONSE._serialized_start=269
+  _PUSHENVIRONMENTDEPLOYMENTSTATERESPONSE._serialized_end=309
+  _DEPLOYMENTMANAGEMENTSERVICE._serialized_start=312
+  _DEPLOYMENTMANAGEMENTSERVICE._serialized_end=513
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 isort:skip_file
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import qwak.feature_store.features.real_time_feature_extractor_deployment_pb2
+import qwak.feature_store.features.deployment_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
@@ -20,20 +20,20 @@
 class PushEnvironmentDeploymentStateRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
     DEPLOYMENT_STATE_FIELD_NUMBER: builtins.int
     environment_id: builtins.str
     @property
-    def deployment_state(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[qwak.feature_store.features.real_time_feature_extractor_deployment_pb2.KubernetesExtractorDeploymentState]: ...
+    def deployment_state(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[qwak.feature_store.features.deployment_pb2.DeploymentState]: ...
     def __init__(
         self,
         *,
         environment_id: builtins.str = ...,
-        deployment_state: collections.abc.Iterable[qwak.feature_store.features.real_time_feature_extractor_deployment_pb2.KubernetesExtractorDeploymentState] | None = ...,
+        deployment_state: collections.abc.Iterable[qwak.feature_store.features.deployment_pb2.DeploymentState] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["deployment_state", b"deployment_state", "environment_id", b"environment_id"]) -> None: ...
 
 global___PushEnvironmentDeploymentStateRequest = PushEnvironmentDeploymentStateRequest
 
 class PushEnvironmentDeploymentStateResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from _qwak_proto.qwak.feature_store.features import execution_pb2 as qwak_dot_feature__store_dot_features_dot_execution__pb2
-from _qwak_proto.qwak.feature_store.features import real_time_feature_extractor_deployment_pb2 as qwak_dot_feature__store_dot_features_dot_real__time__feature__extractor__deployment__pb2
+from _qwak_proto.qwak.feature_store.features import deployment_pb2 as qwak_dot_feature__store_dot_features_dot_deployment__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n=qwak/feature_store/features/real_time_feature_extractor.proto\x12\x1bqwak.feature.store.features\x1a\x1fgoogle/protobuf/timestamp.proto\x1a+qwak/feature_store/features/execution.proto\x1aHqwak/feature_store/features/real_time_feature_extractor_deployment.proto\"\xdc\x01\n\x18RealTimeFeatureExtractor\x12o\n&real_time_feature_extractor_definition\x18\x01 \x01(\x0b\x32?.qwak.feature.store.features.RealTimeFeatureExtractorDefinition\x12O\n\x08metadata\x18\x02 \x01(\x0b\x32=.qwak.feature.store.features.RealTimeFeatureExtractorMetadata\"\x89\x02\n\"RealTimeFeatureExtractorDefinition\x12&\n\x1ereal_time_feature_extractor_id\x18\x01 \x01(\t\x12\x63\n real_time_feature_extractor_spec\x18\x02 \x01(\x0b\x32\x39.qwak.feature.store.features.RealTimeFeatureExtractorSpec\x12V\n\x16last_deployment_status\x18\x05 \x01(\x0e\x32\x36.qwak.feature.store.features.ExtractorDeploymentStatus\"\xc8\x01\n RealTimeFeatureExtractorMetadata\x12\x35\n\x11\x63reated_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x02 \x01(\t\x12?\n\x1blast_modification_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10last_modified_by\x18\x04 \x01(\t\"\xba\x02\n\x1cRealTimeFeatureExtractorSpec\x12K\n\x12real_time_artifact\x18\x01 \x01(\x0b\x32/.qwak.feature.store.features.ExtractionArtifact\x12P\n\x12\x64\x65pendency_manager\x18\x02 \x01(\x0b\x32\x34.qwak.feature.store.features.PythonDependencyManager\x12\\\n\x1c\x63lient_pod_compute_resources\x18\x03 \x01(\x0b\x32\x36.qwak.feature.store.features.ExtractorComputeResources\x12\x1d\n\x15max_staleness_seconds\x18\x04 \x01(\x03\"U\n\x12\x45xtractionArtifact\x12\x34\n\x06\x61ws_s3\x18\x01 \x01(\x0b\x32\".qwak.feature.store.features.AwsS3H\x00\x42\t\n\x07\x66s_type\"\x1e\n\x05\x41wsS3\x12\x15\n\rartifact_path\x18\x01 \x01(\t\"\x98\x02\n\x17PythonDependencyManager\x12\x42\n\x0epython_version\x18\x01 \x01(\x0e\x32*.qwak.feature.store.features.PythonVersion\x12\x45\n\nvirtualenv\x18\x02 \x01(\x0b\x32/.qwak.feature.store.features.VirtualEnvironmentH\x00\x12\x33\n\x05\x63onda\x18\x03 \x01(\x0b\x32\".qwak.feature.store.features.CondaH\x00\x12\x35\n\x06poetry\x18\x04 \x01(\x0b\x32#.qwak.feature.store.features.PoetryH\x00\x42\x06\n\x04type\"*\n\x05\x43onda\x12!\n\x19\x62\x61se64_encoded_conda_file\x18\x01 \x01(\t\"*\n\x06Poetry\x12 \n\x18\x62\x61se64_encoded_lock_file\x18\x01 \x01(\t\"=\n\x12VirtualEnvironment\x12\'\n\x1f\x62\x61se64_encoded_requirements_txt\x18\x01 \x01(\t\"\x9a\x01\n\x19\x45xtractorComputeResources\x12[\n\x19\x63ompute_resource_template\x18\x01 \x01(\x0e\x32\x36.qwak.feature.store.features.execution.ClusterTemplateH\x00\x12\x13\n\x0bparallelism\x18\x02 \x01(\x05\x42\x0b\n\tresources*s\n\rPythonVersion\x12\x1a\n\x16PYTHON_VERSION_INVALID\x10\x00\x12\x16\n\x12PYTHON_VERSION_3_7\x10\x01\x12\x16\n\x12PYTHON_VERSION_3_8\x10\x02\x12\x16\n\x12PYTHON_VERSION_3_9\x10\x03\x42[\n&com.qwak.ai.feature.store.features.apiP\x01Z/qwak/featurestore/features;featurestorefeaturesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n=qwak/feature_store/features/real_time_feature_extractor.proto\x12\x1bqwak.feature.store.features\x1a\x1fgoogle/protobuf/timestamp.proto\x1a+qwak/feature_store/features/execution.proto\x1a,qwak/feature_store/features/deployment.proto\"\xdc\x01\n\x18RealTimeFeatureExtractor\x12o\n&real_time_feature_extractor_definition\x18\x01 \x01(\x0b\x32?.qwak.feature.store.features.RealTimeFeatureExtractorDefinition\x12O\n\x08metadata\x18\x02 \x01(\x0b\x32=.qwak.feature.store.features.RealTimeFeatureExtractorMetadata\"\x80\x02\n\"RealTimeFeatureExtractorDefinition\x12&\n\x1ereal_time_feature_extractor_id\x18\x01 \x01(\t\x12\x63\n real_time_feature_extractor_spec\x18\x02 \x01(\x0b\x32\x39.qwak.feature.store.features.RealTimeFeatureExtractorSpec\x12M\n\x16last_deployment_status\x18\x05 \x01(\x0e\x32-.qwak.feature.store.features.DeploymentStatus\"\xc8\x01\n RealTimeFeatureExtractorMetadata\x12\x35\n\x11\x63reated_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x02 \x01(\t\x12?\n\x1blast_modification_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10last_modified_by\x18\x04 \x01(\t\"\xba\x02\n\x1cRealTimeFeatureExtractorSpec\x12K\n\x12real_time_artifact\x18\x01 \x01(\x0b\x32/.qwak.feature.store.features.ExtractionArtifact\x12P\n\x12\x64\x65pendency_manager\x18\x02 \x01(\x0b\x32\x34.qwak.feature.store.features.PythonDependencyManager\x12\\\n\x1c\x63lient_pod_compute_resources\x18\x03 \x01(\x0b\x32\x36.qwak.feature.store.features.ExtractorComputeResources\x12\x1d\n\x15max_staleness_seconds\x18\x04 \x01(\x03\"U\n\x12\x45xtractionArtifact\x12\x34\n\x06\x61ws_s3\x18\x01 \x01(\x0b\x32\".qwak.feature.store.features.AwsS3H\x00\x42\t\n\x07\x66s_type\"\x1e\n\x05\x41wsS3\x12\x15\n\rartifact_path\x18\x01 \x01(\t\"\x98\x02\n\x17PythonDependencyManager\x12\x42\n\x0epython_version\x18\x01 \x01(\x0e\x32*.qwak.feature.store.features.PythonVersion\x12\x45\n\nvirtualenv\x18\x02 \x01(\x0b\x32/.qwak.feature.store.features.VirtualEnvironmentH\x00\x12\x33\n\x05\x63onda\x18\x03 \x01(\x0b\x32\".qwak.feature.store.features.CondaH\x00\x12\x35\n\x06poetry\x18\x04 \x01(\x0b\x32#.qwak.feature.store.features.PoetryH\x00\x42\x06\n\x04type\"*\n\x05\x43onda\x12!\n\x19\x62\x61se64_encoded_conda_file\x18\x01 \x01(\t\"*\n\x06Poetry\x12 \n\x18\x62\x61se64_encoded_lock_file\x18\x01 \x01(\t\"=\n\x12VirtualEnvironment\x12\'\n\x1f\x62\x61se64_encoded_requirements_txt\x18\x01 \x01(\t\"\x9a\x01\n\x19\x45xtractorComputeResources\x12[\n\x19\x63ompute_resource_template\x18\x01 \x01(\x0e\x32\x36.qwak.feature.store.features.execution.ClusterTemplateH\x00\x12\x13\n\x0bparallelism\x18\x02 \x01(\x05\x42\x0b\n\tresources*s\n\rPythonVersion\x12\x1a\n\x16PYTHON_VERSION_INVALID\x10\x00\x12\x16\n\x12PYTHON_VERSION_3_7\x10\x01\x12\x16\n\x12PYTHON_VERSION_3_8\x10\x02\x12\x16\n\x12PYTHON_VERSION_3_9\x10\x03\x42[\n&com.qwak.ai.feature.store.features.apiP\x01Z/qwak/featurestore/features;featurestorefeaturesb\x06proto3')
 
 _PYTHONVERSION = DESCRIPTOR.enum_types_by_name['PythonVersion']
 PythonVersion = enum_type_wrapper.EnumTypeWrapper(_PYTHONVERSION)
 PYTHON_VERSION_INVALID = 0
 PYTHON_VERSION_3_7 = 1
 PYTHON_VERSION_3_8 = 2
 PYTHON_VERSION_3_9 = 3
@@ -116,32 +116,32 @@
   })
 _sym_db.RegisterMessage(ExtractorComputeResources)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n&com.qwak.ai.feature.store.features.apiP\001Z/qwak/featurestore/features;featurestorefeatures'
-  _PYTHONVERSION._serialized_start=1967
-  _PYTHONVERSION._serialized_end=2082
-  _REALTIMEFEATUREEXTRACTOR._serialized_start=247
-  _REALTIMEFEATUREEXTRACTOR._serialized_end=467
-  _REALTIMEFEATUREEXTRACTORDEFINITION._serialized_start=470
-  _REALTIMEFEATUREEXTRACTORDEFINITION._serialized_end=735
-  _REALTIMEFEATUREEXTRACTORMETADATA._serialized_start=738
-  _REALTIMEFEATUREEXTRACTORMETADATA._serialized_end=938
-  _REALTIMEFEATUREEXTRACTORSPEC._serialized_start=941
-  _REALTIMEFEATUREEXTRACTORSPEC._serialized_end=1255
-  _EXTRACTIONARTIFACT._serialized_start=1257
-  _EXTRACTIONARTIFACT._serialized_end=1342
-  _AWSS3._serialized_start=1344
-  _AWSS3._serialized_end=1374
-  _PYTHONDEPENDENCYMANAGER._serialized_start=1377
-  _PYTHONDEPENDENCYMANAGER._serialized_end=1657
-  _CONDA._serialized_start=1659
-  _CONDA._serialized_end=1701
-  _POETRY._serialized_start=1703
-  _POETRY._serialized_end=1745
-  _VIRTUALENVIRONMENT._serialized_start=1747
-  _VIRTUALENVIRONMENT._serialized_end=1808
-  _EXTRACTORCOMPUTERESOURCES._serialized_start=1811
-  _EXTRACTORCOMPUTERESOURCES._serialized_end=1965
+  _PYTHONVERSION._serialized_start=1930
+  _PYTHONVERSION._serialized_end=2045
+  _REALTIMEFEATUREEXTRACTOR._serialized_start=219
+  _REALTIMEFEATUREEXTRACTOR._serialized_end=439
+  _REALTIMEFEATUREEXTRACTORDEFINITION._serialized_start=442
+  _REALTIMEFEATUREEXTRACTORDEFINITION._serialized_end=698
+  _REALTIMEFEATUREEXTRACTORMETADATA._serialized_start=701
+  _REALTIMEFEATUREEXTRACTORMETADATA._serialized_end=901
+  _REALTIMEFEATUREEXTRACTORSPEC._serialized_start=904
+  _REALTIMEFEATUREEXTRACTORSPEC._serialized_end=1218
+  _EXTRACTIONARTIFACT._serialized_start=1220
+  _EXTRACTIONARTIFACT._serialized_end=1305
+  _AWSS3._serialized_start=1307
+  _AWSS3._serialized_end=1337
+  _PYTHONDEPENDENCYMANAGER._serialized_start=1340
+  _PYTHONDEPENDENCYMANAGER._serialized_end=1620
+  _CONDA._serialized_start=1622
+  _CONDA._serialized_end=1664
+  _POETRY._serialized_start=1666
+  _POETRY._serialized_end=1708
+  _VIRTUALENVIRONMENT._serialized_start=1710
+  _VIRTUALENVIRONMENT._serialized_end=1771
+  _EXTRACTORCOMPUTERESOURCES._serialized_start=1774
+  _EXTRACTORCOMPUTERESOURCES._serialized_end=1928
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
+import qwak.feature_store.features.deployment_pb2
 import qwak.feature_store.features.execution_pb2
-import qwak.feature_store.features.real_time_feature_extractor_deployment_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
@@ -67,22 +67,22 @@
     REAL_TIME_FEATURE_EXTRACTOR_SPEC_FIELD_NUMBER: builtins.int
     LAST_DEPLOYMENT_STATUS_FIELD_NUMBER: builtins.int
     real_time_feature_extractor_id: builtins.str
     """Assigned unique id of the real time extractor"""
     @property
     def real_time_feature_extractor_spec(self) -> global___RealTimeFeatureExtractorSpec:
         """Specifications of the real time extractor"""
-    last_deployment_status: qwak.feature_store.features.real_time_feature_extractor_deployment_pb2.ExtractorDeploymentStatus.ValueType
+    last_deployment_status: qwak.feature_store.features.deployment_pb2.DeploymentStatus.ValueType
     """Last deployment status of the real time extractor"""
     def __init__(
         self,
         *,
         real_time_feature_extractor_id: builtins.str = ...,
         real_time_feature_extractor_spec: global___RealTimeFeatureExtractorSpec | None = ...,
-        last_deployment_status: qwak.feature_store.features.real_time_feature_extractor_deployment_pb2.ExtractorDeploymentStatus.ValueType = ...,
+        last_deployment_status: qwak.feature_store.features.deployment_pb2.DeploymentStatus.ValueType = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["real_time_feature_extractor_spec", b"real_time_feature_extractor_spec"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["last_deployment_status", b"last_deployment_status", "real_time_feature_extractor_id", b"real_time_feature_extractor_id", "real_time_feature_extractor_spec", b"real_time_feature_extractor_spec"]) -> None: ...
 
 global___RealTimeFeatureExtractorDefinition = RealTimeFeatureExtractorDefinition
 
 class RealTimeFeatureExtractorMetadata(google.protobuf.message.Message):
```

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.99/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.99/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.99/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/pyproject.toml` & `qwak_core-0.0.99/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.98"
+version = "0.0.99"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.98/qwak/automations/__init__.py` & `qwak_core-0.0.99/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/automations/automation_executions.py` & `qwak_core-0.0.99/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/automations/automations.py` & `qwak_core-0.0.99/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.99/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.99/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/automations/common.py` & `qwak_core-0.0.99/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.99/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.99/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.99/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.99/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.99/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/alert_management/client.py` & `qwak_core-0.0.99/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/analytics/client.py` & `qwak_core-0.0.99/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/audience/client.py` & `qwak_core-0.0.99/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/automation_management/client.py` & `qwak_core-0.0.99/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.99/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.99/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.99/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.99/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/build_management/client.py` & `qwak_core-0.0.99/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.99/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.99/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/deployment/client.py` & `qwak_core-0.0.99/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.99/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.99/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.99/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.99/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/instance_template/client.py` & `qwak_core-0.0.99/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.99/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/logging_client/client.py` & `qwak_core-0.0.99/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/model_management/client.py` & `qwak_core-0.0.99/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/project/client.py` & `qwak_core-0.0.99/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/secret_service/client.py` & `qwak_core-0.0.99/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.99/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.99/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.99/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.99/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.99/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.99/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.99/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.99/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.99/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.99/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.99/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.99/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.99/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.99/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.99/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/offline/client.py` & `qwak_core-0.0.99/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/feature_store/online/client.py` & `qwak_core-0.0.99/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/inner/const.py` & `qwak_core-0.0.99/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.99/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.99/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.99/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.99/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/inner/singleton_meta.py` & `qwak_core-0.0.99/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/inner/tool/auth.py` & `qwak_core-0.0.99/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.99/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.99/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.99/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.99/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/adapters/__init__.py` & `qwak_core-0.0.99/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.99/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.99/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.99/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.99/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.99/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/base.py` & `qwak_core-0.0.99/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/decorators/api.py` & `qwak_core-0.0.99/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.99/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/experiment_tracking.py` & `qwak_core-0.0.99/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/schema.py` & `qwak_core-0.0.99/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/schema_entities.py` & `qwak_core-0.0.99/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.99/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.99/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.99/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.99/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.99/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.99/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.99/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.99/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.99/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.99/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.99/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.99/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.99/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.99/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.99/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.99/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.99/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.99/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.99/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/qwak_client/client.py` & `qwak_core-0.0.99/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.99/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/qwak_client/models/model.py` & `qwak_core-0.0.99/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.99/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.99/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/tools/logger/logger.py` & `qwak_core-0.0.99/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak/tools/logger/logging.yml` & `qwak_core-0.0.99/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.99/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/qwak_services_mock/services_mock.py` & `qwak_core-0.0.99/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.98/setup.py` & `qwak_core-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.98',
+    'version': '0.0.99',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.98/PKG-INFO` & `qwak_core-0.0.99/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.98
+Version: 0.0.99
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

