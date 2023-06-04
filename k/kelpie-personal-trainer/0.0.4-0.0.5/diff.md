# Comparing `tmp/kelpie_personal_trainer-0.0.4.tar.gz` & `tmp/kelpie_personal_trainer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kelpie_personal_trainer-0.0.4.tar", last modified: Sun Jun  4 17:08:06 2023, max compression
+gzip compressed data, was "kelpie_personal_trainer-0.0.5.tar", last modified: Sun Jun  4 17:14:43 2023, max compression
```

## Comparing `kelpie_personal_trainer-0.0.4.tar` & `kelpie_personal_trainer-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 17:08:06.468182 kelpie_personal_trainer-0.0.4/
--rw-rw-rw-   0        0        0      577 2023-06-04 17:08:06.467183 kelpie_personal_trainer-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-04 17:08:06.439184 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer/
--rw-rw-rw-   0        0        0       34 2023-06-04 17:07:44.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer/__init__.py
--rw-rw-rw-   0        0        0       50 2023-06-04 16:59:47.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer/body_type.py
-drwxrwxrwx   0        0        0        0 2023-06-04 17:08:06.465169 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/
--rw-rw-rw-   0        0        0      577 2023-06-04 17:08:06.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-06-04 17:08:06.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 17:08:06.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 17:08:06.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-04 17:08:06.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 17:08:06.468182 kelpie_personal_trainer-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      749 2023-06-04 17:08:02.000000 kelpie_personal_trainer-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:14:43.783252 kelpie_personal_trainer-0.0.5/
+-rw-rw-rw-   0        0        0      577 2023-06-04 17:14:43.782249 kelpie_personal_trainer-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-04 17:14:43.744251 kelpie_personal_trainer-0.0.5/kelpie_personal_trainer/
+-rw-rw-rw-   0        0        0       18 2023-06-04 17:14:36.000000 kelpie_personal_trainer-0.0.5/kelpie_personal_trainer/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-06-04 16:59:47.000000 kelpie_personal_trainer-0.0.5/kelpie_personal_trainer/body_type.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:14:43.779249 kelpie_personal_trainer-0.0.5/kelpie_personal_trainer.egg-info/
+-rw-rw-rw-   0        0        0      577 2023-06-04 17:14:43.000000 kelpie_personal_trainer-0.0.5/kelpie_personal_trainer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-06-04 17:14:43.000000 kelpie_personal_trainer-0.0.5/kelpie_personal_trainer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 17:14:43.000000 kelpie_personal_trainer-0.0.5/kelpie_personal_trainer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-04 17:14:43.000000 kelpie_personal_trainer-0.0.5/kelpie_personal_trainer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-04 17:14:43.000000 kelpie_personal_trainer-0.0.5/kelpie_personal_trainer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 17:14:43.783252 kelpie_personal_trainer-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-06-04 17:14:40.000000 kelpie_personal_trainer-0.0.5/setup.py
```

### Comparing `kelpie_personal_trainer-0.0.4/PKG-INFO` & `kelpie_personal_trainer-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kelpie_personal_trainer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Basic hello world package
 Home-page: UNKNOWN
 Author: Ariel
 Author-email: <arillesmana2001@gmail.com>
 License: UNKNOWN
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/PKG-INFO` & `kelpie_personal_trainer-0.0.5/kelpie_personal_trainer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kelpie-personal-trainer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Basic hello world package
 Home-page: UNKNOWN
 Author: Ariel
 Author-email: <arillesmana2001@gmail.com>
 License: UNKNOWN
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `kelpie_personal_trainer-0.0.4/setup.py` & `kelpie_personal_trainer-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Basic hello world package'
 
 # Setting up
 setup(
     name="kelpie_personal_trainer",
     version=VERSION,
     author="Ariel",
```

