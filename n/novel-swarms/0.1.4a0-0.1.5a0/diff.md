# Comparing `tmp/novel_swarms-0.1.4a0.tar.gz` & `tmp/novel_swarms-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novel_swarms-0.1.4a0.tar", last modified: Mon May 22 22:36:56 2023, max compression
+gzip compressed data, was "novel_swarms-0.1.5a0.tar", last modified: Sun Jun  4 17:22:08 2023, max compression
```

## Comparing `novel_swarms-0.1.4a0.tar` & `novel_swarms-0.1.5a0.tar`

### file list

```diff
@@ -1,147 +1,151 @@
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/
--rw-rw-r--   0 connor    (1001) connor    (1001)      486 2023-04-18 02:45:46.000000 novel_swarms-0.1.4a0/.gitignore
--rw-rw-r--   0 connor    (1001) connor    (1001)     1107 2023-04-19 20:59:13.000000 novel_swarms-0.1.4a0/LICENSE
--rw-rw-r--   0 connor    (1001) connor    (1001)       42 2022-09-19 15:01:24.000000 novel_swarms-0.1.4a0/MANIFEST.in
--rw-rw-r--   0 connor    (1001) connor    (1001)     6796 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/PKG-INFO
--rw-rw-r--   0 connor    (1001) connor    (1001)     6256 2023-05-22 21:45:25.000000 novel_swarms-0.1.4a0/README.md
--rw-rw-r--   0 connor    (1001) connor    (1001)       72 2023-04-17 22:17:05.000000 novel_swarms-0.1.4a0/git.sh
--rw-rw-r--   0 connor    (1001) connor    (1001)      617 2023-05-22 22:36:52.000000 novel_swarms-0.1.4a0/pyproject.toml
--rw-rw-r--   0 connor    (1001) connor    (1001)     1061 2023-04-27 20:54:12.000000 novel_swarms-0.1.4a0/requirements.txt
--rw-rw-r--   0 connor    (1001) connor    (1001)       38 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/setup.cfg
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.302271 novel_swarms-0.1.4a0/src/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.4a0/src/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.302271 novel_swarms-0.1.4a0/src/novel_swarms/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-15 20:43:52.000000 novel_swarms-0.1.4a0/src/novel_swarms/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.302271 novel_swarms-0.1.4a0/src/novel_swarms/agent/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1199 2023-05-17 17:50:16.000000 novel_swarms-0.1.4a0/src/novel_swarms/agent/Agent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1472 2023-05-19 17:51:10.000000 novel_swarms-0.1.4a0/src/novel_swarms/agent/AgentFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     7341 2023-04-24 18:59:47.000000 novel_swarms-0.1.4a0/src/novel_swarms/agent/DiffDriveAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     6576 2023-05-22 22:11:38.000000 novel_swarms-0.1.4a0/src/novel_swarms/agent/DroneAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1208 2023-04-27 17:48:12.000000 novel_swarms-0.1.4a0/src/novel_swarms/agent/HumanAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4726 2023-05-12 20:50:55.000000 novel_swarms-0.1.4a0/src/novel_swarms/agent/LevyAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     7272 2023-05-19 16:23:44.000000 novel_swarms-0.1.4a0/src/novel_swarms/agent/MazeAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      855 2023-05-22 22:28:16.000000 novel_swarms-0.1.4a0/src/novel_swarms/agent/ModeSwitchingAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2595 2023-03-04 01:21:09.000000 novel_swarms-0.1.4a0/src/novel_swarms/agent/StaticAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     8166 2023-04-04 02:15:06.000000 novel_swarms-0.1.4a0/src/novel_swarms/agent/UnicycleAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:30.000000 novel_swarms-0.1.4a0/src/novel_swarms/agent/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/behavior/
--rw-rw-r--   0 connor    (1001) connor    (1001)      993 2023-05-18 23:13:24.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/AbstractBehavior.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2085 2023-04-04 14:55:04.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/AgentsAtGoal.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1249 2023-05-19 16:08:03.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/AlgebraicConnectivity.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1196 2023-05-19 16:08:03.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/AngularMomentum.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      583 2023-05-19 16:08:03.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/AverageSpeed.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2379 2023-05-22 22:10:50.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/BehaviorFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1340 2023-05-12 16:44:43.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/Centroid.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3349 2023-04-18 15:30:56.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/ConvexHull.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1606 2023-05-22 22:14:28.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/DistanceToGoal.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1176 2023-05-19 16:08:03.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/GroupRotationBehavior.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1849 2023-04-18 19:46:18.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/PersistentHomology.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1746 2023-05-19 16:08:03.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/RadialVariance.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1387 2023-04-24 22:53:06.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/ScatterBehavior.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      700 2023-05-19 16:08:03.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/SensorOffset.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      549 2023-05-19 16:08:03.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/SensorRotation.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1514 2023-04-24 23:01:45.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/SensorSignal.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      616 2023-05-18 23:41:03.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/TotalCollisions.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:40.000000 novel_swarms-0.1.4a0/src/novel_swarms/behavior/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/cache/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1681 2023-01-17 23:54:56.000000 novel_swarms-0.1.4a0/src/novel_swarms/cache/ExternalSimulationArchive.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 22:42:03.000000 novel_swarms-0.1.4a0/src/novel_swarms/cache/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/config/
--rw-rw-r--   0 connor    (1001) connor    (1001)    13756 2023-05-19 17:55:12.000000 novel_swarms-0.1.4a0/src/novel_swarms/config/AgentConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1800 2023-03-13 23:06:38.000000 novel_swarms-0.1.4a0/src/novel_swarms/config/EvolutionaryConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2470 2023-05-22 17:57:25.000000 novel_swarms-0.1.4a0/src/novel_swarms/config/HeterogenSwarmConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)       56 2023-05-17 17:50:16.000000 novel_swarms-0.1.4a0/src/novel_swarms/config/ModeConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      637 2023-01-20 15:33:41.000000 novel_swarms-0.1.4a0/src/novel_swarms/config/OutputTensorConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      520 2022-09-15 20:43:52.000000 novel_swarms-0.1.4a0/src/novel_swarms/config/ResultsConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4095 2023-05-22 22:29:31.000000 novel_swarms-0.1.4a0/src/novel_swarms/config/WorldConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:49.000000 novel_swarms-0.1.4a0/src/novel_swarms/config/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1961 2023-05-19 18:43:55.000000 novel_swarms-0.1.4a0/src/novel_swarms/config/defaults.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/gui/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:58.000000 novel_swarms-0.1.4a0/src/novel_swarms/gui/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      479 2023-05-12 21:01:36.000000 novel_swarms-0.1.4a0/src/novel_swarms/gui/abstractGUI.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3431 2023-04-27 22:51:31.000000 novel_swarms-0.1.4a0/src/novel_swarms/gui/agentGUI.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2401 2022-12-07 17:37:58.000000 novel_swarms-0.1.4a0/src/novel_swarms/gui/connectivityGUI.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4143 2023-05-15 22:49:40.000000 novel_swarms-0.1.4a0/src/novel_swarms/gui/controllerGUI.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2670 2022-09-16 18:13:19.000000 novel_swarms-0.1.4a0/src/novel_swarms/gui/evolutionGUI.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/novelty/
--rw-rw-r--   0 connor    (1001) connor    (1001)    10678 2023-05-22 17:43:57.000000 novel_swarms-0.1.4a0/src/novel_swarms/novelty/BehaviorDiscovery.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     7812 2023-05-22 17:42:55.000000 novel_swarms-0.1.4a0/src/novel_swarms/novelty/GeneRule.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3931 2022-10-26 23:42:12.000000 novel_swarms-0.1.4a0/src/novel_swarms/novelty/NoveltyArchive.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:05.000000 novel_swarms-0.1.4a0/src/novel_swarms/novelty/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3884 2023-05-22 17:31:33.000000 novel_swarms-0.1.4a0/src/novel_swarms/novelty/evolve.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/optim/
--rw-rw-r--   0 connor    (1001) connor    (1001)     6806 2023-05-22 22:14:05.000000 novel_swarms-0.1.4a0/src/novel_swarms/optim/CMAES.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      113 2023-05-03 18:10:54.000000 novel_swarms-0.1.4a0/src/novel_swarms/optim/OptimVar.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-27 15:37:22.000000 novel_swarms-0.1.4a0/src/novel_swarms/optim/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/results/
--rw-rw-r--   0 connor    (1001) connor    (1001)     6926 2023-05-22 18:21:21.000000 novel_swarms-0.1.4a0/src/novel_swarms/results/Cluster.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      612 2022-10-10 15:58:53.000000 novel_swarms-0.1.4a0/src/novel_swarms/results/ClusterPoint.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2728 2023-03-13 21:38:40.000000 novel_swarms-0.1.4a0/src/novel_swarms/results/Trends.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:12.000000 novel_swarms-0.1.4a0/src/novel_swarms/results/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4612 2023-05-22 22:12:51.000000 novel_swarms-0.1.4a0/src/novel_swarms/results/behavior_metrics.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      474 2023-05-22 18:28:05.000000 novel_swarms-0.1.4a0/src/novel_swarms/results/results.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/results/scripts/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.4a0/src/novel_swarms/results/scripts/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4869 2022-09-16 18:58:24.000000 novel_swarms-0.1.4a0/src/novel_swarms/results/scripts/domain_codomain.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/sensors/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1021 2023-01-23 17:59:03.000000 novel_swarms-0.1.4a0/src/novel_swarms/sensors/AbstractSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)    13602 2023-05-19 17:20:52.000000 novel_swarms-0.1.4a0/src/novel_swarms/sensors/BinaryFOVSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4032 2023-05-19 17:21:38.000000 novel_swarms-0.1.4a0/src/novel_swarms/sensors/BinaryLOSSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1779 2023-03-14 00:02:26.000000 novel_swarms-0.1.4a0/src/novel_swarms/sensors/GenomeDependentSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1973 2023-04-27 21:53:05.000000 novel_swarms-0.1.4a0/src/novel_swarms/sensors/RegionalSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      665 2023-05-22 22:11:21.000000 novel_swarms-0.1.4a0/src/novel_swarms/sensors/SensorFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1818 2023-05-19 18:16:53.000000 novel_swarms-0.1.4a0/src/novel_swarms/sensors/SensorSet.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      304 2023-05-22 22:27:55.000000 novel_swarms-0.1.4a0/src/novel_swarms/sensors/StaticSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:21.000000 novel_swarms-0.1.4a0/src/novel_swarms/sensors/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/util/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:29.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/util/collider/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1072 2023-03-04 01:09:15.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/collider/AABB.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2396 2023-03-13 18:33:33.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/collider/AngleSensitiveCC.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1024 2023-04-18 16:06:10.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/collider/CircularCollider.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/collider/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/util/conversion/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1832 2023-05-17 18:31:53.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/conversion/ControllerConverter.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/conversion/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/util/datasets/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1182 2023-05-22 22:27:47.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/datasets/DiffDriveDataset.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1553 2022-09-15 20:43:52.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/datasets/GenomeDataSet.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/datasets/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/util/geometry/
--rw-rw-r--   0 connor    (1001) connor    (1001)     5151 2023-04-17 22:41:54.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/geometry/ConvexHull.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1287 2023-05-05 19:12:46.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/geometry/Point.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1184 2023-04-17 21:58:13.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/geometry/Polygon.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/geometry/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3058 2023-04-19 21:01:00.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/labeler.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/util/processing/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/processing/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1693 2023-05-22 22:09:21.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/processing/multicoreprocessing.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/util/signal/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1809 2023-04-21 17:51:53.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/signal/Signal.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-21 17:17:09.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/signal/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      549 2023-03-30 19:03:58.000000 novel_swarms-0.1.4a0/src/novel_swarms/util/timer.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/world/
--rw-rw-r--   0 connor    (1001) connor    (1001)    16018 2023-05-18 23:51:03.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/RectangularWorld.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3115 2023-05-18 22:57:09.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/World.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      273 2022-09-19 15:08:06.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/WorldFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1324 2023-05-22 22:34:57.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/WorldIO.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:45.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/world/generation/
--rw-rw-r--   0 connor    (1001) connor    (1001)     5347 2023-01-17 20:19:42.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/generation/Maze.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 17:04:53.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/generation/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/world/goals/
--rw-rw-r--   0 connor    (1001) connor    (1001)     2151 2023-05-22 22:11:08.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/goals/Goal.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      404 2023-05-22 22:13:27.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/goals/GoalFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1114 2023-05-22 22:14:12.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/goals/GrowthRegion.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 20:36:43.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/goals/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.306271 novel_swarms-0.1.4a0/src/novel_swarms/world/objects/
--rw-rw-r--   0 connor    (1001) connor    (1001)      299 2023-05-22 22:13:03.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/objects/ObjectFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1493 2023-05-22 22:35:12.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/objects/Wall.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      320 2023-05-19 15:46:02.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/objects/WorldObject.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 16:14:14.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/objects/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4955 2023-05-22 22:07:39.000000 novel_swarms-0.1.4a0/src/novel_swarms/world/simulate.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 22:36:56.302271 novel_swarms-0.1.4a0/src/novel_swarms.egg-info/
--rw-rw-r--   0 connor    (1001) connor    (1001)     6796 2023-05-22 22:36:56.000000 novel_swarms-0.1.4a0/src/novel_swarms.egg-info/PKG-INFO
--rw-rw-r--   0 connor    (1001) connor    (1001)     4699 2023-05-22 22:36:56.000000 novel_swarms-0.1.4a0/src/novel_swarms.egg-info/SOURCES.txt
--rw-rw-r--   0 connor    (1001) connor    (1001)        1 2023-05-22 22:36:56.000000 novel_swarms-0.1.4a0/src/novel_swarms.egg-info/dependency_links.txt
--rw-rw-r--   0 connor    (1001) connor    (1001)       22 2023-05-22 22:36:56.000000 novel_swarms-0.1.4a0/src/novel_swarms.egg-info/top_level.txt
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/
+-rw-rw-r--   0 connor    (1001) connor    (1001)      486 2023-04-18 02:45:46.000000 novel_swarms-0.1.5a0/.gitignore
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1107 2023-04-19 20:59:13.000000 novel_swarms-0.1.5a0/LICENSE
+-rw-rw-r--   0 connor    (1001) connor    (1001)       42 2022-09-19 15:01:24.000000 novel_swarms-0.1.5a0/MANIFEST.in
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6796 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/PKG-INFO
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6256 2023-05-22 21:45:25.000000 novel_swarms-0.1.5a0/README.md
+-rw-rw-r--   0 connor    (1001) connor    (1001)       72 2023-04-17 22:17:05.000000 novel_swarms-0.1.5a0/git.sh
+-rw-rw-r--   0 connor    (1001) connor    (1001)      617 2023-06-04 17:22:01.000000 novel_swarms-0.1.5a0/pyproject.toml
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1061 2023-04-27 20:54:12.000000 novel_swarms-0.1.5a0/requirements.txt
+-rw-rw-r--   0 connor    (1001) connor    (1001)       38 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/setup.cfg
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.043483 novel_swarms-0.1.5a0/src/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.5a0/src/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.043483 novel_swarms-0.1.5a0/src/novel_swarms/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-15 20:43:52.000000 novel_swarms-0.1.5a0/src/novel_swarms/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.043483 novel_swarms-0.1.5a0/src/novel_swarms/agent/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1235 2023-06-04 16:53:12.000000 novel_swarms-0.1.5a0/src/novel_swarms/agent/Agent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1472 2023-05-19 17:51:10.000000 novel_swarms-0.1.5a0/src/novel_swarms/agent/AgentFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     7341 2023-04-24 18:59:47.000000 novel_swarms-0.1.5a0/src/novel_swarms/agent/DiffDriveAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6576 2023-05-22 22:11:38.000000 novel_swarms-0.1.5a0/src/novel_swarms/agent/DroneAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1208 2023-04-27 17:48:12.000000 novel_swarms-0.1.5a0/src/novel_swarms/agent/HumanAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4726 2023-05-12 20:50:55.000000 novel_swarms-0.1.5a0/src/novel_swarms/agent/LevyAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     7272 2023-05-19 16:23:44.000000 novel_swarms-0.1.5a0/src/novel_swarms/agent/MazeAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      855 2023-05-22 22:28:16.000000 novel_swarms-0.1.5a0/src/novel_swarms/agent/ModeSwitchingAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2595 2023-03-04 01:21:09.000000 novel_swarms-0.1.5a0/src/novel_swarms/agent/StaticAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     8478 2023-05-26 20:31:00.000000 novel_swarms-0.1.5a0/src/novel_swarms/agent/UnicycleAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:30.000000 novel_swarms-0.1.5a0/src/novel_swarms/agent/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.043483 novel_swarms-0.1.5a0/src/novel_swarms/behavior/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1033 2023-06-04 16:55:56.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/AbstractBehavior.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2085 2023-04-04 14:55:04.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/AgentsAtGoal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1249 2023-05-19 16:08:03.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/AlgebraicConnectivity.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1196 2023-05-19 16:08:03.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/AngularMomentum.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      583 2023-05-19 16:08:03.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/AverageSpeed.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2379 2023-05-22 22:10:50.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/BehaviorFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1340 2023-05-12 16:44:43.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/Centroid.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3349 2023-04-18 15:30:56.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/ConvexHull.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1606 2023-05-22 22:14:28.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/DistanceToGoal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1176 2023-05-19 16:08:03.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/GroupRotationBehavior.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1849 2023-04-18 19:46:18.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/PersistentHomology.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1746 2023-05-19 16:08:03.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/RadialVariance.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1387 2023-04-24 22:53:06.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/ScatterBehavior.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      700 2023-05-19 16:08:03.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/SensorOffset.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      549 2023-05-19 16:08:03.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/SensorRotation.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1514 2023-04-24 23:01:45.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/SensorSignal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      976 2023-06-04 17:16:13.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/SubGroupWrapper.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      616 2023-05-18 23:41:03.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/TotalCollisions.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      898 2023-06-04 17:08:13.000000 novel_swarms-0.1.5a0/src/novel_swarms/behavior/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.043483 novel_swarms-0.1.5a0/src/novel_swarms/cache/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1681 2023-01-17 23:54:56.000000 novel_swarms-0.1.5a0/src/novel_swarms/cache/ExternalSimulationArchive.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 22:42:03.000000 novel_swarms-0.1.5a0/src/novel_swarms/cache/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.043483 novel_swarms-0.1.5a0/src/novel_swarms/config/
+-rw-rw-r--   0 connor    (1001) connor    (1001)    13756 2023-05-19 17:55:12.000000 novel_swarms-0.1.5a0/src/novel_swarms/config/AgentConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1800 2023-03-13 23:06:38.000000 novel_swarms-0.1.5a0/src/novel_swarms/config/EvolutionaryConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2547 2023-06-04 17:00:37.000000 novel_swarms-0.1.5a0/src/novel_swarms/config/HeterogenSwarmConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)       56 2023-05-17 17:50:16.000000 novel_swarms-0.1.5a0/src/novel_swarms/config/ModeConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      637 2023-01-20 15:33:41.000000 novel_swarms-0.1.5a0/src/novel_swarms/config/OutputTensorConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      520 2022-09-15 20:43:52.000000 novel_swarms-0.1.5a0/src/novel_swarms/config/ResultsConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4095 2023-05-22 22:29:31.000000 novel_swarms-0.1.5a0/src/novel_swarms/config/WorldConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:49.000000 novel_swarms-0.1.5a0/src/novel_swarms/config/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1961 2023-05-19 18:43:55.000000 novel_swarms-0.1.5a0/src/novel_swarms/config/defaults.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.043483 novel_swarms-0.1.5a0/src/novel_swarms/gui/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:58.000000 novel_swarms-0.1.5a0/src/novel_swarms/gui/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      479 2023-05-12 21:01:36.000000 novel_swarms-0.1.5a0/src/novel_swarms/gui/abstractGUI.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3431 2023-04-27 22:51:31.000000 novel_swarms-0.1.5a0/src/novel_swarms/gui/agentGUI.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2401 2022-12-07 17:37:58.000000 novel_swarms-0.1.5a0/src/novel_swarms/gui/connectivityGUI.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4143 2023-05-15 22:49:40.000000 novel_swarms-0.1.5a0/src/novel_swarms/gui/controllerGUI.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2670 2022-09-16 18:13:19.000000 novel_swarms-0.1.5a0/src/novel_swarms/gui/evolutionGUI.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/novelty/
+-rw-rw-r--   0 connor    (1001) connor    (1001)    10678 2023-05-22 17:43:57.000000 novel_swarms-0.1.5a0/src/novel_swarms/novelty/BehaviorDiscovery.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     7812 2023-05-22 17:42:55.000000 novel_swarms-0.1.5a0/src/novel_swarms/novelty/GeneRule.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3931 2022-10-26 23:42:12.000000 novel_swarms-0.1.5a0/src/novel_swarms/novelty/NoveltyArchive.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:05.000000 novel_swarms-0.1.5a0/src/novel_swarms/novelty/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3884 2023-05-22 17:31:33.000000 novel_swarms-0.1.5a0/src/novel_swarms/novelty/evolve.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/optim/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6806 2023-05-22 22:14:05.000000 novel_swarms-0.1.5a0/src/novel_swarms/optim/CMAES.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      113 2023-05-03 18:10:54.000000 novel_swarms-0.1.5a0/src/novel_swarms/optim/OptimVar.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-27 15:37:22.000000 novel_swarms-0.1.5a0/src/novel_swarms/optim/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/results/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6926 2023-05-22 18:21:21.000000 novel_swarms-0.1.5a0/src/novel_swarms/results/Cluster.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      612 2022-10-10 15:58:53.000000 novel_swarms-0.1.5a0/src/novel_swarms/results/ClusterPoint.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2728 2023-03-13 21:38:40.000000 novel_swarms-0.1.5a0/src/novel_swarms/results/Trends.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:12.000000 novel_swarms-0.1.5a0/src/novel_swarms/results/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4612 2023-05-22 22:12:51.000000 novel_swarms-0.1.5a0/src/novel_swarms/results/behavior_metrics.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      474 2023-05-22 18:28:05.000000 novel_swarms-0.1.5a0/src/novel_swarms/results/results.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/results/scripts/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.5a0/src/novel_swarms/results/scripts/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4869 2022-09-16 18:58:24.000000 novel_swarms-0.1.5a0/src/novel_swarms/results/scripts/domain_codomain.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/sensors/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1021 2023-01-23 17:59:03.000000 novel_swarms-0.1.5a0/src/novel_swarms/sensors/AbstractSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)    13602 2023-05-19 17:20:52.000000 novel_swarms-0.1.5a0/src/novel_swarms/sensors/BinaryFOVSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4032 2023-05-19 17:21:38.000000 novel_swarms-0.1.5a0/src/novel_swarms/sensors/BinaryLOSSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1779 2023-03-14 00:02:26.000000 novel_swarms-0.1.5a0/src/novel_swarms/sensors/GenomeDependentSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1973 2023-04-27 21:53:05.000000 novel_swarms-0.1.5a0/src/novel_swarms/sensors/RegionalSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      665 2023-05-22 22:11:21.000000 novel_swarms-0.1.5a0/src/novel_swarms/sensors/SensorFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1818 2023-05-19 18:16:53.000000 novel_swarms-0.1.5a0/src/novel_swarms/sensors/SensorSet.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      304 2023-05-22 22:27:55.000000 novel_swarms-0.1.5a0/src/novel_swarms/sensors/StaticSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:21.000000 novel_swarms-0.1.5a0/src/novel_swarms/sensors/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/util/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:29.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/util/collider/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1072 2023-03-04 01:09:15.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/collider/AABB.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2396 2023-03-13 18:33:33.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/collider/AngleSensitiveCC.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1024 2023-04-18 16:06:10.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/collider/CircularCollider.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/collider/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/util/conversion/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1913 2023-05-25 16:57:04.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/conversion/ControllerConverter.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/conversion/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/util/datasets/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1182 2023-05-22 22:27:47.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/datasets/DiffDriveDataset.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1553 2022-09-15 20:43:52.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/datasets/GenomeDataSet.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/datasets/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/util/geometry/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     5151 2023-04-17 22:41:54.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/geometry/ConvexHull.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1287 2023-05-05 19:12:46.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/geometry/Point.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1184 2023-04-17 21:58:13.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/geometry/Polygon.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/geometry/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3058 2023-04-19 21:01:00.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/labeler.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/util/processing/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/processing/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1693 2023-05-22 22:09:21.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/processing/multicoreprocessing.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/util/signal/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1809 2023-04-21 17:51:53.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/signal/Signal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-21 17:17:09.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/signal/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      549 2023-03-30 19:03:58.000000 novel_swarms-0.1.5a0/src/novel_swarms/util/timer.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/world/
+-rw-rw-r--   0 connor    (1001) connor    (1001)    16018 2023-05-18 23:51:03.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/RectangularWorld.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3115 2023-05-18 22:57:09.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/World.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      273 2022-09-19 15:08:06.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/WorldFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1431 2023-05-25 17:55:23.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/WorldIO.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:45.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/world/generation/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     5347 2023-01-17 20:19:42.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/generation/Maze.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 17:04:53.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/generation/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/world/goals/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2151 2023-05-22 22:11:08.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/goals/Goal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      404 2023-05-22 22:13:27.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/goals/GoalFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1114 2023-05-22 22:14:12.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/goals/GrowthRegion.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 20:36:43.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/goals/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/world/objects/
+-rw-rw-r--   0 connor    (1001) connor    (1001)      299 2023-05-22 22:13:03.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/objects/ObjectFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1493 2023-05-22 22:35:12.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/objects/Wall.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      320 2023-05-19 15:46:02.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/objects/WorldObject.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 16:14:14.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/objects/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     5277 2023-05-23 15:39:52.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/simulate.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.047483 novel_swarms-0.1.5a0/src/novel_swarms/world/subscribers/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1279 2023-05-25 15:21:12.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/subscribers/World2Gif.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-05-23 15:21:47.000000 novel_swarms-0.1.5a0/src/novel_swarms/world/subscribers/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-06-04 17:22:08.043483 novel_swarms-0.1.5a0/src/novel_swarms.egg-info/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6796 2023-06-04 17:22:08.000000 novel_swarms-0.1.5a0/src/novel_swarms.egg-info/PKG-INFO
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4839 2023-06-04 17:22:08.000000 novel_swarms-0.1.5a0/src/novel_swarms.egg-info/SOURCES.txt
+-rw-rw-r--   0 connor    (1001) connor    (1001)        1 2023-06-04 17:22:08.000000 novel_swarms-0.1.5a0/src/novel_swarms.egg-info/dependency_links.txt
+-rw-rw-r--   0 connor    (1001) connor    (1001)       22 2023-06-04 17:22:08.000000 novel_swarms-0.1.5a0/src/novel_swarms.egg-info/top_level.txt
```

### Comparing `novel_swarms-0.1.4a0/LICENSE` & `novel_swarms-0.1.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/PKG-INFO` & `novel_swarms-0.1.5a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novel_swarms
-Version: 0.1.4a0
+Version: 0.1.5a0
 Summary: A Swarm Simulation Package
 Author-email: Connor Mattson <c.mattson@utah.edu>
 Project-URL: Homepage, https://github.com/Connor-Mattson/RobotSwarmSimulator
 Project-URL: Bug Tracker, https://github.com/Connor-Mattson/RobotSwarmSimulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `novel_swarms-0.1.4a0/README.md` & `novel_swarms-0.1.5a0/README.md`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/pyproject.toml` & `novel_swarms-0.1.5a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "novel_swarms"
-version = "0.1.4-alpha"
+version = "0.1.5-alpha"
 authors = [
   { name="Connor Mattson", email="c.mattson@utah.edu" },
 ]
 description = "A Swarm Simulation Package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `novel_swarms-0.1.4a0/requirements.txt` & `novel_swarms-0.1.5a0/requirements.txt`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/agent/Agent.py` & `novel_swarms-0.1.5a0/src/novel_swarms/agent/Agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import math
 from numpy import array
 from typing import Tuple
 
 
 class Agent:
 
-    def __init__(self, x, y, name=None, sensors=None, angle=0) -> None:
+    def __init__(self, x, y, name=None, sensors=None, angle=0, group=0) -> None:
         self.x_pos = x
         self.y_pos = y
         self.name = name
         self.dy = 0
         self.dx = 0
         self.angle = angle
         self.sensors = sensors
         self.collision_flag = False
         self.stop_on_collision = False
         self.stopped_duration = 0
         self.detection_id = 0
         self.aabb = None
+        self.group = group
         pass
 
     def step(self, check_for_world_boundaries=None) -> None:
         pass
 
     def draw(self, screen) -> None:
         pass
```

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/agent/AgentFactory.py` & `novel_swarms-0.1.5a0/src/novel_swarms/agent/AgentFactory.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/agent/DiffDriveAgent.py` & `novel_swarms-0.1.5a0/src/novel_swarms/agent/DiffDriveAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/agent/DroneAgent.py` & `novel_swarms-0.1.5a0/src/novel_swarms/agent/DroneAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/agent/HumanAgent.py` & `novel_swarms-0.1.5a0/src/novel_swarms/agent/HumanAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/agent/LevyAgent.py` & `novel_swarms-0.1.5a0/src/novel_swarms/agent/LevyAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/agent/MazeAgent.py` & `novel_swarms-0.1.5a0/src/novel_swarms/agent/MazeAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/agent/ModeSwitchingAgent.py` & `novel_swarms-0.1.5a0/src/novel_swarms/agent/ModeSwitchingAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/agent/StaticAgent.py` & `novel_swarms-0.1.5a0/src/novel_swarms/agent/StaticAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/agent/UnicycleAgent.py` & `novel_swarms-0.1.5a0/src/novel_swarms/agent/UnicycleAgent.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ..util.timer import Timer
 from ..util.collider.AABB import AABB
 from ..util.collider.AngleSensitiveCC import AngleSensitiveCC
 
 
 class UnicycleAgent(Agent):
     SEED = -1
-    DEBUG = False
+    DEBUG = True
 
     def __init__(self, config: UnicycleAgentConfig = None, name=None) -> None:
 
         self.controller = config.controller
 
         if config.seed is not None:
             self.seed(config.seed)
@@ -59,14 +59,15 @@
             if isinstance(sensor, GenomeBinarySensor) or isinstance(sensor, GenomeFOVSensor):
                 sensor.augment_from_genome(config.controller)
 
         self.aabb = None
         self.collider = None
         self.body_filled = config.body_filled
         self.body_color = config.body_color
+        self.c_now = (0, 0)
 
         self.attach_agent_to_sensors()
 
         # Set Trace Settings if a trace was assigned to this object.
         self.trace_color = config.trace_color
         self.trace = config.trace_length is not None
         if self.trace:
@@ -87,14 +88,16 @@
         self.collider = None
 
         if world.goals and world.goals[0].agent_achieved_goal(self):
             v, omega = 0, 0
         else:
             v, omega = self.interpretSensors()
 
+        self.c_now = v, omega
+
         # Define Idiosyncrasies that may occur in actuation/sensing
         idiosync_1 = self.i_1
         idiosync_2 = self.i_2
 
         self.dx = v * math.cos(self.angle) * idiosync_1
         self.dy = v * math.sin(self.angle) * idiosync_1
         dw = omega * idiosync_2
@@ -198,14 +201,15 @@
         v = self.controller[sensor_state * 2]
         omega = self.controller[(sensor_state * 2) + 1]
         return v, omega
 
     def debug_draw(self, screen):
         # self.aabb.draw(screen)
         self.collider.draw(screen)
+        pygame.draw.circle(screen, (255, 0, 255), self.get_icc(), 3, width=0)
 
     def get_action(self):
         return np.array([self.dx * self.dt, self.dy, self.dt])
 
     def get_aabb(self):
         """
         Return the Bounding Box of the agent
@@ -225,9 +229,15 @@
     def add_to_trace(self, x, y):
         if not self.trace:
             return
         self.trace_path.append((x, y))
         if len(self.trace_path) > self.trace_length:
             self.trace_path.pop(0)
 
+    def get_icc(self):
+        v, w = self.c_now
+        r = v / w
+        print(r)
+        return self.x_pos - (r * np.sin(self.angle)), self.y_pos + (r * np.cos(self.angle))
+
     def __str__(self) -> str:
-        return "(x: {}, y: {}, r: {}, θ: {})".format(self.x_pos, self.y_pos, self.radius, self.angle)
+        return "(x: {}, y: {}, r: {}, θ: {})".format(self.x_pos, self.y_pos, self.radius, self.angle)
```

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/AbstractBehavior.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/AbstractBehavior.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,8 +28,11 @@
         self.current_value = 0
         self.value_history = []
 
     def draw(self, screen):
         pass
 
     def as_config_dict(self):
-        return {"name": self.name, "history_size": self.history_size}
+        return {"name": self.name, "history_size": self.history_size}
+
+    def calculate(self):
+        pass
```

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/AgentsAtGoal.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/AgentsAtGoal.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/AlgebraicConnectivity.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/AlgebraicConnectivity.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/AngularMomentum.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/AngularMomentum.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/AverageSpeed.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/AverageSpeed.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/BehaviorFactory.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/BehaviorFactory.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/Centroid.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/Centroid.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/ConvexHull.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/ConvexHull.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/DistanceToGoal.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/DistanceToGoal.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/GroupRotationBehavior.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/GroupRotationBehavior.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/PersistentHomology.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/PersistentHomology.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/RadialVariance.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/RadialVariance.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/ScatterBehavior.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/ScatterBehavior.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/SensorOffset.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/SensorOffset.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/SensorRotation.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/SensorRotation.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/SensorSignal.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/SensorSignal.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/behavior/TotalCollisions.py` & `novel_swarms-0.1.5a0/src/novel_swarms/behavior/TotalCollisions.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/cache/ExternalSimulationArchive.py` & `novel_swarms-0.1.5a0/src/novel_swarms/cache/ExternalSimulationArchive.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/config/AgentConfig.py` & `novel_swarms-0.1.5a0/src/novel_swarms/config/AgentConfig.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/config/EvolutionaryConfig.py` & `novel_swarms-0.1.5a0/src/novel_swarms/config/EvolutionaryConfig.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/config/HeterogenSwarmConfig.py` & `novel_swarms-0.1.5a0/src/novel_swarms/config/HeterogenSwarmConfig.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,18 +14,21 @@
         return self.subpopulation_information.keys()
 
     def get_counts(self):
         return self.subpopulation_information.values()
 
     def build_agent_population(self):
         population = []
+        group = 0
         for key in self.subpopulation_information:
             for n in range(self.subpopulation_information[key]):
                 agent = AgentFactory.create(key)
+                agent.group = group
                 population.append(agent)
+            group += 1
         return population
 
     def attach_world_config(self, world_config):
         self.world = world_config
         for key in self.subpopulation_information:
             key.attach_world_config(world_config)
```

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/config/OutputTensorConfig.py` & `novel_swarms-0.1.5a0/src/novel_swarms/config/OutputTensorConfig.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/config/ResultsConfig.py` & `novel_swarms-0.1.5a0/src/novel_swarms/config/ResultsConfig.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/config/WorldConfig.py` & `novel_swarms-0.1.5a0/src/novel_swarms/config/WorldConfig.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/config/defaults.py` & `novel_swarms-0.1.5a0/src/novel_swarms/config/defaults.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/gui/agentGUI.py` & `novel_swarms-0.1.5a0/src/novel_swarms/gui/agentGUI.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/gui/connectivityGUI.py` & `novel_swarms-0.1.5a0/src/novel_swarms/gui/connectivityGUI.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/gui/controllerGUI.py` & `novel_swarms-0.1.5a0/src/novel_swarms/gui/controllerGUI.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/gui/evolutionGUI.py` & `novel_swarms-0.1.5a0/src/novel_swarms/gui/evolutionGUI.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/novelty/BehaviorDiscovery.py` & `novel_swarms-0.1.5a0/src/novel_swarms/novelty/BehaviorDiscovery.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/novelty/GeneRule.py` & `novel_swarms-0.1.5a0/src/novel_swarms/novelty/GeneRule.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/novelty/NoveltyArchive.py` & `novel_swarms-0.1.5a0/src/novel_swarms/novelty/NoveltyArchive.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/novelty/evolve.py` & `novel_swarms-0.1.5a0/src/novel_swarms/novelty/evolve.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/optim/CMAES.py` & `novel_swarms-0.1.5a0/src/novel_swarms/optim/CMAES.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/results/Cluster.py` & `novel_swarms-0.1.5a0/src/novel_swarms/results/Cluster.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/results/ClusterPoint.py` & `novel_swarms-0.1.5a0/src/novel_swarms/results/ClusterPoint.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/results/Trends.py` & `novel_swarms-0.1.5a0/src/novel_swarms/results/Trends.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/results/behavior_metrics.py` & `novel_swarms-0.1.5a0/src/novel_swarms/results/behavior_metrics.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/results/scripts/domain_codomain.py` & `novel_swarms-0.1.5a0/src/novel_swarms/results/scripts/domain_codomain.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/sensors/AbstractSensor.py` & `novel_swarms-0.1.5a0/src/novel_swarms/sensors/AbstractSensor.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/sensors/BinaryFOVSensor.py` & `novel_swarms-0.1.5a0/src/novel_swarms/sensors/BinaryFOVSensor.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/sensors/BinaryLOSSensor.py` & `novel_swarms-0.1.5a0/src/novel_swarms/sensors/BinaryLOSSensor.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/sensors/GenomeDependentSensor.py` & `novel_swarms-0.1.5a0/src/novel_swarms/sensors/GenomeDependentSensor.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/sensors/RegionalSensor.py` & `novel_swarms-0.1.5a0/src/novel_swarms/sensors/RegionalSensor.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/sensors/SensorFactory.py` & `novel_swarms-0.1.5a0/src/novel_swarms/sensors/SensorFactory.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/sensors/SensorSet.py` & `novel_swarms-0.1.5a0/src/novel_swarms/sensors/SensorSet.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/util/collider/AABB.py` & `novel_swarms-0.1.5a0/src/novel_swarms/util/collider/AABB.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/util/collider/AngleSensitiveCC.py` & `novel_swarms-0.1.5a0/src/novel_swarms/util/collider/AngleSensitiveCC.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/util/collider/CircularCollider.py` & `novel_swarms-0.1.5a0/src/novel_swarms/util/collider/CircularCollider.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/util/conversion/ControllerConverter.py` & `novel_swarms-0.1.5a0/src/novel_swarms/util/conversion/ControllerConverter.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,13 +43,15 @@
 
         v_r, v_l = self.from_controller[0], self.from_controller[1]
         v_off = (v_r + v_l) / 2
         dtheta_off = (v_r - v_l) / 7
         return [dtheta_on / dtheta_off, v_on / v_off]
 
 if __name__ == "__main__":
-    wheel_radius = 2.0
-    agent_radius = 5.0
-    input_controller = [0.2, 0.7, -0.5, -0.1]
+    wheel_radius = 4.1
+    agent_radius = 15.1 / 2
+    input_controller = [0.65, 1.0, 0.4, 0.5]
+    SCALE = 4.5
+    input_controller = [i * SCALE for i in input_controller]
 
     converter = DiffDriveToUnicycle(input_controller, agent_radius, wheel_radius)
     print(converter.convert())
```

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/util/datasets/DiffDriveDataset.py` & `novel_swarms-0.1.5a0/src/novel_swarms/util/datasets/DiffDriveDataset.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/util/datasets/GenomeDataSet.py` & `novel_swarms-0.1.5a0/src/novel_swarms/util/datasets/GenomeDataSet.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/util/geometry/ConvexHull.py` & `novel_swarms-0.1.5a0/src/novel_swarms/util/geometry/ConvexHull.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/util/geometry/Point.py` & `novel_swarms-0.1.5a0/src/novel_swarms/util/geometry/Point.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/util/geometry/Polygon.py` & `novel_swarms-0.1.5a0/src/novel_swarms/util/geometry/Polygon.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/util/labeler.py` & `novel_swarms-0.1.5a0/src/novel_swarms/util/labeler.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/util/processing/multicoreprocessing.py` & `novel_swarms-0.1.5a0/src/novel_swarms/util/processing/multicoreprocessing.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/util/signal/Signal.py` & `novel_swarms-0.1.5a0/src/novel_swarms/util/signal/Signal.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/util/timer.py` & `novel_swarms-0.1.5a0/src/novel_swarms/util/timer.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/world/RectangularWorld.py` & `novel_swarms-0.1.5a0/src/novel_swarms/world/RectangularWorld.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/world/World.py` & `novel_swarms-0.1.5a0/src/novel_swarms/world/World.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/world/WorldIO.py` & `novel_swarms-0.1.5a0/src/novel_swarms/world/WorldIO.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,17 +28,20 @@
     @staticmethod
     def sim_from_json(file_name):
         from src.novel_swarms.config.WorldConfig import RectangularWorldConfig
         from src.novel_swarms.world.simulate import main as sim
 
         d = WorldIO.load_world_dictionary(file_name)
         config = RectangularWorldConfig.from_dict(d)
+        # for c in config.agentConfig.get_configs():
+        #     c.body_filled = True
+        #     c.agent_radius = 7
         sim(config)
 
 
 
 """
 Given a File, JSON_WORLD, simulate the entire experiment with a single function call
 """
 if __name__ == "__main__":
-    JSON_WORLD = "../../../demo/results/experiments/heterogeneous_behaviors/embedded-cycles-heterogeneous.json"
+    JSON_WORLD = "../../../demo/results/experiments/heterogeneous_behaviors/gmu-nested-mill.json"
     WorldIO.sim_from_json(JSON_WORLD)
```

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/world/generation/Maze.py` & `novel_swarms-0.1.5a0/src/novel_swarms/world/generation/Maze.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/world/goals/Goal.py` & `novel_swarms-0.1.5a0/src/novel_swarms/world/goals/Goal.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/world/goals/GrowthRegion.py` & `novel_swarms-0.1.5a0/src/novel_swarms/world/goals/GrowthRegion.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/world/objects/Wall.py` & `novel_swarms-0.1.5a0/src/novel_swarms/world/objects/Wall.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms/world/simulate.py` & `novel_swarms-0.1.5a0/src/novel_swarms/world/simulate.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     # define a variable to control the main loop
     running = True
     paused = False
     draw_world = True
 
     # Create the simulation world
     world = WorldFactory.create(world_config)
+    world_subscribers = []
 
     # Create the GUI
     if show_gui and not gui:
         gui = DifferentialDriveGUI(x=world_config.w, y=0, h=world_config.h, w=gui_width)
 
     # Attach the world to the gui and vice versa
     if gui:
@@ -78,14 +79,17 @@
                         steps_per_frame /= 2
                         steps_per_frame = round(steps_per_frame)
                     if event.key == pygame.K_w:
                         draw_world = not draw_world
                     if event.key == pygame.K_F3:
                         from .WorldIO import WorldIO
                         WorldIO.save_world(world)
+                    if event.key == pygame.K_F4:
+                        from .subscribers.World2Gif import World2Gif
+                        world_subscribers.append(World2Gif())
                     if world_key_events:
                         world.handle_key_press(event)
                     if gui and gui_key_events:
                         gui.pass_key_events(event)
                     if event.key in labels:
                         return event.key, steps_taken
 
@@ -111,14 +115,18 @@
             if total_allowed_steps is not None:
                 # noinspection PyTypeChecker
                 if steps_taken > total_allowed_steps:
                     running = False
                     return world
 
             world.step()
+
+            # Broadcast to any world subscribers
+            _ = [sub.notify(screen) for sub in world_subscribers]
+
             steps_taken += 1
             # if steps_taken % 1000 == 0:
             # print(f"Total steps: {steps_taken}")
 
         # Draw!
         if gui and screen:
             gui.set_time(steps_taken)
@@ -128,9 +136,7 @@
             gui.step()
             gui.draw(screen)
 
         # Limit the FPS of the simulation to FRAMERATE
         if gui:
             pygame.display.flip()
             pygame.time.Clock().tick(FRAMERATE)
-
-
```

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms.egg-info/PKG-INFO` & `novel_swarms-0.1.5a0/src/novel_swarms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novel-swarms
-Version: 0.1.4a0
+Version: 0.1.5a0
 Summary: A Swarm Simulation Package
 Author-email: Connor Mattson <c.mattson@utah.edu>
 Project-URL: Homepage, https://github.com/Connor-Mattson/RobotSwarmSimulator
 Project-URL: Bug Tracker, https://github.com/Connor-Mattson/RobotSwarmSimulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `novel_swarms-0.1.4a0/src/novel_swarms.egg-info/SOURCES.txt` & `novel_swarms-0.1.5a0/src/novel_swarms.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 src/novel_swarms/behavior/GroupRotationBehavior.py
 src/novel_swarms/behavior/PersistentHomology.py
 src/novel_swarms/behavior/RadialVariance.py
 src/novel_swarms/behavior/ScatterBehavior.py
 src/novel_swarms/behavior/SensorOffset.py
 src/novel_swarms/behavior/SensorRotation.py
 src/novel_swarms/behavior/SensorSignal.py
+src/novel_swarms/behavior/SubGroupWrapper.py
 src/novel_swarms/behavior/TotalCollisions.py
 src/novel_swarms/behavior/__init__.py
 src/novel_swarms/cache/ExternalSimulationArchive.py
 src/novel_swarms/cache/__init__.py
 src/novel_swarms/config/AgentConfig.py
 src/novel_swarms/config/EvolutionaryConfig.py
 src/novel_swarms/config/HeterogenSwarmConfig.py
@@ -113,8 +114,10 @@
 src/novel_swarms/world/goals/Goal.py
 src/novel_swarms/world/goals/GoalFactory.py
 src/novel_swarms/world/goals/GrowthRegion.py
 src/novel_swarms/world/goals/__init__.py
 src/novel_swarms/world/objects/ObjectFactory.py
 src/novel_swarms/world/objects/Wall.py
 src/novel_swarms/world/objects/WorldObject.py
-src/novel_swarms/world/objects/__init__.py
+src/novel_swarms/world/objects/__init__.py
+src/novel_swarms/world/subscribers/World2Gif.py
+src/novel_swarms/world/subscribers/__init__.py
```

