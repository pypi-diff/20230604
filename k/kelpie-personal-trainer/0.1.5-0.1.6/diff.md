# Comparing `tmp/kelpie_personal_trainer-0.1.5.tar.gz` & `tmp/kelpie_personal_trainer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kelpie_personal_trainer-0.1.5.tar", last modified: Sun Jun  4 18:22:16 2023, max compression
+gzip compressed data, was "kelpie_personal_trainer-0.1.6.tar", last modified: Sun Jun  4 18:24:04 2023, max compression
```

## Comparing `kelpie_personal_trainer-0.1.5.tar` & `kelpie_personal_trainer-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 18:22:16.774937 kelpie_personal_trainer-0.1.5/
--rw-rw-rw-   0        0        0      506 2023-06-04 18:22:16.772938 kelpie_personal_trainer-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-04 18:22:16.730938 kelpie_personal_trainer-0.1.5/kelpie_personal_trainer/
--rw-rw-rw-   0        0        0        0 2023-06-04 17:57:15.000000 kelpie_personal_trainer-0.1.5/kelpie_personal_trainer/__init__.py
--rw-rw-rw-   0        0        0     2593 2023-06-04 18:11:08.000000 kelpie_personal_trainer-0.1.5/kelpie_personal_trainer/body_type.py
-drwxrwxrwx   0        0        0        0 2023-06-04 18:22:16.769938 kelpie_personal_trainer-0.1.5/kelpie_personal_trainer.egg-info/
--rw-rw-rw-   0        0        0      506 2023-06-04 18:22:16.000000 kelpie_personal_trainer-0.1.5/kelpie_personal_trainer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-06-04 18:22:16.000000 kelpie_personal_trainer-0.1.5/kelpie_personal_trainer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 18:22:16.000000 kelpie_personal_trainer-0.1.5/kelpie_personal_trainer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-04 18:22:16.000000 kelpie_personal_trainer-0.1.5/kelpie_personal_trainer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-04 18:22:16.000000 kelpie_personal_trainer-0.1.5/kelpie_personal_trainer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 18:22:16.775938 kelpie_personal_trainer-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-06-04 18:21:54.000000 kelpie_personal_trainer-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:24:04.858340 kelpie_personal_trainer-0.1.6/
+-rw-rw-rw-   0        0        0      506 2023-06-04 18:24:04.857340 kelpie_personal_trainer-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-04 18:24:04.839342 kelpie_personal_trainer-0.1.6/kelpie_personal_trainer/
+-rw-rw-rw-   0        0        0        0 2023-06-04 17:57:15.000000 kelpie_personal_trainer-0.1.6/kelpie_personal_trainer/__init__.py
+-rw-rw-rw-   0        0        0     2593 2023-06-04 18:11:08.000000 kelpie_personal_trainer-0.1.6/kelpie_personal_trainer/body_type.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:24:04.855341 kelpie_personal_trainer-0.1.6/kelpie_personal_trainer.egg-info/
+-rw-rw-rw-   0        0        0      506 2023-06-04 18:24:04.000000 kelpie_personal_trainer-0.1.6/kelpie_personal_trainer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-06-04 18:24:04.000000 kelpie_personal_trainer-0.1.6/kelpie_personal_trainer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 18:24:04.000000 kelpie_personal_trainer-0.1.6/kelpie_personal_trainer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-04 18:24:04.000000 kelpie_personal_trainer-0.1.6/kelpie_personal_trainer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-04 18:24:04.000000 kelpie_personal_trainer-0.1.6/kelpie_personal_trainer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 18:24:04.858340 kelpie_personal_trainer-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      881 2023-06-04 18:23:42.000000 kelpie_personal_trainer-0.1.6/setup.py
```

### Comparing `kelpie_personal_trainer-0.1.5/kelpie_personal_trainer/body_type.py` & `kelpie_personal_trainer-0.1.6/kelpie_personal_trainer/body_type.py`

 * *Files identical despite different names*

### Comparing `kelpie_personal_trainer-0.1.5/setup.py` & `kelpie_personal_trainer-0.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'Personal Trainer Library'
 
 # Setting up
 setup(
     name="kelpie_personal_trainer",
     version=VERSION,
     author="Ariel",
     author_email="<arillesmana2001@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
-    packages=find_packages(include=['kelpie_personal_trainer', 'models']),
+    packages=find_packages(include=['kelpie_personal_trainer', 'kelpie_personal_trainer.models']),
     include_package_data=True,
     install_requires=['pandas', 'opencv-python', 'mediapipe', 'numpy'],
     keywords=['python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

