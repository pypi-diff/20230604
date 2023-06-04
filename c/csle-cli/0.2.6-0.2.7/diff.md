# Comparing `tmp/csle_cli-0.2.6.tar.gz` & `tmp/csle_cli-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cli-0.2.6.tar", last modified: Sun Jun  4 07:41:01 2023, max compression
+gzip compressed data, was "csle_cli-0.2.7.tar", last modified: Sun Jun  4 08:34:08 2023, max compression
```

## Comparing `csle_cli-0.2.6.tar` & `csle_cli-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:41:01.210060 csle_cli-0.2.6/
--rw-rw-r--   0 kim       (1000) kim       (1000)      629 2023-06-04 07:41:01.210060 csle_cli-0.2.6/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)    22943 2023-03-28 14:03:22.000000 csle_cli-0.2.6/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      668 2023-03-28 14:03:22.000000 csle_cli-0.2.6/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1368 2023-06-04 07:41:01.210060 csle_cli-0.2.6/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cli-0.2.6/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:41:01.206060 csle_cli-0.2.6/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:41:01.210060 csle_cli-0.2.6/src/csle_cli/
--rw-rw-r--   0 kim       (1000) kim       (1000)       38 2023-03-28 14:03:22.000000 csle_cli-0.2.6/src/csle_cli/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 07:39:12.000000 csle_cli-0.2.6/src/csle_cli/__version__.py
--rwxrwxr-x   0 kim       (1000) kim       (1000)   111257 2023-03-28 14:03:22.000000 csle_cli-0.2.6/src/csle_cli/cli.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:41:01.210060 csle_cli-0.2.6/src/csle_cli.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      629 2023-06-04 07:41:00.000000 csle_cli-0.2.6/src/csle_cli.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      369 2023-06-04 07:41:01.000000 csle_cli-0.2.6/src/csle_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 07:41:00.000000 csle_cli-0.2.6/src/csle_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       47 2023-06-04 07:41:01.000000 csle_cli-0.2.6/src/csle_cli.egg-info/entry_points.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:27.000000 csle_cli-0.2.6/src/csle_cli.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      291 2023-06-04 07:41:01.000000 csle_cli-0.2.6/src/csle_cli.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        9 2023-06-04 07:41:01.000000 csle_cli-0.2.6/src/csle_cli.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:34:08.459704 csle_cli-0.2.7/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      629 2023-06-04 08:34:08.459704 csle_cli-0.2.7/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)    22943 2023-03-28 14:03:22.000000 csle_cli-0.2.7/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      668 2023-03-28 14:03:22.000000 csle_cli-0.2.7/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1368 2023-06-04 08:34:08.459704 csle_cli-0.2.7/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cli-0.2.7/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:34:08.459704 csle_cli-0.2.7/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:34:08.459704 csle_cli-0.2.7/src/csle_cli/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       38 2023-03-28 14:03:22.000000 csle_cli-0.2.7/src/csle_cli/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 08:32:18.000000 csle_cli-0.2.7/src/csle_cli/__version__.py
+-rwxrwxr-x   0 kim       (1000) kim       (1000)   111257 2023-03-28 14:03:22.000000 csle_cli-0.2.7/src/csle_cli/cli.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:34:08.459704 csle_cli-0.2.7/src/csle_cli.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      629 2023-06-04 08:34:08.000000 csle_cli-0.2.7/src/csle_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      369 2023-06-04 08:34:08.000000 csle_cli-0.2.7/src/csle_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 08:34:08.000000 csle_cli-0.2.7/src/csle_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       47 2023-06-04 08:34:08.000000 csle_cli-0.2.7/src/csle_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:27.000000 csle_cli-0.2.7/src/csle_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      291 2023-06-04 08:34:08.000000 csle_cli-0.2.7/src/csle_cli.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        9 2023-06-04 08:34:08.000000 csle_cli-0.2.7/src/csle_cli.egg-info/top_level.txt
```

### Comparing `csle_cli-0.2.6/PKG-INFO` & `csle_cli-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cli
-Version: 0.2.6
+Version: 0.2.7
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cli-0.2.6/README.md` & `csle_cli-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `csle_cli-0.2.6/pyproject.toml` & `csle_cli-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cli-0.2.6/setup.cfg` & `csle_cli-0.2.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	click>=8.1.3
-	csle-common>=0.2.6
-	csle-cluster>=0.2.6
-	csle-collector>=0.2.6
-	csle-attacker>=0.2.6
-	csle-defender>=0.2.6
-	csle-system-identification>=0.2.6
-	gym-csle-stopping-game>=0.2.6
-	csle-agents>=0.2.6
+	csle-common>=0.2.7
+	csle-cluster>=0.2.7
+	csle-collector>=0.2.7
+	csle-attacker>=0.2.7
+	csle-defender>=0.2.7
+	csle-system-identification>=0.2.7
+	gym-csle-stopping-game>=0.2.7
+	csle-agents>=0.2.7
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cli-0.2.6/src/csle_cli/cli.py` & `csle_cli-0.2.7/src/csle_cli/cli.py`

 * *Files identical despite different names*

### Comparing `csle_cli-0.2.6/src/csle_cli.egg-info/PKG-INFO` & `csle_cli-0.2.7/src/csle_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cli
-Version: 0.2.6
+Version: 0.2.7
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

