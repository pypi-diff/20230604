# Comparing `tmp/qwak_core-0.0.93.tar.gz` & `tmp/qwak_core-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.93.tar", max compression
+gzip compressed data, was "qwak_core-0.0.94.tar", max compression
```

## Comparing `qwak_core-0.0.93.tar` & `qwak_core-0.0.94.tar`

### file list

```diff
@@ -1,588 +1,588 @@
--rw-r--r--   0        0        0      264 2023-06-01 09:07:05.116383 qwak_core-0.0.93/README.md
--rw-r--r--   0        0        0        0 2023-06-01 09:08:57.349039 qwak_core-0.0.93/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-06-01 09:08:57.381039 qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-06-01 09:08:34.124915 qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.381039 qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-06-01 09:08:57.377039 qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-06-01 09:08:33.732912 qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.377039 qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-06-01 09:08:57.381039 qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-06-01 09:08:33.928913 qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.381039 qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-06-01 09:08:57.369039 qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-06-01 09:08:33.140909 qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-06-01 09:08:57.373039 qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-06-01 09:08:57.373039 qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-06-01 09:08:33.348910 qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.373039 qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4901 2023-06-01 09:08:57.373039 qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5995 2023-06-01 09:08:33.540911 qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.377039 qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-06-01 09:08:57.349039 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-06-01 09:08:32.932908 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-06-01 09:08:57.357039 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5707 2023-06-01 09:08:57.357039 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8170 2023-06-01 09:08:34.360916 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.357039 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-06-01 09:08:57.361039 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-06-01 09:08:34.768918 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.365039 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-06-01 09:08:57.365039 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-06-01 09:08:35.004920 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-06-01 09:08:57.365039 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-06-01 09:08:57.361039 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-06-01 09:08:34.564917 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.361039 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-06-01 09:08:57.369039 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-06-01 09:08:35.208921 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.369039 qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-06-01 09:08:57.413040 qwak_core-0.0.93/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-06-01 09:08:37.960937 qwak_core-0.0.93/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.413040 qwak_core-0.0.93/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-06-01 09:08:57.417040 qwak_core-0.0.93/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-06-01 09:08:38.176938 qwak_core-0.0.93/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-06-01 09:08:57.417040 qwak_core-0.0.93/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-06-01 09:08:57.497040 qwak_core-0.0.93/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-06-01 09:08:44.708977 qwak_core-0.0.93/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.497040 qwak_core-0.0.93/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-06-01 09:08:57.497040 qwak_core-0.0.93/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-06-01 09:08:44.908978 qwak_core-0.0.93/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-06-01 09:08:57.501040 qwak_core-0.0.93/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-06-01 09:08:57.505040 qwak_core-0.0.93/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-06-01 09:08:45.948984 qwak_core-0.0.93/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-06-01 09:08:57.505040 qwak_core-0.0.93/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-06-01 09:08:57.501040 qwak_core-0.0.93/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-06-01 09:08:45.748983 qwak_core-0.0.93/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.501040 qwak_core-0.0.93/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-06-01 09:08:57.505040 qwak_core-0.0.93/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-06-01 09:08:46.144985 qwak_core-0.0.93/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.509040 qwak_core-0.0.93/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-06-01 09:08:57.509040 qwak_core-0.0.93/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-06-01 09:08:46.348986 qwak_core-0.0.93/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-06-01 09:08:57.509040 qwak_core-0.0.93/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-06-01 09:08:57.617041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-06-01 09:08:54.877026 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.617041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-06-01 09:08:57.613041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-06-01 09:08:54.477025 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.613041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-06-01 09:08:57.613041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-06-01 09:08:54.673025 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.617041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-06-01 09:08:57.609041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-06-01 09:08:54.081023 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-06-01 09:08:57.609041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-06-01 09:08:57.609041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-06-01 09:08:54.281024 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.609041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-06-01 09:08:57.625041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-06-01 09:08:55.449029 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.625041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-06-01 09:08:57.621041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-06-01 09:08:55.257028 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.621041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-06-01 09:08:57.617041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-06-01 09:08:55.069027 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.621041 qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-06-01 09:08:57.605041 qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-06-01 09:08:53.865022 qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.605041 qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-06-01 09:08:57.601041 qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-06-01 09:08:53.449020 qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.601041 qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-06-01 09:08:57.601041 qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-06-01 09:08:53.669021 qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-06-01 09:08:57.605041 qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    20255 2023-06-01 09:08:57.537040 qwak_core-0.0.93/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    17495 2023-06-01 09:08:48.420998 qwak_core-0.0.93/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    20359 2023-06-01 09:08:57.537040 qwak_core-0.0.93/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-06-01 09:08:57.537040 qwak_core-0.0.93/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-06-01 09:08:48.224997 qwak_core-0.0.93/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.537040 qwak_core-0.0.93/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11691 2023-06-01 09:08:57.525040 qwak_core-0.0.93/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18850 2023-06-01 09:08:47.800995 qwak_core-0.0.93/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.525040 qwak_core-0.0.93/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-06-01 09:08:57.529040 qwak_core-0.0.93/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-06-01 09:08:48.004996 qwak_core-0.0.93/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.529040 qwak_core-0.0.93/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-06-01 09:08:57.529040 qwak_core-0.0.93/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-06-01 09:08:48.616999 qwak_core-0.0.93/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-06-01 09:08:57.533040 qwak_core-0.0.93/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38290 2023-06-01 09:08:57.533040 qwak_core-0.0.93/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52702 2023-06-01 09:08:49.041001 qwak_core-0.0.93/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-06-01 09:08:57.533040 qwak_core-0.0.93/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-06-01 09:08:57.545040 qwak_core-0.0.93/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-06-01 09:08:49.449003 qwak_core-0.0.93/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.545040 qwak_core-0.0.93/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-06-01 09:08:57.549040 qwak_core-0.0.93/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-06-01 09:08:49.657004 qwak_core-0.0.93/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-06-01 09:08:57.549040 qwak_core-0.0.93/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-06-01 09:08:57.517040 qwak_core-0.0.93/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-06-01 09:08:47.184991 qwak_core-0.0.93/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.521040 qwak_core-0.0.93/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-06-01 09:08:57.521040 qwak_core-0.0.93/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-06-01 09:08:47.392992 qwak_core-0.0.93/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-06-01 09:08:57.521040 qwak_core-0.0.93/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-06-01 09:08:57.513040 qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-06-01 09:08:46.764989 qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.513040 qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-06-01 09:08:57.513040 qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-06-01 09:08:46.564988 qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.513040 qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-06-01 09:08:57.517040 qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-06-01 09:08:46.976990 qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-06-01 09:08:57.517040 qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-06-01 09:08:57.401039 qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-06-01 09:08:36.980931 qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.405040 qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-06-01 09:08:57.405040 qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-06-01 09:08:37.176932 qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.405040 qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-06-01 09:08:57.405040 qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-06-01 09:08:37.372934 qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-06-01 09:08:57.409040 qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-06-01 09:08:57.473040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-06-01 09:08:43.520970 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.473040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-06-01 09:08:57.469040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-06-01 09:08:43.316969 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-06-01 09:08:57.473040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2023-06-01 09:08:57.441040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2023-06-01 09:08:40.816954 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.445040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2023-06-01 09:08:57.441040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2023-06-01 09:08:40.592953 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.441040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-06-01 09:08:57.433040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-06-01 09:08:39.920949 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.433040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-06-01 09:08:57.437040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-06-01 09:08:40.372951 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-06-01 09:08:57.437040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-06-01 09:08:57.445040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-06-01 09:08:41.068955 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.445040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-06-01 09:08:57.445040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-06-01 09:08:41.308957 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-06-01 09:08:57.449040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25269 2023-06-01 09:08:57.437040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37664 2023-06-01 09:08:40.140950 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.437040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-06-01 09:08:57.449040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-06-01 09:08:41.540958 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.449040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    10202 2023-06-01 09:08:57.453040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py
--rw-r--r--   0        0        0    16565 2023-06-01 09:08:42.008961 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.457040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2_grpc.py
--rw-r--r--   0        0        0     3559 2023-06-01 09:08:57.457040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py
--rw-r--r--   0        0        0     1759 2023-06-01 09:08:42.228962 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi
--rw-r--r--   0        0        0     3608 2023-06-01 09:08:57.457040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0    10604 2023-06-01 09:08:57.453040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    13410 2023-06-01 09:08:41.780959 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.453040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-06-01 09:08:57.477040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-06-01 09:08:56.841036 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.477040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-06-01 09:08:57.477040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-06-01 09:08:57.045037 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-06-01 09:08:57.481040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-06-01 09:08:57.481040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-06-01 09:08:44.116973 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.481040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-06-01 09:08:57.485040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-06-01 09:08:44.316974 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-06-01 09:08:57.485040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-06-01 09:08:57.485040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-06-01 09:08:44.512976 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.489040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-06-01 09:08:57.493040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-06-01 09:08:45.344980 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.493040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-06-01 09:08:57.489040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-06-01 09:08:45.132979 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-06-01 09:08:57.489040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-06-01 09:08:57.493040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-06-01 09:08:45.552981 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.497040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-06-01 09:08:57.457040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-06-01 09:08:42.456963 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.461040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-06-01 09:08:57.461040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-06-01 09:08:42.684965 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.465040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-06-01 09:08:57.465040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-06-01 09:08:42.916966 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-06-01 09:08:57.465040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-06-01 09:08:57.469040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-06-01 09:08:43.116967 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.469040 qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-06-01 09:08:57.625041 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-06-01 09:08:55.637030 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.625041 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-06-01 09:08:57.629041 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-06-01 09:08:55.825030 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-06-01 09:08:57.629041 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-06-01 09:08:57.629041 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-06-01 09:08:56.017031 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.633041 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-06-01 09:08:57.633041 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-06-01 09:08:56.217033 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-06-01 09:08:57.633041 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-06-01 09:08:57.633041 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-06-01 09:08:56.433034 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-06-01 09:08:57.637041 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-06-01 09:08:57.637041 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-06-01 09:08:56.637035 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.637041 qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-06-01 09:08:57.549040 qwak_core-0.0.93/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-06-01 09:08:49.857005 qwak_core-0.0.93/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.549040 qwak_core-0.0.93/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-06-01 09:08:57.553040 qwak_core-0.0.93/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-06-01 09:08:50.057006 qwak_core-0.0.93/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-06-01 09:08:57.553040 qwak_core-0.0.93/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-06-01 09:08:57.421040 qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-06-01 09:08:39.044943 qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.421040 qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-06-01 09:08:57.425040 qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-06-01 09:08:39.264945 qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.425040 qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-06-01 09:08:57.425040 qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-06-01 09:08:39.476946 qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-06-01 09:08:57.429040 qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-06-01 09:08:57.429040 qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-06-01 09:08:39.700947 qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.433040 qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-06-01 09:08:57.525040 qwak_core-0.0.93/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-06-01 09:08:47.592994 qwak_core-0.0.93/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-06-01 09:08:57.525040 qwak_core-0.0.93/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-06-01 09:08:57.553040 qwak_core-0.0.93/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-06-01 09:08:50.253006 qwak_core-0.0.93/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.557041 qwak_core-0.0.93/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-06-01 09:08:57.557041 qwak_core-0.0.93/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-06-01 09:08:50.449007 qwak_core-0.0.93/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-06-01 09:08:57.557041 qwak_core-0.0.93/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-06-01 09:08:57.573041 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-06-01 09:08:51.629012 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.573041 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-06-01 09:08:57.577041 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-06-01 09:08:51.821013 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.577041 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-06-01 09:08:57.577041 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-06-01 09:08:52.021014 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.581040 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-06-01 09:08:57.581040 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-06-01 09:08:52.217015 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.581040 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-06-01 09:08:57.585041 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-06-01 09:08:52.425016 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.585041 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-06-01 09:08:57.589041 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-06-01 09:08:52.645017 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-06-01 09:08:57.593041 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-06-01 09:08:57.593041 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-06-01 09:08:52.845018 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.593041 qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-06-01 09:08:57.561040 qwak_core-0.0.93/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-06-01 09:08:50.857009 qwak_core-0.0.93/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.565040 qwak_core-0.0.93/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-06-01 09:08:57.569041 qwak_core-0.0.93/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-06-01 09:08:51.433011 qwak_core-0.0.93/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.573041 qwak_core-0.0.93/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-06-01 09:08:57.565040 qwak_core-0.0.93/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-06-01 09:08:51.049010 qwak_core-0.0.93/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-06-01 09:08:57.565040 qwak_core-0.0.93/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-06-01 09:08:57.569041 qwak_core-0.0.93/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-06-01 09:08:51.237011 qwak_core-0.0.93/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.569041 qwak_core-0.0.93/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-06-01 09:08:57.541040 qwak_core-0.0.93/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-06-01 09:08:49.253002 qwak_core-0.0.93/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-06-01 09:08:57.545040 qwak_core-0.0.93/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-06-01 09:08:57.397040 qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-06-01 09:08:38.612941 qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-06-01 09:08:57.397040 qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-06-01 09:08:57.397040 qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-06-01 09:08:38.396940 qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.397040 qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-06-01 09:08:57.401039 qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-06-01 09:08:38.828942 qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-06-01 09:08:57.401039 qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-06-01 09:08:57.541040 qwak_core-0.0.93/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-06-01 09:08:48.821000 qwak_core-0.0.93/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-06-01 09:08:57.541040 qwak_core-0.0.93/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-06-01 09:08:57.561040 qwak_core-0.0.93/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-06-01 09:08:50.649008 qwak_core-0.0.93/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-06-01 09:08:57.561040 qwak_core-0.0.93/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-06-01 09:08:57.393040 qwak_core-0.0.93/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-06-01 09:08:36.200927 qwak_core-0.0.93/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.393040 qwak_core-0.0.93/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-06-01 09:08:57.389039 qwak_core-0.0.93/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-06-01 09:08:36.008926 qwak_core-0.0.93/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-06-01 09:08:57.393040 qwak_core-0.0.93/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-06-01 09:08:57.385039 qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-06-01 09:08:35.408922 qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.385039 qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-06-01 09:08:57.385039 qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-06-01 09:08:35.608923 qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.389039 qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-06-01 09:08:57.389039 qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-06-01 09:08:35.808925 qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-06-01 09:08:57.389039 qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-06-01 09:08:57.597041 qwak_core-0.0.93/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-06-01 09:08:53.245019 qwak_core-0.0.93/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-06-01 09:08:57.597041 qwak_core-0.0.93/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-06-01 09:08:57.597041 qwak_core-0.0.93/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-06-01 09:08:53.049018 qwak_core-0.0.93/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.597041 qwak_core-0.0.93/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    10851 2023-06-01 09:08:57.409040 qwak_core-0.0.93/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    13974 2023-06-01 09:08:37.572935 qwak_core-0.0.93/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.409040 qwak_core-0.0.93/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3044 2023-06-01 09:08:57.413040 qwak_core-0.0.93/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2641 2023-06-01 09:08:37.764936 qwak_core-0.0.93/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-01 09:08:57.413040 qwak_core-0.0.93/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-06-01 09:08:59.477052 qwak_core-0.0.93/pyproject.toml
--rw-r--r--   0        0        0      447 2023-06-01 09:08:59.477052 qwak_core-0.0.93/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-06-01 09:07:05.116383 qwak_core-0.0.93/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    15319 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-06-01 09:07:05.120384 qwak_core-0.0.93/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-06-01 09:07:05.124384 qwak_core-0.0.93/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.93/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.93/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-06-04 14:33:29.196169 qwak_core-0.0.94/README.md
+-rw-r--r--   0        0        0        0 2023-06-04 14:35:11.845088 qwak_core-0.0.94/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-06-04 14:35:11.869089 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-06-04 14:34:51.600919 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.869089 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-06-04 14:35:11.865089 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-06-04 14:34:51.236916 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.865089 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-06-04 14:35:11.865089 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-06-04 14:34:51.424918 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.865089 qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-06-04 14:35:11.857088 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-06-04 14:34:50.712912 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-06-04 14:35:11.857088 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-06-04 14:35:11.861089 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-06-04 14:34:50.884913 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.861089 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4901 2023-06-04 14:35:11.861089 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5995 2023-06-04 14:34:51.060915 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.861089 qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-06-04 14:35:11.845088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-06-04 14:34:50.532910 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-06-04 14:35:11.845088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5707 2023-06-04 14:35:11.849089 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8170 2023-06-04 14:34:51.780920 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.849089 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-06-04 14:35:11.853088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-06-04 14:34:52.132923 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.853088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-06-04 14:35:11.853088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-06-04 14:34:52.308925 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-06-04 14:35:11.853088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-06-04 14:35:11.849089 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-06-04 14:34:51.956922 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.849089 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-06-04 14:35:11.857088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-06-04 14:34:52.492926 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.857088 qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-06-04 14:35:11.897089 qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-06-04 14:34:54.972947 qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.897089 qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-06-04 14:35:11.897089 qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-06-04 14:34:55.152948 qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-06-04 14:35:11.897089 qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-06-04 14:35:11.965089 qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-06-04 14:35:00.584994 qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.969089 qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-06-04 14:35:11.969089 qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-06-04 14:35:00.768995 qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-06-04 14:35:11.969089 qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-06-04 14:35:11.973089 qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-06-04 14:35:01.705003 qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-06-04 14:35:11.973089 qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-06-04 14:35:11.969089 qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-06-04 14:35:01.525002 qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.973089 qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-06-04 14:35:11.973089 qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-06-04 14:35:01.881005 qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.977089 qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-06-04 14:35:11.977089 qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-06-04 14:35:02.057006 qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-06-04 14:35:11.977089 qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-06-04 14:35:12.061090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-06-04 14:35:09.625070 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.061090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-06-04 14:35:12.057090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-06-04 14:35:09.265067 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.057090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-06-04 14:35:12.061090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-06-04 14:35:09.441069 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.061090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-06-04 14:35:12.053090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-06-04 14:35:08.905064 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-06-04 14:35:12.053090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-06-04 14:35:12.057090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-06-04 14:35:09.089066 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.057090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-06-04 14:35:12.069090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-06-04 14:35:10.153075 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.069090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-06-04 14:35:12.065090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-06-04 14:35:09.981073 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.065090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-06-04 14:35:12.065090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-06-04 14:35:09.801072 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.065090 qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-06-04 14:35:12.053090 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-06-04 14:35:08.721063 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.053090 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-06-04 14:35:12.049090 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-06-04 14:35:08.353060 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.049090 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-06-04 14:35:12.049090 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-06-04 14:35:08.541061 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-06-04 14:35:12.049090 qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20255 2023-06-04 14:35:12.001089 qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    17495 2023-06-04 14:35:03.861022 qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-06-04 14:35:12.001089 qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-06-04 14:35:11.997089 qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-06-04 14:35:03.677020 qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.001089 qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11691 2023-06-04 14:35:11.989089 qwak_core-0.0.94/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18850 2023-06-04 14:35:03.325017 qwak_core-0.0.94/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.993089 qwak_core-0.0.94/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-06-04 14:35:11.993089 qwak_core-0.0.94/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-06-04 14:35:03.497018 qwak_core-0.0.94/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.993089 qwak_core-0.0.94/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-06-04 14:35:11.993089 qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-06-04 14:35:04.037023 qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-06-04 14:35:11.997089 qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38290 2023-06-04 14:35:11.997089 qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52702 2023-06-04 14:35:04.429026 qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-06-04 14:35:11.997089 qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-06-04 14:35:12.009090 qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-06-04 14:35:04.801030 qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.009090 qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-06-04 14:35:12.009090 qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-06-04 14:35:04.977031 qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-06-04 14:35:12.009090 qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-06-04 14:35:11.985089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-06-04 14:35:02.793012 qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.985089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-06-04 14:35:11.985089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-06-04 14:35:02.969014 qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-06-04 14:35:11.989089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-06-04 14:35:11.981089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-06-04 14:35:02.429009 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.981089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-06-04 14:35:11.977089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-06-04 14:35:02.245008 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.981089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-06-04 14:35:11.981089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-06-04 14:35:02.617011 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-06-04 14:35:11.985089 qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-06-04 14:35:11.885089 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-06-04 14:34:54.084939 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.885089 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-06-04 14:35:11.889089 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-06-04 14:34:54.260941 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.889089 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-06-04 14:35:11.889089 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-06-04 14:34:54.444942 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-06-04 14:35:11.889089 qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-06-04 14:35:11.949089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-06-04 14:34:59.528985 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.949089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-06-04 14:35:11.945089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-06-04 14:34:59.348983 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-06-04 14:35:11.945089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2023-06-04 14:35:11.925089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2023-06-04 14:34:57.408967 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.925089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2023-06-04 14:35:11.921089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2023-06-04 14:34:57.232965 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.921089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-06-04 14:35:11.917089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-06-04 14:34:56.684961 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.917089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-06-04 14:35:11.921089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-06-04 14:34:57.056964 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-06-04 14:35:11.921089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-06-04 14:35:11.925089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-06-04 14:34:57.584968 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.925089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-06-04 14:35:11.929089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-06-04 14:34:57.760970 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-06-04 14:35:11.929089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25269 2023-06-04 14:35:11.917089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37664 2023-06-04 14:34:56.868962 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.917089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-06-04 14:35:11.929089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-06-04 14:34:57.932971 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.929089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    10202 2023-06-04 14:35:11.933089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py
+-rw-r--r--   0        0        0    16565 2023-06-04 14:34:58.284974 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.933089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     3559 2023-06-04 14:35:11.937089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py
+-rw-r--r--   0        0        0     1759 2023-06-04 14:34:58.460976 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi
+-rw-r--r--   0        0        0     3608 2023-06-04 14:35:11.937089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10604 2023-06-04 14:35:11.933089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    13410 2023-06-04 14:34:58.108973 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.933089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-06-04 14:35:11.949089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-06-04 14:35:11.409085 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.949089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-06-04 14:35:11.953089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-06-04 14:35:11.593087 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-06-04 14:35:11.953089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-06-04 14:35:11.953089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-06-04 14:35:00.056989 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.953089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-06-04 14:35:11.957089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-06-04 14:35:00.232991 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-06-04 14:35:11.957089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-06-04 14:35:11.957089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-06-04 14:35:00.408992 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.961089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-06-04 14:35:11.961089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-06-04 14:35:01.132998 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.965089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-06-04 14:35:11.961089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-06-04 14:35:00.948997 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-06-04 14:35:11.961089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-06-04 14:35:11.965089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-06-04 14:35:01.345000 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.965089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-06-04 14:35:11.937089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-06-04 14:34:58.640977 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.937089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-06-04 14:35:11.941089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-06-04 14:34:58.816979 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.941089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-06-04 14:35:11.941089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-06-04 14:34:58.996980 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-06-04 14:35:11.941089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-06-04 14:35:11.945089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-06-04 14:34:59.172982 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.945089 qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-06-04 14:35:12.069090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-06-04 14:35:10.329076 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.069090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-06-04 14:35:12.073090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-06-04 14:35:10.505078 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-06-04 14:35:12.073090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-06-04 14:35:12.073090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-06-04 14:35:10.681079 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.073090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-06-04 14:35:12.077090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-06-04 14:35:10.865081 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-06-04 14:35:12.077090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-06-04 14:35:12.077090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-06-04 14:35:11.049082 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-06-04 14:35:12.081090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-06-04 14:35:12.081090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-06-04 14:35:11.225084 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.081090 qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-06-04 14:35:12.013090 qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-06-04 14:35:05.153032 qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.013090 qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-06-04 14:35:12.013090 qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-06-04 14:35:05.325034 qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-06-04 14:35:12.013090 qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-06-04 14:35:11.901089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-06-04 14:34:55.964955 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.905089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-06-04 14:35:11.905089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-06-04 14:34:56.140956 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.905089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-06-04 14:35:11.909089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-06-04 14:34:56.324958 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-06-04 14:35:11.909089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-06-04 14:35:11.913089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-06-04 14:34:56.500959 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.913089 qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-06-04 14:35:11.989089 qwak_core-0.0.94/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-06-04 14:35:03.145015 qwak_core-0.0.94/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-06-04 14:35:11.989089 qwak_core-0.0.94/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-06-04 14:35:12.017089 qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-06-04 14:35:05.501035 qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.017089 qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-06-04 14:35:12.017089 qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-06-04 14:35:05.677037 qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-06-04 14:35:12.017089 qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-06-04 14:35:12.029090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-06-04 14:35:06.733046 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.029090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-06-04 14:35:12.033090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-06-04 14:35:06.917047 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.033090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-06-04 14:35:12.033090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-06-04 14:35:07.097049 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.033090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-06-04 14:35:12.037090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-06-04 14:35:07.277050 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.037090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-06-04 14:35:12.037090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-06-04 14:35:07.457052 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.037090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-06-04 14:35:12.041090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-06-04 14:35:07.653054 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-06-04 14:35:12.041090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-06-04 14:35:12.041090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-06-04 14:35:07.829055 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.041090 qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-06-04 14:35:12.021090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-06-04 14:35:06.029040 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.021090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-06-04 14:35:12.029090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-06-04 14:35:06.557044 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.029090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-06-04 14:35:12.025090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-06-04 14:35:06.205041 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-06-04 14:35:12.025090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-06-04 14:35:12.025090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-06-04 14:35:06.385043 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.025090 qwak_core-0.0.94/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-06-04 14:35:12.005089 qwak_core-0.0.94/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-06-04 14:35:04.625028 qwak_core-0.0.94/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-06-04 14:35:12.005089 qwak_core-0.0.94/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-06-04 14:35:11.881089 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-06-04 14:34:55.564951 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-06-04 14:35:11.881089 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-06-04 14:35:11.881089 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-06-04 14:34:55.352949 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.881089 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-06-04 14:35:11.885089 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-06-04 14:34:55.780953 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-06-04 14:35:11.885089 qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-06-04 14:35:12.001089 qwak_core-0.0.94/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-06-04 14:35:04.233025 qwak_core-0.0.94/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-06-04 14:35:12.005089 qwak_core-0.0.94/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-06-04 14:35:12.021090 qwak_core-0.0.94/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-06-04 14:35:05.853038 qwak_core-0.0.94/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-06-04 14:35:12.021090 qwak_core-0.0.94/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-06-04 14:35:11.877089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-06-04 14:34:53.372933 qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.877089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-06-04 14:35:11.877089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-06-04 14:34:53.196932 qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-06-04 14:35:11.877089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-06-04 14:35:11.869089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-06-04 14:34:52.664928 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.869089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-06-04 14:35:11.873089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-06-04 14:34:52.840929 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.873089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-06-04 14:35:11.873089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-06-04 14:34:53.016930 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-06-04 14:35:11.873089 qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-06-04 14:35:12.045090 qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-06-04 14:35:08.181058 qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-06-04 14:35:12.045090 qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-06-04 14:35:12.045090 qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-06-04 14:35:08.005056 qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:12.045090 qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    10961 2023-06-04 14:35:11.893089 qwak_core-0.0.94/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    14256 2023-06-04 14:34:54.620944 qwak_core-0.0.94/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.893089 qwak_core-0.0.94/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3072 2023-06-04 14:35:11.893089 qwak_core-0.0.94/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2663 2023-06-04 14:34:54.796945 qwak_core-0.0.94/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-04 14:35:11.893089 qwak_core-0.0.94/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-06-04 14:35:13.161097 qwak_core-0.0.94/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-06-04 14:35:13.161097 qwak_core-0.0.94/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-06-04 14:33:29.196169 qwak_core-0.0.94/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    15319 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.200169 qwak_core-0.0.94/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-06-04 14:33:29.204169 qwak_core-0.0.94/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.94/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.94/PKG-INFO
```

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/qwak/user_application/common/v0/resources.proto\x12\x1fqwak.user_application.common.v0\"u\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12\x41\n\x0cmemory_units\x18\x03 \x01(\x0e\x32+.qwak.user_application.common.v0.MemoryUnit\"^\n\x0cGpuResources\x12:\n\x08gpu_type\x18\x01 \x01(\x0e\x32(.qwak.user_application.common.v0.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"s\n SparkClusterResourceTemplateSpec\x12O\n\x08template\x18\x01 \x01(\x0e\x32=.qwak.user_application.common.v0.SparkClusterResourceTemplate\"\xc3\x01\n\x1aSparkResourceConfiguration\x12\x15\n\rdriver_memory\x18\x01 \x01(\t\x12\x14\n\x0c\x64river_cores\x18\x02 \x01(\x05\x12\x19\n\x11initial_executors\x18\x03 \x01(\x05\x12\x15\n\rmin_executors\x18\x04 \x01(\x05\x12\x15\n\rmax_executors\x18\x05 \x01(\x05\x12\x17\n\x0f\x65xecutor_memory\x18\x06 \x01(\t\x12\x16\n\x0e\x65xecutor_cores\x18\x07 \x01(\x05\"5\n\x1ePodComputeResourceTemplateSpec\x12\x13\n\x0btemplate_id\x18\x01 \x01(\t\"\xf3\x01\n\x13PodComputeResources\x12P\n\x11optimization_type\x18\x01 \x01(\x0e\x32\x35.qwak.user_application.common.v0.NodeOptimizationType\x12\x44\n\rcpu_resources\x18\x02 \x01(\x0b\x32-.qwak.user_application.common.v0.CpuResources\x12\x44\n\rgpu_resources\x18\x03 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResources\"t\n\x15SparkComputeResources\x12[\n\x16resource_configuration\x18\x01 \x01(\x0b\x32;.qwak.user_application.common.v0.SparkResourceConfiguration\"\xe5\x01\n\x1b\x43lientSparkComputeResources\x12Z\n\rtemplate_spec\x18\x01 \x01(\x0b\x32\x41.qwak.user_application.common.v0.SparkClusterResourceTemplateSpecH\x00\x12]\n\x16resource_configuration\x18\x02 \x01(\x0b\x32;.qwak.user_application.common.v0.SparkResourceConfigurationH\x00\x42\x0b\n\tresources\"\xe9\x02\n\x19\x43lientPodComputeResources\x12U\n\x16node_optimization_type\x18\x01 \x01(\x0e\x32\x35.qwak.user_application.common.v0.NodeOptimizationType\x12X\n\rtemplate_spec\x18\x02 \x01(\x0b\x32?.qwak.user_application.common.v0.PodComputeResourceTemplateSpecH\x00\x12\x46\n\rcpu_resources\x18\x03 \x01(\x0b\x32-.qwak.user_application.common.v0.CpuResourcesH\x00\x12\x46\n\rgpu_resources\x18\x04 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesH\x00\x42\x0b\n\tresources*7\n\nMemoryUnit\x12\x17\n\x13INVALID_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*q\n\x07GpuType\x12\x14\n\x10INVALID_GPU_TYPE\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05*\x88\x02\n\x1cSparkClusterResourceTemplate\x12\"\n\x1eSPARK_CLUSTER_RESOURCE_INVALID\x10\x00\x12 \n\x1cSPARK_CLUSTER_RESOURCE_SMALL\x10\x01\x12!\n\x1dSPARK_CLUSTER_RESOURCE_MEDIUM\x10\x02\x12 \n\x1cSPARK_CLUSTER_RESOURCE_LARGE\x10\x03\x12\x1d\n\x19SPARK_CLUSTER_RESOURCE_XL\x10\x04\x12\x1e\n\x1aSPARK_CLUSTER_RESOURCE_2XL\x10\x05\x12\x1e\n\x1aSPARK_CLUSTER_RESOURCE_3XL\x10\x06*\x8a\x01\n\x14NodeOptimizationType\x12\x1d\n\x19NODE_OPTIMIZATION_INVALID\x10\x00\x12\x1a\n\x16NODE_OPTIMIZATION_NONE\x10\x01\x12\x19\n\x15NODE_OPTIMIZATION_CPU\x10\x02\x12\x1c\n\x18NODE_OPTIMIZATION_MEMORY\x10\x03\x42\xc5\x01\n&com.qwak.ai.user_application.common.v0P\x01Z\x98\x01github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application_value/common/v0;user_application_common_v0b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/qwak/user_application/common/v0/resources.proto\x12\x1fqwak.user_application.common.v0\"u\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12\x41\n\x0cmemory_units\x18\x03 \x01(\x0e\x32+.qwak.user_application.common.v0.MemoryUnit\"^\n\x0cGpuResources\x12:\n\x08gpu_type\x18\x01 \x01(\x0e\x32(.qwak.user_application.common.v0.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"s\n SparkClusterResourceTemplateSpec\x12O\n\x08template\x18\x01 \x01(\x0e\x32=.qwak.user_application.common.v0.SparkClusterResourceTemplate\"\xc3\x01\n\x1aSparkResourceConfiguration\x12\x15\n\rdriver_memory\x18\x01 \x01(\t\x12\x14\n\x0c\x64river_cores\x18\x02 \x01(\x05\x12\x19\n\x11initial_executors\x18\x03 \x01(\x05\x12\x15\n\rmin_executors\x18\x04 \x01(\x05\x12\x15\n\rmax_executors\x18\x05 \x01(\x05\x12\x17\n\x0f\x65xecutor_memory\x18\x06 \x01(\t\x12\x16\n\x0e\x65xecutor_cores\x18\x07 \x01(\x05\"5\n\x1ePodComputeResourceTemplateSpec\x12\x13\n\x0btemplate_id\x18\x01 \x01(\t\"\xcb\x02\n\x13PodComputeResources\x12P\n\x11optimization_type\x18\x01 \x01(\x0e\x32\x35.qwak.user_application.common.v0.NodeOptimizationType\x12\x44\n\rcpu_resources\x18\x02 \x01(\x0b\x32-.qwak.user_application.common.v0.CpuResources\x12\x44\n\rgpu_resources\x18\x03 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResources\x12V\n\rtemplate_spec\x18\x04 \x01(\x0b\x32?.qwak.user_application.common.v0.PodComputeResourceTemplateSpec\"t\n\x15SparkComputeResources\x12[\n\x16resource_configuration\x18\x01 \x01(\x0b\x32;.qwak.user_application.common.v0.SparkResourceConfiguration\"\xe5\x01\n\x1b\x43lientSparkComputeResources\x12Z\n\rtemplate_spec\x18\x01 \x01(\x0b\x32\x41.qwak.user_application.common.v0.SparkClusterResourceTemplateSpecH\x00\x12]\n\x16resource_configuration\x18\x02 \x01(\x0b\x32;.qwak.user_application.common.v0.SparkResourceConfigurationH\x00\x42\x0b\n\tresources\"\xe9\x02\n\x19\x43lientPodComputeResources\x12U\n\x16node_optimization_type\x18\x01 \x01(\x0e\x32\x35.qwak.user_application.common.v0.NodeOptimizationType\x12X\n\rtemplate_spec\x18\x02 \x01(\x0b\x32?.qwak.user_application.common.v0.PodComputeResourceTemplateSpecH\x00\x12\x46\n\rcpu_resources\x18\x03 \x01(\x0b\x32-.qwak.user_application.common.v0.CpuResourcesH\x00\x12\x46\n\rgpu_resources\x18\x04 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesH\x00\x42\x0b\n\tresources*7\n\nMemoryUnit\x12\x17\n\x13INVALID_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*q\n\x07GpuType\x12\x14\n\x10INVALID_GPU_TYPE\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05*\x88\x02\n\x1cSparkClusterResourceTemplate\x12\"\n\x1eSPARK_CLUSTER_RESOURCE_INVALID\x10\x00\x12 \n\x1cSPARK_CLUSTER_RESOURCE_SMALL\x10\x01\x12!\n\x1dSPARK_CLUSTER_RESOURCE_MEDIUM\x10\x02\x12 \n\x1cSPARK_CLUSTER_RESOURCE_LARGE\x10\x03\x12\x1d\n\x19SPARK_CLUSTER_RESOURCE_XL\x10\x04\x12\x1e\n\x1aSPARK_CLUSTER_RESOURCE_2XL\x10\x05\x12\x1e\n\x1aSPARK_CLUSTER_RESOURCE_3XL\x10\x06*\x8a\x01\n\x14NodeOptimizationType\x12\x1d\n\x19NODE_OPTIMIZATION_INVALID\x10\x00\x12\x1a\n\x16NODE_OPTIMIZATION_NONE\x10\x01\x12\x19\n\x15NODE_OPTIMIZATION_CPU\x10\x02\x12\x1c\n\x18NODE_OPTIMIZATION_MEMORY\x10\x03\x42\xc5\x01\n&com.qwak.ai.user_application.common.v0P\x01Z\x98\x01github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application_value/common/v0;user_application_common_v0b\x06proto3')
 
 _MEMORYUNIT = DESCRIPTOR.enum_types_by_name['MemoryUnit']
 MemoryUnit = enum_type_wrapper.EnumTypeWrapper(_MEMORYUNIT)
 _GPUTYPE = DESCRIPTOR.enum_types_by_name['GpuType']
 GpuType = enum_type_wrapper.EnumTypeWrapper(_GPUTYPE)
 _SPARKCLUSTERRESOURCETEMPLATE = DESCRIPTOR.enum_types_by_name['SparkClusterResourceTemplate']
 SparkClusterResourceTemplate = enum_type_wrapper.EnumTypeWrapper(_SPARKCLUSTERRESOURCETEMPLATE)
@@ -119,34 +119,34 @@
   })
 _sym_db.RegisterMessage(ClientPodComputeResources)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n&com.qwak.ai.user_application.common.v0P\001Z\230\001github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application_value/common/v0;user_application_common_v0'
-  _MEMORYUNIT._serialized_start=1629
-  _MEMORYUNIT._serialized_end=1684
-  _GPUTYPE._serialized_start=1686
-  _GPUTYPE._serialized_end=1799
-  _SPARKCLUSTERRESOURCETEMPLATE._serialized_start=1802
-  _SPARKCLUSTERRESOURCETEMPLATE._serialized_end=2066
-  _NODEOPTIMIZATIONTYPE._serialized_start=2069
-  _NODEOPTIMIZATIONTYPE._serialized_end=2207
+  _MEMORYUNIT._serialized_start=1717
+  _MEMORYUNIT._serialized_end=1772
+  _GPUTYPE._serialized_start=1774
+  _GPUTYPE._serialized_end=1887
+  _SPARKCLUSTERRESOURCETEMPLATE._serialized_start=1890
+  _SPARKCLUSTERRESOURCETEMPLATE._serialized_end=2154
+  _NODEOPTIMIZATIONTYPE._serialized_start=2157
+  _NODEOPTIMIZATIONTYPE._serialized_end=2295
   _CPURESOURCES._serialized_start=84
   _CPURESOURCES._serialized_end=201
   _GPURESOURCES._serialized_start=203
   _GPURESOURCES._serialized_end=297
   _SPARKCLUSTERRESOURCETEMPLATESPEC._serialized_start=299
   _SPARKCLUSTERRESOURCETEMPLATESPEC._serialized_end=414
   _SPARKRESOURCECONFIGURATION._serialized_start=417
   _SPARKRESOURCECONFIGURATION._serialized_end=612
   _PODCOMPUTERESOURCETEMPLATESPEC._serialized_start=614
   _PODCOMPUTERESOURCETEMPLATESPEC._serialized_end=667
   _PODCOMPUTERESOURCES._serialized_start=670
-  _PODCOMPUTERESOURCES._serialized_end=913
-  _SPARKCOMPUTERESOURCES._serialized_start=915
-  _SPARKCOMPUTERESOURCES._serialized_end=1031
-  _CLIENTSPARKCOMPUTERESOURCES._serialized_start=1034
-  _CLIENTSPARKCOMPUTERESOURCES._serialized_end=1263
-  _CLIENTPODCOMPUTERESOURCES._serialized_start=1266
-  _CLIENTPODCOMPUTERESOURCES._serialized_end=1627
+  _PODCOMPUTERESOURCES._serialized_end=1001
+  _SPARKCOMPUTERESOURCES._serialized_start=1003
+  _SPARKCOMPUTERESOURCES._serialized_end=1119
+  _CLIENTSPARKCOMPUTERESOURCES._serialized_start=1122
+  _CLIENTSPARKCOMPUTERESOURCES._serialized_end=1351
+  _CLIENTPODCOMPUTERESOURCES._serialized_start=1354
+  _CLIENTPODCOMPUTERESOURCES._serialized_end=1715
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -212,28 +212,32 @@
 
 class PodComputeResources(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OPTIMIZATION_TYPE_FIELD_NUMBER: builtins.int
     CPU_RESOURCES_FIELD_NUMBER: builtins.int
     GPU_RESOURCES_FIELD_NUMBER: builtins.int
+    TEMPLATE_SPEC_FIELD_NUMBER: builtins.int
     optimization_type: global___NodeOptimizationType.ValueType
     @property
     def cpu_resources(self) -> global___CpuResources: ...
     @property
     def gpu_resources(self) -> global___GpuResources: ...
+    @property
+    def template_spec(self) -> global___PodComputeResourceTemplateSpec: ...
     def __init__(
         self,
         *,
         optimization_type: global___NodeOptimizationType.ValueType = ...,
         cpu_resources: global___CpuResources | None = ...,
         gpu_resources: global___GpuResources | None = ...,
+        template_spec: global___PodComputeResourceTemplateSpec | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["cpu_resources", b"cpu_resources", "gpu_resources", b"gpu_resources"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cpu_resources", b"cpu_resources", "gpu_resources", b"gpu_resources", "optimization_type", b"optimization_type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["cpu_resources", b"cpu_resources", "gpu_resources", b"gpu_resources", "template_spec", b"template_spec"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cpu_resources", b"cpu_resources", "gpu_resources", b"gpu_resources", "optimization_type", b"optimization_type", "template_spec", b"template_spec"]) -> None: ...
 
 global___PodComputeResources = PodComputeResources
 
 class SparkComputeResources(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESOURCE_CONFIGURATION_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.94/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/qwak/user_application/v0/user_application.proto\x12\x18qwak.user_application.v0\x1a\x1cgoogle/protobuf/struct.proto\".\n\x04Spec\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"0\n\x06Status\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct*\xce\x01\n\x04Type\x12!\n\x1dINVALID_USER_APPLICATION_TYPE\x10\x00\x12\x10\n\x0cREMOTE_BUILD\x10\x01\x12\x1b\n\x17\x42\x41TCH_FEATURE_PROCESSOR\x10\x02\x12\x1f\n\x1bSTREAMING_FEATURE_PROCESSOR\x10\x03\x12\x18\n\x14\x42\x41TCH_INFERENCE_TASK\x10\x04\x12\x14\n\x10MODEL_DEPLOYMENT\x10\x05\x12\x11\n\rMODEL_MONITOR\x10\x06\x12\x10\n\x0cMICROSERVICE\x10\x07\x42\xaa\x01\n\x1f\x63om.qwak.ai.user_application.v0P\x01Z\x84\x01github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application/v0;user_application_v0b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/qwak/user_application/v0/user_application.proto\x12\x18qwak.user_application.v0\x1a\x1cgoogle/protobuf/struct.proto\".\n\x04Spec\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"0\n\x06Status\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct*\xd9\x01\n\x04Type\x12!\n\x1dINVALID_USER_APPLICATION_TYPE\x10\x00\x12\x10\n\x0cREMOTE_BUILD\x10\x01\x12\x1b\n\x17\x42\x41TCH_FEATURE_PROCESSOR\x10\x02\x12\x1f\n\x1bSTREAMING_FEATURE_PROCESSOR\x10\x03\x12\x18\n\x14\x42\x41TCH_INFERENCE_TASK\x10\x04\x12\x14\n\x10MODEL_DEPLOYMENT\x10\x05\x12\x11\n\rMODEL_MONITOR\x10\x06\x12\x1b\n\x17\x44\x45PLOYMENT_MICROSERVICE\x10\x07\x42\xaa\x01\n\x1f\x63om.qwak.ai.user_application.v0P\x01Z\x84\x01github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application/v0;user_application_v0b\x06proto3')
 
 _TYPE = DESCRIPTOR.enum_types_by_name['Type']
 Type = enum_type_wrapper.EnumTypeWrapper(_TYPE)
 INVALID_USER_APPLICATION_TYPE = 0
 REMOTE_BUILD = 1
 BATCH_FEATURE_PROCESSOR = 2
 STREAMING_FEATURE_PROCESSOR = 3
 BATCH_INFERENCE_TASK = 4
 MODEL_DEPLOYMENT = 5
 MODEL_MONITOR = 6
-MICROSERVICE = 7
+DEPLOYMENT_MICROSERVICE = 7
 
 
 _SPEC = DESCRIPTOR.message_types_by_name['Spec']
 _STATUS = DESCRIPTOR.message_types_by_name['Status']
 Spec = _reflection.GeneratedProtocolMessageType('Spec', (_message.Message,), {
   'DESCRIPTOR' : _SPEC,
   '__module__' : 'qwak.user_application.v0.user_application_pb2'
@@ -47,13 +47,13 @@
 _sym_db.RegisterMessage(Status)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\037com.qwak.ai.user_application.v0P\001Z\204\001github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application/v0;user_application_v0'
   _TYPE._serialized_start=206
-  _TYPE._serialized_end=412
+  _TYPE._serialized_end=423
   _SPEC._serialized_start=107
   _SPEC._serialized_end=153
   _STATUS._serialized_start=155
   _STATUS._serialized_end=203
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.93/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.94/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -26,26 +26,26 @@
     INVALID_USER_APPLICATION_TYPE: _Type.ValueType  # 0
     REMOTE_BUILD: _Type.ValueType  # 1
     BATCH_FEATURE_PROCESSOR: _Type.ValueType  # 2
     STREAMING_FEATURE_PROCESSOR: _Type.ValueType  # 3
     BATCH_INFERENCE_TASK: _Type.ValueType  # 4
     MODEL_DEPLOYMENT: _Type.ValueType  # 5
     MODEL_MONITOR: _Type.ValueType  # 6
-    MICROSERVICE: _Type.ValueType  # 7
+    DEPLOYMENT_MICROSERVICE: _Type.ValueType  # 7
 
 class Type(_Type, metaclass=_TypeEnumTypeWrapper): ...
 
 INVALID_USER_APPLICATION_TYPE: Type.ValueType  # 0
 REMOTE_BUILD: Type.ValueType  # 1
 BATCH_FEATURE_PROCESSOR: Type.ValueType  # 2
 STREAMING_FEATURE_PROCESSOR: Type.ValueType  # 3
 BATCH_INFERENCE_TASK: Type.ValueType  # 4
 MODEL_DEPLOYMENT: Type.ValueType  # 5
 MODEL_MONITOR: Type.ValueType  # 6
-MICROSERVICE: Type.ValueType  # 7
+DEPLOYMENT_MICROSERVICE: Type.ValueType  # 7
 global___Type = Type
 
 class Spec(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALUE_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `qwak_core-0.0.93/pyproject.toml` & `qwak_core-0.0.94/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.93"
+version = "0.0.94"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.93/qwak/automations/__init__.py` & `qwak_core-0.0.94/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/automations/automation_executions.py` & `qwak_core-0.0.94/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/automations/automations.py` & `qwak_core-0.0.94/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.94/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.94/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/automations/common.py` & `qwak_core-0.0.94/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.94/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.94/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.94/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.94/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.94/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/alert_management/client.py` & `qwak_core-0.0.94/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/analytics/client.py` & `qwak_core-0.0.94/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/audience/client.py` & `qwak_core-0.0.94/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/automation_management/client.py` & `qwak_core-0.0.94/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.94/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.94/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.94/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.94/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/build_management/client.py` & `qwak_core-0.0.94/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.94/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.94/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/deployment/client.py` & `qwak_core-0.0.94/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.94/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.94/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.94/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.94/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/instance_template/client.py` & `qwak_core-0.0.94/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.94/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/logging_client/client.py` & `qwak_core-0.0.94/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/model_management/client.py` & `qwak_core-0.0.94/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/project/client.py` & `qwak_core-0.0.94/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/secret_service/client.py` & `qwak_core-0.0.94/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.94/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.94/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.94/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.94/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.94/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.94/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.94/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.94/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.94/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.94/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.94/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.94/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.94/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.94/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.94/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/offline/client.py` & `qwak_core-0.0.94/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/feature_store/online/client.py` & `qwak_core-0.0.94/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/inner/const.py` & `qwak_core-0.0.94/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.94/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.94/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.94/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.94/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/inner/singleton_meta.py` & `qwak_core-0.0.94/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/inner/tool/auth.py` & `qwak_core-0.0.94/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.94/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.94/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.94/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.94/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/adapters/__init__.py` & `qwak_core-0.0.94/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.94/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.94/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.94/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.94/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.94/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/base.py` & `qwak_core-0.0.94/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/decorators/api.py` & `qwak_core-0.0.94/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.94/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/experiment_tracking.py` & `qwak_core-0.0.94/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/schema.py` & `qwak_core-0.0.94/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/schema_entities.py` & `qwak_core-0.0.94/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.94/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.94/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.94/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.94/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.94/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.94/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.94/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.94/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.94/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.94/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.94/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.94/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/qwak_client/client.py` & `qwak_core-0.0.94/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.94/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/qwak_client/models/model.py` & `qwak_core-0.0.94/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.94/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.94/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/tools/logger/logger.py` & `qwak_core-0.0.94/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak/tools/logger/logging.yml` & `qwak_core-0.0.94/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.94/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/qwak_services_mock/services_mock.py` & `qwak_core-0.0.94/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.93/setup.py` & `qwak_core-0.0.94/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.93',
+    'version': '0.0.94',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.93/PKG-INFO` & `qwak_core-0.0.94/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.93
+Version: 0.0.94
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

