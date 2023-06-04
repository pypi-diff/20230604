# Comparing `tmp/templa-0.1.0.tar.gz` & `tmp/templa-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templa-0.1.0.tar", max compression
+gzip compressed data, was "templa-1.0.0.tar", max compression
```

## Comparing `templa-0.1.0.tar` & `templa-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-06-04 10:36:55.032322 templa-0.1.0/LICENSE
--rw-r--r--   0        0        0     3777 2023-06-04 10:36:55.032322 templa-0.1.0/README.md
--rw-r--r--   0        0        0     1541 2023-06-04 10:36:55.036321 templa-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      790 2023-06-04 10:36:55.040321 templa-0.1.0/src/templa/__init__.py
--rw-r--r--   0        0        0     9257 2023-06-04 10:36:55.040321 templa-0.1.0/src/templa/builder.py
--rw-r--r--   0        0        0     2810 2023-06-04 10:36:55.040321 templa-0.1.0/src/templa/config.py
--rw-r--r--   0        0        0        0 2023-06-04 10:36:55.040321 templa-0.1.0/src/templa/py.typed
--rw-r--r--   0        0        0     2855 2023-06-04 10:36:55.040321 templa-0.1.0/src/templa/yaml_builder.py
--rw-r--r--   0        0        0     4239 1970-01-01 00:00:00.000000 templa-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-06-04 12:07:30.966067 templa-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-06-04 12:07:30.966067 templa-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4059 2023-06-04 12:07:30.966067 templa-1.0.0/README.md
+-rw-r--r--   0        0        0     1731 2023-06-04 12:07:30.970067 templa-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      790 2023-06-04 12:07:30.970067 templa-1.0.0/src/templa/__init__.py
+-rw-r--r--   0        0        0     9257 2023-06-04 12:07:30.970067 templa-1.0.0/src/templa/builder.py
+-rw-r--r--   0        0        0     2810 2023-06-04 12:07:30.970067 templa-1.0.0/src/templa/config.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:07:30.970067 templa-1.0.0/src/templa/py.typed
+-rw-r--r--   0        0        0     2891 2023-06-04 12:07:30.970067 templa-1.0.0/src/templa/yaml_builder.py
+-rw-r--r--   0        0        0     4791 1970-01-01 00:00:00.000000 templa-1.0.0/PKG-INFO
```

### Comparing `templa-0.1.0/LICENSE` & `templa-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `templa-0.1.0/README.md` & `templa-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Run Tests](https://github.com/yuxki/templa/actions/workflows/tests.yml/badge.svg)](https://github.com/yuxki/templa/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/templa/badge/?version=latest)](https://templa.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/yuxki/templa/badge.svg?branch=master)](https://coveralls.io/github/yuxki/templa?branch=master)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Stable Version](https://img.shields.io/pypi/v/templa)](https://pypi.org/project/templa/)
+[![Python Versions](https://img.shields.io/pypi/pyversions/templa)](https://pypi.org/project/templa)
 
 # templa
 
 Templa is a Python library that offers a flexible and typed building system using
 Jinja2 templates for your code. It allows you to easily render, parse, process,
 and build. The following are the assumed build processes in Templa:
 
 - Define the required context with dataclass for rendering a Jinja2 formatted template.
 - Render the template with Jinja2 library using the provided context.
 - Extract relevant information and elements from the rendered template for further processing.
 - Perform necessary processing on the parsed rendered template.
 - Utilize the processed rendered template to generate desired outputs or objects.
 
+
+## Installation
+```shell
+$ pip install templa
+```
+
+## Example
+
 ```python
 from dataclasses import dataclass
 from typing import List
 from typing import Optional
 
 import jinja2
 import yaml
@@ -92,12 +103,7 @@
     built_target = builder.build(processed_target)
     print(builder.fetch_built(built_target))
 
 
 if __name__ == "__main__":
     build_sample_template()
 ```
-
-## Install
-```shell
-$ pip install 'templa@git+https://github.com/yuxki/templa.git'
-```
```

### Comparing `templa-0.1.0/pyproject.toml` & `templa-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 [tool.poetry]
 name = "templa"
-version = "0.1.0"
-description = ""
+version = "1.0.0"
+description = "Building system using Jinja2 templates for your code."
 authors = ["yuxki <yuxki.ryoshi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://github.com/yuxki/templa"
+documentation = "https://templa.readthedocs.io/en/latest/index.html"
+include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
-python = "^3.9.16"
+python = "^3.8"
 jinja2 = "3.1.2"
 pyyaml = "6.0"
 
 [tool.poetry.group.dev.dependencies]
 tox = "^4.5.1"
 pre-commit = "^3.3.2"
 mypy = "^1.3.0"
 dodgy = "^0.2.1"
-flake8 = "^6.0.0"
 types-pyyaml = "^6.0.12.9"
 black = "^23.3.0"
 pytest = "^7.3.1"
 coveralls = "^3.3.1"
+flake8 = "4.0.1"
 
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.0.1"
 furo = "^2023.5.20"
 pydantic = "^1.10.8"
```

### Comparing `templa-0.1.0/src/templa/__init__.py` & `templa-1.0.0/src/templa/__init__.py`

 * *Files identical despite different names*

### Comparing `templa-0.1.0/src/templa/builder.py` & `templa-1.0.0/src/templa/builder.py`

 * *Files identical despite different names*

### Comparing `templa-0.1.0/src/templa/config.py` & `templa-1.0.0/src/templa/config.py`

 * *Files identical despite different names*

### Comparing `templa-0.1.0/src/templa/yaml_builder.py` & `templa-1.0.0/src/templa/yaml_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from collections import OrderedDict
 from typing import Any
 
 import yaml
 from jinja2 import Environment
 from jinja2 import Template
```

### Comparing `templa-0.1.0/PKG-INFO` & `templa-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,55 @@
 Metadata-Version: 2.1
 Name: templa
-Version: 0.1.0
-Summary: 
+Version: 1.0.0
+Summary: Building system using Jinja2 templates for your code.
+Home-page: https://github.com/yuxki/templa
 License: MIT
 Author: yuxki
 Author-email: yuxki.ryoshi@gmail.com
-Requires-Python: >=3.9.16,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jinja2 (==3.1.2)
 Requires-Dist: pyyaml (==6.0)
+Project-URL: Documentation, https://templa.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Run Tests](https://github.com/yuxki/templa/actions/workflows/tests.yml/badge.svg)](https://github.com/yuxki/templa/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/templa/badge/?version=latest)](https://templa.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/yuxki/templa/badge.svg?branch=master)](https://coveralls.io/github/yuxki/templa?branch=master)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Stable Version](https://img.shields.io/pypi/v/templa)](https://pypi.org/project/templa/)
+[![Python Versions](https://img.shields.io/pypi/pyversions/templa)](https://pypi.org/project/templa)
 
 # templa
 
 Templa is a Python library that offers a flexible and typed building system using
 Jinja2 templates for your code. It allows you to easily render, parse, process,
 and build. The following are the assumed build processes in Templa:
 
 - Define the required context with dataclass for rendering a Jinja2 formatted template.
 - Render the template with Jinja2 library using the provided context.
 - Extract relevant information and elements from the rendered template for further processing.
 - Perform necessary processing on the parsed rendered template.
 - Utilize the processed rendered template to generate desired outputs or objects.
 
+
+## Installation
+```shell
+$ pip install templa
+```
+
+## Example
+
 ```python
 from dataclasses import dataclass
 from typing import List
 from typing import Optional
 
 import jinja2
 import yaml
@@ -109,12 +124,7 @@
     print(builder.fetch_built(built_target))
 
 
 if __name__ == "__main__":
     build_sample_template()
 ```
 
-## Install
-```shell
-$ pip install 'templa@git+https://github.com/yuxki/templa.git'
-```
-
```

