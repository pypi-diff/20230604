# Comparing `tmp/whatsapp-chatbot-python-0.2.0.tar.gz` & `tmp/whatsapp-chatbot-python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chatbot-python-0.2.0.tar", last modified: Fri Jun  2 06:13:43 2023, max compression
+gzip compressed data, was "whatsapp-chatbot-python-0.2.1.tar", last modified: Sun Jun  4 07:05:21 2023, max compression
```

## Comparing `whatsapp-chatbot-python-0.2.0.tar` & `whatsapp-chatbot-python-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 06:13:43.795410 whatsapp-chatbot-python-0.2.0/
--rw-rw-rw-   0        0        0    18829 2023-05-30 11:55:05.000000 whatsapp-chatbot-python-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     8648 2023-06-02 06:13:43.794407 whatsapp-chatbot-python-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     7623 2023-06-01 09:39:39.000000 whatsapp-chatbot-python-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-02 06:13:43.795410 whatsapp-chatbot-python-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1405 2023-06-02 06:13:11.000000 whatsapp-chatbot-python-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:13:43.784381 whatsapp-chatbot-python-0.2.0/tests/
--rw-rw-rw-   0        0        0     1224 2023-06-01 09:34:28.000000 whatsapp-chatbot-python-0.2.0/tests/test_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:13:43.786386 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/
--rw-rw-rw-   0        0        0      184 2023-06-01 09:19:08.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/__init__.py
--rw-rw-rw-   0        0        0     1020 2023-06-01 09:17:35.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/bot.py
--rw-rw-rw-   0        0        0     3569 2023-05-30 11:55:05.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/filters.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:13:43.793404 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/
--rw-rw-rw-   0        0        0        0 2023-05-30 11:55:05.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/__init__.py
--rw-rw-rw-   0        0        0     3277 2023-05-30 11:55:05.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/handler.py
--rw-rw-rw-   0        0        0     1821 2023-05-30 11:55:05.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/observer.py
--rw-rw-rw-   0        0        0     1144 2023-05-30 11:55:05.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/router.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:13:43.790397 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/
--rw-rw-rw-   0        0        0     8648 2023-06-02 06:13:43.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-06-02 06:13:43.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 06:13:43.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-02 06:13:43.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-02 06:13:43.000000 whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 07:05:21.641748 whatsapp-chatbot-python-0.2.1/
+-rw-rw-rw-   0        0        0    18829 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     8648 2023-06-04 07:05:21.641748 whatsapp-chatbot-python-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7623 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-04 07:05:21.641748 whatsapp-chatbot-python-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1405 2023-06-04 07:00:41.000000 whatsapp-chatbot-python-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:05:21.630719 whatsapp-chatbot-python-0.2.1/tests/
+-rw-rw-rw-   0        0        0     1224 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/tests/test_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:05:21.633727 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/
+-rw-rw-rw-   0        0        0      184 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/__init__.py
+-rw-rw-rw-   0        0        0     1020 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/bot.py
+-rw-rw-rw-   0        0        0     3569 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/filters.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:05:21.640745 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/
+-rw-rw-rw-   0        0        0        0 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/__init__.py
+-rw-rw-rw-   0        0        0     3277 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/handler.py
+-rw-rw-rw-   0        0        0     1821 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/observer.py
+-rw-rw-rw-   0        0        0     1144 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/router.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:05:21.637737 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/
+-rw-rw-rw-   0        0        0     8648 2023-06-04 07:05:21.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-06-04 07:05:21.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 07:05:21.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-04 07:05:21.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-04 07:05:21.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/top_level.txt
```

### Comparing `whatsapp-chatbot-python-0.2.0/LICENSE` & `whatsapp-chatbot-python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.0/PKG-INFO` & `whatsapp-chatbot-python-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatsapp-chatbot-python-0.2.0/README.md` & `whatsapp-chatbot-python-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.0/setup.py` & `whatsapp-chatbot-python-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-chatbot-python",
-    version="0.2.0",
+    version="0.2.1",
     description=(
         "This library helps you easily create"
         " a Python chatbot with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
@@ -29,10 +29,10 @@
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Application Frameworks"
     ],
     license=(
         "Creative Commons Attribution-NoDerivatives 4.0 International"
         " (CC BY-ND 4.0)"
     ),
-    install_requires=["whatsapp-api-client-python==0.0.35"],
+    install_requires=["whatsapp-api-client-python==0.0.36"],
     python_requires=">=3.7"
 )
```

### Comparing `whatsapp-chatbot-python-0.2.0/tests/test_manager.py` & `whatsapp-chatbot-python-0.2.1/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/bot.py` & `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/bot.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/filters.py` & `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/filters.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/handler.py` & `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/handler.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/observer.py` & `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/observer.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python/manager/router.py` & `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/router.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/PKG-INFO` & `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatsapp-chatbot-python-0.2.0/whatsapp_chatbot_python.egg-info/SOURCES.txt` & `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

