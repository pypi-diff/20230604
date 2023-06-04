# Comparing `tmp/kelpie_personal_trainer-0.1.8.tar.gz` & `tmp/kelpie_personal_trainer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kelpie_personal_trainer-0.1.8.tar", last modified: Sun Jun  4 18:28:30 2023, max compression
+gzip compressed data, was "kelpie_personal_trainer-0.1.9.tar", last modified: Sun Jun  4 18:30:47 2023, max compression
```

## Comparing `kelpie_personal_trainer-0.1.8.tar` & `kelpie_personal_trainer-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 18:28:30.206831 kelpie_personal_trainer-0.1.8/
--rw-rw-rw-   0        0        0      506 2023-06-04 18:28:30.205829 kelpie_personal_trainer-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-04 18:28:30.186367 kelpie_personal_trainer-0.1.8/kelpie_personal_trainer/
--rw-rw-rw-   0        0        0        0 2023-06-04 17:57:15.000000 kelpie_personal_trainer-0.1.8/kelpie_personal_trainer/__init__.py
--rw-rw-rw-   0        0        0     2593 2023-06-04 18:11:08.000000 kelpie_personal_trainer-0.1.8/kelpie_personal_trainer/body_type.py
-drwxrwxrwx   0        0        0        0 2023-06-04 18:28:30.203829 kelpie_personal_trainer-0.1.8/kelpie_personal_trainer/models/
--rw-rw-rw-   0        0        0    14678 2023-06-04 17:42:30.000000 kelpie_personal_trainer-0.1.8/kelpie_personal_trainer/models/knnpickle_file.pickle
-drwxrwxrwx   0        0        0        0 2023-06-04 18:28:30.201874 kelpie_personal_trainer-0.1.8/kelpie_personal_trainer.egg-info/
--rw-rw-rw-   0        0        0      506 2023-06-04 18:28:30.000000 kelpie_personal_trainer-0.1.8/kelpie_personal_trainer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2023-06-04 18:28:30.000000 kelpie_personal_trainer-0.1.8/kelpie_personal_trainer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 18:28:30.000000 kelpie_personal_trainer-0.1.8/kelpie_personal_trainer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-04 18:28:30.000000 kelpie_personal_trainer-0.1.8/kelpie_personal_trainer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-04 18:28:30.000000 kelpie_personal_trainer-0.1.8/kelpie_personal_trainer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 18:28:30.206831 kelpie_personal_trainer-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      889 2023-06-04 18:28:07.000000 kelpie_personal_trainer-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:30:47.049971 kelpie_personal_trainer-0.1.9/
+-rw-rw-rw-   0        0        0      506 2023-06-04 18:30:47.048971 kelpie_personal_trainer-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-04 18:30:47.029969 kelpie_personal_trainer-0.1.9/kelpie_personal_trainer/
+-rw-rw-rw-   0        0        0        0 2023-06-04 17:57:15.000000 kelpie_personal_trainer-0.1.9/kelpie_personal_trainer/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-06-04 18:29:53.000000 kelpie_personal_trainer-0.1.9/kelpie_personal_trainer/body_type.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:30:47.045969 kelpie_personal_trainer-0.1.9/kelpie_personal_trainer/models/
+-rw-rw-rw-   0        0        0    14678 2023-06-04 17:42:30.000000 kelpie_personal_trainer-0.1.9/kelpie_personal_trainer/models/knnpickle_file.pickle
+drwxrwxrwx   0        0        0        0 2023-06-04 18:30:47.043968 kelpie_personal_trainer-0.1.9/kelpie_personal_trainer.egg-info/
+-rw-rw-rw-   0        0        0      506 2023-06-04 18:30:46.000000 kelpie_personal_trainer-0.1.9/kelpie_personal_trainer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2023-06-04 18:30:47.000000 kelpie_personal_trainer-0.1.9/kelpie_personal_trainer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 18:30:46.000000 kelpie_personal_trainer-0.1.9/kelpie_personal_trainer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-04 18:30:46.000000 kelpie_personal_trainer-0.1.9/kelpie_personal_trainer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-04 18:30:46.000000 kelpie_personal_trainer-0.1.9/kelpie_personal_trainer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 18:30:47.049971 kelpie_personal_trainer-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      889 2023-06-04 18:30:29.000000 kelpie_personal_trainer-0.1.9/setup.py
```

### Comparing `kelpie_personal_trainer-0.1.8/kelpie_personal_trainer/body_type.py` & `kelpie_personal_trainer-0.1.9/kelpie_personal_trainer/body_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pickle
 import cv2
 import mediapipe as mp
 import numpy as np
 import pandas as pd
 
 
-filename = "models/knnpickle_file.pickle"
+filename = "./models/knnpickle_file.pickle"
 model = pickle.load(open(filename, 'rb'))
 
 
 def get_index(name):
     landmark_names = [
         'nose',
         'left_eye_inner', 'left_eye', 'left_eye_outer',
```

### Comparing `kelpie_personal_trainer-0.1.8/kelpie_personal_trainer/models/knnpickle_file.pickle` & `kelpie_personal_trainer-0.1.9/kelpie_personal_trainer/models/knnpickle_file.pickle`

 * *Files identical despite different names*

### Comparing `kelpie_personal_trainer-0.1.8/setup.py` & `kelpie_personal_trainer-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 DESCRIPTION = 'Personal Trainer Library'
 
 # Setting up
 setup(
     name="kelpie_personal_trainer",
     version=VERSION,
     author="Ariel",
```

