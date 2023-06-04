# Comparing `tmp/repo_chat-0.1.2.tar.gz` & `tmp/repo_chat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo_chat-0.1.2.tar", last modified: Sun Jun  4 00:47:31 2023, max compression
+gzip compressed data, was "repo_chat-0.1.3.tar", last modified: Sun Jun  4 20:44:01 2023, max compression
```

## Comparing `repo_chat-0.1.2.tar` & `repo_chat-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 00:47:31.993024 repo_chat-0.1.2/
--rw-rw-rw-   0        0        0     2924 2023-06-04 00:47:31.992025 repo_chat-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2472 2023-06-03 13:27:45.000000 repo_chat-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 00:47:31.981500 repo_chat-0.1.2/repo_chat/
--rw-rw-rw-   0        0        0        0 2023-06-04 00:46:17.000000 repo_chat-0.1.2/repo_chat/__init__.py
--rw-rw-rw-   0        0        0     1532 2023-06-02 20:27:42.000000 repo_chat-0.1.2/repo_chat/chain_manager.py
--rw-rw-rw-   0        0        0     4895 2023-06-03 21:06:12.000000 repo_chat-0.1.2/repo_chat/chat_utils.py
--rw-rw-rw-   0        0        0     4003 2023-05-26 19:35:36.000000 repo_chat-0.1.2/repo_chat/eval_utils.py
--rw-rw-rw-   0        0        0     3131 2023-06-03 21:06:12.000000 repo_chat-0.1.2/repo_chat/templates.py
-drwxrwxrwx   0        0        0        0 2023-06-04 00:47:31.990017 repo_chat-0.1.2/repo_chat.egg-info/
--rw-rw-rw-   0        0        0     2924 2023-06-04 00:47:31.000000 repo_chat-0.1.2/repo_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-04 00:47:31.000000 repo_chat-0.1.2/repo_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 00:47:31.000000 repo_chat-0.1.2/repo_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-06-04 00:47:31.000000 repo_chat-0.1.2/repo_chat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-04 00:47:31.000000 repo_chat-0.1.2/repo_chat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 00:47:31.993024 repo_chat-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      918 2023-06-04 00:47:20.000000 repo_chat-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 20:44:01.376908 repo_chat-0.1.3/
+-rw-rw-rw-   0        0        0     2924 2023-06-04 20:44:01.375920 repo_chat-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2472 2023-06-03 13:27:45.000000 repo_chat-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 20:44:01.363897 repo_chat-0.1.3/repo_chat/
+-rw-rw-rw-   0        0        0        0 2023-06-04 00:46:17.000000 repo_chat-0.1.3/repo_chat/__init__.py
+-rw-rw-rw-   0        0        0     1666 2023-06-04 20:39:36.000000 repo_chat-0.1.3/repo_chat/chain_manager.py
+-rw-rw-rw-   0        0        0     4895 2023-06-03 21:06:12.000000 repo_chat-0.1.3/repo_chat/chat_utils.py
+-rw-rw-rw-   0        0        0     4003 2023-05-26 19:35:36.000000 repo_chat-0.1.3/repo_chat/eval_utils.py
+-rw-rw-rw-   0        0        0     3131 2023-06-03 21:06:12.000000 repo_chat-0.1.3/repo_chat/templates.py
+drwxrwxrwx   0        0        0        0 2023-06-04 20:44:01.373910 repo_chat-0.1.3/repo_chat.egg-info/
+-rw-rw-rw-   0        0        0     2924 2023-06-04 20:44:01.000000 repo_chat-0.1.3/repo_chat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-04 20:44:01.000000 repo_chat-0.1.3/repo_chat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 20:44:01.000000 repo_chat-0.1.3/repo_chat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-04 20:44:01.000000 repo_chat-0.1.3/repo_chat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 20:44:01.000000 repo_chat-0.1.3/repo_chat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 20:44:01.377907 repo_chat-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      918 2023-06-04 20:43:18.000000 repo_chat-0.1.3/setup.py
```

### Comparing `repo_chat-0.1.2/PKG-INFO` & `repo_chat-0.1.3/repo_chat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: repo_chat
-Version: 0.1.2
+Name: repo-chat
+Version: 0.1.3
 Summary: Using LLMS to facilitate document retrieval and chat operations
 Home-page: https://github.com/voynow/repo-chat
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `repo_chat-0.1.2/README.md` & `repo_chat-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `repo_chat-0.1.2/repo_chat/chain_manager.py` & `repo_chat-0.1.3/repo_chat/chain_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from langchain.prompts import PromptTemplate
 from langchain.chat_models import ChatOpenAI
 from langchain.chains import LLMChain
 from repo_chat import templates
 
 dotenv.load_dotenv()
 OPENAI_API_KEY = os.getenv("OPENAI_API_KEY")
+if not OPENAI_API_KEY:
+    raise ValueError("OPENAI_API_KEY not found. Either create a .env file or set the environment variable.")
 
 
 class CustomChain:
     """
     A class to manage creating and storing chains/openai credentials.
     """
```

### Comparing `repo_chat-0.1.2/repo_chat/chat_utils.py` & `repo_chat-0.1.3/repo_chat/chat_utils.py`

 * *Files identical despite different names*

### Comparing `repo_chat-0.1.2/repo_chat/eval_utils.py` & `repo_chat-0.1.3/repo_chat/eval_utils.py`

 * *Files identical despite different names*

### Comparing `repo_chat-0.1.2/repo_chat/templates.py` & `repo_chat-0.1.3/repo_chat/templates.py`

 * *Files identical despite different names*

### Comparing `repo_chat-0.1.2/repo_chat.egg-info/PKG-INFO` & `repo_chat-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: repo-chat
-Version: 0.1.2
+Name: repo_chat
+Version: 0.1.3
 Summary: Using LLMS to facilitate document retrieval and chat operations
 Home-page: https://github.com/voynow/repo-chat
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `repo_chat-0.1.2/setup.py` & `repo_chat-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="repo_chat",
-    version="0.1.2",
+    version="0.1.3",
     author="Jamie Voynow",
     author_email="voynow99@gmail.com",
     description="Using LLMS to facilitate document retrieval and chat operations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/voynow/repo-chat",
     packages=find_packages(),
```

