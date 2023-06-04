# Comparing `tmp/csle_cli-0.2.4.tar.gz` & `tmp/csle_cli-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cli-0.2.4.tar", last modified: Wed May 31 13:45:55 2023, max compression
+gzip compressed data, was "csle_cli-0.2.5.tar", last modified: Sun Jun  4 07:15:13 2023, max compression
```

## Comparing `csle_cli-0.2.4.tar` & `csle_cli-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:55.372233 csle_cli-0.2.4/
--rw-r--r--   0 kimham     (501) staff       (20)      629 2023-05-31 13:45:55.372347 csle_cli-0.2.4/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)    22943 2023-02-12 17:03:02.000000 csle_cli-0.2.4/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      668 2023-02-12 08:59:32.000000 csle_cli-0.2.4/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1368 2023-05-31 13:45:55.373164 csle_cli-0.2.4/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_cli-0.2.4/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:55.364084 csle_cli-0.2.4/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:55.367759 csle_cli-0.2.4/src/csle_cli/
--rw-r--r--   0 kimham     (501) staff       (20)       38 2022-11-28 13:00:49.000000 csle_cli-0.2.4/src/csle_cli/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 13:42:03.000000 csle_cli-0.2.4/src/csle_cli/__version__.py
--rwxr-xr-x   0 kimham     (501) staff       (20)   111257 2023-03-22 11:50:26.000000 csle_cli-0.2.4/src/csle_cli/cli.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:45:55.372031 csle_cli-0.2.4/src/csle_cli.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      629 2023-05-31 13:45:54.000000 csle_cli-0.2.4/src/csle_cli.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      369 2023-05-31 13:45:55.000000 csle_cli-0.2.4/src/csle_cli.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 13:45:54.000000 csle_cli-0.2.4/src/csle_cli.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)       47 2023-05-31 13:45:55.000000 csle_cli-0.2.4/src/csle_cli.egg-info/entry_points.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:04:54.000000 csle_cli-0.2.4/src/csle_cli.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      291 2023-05-31 13:45:55.000000 csle_cli-0.2.4/src/csle_cli.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)        9 2023-05-31 13:45:55.000000 csle_cli-0.2.4/src/csle_cli.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:15:13.853093 csle_cli-0.2.5/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      629 2023-06-04 07:15:13.853093 csle_cli-0.2.5/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)    22943 2023-03-28 14:03:22.000000 csle_cli-0.2.5/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      668 2023-03-28 14:03:22.000000 csle_cli-0.2.5/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1368 2023-06-04 07:15:13.853093 csle_cli-0.2.5/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cli-0.2.5/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:15:13.849094 csle_cli-0.2.5/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:15:13.849094 csle_cli-0.2.5/src/csle_cli/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       38 2023-03-28 14:03:22.000000 csle_cli-0.2.5/src/csle_cli/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 07:13:34.000000 csle_cli-0.2.5/src/csle_cli/__version__.py
+-rwxrwxr-x   0 kim       (1000) kim       (1000)   111257 2023-03-28 14:03:22.000000 csle_cli-0.2.5/src/csle_cli/cli.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:15:13.853093 csle_cli-0.2.5/src/csle_cli.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      629 2023-06-04 07:15:13.000000 csle_cli-0.2.5/src/csle_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      369 2023-06-04 07:15:13.000000 csle_cli-0.2.5/src/csle_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 07:15:13.000000 csle_cli-0.2.5/src/csle_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       47 2023-06-04 07:15:13.000000 csle_cli-0.2.5/src/csle_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:27.000000 csle_cli-0.2.5/src/csle_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      291 2023-06-04 07:15:13.000000 csle_cli-0.2.5/src/csle_cli.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        9 2023-06-04 07:15:13.000000 csle_cli-0.2.5/src/csle_cli.egg-info/top_level.txt
```

### Comparing `csle_cli-0.2.4/PKG-INFO` & `csle_cli-0.2.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cli
-Version: 0.2.4
+Version: 0.2.5
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cli-0.2.4/README.md` & `csle_cli-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `csle_cli-0.2.4/pyproject.toml` & `csle_cli-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cli-0.2.4/setup.cfg` & `csle_cli-0.2.5/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	click>=8.1.3
-	csle-common>=0.2.4
-	csle-cluster>=0.2.4
-	csle-collector>=0.2.4
-	csle-attacker>=0.2.4
-	csle-defender>=0.2.4
-	csle-system-identification>=0.2.4
-	gym-csle-stopping-game>=0.2.4
-	csle-agents>=0.2.4
+	csle-common>=0.2.5
+	csle-cluster>=0.2.5
+	csle-collector>=0.2.5
+	csle-attacker>=0.2.5
+	csle-defender>=0.2.5
+	csle-system-identification>=0.2.5
+	gym-csle-stopping-game>=0.2.5
+	csle-agents>=0.2.5
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cli-0.2.4/src/csle_cli/cli.py` & `csle_cli-0.2.5/src/csle_cli/cli.py`

 * *Files identical despite different names*

### Comparing `csle_cli-0.2.4/src/csle_cli.egg-info/PKG-INFO` & `csle_cli-0.2.5/src/csle_cli.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cli
-Version: 0.2.4
+Version: 0.2.5
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

