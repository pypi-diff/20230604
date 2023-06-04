# Comparing `tmp/gym_csle_stopping_game-0.2.4.tar.gz` & `tmp/gym_csle_stopping_game-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_stopping_game-0.2.4.tar", last modified: Wed May 31 13:44:11 2023, max compression
+gzip compressed data, was "gym_csle_stopping_game-0.2.5.tar", last modified: Sun Jun  4 07:14:29 2023, max compression
```

## Comparing `gym_csle_stopping_game-0.2.4.tar` & `gym_csle_stopping_game-0.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:44:11.287710 gym_csle_stopping_game-0.2.4/
--rw-r--r--   0 kimham     (501) staff       (20)      715 2023-05-31 13:44:11.287896 gym_csle_stopping_game-0.2.4/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      703 2023-03-22 11:50:26.000000 gym_csle_stopping_game-0.2.4/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1378 2023-05-31 13:44:11.288690 gym_csle_stopping_game-0.2.4/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.2.4/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:44:11.274126 gym_csle_stopping_game-0.2.4/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:44:11.276201 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/
--rw-r--r--   0 kimham     (501) staff       (20)      657 2023-03-22 11:50:26.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 13:42:03.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:44:11.279858 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     1030 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:44:11.282912 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/dao/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/dao/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     3002 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     4961 2023-03-22 11:50:26.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/dao/stopping_game_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3249 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     1375 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/dao/stopping_game_state.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:44:11.285807 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/envs/
--rw-r--r--   0 kimham     (501) staff       (20)       74 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/envs/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    24656 2023-04-25 09:14:08.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/envs/stopping_game_env.py
--rw-r--r--   0 kimham     (501) staff       (20)     9022 2023-04-25 09:09:21.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
--rw-r--r--   0 kimham     (501) staff       (20)     7749 2023-04-25 09:08:36.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:44:11.286804 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/util/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/util/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    18598 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/util/stopping_game_util.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 13:44:11.279089 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      715 2023-05-31 13:44:10.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     1130 2023-05-31 13:44:11.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 13:44:10.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:04:06.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      259 2023-05-31 13:44:11.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       23 2023-05-31 13:44:11.000000 gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:29.341234 gym_csle_stopping_game-0.2.5/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      715 2023-06-04 07:14:29.341234 gym_csle_stopping_game-0.2.5/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      703 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.5/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1378 2023-06-04 07:14:29.341234 gym_csle_stopping_game-0.2.5/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.5/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:29.337234 gym_csle_stopping_game-0.2.5/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:29.337234 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      657 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 07:13:34.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:29.341234 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1030 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:29.341234 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3002 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4961 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/dao/stopping_game_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3249 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1375 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/dao/stopping_game_state.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:29.341234 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/envs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       74 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/envs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    24656 2023-04-30 06:59:23.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/envs/stopping_game_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9022 2023-04-18 14:59:42.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7749 2023-04-30 06:59:23.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:29.341234 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18598 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/util/stopping_game_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:14:29.341234 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      715 2023-06-04 07:14:28.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1130 2023-06-04 07:14:29.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 07:14:29.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:50:52.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      259 2023-06-04 07:14:29.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       23 2023-06-04 07:14:29.000000 gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game.egg-info/top_level.txt
```

### Comparing `gym_csle_stopping_game-0.2.4/PKG-INFO` & `gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gym_csle_stopping_game
-Version: 0.2.4
+Name: gym-csle-stopping-game
+Version: 0.2.5
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.2.4/pyproject.toml` & `gym_csle_stopping_game-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.4/setup.cfg` & `gym_csle_stopping_game-0.2.5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	gymnasium>=0.27.1
-	csle-common>=0.2.4
-	csle-attacker>=0.2.4
-	csle-defender>=0.2.4
-	csle-collector>=0.2.4
+	csle-common>=0.2.5
+	csle-attacker>=0.2.5
+	csle-defender>=0.2.5
+	csle-collector>=0.2.5
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/__init__.py` & `gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/constants/constants.py` & `gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/constants/constants.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py` & `gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/dao/stopping_game_config.py` & `gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/dao/stopping_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py` & `gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/dao/stopping_game_state.py` & `gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/dao/stopping_game_state.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/envs/stopping_game_env.py` & `gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/envs/stopping_game_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py` & `gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py` & `gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game/util/stopping_game_util.py` & `gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game/util/stopping_game_util.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game.egg-info/PKG-INFO` & `gym_csle_stopping_game-0.2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gym-csle-stopping-game
-Version: 0.2.4
+Name: gym_csle_stopping_game
+Version: 0.2.5
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.2.4/src/gym_csle_stopping_game.egg-info/SOURCES.txt` & `gym_csle_stopping_game-0.2.5/src/gym_csle_stopping_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

