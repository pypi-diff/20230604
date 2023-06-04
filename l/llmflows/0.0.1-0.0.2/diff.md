# Comparing `tmp/llmflows-0.0.1.tar.gz` & `tmp/llmflows-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmflows-0.0.1.tar", last modified: Mon May 29 04:07:54 2023, max compression
+gzip compressed data, was "llmflows-0.0.2.tar", last modified: Sun Jun  4 17:54:47 2023, max compression
```

## Comparing `llmflows-0.0.1.tar` & `llmflows-0.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 stoyan     (501) staff       (20)        0 2023-05-29 04:07:54.797179 llmflows-0.0.1/
--rw-r--r--   0 stoyan     (501) staff       (20)     1063 2023-04-19 02:15:48.000000 llmflows-0.0.1/LICENSE
--rw-r--r--   0 stoyan     (501) staff       (20)     6230 2023-05-29 04:07:54.797046 llmflows-0.0.1/PKG-INFO
--rw-r--r--   0 stoyan     (501) staff       (20)     5711 2023-05-28 23:10:07.000000 llmflows-0.0.1/README.md
-drwxr-xr-x   0 stoyan     (501) staff       (20)        0 2023-05-29 04:07:54.790955 llmflows-0.0.1/llmflow/
--rw-r--r--   0 stoyan     (501) staff       (20)        0 2023-04-19 05:02:17.000000 llmflows-0.0.1/llmflow/__init__.py
-drwxr-xr-x   0 stoyan     (501) staff       (20)        0 2023-05-29 04:07:54.793238 llmflows-0.0.1/llmflow/examples/
--rw-r--r--   0 stoyan     (501) staff       (20)        0 2023-04-22 20:06:43.000000 llmflows-0.0.1/llmflow/examples/__init__.py
--rw-r--r--   0 stoyan     (501) staff       (20)     2153 2023-05-27 17:35:10.000000 llmflows-0.0.1/llmflow/examples/chaining_chat_llms_4_2.py
--rw-r--r--   0 stoyan     (501) staff       (20)     1878 2023-05-25 15:52:10.000000 llmflows-0.0.1/llmflow/examples/chaining_llms_4_1.py
--rw-r--r--   0 stoyan     (501) staff       (20)     1236 2023-05-27 17:35:10.000000 llmflows-0.0.1/llmflow/examples/chat_llm_2_2.py
--rw-r--r--   0 stoyan     (501) staff       (20)     1328 2023-05-27 17:35:10.000000 llmflows-0.0.1/llmflow/examples/chat_prompt_templates_3_2.py
--rw-r--r--   0 stoyan     (501) staff       (20)     2917 2023-05-28 15:40:05.000000 llmflows-0.0.1/llmflow/examples/complex_async_flows_6_1.py
--rw-r--r--   0 stoyan     (501) staff       (20)     2563 2023-05-28 02:11:08.000000 llmflows-0.0.1/llmflow/examples/complex_flows_6_1.py
--rw-r--r--   0 stoyan     (501) staff       (20)     2256 2023-05-28 02:11:08.000000 llmflows-0.0.1/llmflow/examples/creating_flows_5_1.py
--rw-r--r--   0 stoyan     (501) staff       (20)     2979 2023-05-25 15:51:47.000000 llmflows-0.0.1/llmflow/examples/getting_started_1_1.py
--rw-r--r--   0 stoyan     (501) staff       (20)     2955 2023-05-27 17:35:10.000000 llmflows-0.0.1/llmflow/examples/getting_started_1_2.py
--rw-r--r--   0 stoyan     (501) staff       (20)      773 2023-05-25 15:51:37.000000 llmflows-0.0.1/llmflow/examples/llm_2_1.py
--rw-r--r--   0 stoyan     (501) staff       (20)     1053 2023-05-25 15:51:30.000000 llmflows-0.0.1/llmflow/examples/prompt_templates_3_1.py
--rw-r--r--   0 stoyan     (501) staff       (20)     6828 2023-05-25 15:51:27.000000 llmflows-0.0.1/llmflow/examples/question_answering.py
-drwxr-xr-x   0 stoyan     (501) staff       (20)        0 2023-05-29 04:07:54.794872 llmflows-0.0.1/llmflow/flows/
--rw-r--r--   0 stoyan     (501) staff       (20)        0 2023-04-19 05:02:17.000000 llmflows-0.0.1/llmflow/flows/__init__.py
--rw-r--r--   0 stoyan     (501) staff       (20)     3563 2023-05-28 16:29:21.000000 llmflows-0.0.1/llmflow/flows/async_flow.py
--rw-r--r--   0 stoyan     (501) staff       (20)     3306 2023-05-28 16:27:47.000000 llmflows-0.0.1/llmflow/flows/async_flowstep.py
--rw-r--r--   0 stoyan     (501) staff       (20)     3694 2023-05-28 16:29:26.000000 llmflows-0.0.1/llmflow/flows/flow.py
--rw-r--r--   0 stoyan     (501) staff       (20)     3380 2023-05-28 16:27:47.000000 llmflows-0.0.1/llmflow/flows/flowstep.py
--rw-r--r--   0 stoyan     (501) staff       (20)        0 2023-05-21 18:01:07.000000 llmflows-0.0.1/llmflow/flows/threaded_flow.py
--rw-r--r--   0 stoyan     (501) staff       (20)        0 2023-05-21 18:02:08.000000 llmflows-0.0.1/llmflow/flows/threaded_flowstep.py
-drwxr-xr-x   0 stoyan     (501) staff       (20)        0 2023-05-29 04:07:54.795686 llmflows-0.0.1/llmflow/llms/
--rw-r--r--   0 stoyan     (501) staff       (20)        0 2023-04-19 05:02:17.000000 llmflows-0.0.1/llmflow/llms/__init__.py
--rw-r--r--   0 stoyan     (501) staff       (20)      495 2023-05-26 04:44:50.000000 llmflows-0.0.1/llmflow/llms/llm.py
--rw-r--r--   0 stoyan     (501) staff       (20)     2260 2023-05-28 15:53:26.000000 llmflows-0.0.1/llmflow/llms/openai.py
--rw-r--r--   0 stoyan     (501) staff       (20)     3823 2023-05-27 17:35:10.000000 llmflows-0.0.1/llmflow/llms/openai_chat.py
--rw-r--r--   0 stoyan     (501) staff       (20)     1928 2023-05-26 05:06:32.000000 llmflows-0.0.1/llmflow/llms/openai_embeddings.py
-drwxr-xr-x   0 stoyan     (501) staff       (20)        0 2023-05-29 04:07:54.795912 llmflows-0.0.1/llmflow/prompts/
--rw-r--r--   0 stoyan     (501) staff       (20)        0 2023-04-19 05:02:55.000000 llmflows-0.0.1/llmflow/prompts/__init__.py
--rw-r--r--   0 stoyan     (501) staff       (20)     1403 2023-05-26 05:08:19.000000 llmflows-0.0.1/llmflow/prompts/prompt_template.py
-drwxr-xr-x   0 stoyan     (501) staff       (20)        0 2023-05-29 04:07:54.796278 llmflows-0.0.1/llmflow/vectorstores/
--rw-r--r--   0 stoyan     (501) staff       (20)        0 2023-04-19 05:02:17.000000 llmflows-0.0.1/llmflow/vectorstores/__init__.py
--rw-r--r--   0 stoyan     (501) staff       (20)     2546 2023-05-26 04:53:05.000000 llmflows-0.0.1/llmflow/vectorstores/pinecone.py
--rw-r--r--   0 stoyan     (501) staff       (20)     2674 2023-05-26 05:10:11.000000 llmflows-0.0.1/llmflow/vectorstores/vector_doc.py
-drwxr-xr-x   0 stoyan     (501) staff       (20)        0 2023-05-29 04:07:54.796866 llmflows-0.0.1/llmflows.egg-info/
--rw-r--r--   0 stoyan     (501) staff       (20)     6230 2023-05-29 04:07:54.000000 llmflows-0.0.1/llmflows.egg-info/PKG-INFO
--rw-r--r--   0 stoyan     (501) staff       (20)     1203 2023-05-29 04:07:54.000000 llmflows-0.0.1/llmflows.egg-info/SOURCES.txt
--rw-r--r--   0 stoyan     (501) staff       (20)        1 2023-05-29 04:07:54.000000 llmflows-0.0.1/llmflows.egg-info/dependency_links.txt
--rw-r--r--   0 stoyan     (501) staff       (20)       79 2023-05-29 04:07:54.000000 llmflows-0.0.1/llmflows.egg-info/requires.txt
--rw-r--r--   0 stoyan     (501) staff       (20)        8 2023-05-29 04:07:54.000000 llmflows-0.0.1/llmflows.egg-info/top_level.txt
--rw-r--r--   0 stoyan     (501) staff       (20)      722 2023-05-29 04:07:37.000000 llmflows-0.0.1/pyproject.toml
--rw-r--r--   0 stoyan     (501) staff       (20)       38 2023-05-29 04:07:54.797219 llmflows-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.023666 llmflows-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-04 17:54:37.000000 llmflows-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-04 17:54:47.023666 llmflows-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-06-04 17:54:37.000000 llmflows-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.015667 llmflows-0.0.2/llmflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.019667 llmflows-0.0.2/llmflows/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/chaining_chat_llms_4_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/chaining_llms_4_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/chat_llm_2_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/chat_prompt_templates_3_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/complex_async_flows_6_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/complex_flows_6_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/creating_flows_5_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/getting_started_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/getting_started_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/llm_2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/prompt_templates_3_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/question_answering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.023666 llmflows-0.0.2/llmflows/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/async_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/async_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/threaded_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/threaded_flowstep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.023666 llmflows-0.0.2/llmflows/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/llms/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/llms/openai_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/llms/openai_embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.023666 llmflows-0.0.2/llmflows/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/prompts/prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.023666 llmflows-0.0.2/llmflows/vectorstores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/vectorstores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/vectorstores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/vectorstores/vector_doc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.015667 llmflows-0.0.2/llmflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-04 17:54:47.000000 llmflows-0.0.2/llmflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-04 17:54:47.000000 llmflows-0.0.2/llmflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 17:54:47.000000 llmflows-0.0.2/llmflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-04 17:54:47.000000 llmflows-0.0.2/llmflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 17:54:47.000000 llmflows-0.0.2/llmflows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-04 17:54:37.000000 llmflows-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 17:54:47.023666 llmflows-0.0.2/setup.cfg
```

### Comparing `llmflows-0.0.1/LICENSE` & `llmflows-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.1/PKG-INFO` & `llmflows-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflows
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple and lightweight library for creating LLM-powered applications.
 Author: Stoyan Stoyanov
 Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflow
 Project-URL: github, https://github.com/stoyan-stoyanov/llmflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,65 +12,65 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <img src="docs/logo.png" />
 </p>
 
-[![Twitter](https://img.shields.io/twitter/follow/LLMFlow?style=social)](https://twitter.com/LLMFlow)
+[![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
 
 ## Installation
 ```
-pip install llmflow
+pip install llmflows
 ```
 
-## What is LLMFlow?
+## What is LLMFlowss?
 A simple and lightweitght library for creating LLM-powered applications.
 
 ## Philosophy
 
 ### Simple
-We have created LLMFlow with simplicity in mind while balancing for usability. We have a minimal set of classes that allow users to build powerful LLM-powered apps without compromising on capabilities.
+We have created LLMFlows with simplicity in mind while balancing for usability. We have a minimal set of classes that allow users to build powerful LLM-powered apps without compromising on capabilities.
 
 ### Explicit
 We allow users to easily create complex LLM flows but we don't 
 
 ### Transparent
 We don't have classes with hidden prompts - prompts are for you to decide.
 
 ## Example
 Here is a basic example for creating an LLM with PromptTemplate:
-```python
 
-from llmflow.llms.openai import OpenAI
-from llmflow.prompts.prompt_template import PromptTemplate
+```python
 
+from llmflows.llms.openai import OpenAI
+from llmflows.prompts.prompt_template import PromptTemplate
 
 prompt_template = PromptTemplate(
-    prompt="Generate a title for a 90s hip-hop song about {topic}."
+   prompt="Generate a title for a 90s hip-hop song about {topic}."
 )
 llm_prompt = prompt_template.get_prompt(topic="friendship")
 
 print(llm_prompt)
 
 llm = OpenAI()
 song_title = llm.generate(llm_prompt)
 print(song_title)
 
 ```
 
-While this is a good example on how easy it is to use LLMFlow, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
+While this is a good example on how easy it is to use LLMFlows, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
 ![Complex flow](docs/complex_flow.png)
-With LLMFlow it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlow will figure out the dependencies for you and make sure each flowstep is executed only when the flowsteps it depends on are complete:
+With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies for you and make sure each flowstep is executed only when the flowsteps it depends on are complete:
 
 ```python
-from llmflow.flows.flow import Flow
-from llmflow.flows.flowstep import FlowStep
-from llmflow.llms.openai import OpenAI
-from llmflow.prompts.prompt_template import PromptTemplate
+from llmflows.flows.flow import Flow
+from llmflows.flows.flowstep import FlowStep
+from llmflows.llms.openai import OpenAI
+from llmflows.prompts.prompt_template import PromptTemplate
 
 # Create LLM
 open_ai_llm = OpenAI()
 
 # Create prompt templates
 title_template = PromptTemplate("What is a good title of a movie about {topic}?")
 song_template = PromptTemplate(
@@ -119,15 +119,15 @@
 flowstep3.connect(flowstep4)
 
 # Create and run Flow
 soundtrack_flow = Flow(flowstep1)
 soundtrack_flow.execute(topic="friendship")
 
 ```
-In fact, LLMFlow provides async, and threaded classes so any complex DAG can be executed in parallel.
+In fact, LLMFlows provides async, and threaded classes so any complex DAG can be executed in parallel.
 For more examples such as how to create Q&A apps and web applications with Flask and FastAPI check our documentation.
 
 ## Usage patterns 
 1. Use LLMs-only
 
     Use the LLM and Agents classes and tools to build free-roaming agents   
 
@@ -138,15 +138,15 @@
 3. Build web apps
 
     Execute agents inside flowsteps where you can build conversational experiences with different stages and requirements
 
 ## FAQ
 
 ### How is this different than langchian?
-Langchain is an amazing library and LLMFlow has been certainly been inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and while this is great for beginners and people who are not in the field of machine learning and language models, this can be a bit overwhelming. There are a lot of classes, hidden prompts in chains and many ways to do things. In contrast we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
+Langchain is an amazing library and LLMFlows has been certainly been inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and while this is great for beginners and people who are not in the field of machine learning and language models, this can be a bit overwhelming. There are a lot of classes, hidden prompts in chains and many ways to do things. In contrast we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
 
 ### You only have OpenAI wrappers but I want to use ACMELLM
 We decided to release the library initially supporting only OpenAI LLMs but we have a roadmap and we will slowly add new wrappers around the most popular models. If you are willing to spend some time we are looking for contributors and maintainers
 
 ### You only support Pinecone and Redis vector DBs do you have plans to extend the list?
 Yes! We will also add Redis, Elastic Search and other popular solutions over time. If you want to help us out check out our contribution section.
```

### Comparing `llmflows-0.0.1/README.md` & `llmflows-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 <p align="center">
   <img src="docs/logo.png" />
 </p>
 
-[![Twitter](https://img.shields.io/twitter/follow/LLMFlow?style=social)](https://twitter.com/LLMFlow)
+[![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
 
 ## Installation
 ```
-pip install llmflow
+pip install llmflows
 ```
 
-## What is LLMFlow?
+## What is LLMFlowss?
 A simple and lightweitght library for creating LLM-powered applications.
 
 ## Philosophy
 
 ### Simple
-We have created LLMFlow with simplicity in mind while balancing for usability. We have a minimal set of classes that allow users to build powerful LLM-powered apps without compromising on capabilities.
+We have created LLMFlows with simplicity in mind while balancing for usability. We have a minimal set of classes that allow users to build powerful LLM-powered apps without compromising on capabilities.
 
 ### Explicit
 We allow users to easily create complex LLM flows but we don't 
 
 ### Transparent
 We don't have classes with hidden prompts - prompts are for you to decide.
 
 ## Example
 Here is a basic example for creating an LLM with PromptTemplate:
-```python
 
-from llmflow.llms.openai import OpenAI
-from llmflow.prompts.prompt_template import PromptTemplate
+```python
 
+from llmflows.llms.openai import OpenAI
+from llmflows.prompts.prompt_template import PromptTemplate
 
 prompt_template = PromptTemplate(
-    prompt="Generate a title for a 90s hip-hop song about {topic}."
+   prompt="Generate a title for a 90s hip-hop song about {topic}."
 )
 llm_prompt = prompt_template.get_prompt(topic="friendship")
 
 print(llm_prompt)
 
 llm = OpenAI()
 song_title = llm.generate(llm_prompt)
 print(song_title)
 
 ```
 
-While this is a good example on how easy it is to use LLMFlow, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
+While this is a good example on how easy it is to use LLMFlows, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
 ![Complex flow](docs/complex_flow.png)
-With LLMFlow it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlow will figure out the dependencies for you and make sure each flowstep is executed only when the flowsteps it depends on are complete:
+With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies for you and make sure each flowstep is executed only when the flowsteps it depends on are complete:
 
 ```python
-from llmflow.flows.flow import Flow
-from llmflow.flows.flowstep import FlowStep
-from llmflow.llms.openai import OpenAI
-from llmflow.prompts.prompt_template import PromptTemplate
+from llmflows.flows.flow import Flow
+from llmflows.flows.flowstep import FlowStep
+from llmflows.llms.openai import OpenAI
+from llmflows.prompts.prompt_template import PromptTemplate
 
 # Create LLM
 open_ai_llm = OpenAI()
 
 # Create prompt templates
 title_template = PromptTemplate("What is a good title of a movie about {topic}?")
 song_template = PromptTemplate(
@@ -105,15 +105,15 @@
 flowstep3.connect(flowstep4)
 
 # Create and run Flow
 soundtrack_flow = Flow(flowstep1)
 soundtrack_flow.execute(topic="friendship")
 
 ```
-In fact, LLMFlow provides async, and threaded classes so any complex DAG can be executed in parallel.
+In fact, LLMFlows provides async, and threaded classes so any complex DAG can be executed in parallel.
 For more examples such as how to create Q&A apps and web applications with Flask and FastAPI check our documentation.
 
 ## Usage patterns 
 1. Use LLMs-only
 
     Use the LLM and Agents classes and tools to build free-roaming agents   
 
@@ -124,15 +124,15 @@
 3. Build web apps
 
     Execute agents inside flowsteps where you can build conversational experiences with different stages and requirements
 
 ## FAQ
 
 ### How is this different than langchian?
-Langchain is an amazing library and LLMFlow has been certainly been inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and while this is great for beginners and people who are not in the field of machine learning and language models, this can be a bit overwhelming. There are a lot of classes, hidden prompts in chains and many ways to do things. In contrast we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
+Langchain is an amazing library and LLMFlows has been certainly been inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and while this is great for beginners and people who are not in the field of machine learning and language models, this can be a bit overwhelming. There are a lot of classes, hidden prompts in chains and many ways to do things. In contrast we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
 
 ### You only have OpenAI wrappers but I want to use ACMELLM
 We decided to release the library initially supporting only OpenAI LLMs but we have a roadmap and we will slowly add new wrappers around the most popular models. If you are willing to spend some time we are looking for contributors and maintainers
 
 ### You only support Pinecone and Redis vector DBs do you have plans to extend the list?
 Yes! We will also add Redis, Elastic Search and other popular solutions over time. If you want to help us out check out our contribution section.
```

### Comparing `llmflows-0.0.1/llmflow/examples/chaining_chat_llms_4_2.py` & `llmflows-0.0.2/llmflows/examples/chaining_chat_llms_4_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 Example:
     $ python chaining_chat_llms_4_2.py
     "The Power of Friendship"
     "Verse 1: When I'm feeling down, you're always there to lift me up..."
     "Verse 1: When the darkness comes, I'll stand my ground and fight..."
 
 Note:
-    This script requires the llmflow package to be installed, as well as an OpenAI 
+    This script requires the llmflows package to be installed, as well as an OpenAI
     API key with access to the GPT-3 API.
 """
 
-from llmflow.llms.openai_chat import OpenAIChat
-from llmflow.prompts.prompt_template import PromptTemplate
+from llmflows.llms.openai_chat import OpenAIChat
+from llmflows.prompts.prompt_template import PromptTemplate
 
 title_llm = OpenAIChat(
     system_prompt="You are a useful AI that can come up with song titles"
 )
 writer_llm = OpenAIChat(
     system_prompt="You are a useful AI that can write song lyrics"
 )
```

### Comparing `llmflows-0.0.1/llmflow/examples/chaining_llms_4_1.py` & `llmflows-0.0.2/llmflows/examples/chaining_llms_4_1.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 Example:
     $ python chaining_llms_4_1.py
     "The Power of Friendship"
     "Verse 1: When I'm feeling down, you're always there to lift me up..."
     "Verse 1: When the darkness comes, I'll stand my ground and fight..."
 
 Note:
-    This script requires the llmflow package to be installed, as well as an OpenAI 
+    This script requires the llmflows package to be installed, as well as an OpenAI
     API key with access to the GPT-3 API.
 """
 
-from llmflow.llms.openai import OpenAI
-from llmflow.prompts.prompt_template import PromptTemplate
+from llmflows.llms.openai import OpenAI
+from llmflows.prompts.prompt_template import PromptTemplate
 
 title_llm = OpenAI()
 writer_llm = OpenAI()
 heavy_metal_llm = OpenAI()
 
 title_prompt_template = PromptTemplate(
     prompt="What is a good title of a song about {topic}"
```

### Comparing `llmflows-0.0.1/llmflow/examples/chat_llm_2_2.py` & `llmflows-0.0.2/llmflows/examples/chat_llm_2_2.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     You: I'm trying to install a Python package with pip, but it's not working.
     LLM: What error message are you getting?
     You: It says 'pip' is not recognized as an internal or external command.
     LLM: It sounds like pip is not in your system PATH. Have you tried adding it 
     to your PATH?
 
 Note:
-    This script requires the llmflow package to be installed, as well as an OpenAI 
+    This script requires the llmflows package to be installed, as well as an OpenAI
     API key with access to the GPT-3 API.
 """
 
-from llmflow.llms.openai_chat import OpenAIChat
+from llmflows.llms.openai_chat import OpenAIChat
 
 
 llm = OpenAIChat(system_prompt="You are a useful assistant")
 
 while True:
     user_message = input("You:")
     llm.add_message(user_message)
```

### Comparing `llmflows-0.0.1/llmflow/examples/chat_prompt_templates_3_2.py` & `llmflows-0.0.2/llmflows/examples/chat_prompt_templates_3_2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: skip-file
 
 """
-This script demonstrates how to use the llmflow package to create a chatbot using a 
+This script demonstrates how to use the llmflows package to create a chatbot using a
 prompt template.
 
 The script defines a prompt template with placeholders for a character and a name, and 
 uses the PromptTemplate class to generate a prompt with the character "clown" and the 
 name "Bob". It then initializes an OpenAIChatLLM object with the prompt, and enters a 
 loop where it prompts the user for input and generates a response using the 
 OpenAIChatLLM object.
@@ -13,20 +13,20 @@
 Example:
     $ python chat_prompt_templates_3_2.py
     You are a clown and you talk like a clown. Your name is Bob.
     You: Hi there!
     LLM: Hi Bob the clown! How can I help you today?
 
 Note:
-    This script requires the llmflow package to be installed, as well as an OpenAI API 
+    This script requires the llmflows package to be installed, as well as an OpenAI API
     key with access to the GPT-3 API.
 """
 
-from llmflow.llms.openai_chat import OpenAIChat
-from llmflow.prompts.prompt_template import PromptTemplate
+from llmflows.llms.openai_chat import OpenAIChat
+from llmflows.prompts.prompt_template import PromptTemplate
 
 
 prompt_template = PromptTemplate(
     prompt="You are a {character} and you talk like a {character}. Your name is {name}."
 )
 llm_prompt = prompt_template.get_prompt(character="clown", name="Bob")
```

### Comparing `llmflows-0.0.1/llmflow/examples/complex_async_flows_6_1.py` & `llmflows-0.0.2/llmflows/examples/complex_async_flows_6_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: skip-file
 
 """
-This script demonstrates how to use the llmflow package to create a complex data 
+This script demonstrates how to use the llmflows package to create a complex data
 processing pipeline using multiple flow steps.
 
 The script creates an OpenAI language model (LLM) and several prompt templates, and 
 uses them to define four flow steps: one for generating a movie title, one for 
 generating a song title for the movie, one for generating two main characters for 
 the movie, and one for generating lyrics for a song based on the movie title and 
 main characters. The script then connects the flow steps together to create a data 
@@ -18,22 +18,22 @@
         "song_title": "The Last Unicorn",
         "main_characters": "Amalthea and Schmendrick",
         "lyrics": "In a world of darkness and despair, two heroes rise to fight the 
             evil that threatens to destroy them..."
     }
 
 Note:
-    This script requires the llmflow package to be installed, as well as an OpenAI API 
+    This script requires the llmflows package to be installed, as well as an OpenAI API
     key with access to the GPT-3 API.
 """
 
-from llmflow.flows.async_flow import AsyncFlow
-from llmflow.flows.async_flowstep import AsyncFlowStep
-from llmflow.llms.openai import OpenAI
-from llmflow.prompts.prompt_template import PromptTemplate
+from llmflows.flows.async_flow import AsyncFlow
+from llmflows.flows.async_flowstep import AsyncFlowStep
+from llmflows.llms.openai import OpenAI
+from llmflows.prompts.prompt_template import PromptTemplate
 import asyncio
 
 # Create LLM
 open_ai_llm = OpenAI()
 
 # Create prompt templates
 title_template = PromptTemplate("What is a good title of a movie about {topic}?")
```

### Comparing `llmflows-0.0.1/llmflow/examples/complex_flows_6_1.py` & `llmflows-0.0.2/llmflows/examples/complex_flows_6_1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: skip-file
 
 """
-This script demonstrates how to use the llmflow package to create a complex data 
+This script demonstrates how to use the llmflows package to create a complex data
 processing pipeline using multiple flow steps.
 
 The script creates an OpenAI language model (LLM) and several prompt templates, and 
 uses them to define four flow steps: one for generating a movie title, one for 
 generating a song title for the movie, one for generating two main characters for 
 the movie, and one for generating lyrics for a song based on the movie title and 
 main characters. The script then connects the flow steps together to create a data 
@@ -18,22 +18,22 @@
         "song_title": "The Last Unicorn",
         "main_characters": "Amalthea and Schmendrick",
         "lyrics": "In a world of darkness and despair, two heroes rise to fight the 
             evil that threatens to destroy them..."
     }
 
 Note:
-    This script requires the llmflow package to be installed, as well as an OpenAI API 
+    This script requires the llmflows package to be installed, as well as an OpenAI API
     key with access to the GPT-3 API.
 """
 
-from llmflow.flows.flow import Flow
-from llmflow.flows.flowstep import FlowStep
-from llmflow.llms.openai import OpenAI
-from llmflow.prompts.prompt_template import PromptTemplate
+from llmflows.flows.flow import Flow
+from llmflows.flows.flowstep import FlowStep
+from llmflows.llms.openai import OpenAI
+from llmflows.prompts.prompt_template import PromptTemplate
 
 # Create LLM
 open_ai_llm = OpenAI()
 
 # Create prompt templates
 title_template = PromptTemplate("What is a good title of a movie about {topic}?")
 song_template = PromptTemplate(
@@ -79,8 +79,9 @@
 # Connect flowsteps
 flowstep1.connect(flowstep2, flowstep3, flowstep4)
 flowstep2.connect(flowstep4)
 flowstep3.connect(flowstep4)
 
 # Create and run Flow
 soundtrack_flow = Flow(flowstep1)
-soundtrack_flow.execute(topic="friendship", verbose=True)
+results = soundtrack_flow.execute(topic="friendship", verbose=True)
+print(results)
```

### Comparing `llmflows-0.0.1/llmflow/examples/creating_flows_5_1.py` & `llmflows-0.0.2/llmflows/examples/creating_flows_5_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: skip-file
 
 """
-This script demonstrates how to create a data processing pipeline using the llmflow 
+This script demonstrates how to create a data processing pipeline using the llmflows
 package.
 
 The script creates three OpenAI language models (LLMs) and three prompt templates, 
 and uses them to define three flow steps: one for generating a song title, one for 
 generating lyrics for that title, and one for generating a heavy metal paraphrase of 
 the lyrics. The script then connects the flow steps together to create a data 
 processing pipeline.
@@ -15,22 +15,22 @@
     {
         "song_title": "The Power of Friendship",
         "lyrics": "When I'm feeling down, you're always there to lift me up",
         "heavy_metal_lyrics": "When the darkness comes, I'll stand my ground and fight"
     }
 
 Note:
-    This script requires the llmflow package to be installed, as well as an OpenAI API 
+    This script requires the llmflows package to be installed, as well as an OpenAI API
     key with access to the GPT-3 API.
 """
 
-from llmflow.flows.flow import Flow
-from llmflow.flows.flowstep import FlowStep
-from llmflow.llms.openai import OpenAI
-from llmflow.prompts.prompt_template import PromptTemplate
+from llmflows.flows.flow import Flow
+from llmflows.flows.flowstep import FlowStep
+from llmflows.llms.openai import OpenAI
+from llmflows.prompts.prompt_template import PromptTemplate
 
 # Create LLMs
 title_llm = OpenAI()
 lyrics_llm = OpenAI()
 heavy_metal_llm = OpenAI()
 
 # Create prompt templates
@@ -68,8 +68,9 @@
 
 # Connect flowsteps
 title_flowstep.connect(lyrics_flowstep)
 lyrics_flowstep.connect(heavy_metal_flowstep)
 
 # Create and run Flow
 songwriting_flow = Flow(title_flowstep)
-songwriting_flow.execute(topic="love")  # provide initial data for the flow
+result = songwriting_flow.execute(topic="love")  # provide initial data for the flow
+print(result)
```

### Comparing `llmflows-0.0.1/llmflow/examples/getting_started_1_1.py` & `llmflows-0.0.2/llmflows/examples/getting_started_1_1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # pylint: skip-file
 
 """
-This script demonstrates how to use the llmflow package to generate prompts and format 
+This script demonstrates how to use the llmflows package to generate prompts and format
 them with user input.
 
 The script initializes an OpenAI language model (LLM) wrapper with a high temperature 
 setting, and uses it to generate a company name based on a prompt. The prompt includes 
 a placeholder for a product, which is filled in with the value "colorful socks" using 
 Python's string formatting syntax.
 
 Example:
     $ python getting_started_1_1.py
     "Rainbow Threads Inc."
 
 Note:
-    This script requires the llmflow package to be installed, as well as an OpenAI API 
+    This script requires the llmflows package to be installed, as well as an OpenAI API
     key with access to the GPT-3 API.
 """
 
 """
 The most basic building block of LangChain is calling an LLM on some input. Let’s walk 
 through a simple example of
 how to do this. For this purpose, let’s pretend we are building a service that 
 generates a company name based on what
 the company makes. In order to do this, we first need to import the LLM wrapper.
 """
 
-from llmflow.llms.openai import OpenAI
+from llmflows.llms.openai import OpenAI
 
 """
 We can then initialize the wrapper with any arguments. In this example, we probably 
 want the outputs to be MORE 
 random, so we’ll initialize it with a HIGH temperature.
 """
 
@@ -59,15 +59,15 @@
 company does, and then format the prompt with that information.
 
 This is easy to do with LangChain!
 
 First lets define the prompt template:
 """
 
-from llmflow.prompts.prompt_template import PromptTemplate
+from llmflows.prompts.prompt_template import PromptTemplate
 
 prompt_template = PromptTemplate(
     prompt="What is a good name for a company that makes {product}?"
 )
 
 """
 Let’s now see how this works! We can call the .get_prompt method to format it.
```

### Comparing `llmflows-0.0.1/llmflow/examples/getting_started_1_2.py` & `llmflows-0.0.2/llmflows/examples/getting_started_1_2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # pylint: skip-file
 
 """
-This script demonstrates how to use the llmflow package to generate prompts and format 
+This script demonstrates how to use the llmflows package to generate prompts and format
 them with user input.
 
 The script defines a prompt template with a placeholder for a product, and uses the 
 PromptTemplate class to generate a prompt with the product "colorful socks". It then 
 prints the formatted prompt to the console.
 
 Example:
     $ python getting_started_1_2.py
     What is a good name for a company that makes colorful socks?
 
 Note:
-    This script requires the llmflow package to be installed, as well as an OpenAI API 
+    This script requires the llmflows package to be installed, as well as an OpenAI API
     key with access to the GPT-3 API.
 """
 
 """
 The most basic building block of LangChain is calling an LLM on some input. Let’s walk 
 through a simple example of
 how to do this. For this purpose, let’s pretend we are building a service that 
 generates a company name based on what
 the company makes. In order to do this, we first need to import the LLM wrapper.
 """
 
-from llmflow.llms.openai_chat import OpenAIChat
+from llmflows.llms.openai_chat import OpenAIChat
 
 """
 We can then initialize the wrapper with any arguments. In this example, 
 we probably want the outputs to be MORE 
 random, so we’ll initialize it with a HIGH temperature.
 """
 
@@ -60,15 +60,15 @@
 company does, and then format the prompt with that information.
 
 This is easy to do with LangChain!
 
 First lets define the prompt template:
 """
 
-from llmflow.prompts.prompt_template import PromptTemplate
+from llmflows.prompts.prompt_template import PromptTemplate
 
 prompt_template = PromptTemplate(
     prompt="What is a good name for a company that makes {product}?"
 )
 
 """
 Let’s now see how this works! We can call the .get_prompt method to format it.
```

### Comparing `llmflows-0.0.1/llmflow/examples/llm_2_1.py` & `llmflows-0.0.2/llmflows/examples/llm_2_1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # pylint: skip-file
 
 """
-This script demonstrates how to use the OpenAI class from the llmflow package to 
+This script demonstrates how to use the OpenAI class from the llmflows package to
 generate text using the OpenAI GPT-3 language model.
 
 The script creates an instance of the OpenAI class, which provides a simple interface 
 for generating text using the OpenAI GPT-3 API. It then uses the generate method of 
 the OpenAI class to generate a cool title for an 80s rock song, and prints the result 
 to the console.
 
 Example:
     $ python llm_2_1.py
     "Rockin' the Night Away"
 
 Note:
-    This script requires the llmflow package to be installed, as well as an OpenAI API key with access to the GPT-3 API.
+    This script requires the llmflows package to be installed, as well as an OpenAI API key with access to the GPT-3 API.
 """
 
-from llmflow.llms.openai import OpenAI
+from llmflows.llms.openai import OpenAI
 
 
 llm = OpenAI()
 result = llm.generate(prompt="Generate a cool title an 80s rock song")
 print(result)
```

### Comparing `llmflows-0.0.1/llmflow/examples/prompt_templates_3_1.py` & `llmflows-0.0.2/llmflows/examples/prompt_templates_3_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 Example:
     $ python prompt_templates_3_1.py
     Generate a title for a 90s hip-hop song about friendship.
     "Friends 'til the End" 
 
 Note:
-    This script requires the llmflow package to be installed, as well as an OpenAI API key with access to the GPT-3 API.
+    This script requires the llmflows package to be installed, as well as an OpenAI API key with access to the GPT-3 API.
 """
 
-from llmflow.llms.openai import OpenAI
-from llmflow.prompts.prompt_template import PromptTemplate
+from llmflows.llms.openai import OpenAI
+from llmflows.prompts.prompt_template import PromptTemplate
 
 
 prompt_template = PromptTemplate(
     prompt="Generate a title for a 90s hip-hop song about {topic}."
 )
 llm_prompt = prompt_template.get_prompt(topic="friendship")
```

### Comparing `llmflows-0.0.1/llmflow/examples/question_answering.py` & `llmflows-0.0.2/llmflows/examples/question_answering.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 Example:
     $ python question_answering.py
     Q: How was dark energy discovered?
     A: Dark energy was discovered in 1998 by two teams of astronomers studying 
     supernovae.
 
 Note:
-    This script requires the llmflow and pinecone packages to be installed, as well as 
+    This script requires the llmflows and pinecone packages to be installed, as well as
     an OpenAI API key with access to the GPT-3 API and a Pinecone API key.
 """
 
-from llmflow.llms.openai_embeddings import OpenAIEmbeddings
-from llmflow.llms.openai import OpenAI
-from llmflow.prompts.prompt_template import PromptTemplate
-from llmflow.vectorstores.vector_doc import VectorDoc
-from llmflow.vectorstores.pinecone import Pinecone
+from llmflows.llms.openai_embeddings import OpenAIEmbeddings
+from llmflows.llms.openai import OpenAI
+from llmflows.prompts.prompt_template import PromptTemplate
+from llmflows.vectorstores.vector_doc import VectorDoc
+from llmflows.vectorstores.pinecone import Pinecone
 import os
 
 """
 Before starting this tutorial go and create an index in Pinecone with dimension of 1536 
 (the default dimension or openai's embeddings)
 """
 PINECONE_API_KEY = os.environ.get("PINECONE_API_KEY", "<YOUR-API-KEY>")
@@ -102,15 +102,15 @@
 
 # Convert text docs to VectorDocs and get embeddings
 vector_docs = [VectorDoc(doc=doc) for doc in docs]
 embedded_docs = embeddings_llm.embed(vector_docs)
 
 # initialize Pinecone
 vector_db = Pinecone(
-    index_name="llmflow-tutorial",
+    index_name="llmflows-tutorial",
     api_key=PINECONE_API_KEY,
     environment="us-west4-gcp-free",
 )
 
 # Add the embedded documents to the vector database
 # vector_db.upsert(docs=embedded_docs)
```

### Comparing `llmflows-0.0.1/llmflow/flows/async_flow.py` & `llmflows-0.0.2/llmflows/flows/async_flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=R0801
 
 """
 Async implementations of flow classes defined in another module.
 """
 
 import asyncio
-from llmflow.flows.async_flowstep import AsyncFlowStep
+from llmflows.flows.async_flowstep import AsyncFlowStep
 
 
 class AsyncBaseFlow:
     """Base class for all async flows."""
 
     def __init__(self, first_step: AsyncFlowStep):
         """
@@ -49,14 +49,16 @@
         """
         Initializes the AsyncFlow.
 
         Args:
             first_step (AsyncFlowStep): The first step of the flow.
         """
         super().__init__(first_step)
+        self.results = []
+        self._results_lock = asyncio.Lock()
         self.executed_steps = set()
         self._check_unique_output_keys()
 
     def _check_unique_output_keys(self):
         """
         Ensures unique output keys among steps.
 
@@ -88,14 +90,15 @@
         Executes the flow.
 
         Args:
             verbose (bool): If true, flowstep outputs are printed.
             **inputs (str): Inputs to the flow.
         """
         await self._execute_step(self.first_step, inputs, verbose)
+        return self.results
 
     async def _execute_step(self, step: AsyncFlowStep, inputs: dict, verbose: bool):
         """
         Concurrently executes a step and all subsequent steps.
 
         Args:
             step (AsyncFlowStep): The step to execute.
@@ -108,14 +111,20 @@
         required_inputs = {key: inputs[key] for key in step.prompt_template.variables}
 
         if step not in self.executed_steps:
             new_inputs = await step.execute(required_inputs, verbose)
             self.executed_steps.add(step)
 
             if new_inputs:
+                async with self._results_lock:
+                    self.results.append({
+                        'step': step.name,
+                        'output_key': step.output_key,
+                        'output_value': new_inputs[step.output_key]
+                    })
                 inputs.update(new_inputs)
 
         if step.next_steps:
             await asyncio.gather(
                 *[self._execute_step(next_step, inputs, verbose)
                   for next_step in step.next_steps]
             )
```

### Comparing `llmflows-0.0.1/llmflow/flows/async_flowstep.py` & `llmflows-0.0.2/llmflows/flows/async_flowstep.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# pylint: disable=R0801
+# pylint: disable=R0801, R0913
 
 """
 This module provides async flow step classes: AsyncBaseFlowStep and AsyncFlowStep.
 These steps form the fundamental units in an AsyncFlow, allowing async processing.
 """
 
-from typing import List, Dict, Any
+from typing import List, Dict, Any, Callable
 
 
 class AsyncBaseFlowStep:
     """Base class for all asynchronous flow steps."""
 
     def __init__(self, name: str, output_key: str):
         """
@@ -65,41 +65,55 @@
         if len(output_keys) != len(set(output_keys)):
             raise ValueError("All connected flowsteps must have unique output keys.")
 
 
 class AsyncFlowStep(AsyncBaseFlowStep):
     """A specific implementation of asynchronous flow step."""
 
-    def __init__(self, name: str, llm: Any, prompt_template: Any, output_key: str):
+    def __init__(
+        self,
+        name: str,
+        llm: Any,
+        prompt_template: Any,
+        output_key: str,
+        callbacks: List[Callable] = None,
+    ):
         """
         Initializes the AsyncFlowStep.
 
         Args:
             name (str): The name of the flow step.
             llm (Any): The language model used for generation.
             prompt_template (Any): Template for generating the prompt.
             output_key (str): The unique output key of the flow step.
         """
         super().__init__(name, output_key)
         self.llm = llm
         self.prompt_template = prompt_template
+        self.callbacks = callbacks if callbacks else []
 
     async def execute(
         self, inputs: Dict[str, Any], verbose: bool = False
     ) -> Dict[str, Any]:
         """
         Executes the flow step asynchronously.
 
         Args:
             inputs (Dict[str, Any]): Inputs to the step.
             verbose (bool): If true, step output is printed.
 
         Returns:
             Dict[str, Any]: Output of the step, with output_key as the key.
         """
+        print(f"Flowstep {self.name} started")
         prompt = self.prompt_template.get_prompt(**inputs)
         result = await self.llm.generate_async(prompt)
 
+        for callback in self.callbacks:
+            if verbose:
+                print(f"{self.name} Executing Callback: {callback.__name__}")
+            callback(result)
+
         if verbose:
             print(f"{self.name}:\n{result}\n")
 
         return {self.output_key: result}
```

### Comparing `llmflows-0.0.1/llmflow/flows/flow.py` & `llmflows-0.0.2/llmflows/flows/flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pylint: disable=R0801
 
 """
 This module provides implementations of BaseFlow and Flow.
 """
 
-from llmflow.flows.flowstep import FlowStep
+from llmflows.flows.flowstep import FlowStep
 
 
 class BaseFlow:
     """
     Base class for all flows. Each specific flow should extend this class.
     """
 
@@ -56,14 +56,15 @@
 
     Raises:
         ValueError: If flow steps have same output key.
     """
 
     def __init__(self, first_step: FlowStep):
         super().__init__(first_step)
+        self.results = []
         self.executed_steps = set()
         self._check_unique_output_keys()
 
     def _check_unique_output_keys(self):
         """
         Checks that all flow steps have unique output keys.
 
@@ -98,14 +99,15 @@
             verbose: Specifies if the flowstep should print their output
             **inputs: The inputs to the flow.
 
         Raises:
             ValueError: If any required inputs are missing.
         """
         self._execute_step(self.first_step, inputs, verbose)
+        return self.results
 
     def _execute_step(self, step, inputs, verbose):
         """
         DFS-like execution of the given step with the given inputs.
 
         Args:
             step (FlowStep): The step to execute.
@@ -121,11 +123,16 @@
 
         # If step has not been executed yet, execute it.
         if step not in self.executed_steps:
             new_inputs = step.execute(required_inputs, verbose)
             self.executed_steps.add(step)
 
             if new_inputs:
+                self.results.append({
+                    'step': step.name,
+                    'output_key': step.output_key,
+                    'output_value': new_inputs[step.output_key]
+                })
                 inputs.update(new_inputs)
 
         for next_step in step.next_steps:
             self._execute_step(next_step, inputs, verbose)
```

### Comparing `llmflows-0.0.1/llmflow/flows/flowstep.py` & `llmflows-0.0.2/llmflows/flows/flowstep.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# pylint: disable=R0801
+# pylint: disable=R0801, R0913
 
 """
 This module contains the BaseFlowStep class which serves as a base class for
 flow steps in a data processing pipeline.
 
 This module defines the FlowStep class which is an implementation of a step 
 in a data processing pipeline, based on the BaseFlowStep class.
 """
 
-from typing import Dict, Any, List
+from typing import Dict, Any, List, Callable
 
 
 class BaseFlowStep:
     """
     Base class for flow steps in a data processing pipeline.
 
     Attributes:
@@ -64,34 +64,40 @@
             *steps (BaseFlowStep): Flow steps to connect to.
 
         Raises:
             ValueError: If connected flow steps have same output key.
         """
         output_keys = [step.output_key for step in steps]
         if len(output_keys) != len(set(output_keys)):
-            raise ValueError(
-                "All connected flowsteps must have unique output keys."
-            )
+            raise ValueError("All connected flowsteps must have unique output keys.")
 
 
 class FlowStep(BaseFlowStep):
     """
     Represents a specific step in a Flow.
 
     Attributes:
         name (str): The name of the flow step.
         output_key (str): The key for the output of the flow step.
         llm: Language model to be used in the flow step.
         prompt_template: Template for the prompt to be used with the language model.
     """
 
-    def __init__(self, name: str, llm: Any, prompt_template: Any, output_key: str):
+    def __init__(
+        self,
+        name: str,
+        llm: Any,
+        prompt_template: Any,
+        output_key: str,
+        callbacks: List[Callable] = None,
+    ):
         super().__init__(name, output_key)
         self.llm = llm
         self.prompt_template = prompt_template
+        self.callbacks = callbacks if callbacks is not None else []
 
     def execute(self, inputs: Dict[str, Any], verbose: bool = False) -> Dict[str, Any]:
         """
         Executes the flow step with provided inputs.
 
         Args:
             verbose: bool: Specifies if the flowstep should print its output
@@ -99,11 +105,16 @@
 
         Returns:
             Dict[str, Any]: Dictionary with the output key and the result.
         """
         prompt = self.prompt_template.get_prompt(**inputs)
         result = self.llm.generate(prompt)
 
+        for callback in self.callbacks:
+            if verbose:
+                print(f"{self.name} Executing Callback: {callback.__name__}")
+            callback(result)
+
         if verbose:
-            print(f'{self.name}:\n{result}\n')
+            print(f"{self.name}:\n{result}\n")
 
         return {self.output_key: result}
```

### Comparing `llmflows-0.0.1/llmflow/llms/openai.py` & `llmflows-0.0.2/llmflows/llms/openai.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.1/llmflow/llms/openai_chat.py` & `llmflows-0.0.2/llmflows/llms/openai_chat.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.1/llmflow/llms/openai_embeddings.py` & `llmflows-0.0.2/llmflows/llms/openai_embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 This module helps with creating embeddings form OpenAIs API.
 """
 
 import os
 from typing import Union, List
 import openai
-from llmflow.vectorstores.vector_doc import VectorDoc
+from llmflows.vectorstores.vector_doc import VectorDoc
 from .llm import BaseLLM
 
 
 
 class OpenAIEmbeddings(BaseLLM):
     """
     A class for interacting with the OpenAI embeddings API.
```

### Comparing `llmflows-0.0.1/llmflow/prompts/prompt_template.py` & `llmflows-0.0.2/llmflows/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.1/llmflow/vectorstores/pinecone.py` & `llmflows-0.0.2/llmflows/vectorstores/pinecone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module to interact with Pinecone, a vector database service.
 
 This module contains a class `Pinecone` which provides several methods to
 interact with the Pinecone vector database service.
 """
 
 import pinecone # pylint: disable=import-error
-from llmflow.vectorstores.vector_doc import VectorDoc
+from llmflows.vectorstores.vector_doc import VectorDoc
 
 
 class Pinecone:
     """Interact with Pinecone, a vector database service.
 
     This class has methods to initialize the Pinecone client, describe the index,
     search the index for similar vectors, and insert or update vectors in the index.
```

### Comparing `llmflows-0.0.1/llmflow/vectorstores/vector_doc.py` & `llmflows-0.0.2/llmflows/vectorstores/vector_doc.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.1/llmflows.egg-info/PKG-INFO` & `llmflows-0.0.2/llmflows.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflows
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple and lightweight library for creating LLM-powered applications.
 Author: Stoyan Stoyanov
 Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflow
 Project-URL: github, https://github.com/stoyan-stoyanov/llmflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,65 +12,65 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <img src="docs/logo.png" />
 </p>
 
-[![Twitter](https://img.shields.io/twitter/follow/LLMFlow?style=social)](https://twitter.com/LLMFlow)
+[![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
 
 ## Installation
 ```
-pip install llmflow
+pip install llmflows
 ```
 
-## What is LLMFlow?
+## What is LLMFlowss?
 A simple and lightweitght library for creating LLM-powered applications.
 
 ## Philosophy
 
 ### Simple
-We have created LLMFlow with simplicity in mind while balancing for usability. We have a minimal set of classes that allow users to build powerful LLM-powered apps without compromising on capabilities.
+We have created LLMFlows with simplicity in mind while balancing for usability. We have a minimal set of classes that allow users to build powerful LLM-powered apps without compromising on capabilities.
 
 ### Explicit
 We allow users to easily create complex LLM flows but we don't 
 
 ### Transparent
 We don't have classes with hidden prompts - prompts are for you to decide.
 
 ## Example
 Here is a basic example for creating an LLM with PromptTemplate:
-```python
 
-from llmflow.llms.openai import OpenAI
-from llmflow.prompts.prompt_template import PromptTemplate
+```python
 
+from llmflows.llms.openai import OpenAI
+from llmflows.prompts.prompt_template import PromptTemplate
 
 prompt_template = PromptTemplate(
-    prompt="Generate a title for a 90s hip-hop song about {topic}."
+   prompt="Generate a title for a 90s hip-hop song about {topic}."
 )
 llm_prompt = prompt_template.get_prompt(topic="friendship")
 
 print(llm_prompt)
 
 llm = OpenAI()
 song_title = llm.generate(llm_prompt)
 print(song_title)
 
 ```
 
-While this is a good example on how easy it is to use LLMFlow, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
+While this is a good example on how easy it is to use LLMFlows, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
 ![Complex flow](docs/complex_flow.png)
-With LLMFlow it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlow will figure out the dependencies for you and make sure each flowstep is executed only when the flowsteps it depends on are complete:
+With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies for you and make sure each flowstep is executed only when the flowsteps it depends on are complete:
 
 ```python
-from llmflow.flows.flow import Flow
-from llmflow.flows.flowstep import FlowStep
-from llmflow.llms.openai import OpenAI
-from llmflow.prompts.prompt_template import PromptTemplate
+from llmflows.flows.flow import Flow
+from llmflows.flows.flowstep import FlowStep
+from llmflows.llms.openai import OpenAI
+from llmflows.prompts.prompt_template import PromptTemplate
 
 # Create LLM
 open_ai_llm = OpenAI()
 
 # Create prompt templates
 title_template = PromptTemplate("What is a good title of a movie about {topic}?")
 song_template = PromptTemplate(
@@ -119,15 +119,15 @@
 flowstep3.connect(flowstep4)
 
 # Create and run Flow
 soundtrack_flow = Flow(flowstep1)
 soundtrack_flow.execute(topic="friendship")
 
 ```
-In fact, LLMFlow provides async, and threaded classes so any complex DAG can be executed in parallel.
+In fact, LLMFlows provides async, and threaded classes so any complex DAG can be executed in parallel.
 For more examples such as how to create Q&A apps and web applications with Flask and FastAPI check our documentation.
 
 ## Usage patterns 
 1. Use LLMs-only
 
     Use the LLM and Agents classes and tools to build free-roaming agents   
 
@@ -138,15 +138,15 @@
 3. Build web apps
 
     Execute agents inside flowsteps where you can build conversational experiences with different stages and requirements
 
 ## FAQ
 
 ### How is this different than langchian?
-Langchain is an amazing library and LLMFlow has been certainly been inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and while this is great for beginners and people who are not in the field of machine learning and language models, this can be a bit overwhelming. There are a lot of classes, hidden prompts in chains and many ways to do things. In contrast we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
+Langchain is an amazing library and LLMFlows has been certainly been inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and while this is great for beginners and people who are not in the field of machine learning and language models, this can be a bit overwhelming. There are a lot of classes, hidden prompts in chains and many ways to do things. In contrast we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
 
 ### You only have OpenAI wrappers but I want to use ACMELLM
 We decided to release the library initially supporting only OpenAI LLMs but we have a roadmap and we will slowly add new wrappers around the most popular models. If you are willing to spend some time we are looking for contributors and maintainers
 
 ### You only support Pinecone and Redis vector DBs do you have plans to extend the list?
 Yes! We will also add Redis, Elastic Search and other popular solutions over time. If you want to help us out check out our contribution section.
```

### Comparing `llmflows-0.0.1/llmflows.egg-info/SOURCES.txt` & `llmflows-0.0.2/llmflows.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 LICENSE
 README.md
 pyproject.toml
-llmflow/__init__.py
-llmflow/examples/__init__.py
-llmflow/examples/chaining_chat_llms_4_2.py
-llmflow/examples/chaining_llms_4_1.py
-llmflow/examples/chat_llm_2_2.py
-llmflow/examples/chat_prompt_templates_3_2.py
-llmflow/examples/complex_async_flows_6_1.py
-llmflow/examples/complex_flows_6_1.py
-llmflow/examples/creating_flows_5_1.py
-llmflow/examples/getting_started_1_1.py
-llmflow/examples/getting_started_1_2.py
-llmflow/examples/llm_2_1.py
-llmflow/examples/prompt_templates_3_1.py
-llmflow/examples/question_answering.py
-llmflow/flows/__init__.py
-llmflow/flows/async_flow.py
-llmflow/flows/async_flowstep.py
-llmflow/flows/flow.py
-llmflow/flows/flowstep.py
-llmflow/flows/threaded_flow.py
-llmflow/flows/threaded_flowstep.py
-llmflow/llms/__init__.py
-llmflow/llms/llm.py
-llmflow/llms/openai.py
-llmflow/llms/openai_chat.py
-llmflow/llms/openai_embeddings.py
-llmflow/prompts/__init__.py
-llmflow/prompts/prompt_template.py
-llmflow/vectorstores/__init__.py
-llmflow/vectorstores/pinecone.py
-llmflow/vectorstores/vector_doc.py
+llmflows/__init__.py
 llmflows.egg-info/PKG-INFO
 llmflows.egg-info/SOURCES.txt
 llmflows.egg-info/dependency_links.txt
 llmflows.egg-info/requires.txt
-llmflows.egg-info/top_level.txt
+llmflows.egg-info/top_level.txt
+llmflows/examples/__init__.py
+llmflows/examples/chaining_chat_llms_4_2.py
+llmflows/examples/chaining_llms_4_1.py
+llmflows/examples/chat_llm_2_2.py
+llmflows/examples/chat_prompt_templates_3_2.py
+llmflows/examples/complex_async_flows_6_1.py
+llmflows/examples/complex_flows_6_1.py
+llmflows/examples/creating_flows_5_1.py
+llmflows/examples/getting_started_1_1.py
+llmflows/examples/getting_started_1_2.py
+llmflows/examples/llm_2_1.py
+llmflows/examples/prompt_templates_3_1.py
+llmflows/examples/question_answering.py
+llmflows/flows/__init__.py
+llmflows/flows/async_flow.py
+llmflows/flows/async_flowstep.py
+llmflows/flows/flow.py
+llmflows/flows/flowstep.py
+llmflows/flows/threaded_flow.py
+llmflows/flows/threaded_flowstep.py
+llmflows/llms/__init__.py
+llmflows/llms/llm.py
+llmflows/llms/openai.py
+llmflows/llms/openai_chat.py
+llmflows/llms/openai_embeddings.py
+llmflows/prompts/__init__.py
+llmflows/prompts/prompt_template.py
+llmflows/vectorstores/__init__.py
+llmflows/vectorstores/pinecone.py
+llmflows/vectorstores/vector_doc.py
```

### Comparing `llmflows-0.0.1/pyproject.toml` & `llmflows-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llmflows"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Stoyan Stoyanov"},
 ]
 description = "A simple and lightweight library for creating LLM-powered applications."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

