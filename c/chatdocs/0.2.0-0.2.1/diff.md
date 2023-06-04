# Comparing `tmp/chatdocs-0.2.0.tar.gz` & `tmp/chatdocs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatdocs-0.2.0.tar", last modified: Sun Jun  4 09:41:07 2023, max compression
+gzip compressed data, was "chatdocs-0.2.1.tar", last modified: Sun Jun  4 21:21:05 2023, max compression
```

## Comparing `chatdocs-0.2.0.tar` & `chatdocs-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 09:41:07.061561 chatdocs-0.2.0/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7086 2023-06-04 09:41:07.061561 chatdocs-0.2.0/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4651 2023-06-04 09:35:47.000000 chatdocs-0.2.0/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 09:41:07.061561 chatdocs-0.2.0/chatdocs/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.2.0/chatdocs/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.2.0/chatdocs/__main__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5657 2023-06-04 03:56:33.000000 chatdocs-0.2.0/chatdocs/add.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      447 2023-06-04 05:02:07.000000 chatdocs-0.2.0/chatdocs/chains.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1284 2023-06-04 05:03:43.000000 chatdocs-0.2.0/chatdocs/chat.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      665 2023-06-04 04:02:06.000000 chatdocs-0.2.0/chatdocs/config.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 09:41:07.061561 chatdocs-0.2.0/chatdocs/data/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      444 2023-06-04 08:12:22.000000 chatdocs-0.2.0/chatdocs/data/chatdocs.yml
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      232 2023-06-04 02:56:51.000000 chatdocs-0.2.0/chatdocs/download.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      491 2023-06-04 01:27:28.000000 chatdocs-0.2.0/chatdocs/embeddings.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1046 2023-06-04 01:41:19.000000 chatdocs-0.2.0/chatdocs/llms.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1129 2023-06-04 06:27:56.000000 chatdocs-0.2.0/chatdocs/main.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      368 2023-06-04 01:08:37.000000 chatdocs-0.2.0/chatdocs/utils.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      914 2023-06-04 03:51:59.000000 chatdocs-0.2.0/chatdocs/vectorstores.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 09:41:07.061561 chatdocs-0.2.0/chatdocs.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7086 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      504 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/entry_points.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      391 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/top_level.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-04 09:41:07.061561 chatdocs-0.2.0/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2127 2023-06-04 09:40:27.000000 chatdocs-0.2.0/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 21:21:05.441810 chatdocs-0.2.1/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7448 2023-06-04 21:21:05.441810 chatdocs-0.2.1/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4917 2023-06-04 21:11:41.000000 chatdocs-0.2.1/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 21:21:05.431810 chatdocs-0.2.1/chatdocs/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.2.1/chatdocs/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.2.1/chatdocs/__main__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5657 2023-06-04 03:56:33.000000 chatdocs-0.2.1/chatdocs/add.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      554 2023-06-04 12:15:53.000000 chatdocs-0.2.1/chatdocs/chains.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1307 2023-06-04 17:42:56.000000 chatdocs-0.2.1/chatdocs/chat.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      665 2023-06-04 04:02:06.000000 chatdocs-0.2.1/chatdocs/config.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 21:21:05.431810 chatdocs-0.2.1/chatdocs/data/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      456 2023-06-04 15:38:55.000000 chatdocs-0.2.1/chatdocs/data/chatdocs.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4272 2023-06-04 20:29:35.000000 chatdocs-0.2.1/chatdocs/data/index.html
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      232 2023-06-04 02:56:51.000000 chatdocs-0.2.1/chatdocs/download.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      491 2023-06-04 01:27:28.000000 chatdocs-0.2.1/chatdocs/embeddings.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1108 2023-06-04 17:37:23.000000 chatdocs-0.2.1/chatdocs/llms.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1259 2023-06-04 11:04:07.000000 chatdocs-0.2.1/chatdocs/main.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1693 2023-06-04 19:41:17.000000 chatdocs-0.2.1/chatdocs/ui.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      368 2023-06-04 01:08:37.000000 chatdocs-0.2.1/chatdocs/utils.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      914 2023-06-04 03:51:59.000000 chatdocs-0.2.1/chatdocs/vectorstores.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 21:21:05.431810 chatdocs-0.2.1/chatdocs.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7448 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      544 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/entry_points.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      413 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/top_level.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-04 21:21:05.441810 chatdocs-0.2.1/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2179 2023-06-04 21:20:27.000000 chatdocs-0.2.1/setup.py
```

### Comparing `chatdocs-0.2.0/PKG-INFO` & `chatdocs-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatdocs
-Version: 0.2.0
+Version: 0.2.1
 Summary: Chat with your documents offline using AI.
 Home-page: https://github.com/marella/chatdocs
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [ChatDocs](https://github.com/marella/chatdocs) [![PyPI](https://img.shields.io/pypi/v/chatdocs)](https://pypi.org/project/chatdocs/) [![tests](https://github.com/marella/chatdocs/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/chatdocs/actions/workflows/tests.yml)
         
@@ -18,14 +18,15 @@
         - [Configuration](#configuration)
         - [GPU](#gpu)
         
         ## Features
         
         - Supports many GGML models via [C Transformers](https://github.com/marella/ctransformers)
         - Supports [🤗 Transformers](https://github.com/huggingface/transformers)
+        - Web UI
         - GPU support
         - Highly configurable via `chatdocs.yml`
         
         ## Installation
         
         Install the tool using:
         
@@ -50,17 +51,32 @@
         ```
         
         > The processed documents will be stored in `db` directory by default.
         
         Chat with your documents using:
         
         ```sh
+        chatdocs ui
+        ```
+        
+        Open http://localhost:5000 in your browser to access the web UI.
+        
+        It also has a nice command-line interface:
+        
+        ```sh
         chatdocs chat
         ```
         
+        <details>
+        <summary><strong>Show preview</strong></summary><br>
+        
+        ![Demo](https://github.com/marella/chatdocs/raw/main/docs/cli.png)
+        
+        </details>
+        
         ## Configuration
         
         All the configuration options can be changed using the `chatdocs.yml` config file. Create a `chatdocs.yml` file in some directory and run all commands from that directory. For reference, see the default [`chatdocs.yml`](https://github.com/marella/chatdocs/blob/main/chatdocs/data/chatdocs.yml) file.
         
         You don't have to copy the entire file, just add the config options you want to change as it will be merged with the default config. For example, see [`tests/fixtures/chatdocs.yml`](https://github.com/marella/chatdocs/blob/main/tests/fixtures/chatdocs.yml) which changes only some of the config options.
         
         ### Embeddings
@@ -172,18 +188,14 @@
         ```yml
         huggingface:
           device: 0
         ```
         
         You may have to reinstall PyTorch with CUDA enabled by following the instructions [here](https://pytorch.org/get-started/locally/).
         
-        ## UI
-        
-        Coming Soon
-        
         ## License
         
         [MIT](https://github.com/marella/chatdocs/blob/main/LICENSE)
         
 Keywords: chatdocs ctransformers transformers langchain chroma ai llm
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `chatdocs-0.2.0/README.md` & `chatdocs-0.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 - [Configuration](#configuration)
 - [GPU](#gpu)
 
 ## Features
 
 - Supports many GGML models via [C Transformers](https://github.com/marella/ctransformers)
 - Supports [🤗 Transformers](https://github.com/huggingface/transformers)
+- Web UI
 - GPU support
 - Highly configurable via `chatdocs.yml`
 
 ## Installation
 
 Install the tool using:
 
@@ -42,17 +43,32 @@
 ```
 
 > The processed documents will be stored in `db` directory by default.
 
 Chat with your documents using:
 
 ```sh
+chatdocs ui
+```
+
+Open http://localhost:5000 in your browser to access the web UI.
+
+It also has a nice command-line interface:
+
+```sh
 chatdocs chat
 ```
 
+<details>
+<summary><strong>Show preview</strong></summary><br>
+
+![Demo](https://github.com/marella/chatdocs/raw/main/docs/cli.png)
+
+</details>
+
 ## Configuration
 
 All the configuration options can be changed using the `chatdocs.yml` config file. Create a `chatdocs.yml` file in some directory and run all commands from that directory. For reference, see the default [`chatdocs.yml`](https://github.com/marella/chatdocs/blob/main/chatdocs/data/chatdocs.yml) file.
 
 You don't have to copy the entire file, just add the config options you want to change as it will be merged with the default config. For example, see [`tests/fixtures/chatdocs.yml`](https://github.com/marella/chatdocs/blob/main/tests/fixtures/chatdocs.yml) which changes only some of the config options.
 
 ### Embeddings
@@ -164,14 +180,10 @@
 ```yml
 huggingface:
   device: 0
 ```
 
 You may have to reinstall PyTorch with CUDA enabled by following the instructions [here](https://pytorch.org/get-started/locally/).
 
-## UI
-
-Coming Soon
-
 ## License
 
 [MIT](https://github.com/marella/chatdocs/blob/main/LICENSE)
```

### Comparing `chatdocs-0.2.0/chatdocs/add.py` & `chatdocs-0.2.1/chatdocs/add.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.0/chatdocs/chat.py` & `chatdocs-0.2.1/chatdocs/chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from rich.panel import Panel
 
 from .chains import get_retrieval_qa
 from .utils import print_answer
 
 
 def chat(config: Dict[str, Any], query: Optional[str] = None) -> None:
-    qa = get_retrieval_qa(config)
+    qa = get_retrieval_qa(config, callback=print_answer)
 
     interactive = not query
     print()
     if interactive:
         print("Type your query below and press Enter.")
         print("Type 'exit' or 'quit' or 'q' to exit the application.\n")
     while True:
```

### Comparing `chatdocs-0.2.0/chatdocs/config.py` & `chatdocs-0.2.1/chatdocs/config.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.0/chatdocs/main.py` & `chatdocs-0.2.1/chatdocs/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,7 +50,15 @@
     ] = None,
     config: ConfigPath = None,
 ):
     from .chat import chat
 
     config = get_config(config)
     chat(config=config, query=query)
+
+
+@app.command()
+def ui(config: ConfigPath = None):
+    from .ui import ui
+
+    config = get_config(config)
+    ui(config=config)
```

### Comparing `chatdocs-0.2.0/chatdocs/vectorstores.py` & `chatdocs-0.2.1/chatdocs/vectorstores.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.0/chatdocs.egg-info/PKG-INFO` & `chatdocs-0.2.1/chatdocs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatdocs
-Version: 0.2.0
+Version: 0.2.1
 Summary: Chat with your documents offline using AI.
 Home-page: https://github.com/marella/chatdocs
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [ChatDocs](https://github.com/marella/chatdocs) [![PyPI](https://img.shields.io/pypi/v/chatdocs)](https://pypi.org/project/chatdocs/) [![tests](https://github.com/marella/chatdocs/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/chatdocs/actions/workflows/tests.yml)
         
@@ -18,14 +18,15 @@
         - [Configuration](#configuration)
         - [GPU](#gpu)
         
         ## Features
         
         - Supports many GGML models via [C Transformers](https://github.com/marella/ctransformers)
         - Supports [🤗 Transformers](https://github.com/huggingface/transformers)
+        - Web UI
         - GPU support
         - Highly configurable via `chatdocs.yml`
         
         ## Installation
         
         Install the tool using:
         
@@ -50,17 +51,32 @@
         ```
         
         > The processed documents will be stored in `db` directory by default.
         
         Chat with your documents using:
         
         ```sh
+        chatdocs ui
+        ```
+        
+        Open http://localhost:5000 in your browser to access the web UI.
+        
+        It also has a nice command-line interface:
+        
+        ```sh
         chatdocs chat
         ```
         
+        <details>
+        <summary><strong>Show preview</strong></summary><br>
+        
+        ![Demo](https://github.com/marella/chatdocs/raw/main/docs/cli.png)
+        
+        </details>
+        
         ## Configuration
         
         All the configuration options can be changed using the `chatdocs.yml` config file. Create a `chatdocs.yml` file in some directory and run all commands from that directory. For reference, see the default [`chatdocs.yml`](https://github.com/marella/chatdocs/blob/main/chatdocs/data/chatdocs.yml) file.
         
         You don't have to copy the entire file, just add the config options you want to change as it will be merged with the default config. For example, see [`tests/fixtures/chatdocs.yml`](https://github.com/marella/chatdocs/blob/main/tests/fixtures/chatdocs.yml) which changes only some of the config options.
         
         ### Embeddings
@@ -172,18 +188,14 @@
         ```yml
         huggingface:
           device: 0
         ```
         
         You may have to reinstall PyTorch with CUDA enabled by following the instructions [here](https://pytorch.org/get-started/locally/).
         
-        ## UI
-        
-        Coming Soon
-        
         ## License
         
         [MIT](https://github.com/marella/chatdocs/blob/main/LICENSE)
         
 Keywords: chatdocs ctransformers transformers langchain chroma ai llm
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `chatdocs-0.2.0/setup.py` & `chatdocs-0.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,36 +3,37 @@
 with open("README.md") as f:
     long_description = f.read()
 
 name = "chatdocs"
 
 setup(
     name=name,
-    version="0.2.0",
+    version="0.2.1",
     description="Chat with your documents offline using AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ravindra Marella",
     author_email="mv.ravindra007@gmail.com",
     url="https://github.com/marella/{}".format(name),
     license="MIT",
     packages=[name],
-    package_data={name: ["data/chatdocs.yml"]},
+    package_data={name: ["data/chatdocs.yml", "data/index.html"]},
     entry_points={
         "console_scripts": [
             f"{name} = {name}.main:app",
         ],
     },
     install_requires=[
         "chromadb>=0.3.0,<0.4.0",
         "ctransformers>=0.2.5,<0.3.0",
         "deepmerge>=1.1.0,<2.0.0",
         "InstructorEmbedding>=1.0.1,<2.0.0",
         "langchain>=0.0.181",
         "pyyaml>=6.0",
+        "quart>=0.18.3,<0.19.0",
         "sentence-transformers>=2.2.2,<3.0.0",
         "tqdm>=4.64.1,<5.0.0",
         "typer>=0.9.0",
         "typing-extensions>=4.4.0,<5.0.0",
         # Document Loaders
         "extract-msg>=0.41.0,<0.42.0",
         "pandoc>=2.3,<3.0.0",
```

