# Comparing `tmp/django_jsheet-0.2.1.tar.gz` & `tmp/django_jsheet-0.2.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_jsheet-0.2.1.tar", last modified: Sun Jun  4 14:14:41 2023, max compression
+gzip compressed data, was "django_jsheet-0.2.1.1a0.tar", last modified: Sun Jun  4 14:44:48 2023, max compression
```

## Comparing `django_jsheet-0.2.1.tar` & `django_jsheet-0.2.1.1a0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:14:41.245387 django_jsheet-0.2.1/
--rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/LICENSE
--rw-r--r--   0 shadmod    (501) admin       (80)     1408 2023-06-04 14:14:41.245041 django_jsheet-0.2.1/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      334 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/README.md
--rw-r--r--   0 shadmod    (501) admin       (80)     1116 2023-06-04 14:07:25.000000 django_jsheet-0.2.1/pyproject.toml
--rw-r--r--   0 shadmod    (501) admin       (80)       38 2023-06-04 14:14:41.245564 django_jsheet-0.2.1/setup.cfg
--rw-r--r--   0 shadmod    (501) admin       (80)      871 2023-06-04 14:08:17.000000 django_jsheet-0.2.1/setup.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:14:41.237861 django_jsheet-0.2.1/src/
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:14:41.240732 django_jsheet-0.2.1/src/core/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/src/core/__init__.py
--rw-r--r--   0 shadmod    (501) admin       (80)    10692 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/src/core/django_sheet.py
--rw-r--r--   0 shadmod    (501) admin       (80)    10675 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/src/core/views.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:14:41.243516 django_jsheet-0.2.1/src/django_jsheet.egg-info/
--rw-r--r--   0 shadmod    (501) admin       (80)     1408 2023-06-04 14:14:41.000000 django_jsheet-0.2.1/src/django_jsheet.egg-info/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      325 2023-06-04 14:14:41.000000 django_jsheet-0.2.1/src/django_jsheet.egg-info/SOURCES.txt
--rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-04 14:14:41.000000 django_jsheet-0.2.1/src/django_jsheet.egg-info/dependency_links.txt
--rw-r--r--   0 shadmod    (501) admin       (80)       18 2023-06-04 14:14:41.000000 django_jsheet-0.2.1/src/django_jsheet.egg-info/top_level.txt
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:14:41.244191 django_jsheet-0.2.1/src/templatetags/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/src/templatetags/__init__.py
--rw-r--r--   0 shadmod    (501) admin       (80)     4553 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/src/templatetags/jsheet.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:44:48.322491 django_jsheet-0.2.1.1a0/
+-rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/LICENSE
+-rw-r--r--   0 shadmod    (501) admin       (80)      912 2023-06-04 14:44:48.322130 django_jsheet-0.2.1.1a0/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      334 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/README.md
+-rw-r--r--   0 shadmod    (501) admin       (80)       38 2023-06-04 14:44:48.322584 django_jsheet-0.2.1.1a0/setup.cfg
+-rw-r--r--   0 shadmod    (501) admin       (80)      973 2023-06-04 14:42:34.000000 django_jsheet-0.2.1.1a0/setup.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:44:48.316660 django_jsheet-0.2.1.1a0/src/
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:44:48.318966 django_jsheet-0.2.1.1a0/src/core/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/src/core/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)    10692 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/src/core/django_sheet.py
+-rw-r--r--   0 shadmod    (501) admin       (80)    10675 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/src/core/views.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:44:48.320806 django_jsheet-0.2.1.1a0/src/django_jsheet.egg-info/
+-rw-r--r--   0 shadmod    (501) admin       (80)      912 2023-06-04 14:44:48.000000 django_jsheet-0.2.1.1a0/src/django_jsheet.egg-info/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      310 2023-06-04 14:44:48.000000 django_jsheet-0.2.1.1a0/src/django_jsheet.egg-info/SOURCES.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-04 14:44:48.000000 django_jsheet-0.2.1.1a0/src/django_jsheet.egg-info/dependency_links.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       32 2023-06-04 14:44:48.000000 django_jsheet-0.2.1.1a0/src/django_jsheet.egg-info/top_level.txt
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:44:48.321622 django_jsheet-0.2.1.1a0/src/templatetags/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/src/templatetags/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)     4553 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/src/templatetags/jsheet.py
```

### Comparing `django_jsheet-0.2.1/LICENSE` & `django_jsheet-0.2.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.1/PKG-INFO` & `django_jsheet-0.2.1.1a0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 Metadata-Version: 2.1
 Name: django_jsheet
-Version: 0.2.1
+Version: 0.2.1.1a0
 Summary: A little tool to render a simple excel sheet in webpage
 Home-page: https://github.com/shadMod/django-jsheet
 Author: shadMod
-Author-email: shadMod <support@shadmod.it>
-Maintainer-email: ShadMod <support@shadmod.it>
-License: MIT License
-Project-URL: Homepage, https://github.com/shadMod/django-jsheet
+Author-email: support@shadmod.it
 Project-URL: Bug Tracker, https://github.com/shadMod/django-jsheet/issues
-Keywords: Django JSheet,Django-JSheet,Django_JSheet
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django JSheet
 
 Django JSheet is a little tool to render a simple excel sheet in webpage
```

### Comparing `django_jsheet-0.2.1/setup.py` & `django_jsheet-0.2.1.1a0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django_jsheet",
-    version="0.2.1",
+    version="0.2.1.1a",
     author="shadMod",
     author_email="support@shadmod.it",
     description="A little tool to render a simple excel sheet in webpage",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shadMod/django-jsheet",
     project_urls={
@@ -17,11 +17,15 @@
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    py_modules=["django_jsheet"],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
+    package_data={
+        "assets": ["assets/index.js"],
+    },
     python_requires=">=3.7"
 )
```

### Comparing `django_jsheet-0.2.1/src/core/django_sheet.py` & `django_jsheet-0.2.1.1a0/src/core/django_sheet.py`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.1/src/core/views.py` & `django_jsheet-0.2.1.1a0/src/core/views.py`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.1/src/django_jsheet.egg-info/PKG-INFO` & `django_jsheet-0.2.1.1a0/src/django_jsheet.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 Metadata-Version: 2.1
 Name: django-jsheet
-Version: 0.2.1
+Version: 0.2.1.1a0
 Summary: A little tool to render a simple excel sheet in webpage
 Home-page: https://github.com/shadMod/django-jsheet
 Author: shadMod
-Author-email: shadMod <support@shadmod.it>
-Maintainer-email: ShadMod <support@shadmod.it>
-License: MIT License
-Project-URL: Homepage, https://github.com/shadMod/django-jsheet
+Author-email: support@shadmod.it
 Project-URL: Bug Tracker, https://github.com/shadMod/django-jsheet/issues
-Keywords: Django JSheet,Django-JSheet,Django_JSheet
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django JSheet
 
 Django JSheet is a little tool to render a simple excel sheet in webpage
```

### Comparing `django_jsheet-0.2.1/src/templatetags/jsheet.py` & `django_jsheet-0.2.1.1a0/src/templatetags/jsheet.py`

 * *Files identical despite different names*

