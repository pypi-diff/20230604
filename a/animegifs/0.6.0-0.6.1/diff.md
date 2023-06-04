# Comparing `tmp/animegifs-0.6.0.tar.gz` & `tmp/animegifs-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.6.0.tar", last modified: Thu Jun  1 17:23:04 2023, max compression
+gzip compressed data, was "animegifs-0.6.1.tar", last modified: Sun Jun  4 19:12:57 2023, max compression
```

## Comparing `animegifs-0.6.0.tar` & `animegifs-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 17:23:04.551180 animegifs-0.6.0/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     1968 2023-06-01 17:23:04.550180 animegifs-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1338 2023-06-01 16:28:39.000000 animegifs-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 17:23:04.532178 animegifs-0.6.0/animegifs/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.6.0/animegifs/__init__.py
--rw-rw-rw-   0        0        0     3316 2023-06-01 16:13:07.000000 animegifs-0.6.0/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2023-06-01 17:23:04.548180 animegifs-0.6.0/animegifs/distutils/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.6.0/animegifs/distutils/__init__.py
--rw-rw-rw-   0        0        0     1586 2023-06-01 16:01:08.000000 animegifs-0.6.0/animegifs/distutils/errors.py
--rw-rw-rw-   0        0        0     1418 2023-06-01 16:28:39.000000 animegifs-0.6.0/animegifs/distutils/gifs.py
-drwxrwxrwx   0        0        0        0 2023-06-01 17:23:04.540181 animegifs-0.6.0/animegifs.egg-info/
--rw-rw-rw-   0        0        0     1968 2023-06-01 17:23:04.000000 animegifs-0.6.0/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-06-01 17:23:04.000000 animegifs-0.6.0/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 17:23:04.000000 animegifs-0.6.0/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-01 17:23:04.000000 animegifs-0.6.0/animegifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-01 17:23:04.000000 animegifs-0.6.0/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 17:23:04.551180 animegifs-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-06-01 16:46:00.000000 animegifs-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:12:57.537700 animegifs-0.6.1/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0     2050 2023-06-04 19:12:57.537700 animegifs-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1412 2023-06-04 19:10:24.000000 animegifs-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 19:12:57.518699 animegifs-0.6.1/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.6.1/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-06-04 19:10:24.000000 animegifs-0.6.1/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:12:57.535701 animegifs-0.6.1/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.6.1/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0     1586 2023-06-01 16:01:08.000000 animegifs-0.6.1/animegifs/distutils/errors.py
+-rw-rw-rw-   0        0        0     1568 2023-06-04 19:10:24.000000 animegifs-0.6.1/animegifs/distutils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:12:57.526701 animegifs-0.6.1/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     2050 2023-06-04 19:12:57.000000 animegifs-0.6.1/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-06-04 19:12:57.000000 animegifs-0.6.1/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 19:12:57.000000 animegifs-0.6.1/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-04 19:12:57.000000 animegifs-0.6.1/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 19:12:57.000000 animegifs-0.6.1/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 19:12:57.538699 animegifs-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-06-04 19:10:24.000000 animegifs-0.6.1/setup.py
```

### Comparing `animegifs-0.6.0/LICENSE` & `animegifs-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.6.0/PKG-INFO` & `animegifs-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.6.0
+Version: 0.6.1
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
 Platform: UNKNOWN
@@ -53,14 +53,15 @@
 * Blush
 * Bonk
 * Brofist
 * Cry
 * Cuddle
 * Dance
 * Disgust
+* Exploding
 * Facedesk
 * Facepalm
 * Flick
 * Flirt
 * Handhold
 * Happy
 * Harass
@@ -69,14 +70,15 @@
 * Icecream
 * Insult
 * Kill
 * Kiss
 * Lick
 * Love
 * Marry
+* Nod
 * Nosebleed
 * Nuzzle
 * Pat
 * Peck
 * Poke
 * Popcorn
 * Pout
@@ -89,14 +91,20 @@
 * Shrug
 * Sip
 * Slap
 * Smirk
 * Sorry
 * Spank
 * Stare
+* Tease
+* Threat
+* Tickle
+* Tired
+* Wave
+* Yawn
 
 **Special Category List**
 
 * Random
 * Steal-magic
 
 WIP.
```

### Comparing `animegifs-0.6.0/README.md` & `animegifs-0.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 * Blush
 * Bonk
 * Brofist
 * Cry
 * Cuddle
 * Dance
 * Disgust
+* Exploding
 * Facedesk
 * Facepalm
 * Flick
 * Flirt
 * Handhold
 * Happy
 * Harass
@@ -51,14 +52,15 @@
 * Icecream
 * Insult
 * Kill
 * Kiss
 * Lick
 * Love
 * Marry
+* Nod
 * Nosebleed
 * Nuzzle
 * Pat
 * Peck
 * Poke
 * Popcorn
 * Pout
@@ -71,14 +73,20 @@
 * Shrug
 * Sip
 * Slap
 * Smirk
 * Sorry
 * Spank
 * Stare
+* Tease
+* Threat
+* Tickle
+* Tired
+* Wave
+* Yawn
 
 **Special Category List**
 
 * Random
 * Steal-magic
 
 WIP.
```

### Comparing `animegifs-0.6.0/animegifs/animegifs.py` & `animegifs-0.6.1/animegifs/animegifs.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
     def get_gif(self, category: str) -> str:
         """
         Insert a valid category and get a gif.
 
         Args:
             category (str): Valid categories: attack, bite, bloodsuck, blush, bonk,
-                brofist, cry, cuddle, dance, disgust, facedesk, facepalm, flick, flirt,
+                brofist, cry, cuddle, dance, disgust, exploding, facedesk, facepalm, flick, flirt,
                 handhold, happy, harass, highfive, hug, icecream, insult, kill, kiss,
-                lick, love, marry, nosebleed, nuzzle, pat, peck, poke, popcorn, pout,
+                lick, love, marry, nod, nosebleed, nuzzle, pat, peck, poke, popcorn, pout,
                 punch, punish, random, run, sad, scared, shoot, shrug, sip, slap, smirk,
-                sorry, spank, stare.
+                sorry, spank, stare, tease, threat, tickle, tired, wave, yawn.
 
         Returns:
             gif: gif (url) -> str
         """
         if type(category) is int:
             raise errors.CategoryIntegral(category)
         elif category.lower() in gifs.gifs_name_list:
```

### Comparing `animegifs-0.6.0/animegifs/distutils/errors.py` & `animegifs-0.6.1/animegifs/distutils/errors.py`

 * *Files identical despite different names*

### Comparing `animegifs-0.6.0/animegifs/distutils/gifs.py` & `animegifs-0.6.1/animegifs/distutils/gifs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,28 @@
 
 global TOKEN
 TOKEN = None
 gifs_name_list = ["attack",
                   "bite", 'bloodsuck', 'blush', 'bonk', 'brofist',
                   'cry', 'cuddle',
                   'dance', 'disgust',
+                  'exploding',
                   'facedesk', 'facepalm', 'flick', 'flirt',
                   'handhold', 'happy', 'harass', 'highfive', 'hug',
                   'icecream', 'insult',
                   'kill', 'kiss',
                   'lick', 'love',
                   'marry',
-                  'nosebleed', 'nuzzle',
+                  'nod', 'nosebleed', 'nuzzle',
                   'pat', 'peck', 'poke', 'popcorn', 'pout', 'punch', 'punish',
                   'random', 'run',
-                  'sad', 'scared', 'shoot', 'shrug', 'sip', 'slap', 'smirk', 'sorry', 'spank', 'stare']
+                  'sad', 'scared', 'shoot', 'shrug', 'sip', 'slap', 'smirk', 'sorry', 'spank', 'stare',
+                  'tease', 'threat', 'tickle', 'tired',
+                  'wave',
+                  'yawn']
 
 def authentication():
     response = requests.post("https://enkidu-app-5a3qq2fqya-uc.a.run.app/key1")
     auth_key = response.json()['key']
     return auth_key
 
 def access():
```

### Comparing `animegifs-0.6.0/animegifs.egg-info/PKG-INFO` & `animegifs-0.6.1/animegifs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.6.0
+Version: 0.6.1
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
 Platform: UNKNOWN
@@ -53,14 +53,15 @@
 * Blush
 * Bonk
 * Brofist
 * Cry
 * Cuddle
 * Dance
 * Disgust
+* Exploding
 * Facedesk
 * Facepalm
 * Flick
 * Flirt
 * Handhold
 * Happy
 * Harass
@@ -69,14 +70,15 @@
 * Icecream
 * Insult
 * Kill
 * Kiss
 * Lick
 * Love
 * Marry
+* Nod
 * Nosebleed
 * Nuzzle
 * Pat
 * Peck
 * Poke
 * Popcorn
 * Pout
@@ -89,14 +91,20 @@
 * Shrug
 * Sip
 * Slap
 * Smirk
 * Sorry
 * Spank
 * Stare
+* Tease
+* Threat
+* Tickle
+* Tired
+* Wave
+* Yawn
 
 **Special Category List**
 
 * Random
 * Steal-magic
 
 WIP.
```

### Comparing `animegifs-0.6.0/setup.py` & `animegifs-0.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.6.0'
+VERSION = '0.6.1'
 
 setup(
     name='animegifs',
     package_dir={"anime_gifs": "animegifs"},
     packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
```

