# Comparing `tmp/csle_attacker-0.2.4.tar.gz` & `tmp/csle_attacker-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_attacker-0.2.4.tar", last modified: Wed May 31 13:43:05 2023, max compression
+gzip compressed data, was "csle_attacker-0.2.5.tar", last modified: Sun Jun  4 07:14:02 2023, max compression
```

## Comparing `csle_attacker-0.2.4.tar` & `csle_attacker-0.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:05.944818 csle_attacker-0.2.4/
--rw-r--r--   0 kimham     (501) staff       (20)      659 2023-05-31 13:43:05.944937 csle_attacker-0.2.4/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     3922 2023-01-11 18:45:47.000000 csle_attacker-0.2.4/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      673 2023-02-12 08:59:32.000000 csle_attacker-0.2.4/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1218 2023-05-31 13:43:05.945491 csle_attacker-0.2.4/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:05.933069 csle_attacker-0.2.4/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:05.936040 csle_attacker-0.2.4/src/csle_attacker/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 13:42:03.000000 csle_attacker-0.2.4/src/csle_attacker/__version__.py
--rw-r--r--   0 kimham     (501) staff       (20)      941 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/attacker.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:05.940961 csle_attacker-0.2.4/src/csle_attacker/emulation/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      994 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/attacker_stopping_middleware.py
--rw-r--r--   0 kimham     (501) staff       (20)    11411 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/emulated_attacker.py
--rw-r--r--   0 kimham     (501) staff       (20)    11560 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/exploit_middleware.py
--rw-r--r--   0 kimham     (501) staff       (20)     4676 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/post_exploit_middleware.py
--rw-r--r--   0 kimham     (501) staff       (20)     5951 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/recon_middleware.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:05.943987 csle_attacker-0.2.4/src/csle_attacker/emulation/util/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/util/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    45611 2023-04-19 06:25:48.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/util/exploit_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     7585 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/util/nikto_util.py
--rw-r--r--   0 kimham     (501) staff       (20)    34189 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/util/nmap_util.py
--rw-r--r--   0 kimham     (501) staff       (20)    29810 2022-11-28 13:00:49.000000 csle_attacker-0.2.4/src/csle_attacker/emulation/util/shell_util.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:43:05.938195 csle_attacker-0.2.4/src/csle_attacker.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      659 2023-05-31 13:43:05.000000 csle_attacker-0.2.4/src/csle_attacker.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      916 2023-05-31 13:43:05.000000 csle_attacker-0.2.4/src/csle_attacker.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 13:43:05.000000 csle_attacker-0.2.4/src/csle_attacker.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:33.000000 csle_attacker-0.2.4/src/csle_attacker.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      177 2023-05-31 13:43:05.000000 csle_attacker-0.2.4/src/csle_attacker.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       14 2023-05-31 13:43:05.000000 csle_attacker-0.2.4/src/csle_attacker.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:02.673316 csle_attacker-0.2.5/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      659 2023-06-04 07:14:02.673316 csle_attacker-0.2.5/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3922 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      673 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1218 2023-06-04 07:14:02.673316 csle_attacker-0.2.5/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:02.669316 csle_attacker-0.2.5/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:02.669316 csle_attacker-0.2.5/src/csle_attacker/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/src/csle_attacker/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 07:13:34.000000 csle_attacker-0.2.5/src/csle_attacker/__version__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      941 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/src/csle_attacker/attacker.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:02.669316 csle_attacker-0.2.5/src/csle_attacker/emulation/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/src/csle_attacker/emulation/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      994 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/src/csle_attacker/emulation/attacker_stopping_middleware.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11411 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/src/csle_attacker/emulation/emulated_attacker.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11560 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/src/csle_attacker/emulation/exploit_middleware.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4676 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/src/csle_attacker/emulation/post_exploit_middleware.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5951 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/src/csle_attacker/emulation/recon_middleware.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:02.673316 csle_attacker-0.2.5/src/csle_attacker/emulation/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/src/csle_attacker/emulation/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    45611 2023-04-18 12:47:39.000000 csle_attacker-0.2.5/src/csle_attacker/emulation/util/exploit_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7585 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/src/csle_attacker/emulation/util/nikto_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    34189 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/src/csle_attacker/emulation/util/nmap_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    29810 2023-03-28 14:03:22.000000 csle_attacker-0.2.5/src/csle_attacker/emulation/util/shell_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:02.669316 csle_attacker-0.2.5/src/csle_attacker.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      659 2023-06-04 07:14:02.000000 csle_attacker-0.2.5/src/csle_attacker.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      916 2023-06-04 07:14:02.000000 csle_attacker-0.2.5/src/csle_attacker.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 07:14:02.000000 csle_attacker-0.2.5/src/csle_attacker.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:55.000000 csle_attacker-0.2.5/src/csle_attacker.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      177 2023-06-04 07:14:02.000000 csle_attacker-0.2.5/src/csle_attacker.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       14 2023-06-04 07:14:02.000000 csle_attacker-0.2.5/src/csle_attacker.egg-info/top_level.txt
```

### Comparing `csle_attacker-0.2.4/PKG-INFO` & `csle_attacker-0.2.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_attacker
-Version: 0.2.4
+Version: 0.2.5
 Summary: Scripts for emulated cyber attacks in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attacker-0.2.4/README.md` & `csle_attacker-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.4/pyproject.toml` & `csle_attacker-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.4/setup.cfg` & `csle_attacker-0.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.2.4
+	csle-common>=0.2.5
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_attacker-0.2.4/src/csle_attacker/attacker.py` & `csle_attacker-0.2.5/src/csle_attacker/attacker.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.4/src/csle_attacker/emulation/attacker_stopping_middleware.py` & `csle_attacker-0.2.5/src/csle_attacker/emulation/attacker_stopping_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.4/src/csle_attacker/emulation/emulated_attacker.py` & `csle_attacker-0.2.5/src/csle_attacker/emulation/emulated_attacker.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.4/src/csle_attacker/emulation/exploit_middleware.py` & `csle_attacker-0.2.5/src/csle_attacker/emulation/exploit_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.4/src/csle_attacker/emulation/post_exploit_middleware.py` & `csle_attacker-0.2.5/src/csle_attacker/emulation/post_exploit_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.4/src/csle_attacker/emulation/recon_middleware.py` & `csle_attacker-0.2.5/src/csle_attacker/emulation/recon_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.4/src/csle_attacker/emulation/util/exploit_util.py` & `csle_attacker-0.2.5/src/csle_attacker/emulation/util/exploit_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.4/src/csle_attacker/emulation/util/nikto_util.py` & `csle_attacker-0.2.5/src/csle_attacker/emulation/util/nikto_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.4/src/csle_attacker/emulation/util/nmap_util.py` & `csle_attacker-0.2.5/src/csle_attacker/emulation/util/nmap_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.4/src/csle_attacker/emulation/util/shell_util.py` & `csle_attacker-0.2.5/src/csle_attacker/emulation/util/shell_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.2.4/src/csle_attacker.egg-info/PKG-INFO` & `csle_attacker-0.2.5/src/csle_attacker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-attacker
-Version: 0.2.4
+Version: 0.2.5
 Summary: Scripts for emulated cyber attacks in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attacker-0.2.4/src/csle_attacker.egg-info/SOURCES.txt` & `csle_attacker-0.2.5/src/csle_attacker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

