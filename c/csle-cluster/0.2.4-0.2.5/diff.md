# Comparing `tmp/csle_cluster-0.2.4.tar.gz` & `tmp/csle_cluster-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cluster-0.2.4.tar", last modified: Wed May 31 13:46:12 2023, max compression
+gzip compressed data, was "csle_cluster-0.2.5.tar", last modified: Sun Jun  4 07:15:22 2023, max compression
```

## Comparing `csle_cluster-0.2.4.tar` & `csle_cluster-0.2.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:46:12.428485 csle_cluster-0.2.4/
--rw-r--r--   0 kimham     (501) staff       (20)      804 2023-05-31 13:46:12.428637 csle_cluster-0.2.4/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     4256 2023-03-05 07:26:30.000000 csle_cluster-0.2.4/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      672 2023-02-12 09:12:26.000000 csle_cluster-0.2.4/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1406 2023-05-31 13:46:12.429372 csle_cluster-0.2.4/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_cluster-0.2.4/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:46:12.410495 csle_cluster-0.2.4/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:46:12.412929 csle_cluster-0.2.4/src/csle_cluster/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2023-02-12 09:44:18.000000 csle_cluster-0.2.4/src/csle_cluster/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 13:42:03.000000 csle_cluster-0.2.4/src/csle_cluster/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:46:12.424789 csle_cluster-0.2.4/src/csle_cluster/cluster_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_cluster-0.2.4/src/csle_cluster/cluster_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)   229454 2023-05-31 11:33:47.000000 csle_cluster-0.2.4/src/csle_cluster/cluster_manager/cluster_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)   269186 2023-05-01 07:57:15.000000 csle_cluster-0.2.4/src/csle_cluster/cluster_manager/cluster_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)   197343 2023-03-31 11:14:06.000000 csle_cluster-0.2.4/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)   349502 2023-03-31 11:14:06.000000 csle_cluster-0.2.4/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)   202990 2023-03-31 11:14:06.000000 csle_cluster-0.2.4/src/csle_cluster/cluster_manager/cluster_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)   188175 2023-04-19 06:25:48.000000 csle_cluster-0.2.4/src/csle_cluster/cluster_manager/query_cluster_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:46:12.427649 csle_cluster-0.2.4/src/csle_cluster/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-03-05 07:26:30.000000 csle_cluster-0.2.4/src/csle_cluster/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      375 2023-03-16 16:24:28.000000 csle_cluster-0.2.4/src/csle_cluster/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:46:12.414752 csle_cluster-0.2.4/src/csle_cluster.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      804 2023-05-31 13:46:11.000000 csle_cluster-0.2.4/src/csle_cluster.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      805 2023-05-31 13:46:12.000000 csle_cluster-0.2.4/src/csle_cluster.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 13:46:12.000000 csle_cluster-0.2.4/src/csle_cluster.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-02-12 09:44:23.000000 csle_cluster-0.2.4/src/csle_cluster.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      251 2023-05-31 13:46:12.000000 csle_cluster-0.2.4/src/csle_cluster.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       13 2023-05-31 13:46:12.000000 csle_cluster-0.2.4/src/csle_cluster.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:15:22.253067 csle_cluster-0.2.5/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      804 2023-06-04 07:15:22.253067 csle_cluster-0.2.5/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4256 2023-03-28 14:03:22.000000 csle_cluster-0.2.5/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      672 2023-03-28 14:03:22.000000 csle_cluster-0.2.5/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1406 2023-06-04 07:15:22.253067 csle_cluster-0.2.5/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cluster-0.2.5/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:15:22.229067 csle_cluster-0.2.5/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:15:22.237067 csle_cluster-0.2.5/src/csle_cluster/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_cluster-0.2.5/src/csle_cluster/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 07:13:34.000000 csle_cluster-0.2.5/src/csle_cluster/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:15:22.253067 csle_cluster-0.2.5/src/csle_cluster/cluster_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.2.5/src/csle_cluster/cluster_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   229454 2023-06-04 07:11:42.000000 csle_cluster-0.2.5/src/csle_cluster/cluster_manager/cluster_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   269186 2023-05-03 08:18:28.000000 csle_cluster-0.2.5/src/csle_cluster/cluster_manager/cluster_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   197343 2023-03-28 14:03:22.000000 csle_cluster-0.2.5/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   349502 2023-03-28 14:03:22.000000 csle_cluster-0.2.5/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   202990 2023-03-28 14:03:22.000000 csle_cluster-0.2.5/src/csle_cluster/cluster_manager/cluster_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   188175 2023-04-18 12:48:07.000000 csle_cluster-0.2.5/src/csle_cluster/cluster_manager/query_cluster_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:15:22.253067 csle_cluster-0.2.5/src/csle_cluster/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.2.5/src/csle_cluster/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      375 2023-03-28 14:03:22.000000 csle_cluster-0.2.5/src/csle_cluster/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:15:22.241067 csle_cluster-0.2.5/src/csle_cluster.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      804 2023-06-04 07:15:21.000000 csle_cluster-0.2.5/src/csle_cluster.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      805 2023-06-04 07:15:22.000000 csle_cluster-0.2.5/src/csle_cluster.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 07:15:21.000000 csle_cluster-0.2.5/src/csle_cluster.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-04 13:33:55.000000 csle_cluster-0.2.5/src/csle_cluster.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      251 2023-06-04 07:15:22.000000 csle_cluster-0.2.5/src/csle_cluster.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       13 2023-06-04 07:15:22.000000 csle_cluster-0.2.5/src/csle_cluster.egg-info/top_level.txt
```

### Comparing `csle_cluster-0.2.4/PKG-INFO` & `csle_cluster-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cluster
-Version: 0.2.4
+Version: 0.2.5
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.2.4/README.md` & `csle_cluster-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.4/pyproject.toml` & `csle_cluster-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.4/setup.cfg` & `csle_cluster-0.2.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	grpcio>=1.27.2
 	grpcio-tools>=1.27.2
-	csle-collector>=0.2.4
-	csle-common>=0.2.4
-	csle-ryu>=0.2.4
+	csle-collector>=0.2.5
+	csle-common>=0.2.5
+	csle-ryu>=0.2.5
 python_requires = >=3.5
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cluster-0.2.4/src/csle_cluster/cluster_manager/cluster_controller.py` & `csle_cluster-0.2.5/src/csle_cluster/cluster_manager/cluster_controller.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.4/src/csle_cluster/cluster_manager/cluster_manager.py` & `csle_cluster-0.2.5/src/csle_cluster/cluster_manager/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.4/src/csle_cluster/cluster_manager/cluster_manager_pb2.py` & `csle_cluster-0.2.5/src/csle_cluster/cluster_manager/cluster_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.4/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py` & `csle_cluster-0.2.5/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.4/src/csle_cluster/cluster_manager/cluster_manager_util.py` & `csle_cluster-0.2.5/src/csle_cluster/cluster_manager/cluster_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.4/src/csle_cluster/cluster_manager/query_cluster_manager.py` & `csle_cluster-0.2.5/src/csle_cluster/cluster_manager/query_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.4/src/csle_cluster.egg-info/PKG-INFO` & `csle_cluster-0.2.5/src/csle_cluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cluster
-Version: 0.2.4
+Version: 0.2.5
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.2.4/src/csle_cluster.egg-info/SOURCES.txt` & `csle_cluster-0.2.5/src/csle_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

