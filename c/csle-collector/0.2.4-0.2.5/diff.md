# Comparing `tmp/csle_collector-0.2.4.tar.gz` & `tmp/csle_collector-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_collector-0.2.4.tar", last modified: Wed May 31 13:42:27 2023, max compression
+gzip compressed data, was "csle_collector-0.2.5.tar", last modified: Sun Jun  4 07:13:46 2023, max compression
```

## Comparing `csle_collector-0.2.4.tar` & `csle_collector-0.2.5.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.875038 csle_collector-0.2.4/
--rw-r--r--   0 kimham     (501) staff       (20)      803 2023-05-31 13:42:27.875186 csle_collector-0.2.4/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     5807 2023-03-05 07:26:30.000000 csle_collector-0.2.4/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      674 2023-02-12 08:59:32.000000 csle_collector-0.2.4/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1454 2023-05-31 13:42:27.875845 csle_collector-0.2.4/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_collector-0.2.4/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.808683 csle_collector-0.2.4/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.812632 csle_collector-0.2.4/src/csle_collector/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 13:42:03.000000 csle_collector-0.2.4/src/csle_collector/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.818212 csle_collector-0.2.4/src/csle_collector/client_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/client_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     9996 2023-05-31 11:11:40.000000 csle_collector-0.2.4/src/csle_collector/client_manager/client_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     5660 2023-05-31 12:09:00.000000 csle_collector-0.2.4/src/csle_collector/client_manager/client_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     8592 2023-05-31 12:09:30.000000 csle_collector-0.2.4/src/csle_collector/client_manager/client_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     2179 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/client_manager/client_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     4316 2023-05-24 17:43:06.000000 csle_collector-0.2.4/src/csle_collector/client_manager/client_population_metrics.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.834654 csle_collector-0.2.4/src/csle_collector/client_manager/dao/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-05-31 07:06:48.000000 csle_collector-0.2.4/src/csle_collector/client_manager/dao/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2379 2023-05-31 08:44:30.000000 csle_collector-0.2.4/src/csle_collector/client_manager/dao/arrival_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     9508 2023-05-31 11:02:02.000000 csle_collector-0.2.4/src/csle_collector/client_manager/dao/client.py
--rw-r--r--   0 kimham     (501) staff       (20)      340 2023-05-31 07:06:48.000000 csle_collector-0.2.4/src/csle_collector/client_manager/dao/client_arrival_type.py
--rw-r--r--   0 kimham     (501) staff       (20)     2140 2023-05-31 08:47:06.000000 csle_collector-0.2.4/src/csle_collector/client_manager/dao/constant_arrival_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     2859 2023-05-31 08:49:42.000000 csle_collector-0.2.4/src/csle_collector/client_manager/dao/eptmp_arrival_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     1780 2023-05-31 07:06:48.000000 csle_collector-0.2.4/src/csle_collector/client_manager/dao/eptmp_rate_function.py
--rw-r--r--   0 kimham     (501) staff       (20)     2695 2023-05-31 08:50:44.000000 csle_collector-0.2.4/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3098 2023-05-31 08:52:02.000000 csle_collector-0.2.4/src/csle_collector/client_manager/dao/sine_arrival_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     2447 2023-05-31 08:53:06.000000 csle_collector-0.2.4/src/csle_collector/client_manager/dao/spiking_arrival_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     5539 2023-05-31 09:04:14.000000 csle_collector-0.2.4/src/csle_collector/client_manager/dao/workflow_markov_chain.py
--rw-r--r--   0 kimham     (501) staff       (20)     5131 2023-05-31 12:11:16.000000 csle_collector-0.2.4/src/csle_collector/client_manager/dao/workflow_service.py
--rw-r--r--   0 kimham     (501) staff       (20)     5268 2023-05-31 09:47:00.000000 csle_collector-0.2.4/src/csle_collector/client_manager/dao/workflows_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     4064 2023-05-31 11:16:13.000000 csle_collector-0.2.4/src/csle_collector/client_manager/query_clients.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.838540 csle_collector-0.2.4/src/csle_collector/client_manager/threads/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-05-31 07:06:48.000000 csle_collector-0.2.4/src/csle_collector/client_manager/threads/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     6971 2023-05-31 11:09:17.000000 csle_collector-0.2.4/src/csle_collector/client_manager/threads/arrival_thread.py
--rw-r--r--   0 kimham     (501) staff       (20)      971 2023-05-31 11:06:56.000000 csle_collector-0.2.4/src/csle_collector/client_manager/threads/client_thread.py
--rw-r--r--   0 kimham     (501) staff       (20)     2374 2023-05-31 11:10:19.000000 csle_collector-0.2.4/src/csle_collector/client_manager/threads/producer_thread.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.839743 csle_collector-0.2.4/src/csle_collector/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    36309 2023-04-19 06:25:48.000000 csle_collector-0.2.4/src/csle_collector/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.845714 csle_collector-0.2.4/src/csle_collector/docker_stats_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-02-12 12:41:34.000000 csle_collector-0.2.4/src/csle_collector/docker_stats_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    12394 2023-03-15 11:36:56.000000 csle_collector-0.2.4/src/csle_collector/docker_stats_manager/docker_stats.py
--rw-r--r--   0 kimham     (501) staff       (20)    13540 2023-03-05 11:13:10.000000 csle_collector-0.2.4/src/csle_collector/docker_stats_manager/docker_stats_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     4589 2023-02-12 12:41:34.000000 csle_collector-0.2.4/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     6193 2023-02-12 12:41:34.000000 csle_collector-0.2.4/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     8801 2023-02-12 12:41:34.000000 csle_collector-0.2.4/src/csle_collector/docker_stats_manager/docker_stats_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     3994 2023-03-20 09:39:38.000000 csle_collector-0.2.4/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.848926 csle_collector-0.2.4/src/csle_collector/elk_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/elk_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    10740 2023-03-22 11:50:26.000000 csle_collector-0.2.4/src/csle_collector/elk_manager/elk_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     5923 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/elk_manager/elk_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)    14300 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     1540 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/elk_manager/elk_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     5768 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/elk_manager/query_elk_server.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.855006 csle_collector-0.2.4/src/csle_collector/host_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/host_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      875 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/host_manager/failed_login_attempt.py
--rw-r--r--   0 kimham     (501) staff       (20)    65375 2023-03-31 11:14:06.000000 csle_collector-0.2.4/src/csle_collector/host_manager/host_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)    13966 2023-03-31 11:14:06.000000 csle_collector-0.2.4/src/csle_collector/host_manager/host_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)    28800 2023-03-31 11:14:06.000000 csle_collector-0.2.4/src/csle_collector/host_manager/host_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)    33850 2023-03-05 07:26:30.000000 csle_collector-0.2.4/src/csle_collector/host_manager/host_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     7783 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/host_manager/host_metrics.py
--rw-r--r--   0 kimham     (501) staff       (20)    16572 2023-03-31 11:14:06.000000 csle_collector-0.2.4/src/csle_collector/host_manager/query_host_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     1292 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/host_manager/successful_login.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.858070 csle_collector-0.2.4/src/csle_collector/kafka_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/kafka_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     6616 2023-03-22 11:50:26.000000 csle_collector-0.2.4/src/csle_collector/kafka_manager/kafka_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     4116 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/kafka_manager/kafka_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     8484 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     1442 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/kafka_manager/kafka_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     3233 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/kafka_manager/query_kafka_server.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.862212 csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2931 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py
--rw-r--r--   0 kimham     (501) staff       (20)    10847 2023-03-16 08:28:05.000000 csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py
--rw-r--r--   0 kimham     (501) staff       (20)    11386 2023-03-22 11:50:26.000000 csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     7479 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)    10801 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)    13329 2022-11-30 17:44:15.000000 csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     5377 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.865189 csle_collector-0.2.4/src/csle_collector/ryu_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/ryu_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     3936 2022-12-07 13:13:59.000000 csle_collector-0.2.4/src/csle_collector/ryu_manager/query_ryu_server.py
--rw-r--r--   0 kimham     (501) staff       (20)    18068 2023-04-19 06:25:48.000000 csle_collector-0.2.4/src/csle_collector/ryu_manager/ryu_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     4363 2022-12-07 08:23:15.000000 csle_collector-0.2.4/src/csle_collector/ryu_manager/ryu_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     8368 2022-12-07 08:23:40.000000 csle_collector-0.2.4/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     2086 2022-12-07 08:18:55.000000 csle_collector-0.2.4/src/csle_collector/ryu_manager/ryu_manager_util.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.870158 csle_collector-0.2.4/src/csle_collector/snort_ids_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/snort_ids_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     5787 2023-03-31 11:14:06.000000 csle_collector-0.2.4/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     7996 2023-03-31 11:14:06.000000 csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_alert.py
--rw-r--r--   0 kimham     (501) staff       (20)    11779 2023-03-31 11:14:06.000000 csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py
--rw-r--r--   0 kimham     (501) staff       (20)     9176 2023-03-31 11:14:06.000000 csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py
--rw-r--r--   0 kimham     (501) staff       (20)    13005 2023-03-31 11:14:06.000000 csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     8283 2023-03-31 11:14:06.000000 csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)    10801 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)    16748 2023-03-31 11:14:06.000000 csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     4288 2023-03-31 11:14:06.000000 csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.874453 csle_collector-0.2.4/src/csle_collector/traffic_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/traffic_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2534 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/traffic_manager/query_traffic_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     7492 2023-05-31 11:44:33.000000 csle_collector-0.2.4/src/csle_collector/traffic_manager/traffic_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     3087 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/traffic_manager/traffic_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     5596 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     1477 2022-11-28 13:00:49.000000 csle_collector-0.2.4/src/csle_collector/traffic_manager/traffic_manager_util.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:27.814643 csle_collector-0.2.4/src/csle_collector.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      803 2023-05-31 13:42:27.000000 csle_collector-0.2.4/src/csle_collector.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     5103 2023-05-31 13:42:27.000000 csle_collector-0.2.4/src/csle_collector.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 13:42:27.000000 csle_collector-0.2.4/src/csle_collector.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:14.000000 csle_collector-0.2.4/src/csle_collector.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      293 2023-05-31 13:42:27.000000 csle_collector-0.2.4/src/csle_collector.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       15 2023-05-31 13:42:27.000000 csle_collector-0.2.4/src/csle_collector.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.253367 csle_collector-0.2.5/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      803 2023-06-04 07:13:46.253367 csle_collector-0.2.5/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5807 2023-03-28 14:03:22.000000 csle_collector-0.2.5/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      674 2023-03-28 14:03:22.000000 csle_collector-0.2.5/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1454 2023-06-04 07:13:46.253367 csle_collector-0.2.5/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_collector-0.2.5/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.237367 csle_collector-0.2.5/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.237367 csle_collector-0.2.5/src/csle_collector/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 07:13:34.000000 csle_collector-0.2.5/src/csle_collector/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.241367 csle_collector-0.2.5/src/csle_collector/client_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/client_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9996 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/client_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5660 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/client_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8592 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/client_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2179 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/client_manager/client_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4316 2023-05-30 09:03:51.000000 csle_collector-0.2.5/src/csle_collector/client_manager/client_population_metrics.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.241367 csle_collector-0.2.5/src/csle_collector/client_manager/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-30 09:40:47.000000 csle_collector-0.2.5/src/csle_collector/client_manager/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2379 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/dao/arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9508 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/dao/client.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      340 2023-05-30 13:25:09.000000 csle_collector-0.2.5/src/csle_collector/client_manager/dao/client_arrival_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2140 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/dao/constant_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2859 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/dao/eptmp_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1780 2023-05-30 09:45:21.000000 csle_collector-0.2.5/src/csle_collector/client_manager/dao/eptmp_rate_function.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2695 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3098 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/dao/sine_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2447 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/dao/spiking_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5539 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/dao/workflow_markov_chain.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5131 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/dao/workflow_service.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5268 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/dao/workflows_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4066 2023-06-04 07:12:33.000000 csle_collector-0.2.5/src/csle_collector/client_manager/query_clients.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.241367 csle_collector-0.2.5/src/csle_collector/client_manager/threads/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-30 09:20:57.000000 csle_collector-0.2.5/src/csle_collector/client_manager/threads/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6971 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/threads/arrival_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      971 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/threads/client_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2374 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/client_manager/threads/producer_thread.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.241367 csle_collector-0.2.5/src/csle_collector/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    36309 2023-04-18 12:48:07.000000 csle_collector-0.2.5/src/csle_collector/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.245367 csle_collector-0.2.5/src/csle_collector/docker_stats_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/docker_stats_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12394 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/docker_stats_manager/docker_stats.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13540 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/docker_stats_manager/docker_stats_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4589 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6193 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8801 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/docker_stats_manager/docker_stats_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3994 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.245367 csle_collector-0.2.5/src/csle_collector/elk_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/elk_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10740 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/elk_manager/elk_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5923 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/elk_manager/elk_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14300 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1540 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/elk_manager/elk_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5768 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/elk_manager/query_elk_server.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.249367 csle_collector-0.2.5/src/csle_collector/host_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/host_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      875 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/host_manager/failed_login_attempt.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    65375 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/host_manager/host_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13966 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/host_manager/host_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    28800 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/host_manager/host_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    33850 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/host_manager/host_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7783 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/host_manager/host_metrics.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16572 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/host_manager/query_host_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1292 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/host_manager/successful_login.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.249367 csle_collector-0.2.5/src/csle_collector/kafka_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/kafka_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6616 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/kafka_manager/kafka_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4116 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/kafka_manager/kafka_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8484 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1442 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/kafka_manager/kafka_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3233 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/kafka_manager/query_kafka_server.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.249367 csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2931 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10847 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11386 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7479 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13329 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5377 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.253367 csle_collector-0.2.5/src/csle_collector/ryu_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/ryu_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/ryu_manager/query_ryu_server.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18068 2023-04-18 12:46:51.000000 csle_collector-0.2.5/src/csle_collector/ryu_manager/ryu_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4363 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/ryu_manager/ryu_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8368 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2086 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/ryu_manager/ryu_manager_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.253367 csle_collector-0.2.5/src/csle_collector/snort_ids_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/snort_ids_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5787 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7996 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_alert.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11779 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9176 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13005 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8283 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16748 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4288 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.253367 csle_collector-0.2.5/src/csle_collector/traffic_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/traffic_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2534 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/traffic_manager/query_traffic_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7492 2023-06-04 07:11:42.000000 csle_collector-0.2.5/src/csle_collector/traffic_manager/traffic_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3087 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/traffic_manager/traffic_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5596 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1477 2023-03-28 14:03:22.000000 csle_collector-0.2.5/src/csle_collector/traffic_manager/traffic_manager_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:46.241367 csle_collector-0.2.5/src/csle_collector.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      803 2023-06-04 07:13:45.000000 csle_collector-0.2.5/src/csle_collector.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5103 2023-06-04 07:13:46.000000 csle_collector-0.2.5/src/csle_collector.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 07:13:45.000000 csle_collector-0.2.5/src/csle_collector.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:37.000000 csle_collector-0.2.5/src/csle_collector.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      293 2023-06-04 07:13:46.000000 csle_collector-0.2.5/src/csle_collector.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       15 2023-06-04 07:13:46.000000 csle_collector-0.2.5/src/csle_collector.egg-info/top_level.txt
```

### Comparing `csle_collector-0.2.4/PKG-INFO` & `csle_collector-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_collector
-Version: 0.2.4
+Version: 0.2.5
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.2.4/README.md` & `csle_collector-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/pyproject.toml` & `csle_collector-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/setup.cfg` & `csle_collector-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/client_manager.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/client_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/client_manager_pb2.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/client_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/client_manager_pb2_grpc.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/client_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/client_manager_util.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/client_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/client_population_metrics.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/client_population_metrics.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/dao/arrival_config.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/dao/arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/dao/client.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/dao/client.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/dao/constant_arrival_config.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/dao/constant_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/dao/eptmp_arrival_config.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/dao/eptmp_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/dao/eptmp_rate_function.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/dao/eptmp_rate_function.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/dao/sine_arrival_config.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/dao/sine_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/dao/spiking_arrival_config.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/dao/spiking_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/dao/workflow_markov_chain.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/dao/workflow_markov_chain.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/dao/workflow_service.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/dao/workflow_service.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/dao/workflows_config.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/dao/workflows_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/query_clients.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/query_clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     :param stub: the stub to the gRPC server
     :param time_step_len_seconds: length of a time-step in the emulation
     :param workflows_config: configuration of the workflows
     :param clients: list of client profiles
     :param timeout: the timeout for sending a request to the GRPC server
     :return: a clients DTO describing the state of the clients
     """
-    clients_grpcs = list(map(lambda x: x.to_grpc_object, clients))
+    clients_grpcs = list(map(lambda x: x.to_grpc_object(), clients))
     workflows_config_grpc = workflows_config.to_grpc_object()
     start_clients_msg = csle_collector.client_manager.client_manager_pb2.StartClientsMsg(
         time_step_len_seconds=time_step_len_seconds, clients=clients_grpcs,
         workflows_config_grpc=workflows_config_grpc)
     clients_dto = stub.startClients(start_clients_msg, timeout=timeout)
     return clients_dto
```

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/threads/arrival_thread.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/threads/arrival_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/threads/client_thread.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/threads/client_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/client_manager/threads/producer_thread.py` & `csle_collector-0.2.5/src/csle_collector/client_manager/threads/producer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/constants/constants.py` & `csle_collector-0.2.5/src/csle_collector/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/docker_stats_manager/docker_stats.py` & `csle_collector-0.2.5/src/csle_collector/docker_stats_manager/docker_stats.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/docker_stats_manager/docker_stats_manager.py` & `csle_collector-0.2.5/src/csle_collector/docker_stats_manager/docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py` & `csle_collector-0.2.5/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py` & `csle_collector-0.2.5/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/docker_stats_manager/docker_stats_util.py` & `csle_collector-0.2.5/src/csle_collector/docker_stats_manager/docker_stats_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py` & `csle_collector-0.2.5/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/elk_manager/elk_manager.py` & `csle_collector-0.2.5/src/csle_collector/elk_manager/elk_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/elk_manager/elk_manager_pb2.py` & `csle_collector-0.2.5/src/csle_collector/elk_manager/elk_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py` & `csle_collector-0.2.5/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/elk_manager/elk_manager_util.py` & `csle_collector-0.2.5/src/csle_collector/elk_manager/elk_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/elk_manager/query_elk_server.py` & `csle_collector-0.2.5/src/csle_collector/elk_manager/query_elk_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/host_manager/failed_login_attempt.py` & `csle_collector-0.2.5/src/csle_collector/host_manager/failed_login_attempt.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/host_manager/host_manager.py` & `csle_collector-0.2.5/src/csle_collector/host_manager/host_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/host_manager/host_manager_pb2.py` & `csle_collector-0.2.5/src/csle_collector/host_manager/host_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/host_manager/host_manager_pb2_grpc.py` & `csle_collector-0.2.5/src/csle_collector/host_manager/host_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/host_manager/host_manager_util.py` & `csle_collector-0.2.5/src/csle_collector/host_manager/host_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/host_manager/host_metrics.py` & `csle_collector-0.2.5/src/csle_collector/host_manager/host_metrics.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/host_manager/query_host_manager.py` & `csle_collector-0.2.5/src/csle_collector/host_manager/query_host_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/host_manager/successful_login.py` & `csle_collector-0.2.5/src/csle_collector/host_manager/successful_login.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/kafka_manager/kafka_manager.py` & `csle_collector-0.2.5/src/csle_collector/kafka_manager/kafka_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/kafka_manager/kafka_manager_pb2.py` & `csle_collector-0.2.5/src/csle_collector/kafka_manager/kafka_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py` & `csle_collector-0.2.5/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/kafka_manager/kafka_manager_util.py` & `csle_collector-0.2.5/src/csle_collector/kafka_manager/kafka_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/kafka_manager/query_kafka_server.py` & `csle_collector-0.2.5/src/csle_collector/kafka_manager/query_kafka_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py` & `csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py` & `csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py` & `csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py` & `csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py` & `csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py` & `csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py` & `csle_collector-0.2.5/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/ryu_manager/query_ryu_server.py` & `csle_collector-0.2.5/src/csle_collector/ryu_manager/query_ryu_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/ryu_manager/ryu_manager.py` & `csle_collector-0.2.5/src/csle_collector/ryu_manager/ryu_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/ryu_manager/ryu_manager_pb2.py` & `csle_collector-0.2.5/src/csle_collector/ryu_manager/ryu_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py` & `csle_collector-0.2.5/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/ryu_manager/ryu_manager_util.py` & `csle_collector-0.2.5/src/csle_collector/ryu_manager/ryu_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py` & `csle_collector-0.2.5/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_alert.py` & `csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py` & `csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py` & `csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_manager.py` & `csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py` & `csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py` & `csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py` & `csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py` & `csle_collector-0.2.5/src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/traffic_manager/query_traffic_manager.py` & `csle_collector-0.2.5/src/csle_collector/traffic_manager/query_traffic_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/traffic_manager/traffic_manager.py` & `csle_collector-0.2.5/src/csle_collector/traffic_manager/traffic_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/traffic_manager/traffic_manager_pb2.py` & `csle_collector-0.2.5/src/csle_collector/traffic_manager/traffic_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py` & `csle_collector-0.2.5/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector/traffic_manager/traffic_manager_util.py` & `csle_collector-0.2.5/src/csle_collector/traffic_manager/traffic_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.4/src/csle_collector.egg-info/PKG-INFO` & `csle_collector-0.2.5/src/csle_collector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-collector
-Version: 0.2.4
+Version: 0.2.5
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.2.4/src/csle_collector.egg-info/SOURCES.txt` & `csle_collector-0.2.5/src/csle_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

