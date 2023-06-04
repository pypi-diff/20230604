# Comparing `tmp/voyager_dev-0.0.1-py3-none-any.whl.zip` & `tmp/voyager_dev-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 3696 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-03 23:01 voyager_dev/__init__.py
--rw-r--r--  2.0 unx     2614 b- defN 23-Jun-03 23:01 voyager_dev/voyager_dev.py
--rw-r--r--  2.0 unx     1807 b- defN 23-Jun-03 23:01 voyager_dev-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 23:01 voyager_dev-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 23-Jun-03 23:01 voyager_dev-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-03 23:01 voyager_dev-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      573 b- defN 23-Jun-03 23:01 voyager_dev-0.0.1.dist-info/RECORD
-7 files, 5160 bytes uncompressed, 2668 bytes compressed:  48.3%
+Zip file size: 4622 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-04 15:53 voyager_dev/__init__.py
+-rw-r--r--  2.0 unx      997 b- defN 23-Jun-04 15:53 voyager_dev/create_directory_diagram.py
+-rw-r--r--  2.0 unx     2614 b- defN 23-Jun-04 15:53 voyager_dev/voyager_dev.py
+-rw-r--r--  2.0 unx     2457 b- defN 23-Jun-04 15:53 voyager_dev-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 15:53 voyager_dev-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-04 15:53 voyager_dev-0.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-04 15:53 voyager_dev-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      668 b- defN 23-Jun-04 15:53 voyager_dev-0.0.2.dist-info/RECORD
+8 files, 6902 bytes uncompressed, 3440 bytes compressed:  50.2%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: voyager_dev/__init__.py
 Comment: 
 
+Filename: voyager_dev/create_directory_diagram.py
+Comment: 
+
 Filename: voyager_dev/voyager_dev.py
 Comment: 
 
-Filename: voyager_dev-0.0.1.dist-info/METADATA
+Filename: voyager_dev-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: voyager_dev-0.0.1.dist-info/WHEEL
+Filename: voyager_dev-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: voyager_dev-0.0.1.dist-info/entry_points.txt
+Filename: voyager_dev-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: voyager_dev-0.0.1.dist-info/top_level.txt
+Filename: voyager_dev-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: voyager_dev-0.0.1.dist-info/RECORD
+Filename: voyager_dev-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `voyager_dev-0.0.1.dist-info/METADATA` & `voyager_dev-0.0.2.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: voyager-dev
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for coding assistance
-Home-page: https://github.com/coyotespike/voyager_dev
+Home-page: https://github.com/coyotespike/voyager-dev
 Author: Timothy Roy
 Author-email: tim@gradientflow.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,17 +14,23 @@
 Description-Content-Type: text/markdown
 
 ## ✨ Coding Assistant ✨
 
 
 This project aims to develop a usable coding agent, which will work iteratively in collaboration with a developer.
 
-At the current time, BabyAgi/AutoGPT approaches are too unstable to be of very much assistance. However, there is every reason to develop an agent that learns from its environment, from its mistakes, and from your chat history, and develops tools as needed (Voyager).
+At the current time, BabyAgi/AutoGPT approaches are too unstable to be of very much assistance. However, there is every reason to develop an agent that learns from its environment, from its mistakes, and from your chat history. In the future we hope to allow it to develop LangChain tools as needed (Voyager).
 
-# Usage
+## Usage
+
+After installation, you can run `voyager_dev` from anywhere on the command line. You may optionally provide a prompt, `voyager_dev what is the weather today?`, or you can just hit enter and it will ask you for a prompt.
+
+For more complex prompts, place them in a file and provide the filename as the prompt. For example, `voyager_dev myprompt.txt`. This enables multiline prompts more easily.
+
+## Installation
 
 You can install this from [PyPi](https://pypi.org/project/voyager-dev/) with `pip install voyager_dev`.
 
 Alternatively, you can clone this repository. Then to install this repository as a global Python CLI tool, run `pip install -e .`
 
 Either way, you should also put your OpenAI and Google Search API keys in your .bashrc or .zshrc file, like this:
 
@@ -32,11 +38,13 @@
 export OPENAI_API_KEY=yourkeyhere
 export GOOGLE_API_KEY=yourkeyhere
 export GOOGLE_CSE_ID=yourkeyhere
 ```
 
 You can get the latter two by creating the GOOGLE_API_KEY in the [Google Cloud credential console](https://console.cloud.google.com/apis/credentials) and a GOOGLE_CSE_ID using the [Programmable Search Engine](https://programmablesearchengine.google.com/controlpanel/create). Examine the output carefully the first time you run it, Google may return a detailed error telling you how to fix it.
 
-After that, you can simply type `voyager_dev` anywhere on the command line.
+Finally, install and run redis (for the memory store) with `brew install redis` and `brew services start redis`. (You can also use `redis-server` if you don't want it to run in the background.)
 
+After that, you can simply type `voyager_dev` anywhere on the command line.
 
+#
```

