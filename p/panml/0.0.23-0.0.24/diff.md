# Comparing `tmp/panml-0.0.23.tar.gz` & `tmp/panml-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.23.tar", last modified: Thu Jun  1 22:37:31 2023, max compression
+gzip compressed data, was "panml-0.0.24.tar", last modified: Sun Jun  4 01:50:25 2023, max compression
```

## Comparing `panml-0.0.23.tar` & `panml-0.0.24.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.378286 panml-0.0.23/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.23/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)    14824 2023-06-01 22:37:31.378644 panml-0.0.23/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)    13645 2023-06-01 11:12:21.000000 panml-0.0.23/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.370960 panml-0.0.23/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.23/panml/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     3617 2023-06-01 11:12:21.000000 panml-0.0.23/panml/constants.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.372947 panml-0.0.23/panml/core/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.23/panml/core/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.373594 panml-0.0.23/panml/core/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.23/panml/core/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.23/panml/core/clustering/faiss.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.375263 panml-0.0.23/panml/core/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.23/panml/core/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    20353 2023-06-01 22:37:04.000000 panml-0.0.23/panml/core/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    13741 2023-06-01 22:37:04.000000 panml-0.0.23/panml/core/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     3085 2023-05-28 12:46:27.000000 panml-0.0.23/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2608 2023-05-28 12:46:27.000000 panml-0.0.23/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.372627 panml-0.0.23/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)    14824 2023-06-01 22:37:31.000000 panml-0.0.23/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      468 2023-06-01 22:37:31.000000 panml-0.0.23/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-01 22:37:31.000000 panml-0.0.23/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-06-01 22:37:31.000000 panml-0.0.23/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-01 22:37:31.000000 panml-0.0.23/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-01 22:37:31.379730 panml-0.0.23/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2384 2023-06-01 22:37:04.000000 panml-0.0.23/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-01 22:37:31.377142 panml-0.0.23/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-05-25 13:23:02.000000 panml-0.0.23/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-0.0.23/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.647239 panml-0.0.24/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.24/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14672 2023-06-04 01:50:25.647704 panml-0.0.24/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13493 2023-06-04 01:49:06.000000 panml-0.0.24/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.634129 panml-0.0.24/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.24/panml/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3617 2023-06-01 11:12:21.000000 panml-0.0.24/panml/constants.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.639180 panml-0.0.24/panml/core/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.24/panml/core/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.640376 panml-0.0.24/panml/core/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.24/panml/core/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.24/panml/core/clustering/faiss.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.643984 panml-0.0.24/panml/core/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.24/panml/core/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    20353 2023-06-01 22:37:04.000000 panml-0.0.24/panml/core/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13741 2023-06-01 22:37:04.000000 panml-0.0.24/panml/core/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3085 2023-05-28 12:46:27.000000 panml-0.0.24/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2608 2023-05-28 12:46:27.000000 panml-0.0.24/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.638504 panml-0.0.24/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14672 2023-06-04 01:50:25.000000 panml-0.0.24/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      468 2023-06-04 01:50:25.000000 panml-0.0.24/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-04 01:50:25.000000 panml-0.0.24/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-06-04 01:50:25.000000 panml-0.0.24/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-04 01:50:25.000000 panml-0.0.24/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-04 01:50:25.649281 panml-0.0.24/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2384 2023-06-04 01:49:06.000000 panml-0.0.24/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.646038 panml-0.0.24/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-05-25 13:23:02.000000 panml-0.0.24/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-0.0.24/test/test_VectorEngine.py
```

### Comparing `panml-0.0.23/LICENSE` & `panml-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-0.0.23/PKG-INFO` & `panml-0.0.24/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.23
+Version: 0.0.24
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
@@ -25,19 +25,19 @@
 License-File: LICENSE
 
 ## PanML: A high level generative AI/ML development and analysis library
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 [![](https://dcbadge.vercel.app/api/server/cCsaqv9KFf?compact=true&style=flat)](https://discord.gg/cCsaqv9KFf)
 
-## Goal
-This package aims to make analysis and experimentation of generative AI/ML models broadly accessible, by providing a simple and consistent interface to foundation models, and abstract methods to support some of the common use-cases. This includes using smaller, less compute heavy Open Source language models to support the various NLP-based Data Science workflows in the industry. Additionally, we want to empower Data Science projects with the tools to easily productionise custom-built generative models.
-
-
-We are passionate about AI technology and AI safety, and this supports our contribution towards a beneficial outcome in an AI-powered world. Please note this is a work in progress, so very much open for collaboration and contribution. 
+A library with simple to use abstractions when working with LLMs inspired by the sckit-learn style API. <br>
+🔍 Easily explore and experiment with commercial and open source LLMs, including ones that can be run on your local machine. <br>
+⚡ Easily integrate language models of different sizes, including smaller, less compute heavy but still very useful LLMs in NLP-based Data Science contexts. <br>
+🚀 Support the development of LLM workflows with off-the-shelf or custom-built generative models. <br><br>
+Please note this is a work in progress, and it's open for collabration and contribution.
 
 ### What this library covers
 - [Inference and analysis of LLM](https://github.com/Pan-ML/panml/wiki/5.-Generative-model-analysis)
 - [Prompt chain engineering a LLM](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering)
 - [Fine tuning of LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM)
 - [Document question answering using LLM](https://github.com/Pan-ML/panml/wiki/7.-Retrieve-similar-documents-using-vector-search)
 - [Variable integrated code generation using LLM](https://github.com/Pan-ML/panml/wiki/4.-Prompted-code-generation)
@@ -46,29 +46,14 @@
 - [HuggingFace Hub](https://huggingface.co) - open source LLMs from Google, EleutherAI, Cerebras, StabilityAI, H2O, Salesforce, and others
 - [OpenAI](https://openai.com) - text-davinci-002/003, GPT3/3.5
 
 See model options in [library supported models](https://github.com/Pan-ML/panml/wiki/8.-Supported-models)
 
 For performance overview of open source LLMs (including models not currently covered in this library), you can find the information on the [HuggingFace Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard).
 
-### Roadmap
-
-Model development and analysis
-- Support for additional open source and commercial language model
-- Model evaluation methods (including adversarial evaluation)
-- Prompt engineering support and analysis (adding further methods and adding support for more LLMs)
-- Parameter-efficient fine tuning (e.g. LoRA, prompt tuning etc)
-- Model intepretability methods
-- Model emergent effect simulation and analysis (related to long term AI safety risks)
-
-Model productionisation
-- Automated refactoring of experimental code into source code
-- Automated API wrapper generation
-- Automated dockerization
-
 ### Support
 
 You can support us by contributing to this project, as well as providing feedback and ideas in the [issues](https://github.com/Pan-ML/panml/issues) section. 
 
 We would also appreciate if you can give panml a ⭐ on GitHub, and if it adds value to you, sharing this with others in your network on LinkedIn/Twitter/Medium etc who would also find this useful.
 
 
@@ -330,8 +315,23 @@
 ```
 
 ### Running tests
 ```
 python3 -m unittest
 ```
 
+### Roadmap
+
+Model development and analysis
+- Support for additional open source and commercial language model
+- Model evaluation methods (including adversarial evaluation)
+- Prompt engineering support and analysis (adding further methods and adding support for more LLMs)
+- Parameter-efficient fine tuning (e.g. LoRA, prompt tuning etc)
+- Model intepretability methods
+- Model emergent effect simulation and analysis (related to long term AI safety risks)
+
+Model productionisation
+- Automated refactoring of experimental code into source code
+- Automated API wrapper generation
+- Automated dockerization
+
```

### Comparing `panml-0.0.23/README.md` & `panml-0.0.24/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ## PanML: A high level generative AI/ML development and analysis library
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 [![](https://dcbadge.vercel.app/api/server/cCsaqv9KFf?compact=true&style=flat)](https://discord.gg/cCsaqv9KFf)
 
-## Goal
-This package aims to make analysis and experimentation of generative AI/ML models broadly accessible, by providing a simple and consistent interface to foundation models, and abstract methods to support some of the common use-cases. This includes using smaller, less compute heavy Open Source language models to support the various NLP-based Data Science workflows in the industry. Additionally, we want to empower Data Science projects with the tools to easily productionise custom-built generative models.
-
-
-We are passionate about AI technology and AI safety, and this supports our contribution towards a beneficial outcome in an AI-powered world. Please note this is a work in progress, so very much open for collaboration and contribution. 
+A library with simple to use abstractions when working with LLMs inspired by the sckit-learn style API. <br>
+🔍 Easily explore and experiment with commercial and open source LLMs, including ones that can be run on your local machine. <br>
+⚡ Easily integrate language models of different sizes, including smaller, less compute heavy but still very useful LLMs in NLP-based Data Science contexts. <br>
+🚀 Support the development of LLM workflows with off-the-shelf or custom-built generative models. <br><br>
+Please note this is a work in progress, and it's open for collabration and contribution.
 
 ### What this library covers
 - [Inference and analysis of LLM](https://github.com/Pan-ML/panml/wiki/5.-Generative-model-analysis)
 - [Prompt chain engineering a LLM](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering)
 - [Fine tuning of LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM)
 - [Document question answering using LLM](https://github.com/Pan-ML/panml/wiki/7.-Retrieve-similar-documents-using-vector-search)
 - [Variable integrated code generation using LLM](https://github.com/Pan-ML/panml/wiki/4.-Prompted-code-generation)
@@ -20,29 +20,14 @@
 - [HuggingFace Hub](https://huggingface.co) - open source LLMs from Google, EleutherAI, Cerebras, StabilityAI, H2O, Salesforce, and others
 - [OpenAI](https://openai.com) - text-davinci-002/003, GPT3/3.5
 
 See model options in [library supported models](https://github.com/Pan-ML/panml/wiki/8.-Supported-models)
 
 For performance overview of open source LLMs (including models not currently covered in this library), you can find the information on the [HuggingFace Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard).
 
-### Roadmap
-
-Model development and analysis
-- Support for additional open source and commercial language model
-- Model evaluation methods (including adversarial evaluation)
-- Prompt engineering support and analysis (adding further methods and adding support for more LLMs)
-- Parameter-efficient fine tuning (e.g. LoRA, prompt tuning etc)
-- Model intepretability methods
-- Model emergent effect simulation and analysis (related to long term AI safety risks)
-
-Model productionisation
-- Automated refactoring of experimental code into source code
-- Automated API wrapper generation
-- Automated dockerization
-
 ### Support
 
 You can support us by contributing to this project, as well as providing feedback and ideas in the [issues](https://github.com/Pan-ML/panml/issues) section. 
 
 We would also appreciate if you can give panml a ⭐ on GitHub, and if it adds value to you, sharing this with others in your network on LinkedIn/Twitter/Medium etc who would also find this useful.
 
 
@@ -303,7 +288,22 @@
 pip install -r requirements.txt
 ```
 
 ### Running tests
 ```
 python3 -m unittest
 ```
+
+### Roadmap
+
+Model development and analysis
+- Support for additional open source and commercial language model
+- Model evaluation methods (including adversarial evaluation)
+- Prompt engineering support and analysis (adding further methods and adding support for more LLMs)
+- Parameter-efficient fine tuning (e.g. LoRA, prompt tuning etc)
+- Model intepretability methods
+- Model emergent effect simulation and analysis (related to long term AI safety risks)
+
+Model productionisation
+- Automated refactoring of experimental code into source code
+- Automated API wrapper generation
+- Automated dockerization
```

### Comparing `panml-0.0.23/panml/constants.py` & `panml-0.0.24/panml/constants.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.23/panml/core/clustering/faiss.py` & `panml-0.0.24/panml/core/clustering/faiss.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.23/panml/core/llm/huggingface.py` & `panml-0.0.24/panml/core/llm/huggingface.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.23/panml/core/llm/openai.py` & `panml-0.0.24/panml/core/llm/openai.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.23/panml/models.py` & `panml-0.0.24/panml/models.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.23/panml/search.py` & `panml-0.0.24/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.23/panml.egg-info/PKG-INFO` & `panml-0.0.24/panml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.23
+Version: 0.0.24
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
@@ -25,19 +25,19 @@
 License-File: LICENSE
 
 ## PanML: A high level generative AI/ML development and analysis library
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 [![](https://dcbadge.vercel.app/api/server/cCsaqv9KFf?compact=true&style=flat)](https://discord.gg/cCsaqv9KFf)
 
-## Goal
-This package aims to make analysis and experimentation of generative AI/ML models broadly accessible, by providing a simple and consistent interface to foundation models, and abstract methods to support some of the common use-cases. This includes using smaller, less compute heavy Open Source language models to support the various NLP-based Data Science workflows in the industry. Additionally, we want to empower Data Science projects with the tools to easily productionise custom-built generative models.
-
-
-We are passionate about AI technology and AI safety, and this supports our contribution towards a beneficial outcome in an AI-powered world. Please note this is a work in progress, so very much open for collaboration and contribution. 
+A library with simple to use abstractions when working with LLMs inspired by the sckit-learn style API. <br>
+🔍 Easily explore and experiment with commercial and open source LLMs, including ones that can be run on your local machine. <br>
+⚡ Easily integrate language models of different sizes, including smaller, less compute heavy but still very useful LLMs in NLP-based Data Science contexts. <br>
+🚀 Support the development of LLM workflows with off-the-shelf or custom-built generative models. <br><br>
+Please note this is a work in progress, and it's open for collabration and contribution.
 
 ### What this library covers
 - [Inference and analysis of LLM](https://github.com/Pan-ML/panml/wiki/5.-Generative-model-analysis)
 - [Prompt chain engineering a LLM](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering)
 - [Fine tuning of LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM)
 - [Document question answering using LLM](https://github.com/Pan-ML/panml/wiki/7.-Retrieve-similar-documents-using-vector-search)
 - [Variable integrated code generation using LLM](https://github.com/Pan-ML/panml/wiki/4.-Prompted-code-generation)
@@ -46,29 +46,14 @@
 - [HuggingFace Hub](https://huggingface.co) - open source LLMs from Google, EleutherAI, Cerebras, StabilityAI, H2O, Salesforce, and others
 - [OpenAI](https://openai.com) - text-davinci-002/003, GPT3/3.5
 
 See model options in [library supported models](https://github.com/Pan-ML/panml/wiki/8.-Supported-models)
 
 For performance overview of open source LLMs (including models not currently covered in this library), you can find the information on the [HuggingFace Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard).
 
-### Roadmap
-
-Model development and analysis
-- Support for additional open source and commercial language model
-- Model evaluation methods (including adversarial evaluation)
-- Prompt engineering support and analysis (adding further methods and adding support for more LLMs)
-- Parameter-efficient fine tuning (e.g. LoRA, prompt tuning etc)
-- Model intepretability methods
-- Model emergent effect simulation and analysis (related to long term AI safety risks)
-
-Model productionisation
-- Automated refactoring of experimental code into source code
-- Automated API wrapper generation
-- Automated dockerization
-
 ### Support
 
 You can support us by contributing to this project, as well as providing feedback and ideas in the [issues](https://github.com/Pan-ML/panml/issues) section. 
 
 We would also appreciate if you can give panml a ⭐ on GitHub, and if it adds value to you, sharing this with others in your network on LinkedIn/Twitter/Medium etc who would also find this useful.
 
 
@@ -330,8 +315,23 @@
 ```
 
 ### Running tests
 ```
 python3 -m unittest
 ```
 
+### Roadmap
+
+Model development and analysis
+- Support for additional open source and commercial language model
+- Model evaluation methods (including adversarial evaluation)
+- Prompt engineering support and analysis (adding further methods and adding support for more LLMs)
+- Parameter-efficient fine tuning (e.g. LoRA, prompt tuning etc)
+- Model intepretability methods
+- Model emergent effect simulation and analysis (related to long term AI safety risks)
+
+Model productionisation
+- Automated refactoring of experimental code into source code
+- Automated API wrapper generation
+- Automated dockerization
+
```

### Comparing `panml-0.0.23/setup.py` & `panml-0.0.24/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '0.0.23', # version
+  version = '0.0.24', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'PanML team', # team name
   author_email = 'teampanml@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
```

### Comparing `panml-0.0.23/test/test_ModelPack.py` & `panml-0.0.24/test/test_ModelPack.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.23/test/test_VectorEngine.py` & `panml-0.0.24/test/test_VectorEngine.py`

 * *Files identical despite different names*

