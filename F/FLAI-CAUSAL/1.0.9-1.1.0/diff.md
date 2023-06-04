# Comparing `tmp/FLAI_CAUSAL-1.0.9.tar.gz` & `tmp/FLAI_CAUSAL-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAI_CAUSAL-1.0.9.tar", last modified: Sat Jun  3 17:57:07 2023, max compression
+gzip compressed data, was "FLAI_CAUSAL-1.1.0.tar", last modified: Sun Jun  4 10:48:11 2023, max compression
```

## Comparing `FLAI_CAUSAL-1.0.9.tar` & `FLAI_CAUSAL-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:57:07.966318 FLAI_CAUSAL-1.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:57:07.962318 FLAI_CAUSAL-1.0.9/FLAI/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 17:56:58.000000 FLAI_CAUSAL-1.0.9/FLAI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13502 2023-06-03 17:56:58.000000 FLAI_CAUSAL-1.0.9/FLAI/causal_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-06-03 17:56:58.000000 FLAI_CAUSAL-1.0.9/FLAI/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:57:07.962318 FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-03 17:57:07.000000 FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-03 17:57:07.000000 FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:57:07.000000 FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-03 17:57:07.000000 FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 17:57:07.000000 FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-03 17:56:58.000000 FLAI_CAUSAL-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-03 17:57:07.966318 FLAI_CAUSAL-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-03 17:56:58.000000 FLAI_CAUSAL-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:57:07.966318 FLAI_CAUSAL-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-03 17:56:58.000000 FLAI_CAUSAL-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:48:11.913789 FLAI_CAUSAL-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:48:11.913789 FLAI_CAUSAL-1.1.0/FLAI/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 10:47:59.000000 FLAI_CAUSAL-1.1.0/FLAI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-06-04 10:47:59.000000 FLAI_CAUSAL-1.1.0/FLAI/causal_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-06-04 10:47:59.000000 FLAI_CAUSAL-1.1.0/FLAI/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:48:11.913789 FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-04 10:48:11.000000 FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-04 10:48:11.000000 FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 10:48:11.000000 FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-04 10:48:11.000000 FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 10:48:11.000000 FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 10:47:59.000000 FLAI_CAUSAL-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-04 10:48:11.913789 FLAI_CAUSAL-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-04 10:47:59.000000 FLAI_CAUSAL-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 10:48:11.913789 FLAI_CAUSAL-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-04 10:47:59.000000 FLAI_CAUSAL-1.1.0/setup.py
```

### Comparing `FLAI_CAUSAL-1.0.9/FLAI/causal_graph.py` & `FLAI_CAUSAL-1.1.0/FLAI/causal_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,42 +67,40 @@
         test (str, optional): Type of test to be performed. Default is 'chi_square'.
         prune (bool, optional): If true, prunes the network after the test. Default is True.
         verbose (int, optional): Verbosity level. Default is 0.
         """
 
         self.graph = bn.independence_test(self.graph, flai_dataset.data, test, prune,verbose= verbose)
 
-    def inference(self,variables = [],evidence = {}):
+    def inference(self,variables = [],evidence = {},verbose=0):
         """
         Performs inference on the network given evidence.
 
         Args:
         variables (list, optional): List of variables to be included in the inference. Default is an empty list.
         evidence (dict, optional): Dictionary of evidence in the form {variable: value}. Default is an empty dictionary.
         """
 
         if len(variables) == 0:
             raise Exception("Variables should be provided") 
-        if len(evidence) == 0:
-            raise Exception("Evidence should be provided")  
-        return bn.inference.fit(self.graph, variables=variables, evidence=evidence).df          
+        return bn.inference.fit(self.graph, variables=variables, evidence=evidence,verbose = verbose).df          
 
-    def predict(self, data = None, variables = []):
+    def predict(self, data = None, variables = [],verbose=0):
         """
         Makes predictions based on the network.
 
         Args:
         data (DataFrame, optional): Data used for making predictions. Default is None.
         variables (list, optional): List of variables to be predicted. Default is an empty list.
         """
         if len(variables) == 0:
             raise Exception("Variables should be provided") 
         if data is None:
             raise Exception("Data should be provided") 
-        return bn.predict(self.graph, data, variables = variables)
+        return bn.predict(self.graph, data, variables = variables, verbose=verbose)
     
     def learn_cpd(self, flai_dataset = None, methodtype= None,verbose = 0):
         """
         Learn the Conditional Probability Distribution (CPD) for the network.
 
         Args:
         flai_dataset (flai.data.Data, optional): Dataset to be used for learning the CPD. Default is None.
```

### Comparing `FLAI_CAUSAL-1.0.9/FLAI/data.py` & `FLAI_CAUSAL-1.1.0/FLAI/data.py`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.9/FLAI_CAUSAL.egg-info/PKG-INFO` & `FLAI_CAUSAL-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1
-Name: FLAI-CAUSAL
-Version: 1.0.9
-Summary: Library to creat causal model and mitigate the bias.
-Home-page: https://github.com/rugonzs/FLAI
-Author: Rubén González Sendino
-Author-email: rubo.g@icloud.com
-License: Apache-2.0 license
-Project-URL: Documentation, https://scikit-learn.org/stable/documentation.html
-Project-URL: Source Code, https://github.com/rugonzs/FLAI
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 
 # FLAI : Fairness Learning in Artificial Intelligence
 
 [![Upload Python Package](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml)
 
+[![Upload Docs](https://github.com/rugonzs/FLAI/actions/workflows/docs.yml/badge.svg)](https://github.com/rugonzs/FLAI/actions/workflows/docs.yml)
+
+[![PyPI Version](https://img.shields.io/pypi/v/flai-causal)](https://pypi.org/project/flai-causal/)
+
+[![Downloads](https://static.pepy.tech/badge/flai-causal)](https://pepy.tech/project/flai-causal)
+
+[![Downloads](https://static.pepy.tech/badge/flai-causal/month)](https://pepy.tech/project/flai-causal)
+
+[![Downloads](https://static.pepy.tech/badge/flai-causal/week)](https://pepy.tech/project/flai-causal)
+
 Python library developed by Rubén González during his phD. research. His mission? To mitigate bias and discrimination through the application of causal algorithms.
 
 [Demo](https://www.rubengonzalez.ai/demo)
 
+[Documentation](https://rugonzs.github.io/FLAI/)
+
 ## Overview
 
 ![Overview](https://github.com/rugonzs/FLAI/blob/main/Documents/fair_algorithm.svg)
 
 **FLAI** is a Python library designed with two key functionalities: building a **causal algorithm** and **mitigating biases** within it.
 
 1. **Causal Algorithm Creation:** This library facilitates the development of a reliable causal algorithm, setting the stage for impartial data analysis.
```

### Comparing `FLAI_CAUSAL-1.0.9/LICENSE` & `FLAI_CAUSAL-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.9/PKG-INFO` & `FLAI_CAUSAL-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 Metadata-Version: 2.1
 Name: FLAI_CAUSAL
-Version: 1.0.9
+Version: 1.1.0
 Summary: Library to creat causal model and mitigate the bias.
 Home-page: https://github.com/rugonzs/FLAI
 Author: Rubén González Sendino
 Author-email: rubo.g@icloud.com
 License: Apache-2.0 license
-Project-URL: Documentation, https://scikit-learn.org/stable/documentation.html
+Project-URL: Documentation, https://rugonzs.github.io/FLAI/
 Project-URL: Source Code, https://github.com/rugonzs/FLAI
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
 # FLAI : Fairness Learning in Artificial Intelligence
 
 [![Upload Python Package](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml)
 
+[![Upload Docs](https://github.com/rugonzs/FLAI/actions/workflows/docs.yml/badge.svg)](https://github.com/rugonzs/FLAI/actions/workflows/docs.yml)
+
+[![PyPI Version](https://img.shields.io/pypi/v/flai-causal)](https://pypi.org/project/flai-causal/)
+
+[![Downloads](https://static.pepy.tech/badge/flai-causal)](https://pepy.tech/project/flai-causal)
+
+[![Downloads](https://static.pepy.tech/badge/flai-causal/month)](https://pepy.tech/project/flai-causal)
+
+[![Downloads](https://static.pepy.tech/badge/flai-causal/week)](https://pepy.tech/project/flai-causal)
+
 Python library developed by Rubén González during his phD. research. His mission? To mitigate bias and discrimination through the application of causal algorithms.
 
 [Demo](https://www.rubengonzalez.ai/demo)
 
+[Documentation](https://rugonzs.github.io/FLAI/)
+
 ## Overview
 
 ![Overview](https://github.com/rugonzs/FLAI/blob/main/Documents/fair_algorithm.svg)
 
 **FLAI** is a Python library designed with two key functionalities: building a **causal algorithm** and **mitigating biases** within it.
 
 1. **Causal Algorithm Creation:** This library facilitates the development of a reliable causal algorithm, setting the stage for impartial data analysis.
```

### Comparing `FLAI_CAUSAL-1.0.9/README.md` & `FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,42 @@
+Metadata-Version: 2.1
+Name: FLAI-CAUSAL
+Version: 1.1.0
+Summary: Library to creat causal model and mitigate the bias.
+Home-page: https://github.com/rugonzs/FLAI
+Author: Rubén González Sendino
+Author-email: rubo.g@icloud.com
+License: Apache-2.0 license
+Project-URL: Documentation, https://rugonzs.github.io/FLAI/
+Project-URL: Source Code, https://github.com/rugonzs/FLAI
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 
 # FLAI : Fairness Learning in Artificial Intelligence
 
 [![Upload Python Package](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml)
 
+[![Upload Docs](https://github.com/rugonzs/FLAI/actions/workflows/docs.yml/badge.svg)](https://github.com/rugonzs/FLAI/actions/workflows/docs.yml)
+
+[![PyPI Version](https://img.shields.io/pypi/v/flai-causal)](https://pypi.org/project/flai-causal/)
+
+[![Downloads](https://static.pepy.tech/badge/flai-causal)](https://pepy.tech/project/flai-causal)
+
+[![Downloads](https://static.pepy.tech/badge/flai-causal/month)](https://pepy.tech/project/flai-causal)
+
+[![Downloads](https://static.pepy.tech/badge/flai-causal/week)](https://pepy.tech/project/flai-causal)
+
 Python library developed by Rubén González during his phD. research. His mission? To mitigate bias and discrimination through the application of causal algorithms.
 
 [Demo](https://www.rubengonzalez.ai/demo)
 
+[Documentation](https://rugonzs.github.io/FLAI/)
+
 ## Overview
 
 ![Overview](https://github.com/rugonzs/FLAI/blob/main/Documents/fair_algorithm.svg)
 
 **FLAI** is a Python library designed with two key functionalities: building a **causal algorithm** and **mitigating biases** within it.
 
 1. **Causal Algorithm Creation:** This library facilitates the development of a reliable causal algorithm, setting the stage for impartial data analysis.
```

### Comparing `FLAI_CAUSAL-1.0.9/setup.py` & `FLAI_CAUSAL-1.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.9' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '1.1.0' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'FLAI_CAUSAL' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Rubén González Sendino' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'rubo.g@icloud.com' #Modificar con vuestros datos
 URL = 'https://github.com/rugonzs/FLAI' #Modificar con vuestros datos
 
 LICENSE = 'Apache-2.0 license' #Tipo de licencia
 DESCRIPTION = 'Library to creat causal model and mitigate the bias.' #Descripción corta
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8') #Referencia al documento README con una descripción más elaborada
 LONG_DESC_TYPE = "text/markdown"
 PROJECT_URLS = {
-    "Documentation": "https://scikit-learn.org/stable/documentation.html",
+    "Documentation": "https://rugonzs.github.io/FLAI/",
     "Source Code": 'https://github.com/rugonzs/FLAI',
 }
 
 #Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
       'bnlearn==0.7.8','networkx==2.8.8','matplotlib==3.6.2','pgmpy==0.1.20','numpy==1.23.4', 'pandas==1.5.1','scikit-learn==1.0.2','scipy==1.9.3','statsmodels==0.13.5'
       ]
```

