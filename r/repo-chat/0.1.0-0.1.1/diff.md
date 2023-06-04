# Comparing `tmp/repo-chat-0.1.0.tar.gz` & `tmp/repo_chat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo-chat-0.1.0.tar", last modified: Sat Jun  3 20:32:50 2023, max compression
+gzip compressed data, was "repo_chat-0.1.1.tar", last modified: Sun Jun  4 00:33:43 2023, max compression
```

## Comparing `repo-chat-0.1.0.tar` & `repo_chat-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 20:32:50.382106 repo-chat-0.1.0/
--rw-rw-rw-   0        0        0     2924 2023-06-03 20:32:50.381107 repo-chat-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2472 2023-06-03 13:27:45.000000 repo-chat-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 20:32:50.380103 repo-chat-0.1.0/repo_chat.egg-info/
--rw-rw-rw-   0        0        0     2924 2023-06-03 20:32:50.000000 repo-chat-0.1.0/repo_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-03 20:32:50.000000 repo-chat-0.1.0/repo_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 20:32:50.000000 repo-chat-0.1.0/repo_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-06-03 20:32:50.000000 repo-chat-0.1.0/repo_chat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 20:32:50.000000 repo-chat-0.1.0/repo_chat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 20:32:50.383104 repo-chat-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      918 2023-06-03 20:26:48.000000 repo-chat-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 00:33:43.076262 repo_chat-0.1.1/
+-rw-rw-rw-   0        0        0     2924 2023-06-04 00:33:43.075266 repo_chat-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2472 2023-06-03 13:27:45.000000 repo_chat-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 00:33:43.073746 repo_chat-0.1.1/repo_chat.egg-info/
+-rw-rw-rw-   0        0        0     2924 2023-06-04 00:33:42.000000 repo_chat-0.1.1/repo_chat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-04 00:33:42.000000 repo_chat-0.1.1/repo_chat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 00:33:42.000000 repo_chat-0.1.1/repo_chat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-04 00:33:42.000000 repo_chat-0.1.1/repo_chat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 00:33:42.000000 repo_chat-0.1.1/repo_chat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 00:33:43.077264 repo_chat-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      918 2023-06-04 00:33:41.000000 repo_chat-0.1.1/setup.py
```

### Comparing `repo-chat-0.1.0/PKG-INFO` & `repo_chat-0.1.1/repo_chat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-chat
-Version: 0.1.0
+Version: 0.1.1
 Summary: Using LLMS to facilitate document retrieval and chat operations
 Home-page: https://github.com/voynow/repo-chat
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `repo-chat-0.1.0/README.md` & `repo_chat-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `repo-chat-0.1.0/repo_chat.egg-info/PKG-INFO` & `repo_chat-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: repo-chat
-Version: 0.1.0
+Name: repo_chat
+Version: 0.1.1
 Summary: Using LLMS to facilitate document retrieval and chat operations
 Home-page: https://github.com/voynow/repo-chat
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `repo-chat-0.1.0/setup.py` & `repo_chat-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    name="repo-chat",
-    version="0.1.0",
+    name="repo_chat",
+    version="0.1.1",
     author="Jamie Voynow",
     author_email="voynow99@gmail.com",
     description="Using LLMS to facilitate document retrieval and chat operations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/voynow/repo-chat",
     packages=find_packages(),
```

