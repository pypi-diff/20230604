# Comparing `tmp/CoderSchoolAI-0.0.2.tar.gz` & `tmp/CoderSchoolAI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoderSchoolAI-0.0.2.tar", last modified: Sun Jun  4 13:48:35 2023, max compression
+gzip compressed data, was "CoderSchoolAI-0.0.3.tar", last modified: Sun Jun  4 14:01:26 2023, max compression
```

## Comparing `CoderSchoolAI-0.0.2.tar` & `CoderSchoolAI-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.817320 CoderSchoolAI-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.742370 CoderSchoolAI-0.0.2/CoderSchoolAI/
-drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.726319 CoderSchoolAI-0.0.2/CoderSchoolAI/Assets/
-drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.767320 CoderSchoolAI-0.0.2/CoderSchoolAI/Assets/CoderSchoolAI/
--rw-rw-rw-   0        0        0   143548 2023-05-26 14:42:41.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Assets/CoderSchoolAI/CoderSchoolAI-Logo.png
-drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.771319 CoderSchoolAI-0.0.2/CoderSchoolAI/Assets/Snake/
--rw-rw-rw-   0        0        0    42206 2023-06-04 13:26:34.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Assets/Snake/Apple.png
-drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.779319 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/
--rw-rw-rw-   0        0        0     4420 2023-05-24 16:35:17.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/Agent.py
--rw-rw-rw-   0        0        0     3057 2023-05-18 18:22:36.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/Attributes.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.788346 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/CoderSchoolEnvironments/
--rw-rw-rw-   0        0        0    19236 2023-06-04 13:45:33.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/CoderSchoolEnvironments/SnakeEnvironment.py
--rw-rw-rw-   0        0        0        0 2023-05-12 04:23:34.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/CoderSchoolEnvironments/__init__.py
--rw-rw-rw-   0        0        0     6696 2023-05-27 19:21:43.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/Shell.py
--rw-rw-rw-   0        0        0        0 2023-05-12 04:04:30.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.797318 CoderSchoolAI-0.0.2/CoderSchoolAI/Neural/
--rw-rw-rw-   0        0        0     1661 2023-05-23 05:50:30.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Neural/Block.py
--rw-rw-rw-   0        0        0        0 2023-05-18 17:47:49.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Neural/Net.py
--rw-rw-rw-   0        0        0        0 2023-05-12 04:04:30.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Neural/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.803321 CoderSchoolAI-0.0.2/CoderSchoolAI/Training/
--rw-rw-rw-   0        0        0     6527 2023-05-26 16:55:20.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Training/Algorithms.py
--rw-rw-rw-   0        0        0        0 2023-05-12 04:04:30.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Training/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.809320 CoderSchoolAI-0.0.2/CoderSchoolAI/Util/
--rw-rw-rw-   0        0        0        0 2023-05-12 04:04:54.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Util/__init__.py
--rw-rw-rw-   0        0        0     1010 2023-05-12 05:33:20.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Util/data_utils.py
--rw-rw-rw-   0        0        0      524 2023-05-12 03:04:18.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/Util/misc_utils.py
--rw-rw-rw-   0        0        0     1781 2023-06-04 13:02:10.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.813325 CoderSchoolAI-0.0.2/CoderSchoolAI/cli/
--rw-rw-rw-   0        0        0        0 2023-06-04 13:42:40.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/cli/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-06-04 13:24:08.000000 CoderSchoolAI-0.0.2/CoderSchoolAI/cli/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:48:35.765320 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/
--rw-rw-rw-   0        0        0      397 2023-06-04 13:48:35.000000 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      970 2023-06-04 13:48:35.000000 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 13:48:35.000000 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-04 13:48:35.000000 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2023-06-04 13:48:35.000000 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 13:48:35.000000 CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      183 2023-05-26 14:30:52.000000 CoderSchoolAI-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      397 2023-06-04 13:48:35.815317 CoderSchoolAI-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-10 01:13:09.000000 CoderSchoolAI-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-04 13:48:35.817320 CoderSchoolAI-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      724 2023-06-04 13:47:50.000000 CoderSchoolAI-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:01:26.414596 CoderSchoolAI-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-04 14:01:26.348600 CoderSchoolAI-0.0.3/CoderSchoolAI/
+drwxrwxrwx   0        0        0        0 2023-06-04 14:01:26.335597 CoderSchoolAI-0.0.3/CoderSchoolAI/Assets/
+drwxrwxrwx   0        0        0        0 2023-06-04 14:01:26.375597 CoderSchoolAI-0.0.3/CoderSchoolAI/Assets/CoderSchoolAI/
+-rw-rw-rw-   0        0        0   143548 2023-05-26 14:42:41.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Assets/CoderSchoolAI/CoderSchoolAI-Logo.png
+drwxrwxrwx   0        0        0        0 2023-06-04 14:01:26.377598 CoderSchoolAI-0.0.3/CoderSchoolAI/Assets/Snake/
+-rw-rw-rw-   0        0        0    42206 2023-06-04 13:26:34.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Assets/Snake/Apple.png
+drwxrwxrwx   0        0        0        0 2023-06-04 14:01:26.386598 CoderSchoolAI-0.0.3/CoderSchoolAI/Environment/
+-rw-rw-rw-   0        0        0     4420 2023-05-24 16:35:17.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Environment/Agent.py
+-rw-rw-rw-   0        0        0     3057 2023-05-18 18:22:36.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Environment/Attributes.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:01:26.391598 CoderSchoolAI-0.0.3/CoderSchoolAI/Environment/CoderSchoolEnvironments/
+-rw-rw-rw-   0        0        0    19236 2023-06-04 13:45:33.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Environment/CoderSchoolEnvironments/SnakeEnvironment.py
+-rw-rw-rw-   0        0        0        0 2023-05-12 04:23:34.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Environment/CoderSchoolEnvironments/__init__.py
+-rw-rw-rw-   0        0        0     6696 2023-05-27 19:21:43.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Environment/Shell.py
+-rw-rw-rw-   0        0        0        0 2023-05-12 04:04:30.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Environment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:01:26.397599 CoderSchoolAI-0.0.3/CoderSchoolAI/Neural/
+-rw-rw-rw-   0        0        0     1661 2023-05-23 05:50:30.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Neural/Block.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 17:47:49.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Neural/Net.py
+-rw-rw-rw-   0        0        0        0 2023-05-12 04:04:30.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Neural/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:01:26.401597 CoderSchoolAI-0.0.3/CoderSchoolAI/Training/
+-rw-rw-rw-   0        0        0     6527 2023-05-26 16:55:20.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Training/Algorithms.py
+-rw-rw-rw-   0        0        0        0 2023-05-12 04:04:30.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Training/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:01:26.407598 CoderSchoolAI-0.0.3/CoderSchoolAI/Util/
+-rw-rw-rw-   0        0        0        0 2023-05-12 04:04:54.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Util/__init__.py
+-rw-rw-rw-   0        0        0     1010 2023-05-12 05:33:20.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Util/data_utils.py
+-rw-rw-rw-   0        0        0      524 2023-05-12 03:04:18.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/Util/misc_utils.py
+-rw-rw-rw-   0        0        0     1781 2023-06-04 13:02:10.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:01:26.411596 CoderSchoolAI-0.0.3/CoderSchoolAI/cli/
+-rw-rw-rw-   0        0        0        0 2023-06-04 13:42:40.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/cli/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-06-04 13:24:08.000000 CoderSchoolAI-0.0.3/CoderSchoolAI/cli/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:01:26.373595 CoderSchoolAI-0.0.3/CoderSchoolAI.egg-info/
+-rw-rw-rw-   0        0        0      413 2023-06-04 14:01:26.000000 CoderSchoolAI-0.0.3/CoderSchoolAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      970 2023-06-04 14:01:26.000000 CoderSchoolAI-0.0.3/CoderSchoolAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 14:01:26.000000 CoderSchoolAI-0.0.3/CoderSchoolAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-04 14:01:26.000000 CoderSchoolAI-0.0.3/CoderSchoolAI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2023-06-04 14:01:26.000000 CoderSchoolAI-0.0.3/CoderSchoolAI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-04 14:01:26.000000 CoderSchoolAI-0.0.3/CoderSchoolAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      183 2023-05-26 14:30:52.000000 CoderSchoolAI-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      413 2023-06-04 14:01:26.413597 CoderSchoolAI-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-10 01:13:09.000000 CoderSchoolAI-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-04 14:01:26.414596 CoderSchoolAI-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-06-04 14:01:20.000000 CoderSchoolAI-0.0.3/setup.py
```

### Comparing `CoderSchoolAI-0.0.2/CoderSchoolAI/Assets/CoderSchoolAI/CoderSchoolAI-Logo.png` & `CoderSchoolAI-0.0.3/CoderSchoolAI/Assets/CoderSchoolAI/CoderSchoolAI-Logo.png`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.2/CoderSchoolAI/Assets/Snake/Apple.png` & `CoderSchoolAI-0.0.3/CoderSchoolAI/Assets/Snake/Apple.png`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/Agent.py` & `CoderSchoolAI-0.0.3/CoderSchoolAI/Environment/Agent.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/Attributes.py` & `CoderSchoolAI-0.0.3/CoderSchoolAI/Environment/Attributes.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/CoderSchoolEnvironments/SnakeEnvironment.py` & `CoderSchoolAI-0.0.3/CoderSchoolAI/Environment/CoderSchoolEnvironments/SnakeEnvironment.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.2/CoderSchoolAI/Environment/Shell.py` & `CoderSchoolAI-0.0.3/CoderSchoolAI/Environment/Shell.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.2/CoderSchoolAI/Neural/Block.py` & `CoderSchoolAI-0.0.3/CoderSchoolAI/Neural/Block.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.2/CoderSchoolAI/Training/Algorithms.py` & `CoderSchoolAI-0.0.3/CoderSchoolAI/Training/Algorithms.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.2/CoderSchoolAI/Util/data_utils.py` & `CoderSchoolAI-0.0.3/CoderSchoolAI/Util/data_utils.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.2/CoderSchoolAI/Util/misc_utils.py` & `CoderSchoolAI-0.0.3/CoderSchoolAI/Util/misc_utils.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.2/CoderSchoolAI/__init__.py` & `CoderSchoolAI-0.0.3/CoderSchoolAI/__init__.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.2/CoderSchoolAI/cli/cli.py` & `CoderSchoolAI-0.0.3/CoderSchoolAI/cli/cli.py`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.2/CoderSchoolAI.egg-info/SOURCES.txt` & `CoderSchoolAI-0.0.3/CoderSchoolAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CoderSchoolAI-0.0.2/setup.py` & `CoderSchoolAI-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CoderSchoolAI',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     include_package_data=True,
     description='A Comprehensive Python Library for Creating and Developing Agent AIs.',
     entry_points={
         'console_scripts': [
             'coderschoolai = CoderSchoolAI.cli.cli:main'
         ]
@@ -14,10 +14,10 @@
     author='Jonathan Koch, ',
     author_email='johnnykoch002@example.com, ',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
     ],
-    keywords='sample setuptools development',
-    install_requires=['numpy', 'gym'],
+    keywords='ai agents pygame torch setuptools development',
+    install_requires=['numpy', 'gymnasium', 'pygame',],
 )
```

