# Comparing `tmp/gamer3514-0.0.2.tar.gz` & `tmp/gamer3514-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamer3514-0.0.2.tar", last modified: Sat Jun  3 18:27:16 2023, max compression
+gzip compressed data, was "gamer3514-0.0.3.tar", last modified: Sun Jun  4 11:23:19 2023, max compression
```

## Comparing `gamer3514-0.0.2.tar` & `gamer3514-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 18:27:16.828929 gamer3514-0.0.2/
--rw-rw-rw-   0        0        0     1087 2023-06-03 17:19:31.000000 gamer3514-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1065 2023-06-03 18:27:16.827820 gamer3514-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-06-03 18:26:37.000000 gamer3514-0.0.2/README.md
--rw-rw-rw-   0        0        0      616 2023-06-03 18:19:26.000000 gamer3514-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-03 18:27:16.828929 gamer3514-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-03 18:27:16.796743 gamer3514-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 18:27:16.806916 gamer3514-0.0.2/src/gamer3514/
--rw-rw-rw-   0        0        0        0 2023-06-03 17:12:43.000000 gamer3514-0.0.2/src/gamer3514/__init__.py
--rw-rw-rw-   0        0        0     2949 2023-06-03 18:24:55.000000 gamer3514-0.0.2/src/gamer3514/api.py
-drwxrwxrwx   0        0        0        0 2023-06-03 18:27:16.825901 gamer3514-0.0.2/src/gamer3514.egg-info/
--rw-rw-rw-   0        0        0     1065 2023-06-03 18:27:16.000000 gamer3514-0.0.2/src/gamer3514.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-03 18:27:16.000000 gamer3514-0.0.2/src/gamer3514.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 18:27:16.000000 gamer3514-0.0.2/src/gamer3514.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-03 18:27:16.000000 gamer3514-0.0.2/src/gamer3514.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 11:23:19.181504 gamer3514-0.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-06-03 17:19:31.000000 gamer3514-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1361 2023-06-04 11:23:19.179997 gamer3514-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      832 2023-06-04 11:21:26.000000 gamer3514-0.0.3/README.md
+-rw-rw-rw-   0        0        0      616 2023-06-04 11:23:06.000000 gamer3514-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 11:23:19.181504 gamer3514-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 11:23:19.145431 gamer3514-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 11:23:19.156341 gamer3514-0.0.3/src/gamer3514/
+-rw-rw-rw-   0        0        0        0 2023-06-03 17:12:43.000000 gamer3514-0.0.3/src/gamer3514/__init__.py
+-rw-rw-rw-   0        0        0     5291 2023-06-04 11:21:58.000000 gamer3514-0.0.3/src/gamer3514/api.py
+-rw-rw-rw-   0        0        0      138 2023-06-04 11:20:12.000000 gamer3514-0.0.3/src/gamer3514/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:23:19.178959 gamer3514-0.0.3/src/gamer3514.egg-info/
+-rw-rw-rw-   0        0        0     1361 2023-06-04 11:23:19.000000 gamer3514-0.0.3/src/gamer3514.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-06-04 11:23:19.000000 gamer3514-0.0.3/src/gamer3514.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 11:23:19.000000 gamer3514-0.0.3/src/gamer3514.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 11:23:19.000000 gamer3514-0.0.3/src/gamer3514.egg-info/top_level.txt
```

### Comparing `gamer3514-0.0.2/LICENSE` & `gamer3514-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gamer3514-0.0.2/PKG-INFO` & `gamer3514-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamer3514
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small package that does stuff
 Author-email: Gamer3514 <gamer@sillydev.co.uk>
 Project-URL: Homepage, https://github.com/thegamer3514/gamer3514
 Project-URL: Bug Tracker, https://github.com/thegamer3514/gamer3514/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,26 +20,42 @@
 
 ```bash
 pip install gamer3514
 ```
 
 ## Usage
 
+### Api
 ```python
 from gamer3514 import api
 #NSFW Detection
 api.detectnsfw(imageurl, apikey)
 #Profanity Check
 api.profanitycheck(text, apikey)
 #Text To Braille
 api.texttobraille(text)
 #Random Number
 api.randomnumber(length)
 #Random Topic
 api.randomtopic()
+#Random Cat Image
+api.cat(filepath, apikey)
+#Random Cat Gif
+api.catgif(filepath, apikey)
+#Random Dog Image
+api.dog(filepath, apikey)
+#Donald Tweet
+api.donaldtweet(filepath, text)
+```
+
+### Utils
+```python
+from gamer3514 import utils
+#Get Random Number
+utils.randomnumber()
 ```
 
 ## Resources
 
 - [Discord server](https://discord.gg/3qvpkgWSbF)
 - [Free hosting](https://panel.sillydev.co.uk)
 - Contact me: gamer@sillydev.co.uk
```

### Comparing `gamer3514-0.0.2/src/gamer3514.egg-info/PKG-INFO` & `gamer3514-0.0.3/src/gamer3514.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamer3514
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small package that does stuff
 Author-email: Gamer3514 <gamer@sillydev.co.uk>
 Project-URL: Homepage, https://github.com/thegamer3514/gamer3514
 Project-URL: Bug Tracker, https://github.com/thegamer3514/gamer3514/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,26 +20,42 @@
 
 ```bash
 pip install gamer3514
 ```
 
 ## Usage
 
+### Api
 ```python
 from gamer3514 import api
 #NSFW Detection
 api.detectnsfw(imageurl, apikey)
 #Profanity Check
 api.profanitycheck(text, apikey)
 #Text To Braille
 api.texttobraille(text)
 #Random Number
 api.randomnumber(length)
 #Random Topic
 api.randomtopic()
+#Random Cat Image
+api.cat(filepath, apikey)
+#Random Cat Gif
+api.catgif(filepath, apikey)
+#Random Dog Image
+api.dog(filepath, apikey)
+#Donald Tweet
+api.donaldtweet(filepath, text)
+```
+
+### Utils
+```python
+from gamer3514 import utils
+#Get Random Number
+utils.randomnumber()
 ```
 
 ## Resources
 
 - [Discord server](https://discord.gg/3qvpkgWSbF)
 - [Free hosting](https://panel.sillydev.co.uk)
 - Contact me: gamer@sillydev.co.uk
```

