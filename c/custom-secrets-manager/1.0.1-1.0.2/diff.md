# Comparing `tmp/custom_secrets_manager-1.0.1.tar.gz` & `tmp/custom_secrets_manager-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_secrets_manager-1.0.1.tar", last modified: Sat Jun  3 21:11:47 2023, max compression
+gzip compressed data, was "custom_secrets_manager-1.0.2.tar", last modified: Sat Jun  3 22:04:37 2023, max compression
```

## Comparing `custom_secrets_manager-1.0.1.tar` & `custom_secrets_manager-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 21:11:47.325421 custom_secrets_manager-1.0.1/
--rw-r--r--   0 vashishtha   (501) staff       (20)     1696 2023-06-03 21:11:47.313691 custom_secrets_manager-1.0.1/PKG-INFO
--rw-r--r--   0 vashishtha   (501) staff       (20)      943 2023-06-03 21:05:39.000000 custom_secrets_manager-1.0.1/README.md
-drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 21:11:47.292712 custom_secrets_manager-1.0.1/custom_secrets_manager/
--rw-r--r--   0 vashishtha   (501) staff       (20)       22 2023-06-03 21:10:29.000000 custom_secrets_manager-1.0.1/custom_secrets_manager/__init__.py
--rw-r--r--   0 vashishtha   (501) staff       (20)      460 2023-06-03 19:53:35.000000 custom_secrets_manager-1.0.1/custom_secrets_manager/secrets_loader.py
--rw-r--r--   0 vashishtha   (501) staff       (20)     2422 2023-06-03 19:50:25.000000 custom_secrets_manager-1.0.1/custom_secrets_manager/starter_process.py
-drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 21:11:47.301356 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/
--rw-r--r--   0 vashishtha   (501) staff       (20)     1696 2023-06-03 21:11:46.000000 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/PKG-INFO
--rw-r--r--   0 vashishtha   (501) staff       (20)      414 2023-06-03 21:11:46.000000 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/SOURCES.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)        1 2023-06-03 21:11:46.000000 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/dependency_links.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)       87 2023-06-03 21:11:46.000000 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/entry_points.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)       10 2023-06-03 21:11:46.000000 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/requires.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)       23 2023-06-03 21:11:46.000000 custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/top_level.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)       38 2023-06-03 21:11:47.325866 custom_secrets_manager-1.0.1/setup.cfg
--rw-r--r--   0 vashishtha   (501) staff       (20)     1411 2023-06-03 20:39:12.000000 custom_secrets_manager-1.0.1/setup.py
+drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 22:04:37.368783 custom_secrets_manager-1.0.2/
+-rw-r--r--   0 vashishtha   (501) staff       (20)     1696 2023-06-03 22:04:37.368066 custom_secrets_manager-1.0.2/PKG-INFO
+-rw-r--r--   0 vashishtha   (501) staff       (20)      943 2023-06-03 21:05:39.000000 custom_secrets_manager-1.0.2/README.md
+drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 22:04:37.357760 custom_secrets_manager-1.0.2/custom_secrets_manager/
+-rw-r--r--   0 vashishtha   (501) staff       (20)       22 2023-06-03 22:03:21.000000 custom_secrets_manager-1.0.2/custom_secrets_manager/__init__.py
+-rw-r--r--   0 vashishtha   (501) staff       (20)      638 2023-06-03 21:56:56.000000 custom_secrets_manager-1.0.2/custom_secrets_manager/secrets_loader.py
+-rw-r--r--   0 vashishtha   (501) staff       (20)     2422 2023-06-03 19:50:25.000000 custom_secrets_manager-1.0.2/custom_secrets_manager/starter_process.py
+drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 22:04:37.367324 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/
+-rw-r--r--   0 vashishtha   (501) staff       (20)     1696 2023-06-03 22:04:36.000000 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/PKG-INFO
+-rw-r--r--   0 vashishtha   (501) staff       (20)      414 2023-06-03 22:04:36.000000 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 vashishtha   (501) staff       (20)        1 2023-06-03 22:04:36.000000 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 vashishtha   (501) staff       (20)       87 2023-06-03 22:04:36.000000 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/entry_points.txt
+-rw-r--r--   0 vashishtha   (501) staff       (20)       10 2023-06-03 22:04:36.000000 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/requires.txt
+-rw-r--r--   0 vashishtha   (501) staff       (20)       23 2023-06-03 22:04:36.000000 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/top_level.txt
+-rw-r--r--   0 vashishtha   (501) staff       (20)       38 2023-06-03 22:04:37.368935 custom_secrets_manager-1.0.2/setup.cfg
+-rw-r--r--   0 vashishtha   (501) staff       (20)     1411 2023-06-03 20:39:12.000000 custom_secrets_manager-1.0.2/setup.py
```

### Comparing `custom_secrets_manager-1.0.1/PKG-INFO` & `custom_secrets_manager-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom_secrets_manager
-Version: 1.0.1
+Version: 1.0.2
 Summary: A utility for managing secrets and API keys
 Home-page: https://github.com/vvid643/custom_secrets_manager
 Author: Vashishtha Vidyarthi
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `custom_secrets_manager-1.0.1/README.md` & `custom_secrets_manager-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.1/custom_secrets_manager/starter_process.py` & `custom_secrets_manager-1.0.2/custom_secrets_manager/starter_process.py`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.1/custom_secrets_manager.egg-info/PKG-INFO` & `custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-secrets-manager
-Version: 1.0.1
+Version: 1.0.2
 Summary: A utility for managing secrets and API keys
 Home-page: https://github.com/vvid643/custom_secrets_manager
 Author: Vashishtha Vidyarthi
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `custom_secrets_manager-1.0.1/setup.py` & `custom_secrets_manager-1.0.2/setup.py`

 * *Files identical despite different names*

