# Comparing `tmp/kelpie_personal_trainer-0.0.3.tar.gz` & `tmp/kelpie_personal_trainer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kelpie_personal_trainer-0.0.3.tar", last modified: Sun Jun  4 17:01:17 2023, max compression
+gzip compressed data, was "kelpie_personal_trainer-0.0.4.tar", last modified: Sun Jun  4 17:08:06 2023, max compression
```

## Comparing `kelpie_personal_trainer-0.0.3.tar` & `kelpie_personal_trainer-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 17:01:17.949490 kelpie_personal_trainer-0.0.3/
--rw-rw-rw-   0        0        0      577 2023-06-04 17:01:17.947488 kelpie_personal_trainer-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-04 17:01:17.925489 kelpie_personal_trainer-0.0.3/kelpie_personal_trainer/
--rw-rw-rw-   0        0        0       16 2023-06-04 17:01:09.000000 kelpie_personal_trainer-0.0.3/kelpie_personal_trainer/__init__.py
--rw-rw-rw-   0        0        0       50 2023-06-04 16:59:47.000000 kelpie_personal_trainer-0.0.3/kelpie_personal_trainer/body_type.py
--rw-rw-rw-   0        0        0       47 2023-06-04 16:56:34.000000 kelpie_personal_trainer-0.0.3/kelpie_personal_trainer/main.py
-drwxrwxrwx   0        0        0        0 2023-06-04 17:01:17.945532 kelpie_personal_trainer-0.0.3/kelpie_personal_trainer.egg-info/
--rw-rw-rw-   0        0        0      577 2023-06-04 17:01:17.000000 kelpie_personal_trainer-0.0.3/kelpie_personal_trainer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-06-04 17:01:17.000000 kelpie_personal_trainer-0.0.3/kelpie_personal_trainer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 17:01:17.000000 kelpie_personal_trainer-0.0.3/kelpie_personal_trainer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 17:01:17.000000 kelpie_personal_trainer-0.0.3/kelpie_personal_trainer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-04 17:01:17.000000 kelpie_personal_trainer-0.0.3/kelpie_personal_trainer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 17:01:17.949490 kelpie_personal_trainer-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      747 2023-06-04 17:01:13.000000 kelpie_personal_trainer-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:08:06.468182 kelpie_personal_trainer-0.0.4/
+-rw-rw-rw-   0        0        0      577 2023-06-04 17:08:06.467183 kelpie_personal_trainer-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-04 17:08:06.439184 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer/
+-rw-rw-rw-   0        0        0       34 2023-06-04 17:07:44.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-06-04 16:59:47.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer/body_type.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:08:06.465169 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/
+-rw-rw-rw-   0        0        0      577 2023-06-04 17:08:06.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-06-04 17:08:06.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 17:08:06.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-04 17:08:06.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-04 17:08:06.000000 kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 17:08:06.468182 kelpie_personal_trainer-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-06-04 17:08:02.000000 kelpie_personal_trainer-0.0.4/setup.py
```

### Comparing `kelpie_personal_trainer-0.0.3/PKG-INFO` & `kelpie_personal_trainer-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kelpie_personal_trainer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Basic hello world package
 Home-page: UNKNOWN
 Author: Ariel
 Author-email: <arillesmana2001@gmail.com>
 License: UNKNOWN
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `kelpie_personal_trainer-0.0.3/kelpie_personal_trainer.egg-info/PKG-INFO` & `kelpie_personal_trainer-0.0.4/kelpie_personal_trainer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kelpie-personal-trainer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Basic hello world package
 Home-page: UNKNOWN
 Author: Ariel
 Author-email: <arillesmana2001@gmail.com>
 License: UNKNOWN
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `kelpie_personal_trainer-0.0.3/setup.py` & `kelpie_personal_trainer-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Basic hello world package'
 
 # Setting up
 setup(
     name="kelpie_personal_trainer",
     version=VERSION,
     author="Ariel",
@@ -18,8 +18,8 @@
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```

