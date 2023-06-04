# Comparing `tmp/django_jsheet-0.2.1.4a0.tar.gz` & `tmp/django_jsheet-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_jsheet-0.2.1.4a0.tar", last modified: Sun Jun  4 15:15:09 2023, max compression
+gzip compressed data, was "django_jsheet-0.2.4.tar", last modified: Sun Jun  4 16:14:12 2023, max compression
```

## Comparing `django_jsheet-0.2.1.4a0.tar` & `django_jsheet-0.2.4.tar`

### file list

```diff
@@ -1,28 +1,21 @@
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.108701 django_jsheet-0.2.1.4a0/
--rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/LICENSE
--rw-r--r--   0 shadmod    (501) admin       (80)     1006 2023-06-04 15:15:09.108354 django_jsheet-0.2.1.4a0/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      334 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/README.md
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.091315 django_jsheet-0.2.1.4a0/django_jsheet/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 15:04:42.000000 django_jsheet-0.2.1.4a0/django_jsheet/__init__.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.102358 django_jsheet-0.2.1.4a0/django_jsheet/assets/
--rw-r--r--   0 shadmod    (501) admin       (80)   584927 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/assets/index.js
--rw-r--r--   0 shadmod    (501) admin       (80)    20146 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/assets/jspreadsheet.css
--rw-r--r--   0 shadmod    (501) admin       (80)     1778 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/assets/jspreadsheet.datatables.css
--rw-r--r--   0 shadmod    (501) admin       (80)     5435 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/assets/jspreadsheet.theme.css
--rw-r--r--   0 shadmod    (501) admin       (80)    64721 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/assets/jsuites.css
--rw-r--r--   0 shadmod    (501) admin       (80)   404765 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/assets/jsuites.js
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.088934 django_jsheet-0.2.1.4a0/django_jsheet/src/
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.106387 django_jsheet-0.2.1.4a0/django_jsheet/src/core/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/src/core/__init__.py
--rw-r--r--   0 shadmod    (501) admin       (80)    10692 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/src/core/django_sheet.py
--rw-r--r--   0 shadmod    (501) admin       (80)    10675 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/src/core/views.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.107432 django_jsheet-0.2.1.4a0/django_jsheet/src/templatetags/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/src/templatetags/__init__.py
--rw-r--r--   0 shadmod    (501) admin       (80)     4553 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/src/templatetags/jsheet.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.092809 django_jsheet-0.2.1.4a0/django_jsheet.egg-info/
--rw-r--r--   0 shadmod    (501) admin       (80)     1006 2023-06-04 15:15:09.000000 django_jsheet-0.2.1.4a0/django_jsheet.egg-info/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      616 2023-06-04 15:15:09.000000 django_jsheet-0.2.1.4a0/django_jsheet.egg-info/SOURCES.txt
--rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-04 15:15:09.000000 django_jsheet-0.2.1.4a0/django_jsheet.egg-info/dependency_links.txt
--rw-r--r--   0 shadmod    (501) admin       (80)       14 2023-06-04 15:15:09.000000 django_jsheet-0.2.1.4a0/django_jsheet.egg-info/top_level.txt
--rw-r--r--   0 shadmod    (501) admin       (80)       38 2023-06-04 15:15:09.108795 django_jsheet-0.2.1.4a0/setup.cfg
--rw-r--r--   0 shadmod    (501) admin       (80)     1485 2023-06-04 15:14:54.000000 django_jsheet-0.2.1.4a0/setup.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 16:14:12.095581 django_jsheet-0.2.4/
+-rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-04 13:25:07.000000 django_jsheet-0.2.4/LICENSE
+-rw-r--r--   0 shadmod    (501) admin       (80)     1137 2023-06-04 16:14:12.094980 django_jsheet-0.2.4/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      383 2023-06-04 15:39:11.000000 django_jsheet-0.2.4/README.md
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 16:14:12.088079 django_jsheet-0.2.4/django_jsheet/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 15:04:42.000000 django_jsheet-0.2.4/django_jsheet/__init__.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 16:14:12.085987 django_jsheet-0.2.4/django_jsheet/src/
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 16:14:12.092231 django_jsheet-0.2.4/django_jsheet/src/core/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.4/django_jsheet/src/core/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)    10692 2023-06-04 13:25:07.000000 django_jsheet-0.2.4/django_jsheet/src/core/django_sheet.py
+-rw-r--r--   0 shadmod    (501) admin       (80)    10675 2023-06-04 13:25:07.000000 django_jsheet-0.2.4/django_jsheet/src/core/views.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 16:14:12.093867 django_jsheet-0.2.4/django_jsheet/src/templatetags/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.4/django_jsheet/src/templatetags/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)     4553 2023-06-04 13:25:07.000000 django_jsheet-0.2.4/django_jsheet/src/templatetags/jsheet.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 16:14:12.090062 django_jsheet-0.2.4/django_jsheet.egg-info/
+-rw-r--r--   0 shadmod    (501) admin       (80)     1137 2023-06-04 16:14:12.000000 django_jsheet-0.2.4/django_jsheet.egg-info/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      390 2023-06-04 16:14:12.000000 django_jsheet-0.2.4/django_jsheet.egg-info/SOURCES.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-04 16:14:12.000000 django_jsheet-0.2.4/django_jsheet.egg-info/dependency_links.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       14 2023-06-04 16:14:12.000000 django_jsheet-0.2.4/django_jsheet.egg-info/top_level.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       38 2023-06-04 16:14:12.095748 django_jsheet-0.2.4/setup.cfg
+-rw-r--r--   0 shadmod    (501) admin       (80)     1081 2023-06-04 16:13:09.000000 django_jsheet-0.2.4/setup.py
```

### Comparing `django_jsheet-0.2.1.4a0/LICENSE` & `django_jsheet-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.1.4a0/PKG-INFO` & `django_jsheet-0.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: django_jsheet
-Version: 0.2.1.4a0
+Version: 0.2.4
 Summary: A little tool to render a simple excel sheet in webpage
 Home-page: https://github.com/shadMod/django-jsheet
+Download-URL: https://github.com/shadMod/django-jsheet/archive/refs/tags/0.2.4.tar.gz
 Author: shadMod
 Author-email: support@shadmod.it
 Project-URL: Bug Tracker, https://github.com/shadMod/django-jsheet/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,11 +20,12 @@
 # Django JSheet
 
 Django JSheet is a little tool to render a simple excel sheet in webpage
 
 A sheet is generated with all the data and its history.
 
 No model is required, but you can eventually add it to allows synchronization of data with the db
+(to combine with submodule django_jsheet_assets)
 
 There are many around, but mine is cooler because it's made by me .-.
 
 Good luck! \o/``
```

### Comparing `django_jsheet-0.2.1.4a0/django_jsheet/src/core/django_sheet.py` & `django_jsheet-0.2.4/django_jsheet/src/core/django_sheet.py`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.1.4a0/django_jsheet/src/core/views.py` & `django_jsheet-0.2.4/django_jsheet/src/core/views.py`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.1.4a0/django_jsheet/src/templatetags/jsheet.py` & `django_jsheet-0.2.4/django_jsheet/src/templatetags/jsheet.py`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.1.4a0/django_jsheet.egg-info/PKG-INFO` & `django_jsheet-0.2.4/django_jsheet.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: django-jsheet
-Version: 0.2.1.4a0
+Version: 0.2.4
 Summary: A little tool to render a simple excel sheet in webpage
 Home-page: https://github.com/shadMod/django-jsheet
+Download-URL: https://github.com/shadMod/django-jsheet/archive/refs/tags/0.2.4.tar.gz
 Author: shadMod
 Author-email: support@shadmod.it
 Project-URL: Bug Tracker, https://github.com/shadMod/django-jsheet/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,11 +20,12 @@
 # Django JSheet
 
 Django JSheet is a little tool to render a simple excel sheet in webpage
 
 A sheet is generated with all the data and its history.
 
 No model is required, but you can eventually add it to allows synchronization of data with the db
+(to combine with submodule django_jsheet_assets)
 
 There are many around, but mine is cooler because it's made by me .-.
 
 Good luck! \o/``
```

