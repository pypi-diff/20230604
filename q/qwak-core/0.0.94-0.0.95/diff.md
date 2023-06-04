# Comparing `tmp/qwak_core-0.0.94.tar.gz` & `tmp/qwak_core-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.94.tar", max compression
+gzip compressed data, was "qwak_core-0.0.95.tar", max compression
```

## Comparing `qwak_core-0.0.94.tar` & `qwak_core-0.0.95.tar`

### file list

```diff
@@ -1,588 +1,588 @@
--rw-r--r--   0        0        0      264 2023-06-04 14:33:29.196169 qwak_core-0.0.94/README.md
--rw-r--r--   0        0        0        0 2023-06-04 14:35:11.845088 qwak_core-0.0.94/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-06-04 14:35:11.869089 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-06-04 14:34:51.600919 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.869089 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-06-04 14:35:11.865089 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-06-04 14:34:51.236916 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.865089 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-06-04 14:35:11.865089 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-06-04 14:34:51.424918 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.865089 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-06-04 14:35:11.857088 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-06-04 14:34:50.712912 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-06-04 14:35:11.857088 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-06-04 14:35:11.861089 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-06-04 14:34:50.884913 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.861089 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4901 2023-06-04 14:35:11.861089 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5995 2023-06-04 14:34:51.060915 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.861089 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-06-04 14:35:11.845088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-06-04 14:34:50.532910 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-06-04 14:35:11.845088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5707 2023-06-04 14:35:11.849089 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8170 2023-06-04 14:34:51.780920 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.849089 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-06-04 14:35:11.853088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-06-04 14:34:52.132923 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.853088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-06-04 14:35:11.853088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-06-04 14:34:52.308925 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-06-04 14:35:11.853088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-06-04 14:35:11.849089 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-06-04 14:34:51.956922 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.849089 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-06-04 14:35:11.857088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-06-04 14:34:52.492926 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.857088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-06-04 14:35:11.897089 qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-06-04 14:34:54.972947 qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.897089 qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-06-04 14:35:11.897089 qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-06-04 14:34:55.152948 qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-06-04 14:35:11.897089 qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-06-04 14:35:11.965089 qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-06-04 14:35:00.584994 qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.969089 qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-06-04 14:35:11.969089 qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-06-04 14:35:00.768995 qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-06-04 14:35:11.969089 qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-06-04 14:35:11.973089 qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-06-04 14:35:01.705003 qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-06-04 14:35:11.973089 qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-06-04 14:35:11.969089 qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-06-04 14:35:01.525002 qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.973089 qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-06-04 14:35:11.973089 qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-06-04 14:35:01.881005 qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.977089 qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-06-04 14:35:11.977089 qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-06-04 14:35:02.057006 qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-06-04 14:35:11.977089 qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-06-04 14:35:12.061090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-06-04 14:35:09.625070 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.061090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-06-04 14:35:12.057090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-06-04 14:35:09.265067 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.057090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-06-04 14:35:12.061090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-06-04 14:35:09.441069 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.061090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-06-04 14:35:12.053090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-06-04 14:35:08.905064 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-06-04 14:35:12.053090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-06-04 14:35:12.057090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-06-04 14:35:09.089066 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.057090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-06-04 14:35:12.069090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-06-04 14:35:10.153075 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.069090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-06-04 14:35:12.065090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-06-04 14:35:09.981073 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.065090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-06-04 14:35:12.065090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-06-04 14:35:09.801072 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.065090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-06-04 14:35:12.053090 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-06-04 14:35:08.721063 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.053090 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-06-04 14:35:12.049090 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-06-04 14:35:08.353060 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.049090 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-06-04 14:35:12.049090 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-06-04 14:35:08.541061 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-06-04 14:35:12.049090 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    20255 2023-06-04 14:35:12.001089 qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    17495 2023-06-04 14:35:03.861022 qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    20359 2023-06-04 14:35:12.001089 qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-06-04 14:35:11.997089 qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-06-04 14:35:03.677020 qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.001089 qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11691 2023-06-04 14:35:11.989089 qwak_core-0.0.94/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18850 2023-06-04 14:35:03.325017 qwak_core-0.0.94/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.993089 qwak_core-0.0.94/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-06-04 14:35:11.993089 qwak_core-0.0.94/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-06-04 14:35:03.497018 qwak_core-0.0.94/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.993089 qwak_core-0.0.94/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-06-04 14:35:11.993089 qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-06-04 14:35:04.037023 qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-06-04 14:35:11.997089 qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38290 2023-06-04 14:35:11.997089 qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52702 2023-06-04 14:35:04.429026 qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-06-04 14:35:11.997089 qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-06-04 14:35:12.009090 qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-06-04 14:35:04.801030 qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.009090 qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-06-04 14:35:12.009090 qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-06-04 14:35:04.977031 qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-06-04 14:35:12.009090 qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-06-04 14:35:11.985089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-06-04 14:35:02.793012 qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.985089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-06-04 14:35:11.985089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-06-04 14:35:02.969014 qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-06-04 14:35:11.989089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-06-04 14:35:11.981089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-06-04 14:35:02.429009 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.981089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-06-04 14:35:11.977089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-06-04 14:35:02.245008 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.981089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-06-04 14:35:11.981089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-06-04 14:35:02.617011 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-06-04 14:35:11.985089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-06-04 14:35:11.885089 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-06-04 14:34:54.084939 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.885089 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-06-04 14:35:11.889089 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-06-04 14:34:54.260941 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.889089 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-06-04 14:35:11.889089 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-06-04 14:34:54.444942 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-06-04 14:35:11.889089 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-06-04 14:35:11.949089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-06-04 14:34:59.528985 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.949089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-06-04 14:35:11.945089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-06-04 14:34:59.348983 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-06-04 14:35:11.945089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2023-06-04 14:35:11.925089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2023-06-04 14:34:57.408967 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.925089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2023-06-04 14:35:11.921089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2023-06-04 14:34:57.232965 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.921089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-06-04 14:35:11.917089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-06-04 14:34:56.684961 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.917089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-06-04 14:35:11.921089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-06-04 14:34:57.056964 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-06-04 14:35:11.921089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-06-04 14:35:11.925089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-06-04 14:34:57.584968 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.925089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-06-04 14:35:11.929089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-06-04 14:34:57.760970 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-06-04 14:35:11.929089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25269 2023-06-04 14:35:11.917089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37664 2023-06-04 14:34:56.868962 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.917089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-06-04 14:35:11.929089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-06-04 14:34:57.932971 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.929089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    10202 2023-06-04 14:35:11.933089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py
--rw-r--r--   0        0        0    16565 2023-06-04 14:34:58.284974 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.933089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2_grpc.py
--rw-r--r--   0        0        0     3559 2023-06-04 14:35:11.937089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py
--rw-r--r--   0        0        0     1759 2023-06-04 14:34:58.460976 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi
--rw-r--r--   0        0        0     3608 2023-06-04 14:35:11.937089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0    10604 2023-06-04 14:35:11.933089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    13410 2023-06-04 14:34:58.108973 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.933089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-06-04 14:35:11.949089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-06-04 14:35:11.409085 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.949089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-06-04 14:35:11.953089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-06-04 14:35:11.593087 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-06-04 14:35:11.953089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-06-04 14:35:11.953089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-06-04 14:35:00.056989 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.953089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-06-04 14:35:11.957089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-06-04 14:35:00.232991 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-06-04 14:35:11.957089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-06-04 14:35:11.957089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-06-04 14:35:00.408992 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.961089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-06-04 14:35:11.961089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-06-04 14:35:01.132998 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.965089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-06-04 14:35:11.961089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-06-04 14:35:00.948997 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-06-04 14:35:11.961089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-06-04 14:35:11.965089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-06-04 14:35:01.345000 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.965089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-06-04 14:35:11.937089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-06-04 14:34:58.640977 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.937089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-06-04 14:35:11.941089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-06-04 14:34:58.816979 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.941089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-06-04 14:35:11.941089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-06-04 14:34:58.996980 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-06-04 14:35:11.941089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-06-04 14:35:11.945089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-06-04 14:34:59.172982 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.945089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-06-04 14:35:12.069090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-06-04 14:35:10.329076 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.069090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-06-04 14:35:12.073090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-06-04 14:35:10.505078 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-06-04 14:35:12.073090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-06-04 14:35:12.073090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-06-04 14:35:10.681079 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.073090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-06-04 14:35:12.077090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-06-04 14:35:10.865081 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-06-04 14:35:12.077090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-06-04 14:35:12.077090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-06-04 14:35:11.049082 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-06-04 14:35:12.081090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-06-04 14:35:12.081090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-06-04 14:35:11.225084 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.081090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-06-04 14:35:12.013090 qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-06-04 14:35:05.153032 qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.013090 qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-06-04 14:35:12.013090 qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-06-04 14:35:05.325034 qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-06-04 14:35:12.013090 qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-06-04 14:35:11.901089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-06-04 14:34:55.964955 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.905089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-06-04 14:35:11.905089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-06-04 14:34:56.140956 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.905089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-06-04 14:35:11.909089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-06-04 14:34:56.324958 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-06-04 14:35:11.909089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-06-04 14:35:11.913089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-06-04 14:34:56.500959 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.913089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-06-04 14:35:11.989089 qwak_core-0.0.94/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-06-04 14:35:03.145015 qwak_core-0.0.94/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-06-04 14:35:11.989089 qwak_core-0.0.94/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-06-04 14:35:12.017089 qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-06-04 14:35:05.501035 qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.017089 qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-06-04 14:35:12.017089 qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-06-04 14:35:05.677037 qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-06-04 14:35:12.017089 qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-06-04 14:35:12.029090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-06-04 14:35:06.733046 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.029090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-06-04 14:35:12.033090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-06-04 14:35:06.917047 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.033090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-06-04 14:35:12.033090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-06-04 14:35:07.097049 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.033090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-06-04 14:35:12.037090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-06-04 14:35:07.277050 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.037090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-06-04 14:35:12.037090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-06-04 14:35:07.457052 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.037090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-06-04 14:35:12.041090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-06-04 14:35:07.653054 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-06-04 14:35:12.041090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-06-04 14:35:12.041090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-06-04 14:35:07.829055 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.041090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-06-04 14:35:12.021090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-06-04 14:35:06.029040 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.021090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-06-04 14:35:12.029090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-06-04 14:35:06.557044 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.029090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-06-04 14:35:12.025090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-06-04 14:35:06.205041 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-06-04 14:35:12.025090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-06-04 14:35:12.025090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-06-04 14:35:06.385043 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.025090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-06-04 14:35:12.005089 qwak_core-0.0.94/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-06-04 14:35:04.625028 qwak_core-0.0.94/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-06-04 14:35:12.005089 qwak_core-0.0.94/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-06-04 14:35:11.881089 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-06-04 14:34:55.564951 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-06-04 14:35:11.881089 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-06-04 14:35:11.881089 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-06-04 14:34:55.352949 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.881089 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-06-04 14:35:11.885089 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-06-04 14:34:55.780953 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-06-04 14:35:11.885089 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-06-04 14:35:12.001089 qwak_core-0.0.94/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-06-04 14:35:04.233025 qwak_core-0.0.94/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-06-04 14:35:12.005089 qwak_core-0.0.94/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-06-04 14:35:12.021090 qwak_core-0.0.94/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-06-04 14:35:05.853038 qwak_core-0.0.94/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-06-04 14:35:12.021090 qwak_core-0.0.94/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-06-04 14:35:11.877089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-06-04 14:34:53.372933 qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.877089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-06-04 14:35:11.877089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-06-04 14:34:53.196932 qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-06-04 14:35:11.877089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-06-04 14:35:11.869089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-06-04 14:34:52.664928 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.869089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-06-04 14:35:11.873089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-06-04 14:34:52.840929 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.873089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-06-04 14:35:11.873089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-06-04 14:34:53.016930 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-06-04 14:35:11.873089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-06-04 14:35:12.045090 qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-06-04 14:35:08.181058 qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-06-04 14:35:12.045090 qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-06-04 14:35:12.045090 qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-06-04 14:35:08.005056 qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:12.045090 qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    10961 2023-06-04 14:35:11.893089 qwak_core-0.0.94/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    14256 2023-06-04 14:34:54.620944 qwak_core-0.0.94/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.893089 qwak_core-0.0.94/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3072 2023-06-04 14:35:11.893089 qwak_core-0.0.94/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2663 2023-06-04 14:34:54.796945 qwak_core-0.0.94/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 14:35:11.893089 qwak_core-0.0.94/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-06-04 14:35:13.161097 qwak_core-0.0.94/pyproject.toml
--rw-r--r--   0        0        0      447 2023-06-04 14:35:13.161097 qwak_core-0.0.94/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    15319 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.94/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.94/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-06-04 15:02:32.049421 qwak_core-0.0.95/README.md
+-rw-r--r--   0        0        0        0 2023-06-04 15:04:11.250141 qwak_core-0.0.95/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-06-04 15:04:11.270141 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-06-04 15:03:51.562003 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.270141 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-06-04 15:04:11.266141 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-06-04 15:03:51.222000 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.270141 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-06-04 15:04:11.270141 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-06-04 15:03:51.390001 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.270141 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-06-04 15:04:11.262141 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-06-04 15:03:50.705996 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-06-04 15:04:11.262141 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-06-04 15:04:11.262141 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-06-04 15:03:50.881997 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.266141 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4901 2023-06-04 15:04:11.266141 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5995 2023-06-04 15:03:51.049999 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.266141 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-06-04 15:04:11.250141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-06-04 15:03:50.537995 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-06-04 15:04:11.250141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5707 2023-06-04 15:04:11.250141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8170 2023-06-04 15:03:51.734004 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.254140 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-06-04 15:04:11.254140 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-06-04 15:03:52.070007 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.258141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-06-04 15:04:11.258141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-06-04 15:03:52.242008 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-06-04 15:04:11.258141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-06-04 15:04:11.254140 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-06-04 15:03:51.898005 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.254140 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-06-04 15:04:11.258141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-06-04 15:03:52.414009 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.262141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-06-04 15:04:11.298141 qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-06-04 15:03:54.830027 qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.298141 qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-06-04 15:04:11.298141 qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-06-04 15:03:55.010028 qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-06-04 15:04:11.302141 qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-06-04 15:04:11.370141 qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-06-04 15:04:00.370066 qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.370141 qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-06-04 15:04:11.370141 qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-06-04 15:04:00.546067 qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-06-04 15:04:11.370141 qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-06-04 15:04:11.374141 qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-06-04 15:04:01.422073 qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-06-04 15:04:11.374141 qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-06-04 15:04:11.374141 qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-06-04 15:04:01.246071 qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.374141 qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-06-04 15:04:11.378141 qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-06-04 15:04:01.590074 qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.378141 qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-06-04 15:04:11.378141 qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-06-04 15:04:01.758075 qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-06-04 15:04:11.378141 qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-06-04 15:04:11.462142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-06-04 15:04:09.078126 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.462142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-06-04 15:04:11.458142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-06-04 15:04:08.734123 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.458142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-06-04 15:04:11.458142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-06-04 15:04:08.902124 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.462142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-06-04 15:04:11.454142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-06-04 15:04:08.382121 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-06-04 15:04:11.454142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-06-04 15:04:11.454142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-06-04 15:04:08.562122 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.458142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-06-04 15:04:11.466142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-06-04 15:04:09.590129 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.466142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-06-04 15:04:11.466142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-06-04 15:04:09.418128 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.466142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-06-04 15:04:11.462142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-06-04 15:04:09.250127 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.466142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10989 2023-06-04 15:04:11.450142 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    15193 2023-06-04 15:04:08.202119 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.454142 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-06-04 15:04:11.446142 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-06-04 15:04:07.850117 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.450142 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    44118 2023-06-04 15:04:11.450142 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    58036 2023-06-04 15:04:08.030118 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-06-04 15:04:11.450142 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20255 2023-06-04 15:04:11.402142 qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    17495 2023-06-04 15:04:03.514087 qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-06-04 15:04:11.402142 qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-06-04 15:04:11.402142 qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-06-04 15:04:03.342086 qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.402142 qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11691 2023-06-04 15:04:11.394142 qwak_core-0.0.95/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18850 2023-06-04 15:04:02.998084 qwak_core-0.0.95/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.394142 qwak_core-0.0.95/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-06-04 15:04:11.394142 qwak_core-0.0.95/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-06-04 15:04:03.166085 qwak_core-0.0.95/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.394142 qwak_core-0.0.95/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-06-04 15:04:11.394142 qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-06-04 15:04:03.690088 qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-06-04 15:04:11.398141 qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38290 2023-06-04 15:04:11.398141 qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52702 2023-06-04 15:04:04.062091 qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-06-04 15:04:11.398141 qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-06-04 15:04:11.410142 qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-06-04 15:04:04.418093 qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.410142 qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-06-04 15:04:11.410142 qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-06-04 15:04:04.586094 qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-06-04 15:04:11.410142 qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-06-04 15:04:11.386141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-06-04 15:04:02.474080 qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.386141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-06-04 15:04:11.390142 qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-06-04 15:04:02.646081 qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-06-04 15:04:11.390142 qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-06-04 15:04:11.382141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-06-04 15:04:02.122078 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.382141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-06-04 15:04:11.382141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-06-04 15:04:01.946076 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.382141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-06-04 15:04:11.386141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-06-04 15:04:02.306079 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-06-04 15:04:11.386141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-06-04 15:04:11.290141 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-06-04 15:03:53.962021 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.290141 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-06-04 15:04:11.290141 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-06-04 15:03:54.134022 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.290141 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-06-04 15:04:11.294141 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-06-04 15:03:54.314024 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-06-04 15:04:11.294141 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-06-04 15:04:11.350141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-06-04 15:03:59.322058 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.350141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-06-04 15:04:11.350141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-06-04 15:03:59.150057 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-06-04 15:04:11.350141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2023-06-04 15:04:11.326141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2023-06-04 15:03:57.230044 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.326141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2023-06-04 15:04:11.322141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2023-06-04 15:03:57.054043 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.326141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-06-04 15:04:11.318141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-06-04 15:03:56.514039 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.318141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-06-04 15:04:11.322141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-06-04 15:03:56.882041 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-06-04 15:04:11.322141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-06-04 15:04:11.326141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-06-04 15:03:57.406045 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.330141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-06-04 15:04:11.330141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-06-04 15:03:57.578046 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-06-04 15:04:11.330141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25269 2023-06-04 15:04:11.318141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37664 2023-06-04 15:03:56.694040 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.322141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-06-04 15:04:11.330141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-06-04 15:03:57.746047 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.334141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    10202 2023-06-04 15:04:11.334141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py
+-rw-r--r--   0        0        0    16565 2023-06-04 15:03:58.098050 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.338141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     3559 2023-06-04 15:04:11.338141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py
+-rw-r--r--   0        0        0     1759 2023-06-04 15:03:58.274051 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi
+-rw-r--r--   0        0        0     3608 2023-06-04 15:04:11.338141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10604 2023-06-04 15:04:11.334141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    13410 2023-06-04 15:03:57.922049 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.334141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-06-04 15:04:11.354141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-06-04 15:04:10.822138 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.354141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-06-04 15:04:11.354141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-06-04 15:04:10.998139 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-06-04 15:04:11.354141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-06-04 15:04:11.358141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-06-04 15:03:59.850062 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.358141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-06-04 15:04:11.358141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-06-04 15:04:00.026063 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-06-04 15:04:11.358141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-06-04 15:04:11.362141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-06-04 15:04:00.198064 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.362141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-06-04 15:04:11.366141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-06-04 15:04:00.902069 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.366141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-06-04 15:04:11.362141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-06-04 15:04:00.722068 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-06-04 15:04:11.362141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-06-04 15:04:11.366141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-06-04 15:04:01.074070 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.366141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-06-04 15:04:11.342141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-06-04 15:03:58.450052 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.342141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-06-04 15:04:11.342141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-06-04 15:03:58.622053 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.342141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-06-04 15:04:11.346141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-06-04 15:03:58.798055 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-06-04 15:04:11.346141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-06-04 15:04:11.346141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-06-04 15:03:58.974056 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.346141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-06-04 15:04:11.470142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-06-04 15:04:09.758130 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.470142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-06-04 15:04:11.470142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-06-04 15:04:09.946132 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-06-04 15:04:11.470142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-06-04 15:04:11.474142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-06-04 15:04:10.114133 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.474142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-06-04 15:04:11.474142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-06-04 15:04:10.298134 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-06-04 15:04:11.474142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-06-04 15:04:11.478142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-06-04 15:04:10.478135 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-06-04 15:04:11.478142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-06-04 15:04:11.478142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-06-04 15:04:10.650136 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.478142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-06-04 15:04:11.414142 qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-06-04 15:04:04.754096 qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.414142 qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-06-04 15:04:11.414142 qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-06-04 15:04:04.922097 qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-06-04 15:04:11.414142 qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-06-04 15:04:11.302141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-06-04 15:03:55.810034 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.306141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-06-04 15:04:11.306141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-06-04 15:03:55.982035 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.310141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-06-04 15:04:11.310141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-06-04 15:03:56.158036 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-06-04 15:04:11.314141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-06-04 15:04:11.314141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-06-04 15:03:56.330037 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.318141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-06-04 15:04:11.390142 qwak_core-0.0.95/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-06-04 15:04:02.822082 qwak_core-0.0.95/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-06-04 15:04:11.390142 qwak_core-0.0.95/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-06-04 15:04:11.414142 qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-06-04 15:04:05.094098 qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.418142 qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-06-04 15:04:11.418142 qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-06-04 15:04:05.262099 qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-06-04 15:04:11.418142 qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-06-04 15:04:11.430142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-06-04 15:04:06.286106 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.430142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-06-04 15:04:11.430142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-06-04 15:04:06.454107 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.434142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-06-04 15:04:11.434142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-06-04 15:04:06.630109 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.434142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-06-04 15:04:11.434142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-06-04 15:04:06.802110 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.438142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-06-04 15:04:11.438142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-06-04 15:04:06.982111 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.438142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-06-04 15:04:11.438142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-06-04 15:04:07.170112 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-06-04 15:04:11.442142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-06-04 15:04:11.442142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-06-04 15:04:07.342114 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.442142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-06-04 15:04:11.422142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-06-04 15:04:05.602102 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.422142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-06-04 15:04:11.426142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-06-04 15:04:06.114105 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.430142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-06-04 15:04:11.422142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-06-04 15:04:05.770103 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-06-04 15:04:11.426142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-06-04 15:04:11.426142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-06-04 15:04:05.942104 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.426142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-06-04 15:04:11.406142 qwak_core-0.0.95/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-06-04 15:04:04.250092 qwak_core-0.0.95/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-06-04 15:04:11.406142 qwak_core-0.0.95/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-06-04 15:04:11.286141 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-06-04 15:03:55.418031 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-06-04 15:04:11.286141 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-06-04 15:04:11.282141 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-06-04 15:03:55.206030 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.282141 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-06-04 15:04:11.286141 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-06-04 15:03:55.626033 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-06-04 15:04:11.286141 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-06-04 15:04:11.406142 qwak_core-0.0.95/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-06-04 15:04:03.874090 qwak_core-0.0.95/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-06-04 15:04:11.406142 qwak_core-0.0.95/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-06-04 15:04:11.418142 qwak_core-0.0.95/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-06-04 15:04:05.434100 qwak_core-0.0.95/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-06-04 15:04:11.422142 qwak_core-0.0.95/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-06-04 15:04:11.282141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-06-04 15:03:53.278016 qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.282141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-06-04 15:04:11.278141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-06-04 15:03:53.106015 qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-06-04 15:04:11.278141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-06-04 15:04:11.274141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-06-04 15:03:52.582011 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.274141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-06-04 15:04:11.274141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-06-04 15:03:52.758012 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.274141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-06-04 15:04:11.278141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-06-04 15:03:52.930014 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-06-04 15:04:11.278141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-06-04 15:04:11.446142 qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-06-04 15:04:07.682116 qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-06-04 15:04:11.446142 qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-06-04 15:04:11.442142 qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-06-04 15:04:07.510115 qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.446142 qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    10961 2023-06-04 15:04:11.294141 qwak_core-0.0.95/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    14256 2023-06-04 15:03:54.486025 qwak_core-0.0.95/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.294141 qwak_core-0.0.95/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3072 2023-06-04 15:04:11.298141 qwak_core-0.0.95/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2663 2023-06-04 15:03:54.658026 qwak_core-0.0.95/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 15:04:11.298141 qwak_core-0.0.95/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-06-04 15:04:12.946152 qwak_core-0.0.95/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-06-04 15:04:12.946152 qwak_core-0.0.95/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    15319 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.95/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.95/PKG-INFO
```

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from _qwak_proto.qwak.user_application.common.v0 import resources_pb2 as qwak_dot_user__application_dot_common_dot_v0_dot_resources__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(qwak/batch_job/v1/batch_job_events.proto\x12\rqwak.batchjob\x1a/qwak/user_application/common/v0/resources.proto\"\xa5\x01\n\x14\x42\x61tchJobEventMessage\x12\x45\n\x14\x62\x61tch_job_event_type\x18\x01 \x01(\x0e\x32\'.qwak.batchjob.BatchJobEventTypeMessage\x12\x14\n\x0c\x62\x61tch_job_id\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\r\n\x05\x64\x65lay\x18\x04 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x05 \x01(\x05\"\x84\x02\n\x15\x42\x61tchTaskEventMessage\x12G\n\x15\x62\x61tch_task_event_type\x18\x01 \x01(\x0e\x32(.qwak.batchjob.BatchTaskEventTypeMessage\x12\x14\n\x0c\x62\x61tch_job_id\x18\x02 \x01(\t\x12\x15\n\rbatch_task_id\x18\x03 \x01(\t\x12\x0f\n\x07message\x18\x04 \x01(\t\x12\r\n\x05\x64\x65lay\x18\x05 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x06 \x01(\x05\x12\x43\n\x19\x62\x61tch_task_failure_reason\x18\x07 \x01(\x0b\x32 .qwak.batchjob.TaskFailureReason\"\xec\x01\n\x12WarmupEventMessage\x12\x44\n\x15warmup_job_event_type\x18\x01 \x01(\x0e\x32%.qwak.batchjob.WarmupEventTypeMessage\x12\r\n\x05\x64\x65lay\x18\x02 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x03 \x01(\x05\x12.\n\x0bwarmup_size\x18\x04 \x01(\x0b\x32\x19.qwak.batchjob.WarmupSize\x12?\n\x10model_identifier\x18\x05 \x01(\x0b\x32%.qwak.batchjob.ModelIdentifierMessage\"\xd4\x01\n\nWarmupSize\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12.\n\x0bmemory_unit\x18\x03 \x01(\x0e\x32\x19.qwak.batchjob.MemoryUnit\x12\x13\n\x0bnum_of_pods\x18\x04 \x01(\x05\x12\x17\n\x0ftimeout_seconds\x18\x05 \x01(\x05\x12\x44\n\rgpu_resources\x18\x06 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResources\"|\n\x16ModelIdentifierMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x05 \x01(\t\"\x80\x01\n\x11TaskFailureReason\x12\x46\n\x18task_failure_reason_code\x18\x01 \x01(\x0e\x32$.qwak.batchjob.TaskFailureReasonCode\x12#\n\x1btask_failure_reason_details\x18\x02 \x01(\t*\xf2\x01\n\x18\x42\x61tchJobEventTypeMessage\x12\x1d\n\x19UNDEFINED_BATCH_JOB_EVENT\x10\x00\x12\x17\n\x13\x42\x41TCH_JOB_COMMITTED\x10\x01\x12\x16\n\x12\x42\x41TCH_JOB_PREPARED\x10\x07\x12\x1b\n\x17\x42\x41TCH_JOB_TASKS_CREATED\x10\x02\x12\x17\n\x13\x42\x41TCH_JOB_CANCELLED\x10\x03\x12\x15\n\x11\x42\x41TCH_JOB_CLEANUP\x10\x04\x12\x1c\n\x18\x42\x41TCH_JOB_CHECK_FINISHED\x10\x05\x12\x1b\n\x17\x42\x41TCH_JOB_CHECK_TIMEOUT\x10\x06*\xce\x01\n\x19\x42\x61tchTaskEventTypeMessage\x12\x1e\n\x1aUNDEFINED_BATCH_TASK_EVENT\x10\x00\x12\x16\n\x12\x42\x41TCH_TASK_RUNNING\x10\x01\x12\x17\n\x13\x42\x41TCH_TASK_FINISHED\x10\x02\x12\x15\n\x11\x42\x41TCH_TASK_FAILED\x10\x03\x12\x1b\n\x17\x42\x41TCH_TASK_CHECK_STATUS\x10\x04\x12\x14\n\x10\x42\x41TCH_TASK_START\x10\x05\x12\x16\n\x12\x42\x41TCH_TASK_CLEANUP\x10\x06*e\n\x16WarmupEventTypeMessage\x12\x1e\n\x1aUNDEFINED_WARMUP_JOB_EVENT\x10\x00\x12\x18\n\x14WARMUP_JOB_COMMITTED\x10\x01\x12\x11\n\rWARMUP_CANCEL\x10\x02*+\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\xc0\x04\n\x15TaskFailureReasonCode\x12\x35\n1TASK_FAILURE_REASON_CODE_FAILURE_CODE_UNSPECIFIED\x10\x00\x12\x44\n@TASK_FAILURE_REASON_CODE_NO_REPLICA_SETS_PODS_FOUND_FAILURE_CODE\x10\x01\x12\x43\n?TASK_FAILURE_REASON_CODE_MODEL_CONTAINER_NOT_FOUND_FAILURE_CODE\x10\x02\x12\x37\n3TASK_FAILURE_REASON_CODE_UNSCHEDULABLE_FAILURE_CODE\x10\x03\x12@\n<TASK_FAILURE_REASON_CODE_DOCKER_IMAGE_NOT_FOUND_FAILURE_CODE\x10\x04\x12?\n;TASK_FAILURE_REASON_CODE_MEMORY_LIMIT_EXCEEDED_FAILURE_CODE\x10\x05\x12\x34\n0TASK_FAILURE_REASON_CODE_CRASH_LOOP_FAILURE_CODE\x10\x06\x12\x46\nBTASK_FAILURE_REASON_CODE_CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON\x10\x07\x12+\n\'TASK_FAILURE_REASON_CODE_UNKNOWN_REASON\x10\x08\x42.\n\x19\x63om.qwak.ai.batch.job.apiP\x01Z\x0f./;inferencejobb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(qwak/batch_job/v1/batch_job_events.proto\x12\rqwak.batchjob\x1a/qwak/user_application/common/v0/resources.proto\"\xa5\x01\n\x14\x42\x61tchJobEventMessage\x12\x45\n\x14\x62\x61tch_job_event_type\x18\x01 \x01(\x0e\x32\'.qwak.batchjob.BatchJobEventTypeMessage\x12\x14\n\x0c\x62\x61tch_job_id\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\r\n\x05\x64\x65lay\x18\x04 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x05 \x01(\x05\"\x84\x02\n\x15\x42\x61tchTaskEventMessage\x12G\n\x15\x62\x61tch_task_event_type\x18\x01 \x01(\x0e\x32(.qwak.batchjob.BatchTaskEventTypeMessage\x12\x14\n\x0c\x62\x61tch_job_id\x18\x02 \x01(\t\x12\x15\n\rbatch_task_id\x18\x03 \x01(\t\x12\x0f\n\x07message\x18\x04 \x01(\t\x12\r\n\x05\x64\x65lay\x18\x05 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x06 \x01(\x05\x12\x43\n\x19\x62\x61tch_task_failure_reason\x18\x07 \x01(\x0b\x32 .qwak.batchjob.TaskFailureReason\"\xec\x01\n\x12WarmupEventMessage\x12\x44\n\x15warmup_job_event_type\x18\x01 \x01(\x0e\x32%.qwak.batchjob.WarmupEventTypeMessage\x12\r\n\x05\x64\x65lay\x18\x02 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x03 \x01(\x05\x12.\n\x0bwarmup_size\x18\x04 \x01(\x0b\x32\x19.qwak.batchjob.WarmupSize\x12?\n\x10model_identifier\x18\x05 \x01(\x0b\x32%.qwak.batchjob.ModelIdentifierMessage\"\xb9\x02\n\nWarmupSize\x12\x0f\n\x03\x63pu\x18\x01 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rmemory_amount\x18\x02 \x01(\x05\x42\x02\x18\x01\x12\x32\n\x0bmemory_unit\x18\x03 \x01(\x0e\x32\x19.qwak.batchjob.MemoryUnitB\x02\x18\x01\x12\x13\n\x0bnum_of_pods\x18\x04 \x01(\x05\x12\x17\n\x0ftimeout_seconds\x18\x05 \x01(\x05\x12H\n\rgpu_resources\x18\x06 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesB\x02\x18\x01\x12S\n\x15pod_compute_resources\x18\x07 \x01(\x0b\x32\x34.qwak.user_application.common.v0.PodComputeResources\"|\n\x16ModelIdentifierMessage\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x16\n\x0e\x65nvironment_id\x18\x05 \x01(\t\"\x80\x01\n\x11TaskFailureReason\x12\x46\n\x18task_failure_reason_code\x18\x01 \x01(\x0e\x32$.qwak.batchjob.TaskFailureReasonCode\x12#\n\x1btask_failure_reason_details\x18\x02 \x01(\t*\xf2\x01\n\x18\x42\x61tchJobEventTypeMessage\x12\x1d\n\x19UNDEFINED_BATCH_JOB_EVENT\x10\x00\x12\x17\n\x13\x42\x41TCH_JOB_COMMITTED\x10\x01\x12\x16\n\x12\x42\x41TCH_JOB_PREPARED\x10\x07\x12\x1b\n\x17\x42\x41TCH_JOB_TASKS_CREATED\x10\x02\x12\x17\n\x13\x42\x41TCH_JOB_CANCELLED\x10\x03\x12\x15\n\x11\x42\x41TCH_JOB_CLEANUP\x10\x04\x12\x1c\n\x18\x42\x41TCH_JOB_CHECK_FINISHED\x10\x05\x12\x1b\n\x17\x42\x41TCH_JOB_CHECK_TIMEOUT\x10\x06*\xce\x01\n\x19\x42\x61tchTaskEventTypeMessage\x12\x1e\n\x1aUNDEFINED_BATCH_TASK_EVENT\x10\x00\x12\x16\n\x12\x42\x41TCH_TASK_RUNNING\x10\x01\x12\x17\n\x13\x42\x41TCH_TASK_FINISHED\x10\x02\x12\x15\n\x11\x42\x41TCH_TASK_FAILED\x10\x03\x12\x1b\n\x17\x42\x41TCH_TASK_CHECK_STATUS\x10\x04\x12\x14\n\x10\x42\x41TCH_TASK_START\x10\x05\x12\x16\n\x12\x42\x41TCH_TASK_CLEANUP\x10\x06*e\n\x16WarmupEventTypeMessage\x12\x1e\n\x1aUNDEFINED_WARMUP_JOB_EVENT\x10\x00\x12\x18\n\x14WARMUP_JOB_COMMITTED\x10\x01\x12\x11\n\rWARMUP_CANCEL\x10\x02*+\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\xc0\x04\n\x15TaskFailureReasonCode\x12\x35\n1TASK_FAILURE_REASON_CODE_FAILURE_CODE_UNSPECIFIED\x10\x00\x12\x44\n@TASK_FAILURE_REASON_CODE_NO_REPLICA_SETS_PODS_FOUND_FAILURE_CODE\x10\x01\x12\x43\n?TASK_FAILURE_REASON_CODE_MODEL_CONTAINER_NOT_FOUND_FAILURE_CODE\x10\x02\x12\x37\n3TASK_FAILURE_REASON_CODE_UNSCHEDULABLE_FAILURE_CODE\x10\x03\x12@\n<TASK_FAILURE_REASON_CODE_DOCKER_IMAGE_NOT_FOUND_FAILURE_CODE\x10\x04\x12?\n;TASK_FAILURE_REASON_CODE_MEMORY_LIMIT_EXCEEDED_FAILURE_CODE\x10\x05\x12\x34\n0TASK_FAILURE_REASON_CODE_CRASH_LOOP_FAILURE_CODE\x10\x06\x12\x46\nBTASK_FAILURE_REASON_CODE_CONTAINER_FAIL_TO_LOAD_FOR_UNKNOWN_REASON\x10\x07\x12+\n\'TASK_FAILURE_REASON_CODE_UNKNOWN_REASON\x10\x08\x42.\n\x19\x63om.qwak.ai.batch.job.apiP\x01Z\x0f./;inferencejobb\x06proto3')
 
 _BATCHJOBEVENTTYPEMESSAGE = DESCRIPTOR.enum_types_by_name['BatchJobEventTypeMessage']
 BatchJobEventTypeMessage = enum_type_wrapper.EnumTypeWrapper(_BATCHJOBEVENTTYPEMESSAGE)
 _BATCHTASKEVENTTYPEMESSAGE = DESCRIPTOR.enum_types_by_name['BatchTaskEventTypeMessage']
 BatchTaskEventTypeMessage = enum_type_wrapper.EnumTypeWrapper(_BATCHTASKEVENTTYPEMESSAGE)
 _WARMUPEVENTTYPEMESSAGE = DESCRIPTOR.enum_types_by_name['WarmupEventTypeMessage']
 WarmupEventTypeMessage = enum_type_wrapper.EnumTypeWrapper(_WARMUPEVENTTYPEMESSAGE)
@@ -108,32 +108,40 @@
   })
 _sym_db.RegisterMessage(TaskFailureReason)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\031com.qwak.ai.batch.job.apiP\001Z\017./;inferencejob'
+  _WARMUPSIZE.fields_by_name['cpu']._options = None
+  _WARMUPSIZE.fields_by_name['cpu']._serialized_options = b'\030\001'
+  _WARMUPSIZE.fields_by_name['memory_amount']._options = None
+  _WARMUPSIZE.fields_by_name['memory_amount']._serialized_options = b'\030\001'
+  _WARMUPSIZE.fields_by_name['memory_unit']._options = None
+  _WARMUPSIZE.fields_by_name['memory_unit']._serialized_options = b'\030\001'
+  _WARMUPSIZE.fields_by_name['gpu_resources']._options = None
+  _WARMUPSIZE.fields_by_name['gpu_resources']._serialized_options = b'\030\001'
   _MODELIDENTIFIERMESSAGE.fields_by_name['branch_id']._options = None
   _MODELIDENTIFIERMESSAGE.fields_by_name['branch_id']._serialized_options = b'\030\001'
-  _BATCHJOBEVENTTYPEMESSAGE._serialized_start=1251
-  _BATCHJOBEVENTTYPEMESSAGE._serialized_end=1493
-  _BATCHTASKEVENTTYPEMESSAGE._serialized_start=1496
-  _BATCHTASKEVENTTYPEMESSAGE._serialized_end=1702
-  _WARMUPEVENTTYPEMESSAGE._serialized_start=1704
-  _WARMUPEVENTTYPEMESSAGE._serialized_end=1805
-  _MEMORYUNIT._serialized_start=1807
-  _MEMORYUNIT._serialized_end=1850
-  _TASKFAILUREREASONCODE._serialized_start=1853
-  _TASKFAILUREREASONCODE._serialized_end=2429
+  _BATCHJOBEVENTTYPEMESSAGE._serialized_start=1352
+  _BATCHJOBEVENTTYPEMESSAGE._serialized_end=1594
+  _BATCHTASKEVENTTYPEMESSAGE._serialized_start=1597
+  _BATCHTASKEVENTTYPEMESSAGE._serialized_end=1803
+  _WARMUPEVENTTYPEMESSAGE._serialized_start=1805
+  _WARMUPEVENTTYPEMESSAGE._serialized_end=1906
+  _MEMORYUNIT._serialized_start=1908
+  _MEMORYUNIT._serialized_end=1951
+  _TASKFAILUREREASONCODE._serialized_start=1954
+  _TASKFAILUREREASONCODE._serialized_end=2530
   _BATCHJOBEVENTMESSAGE._serialized_start=109
   _BATCHJOBEVENTMESSAGE._serialized_end=274
   _BATCHTASKEVENTMESSAGE._serialized_start=277
   _BATCHTASKEVENTMESSAGE._serialized_end=537
   _WARMUPEVENTMESSAGE._serialized_start=540
   _WARMUPEVENTMESSAGE._serialized_end=776
   _WARMUPSIZE._serialized_start=779
-  _WARMUPSIZE._serialized_end=991
-  _MODELIDENTIFIERMESSAGE._serialized_start=993
-  _MODELIDENTIFIERMESSAGE._serialized_end=1117
-  _TASKFAILUREREASON._serialized_start=1120
-  _TASKFAILUREREASON._serialized_end=1248
+  _WARMUPSIZE._serialized_end=1092
+  _MODELIDENTIFIERMESSAGE._serialized_start=1094
+  _MODELIDENTIFIERMESSAGE._serialized_end=1218
+  _TASKFAILUREREASON._serialized_start=1221
+  _TASKFAILUREREASON._serialized_end=1349
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -226,35 +226,39 @@
 
     CPU_FIELD_NUMBER: builtins.int
     MEMORY_AMOUNT_FIELD_NUMBER: builtins.int
     MEMORY_UNIT_FIELD_NUMBER: builtins.int
     NUM_OF_PODS_FIELD_NUMBER: builtins.int
     TIMEOUT_SECONDS_FIELD_NUMBER: builtins.int
     GPU_RESOURCES_FIELD_NUMBER: builtins.int
+    POD_COMPUTE_RESOURCES_FIELD_NUMBER: builtins.int
     cpu: builtins.float
     memory_amount: builtins.int
     memory_unit: global___MemoryUnit.ValueType
     num_of_pods: builtins.int
     timeout_seconds: builtins.int
     """The timeout for the warmup"""
     @property
     def gpu_resources(self) -> qwak.user_application.common.v0.resources_pb2.GpuResources:
         """Optional GPU resources for batch"""
+    @property
+    def pod_compute_resources(self) -> qwak.user_application.common.v0.resources_pb2.PodComputeResources: ...
     def __init__(
         self,
         *,
         cpu: builtins.float = ...,
         memory_amount: builtins.int = ...,
         memory_unit: global___MemoryUnit.ValueType = ...,
         num_of_pods: builtins.int = ...,
         timeout_seconds: builtins.int = ...,
         gpu_resources: qwak.user_application.common.v0.resources_pb2.GpuResources | None = ...,
+        pod_compute_resources: qwak.user_application.common.v0.resources_pb2.PodComputeResources | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["gpu_resources", b"gpu_resources"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cpu", b"cpu", "gpu_resources", b"gpu_resources", "memory_amount", b"memory_amount", "memory_unit", b"memory_unit", "num_of_pods", b"num_of_pods", "timeout_seconds", b"timeout_seconds"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["gpu_resources", b"gpu_resources", "pod_compute_resources", b"pod_compute_resources"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cpu", b"cpu", "gpu_resources", b"gpu_resources", "memory_amount", b"memory_amount", "memory_unit", b"memory_unit", "num_of_pods", b"num_of_pods", "pod_compute_resources", b"pod_compute_resources", "timeout_seconds", b"timeout_seconds"]) -> None: ...
 
 global___WarmupSize = WarmupSize
 
 class ModelIdentifierMessage(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MODEL_ID_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from _qwak_proto.qwak.user_application.common.v0 import resources_pb2 as qwak_dot_user__application_dot_common_dot_v0_dot_resources__pb2
 from _qwak_proto.qwak.batch_job.v1 import batch_job_events_pb2 as qwak_dot_batch__job_dot_v1_dot_batch__job__events__pb2
 from _qwak_proto.qwak.administration.authenticated_user.v1 import credentials_pb2 as qwak_dot_administration_dot_authenticated__user_dot_v1_dot_credentials__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)qwak/batch_job/v1/batch_job_service.proto\x12\rqwak.batchjob\x1a\x1fgoogle/protobuf/timestamp.proto\x1a/qwak/user_application/common/v0/resources.proto\x1a(qwak/batch_job/v1/batch_job_events.proto\x1a;qwak/administration/authenticated_user/v1/credentials.proto\"\xb4\x01\n\x15StartWarmupJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x05 \x01(\t\x12\x16\n\x0ewarmup_timeout\x18\x03 \x01(\x05\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x04 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\"B\n\x16StartWarmupJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"S\n\x16\x43\x61ncelWarmupJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\"C\n\x17\x43\x61ncelWarmupJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"\x89\x05\n\x14StartBatchJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x0f \x01(\t\x12\x15\n\rsource_bucket\x18\x03 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x04 \x01(\t\x12\x15\n\rsource_folder\x18\x05 \x01(\t\x12\x1a\n\x12\x64\x65stination_folder\x18\x06 \x01(\t\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x07 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12\x13\n\x0bjob_timeout\x18\x08 \x01(\x05\x12\x14\n\x0ctask_timeout\x18\t \x01(\x05\x12\x35\n\x0finput_file_type\x18\n \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\x12\x37\n\x10output_file_type\x18\x0b \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\x12\x14\n\x0ctoken_secret\x18\x0c \x01(\t\x12\x15\n\rsecret_secret\x18\r \x01(\t\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x0e \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\x12\x34\n\nparameters\x18\x10 \x03(\x0b\x32 .qwak.batchjob.BatchJobParameter\x12\x39\n\x11\x62\x61tch_job_request\x18\x11 \x01(\x0b\x32\x1e.qwak.batchjob.BatchJobRequest\"\xcb\x01\n\x0f\x42\x61tchJobRequest\x12:\n\rmodel_details\x18\x01 \x01(\x0b\x32#.qwak.batchjob.BatchJobModelDetails\x12\x38\n\x0c\x64\x61ta_details\x18\x02 \x01(\x0b\x32\".qwak.batchjob.BatchJobDataDetails\x12\x42\n\x11\x65xecution_details\x18\x04 \x01(\x0b\x32\'.qwak.batchjob.BatchJobExecutionDetails\":\n\x14\x42\x61tchJobModelDetails\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x0f \x01(\t\"\xbc\x01\n\x13\x42\x61tchJobDataDetails\x12\x36\n\x0bsource_path\x18\x01 \x01(\x0b\x32!.qwak.batchjob.BatchJobSourcePath\x12@\n\x10\x64\x65stination_path\x18\x02 \x01(\x0b\x32&.qwak.batchjob.BatchJobDestinationPath\x12\x14\n\x0ctoken_secret\x18\x0c \x01(\t\x12\x15\n\rsecret_secret\x18\r \x01(\t\"y\n\x12\x42\x61tchJobSourcePath\x12\x15\n\rsource_bucket\x18\x01 \x01(\t\x12\x15\n\rsource_folder\x18\x02 \x01(\t\x12\x35\n\x0finput_file_type\x18\x03 \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\"\x8a\x01\n\x17\x42\x61tchJobDestinationPath\x12\x1a\n\x12\x64\x65stination_bucket\x18\x01 \x01(\t\x12\x1a\n\x12\x64\x65stination_folder\x18\x02 \x01(\t\x12\x37\n\x10output_file_type\x18\x03 \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\"\x94\x02\n\x18\x42\x61tchJobExecutionDetails\x12\x13\n\x0bjob_timeout\x18\x01 \x01(\x05\x12\x14\n\x0ctask_timeout\x18\x02 \x01(\x05\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x03 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x04 \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\x12\x34\n\nparameters\x18\x05 \x03(\x0b\x32 .qwak.batchjob.BatchJobParameter\"/\n\x11\x42\x61tchJobParameter\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"S\n\x15StartBatchJobResponse\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\")\n\x15\x43\x61ncelBatchJobRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"B\n\x16\x43\x61ncelBatchJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\",\n\x18GetBatchJobStatusRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"\xac\x01\n\x19GetBatchJobStatusResponse\x12\x38\n\njob_status\x18\x01 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\x12\x16\n\x0e\x66inished_files\x18\x04 \x01(\x05\x12\x13\n\x0btotal_files\x18\x05 \x01(\x05\",\n\x18GetBatchJobReportRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"a\n\x19GetBatchJobReportResponse\x12\x12\n\nsuccessful\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\x12\x17\n\x0freport_messages\x18\x03 \x03(\t\"`\n\x1dUpdateBatchTasksStatusRequest\x12?\n\x11\x62\x61tch_task_events\x18\x01 \x03(\x0b\x32$.qwak.batchjob.BatchTaskEventMessage\"I\n\x1dUpdateBatchTaskStatusResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"Q\n\x19\x41\x64vancedDeploymentOptions\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x01 \x01(\t\x12\x17\n\x0fpurchase_option\x18\x02 \x01(\t\"\x8f\x02\n\x16\x42\x61tchJobDeploymentSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x02\x12\x15\n\rmemory_amount\x18\x03 \x01(\x05\x12\x46\n\x0cmemory_units\x18\x04 \x01(\x0e\x32\x30.qwak.batchjob.BatchJobDeploymentSize.MemoryUnit\x12\x44\n\rgpu_resources\x18\x05 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResources\"+\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02\"?\n\x14ListBatchJobsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\"K\n\x15ListBatchJobsResponse\x12\x32\n\nbatch_jobs\x18\x01 \x03(\x0b\x32\x1e.qwak.batchjob.BatchJobDetails\"\x9d\x02\n\x0f\x42\x61tchJobDetails\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06job_id\x18\x02 \x01(\t\x12\x38\n\njob_status\x18\x03 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12.\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x66\x61ilure_message\x18\x06 \x01(\t\x12\x37\n\x08job_size\x18\x07 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\"+\n\x19GetBatchJobDetailsRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"y\n\x1aGetBatchJobDetailsResponse\x12\x31\n\tbatch_job\x18\x01 \x01(\x0b\x32\x1e.qwak.batchjob.BatchJobMessage\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\"\x84\x04\n\x0f\x42\x61tchJobMessage\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\tbranch_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x04 \x01(\t\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\njob_status\x18\x07 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12\x15\n\rtotal_records\x18\x08 \x01(\x05\x12\x37\n\x08job_size\x18\t \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12;\n\x0freport_messages\x18\n \x03(\x0b\x32\".qwak.batchjob.ExecutionReportLine\x12\x43\n\x16\x65xecution_file_details\x18\x0b \x01(\x0b\x32#.qwak.batchjob.ExecutionFileDetails\x12<\n\x0ftask_executions\x18\x0c \x03(\x0b\x32#.qwak.batchjob.TaskExecutionDetails\"M\n\x13\x45xecutionReportLine\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04line\x18\x02 \x01(\t\"\x95\x02\n\x14\x45xecutionFileDetails\x12\x15\n\rsource_bucket\x18\x01 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x02 \x01(\t\x12\x13\n\x0bsource_path\x18\x03 \x01(\t\x12\x18\n\x10\x64\x65stination_path\x18\x04 \x01(\t\x12\x35\n\x0finput_file_type\x18\x05 \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\x12\x37\n\x10output_file_type\x18\x06 \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\x12\x16\n\x0e\x66inished_files\x18\x07 \x01(\x05\x12\x13\n\x0btotal_files\x18\x08 \x01(\x05\"\xe6\x01\n\x14TaskExecutionDetails\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x35\n\x06status\x18\x02 \x01(\x0e\x32%.qwak.batchjob.BatchTaskStatusMessage\x12.\n\nstart_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0enum_of_records\x18\x05 \x01(\x05\x12\x10\n\x08\x66ilename\x18\x06 \x01(\t\"d\n$GetBatchJobPreSignedUploadUrlRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x17\n\x0fnumber_of_files\x18\x02 \x01(\x05\x12\x11\n\tfile_type\x18\x03 \x01(\t\"\x98\x01\n%GetBatchJobPreSignedUploadUrlResponse\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x13\n\x0boutput_path\x18\x02 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12\x0c\n\x04urls\x18\x04 \x03(\t\x12\x0f\n\x07success\x18\x05 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x06 \x01(\t\"8\n&GetBatchJobPreSignedDownloadUrlRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"a\n\'GetBatchJobPreSignedDownloadUrlResponse\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\"3\n\x1fGetBatchJobUploadDetailsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\"\xb4\x01\n GetBatchJobUploadDetailsResponse\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x13\n\x0boutput_path\x18\x02 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12W\n\x0b\x63redentials\x18\x04 \x01(\x0b\x32\x42.qwak.administration.authenticated_user.v1.AwsTemporaryCredentials\"3\n!GetBatchJobDownloadDetailsRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"\x9b\x01\n\"GetBatchJobDownloadDetailsResponse\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\t\x12W\n\x0b\x63redentials\x18\x03 \x01(\x0b\x32\x42.qwak.administration.authenticated_user.v1.AwsTemporaryCredentials\"\xd7\x01\n\x1aUpdateDefaultParamsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x46\n\x17\x64\x65\x66\x61ult_deployment_size\x18\x03 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x04 \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\"\x1d\n\x1bUpdateDefaultParamsResponse\".\n\x1a\x44\x65leteDefaultParamsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\"\x1d\n\x1b\x44\x65leteDefaultParamsResponse*\x81\x01\n\rInputFileType\x12\x1d\n\x19UNDEFINED_INPUT_FILE_TYPE\x10\x00\x12\x17\n\x13\x43SV_INPUT_FILE_TYPE\x10\x01\x12\x1b\n\x17\x46\x45\x41THER_INPUT_FILE_TYPE\x10\x02\x12\x1b\n\x17PARQUET_INPUT_FILE_TYPE\x10\x03*\x86\x01\n\x0eOutputFileType\x12\x1e\n\x1aUNDEFINED_OUTPUT_FILE_TYPE\x10\x00\x12\x18\n\x14\x43SV_OUTPUT_FILE_TYPE\x10\x01\x12\x1c\n\x18\x46\x45\x41THER_OUTPUT_FILE_TYPE\x10\x02\x12\x1c\n\x18PARQUET_OUTPUT_FILE_TYPE\x10\x03*\x8d\x02\n\x15\x42\x61tchJobStatusMessage\x12\x1e\n\x1aUNDEFINED_BATCH_JOB_STATUS\x10\x00\x12\x1e\n\x1a\x42\x41TCH_JOB_COMMITTED_STATUS\x10\x01\x12\x1c\n\x18\x42\x41TCH_JOB_PENDING_STATUS\x10\x02\x12\x1c\n\x18\x42\x41TCH_JOB_RUNNING_STATUS\x10\x03\x12\x1d\n\x19\x42\x41TCH_JOB_FINISHED_STATUS\x10\x04\x12\x1b\n\x17\x42\x41TCH_JOB_FAILED_STATUS\x10\x05\x12\x1e\n\x1a\x42\x41TCH_JOB_CANCELLED_STATUS\x10\x06\x12\x1c\n\x18\x42\x41TCH_JOB_TIMEOUT_STATUS\x10\x07*\x9c\x02\n\x16\x42\x61tchTaskStatusMessage\x12\x1f\n\x1bUNDEFINED_BATCH_TASK_STATUS\x10\x00\x12\x1f\n\x1b\x42\x41TCH_TASK_COMMITTED_STATUS\x10\x01\x12#\n\x1f\x42\x41TCH_TASK_PENDING_START_STATUS\x10\x02\x12\x1d\n\x19\x42\x41TCH_TASK_RUNNING_STATUS\x10\x03\x12\x1e\n\x1a\x42\x41TCH_TASK_FINISHED_STATUS\x10\x04\x12\x1c\n\x18\x42\x41TCH_TASK_FAILED_STATUS\x10\x05\x12\x1f\n\x1b\x42\x41TCH_TASK_CANCELLED_STATUS\x10\x06\x12\x1d\n\x19\x42\x41TCH_TASK_TIMEOUT_STATUS\x10\x07\x32\xa1\r\n\x19\x42\x61tchJobManagementService\x12Z\n\rStartBatchJob\x12#.qwak.batchjob.StartBatchJobRequest\x1a$.qwak.batchjob.StartBatchJobResponse\x12]\n\x0e\x43\x61ncelBatchJob\x12$.qwak.batchjob.CancelBatchJobRequest\x1a%.qwak.batchjob.CancelBatchJobResponse\x12]\n\x0eStartWarmupJob\x12$.qwak.batchjob.StartWarmupJobRequest\x1a%.qwak.batchjob.StartWarmupJobResponse\x12`\n\x0f\x43\x61ncelWarmupJob\x12%.qwak.batchjob.CancelWarmupJobRequest\x1a&.qwak.batchjob.CancelWarmupJobResponse\x12\x66\n\x11GetBatchJobStatus\x12\'.qwak.batchjob.GetBatchJobStatusRequest\x1a(.qwak.batchjob.GetBatchJobStatusResponse\x12\x66\n\x11GetBatchJobReport\x12\'.qwak.batchjob.GetBatchJobReportRequest\x1a(.qwak.batchjob.GetBatchJobReportResponse\x12t\n\x16UpdateBatchTasksStatus\x12,.qwak.batchjob.UpdateBatchTasksStatusRequest\x1a,.qwak.batchjob.UpdateBatchTaskStatusResponse\x12Z\n\rListBatchJobs\x12#.qwak.batchjob.ListBatchJobsRequest\x1a$.qwak.batchjob.ListBatchJobsResponse\x12i\n\x12GetBatchJobDetails\x12(.qwak.batchjob.GetBatchJobDetailsRequest\x1a).qwak.batchjob.GetBatchJobDetailsResponse\x12\x8a\x01\n\x1dGetBatchJobPreSignedUploadUrl\x12\x33.qwak.batchjob.GetBatchJobPreSignedUploadUrlRequest\x1a\x34.qwak.batchjob.GetBatchJobPreSignedUploadUrlResponse\x12\x90\x01\n\x1fGetBatchJobPreSignedDownloadUrl\x12\x35.qwak.batchjob.GetBatchJobPreSignedDownloadUrlRequest\x1a\x36.qwak.batchjob.GetBatchJobPreSignedDownloadUrlResponse\x12{\n\x18GetBatchJobUploadDetails\x12..qwak.batchjob.GetBatchJobUploadDetailsRequest\x1a/.qwak.batchjob.GetBatchJobUploadDetailsResponse\x12\x81\x01\n\x1aGetBatchJobDownloadDetails\x12\x30.qwak.batchjob.GetBatchJobDownloadDetailsRequest\x1a\x31.qwak.batchjob.GetBatchJobDownloadDetailsResponse\x12l\n\x13UpdateDefaultParams\x12).qwak.batchjob.UpdateDefaultParamsRequest\x1a*.qwak.batchjob.UpdateDefaultParamsResponse\x12l\n\x13\x44\x65leteDefaultParams\x12).qwak.batchjob.DeleteDefaultParamsRequest\x1a*.qwak.batchjob.DeleteDefaultParamsResponseB.\n\x19\x63om.qwak.ai.batch.job.apiP\x01Z\x0f./;inferencejobb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)qwak/batch_job/v1/batch_job_service.proto\x12\rqwak.batchjob\x1a\x1fgoogle/protobuf/timestamp.proto\x1a/qwak/user_application/common/v0/resources.proto\x1a(qwak/batch_job/v1/batch_job_events.proto\x1a;qwak/administration/authenticated_user/v1/credentials.proto\"\xb4\x01\n\x15StartWarmupJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x05 \x01(\t\x12\x16\n\x0ewarmup_timeout\x18\x03 \x01(\x05\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x04 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\"B\n\x16StartWarmupJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"S\n\x16\x43\x61ncelWarmupJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\"C\n\x17\x43\x61ncelWarmupJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"\x89\x05\n\x14StartBatchJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x0f \x01(\t\x12\x15\n\rsource_bucket\x18\x03 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x04 \x01(\t\x12\x15\n\rsource_folder\x18\x05 \x01(\t\x12\x1a\n\x12\x64\x65stination_folder\x18\x06 \x01(\t\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x07 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12\x13\n\x0bjob_timeout\x18\x08 \x01(\x05\x12\x14\n\x0ctask_timeout\x18\t \x01(\x05\x12\x35\n\x0finput_file_type\x18\n \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\x12\x37\n\x10output_file_type\x18\x0b \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\x12\x14\n\x0ctoken_secret\x18\x0c \x01(\t\x12\x15\n\rsecret_secret\x18\r \x01(\t\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x0e \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\x12\x34\n\nparameters\x18\x10 \x03(\x0b\x32 .qwak.batchjob.BatchJobParameter\x12\x39\n\x11\x62\x61tch_job_request\x18\x11 \x01(\x0b\x32\x1e.qwak.batchjob.BatchJobRequest\"\xcb\x01\n\x0f\x42\x61tchJobRequest\x12:\n\rmodel_details\x18\x01 \x01(\x0b\x32#.qwak.batchjob.BatchJobModelDetails\x12\x38\n\x0c\x64\x61ta_details\x18\x02 \x01(\x0b\x32\".qwak.batchjob.BatchJobDataDetails\x12\x42\n\x11\x65xecution_details\x18\x04 \x01(\x0b\x32\'.qwak.batchjob.BatchJobExecutionDetails\":\n\x14\x42\x61tchJobModelDetails\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x0f \x01(\t\"\xbc\x01\n\x13\x42\x61tchJobDataDetails\x12\x36\n\x0bsource_path\x18\x01 \x01(\x0b\x32!.qwak.batchjob.BatchJobSourcePath\x12@\n\x10\x64\x65stination_path\x18\x02 \x01(\x0b\x32&.qwak.batchjob.BatchJobDestinationPath\x12\x14\n\x0ctoken_secret\x18\x0c \x01(\t\x12\x15\n\rsecret_secret\x18\r \x01(\t\"y\n\x12\x42\x61tchJobSourcePath\x12\x15\n\rsource_bucket\x18\x01 \x01(\t\x12\x15\n\rsource_folder\x18\x02 \x01(\t\x12\x35\n\x0finput_file_type\x18\x03 \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\"\x8a\x01\n\x17\x42\x61tchJobDestinationPath\x12\x1a\n\x12\x64\x65stination_bucket\x18\x01 \x01(\t\x12\x1a\n\x12\x64\x65stination_folder\x18\x02 \x01(\t\x12\x37\n\x10output_file_type\x18\x03 \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\"\x94\x02\n\x18\x42\x61tchJobExecutionDetails\x12\x13\n\x0bjob_timeout\x18\x01 \x01(\x05\x12\x14\n\x0ctask_timeout\x18\x02 \x01(\x05\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x03 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x04 \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\x12\x34\n\nparameters\x18\x05 \x03(\x0b\x32 .qwak.batchjob.BatchJobParameter\"/\n\x11\x42\x61tchJobParameter\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"S\n\x15StartBatchJobResponse\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\")\n\x15\x43\x61ncelBatchJobRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"B\n\x16\x43\x61ncelBatchJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\",\n\x18GetBatchJobStatusRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"\xac\x01\n\x19GetBatchJobStatusResponse\x12\x38\n\njob_status\x18\x01 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\x12\x16\n\x0e\x66inished_files\x18\x04 \x01(\x05\x12\x13\n\x0btotal_files\x18\x05 \x01(\x05\",\n\x18GetBatchJobReportRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"a\n\x19GetBatchJobReportResponse\x12\x12\n\nsuccessful\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\x12\x17\n\x0freport_messages\x18\x03 \x03(\t\"`\n\x1dUpdateBatchTasksStatusRequest\x12?\n\x11\x62\x61tch_task_events\x18\x01 \x03(\x0b\x32$.qwak.batchjob.BatchTaskEventMessage\"I\n\x1dUpdateBatchTaskStatusResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"Q\n\x19\x41\x64vancedDeploymentOptions\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x01 \x01(\t\x12\x17\n\x0fpurchase_option\x18\x02 \x01(\t\"\x85\x03\n\x16\x42\x61tchJobDeploymentSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0f\n\x03\x63pu\x18\x02 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rmemory_amount\x18\x03 \x01(\x05\x42\x02\x18\x01\x12J\n\x0cmemory_units\x18\x04 \x01(\x0e\x32\x30.qwak.batchjob.BatchJobDeploymentSize.MemoryUnitB\x02\x18\x01\x12H\n\rgpu_resources\x18\x05 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesB\x02\x18\x01\x12`\n\x1c\x63lient_pod_compute_resources\x18\x06 \x01(\x0b\x32:.qwak.user_application.common.v0.ClientPodComputeResources\"/\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02\x1a\x02\x18\x01\"\x99\x01\n\x15\x42\x61tchJobExecutionSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12S\n\x15pod_compute_resources\x18\x02 \x01(\x0b\x32\x34.qwak.user_application.common.v0.PodComputeResources\x12\x13\n\x0btemplate_id\x18\x03 \x01(\t\"?\n\x14ListBatchJobsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\"K\n\x15ListBatchJobsResponse\x12\x32\n\nbatch_jobs\x18\x01 \x03(\x0b\x32\x1e.qwak.batchjob.BatchJobDetails\"\xe9\x02\n\x0f\x42\x61tchJobDetails\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06job_id\x18\x02 \x01(\t\x12\x38\n\njob_status\x18\x03 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12.\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x66\x61ilure_message\x18\x06 \x01(\t\x12;\n\x08job_size\x18\x07 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSizeB\x02\x18\x01\x12\x46\n\x18\x62\x61tch_job_execution_size\x18\x08 \x01(\x0b\x32$.qwak.batchjob.BatchJobExecutionSize\"+\n\x19GetBatchJobDetailsRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"y\n\x1aGetBatchJobDetailsResponse\x12\x31\n\tbatch_job\x18\x01 \x01(\x0b\x32\x1e.qwak.batchjob.BatchJobMessage\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\"\x84\x04\n\x0f\x42\x61tchJobMessage\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\tbranch_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x04 \x01(\t\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\njob_status\x18\x07 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12\x15\n\rtotal_records\x18\x08 \x01(\x05\x12\x37\n\x08job_size\x18\t \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12;\n\x0freport_messages\x18\n \x03(\x0b\x32\".qwak.batchjob.ExecutionReportLine\x12\x43\n\x16\x65xecution_file_details\x18\x0b \x01(\x0b\x32#.qwak.batchjob.ExecutionFileDetails\x12<\n\x0ftask_executions\x18\x0c \x03(\x0b\x32#.qwak.batchjob.TaskExecutionDetails\"M\n\x13\x45xecutionReportLine\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04line\x18\x02 \x01(\t\"\x95\x02\n\x14\x45xecutionFileDetails\x12\x15\n\rsource_bucket\x18\x01 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x02 \x01(\t\x12\x13\n\x0bsource_path\x18\x03 \x01(\t\x12\x18\n\x10\x64\x65stination_path\x18\x04 \x01(\t\x12\x35\n\x0finput_file_type\x18\x05 \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\x12\x37\n\x10output_file_type\x18\x06 \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\x12\x16\n\x0e\x66inished_files\x18\x07 \x01(\x05\x12\x13\n\x0btotal_files\x18\x08 \x01(\x05\"\xe6\x01\n\x14TaskExecutionDetails\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x35\n\x06status\x18\x02 \x01(\x0e\x32%.qwak.batchjob.BatchTaskStatusMessage\x12.\n\nstart_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0enum_of_records\x18\x05 \x01(\x05\x12\x10\n\x08\x66ilename\x18\x06 \x01(\t\"d\n$GetBatchJobPreSignedUploadUrlRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x17\n\x0fnumber_of_files\x18\x02 \x01(\x05\x12\x11\n\tfile_type\x18\x03 \x01(\t\"\x98\x01\n%GetBatchJobPreSignedUploadUrlResponse\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x13\n\x0boutput_path\x18\x02 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12\x0c\n\x04urls\x18\x04 \x03(\t\x12\x0f\n\x07success\x18\x05 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x06 \x01(\t\"8\n&GetBatchJobPreSignedDownloadUrlRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"a\n\'GetBatchJobPreSignedDownloadUrlResponse\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\"3\n\x1fGetBatchJobUploadDetailsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\"\xb4\x01\n GetBatchJobUploadDetailsResponse\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x13\n\x0boutput_path\x18\x02 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12W\n\x0b\x63redentials\x18\x04 \x01(\x0b\x32\x42.qwak.administration.authenticated_user.v1.AwsTemporaryCredentials\"3\n!GetBatchJobDownloadDetailsRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"\x9b\x01\n\"GetBatchJobDownloadDetailsResponse\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\t\x12W\n\x0b\x63redentials\x18\x03 \x01(\x0b\x32\x42.qwak.administration.authenticated_user.v1.AwsTemporaryCredentials\"\xd7\x01\n\x1aUpdateDefaultParamsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x46\n\x17\x64\x65\x66\x61ult_deployment_size\x18\x03 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x04 \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\"\x1d\n\x1bUpdateDefaultParamsResponse\".\n\x1a\x44\x65leteDefaultParamsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\"\x1d\n\x1b\x44\x65leteDefaultParamsResponse*\x81\x01\n\rInputFileType\x12\x1d\n\x19UNDEFINED_INPUT_FILE_TYPE\x10\x00\x12\x17\n\x13\x43SV_INPUT_FILE_TYPE\x10\x01\x12\x1b\n\x17\x46\x45\x41THER_INPUT_FILE_TYPE\x10\x02\x12\x1b\n\x17PARQUET_INPUT_FILE_TYPE\x10\x03*\x86\x01\n\x0eOutputFileType\x12\x1e\n\x1aUNDEFINED_OUTPUT_FILE_TYPE\x10\x00\x12\x18\n\x14\x43SV_OUTPUT_FILE_TYPE\x10\x01\x12\x1c\n\x18\x46\x45\x41THER_OUTPUT_FILE_TYPE\x10\x02\x12\x1c\n\x18PARQUET_OUTPUT_FILE_TYPE\x10\x03*\x8d\x02\n\x15\x42\x61tchJobStatusMessage\x12\x1e\n\x1aUNDEFINED_BATCH_JOB_STATUS\x10\x00\x12\x1e\n\x1a\x42\x41TCH_JOB_COMMITTED_STATUS\x10\x01\x12\x1c\n\x18\x42\x41TCH_JOB_PENDING_STATUS\x10\x02\x12\x1c\n\x18\x42\x41TCH_JOB_RUNNING_STATUS\x10\x03\x12\x1d\n\x19\x42\x41TCH_JOB_FINISHED_STATUS\x10\x04\x12\x1b\n\x17\x42\x41TCH_JOB_FAILED_STATUS\x10\x05\x12\x1e\n\x1a\x42\x41TCH_JOB_CANCELLED_STATUS\x10\x06\x12\x1c\n\x18\x42\x41TCH_JOB_TIMEOUT_STATUS\x10\x07*\x9c\x02\n\x16\x42\x61tchTaskStatusMessage\x12\x1f\n\x1bUNDEFINED_BATCH_TASK_STATUS\x10\x00\x12\x1f\n\x1b\x42\x41TCH_TASK_COMMITTED_STATUS\x10\x01\x12#\n\x1f\x42\x41TCH_TASK_PENDING_START_STATUS\x10\x02\x12\x1d\n\x19\x42\x41TCH_TASK_RUNNING_STATUS\x10\x03\x12\x1e\n\x1a\x42\x41TCH_TASK_FINISHED_STATUS\x10\x04\x12\x1c\n\x18\x42\x41TCH_TASK_FAILED_STATUS\x10\x05\x12\x1f\n\x1b\x42\x41TCH_TASK_CANCELLED_STATUS\x10\x06\x12\x1d\n\x19\x42\x41TCH_TASK_TIMEOUT_STATUS\x10\x07\x32\xa1\r\n\x19\x42\x61tchJobManagementService\x12Z\n\rStartBatchJob\x12#.qwak.batchjob.StartBatchJobRequest\x1a$.qwak.batchjob.StartBatchJobResponse\x12]\n\x0e\x43\x61ncelBatchJob\x12$.qwak.batchjob.CancelBatchJobRequest\x1a%.qwak.batchjob.CancelBatchJobResponse\x12]\n\x0eStartWarmupJob\x12$.qwak.batchjob.StartWarmupJobRequest\x1a%.qwak.batchjob.StartWarmupJobResponse\x12`\n\x0f\x43\x61ncelWarmupJob\x12%.qwak.batchjob.CancelWarmupJobRequest\x1a&.qwak.batchjob.CancelWarmupJobResponse\x12\x66\n\x11GetBatchJobStatus\x12\'.qwak.batchjob.GetBatchJobStatusRequest\x1a(.qwak.batchjob.GetBatchJobStatusResponse\x12\x66\n\x11GetBatchJobReport\x12\'.qwak.batchjob.GetBatchJobReportRequest\x1a(.qwak.batchjob.GetBatchJobReportResponse\x12t\n\x16UpdateBatchTasksStatus\x12,.qwak.batchjob.UpdateBatchTasksStatusRequest\x1a,.qwak.batchjob.UpdateBatchTaskStatusResponse\x12Z\n\rListBatchJobs\x12#.qwak.batchjob.ListBatchJobsRequest\x1a$.qwak.batchjob.ListBatchJobsResponse\x12i\n\x12GetBatchJobDetails\x12(.qwak.batchjob.GetBatchJobDetailsRequest\x1a).qwak.batchjob.GetBatchJobDetailsResponse\x12\x8a\x01\n\x1dGetBatchJobPreSignedUploadUrl\x12\x33.qwak.batchjob.GetBatchJobPreSignedUploadUrlRequest\x1a\x34.qwak.batchjob.GetBatchJobPreSignedUploadUrlResponse\x12\x90\x01\n\x1fGetBatchJobPreSignedDownloadUrl\x12\x35.qwak.batchjob.GetBatchJobPreSignedDownloadUrlRequest\x1a\x36.qwak.batchjob.GetBatchJobPreSignedDownloadUrlResponse\x12{\n\x18GetBatchJobUploadDetails\x12..qwak.batchjob.GetBatchJobUploadDetailsRequest\x1a/.qwak.batchjob.GetBatchJobUploadDetailsResponse\x12\x81\x01\n\x1aGetBatchJobDownloadDetails\x12\x30.qwak.batchjob.GetBatchJobDownloadDetailsRequest\x1a\x31.qwak.batchjob.GetBatchJobDownloadDetailsResponse\x12l\n\x13UpdateDefaultParams\x12).qwak.batchjob.UpdateDefaultParamsRequest\x1a*.qwak.batchjob.UpdateDefaultParamsResponse\x12l\n\x13\x44\x65leteDefaultParams\x12).qwak.batchjob.DeleteDefaultParamsRequest\x1a*.qwak.batchjob.DeleteDefaultParamsResponseB.\n\x19\x63om.qwak.ai.batch.job.apiP\x01Z\x0f./;inferencejobb\x06proto3')
 
 _INPUTFILETYPE = DESCRIPTOR.enum_types_by_name['InputFileType']
 InputFileType = enum_type_wrapper.EnumTypeWrapper(_INPUTFILETYPE)
 _OUTPUTFILETYPE = DESCRIPTOR.enum_types_by_name['OutputFileType']
 OutputFileType = enum_type_wrapper.EnumTypeWrapper(_OUTPUTFILETYPE)
 _BATCHJOBSTATUSMESSAGE = DESCRIPTOR.enum_types_by_name['BatchJobStatusMessage']
 BatchJobStatusMessage = enum_type_wrapper.EnumTypeWrapper(_BATCHJOBSTATUSMESSAGE)
@@ -74,14 +74,15 @@
 _GETBATCHJOBSTATUSRESPONSE = DESCRIPTOR.message_types_by_name['GetBatchJobStatusResponse']
 _GETBATCHJOBREPORTREQUEST = DESCRIPTOR.message_types_by_name['GetBatchJobReportRequest']
 _GETBATCHJOBREPORTRESPONSE = DESCRIPTOR.message_types_by_name['GetBatchJobReportResponse']
 _UPDATEBATCHTASKSSTATUSREQUEST = DESCRIPTOR.message_types_by_name['UpdateBatchTasksStatusRequest']
 _UPDATEBATCHTASKSTATUSRESPONSE = DESCRIPTOR.message_types_by_name['UpdateBatchTaskStatusResponse']
 _ADVANCEDDEPLOYMENTOPTIONS = DESCRIPTOR.message_types_by_name['AdvancedDeploymentOptions']
 _BATCHJOBDEPLOYMENTSIZE = DESCRIPTOR.message_types_by_name['BatchJobDeploymentSize']
+_BATCHJOBEXECUTIONSIZE = DESCRIPTOR.message_types_by_name['BatchJobExecutionSize']
 _LISTBATCHJOBSREQUEST = DESCRIPTOR.message_types_by_name['ListBatchJobsRequest']
 _LISTBATCHJOBSRESPONSE = DESCRIPTOR.message_types_by_name['ListBatchJobsResponse']
 _BATCHJOBDETAILS = DESCRIPTOR.message_types_by_name['BatchJobDetails']
 _GETBATCHJOBDETAILSREQUEST = DESCRIPTOR.message_types_by_name['GetBatchJobDetailsRequest']
 _GETBATCHJOBDETAILSRESPONSE = DESCRIPTOR.message_types_by_name['GetBatchJobDetailsResponse']
 _BATCHJOBMESSAGE = DESCRIPTOR.message_types_by_name['BatchJobMessage']
 _EXECUTIONREPORTLINE = DESCRIPTOR.message_types_by_name['ExecutionReportLine']
@@ -257,14 +258,21 @@
 BatchJobDeploymentSize = _reflection.GeneratedProtocolMessageType('BatchJobDeploymentSize', (_message.Message,), {
   'DESCRIPTOR' : _BATCHJOBDEPLOYMENTSIZE,
   '__module__' : 'qwak.batch_job.v1.batch_job_service_pb2'
   # @@protoc_insertion_point(class_scope:qwak.batchjob.BatchJobDeploymentSize)
   })
 _sym_db.RegisterMessage(BatchJobDeploymentSize)
 
+BatchJobExecutionSize = _reflection.GeneratedProtocolMessageType('BatchJobExecutionSize', (_message.Message,), {
+  'DESCRIPTOR' : _BATCHJOBEXECUTIONSIZE,
+  '__module__' : 'qwak.batch_job.v1.batch_job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.batchjob.BatchJobExecutionSize)
+  })
+_sym_db.RegisterMessage(BatchJobExecutionSize)
+
 ListBatchJobsRequest = _reflection.GeneratedProtocolMessageType('ListBatchJobsRequest', (_message.Message,), {
   'DESCRIPTOR' : _LISTBATCHJOBSREQUEST,
   '__module__' : 'qwak.batch_job.v1.batch_job_service_pb2'
   # @@protoc_insertion_point(class_scope:qwak.batchjob.ListBatchJobsRequest)
   })
 _sym_db.RegisterMessage(ListBatchJobsRequest)
 
@@ -415,26 +423,38 @@
   DESCRIPTOR._serialized_options = b'\n\031com.qwak.ai.batch.job.apiP\001Z\017./;inferencejob'
   _STARTWARMUPJOBREQUEST.fields_by_name['branch_id']._options = None
   _STARTWARMUPJOBREQUEST.fields_by_name['branch_id']._serialized_options = b'\030\001'
   _CANCELWARMUPJOBREQUEST.fields_by_name['branch_id']._options = None
   _CANCELWARMUPJOBREQUEST.fields_by_name['branch_id']._serialized_options = b'\030\001'
   _STARTBATCHJOBREQUEST.fields_by_name['branch_id']._options = None
   _STARTBATCHJOBREQUEST.fields_by_name['branch_id']._serialized_options = b'\030\001'
+  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._options = None
+  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._serialized_options = b'\030\001'
+  _BATCHJOBDEPLOYMENTSIZE.fields_by_name['cpu']._options = None
+  _BATCHJOBDEPLOYMENTSIZE.fields_by_name['cpu']._serialized_options = b'\030\001'
+  _BATCHJOBDEPLOYMENTSIZE.fields_by_name['memory_amount']._options = None
+  _BATCHJOBDEPLOYMENTSIZE.fields_by_name['memory_amount']._serialized_options = b'\030\001'
+  _BATCHJOBDEPLOYMENTSIZE.fields_by_name['memory_units']._options = None
+  _BATCHJOBDEPLOYMENTSIZE.fields_by_name['memory_units']._serialized_options = b'\030\001'
+  _BATCHJOBDEPLOYMENTSIZE.fields_by_name['gpu_resources']._options = None
+  _BATCHJOBDEPLOYMENTSIZE.fields_by_name['gpu_resources']._serialized_options = b'\030\001'
   _LISTBATCHJOBSREQUEST.fields_by_name['branch_id']._options = None
   _LISTBATCHJOBSREQUEST.fields_by_name['branch_id']._serialized_options = b'\030\001'
+  _BATCHJOBDETAILS.fields_by_name['job_size']._options = None
+  _BATCHJOBDETAILS.fields_by_name['job_size']._serialized_options = b'\030\001'
   _BATCHJOBMESSAGE.fields_by_name['branch_id']._options = None
   _BATCHJOBMESSAGE.fields_by_name['branch_id']._serialized_options = b'\030\001'
-  _INPUTFILETYPE._serialized_start=6342
-  _INPUTFILETYPE._serialized_end=6471
-  _OUTPUTFILETYPE._serialized_start=6474
-  _OUTPUTFILETYPE._serialized_end=6608
-  _BATCHJOBSTATUSMESSAGE._serialized_start=6611
-  _BATCHJOBSTATUSMESSAGE._serialized_end=6880
-  _BATCHTASKSTATUSMESSAGE._serialized_start=6883
-  _BATCHTASKSTATUSMESSAGE._serialized_end=7167
+  _INPUTFILETYPE._serialized_start=6692
+  _INPUTFILETYPE._serialized_end=6821
+  _OUTPUTFILETYPE._serialized_start=6824
+  _OUTPUTFILETYPE._serialized_end=6958
+  _BATCHJOBSTATUSMESSAGE._serialized_start=6961
+  _BATCHJOBSTATUSMESSAGE._serialized_end=7230
+  _BATCHTASKSTATUSMESSAGE._serialized_start=7233
+  _BATCHTASKSTATUSMESSAGE._serialized_end=7517
   _STARTWARMUPJOBREQUEST._serialized_start=246
   _STARTWARMUPJOBREQUEST._serialized_end=426
   _STARTWARMUPJOBRESPONSE._serialized_start=428
   _STARTWARMUPJOBRESPONSE._serialized_end=494
   _CANCELWARMUPJOBREQUEST._serialized_start=496
   _CANCELWARMUPJOBREQUEST._serialized_end=579
   _CANCELWARMUPJOBRESPONSE._serialized_start=581
@@ -472,55 +492,57 @@
   _UPDATEBATCHTASKSSTATUSREQUEST._serialized_start=2913
   _UPDATEBATCHTASKSSTATUSREQUEST._serialized_end=3009
   _UPDATEBATCHTASKSTATUSRESPONSE._serialized_start=3011
   _UPDATEBATCHTASKSTATUSRESPONSE._serialized_end=3084
   _ADVANCEDDEPLOYMENTOPTIONS._serialized_start=3086
   _ADVANCEDDEPLOYMENTOPTIONS._serialized_end=3167
   _BATCHJOBDEPLOYMENTSIZE._serialized_start=3170
-  _BATCHJOBDEPLOYMENTSIZE._serialized_end=3441
-  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._serialized_start=3398
-  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._serialized_end=3441
-  _LISTBATCHJOBSREQUEST._serialized_start=3443
-  _LISTBATCHJOBSREQUEST._serialized_end=3506
-  _LISTBATCHJOBSRESPONSE._serialized_start=3508
-  _LISTBATCHJOBSRESPONSE._serialized_end=3583
-  _BATCHJOBDETAILS._serialized_start=3586
-  _BATCHJOBDETAILS._serialized_end=3871
-  _GETBATCHJOBDETAILSREQUEST._serialized_start=3873
-  _GETBATCHJOBDETAILSREQUEST._serialized_end=3916
-  _GETBATCHJOBDETAILSRESPONSE._serialized_start=3918
-  _GETBATCHJOBDETAILSRESPONSE._serialized_end=4039
-  _BATCHJOBMESSAGE._serialized_start=4042
-  _BATCHJOBMESSAGE._serialized_end=4558
-  _EXECUTIONREPORTLINE._serialized_start=4560
-  _EXECUTIONREPORTLINE._serialized_end=4637
-  _EXECUTIONFILEDETAILS._serialized_start=4640
-  _EXECUTIONFILEDETAILS._serialized_end=4917
-  _TASKEXECUTIONDETAILS._serialized_start=4920
-  _TASKEXECUTIONDETAILS._serialized_end=5150
-  _GETBATCHJOBPRESIGNEDUPLOADURLREQUEST._serialized_start=5152
-  _GETBATCHJOBPRESIGNEDUPLOADURLREQUEST._serialized_end=5252
-  _GETBATCHJOBPRESIGNEDUPLOADURLRESPONSE._serialized_start=5255
-  _GETBATCHJOBPRESIGNEDUPLOADURLRESPONSE._serialized_end=5407
-  _GETBATCHJOBPRESIGNEDDOWNLOADURLREQUEST._serialized_start=5409
-  _GETBATCHJOBPRESIGNEDDOWNLOADURLREQUEST._serialized_end=5465
-  _GETBATCHJOBPRESIGNEDDOWNLOADURLRESPONSE._serialized_start=5467
-  _GETBATCHJOBPRESIGNEDDOWNLOADURLRESPONSE._serialized_end=5564
-  _GETBATCHJOBUPLOADDETAILSREQUEST._serialized_start=5566
-  _GETBATCHJOBUPLOADDETAILSREQUEST._serialized_end=5617
-  _GETBATCHJOBUPLOADDETAILSRESPONSE._serialized_start=5620
-  _GETBATCHJOBUPLOADDETAILSRESPONSE._serialized_end=5800
-  _GETBATCHJOBDOWNLOADDETAILSREQUEST._serialized_start=5802
-  _GETBATCHJOBDOWNLOADDETAILSREQUEST._serialized_end=5853
-  _GETBATCHJOBDOWNLOADDETAILSRESPONSE._serialized_start=5856
-  _GETBATCHJOBDOWNLOADDETAILSRESPONSE._serialized_end=6011
-  _UPDATEDEFAULTPARAMSREQUEST._serialized_start=6014
-  _UPDATEDEFAULTPARAMSREQUEST._serialized_end=6229
-  _UPDATEDEFAULTPARAMSRESPONSE._serialized_start=6231
-  _UPDATEDEFAULTPARAMSRESPONSE._serialized_end=6260
-  _DELETEDEFAULTPARAMSREQUEST._serialized_start=6262
-  _DELETEDEFAULTPARAMSREQUEST._serialized_end=6308
-  _DELETEDEFAULTPARAMSRESPONSE._serialized_start=6310
-  _DELETEDEFAULTPARAMSRESPONSE._serialized_end=6339
-  _BATCHJOBMANAGEMENTSERVICE._serialized_start=7170
-  _BATCHJOBMANAGEMENTSERVICE._serialized_end=8867
+  _BATCHJOBDEPLOYMENTSIZE._serialized_end=3559
+  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._serialized_start=3512
+  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._serialized_end=3559
+  _BATCHJOBEXECUTIONSIZE._serialized_start=3562
+  _BATCHJOBEXECUTIONSIZE._serialized_end=3715
+  _LISTBATCHJOBSREQUEST._serialized_start=3717
+  _LISTBATCHJOBSREQUEST._serialized_end=3780
+  _LISTBATCHJOBSRESPONSE._serialized_start=3782
+  _LISTBATCHJOBSRESPONSE._serialized_end=3857
+  _BATCHJOBDETAILS._serialized_start=3860
+  _BATCHJOBDETAILS._serialized_end=4221
+  _GETBATCHJOBDETAILSREQUEST._serialized_start=4223
+  _GETBATCHJOBDETAILSREQUEST._serialized_end=4266
+  _GETBATCHJOBDETAILSRESPONSE._serialized_start=4268
+  _GETBATCHJOBDETAILSRESPONSE._serialized_end=4389
+  _BATCHJOBMESSAGE._serialized_start=4392
+  _BATCHJOBMESSAGE._serialized_end=4908
+  _EXECUTIONREPORTLINE._serialized_start=4910
+  _EXECUTIONREPORTLINE._serialized_end=4987
+  _EXECUTIONFILEDETAILS._serialized_start=4990
+  _EXECUTIONFILEDETAILS._serialized_end=5267
+  _TASKEXECUTIONDETAILS._serialized_start=5270
+  _TASKEXECUTIONDETAILS._serialized_end=5500
+  _GETBATCHJOBPRESIGNEDUPLOADURLREQUEST._serialized_start=5502
+  _GETBATCHJOBPRESIGNEDUPLOADURLREQUEST._serialized_end=5602
+  _GETBATCHJOBPRESIGNEDUPLOADURLRESPONSE._serialized_start=5605
+  _GETBATCHJOBPRESIGNEDUPLOADURLRESPONSE._serialized_end=5757
+  _GETBATCHJOBPRESIGNEDDOWNLOADURLREQUEST._serialized_start=5759
+  _GETBATCHJOBPRESIGNEDDOWNLOADURLREQUEST._serialized_end=5815
+  _GETBATCHJOBPRESIGNEDDOWNLOADURLRESPONSE._serialized_start=5817
+  _GETBATCHJOBPRESIGNEDDOWNLOADURLRESPONSE._serialized_end=5914
+  _GETBATCHJOBUPLOADDETAILSREQUEST._serialized_start=5916
+  _GETBATCHJOBUPLOADDETAILSREQUEST._serialized_end=5967
+  _GETBATCHJOBUPLOADDETAILSRESPONSE._serialized_start=5970
+  _GETBATCHJOBUPLOADDETAILSRESPONSE._serialized_end=6150
+  _GETBATCHJOBDOWNLOADDETAILSREQUEST._serialized_start=6152
+  _GETBATCHJOBDOWNLOADDETAILSREQUEST._serialized_end=6203
+  _GETBATCHJOBDOWNLOADDETAILSRESPONSE._serialized_start=6206
+  _GETBATCHJOBDOWNLOADDETAILSRESPONSE._serialized_end=6361
+  _UPDATEDEFAULTPARAMSREQUEST._serialized_start=6364
+  _UPDATEDEFAULTPARAMSREQUEST._serialized_end=6579
+  _UPDATEDEFAULTPARAMSRESPONSE._serialized_start=6581
+  _UPDATEDEFAULTPARAMSRESPONSE._serialized_end=6610
+  _DELETEDEFAULTPARAMSREQUEST._serialized_start=6612
+  _DELETEDEFAULTPARAMSREQUEST._serialized_end=6658
+  _DELETEDEFAULTPARAMSRESPONSE._serialized_start=6660
+  _DELETEDEFAULTPARAMSRESPONSE._serialized_end=6689
+  _BATCHJOBMANAGEMENTSERVICE._serialized_start=7520
+  _BATCHJOBMANAGEMENTSERVICE._serialized_end=9217
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -688,39 +688,69 @@
     GIB: BatchJobDeploymentSize.MemoryUnit.ValueType  # 2
 
     NUMBER_OF_PODS_FIELD_NUMBER: builtins.int
     CPU_FIELD_NUMBER: builtins.int
     MEMORY_AMOUNT_FIELD_NUMBER: builtins.int
     MEMORY_UNITS_FIELD_NUMBER: builtins.int
     GPU_RESOURCES_FIELD_NUMBER: builtins.int
+    CLIENT_POD_COMPUTE_RESOURCES_FIELD_NUMBER: builtins.int
     number_of_pods: builtins.int
     """Number of pods to deploy"""
     cpu: builtins.float
     """Cpu"""
     memory_amount: builtins.int
     """Amount of memory"""
     memory_units: global___BatchJobDeploymentSize.MemoryUnit.ValueType
     """Units type of memory"""
     @property
     def gpu_resources(self) -> qwak.user_application.common.v0.resources_pb2.GpuResources:
         """Optional GPU resources for batch"""
+    @property
+    def client_pod_compute_resources(self) -> qwak.user_application.common.v0.resources_pb2.ClientPodComputeResources:
+        """Client Compute Resources"""
     def __init__(
         self,
         *,
         number_of_pods: builtins.int = ...,
         cpu: builtins.float = ...,
         memory_amount: builtins.int = ...,
         memory_units: global___BatchJobDeploymentSize.MemoryUnit.ValueType = ...,
         gpu_resources: qwak.user_application.common.v0.resources_pb2.GpuResources | None = ...,
+        client_pod_compute_resources: qwak.user_application.common.v0.resources_pb2.ClientPodComputeResources | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["gpu_resources", b"gpu_resources"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cpu", b"cpu", "gpu_resources", b"gpu_resources", "memory_amount", b"memory_amount", "memory_units", b"memory_units", "number_of_pods", b"number_of_pods"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["client_pod_compute_resources", b"client_pod_compute_resources", "gpu_resources", b"gpu_resources"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["client_pod_compute_resources", b"client_pod_compute_resources", "cpu", b"cpu", "gpu_resources", b"gpu_resources", "memory_amount", b"memory_amount", "memory_units", b"memory_units", "number_of_pods", b"number_of_pods"]) -> None: ...
 
 global___BatchJobDeploymentSize = BatchJobDeploymentSize
 
+class BatchJobExecutionSize(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    NUMBER_OF_PODS_FIELD_NUMBER: builtins.int
+    POD_COMPUTE_RESOURCES_FIELD_NUMBER: builtins.int
+    TEMPLATE_ID_FIELD_NUMBER: builtins.int
+    number_of_pods: builtins.int
+    """Number of pods in execution"""
+    @property
+    def pod_compute_resources(self) -> qwak.user_application.common.v0.resources_pb2.PodComputeResources:
+        """Resources"""
+    template_id: builtins.str
+    """Template id used"""
+    def __init__(
+        self,
+        *,
+        number_of_pods: builtins.int = ...,
+        pod_compute_resources: qwak.user_application.common.v0.resources_pb2.PodComputeResources | None = ...,
+        template_id: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["pod_compute_resources", b"pod_compute_resources"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["number_of_pods", b"number_of_pods", "pod_compute_resources", b"pod_compute_resources", "template_id", b"template_id"]) -> None: ...
+
+global___BatchJobExecutionSize = BatchJobExecutionSize
+
 class ListBatchJobsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MODEL_ID_FIELD_NUMBER: builtins.int
     BRANCH_ID_FIELD_NUMBER: builtins.int
     model_id: builtins.str
     """The model ID to get the list of batch jobs for"""
@@ -758,14 +788,15 @@
     BUILD_ID_FIELD_NUMBER: builtins.int
     JOB_ID_FIELD_NUMBER: builtins.int
     JOB_STATUS_FIELD_NUMBER: builtins.int
     START_TIME_FIELD_NUMBER: builtins.int
     END_TIME_FIELD_NUMBER: builtins.int
     FAILURE_MESSAGE_FIELD_NUMBER: builtins.int
     JOB_SIZE_FIELD_NUMBER: builtins.int
+    BATCH_JOB_EXECUTION_SIZE_FIELD_NUMBER: builtins.int
     build_id: builtins.str
     """The build id used in the batch job"""
     job_id: builtins.str
     """The batch job id"""
     job_status: global___BatchJobStatusMessage.ValueType
     """The batch job status"""
     @property
@@ -775,27 +806,31 @@
     def end_time(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """The end time for of the batch job"""
     failure_message: builtins.str
     """The failure message of the batch job in case that failed"""
     @property
     def job_size(self) -> global___BatchJobDeploymentSize:
         """The batch job resources size"""
+    @property
+    def batch_job_execution_size(self) -> global___BatchJobExecutionSize:
+        """The batch job resources size"""
     def __init__(
         self,
         *,
         build_id: builtins.str = ...,
         job_id: builtins.str = ...,
         job_status: global___BatchJobStatusMessage.ValueType = ...,
         start_time: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         end_time: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         failure_message: builtins.str = ...,
         job_size: global___BatchJobDeploymentSize | None = ...,
+        batch_job_execution_size: global___BatchJobExecutionSize | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["end_time", b"end_time", "job_size", b"job_size", "start_time", b"start_time"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["build_id", b"build_id", "end_time", b"end_time", "failure_message", b"failure_message", "job_id", b"job_id", "job_size", b"job_size", "job_status", b"job_status", "start_time", b"start_time"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["batch_job_execution_size", b"batch_job_execution_size", "end_time", b"end_time", "job_size", b"job_size", "start_time", b"start_time"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["batch_job_execution_size", b"batch_job_execution_size", "build_id", b"build_id", "end_time", b"end_time", "failure_message", b"failure_message", "job_id", b"job_id", "job_size", b"job_size", "job_status", b"job_status", "start_time", b"start_time"]) -> None: ...
 
 global___BatchJobDetails = BatchJobDetails
 
 class GetBatchJobDetailsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_ID_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.95/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.95/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/pyproject.toml` & `qwak_core-0.0.95/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.94"
+version = "0.0.95"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.94/qwak/automations/__init__.py` & `qwak_core-0.0.95/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/automations/automation_executions.py` & `qwak_core-0.0.95/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/automations/automations.py` & `qwak_core-0.0.95/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.95/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.95/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/automations/common.py` & `qwak_core-0.0.95/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.95/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.95/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.95/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.95/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.95/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/alert_management/client.py` & `qwak_core-0.0.95/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/analytics/client.py` & `qwak_core-0.0.95/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/audience/client.py` & `qwak_core-0.0.95/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/automation_management/client.py` & `qwak_core-0.0.95/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.95/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.95/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.95/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.95/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/build_management/client.py` & `qwak_core-0.0.95/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.95/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.95/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/deployment/client.py` & `qwak_core-0.0.95/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.95/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.95/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.95/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.95/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/instance_template/client.py` & `qwak_core-0.0.95/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.95/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/logging_client/client.py` & `qwak_core-0.0.95/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/model_management/client.py` & `qwak_core-0.0.95/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/project/client.py` & `qwak_core-0.0.95/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/secret_service/client.py` & `qwak_core-0.0.95/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.95/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.95/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.95/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.95/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.95/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.95/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.95/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.95/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.95/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.95/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.95/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.95/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.95/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.95/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/offline/client.py` & `qwak_core-0.0.95/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/feature_store/online/client.py` & `qwak_core-0.0.95/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/inner/const.py` & `qwak_core-0.0.95/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.95/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.95/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.95/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.95/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/inner/singleton_meta.py` & `qwak_core-0.0.95/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/inner/tool/auth.py` & `qwak_core-0.0.95/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.95/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.95/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.95/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.95/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/adapters/__init__.py` & `qwak_core-0.0.95/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.95/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.95/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.95/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.95/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.95/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/base.py` & `qwak_core-0.0.95/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/decorators/api.py` & `qwak_core-0.0.95/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.95/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/experiment_tracking.py` & `qwak_core-0.0.95/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/schema.py` & `qwak_core-0.0.95/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/schema_entities.py` & `qwak_core-0.0.95/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.95/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.95/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.95/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.95/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.95/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.95/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.95/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.95/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.95/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.95/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/qwak_client/client.py` & `qwak_core-0.0.95/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.95/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/qwak_client/models/model.py` & `qwak_core-0.0.95/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.95/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.95/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/tools/logger/logger.py` & `qwak_core-0.0.95/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak/tools/logger/logging.yml` & `qwak_core-0.0.95/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.95/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/qwak_services_mock/services_mock.py` & `qwak_core-0.0.95/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.94/setup.py` & `qwak_core-0.0.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.94',
+    'version': '0.0.95',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.94/PKG-INFO` & `qwak_core-0.0.95/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.94
+Version: 0.0.95
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

