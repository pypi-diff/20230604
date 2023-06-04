# Comparing `tmp/kelpie_personal_trainer-0.1.2.tar.gz` & `tmp/kelpie_personal_trainer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kelpie_personal_trainer-0.1.2.tar", last modified: Sun Jun  4 18:01:12 2023, max compression
+gzip compressed data, was "kelpie_personal_trainer-0.1.3.tar", last modified: Sun Jun  4 18:07:04 2023, max compression
```

## Comparing `kelpie_personal_trainer-0.1.2.tar` & `kelpie_personal_trainer-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 18:01:12.074967 kelpie_personal_trainer-0.1.2/
--rw-rw-rw-   0        0        0      506 2023-06-04 18:01:12.073951 kelpie_personal_trainer-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-04 18:01:12.054953 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer/
--rw-rw-rw-   0        0        0        0 2023-06-04 17:57:15.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer/__init__.py
--rw-rw-rw-   0        0        0     2595 2023-06-04 17:54:32.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer/body_type.py
-drwxrwxrwx   0        0        0        0 2023-06-04 18:01:12.072952 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer.egg-info/
--rw-rw-rw-   0        0        0      506 2023-06-04 18:01:12.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-06-04 18:01:12.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 18:01:12.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-04 18:01:12.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-04 18:01:12.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 18:01:12.075954 kelpie_personal_trainer-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      780 2023-06-04 18:00:48.000000 kelpie_personal_trainer-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:07:04.725126 kelpie_personal_trainer-0.1.3/
+-rw-rw-rw-   0        0        0      506 2023-06-04 18:07:04.724122 kelpie_personal_trainer-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-04 18:07:04.685112 kelpie_personal_trainer-0.1.3/kelpie_personal_trainer/
+-rw-rw-rw-   0        0        0        0 2023-06-04 17:57:15.000000 kelpie_personal_trainer-0.1.3/kelpie_personal_trainer/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-06-04 18:06:34.000000 kelpie_personal_trainer-0.1.3/kelpie_personal_trainer/body_type.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:07:04.705112 kelpie_personal_trainer-0.1.3/kelpie_personal_trainer.egg-info/
+-rw-rw-rw-   0        0        0      506 2023-06-04 18:07:04.000000 kelpie_personal_trainer-0.1.3/kelpie_personal_trainer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-06-04 18:07:04.000000 kelpie_personal_trainer-0.1.3/kelpie_personal_trainer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 18:07:04.000000 kelpie_personal_trainer-0.1.3/kelpie_personal_trainer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-04 18:07:04.000000 kelpie_personal_trainer-0.1.3/kelpie_personal_trainer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-04 18:07:04.000000 kelpie_personal_trainer-0.1.3/kelpie_personal_trainer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 18:07:04.725126 kelpie_personal_trainer-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      780 2023-06-04 18:06:34.000000 kelpie_personal_trainer-0.1.3/setup.py
```

### Comparing `kelpie_personal_trainer-0.1.2/kelpie_personal_trainer/body_type.py` & `kelpie_personal_trainer-0.1.3/kelpie_personal_trainer/body_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pickle
 import cv2
 import mediapipe as mp
 import numpy as np
 import pandas as pd
 
 
-filename = "./models/knnpickle_file.pickle"
+filename = "knnpickle_file.pickle"
 model = pickle.load(open(filename, 'rb'))
 
 
 def get_index(name):
     landmark_names = [
         'nose',
         'left_eye_inner', 'left_eye', 'left_eye_outer',
```

### Comparing `kelpie_personal_trainer-0.1.2/setup.py` & `kelpie_personal_trainer-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'Personal Trainer Library'
 
 # Setting up
 setup(
     name="kelpie_personal_trainer",
     version=VERSION,
     author="Ariel",
```

