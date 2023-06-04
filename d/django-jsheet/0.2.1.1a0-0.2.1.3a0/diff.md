# Comparing `tmp/django_jsheet-0.2.1.1a0.tar.gz` & `tmp/django_jsheet-0.2.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_jsheet-0.2.1.1a0.tar", last modified: Sun Jun  4 14:44:48 2023, max compression
+gzip compressed data, was "django_jsheet-0.2.1.3a0.tar", last modified: Sun Jun  4 15:02:11 2023, max compression
```

## Comparing `django_jsheet-0.2.1.1a0.tar` & `django_jsheet-0.2.1.3a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:44:48.322491 django_jsheet-0.2.1.1a0/
--rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/LICENSE
--rw-r--r--   0 shadmod    (501) admin       (80)      912 2023-06-04 14:44:48.322130 django_jsheet-0.2.1.1a0/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      334 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/README.md
--rw-r--r--   0 shadmod    (501) admin       (80)       38 2023-06-04 14:44:48.322584 django_jsheet-0.2.1.1a0/setup.cfg
--rw-r--r--   0 shadmod    (501) admin       (80)      973 2023-06-04 14:42:34.000000 django_jsheet-0.2.1.1a0/setup.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:44:48.316660 django_jsheet-0.2.1.1a0/src/
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:44:48.318966 django_jsheet-0.2.1.1a0/src/core/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/src/core/__init__.py
--rw-r--r--   0 shadmod    (501) admin       (80)    10692 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/src/core/django_sheet.py
--rw-r--r--   0 shadmod    (501) admin       (80)    10675 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/src/core/views.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:44:48.320806 django_jsheet-0.2.1.1a0/src/django_jsheet.egg-info/
--rw-r--r--   0 shadmod    (501) admin       (80)      912 2023-06-04 14:44:48.000000 django_jsheet-0.2.1.1a0/src/django_jsheet.egg-info/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      310 2023-06-04 14:44:48.000000 django_jsheet-0.2.1.1a0/src/django_jsheet.egg-info/SOURCES.txt
--rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-04 14:44:48.000000 django_jsheet-0.2.1.1a0/src/django_jsheet.egg-info/dependency_links.txt
--rw-r--r--   0 shadmod    (501) admin       (80)       32 2023-06-04 14:44:48.000000 django_jsheet-0.2.1.1a0/src/django_jsheet.egg-info/top_level.txt
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:44:48.321622 django_jsheet-0.2.1.1a0/src/templatetags/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/src/templatetags/__init__.py
--rw-r--r--   0 shadmod    (501) admin       (80)     4553 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.1a0/src/templatetags/jsheet.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:02:11.049356 django_jsheet-0.2.1.3a0/
+-rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/LICENSE
+-rw-r--r--   0 shadmod    (501) admin       (80)     1006 2023-06-04 15:02:11.048955 django_jsheet-0.2.1.3a0/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      334 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/README.md
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:02:11.045388 django_jsheet-0.2.1.3a0/django_jsheet.egg-info/
+-rw-r--r--   0 shadmod    (501) admin       (80)     1006 2023-06-04 15:02:11.000000 django_jsheet-0.2.1.3a0/django_jsheet.egg-info/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      294 2023-06-04 15:02:11.000000 django_jsheet-0.2.1.3a0/django_jsheet.egg-info/SOURCES.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-04 15:02:11.000000 django_jsheet-0.2.1.3a0/django_jsheet.egg-info/dependency_links.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)        4 2023-06-04 15:02:11.000000 django_jsheet-0.2.1.3a0/django_jsheet.egg-info/top_level.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       38 2023-06-04 15:02:11.049583 django_jsheet-0.2.1.3a0/setup.cfg
+-rw-r--r--   0 shadmod    (501) admin       (80)     1048 2023-06-04 15:01:17.000000 django_jsheet-0.2.1.3a0/setup.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:02:11.042200 django_jsheet-0.2.1.3a0/src/
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:02:11.046933 django_jsheet-0.2.1.3a0/src/core/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/src/core/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)    10692 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/src/core/django_sheet.py
+-rw-r--r--   0 shadmod    (501) admin       (80)    10675 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/src/core/views.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:02:11.048061 django_jsheet-0.2.1.3a0/src/templatetags/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/src/templatetags/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)     4553 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/src/templatetags/jsheet.py
```

### Comparing `django_jsheet-0.2.1.1a0/LICENSE` & `django_jsheet-0.2.1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.1.1a0/PKG-INFO` & `django_jsheet-0.2.1.3a0/django_jsheet.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
-Name: django_jsheet
-Version: 0.2.1.1a0
+Name: django-jsheet
+Version: 0.2.1.3a0
 Summary: A little tool to render a simple excel sheet in webpage
 Home-page: https://github.com/shadMod/django-jsheet
 Author: shadMod
 Author-email: support@shadmod.it
 Project-URL: Bug Tracker, https://github.com/shadMod/django-jsheet/issues
 Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django JSheet
 
 Django JSheet is a little tool to render a simple excel sheet in webpage
```

### Comparing `django_jsheet-0.2.1.1a0/setup.py` & `django_jsheet-0.2.1.3a0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django_jsheet",
-    version="0.2.1.1a",
+    version="0.2.1.3a",
     author="shadMod",
     author_email="support@shadmod.it",
     description="A little tool to render a simple excel sheet in webpage",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shadMod/django-jsheet",
     project_urls={
         "Bug Tracker": "https://github.com/shadMod/django-jsheet/issues",
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
-        "Programming Language :: Python :: 3",
+        "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+    ],
+    package_dir={"assets": "assets"},
+    packages=[
+        "src.core", "src.templatetags",
     ],
-    py_modules=["django_jsheet"],
-    package_dir={"": "src"},
-    packages=setuptools.find_packages(where="src"),
     package_data={
-        "assets": ["assets/index.js"],
+        "assets": ["*.js", "*.css"],
     },
     python_requires=">=3.7"
 )
```

### Comparing `django_jsheet-0.2.1.1a0/src/core/django_sheet.py` & `django_jsheet-0.2.1.3a0/src/core/django_sheet.py`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.1.1a0/src/core/views.py` & `django_jsheet-0.2.1.3a0/src/core/views.py`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.1.1a0/src/django_jsheet.egg-info/PKG-INFO` & `django_jsheet-0.2.1.3a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
-Name: django-jsheet
-Version: 0.2.1.1a0
+Name: django_jsheet
+Version: 0.2.1.3a0
 Summary: A little tool to render a simple excel sheet in webpage
 Home-page: https://github.com/shadMod/django-jsheet
 Author: shadMod
 Author-email: support@shadmod.it
 Project-URL: Bug Tracker, https://github.com/shadMod/django-jsheet/issues
 Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django JSheet
 
 Django JSheet is a little tool to render a simple excel sheet in webpage
```

### Comparing `django_jsheet-0.2.1.1a0/src/templatetags/jsheet.py` & `django_jsheet-0.2.1.3a0/src/templatetags/jsheet.py`

 * *Files identical despite different names*

