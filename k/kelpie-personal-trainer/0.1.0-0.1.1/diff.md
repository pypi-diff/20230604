# Comparing `tmp/kelpie_personal_trainer-0.1.0.tar.gz` & `tmp/kelpie_personal_trainer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kelpie_personal_trainer-0.1.0.tar", last modified: Sun Jun  4 17:55:25 2023, max compression
+gzip compressed data, was "kelpie_personal_trainer-0.1.1.tar", last modified: Sun Jun  4 17:57:38 2023, max compression
```

## Comparing `kelpie_personal_trainer-0.1.0.tar` & `kelpie_personal_trainer-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 17:55:25.143390 kelpie_personal_trainer-0.1.0/
--rw-rw-rw-   0        0        0      506 2023-06-04 17:55:25.142397 kelpie_personal_trainer-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-04 17:55:25.103392 kelpie_personal_trainer-0.1.0/kelpie_personal_trainer/
--rw-rw-rw-   0        0        0       87 2023-06-04 17:52:34.000000 kelpie_personal_trainer-0.1.0/kelpie_personal_trainer/__init__.py
--rw-rw-rw-   0        0        0     2595 2023-06-04 17:54:32.000000 kelpie_personal_trainer-0.1.0/kelpie_personal_trainer/body_type.py
-drwxrwxrwx   0        0        0        0 2023-06-04 17:55:25.140389 kelpie_personal_trainer-0.1.0/kelpie_personal_trainer.egg-info/
--rw-rw-rw-   0        0        0      506 2023-06-04 17:55:25.000000 kelpie_personal_trainer-0.1.0/kelpie_personal_trainer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-06-04 17:55:25.000000 kelpie_personal_trainer-0.1.0/kelpie_personal_trainer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 17:55:25.000000 kelpie_personal_trainer-0.1.0/kelpie_personal_trainer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-04 17:55:25.000000 kelpie_personal_trainer-0.1.0/kelpie_personal_trainer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-04 17:55:25.000000 kelpie_personal_trainer-0.1.0/kelpie_personal_trainer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 17:55:25.144398 kelpie_personal_trainer-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-06-04 17:54:32.000000 kelpie_personal_trainer-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:57:38.484296 kelpie_personal_trainer-0.1.1/
+-rw-rw-rw-   0        0        0      506 2023-06-04 17:57:38.483284 kelpie_personal_trainer-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-04 17:57:38.468284 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer/
+-rw-rw-rw-   0        0        0        0 2023-06-04 17:57:15.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-06-04 17:54:32.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer/body_type.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:57:38.482285 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer.egg-info/
+-rw-rw-rw-   0        0        0      506 2023-06-04 17:57:38.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-06-04 17:57:38.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 17:57:38.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-04 17:57:38.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-04 17:57:38.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 17:57:38.485286 kelpie_personal_trainer-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      790 2023-06-04 17:57:20.000000 kelpie_personal_trainer-0.1.1/setup.py
```

### Comparing `kelpie_personal_trainer-0.1.0/kelpie_personal_trainer/body_type.py` & `kelpie_personal_trainer-0.1.1/kelpie_personal_trainer/body_type.py`

 * *Files identical despite different names*

### Comparing `kelpie_personal_trainer-0.1.0/setup.py` & `kelpie_personal_trainer-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Personal Trainer Library'
 
 # Setting up
 setup(
     name="kelpie_personal_trainer",
     version=VERSION,
     author="Ariel",
```

