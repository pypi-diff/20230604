# Comparing `tmp/django_jsheet-0.2.1.3a0.tar.gz` & `tmp/django_jsheet-0.2.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_jsheet-0.2.1.3a0.tar", last modified: Sun Jun  4 15:02:11 2023, max compression
+gzip compressed data, was "django_jsheet-0.2.1.4a0.tar", last modified: Sun Jun  4 15:15:09 2023, max compression
```

## Comparing `django_jsheet-0.2.1.3a0.tar` & `django_jsheet-0.2.1.4a0.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:02:11.049356 django_jsheet-0.2.1.3a0/
--rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/LICENSE
--rw-r--r--   0 shadmod    (501) admin       (80)     1006 2023-06-04 15:02:11.048955 django_jsheet-0.2.1.3a0/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      334 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/README.md
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:02:11.045388 django_jsheet-0.2.1.3a0/django_jsheet.egg-info/
--rw-r--r--   0 shadmod    (501) admin       (80)     1006 2023-06-04 15:02:11.000000 django_jsheet-0.2.1.3a0/django_jsheet.egg-info/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      294 2023-06-04 15:02:11.000000 django_jsheet-0.2.1.3a0/django_jsheet.egg-info/SOURCES.txt
--rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-04 15:02:11.000000 django_jsheet-0.2.1.3a0/django_jsheet.egg-info/dependency_links.txt
--rw-r--r--   0 shadmod    (501) admin       (80)        4 2023-06-04 15:02:11.000000 django_jsheet-0.2.1.3a0/django_jsheet.egg-info/top_level.txt
--rw-r--r--   0 shadmod    (501) admin       (80)       38 2023-06-04 15:02:11.049583 django_jsheet-0.2.1.3a0/setup.cfg
--rw-r--r--   0 shadmod    (501) admin       (80)     1048 2023-06-04 15:01:17.000000 django_jsheet-0.2.1.3a0/setup.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:02:11.042200 django_jsheet-0.2.1.3a0/src/
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:02:11.046933 django_jsheet-0.2.1.3a0/src/core/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/src/core/__init__.py
--rw-r--r--   0 shadmod    (501) admin       (80)    10692 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/src/core/django_sheet.py
--rw-r--r--   0 shadmod    (501) admin       (80)    10675 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/src/core/views.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:02:11.048061 django_jsheet-0.2.1.3a0/src/templatetags/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/src/templatetags/__init__.py
--rw-r--r--   0 shadmod    (501) admin       (80)     4553 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.3a0/src/templatetags/jsheet.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.108701 django_jsheet-0.2.1.4a0/
+-rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/LICENSE
+-rw-r--r--   0 shadmod    (501) admin       (80)     1006 2023-06-04 15:15:09.108354 django_jsheet-0.2.1.4a0/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      334 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/README.md
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.091315 django_jsheet-0.2.1.4a0/django_jsheet/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 15:04:42.000000 django_jsheet-0.2.1.4a0/django_jsheet/__init__.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.102358 django_jsheet-0.2.1.4a0/django_jsheet/assets/
+-rw-r--r--   0 shadmod    (501) admin       (80)   584927 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/assets/index.js
+-rw-r--r--   0 shadmod    (501) admin       (80)    20146 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/assets/jspreadsheet.css
+-rw-r--r--   0 shadmod    (501) admin       (80)     1778 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/assets/jspreadsheet.datatables.css
+-rw-r--r--   0 shadmod    (501) admin       (80)     5435 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/assets/jspreadsheet.theme.css
+-rw-r--r--   0 shadmod    (501) admin       (80)    64721 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/assets/jsuites.css
+-rw-r--r--   0 shadmod    (501) admin       (80)   404765 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/assets/jsuites.js
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.088934 django_jsheet-0.2.1.4a0/django_jsheet/src/
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.106387 django_jsheet-0.2.1.4a0/django_jsheet/src/core/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/src/core/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)    10692 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/src/core/django_sheet.py
+-rw-r--r--   0 shadmod    (501) admin       (80)    10675 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/src/core/views.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.107432 django_jsheet-0.2.1.4a0/django_jsheet/src/templatetags/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/src/templatetags/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)     4553 2023-06-04 13:25:07.000000 django_jsheet-0.2.1.4a0/django_jsheet/src/templatetags/jsheet.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 15:15:09.092809 django_jsheet-0.2.1.4a0/django_jsheet.egg-info/
+-rw-r--r--   0 shadmod    (501) admin       (80)     1006 2023-06-04 15:15:09.000000 django_jsheet-0.2.1.4a0/django_jsheet.egg-info/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      616 2023-06-04 15:15:09.000000 django_jsheet-0.2.1.4a0/django_jsheet.egg-info/SOURCES.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-04 15:15:09.000000 django_jsheet-0.2.1.4a0/django_jsheet.egg-info/dependency_links.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       14 2023-06-04 15:15:09.000000 django_jsheet-0.2.1.4a0/django_jsheet.egg-info/top_level.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       38 2023-06-04 15:15:09.108795 django_jsheet-0.2.1.4a0/setup.cfg
+-rw-r--r--   0 shadmod    (501) admin       (80)     1485 2023-06-04 15:14:54.000000 django_jsheet-0.2.1.4a0/setup.py
```

### Comparing `django_jsheet-0.2.1.3a0/LICENSE` & `django_jsheet-0.2.1.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.1.3a0/PKG-INFO` & `django_jsheet-0.2.1.4a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_jsheet
-Version: 0.2.1.3a0
+Version: 0.2.1.4a0
 Summary: A little tool to render a simple excel sheet in webpage
 Home-page: https://github.com/shadMod/django-jsheet
 Author: shadMod
 Author-email: support@shadmod.it
 Project-URL: Bug Tracker, https://github.com/shadMod/django-jsheet/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `django_jsheet-0.2.1.3a0/django_jsheet.egg-info/PKG-INFO` & `django_jsheet-0.2.1.4a0/django_jsheet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jsheet
-Version: 0.2.1.3a0
+Version: 0.2.1.4a0
 Summary: A little tool to render a simple excel sheet in webpage
 Home-page: https://github.com/shadMod/django-jsheet
 Author: shadMod
 Author-email: support@shadmod.it
 Project-URL: Bug Tracker, https://github.com/shadMod/django-jsheet/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `django_jsheet-0.2.1.3a0/src/core/django_sheet.py` & `django_jsheet-0.2.1.4a0/django_jsheet/src/core/django_sheet.py`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.1.3a0/src/core/views.py` & `django_jsheet-0.2.1.4a0/django_jsheet/src/core/views.py`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.1.3a0/src/templatetags/jsheet.py` & `django_jsheet-0.2.1.4a0/django_jsheet/src/templatetags/jsheet.py`

 * *Files identical despite different names*

