# Comparing `tmp/csle_ryu-0.2.5.tar.gz` & `tmp/csle_ryu-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_ryu-0.2.5.tar", last modified: Sun Jun  4 07:13:38 2023, max compression
+gzip compressed data, was "csle_ryu-0.2.6.tar", last modified: Sun Jun  4 07:39:16 2023, max compression
```

## Comparing `csle_ryu-0.2.5.tar` & `csle_ryu-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.485390 csle_ryu-0.2.5/
--rw-rw-r--   0 kim       (1000) kim       (1000)      639 2023-06-04 07:13:38.485390 csle_ryu-0.2.5/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     3913 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      669 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1244 2023-06-04 07:13:38.485390 csle_ryu-0.2.5/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.481390 csle_ryu-0.2.5/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.481390 csle_ryu-0.2.5/src/csle_ryu/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 07:13:34.000000 csle_ryu-0.2.5/src/csle_ryu/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.481390 csle_ryu-0.2.5/src/csle_ryu/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2484 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.481390 csle_ryu-0.2.5/src/csle_ryu/controllers/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/controllers/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8323 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/controllers/learning_switch_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11773 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/controllers/learning_switch_stp_controller.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.485390 csle_ryu-0.2.5/src/csle_ryu/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4598 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/agg_flow_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8629 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/avg_flow_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15102 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/avg_port_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7004 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/flow_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10600 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/port_statistic.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      253 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/dao/ryu_controller_type.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.485390 csle_ryu-0.2.5/src/csle_ryu/monitor/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/monitor/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14663 2023-03-28 14:03:22.000000 csle_ryu-0.2.5/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:13:38.481390 csle_ryu-0.2.5/src/csle_ryu.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      639 2023-06-04 07:13:38.000000 csle_ryu-0.2.5/src/csle_ryu.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      873 2023-06-04 07:13:38.000000 csle_ryu-0.2.5/src/csle_ryu.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 07:13:38.000000 csle_ryu-0.2.5/src/csle_ryu.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:28.000000 csle_ryu-0.2.5/src/csle_ryu.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      230 2023-06-04 07:13:38.000000 csle_ryu-0.2.5/src/csle_ryu.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        9 2023-06-04 07:13:38.000000 csle_ryu-0.2.5/src/csle_ryu.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:39:16.065703 csle_ryu-0.2.6/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      639 2023-06-04 07:39:16.065703 csle_ryu-0.2.6/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3913 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      669 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1244 2023-06-04 07:39:16.065703 csle_ryu-0.2.6/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:39:16.065703 csle_ryu-0.2.6/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:39:16.065703 csle_ryu-0.2.6/src/csle_ryu/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 07:39:12.000000 csle_ryu-0.2.6/src/csle_ryu/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:39:16.065703 csle_ryu-0.2.6/src/csle_ryu/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2484 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:39:16.065703 csle_ryu-0.2.6/src/csle_ryu/controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8323 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/controllers/learning_switch_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11773 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/controllers/learning_switch_stp_controller.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:39:16.065703 csle_ryu-0.2.6/src/csle_ryu/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4598 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/dao/agg_flow_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8629 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/dao/avg_flow_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15102 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/dao/avg_port_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7004 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/dao/flow_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10600 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/dao/port_statistic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      253 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/dao/ryu_controller_type.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:39:16.065703 csle_ryu-0.2.6/src/csle_ryu/monitor/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/monitor/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14663 2023-03-28 14:03:22.000000 csle_ryu-0.2.6/src/csle_ryu/monitor/flow_and_port_stats_monitor.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:39:16.065703 csle_ryu-0.2.6/src/csle_ryu.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      639 2023-06-04 07:39:15.000000 csle_ryu-0.2.6/src/csle_ryu.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      873 2023-06-04 07:39:16.000000 csle_ryu-0.2.6/src/csle_ryu.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 07:39:15.000000 csle_ryu-0.2.6/src/csle_ryu.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:28.000000 csle_ryu-0.2.6/src/csle_ryu.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      230 2023-06-04 07:39:15.000000 csle_ryu-0.2.6/src/csle_ryu.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        9 2023-06-04 07:39:16.000000 csle_ryu-0.2.6/src/csle_ryu.egg-info/top_level.txt
```

### Comparing `csle_ryu-0.2.5/PKG-INFO` & `csle_ryu-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_ryu
-Version: 0.2.5
+Version: 0.2.6
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.2.5/README.md` & `csle_ryu-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.5/pyproject.toml` & `csle_ryu-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.5/setup.cfg` & `csle_ryu-0.2.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-collector>=0.2.5
+	csle-collector>=0.2.6
 	ryu>=4.34
 	eventlet>=0.30.2
 	confluent-kafka>=1.9.2
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
```

### Comparing `csle_ryu-0.2.5/src/csle_ryu/constants/constants.py` & `csle_ryu-0.2.6/src/csle_ryu/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.5/src/csle_ryu/controllers/learning_switch_controller.py` & `csle_ryu-0.2.6/src/csle_ryu/controllers/learning_switch_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.5/src/csle_ryu/controllers/learning_switch_stp_controller.py` & `csle_ryu-0.2.6/src/csle_ryu/controllers/learning_switch_stp_controller.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.5/src/csle_ryu/dao/agg_flow_statistic.py` & `csle_ryu-0.2.6/src/csle_ryu/dao/agg_flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.5/src/csle_ryu/dao/avg_flow_statistic.py` & `csle_ryu-0.2.6/src/csle_ryu/dao/avg_flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.5/src/csle_ryu/dao/avg_port_statistic.py` & `csle_ryu-0.2.6/src/csle_ryu/dao/avg_port_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.5/src/csle_ryu/dao/flow_statistic.py` & `csle_ryu-0.2.6/src/csle_ryu/dao/flow_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.5/src/csle_ryu/dao/port_statistic.py` & `csle_ryu-0.2.6/src/csle_ryu/dao/port_statistic.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.5/src/csle_ryu/monitor/flow_and_port_stats_monitor.py` & `csle_ryu-0.2.6/src/csle_ryu/monitor/flow_and_port_stats_monitor.py`

 * *Files identical despite different names*

### Comparing `csle_ryu-0.2.5/src/csle_ryu.egg-info/PKG-INFO` & `csle_ryu-0.2.6/src/csle_ryu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-ryu
-Version: 0.2.5
+Version: 0.2.6
 Summary: RYU SDN Controllers in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_ryu-0.2.5/src/csle_ryu.egg-info/SOURCES.txt` & `csle_ryu-0.2.6/src/csle_ryu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

