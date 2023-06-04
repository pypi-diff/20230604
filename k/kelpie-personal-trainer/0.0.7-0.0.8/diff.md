# Comparing `tmp/kelpie_personal_trainer-0.0.7.tar.gz` & `tmp/kelpie_personal_trainer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kelpie_personal_trainer-0.0.7.tar", last modified: Sun Jun  4 17:28:46 2023, max compression
+gzip compressed data, was "kelpie_personal_trainer-0.0.8.tar", last modified: Sun Jun  4 17:36:34 2023, max compression
```

## Comparing `kelpie_personal_trainer-0.0.7.tar` & `kelpie_personal_trainer-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 17:28:46.480925 kelpie_personal_trainer-0.0.7/
--rw-rw-rw-   0        0        0      507 2023-06-04 17:28:46.480925 kelpie_personal_trainer-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-04 17:28:46.447917 kelpie_personal_trainer-0.0.7/kelpie_personal_trainer/
--rw-rw-rw-   0        0        0       34 2023-06-04 17:28:06.000000 kelpie_personal_trainer-0.0.7/kelpie_personal_trainer/__init__.py
--rw-rw-rw-   0        0        0       50 2023-06-04 16:59:47.000000 kelpie_personal_trainer-0.0.7/kelpie_personal_trainer/body_type.py
-drwxrwxrwx   0        0        0        0 2023-06-04 17:28:46.478926 kelpie_personal_trainer-0.0.7/kelpie_personal_trainer.egg-info/
--rw-rw-rw-   0        0        0      507 2023-06-04 17:28:46.000000 kelpie_personal_trainer-0.0.7/kelpie_personal_trainer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-06-04 17:28:46.000000 kelpie_personal_trainer-0.0.7/kelpie_personal_trainer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 17:28:46.000000 kelpie_personal_trainer-0.0.7/kelpie_personal_trainer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 17:28:46.000000 kelpie_personal_trainer-0.0.7/kelpie_personal_trainer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-04 17:28:46.000000 kelpie_personal_trainer-0.0.7/kelpie_personal_trainer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 17:28:46.481927 kelpie_personal_trainer-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      749 2023-06-04 17:28:21.000000 kelpie_personal_trainer-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:36:34.246095 kelpie_personal_trainer-0.0.8/
+-rw-rw-rw-   0        0        0      507 2023-06-04 17:36:34.244089 kelpie_personal_trainer-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-04 17:36:34.216100 kelpie_personal_trainer-0.0.8/kelpie_personal_trainer/
+-rw-rw-rw-   0        0        0        0 2023-06-04 17:36:07.000000 kelpie_personal_trainer-0.0.8/kelpie_personal_trainer/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-06-04 16:59:47.000000 kelpie_personal_trainer-0.0.8/kelpie_personal_trainer/body_type.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:36:34.242133 kelpie_personal_trainer-0.0.8/kelpie_personal_trainer.egg-info/
+-rw-rw-rw-   0        0        0      507 2023-06-04 17:36:34.000000 kelpie_personal_trainer-0.0.8/kelpie_personal_trainer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-06-04 17:36:34.000000 kelpie_personal_trainer-0.0.8/kelpie_personal_trainer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 17:36:34.000000 kelpie_personal_trainer-0.0.8/kelpie_personal_trainer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-04 17:36:34.000000 kelpie_personal_trainer-0.0.8/kelpie_personal_trainer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-04 17:36:34.000000 kelpie_personal_trainer-0.0.8/kelpie_personal_trainer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 17:36:34.246095 kelpie_personal_trainer-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-06-04 17:36:07.000000 kelpie_personal_trainer-0.0.8/setup.py
```

### Comparing `kelpie_personal_trainer-0.0.7/setup.py` & `kelpie_personal_trainer-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Basic hello world package'
 
 # Setting up
 setup(
     name="kelpie_personal_trainer",
     version=VERSION,
     author="Ariel",
```

