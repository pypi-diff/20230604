# Comparing `tmp/csle_ryu-0.2.4.tar.gz` & `tmp/csle_ryu-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_ryu-0.2.4.tar", last modified: Wed May 31 13:42:11 2023, max compression
+gzip compressed data, was "csle_ryu-0.2.5.tar", last modified: Sun Jun  4 07:13:38 2023, max compression
```

## Comparing `csle_ryu-0.2.4.tar` & `csle_ryu-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:11.486201 csle_ryu-0.2.4/
--rw-r--r--   0 kimham     (501) staff       (20)      639 2023-05-31 13:42:11.486316 csle_ryu-0.2.4/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     3913 2023-01-11 18:45:47.000000 csle_ryu-0.2.4/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      669 2023-02-12 08:59:32.000000 csle_ryu-0.2.4/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1244 2023-05-31 13:42:11.486857 csle_ryu-0.2.4/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_ryu-0.2.4/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:11.473791 csle_ryu-0.2.4/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:11.476514 csle_ryu-0.2.4/src/csle_ryu/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_ryu-0.2.4/src/csle_ryu/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 13:42:03.000000 csle_ryu-0.2.4/src/csle_ryu/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:11.479498 csle_ryu-0.2.4/src/csle_ryu/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.2.4/src/csle_ryu/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2484 2023-03-31 11:14:06.000000 csle_ryu-0.2.4/src/csle_ryu/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:11.480856 csle_ryu-0.2.4/src/csle_ryu/controllers/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.2.4/src/csle_ryu/controllers/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     8323 2022-11-28 13:00:49.000000 csle_ryu-0.2.4/src/csle_ryu/controllers/learning_switch_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    11773 2022-12-07 10:40:04.000000 csle_ryu-0.2.4/src/csle_ryu/controllers/learning_switch_stp_controller.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:11.484925 csle_ryu-0.2.4/src/csle_ryu/dao/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.2.4/src/csle_ryu/dao/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     4598 2023-03-22 11:50:26.000000 csle_ryu-0.2.4/src/csle_ryu/dao/agg_flow_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)     8629 2023-03-22 11:50:26.000000 csle_ryu-0.2.4/src/csle_ryu/dao/avg_flow_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)    15102 2023-03-22 11:50:26.000000 csle_ryu-0.2.4/src/csle_ryu/dao/avg_port_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)     7004 2023-03-22 11:50:26.000000 csle_ryu-0.2.4/src/csle_ryu/dao/flow_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)    10600 2023-03-22 11:50:26.000000 csle_ryu-0.2.4/src/csle_ryu/dao/port_statistic.py
--rw-r--r--   0 kimham     (501) staff       (20)      253 2022-11-28 13:00:49.000000 csle_ryu-0.2.4/src/csle_ryu/dao/ryu_controller_type.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:11.485736 csle_ryu-0.2.4/src/csle_ryu/monitor/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_ryu-0.2.4/src/csle_ryu/monitor/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    14663 2023-03-31 11:14:06.000000 csle_ryu-0.2.4/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:42:11.479023 csle_ryu-0.2.4/src/csle_ryu.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      639 2023-05-31 13:42:11.000000 csle_ryu-0.2.4/src/csle_ryu.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      873 2023-05-31 13:42:11.000000 csle_ryu-0.2.4/src/csle_ryu.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 13:42:11.000000 csle_ryu-0.2.4/src/csle_ryu.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:06.000000 csle_ryu-0.2.4/src/csle_ryu.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      230 2023-05-31 13:42:11.000000 csle_ryu-0.2.4/src/csle_ryu.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)        9 2023-05-31 13:42:11.000000 csle_ryu-0.2.4/src/csle_ryu.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.485390 csle_ryu-0.2.5/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      639 2023-06-04 07:13:38.485390 csle_ryu-0.2.5/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3913 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      669 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1244 2023-06-04 07:13:38.485390 csle_ryu-0.2.5/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.481390 csle_ryu-0.2.5/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.481390 csle_ryu-0.2.5/src/csle_ryu/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 07:13:34.000000 csle_ryu-0.2.5/src/csle_ryu/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.481390 csle_ryu-0.2.5/src/csle_ryu/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2484 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.481390 csle_ryu-0.2.5/src/csle_ryu/controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8323 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/controllers/learning_switch_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11773 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/controllers/learning_switch_stp_controller.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.485390 csle_ryu-0.2.5/src/csle_ryu/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4598 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/agg_flow_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8629 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/avg_flow_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15102 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/avg_port_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7004 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/flow_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10600 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/port_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      253 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/ryu_controller_type.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.485390 csle_ryu-0.2.5/src/csle_ryu/monitor/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/monitor/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14663 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.481390 csle_ryu-0.2.5/src/csle_ryu.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      639 2023-06-04 07:13:38.000000 csle_ryu-0.2.5/src/csle_ryu.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      873 2023-06-04 07:13:38.000000 csle_ryu-0.2.5/src/csle_ryu.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 07:13:38.000000 csle_ryu-0.2.5/src/csle_ryu.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:28.000000 csle_ryu-0.2.5/src/csle_ryu.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      230 2023-06-04 07:13:38.000000 csle_ryu-0.2.5/src/csle_ryu.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        9 2023-06-04 07:13:38.000000 csle_ryu-0.2.5/src/csle_ryu.egg-info/top_level.txt
```

### Comparing `csle_ryu-0.2.4/PKG-INFO` & `csle_ryu-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_ryu
-Version: 0.2.4
+Version: 0.2.5
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.2.4/README.md` & `csle_ryu-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.4/pyproject.toml` & `csle_ryu-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.4/setup.cfg` & `csle_ryu-0.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-collector>=0.2.4
+	csle-collector>=0.2.5
 	ryu>=4.34
 	eventlet>=0.30.2
 	confluent-kafka>=1.9.2
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
```

### Comparing `csle_ryu-0.2.4/src/csle_ryu/constants/constants.py` & `csle_ryu-0.2.5/src/csle_ryu/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.4/src/csle_ryu/controllers/learning_switch_controller.py` & `csle_ryu-0.2.5/src/csle_ryu/controllers/learning_switch_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.4/src/csle_ryu/controllers/learning_switch_stp_controller.py` & `csle_ryu-0.2.5/src/csle_ryu/controllers/learning_switch_stp_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.4/src/csle_ryu/dao/agg_flow_statistic.py` & `csle_ryu-0.2.5/src/csle_ryu/dao/agg_flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.4/src/csle_ryu/dao/avg_flow_statistic.py` & `csle_ryu-0.2.5/src/csle_ryu/dao/avg_flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.4/src/csle_ryu/dao/avg_port_statistic.py` & `csle_ryu-0.2.5/src/csle_ryu/dao/avg_port_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.4/src/csle_ryu/dao/flow_statistic.py` & `csle_ryu-0.2.5/src/csle_ryu/dao/flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.4/src/csle_ryu/dao/port_statistic.py` & `csle_ryu-0.2.5/src/csle_ryu/dao/port_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.4/src/csle_ryu/monitor/flow_and_port_stats_monitor.py` & `csle_ryu-0.2.5/src/csle_ryu/monitor/flow_and_port_stats_monitor.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.4/src/csle_ryu.egg-info/PKG-INFO` & `csle_ryu-0.2.5/src/csle_ryu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-ryu
-Version: 0.2.4
+Version: 0.2.5
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.2.4/src/csle_ryu.egg-info/SOURCES.txt` & `csle_ryu-0.2.5/src/csle_ryu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

