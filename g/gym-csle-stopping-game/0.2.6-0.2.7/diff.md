# Comparing `tmp/gym_csle_stopping_game-0.2.6.tar.gz` & `tmp/gym_csle_stopping_game-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_stopping_game-0.2.6.tar", last modified: Sun Jun  4 07:40:12 2023, max compression
+gzip compressed data, was "gym_csle_stopping_game-0.2.7.tar", last modified: Sun Jun  4 08:33:20 2023, max compression
```

## Comparing `gym_csle_stopping_game-0.2.6.tar` & `gym_csle_stopping_game-0.2.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:40:12.009902 gym_csle_stopping_game-0.2.6/
--rw-rw-r--   0 kim       (1000) kim       (1000)      715 2023-06-04 07:40:12.009902 gym_csle_stopping_game-0.2.6/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      703 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.6/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1378 2023-06-04 07:40:12.009902 gym_csle_stopping_game-0.2.6/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.6/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:40:12.005902 gym_csle_stopping_game-0.2.6/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:40:12.009902 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/
--rw-rw-r--   0 kim       (1000) kim       (1000)      657 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 07:39:12.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:40:12.009902 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1030 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:40:12.009902 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3002 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4961 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/dao/stopping_game_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3249 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1375 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/dao/stopping_game_state.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:40:12.009902 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/envs/
--rw-rw-r--   0 kim       (1000) kim       (1000)       74 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/envs/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    24656 2023-04-30 06:59:23.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/envs/stopping_game_env.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     9022 2023-04-18 14:59:42.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7749 2023-04-30 06:59:23.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:40:12.009902 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    18598 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/util/stopping_game_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 07:40:12.009902 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      715 2023-06-04 07:40:11.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1130 2023-06-04 07:40:12.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 07:40:11.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:50:52.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      259 2023-06-04 07:40:11.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       23 2023-06-04 07:40:11.000000 gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:33:20.271369 gym_csle_stopping_game-0.2.7/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      715 2023-06-04 08:33:20.271369 gym_csle_stopping_game-0.2.7/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      703 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.7/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1378 2023-06-04 08:33:20.271369 gym_csle_stopping_game-0.2.7/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.7/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:33:20.267369 gym_csle_stopping_game-0.2.7/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:33:20.267369 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      657 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 08:32:18.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:33:20.267369 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1030 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:33:20.267369 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3002 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4961 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/dao/stopping_game_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3249 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1375 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/dao/stopping_game_state.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:33:20.271369 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/envs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       74 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/envs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    24656 2023-04-30 06:59:23.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/envs/stopping_game_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9022 2023-04-18 14:59:42.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7749 2023-04-30 06:59:23.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:33:20.271369 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18598 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/util/stopping_game_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:33:20.267369 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      715 2023-06-04 08:33:19.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1130 2023-06-04 08:33:20.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 08:33:19.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:50:52.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      259 2023-06-04 08:33:20.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       23 2023-06-04 08:33:20.000000 gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game.egg-info/top_level.txt
```

### Comparing `gym_csle_stopping_game-0.2.6/PKG-INFO` & `gym_csle_stopping_game-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym_csle_stopping_game
-Version: 0.2.6
+Version: 0.2.7
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.2.6/pyproject.toml` & `gym_csle_stopping_game-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.6/setup.cfg` & `gym_csle_stopping_game-0.2.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	gymnasium>=0.27.1
-	csle-common>=0.2.6
-	csle-attacker>=0.2.6
-	csle-defender>=0.2.6
-	csle-collector>=0.2.6
+	csle-common>=0.2.7
+	csle-attacker>=0.2.7
+	csle-defender>=0.2.7
+	csle-collector>=0.2.7
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/__init__.py` & `gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/constants/constants.py` & `gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/constants/constants.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py` & `gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/dao/stopping_game_config.py` & `gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/dao/stopping_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py` & `gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/dao/stopping_game_state.py` & `gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/dao/stopping_game_state.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/envs/stopping_game_env.py` & `gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/envs/stopping_game_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py` & `gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py` & `gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game/util/stopping_game_util.py` & `gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game/util/stopping_game_util.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game.egg-info/PKG-INFO` & `gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-csle-stopping-game
-Version: 0.2.6
+Version: 0.2.7
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.2.6/src/gym_csle_stopping_game.egg-info/SOURCES.txt` & `gym_csle_stopping_game-0.2.7/src/gym_csle_stopping_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

