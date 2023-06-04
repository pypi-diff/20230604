# Comparing `tmp/kelpie_personal_trainer-0.1.1.tar.gz` & `tmp/kelpie_personal_trainer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kelpie_personal_trainer-0.1.1.tar", last modified: Sun Jun  4 17:57:38 2023, max compression
+gzip compressed data, was "kelpie_personal_trainer-0.1.2.tar", last modified: Sun Jun  4 18:01:12 2023, max compression
```

## Comparing `kelpie_personal_trainer-0.1.1.tar` & `kelpie_personal_trainer-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 17:57:38.484296 kelpie_personal_trainer-0.1.1/
--rw-rw-rw-   0        0        0      506 2023-06-04 17:57:38.483284 kelpie_personal_trainer-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-04 17:57:38.468284 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer/
--rw-rw-rw-   0        0        0        0 2023-06-04 17:57:15.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer/__init__.py
--rw-rw-rw-   0        0        0     2595 2023-06-04 17:54:32.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer/body_type.py
-drwxrwxrwx   0        0        0        0 2023-06-04 17:57:38.482285 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer.egg-info/
--rw-rw-rw-   0        0        0      506 2023-06-04 17:57:38.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-06-04 17:57:38.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 17:57:38.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-04 17:57:38.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-04 17:57:38.000000 kelpie_personal_trainer-0.1.1/kelpie_personal_trainer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 17:57:38.485286 kelpie_personal_trainer-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-06-04 17:57:20.000000 kelpie_personal_trainer-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:01:12.074967 kelpie_personal_trainer-0.1.2/
+-rw-rw-rw-   0        0        0      506 2023-06-04 18:01:12.073951 kelpie_personal_trainer-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-04 18:01:12.054953 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer/
+-rw-rw-rw-   0        0        0        0 2023-06-04 17:57:15.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-06-04 17:54:32.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer/body_type.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:01:12.072952 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer.egg-info/
+-rw-rw-rw-   0        0        0      506 2023-06-04 18:01:12.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-06-04 18:01:12.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 18:01:12.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-04 18:01:12.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-04 18:01:12.000000 kelpie_personal_trainer-0.1.2/kelpie_personal_trainer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 18:01:12.075954 kelpie_personal_trainer-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      780 2023-06-04 18:00:48.000000 kelpie_personal_trainer-0.1.2/setup.py
```

### Comparing `kelpie_personal_trainer-0.1.1/kelpie_personal_trainer/body_type.py` & `kelpie_personal_trainer-0.1.2/kelpie_personal_trainer/body_type.py`

 * *Files identical despite different names*

### Comparing `kelpie_personal_trainer-0.1.1/setup.py` & `kelpie_personal_trainer-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Personal Trainer Library'
 
 # Setting up
 setup(
     name="kelpie_personal_trainer",
     version=VERSION,
     author="Ariel",
     author_email="<arillesmana2001@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=['pandas', 'opencv-python', 'pickle', 'mediapipe', 'numpy'],
+    install_requires=['pandas', 'opencv-python', 'mediapipe', 'numpy'],
     keywords=['python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

