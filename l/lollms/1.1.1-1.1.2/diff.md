# Comparing `tmp/lollms-1.1.1.tar.gz` & `tmp/lollms-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-1.1.1.tar", last modified: Sun Jun  4 00:24:09 2023, max compression
+gzip compressed data, was "lollms-1.1.2.tar", last modified: Sun Jun  4 00:27:07 2023, max compression
```

## Comparing `lollms-1.1.1.tar` & `lollms-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 00:24:09.033597 lollms-1.1.1/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     7446 2023-06-04 00:24:09.032596 lollms-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6930 2023-06-04 00:10:01.000000 lollms-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 00:24:09.000773 lollms-1.1.1/lollms/
--rw-rw-rw-   0        0        0    32532 2023-06-03 23:06:41.000000 lollms-1.1.1/lollms/__init__.py
--rw-rw-rw-   0        0        0     8270 2023-06-03 23:04:42.000000 lollms-1.1.1/lollms/binding.py
--rw-rw-rw-   0        0        0     9348 2023-06-03 19:43:42.000000 lollms-1.1.1/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     9734 2023-06-03 23:42:16.000000 lollms-1.1.1/lollms/server.py
-drwxrwxrwx   0        0        0        0 2023-06-04 00:24:09.031594 lollms-1.1.1/lollms.egg-info/
--rw-rw-rw-   0        0        0     7446 2023-06-04 00:24:08.000000 lollms-1.1.1/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-06-04 00:24:08.000000 lollms-1.1.1/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 00:24:08.000000 lollms-1.1.1/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-04 00:24:08.000000 lollms-1.1.1/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      143 2023-06-04 00:24:08.000000 lollms-1.1.1/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-04 00:24:08.000000 lollms-1.1.1/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 00:24:09.033597 lollms-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1382 2023-06-04 00:23:34.000000 lollms-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 00:27:07.431555 lollms-1.1.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     7446 2023-06-04 00:27:07.430559 lollms-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6930 2023-06-04 00:10:01.000000 lollms-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 00:27:07.413991 lollms-1.1.2/lollms/
+-rw-rw-rw-   0        0        0    32532 2023-06-03 23:06:41.000000 lollms-1.1.2/lollms/__init__.py
+-rw-rw-rw-   0        0        0     8270 2023-06-03 23:04:42.000000 lollms-1.1.2/lollms/binding.py
+-rw-rw-rw-   0        0        0     9348 2023-06-03 19:43:42.000000 lollms-1.1.2/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     9734 2023-06-03 23:42:16.000000 lollms-1.1.2/lollms/server.py
+drwxrwxrwx   0        0        0        0 2023-06-04 00:27:07.429548 lollms-1.1.2/lollms.egg-info/
+-rw-rw-rw-   0        0        0     7446 2023-06-04 00:27:07.000000 lollms-1.1.2/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-06-04 00:27:07.000000 lollms-1.1.2/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 00:27:07.000000 lollms-1.1.2/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-04 00:27:07.000000 lollms-1.1.2/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      143 2023-06-04 00:27:07.000000 lollms-1.1.2/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-04 00:27:07.000000 lollms-1.1.2/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 00:27:07.431555 lollms-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1361 2023-06-04 00:27:03.000000 lollms-1.1.2/setup.py
```

### Comparing `lollms-1.1.1/LICENSE` & `lollms-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-1.1.1/PKG-INFO` & `lollms-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lollms-1.1.1/README.md` & `lollms-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lollms-1.1.1/lollms/__init__.py` & `lollms-1.1.2/lollms/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-1.1.1/lollms/binding.py` & `lollms-1.1.2/lollms/binding.py`

 * *Files identical despite different names*

### Comparing `lollms-1.1.1/lollms/langchain_integration.py` & `lollms-1.1.2/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-1.1.1/lollms/server.py` & `lollms-1.1.2/lollms/server.py`

 * *Files identical despite different names*

### Comparing `lollms-1.1.1/lollms.egg-info/PKG-INFO` & `lollms-1.1.2/lollms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lollms-1.1.1/setup.py` & `lollms-1.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 
 
 requirements = read_requirements("requirements.txt")
 requirements_dev = read_requirements("requirements_dev.txt")
 
 setuptools.setup(
     name="lollms",
-    version="1.1.1",
+    version="1.1.2",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
     package_data={
         "lollms": [
-            "lollms/bindings_zoo/*",
-            "lollms/personalities_zoo/*",
-            "lollms/assets/*"
+            "bindings_zoo/*",
+            "personalities_zoo/*",
+            "assets/*"
         ]
     },
     include_package_data=True,
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'lollms-server = lollms.server:main',
```

