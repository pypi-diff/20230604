# Comparing `tmp/saxo_apy-0.2.4.tar.gz` & `tmp/saxo_apy-0.2.5.tar.gz`

## Comparing `saxo_apy-0.2.4.tar` & `saxo_apy-0.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/.DS_Store
--rw-r--r--   0        0        0   207362 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/pdm.lock
--rw-r--r--   0        0        0     6514 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/samples/01_getting_started.ipynb
--rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/samples/02_advanced_login.ipynb
--rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/samples/03_session_management.ipynb
--rw-r--r--   0        0        0    10513 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/samples/04_debugging_and_logging.ipynb
--rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/samples/05_price_alerts_crud.ipynb
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/samples/06_instrument_search.ipynb
--rw-r--r--   0        0        0    10551 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/samples/07_pricing_and_orders.ipynb
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/samples/README.md
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/samples/s01_async_requests.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/samples/s02_streaming_prices.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/saxo_apy/__init__.py
--rw-r--r--   0        0        0    17889 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/saxo_apy/client.py
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/saxo_apy/models.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/saxo_apy/redirect_server.py
--rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/saxo_apy/utils.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/saxo_apy/version.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/tests/test_client.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/tests/test_models.py
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/tests/test_utils.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/tests/fixtures/dummy_access_token.txt
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/tests/fixtures/dummy_app_config_live.json
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/tests/fixtures/dummy_app_config_sim.json
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/tests/fixtures/models.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/LICENSE
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/README.md
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 saxo_apy-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/.DS_Store
+-rw-r--r--   0        0        0   211911 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/pdm.lock
+-rw-r--r--   0        0        0     6514 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/01_getting_started.ipynb
+-rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/02_advanced_login.ipynb
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/03_session_management.ipynb
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/04_debugging_and_logging.ipynb
+-rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/05_price_alerts_crud.ipynb
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/06_instrument_search.ipynb
+-rw-r--r--   0        0        0    10551 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/07_pricing_and_orders.ipynb
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/README.md
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/s01_async_requests.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/s02_streaming_prices.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/saxo_apy/__init__.py
+-rw-r--r--   0        0        0    18398 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/saxo_apy/client.py
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/saxo_apy/models.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/saxo_apy/redirect_server.py
+-rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/saxo_apy/utils.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/saxo_apy/version.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/test_client.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/test_models.py
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/test_utils.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/fixtures/dummy_access_token.txt
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/fixtures/dummy_app_config_live.json
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/fixtures/dummy_app_config_sim.json
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/fixtures/models.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/README.md
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/PKG-INFO
```

### Comparing `saxo_apy-0.2.4/.DS_Store` & `saxo_apy-0.2.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/pdm.lock` & `saxo_apy-0.2.5/pdm.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # This file is @generated by PDM.
 # It is not intended for manual editing.
 
 [[package]]
 name = "anyio"
-version = "3.6.2"
-requires_python = ">=3.6.2"
+version = "3.7.0"
+requires_python = ">=3.7"
 summary = "High level compatibility layer for multiple asynchronous event loop implementations"
 dependencies = [
+    "exceptiongroup; python_version < \"3.11\"",
     "idna>=2.8",
     "sniffio>=1.1",
     "typing-extensions; python_version < \"3.8\"",
 ]
 
 [[package]]
 name = "appnope"
@@ -34,72 +35,76 @@
 summary = "Low-level CFFI bindings for Argon2"
 dependencies = [
     "cffi>=1.0.1",
 ]
 
 [[package]]
 name = "attrs"
-version = "22.2.0"
-requires_python = ">=3.6"
+version = "23.1.0"
+requires_python = ">=3.7"
 summary = "Classes Without Boilerplate"
+dependencies = [
+    "importlib-metadata; python_version < \"3.8\"",
+]
 
 [[package]]
 name = "backcall"
 version = "0.2.0"
 summary = "Specifications for callback functions passed in to an API"
 
 [[package]]
 name = "beautifulsoup4"
-version = "4.11.1"
+version = "4.12.2"
 requires_python = ">=3.6.0"
 summary = "Screen-scraping library"
 dependencies = [
     "soupsieve>1.2",
 ]
 
 [[package]]
 name = "black"
-version = "22.12.0"
+version = "23.3.0"
 requires_python = ">=3.7"
 summary = "The uncompromising code formatter."
 dependencies = [
     "click>=8.0.0",
     "mypy-extensions>=0.4.3",
+    "packaging>=22.0",
     "pathspec>=0.9.0",
     "platformdirs>=2",
-    "tomli>=1.1.0; python_full_version < \"3.11.0a7\"",
+    "tomli>=1.1.0; python_version < \"3.11\"",
     "typed-ast>=1.4.2; python_version < \"3.8\" and implementation_name == \"cpython\"",
     "typing-extensions>=3.10.0.0; python_version < \"3.10\"",
 ]
 
 [[package]]
 name = "black"
-version = "22.12.0"
+version = "23.3.0"
 extras = ["jupyter"]
 requires_python = ">=3.7"
 summary = "The uncompromising code formatter."
 dependencies = [
-    "black==22.12.0",
+    "black==23.3.0",
     "ipython>=7.8.0",
     "tokenize-rt>=3.2.0",
 ]
 
 [[package]]
 name = "bleach"
-version = "5.0.1"
+version = "6.0.0"
 requires_python = ">=3.7"
 summary = "An easy safelist-based HTML-sanitizing tool."
 dependencies = [
     "six>=1.9.0",
     "webencodings",
 ]
 
 [[package]]
 name = "certifi"
-version = "2022.12.7"
+version = "2023.5.7"
 requires_python = ">=3.6"
 summary = "Python package for providing Mozilla's CA Bundle."
 
 [[package]]
 name = "cffi"
 version = "1.15.1"
 summary = "Foreign Function Interface for Python calling C code."
@@ -121,32 +126,32 @@
 name = "colorama"
 version = "0.4.6"
 requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
 summary = "Cross-platform colored terminal text."
 
 [[package]]
 name = "coverage"
-version = "7.0.5"
+version = "7.2.7"
 requires_python = ">=3.7"
 summary = "Code coverage measurement for Python"
 
 [[package]]
 name = "coverage"
-version = "7.0.5"
+version = "7.2.7"
 extras = ["toml"]
 requires_python = ">=3.7"
 summary = "Code coverage measurement for Python"
 dependencies = [
-    "coverage==7.0.5",
+    "coverage==7.2.7",
     "tomli; python_full_version <= \"3.11.0a6\"",
 ]
 
 [[package]]
 name = "debugpy"
-version = "1.6.5"
+version = "1.6.7"
 requires_python = ">=3.7"
 summary = "An implementation of the Debug Adapter Protocol for Python"
 
 [[package]]
 name = "decorator"
 version = "5.1.1"
 requires_python = ">=3.5"
@@ -162,21 +167,21 @@
 name = "entrypoints"
 version = "0.4"
 requires_python = ">=3.6"
 summary = "Discover and load entry points from installed packages."
 
 [[package]]
 name = "exceptiongroup"
-version = "1.1.0"
+version = "1.1.1"
 requires_python = ">=3.7"
 summary = "Backport of PEP 654 (exception groups)"
 
 [[package]]
 name = "fastjsonschema"
-version = "2.16.2"
+version = "2.17.1"
 summary = "Fastest Python implementation of JSON schema"
 
 [[package]]
 name = "flake8"
 version = "5.0.4"
 requires_python = ">=3.6.1"
 summary = "the modular source code checker: pep8 pyflakes and co"
@@ -185,25 +190,25 @@
     "mccabe<0.8.0,>=0.7.0",
     "pycodestyle<2.10.0,>=2.9.0",
     "pyflakes<2.6.0,>=2.5.0",
 ]
 
 [[package]]
 name = "flake8-pyproject"
-version = "1.2.2"
+version = "1.2.3"
 requires_python = ">= 3.6"
 summary = "Flake8 plug-in loading the configuration from pyproject.toml"
 dependencies = [
     "Flake8>=5",
     "TOMLi; python_version < \"3.11\"",
 ]
 
 [[package]]
 name = "flask"
-version = "2.2.2"
+version = "2.2.5"
 requires_python = ">=3.7"
 summary = "A simple framework for building complex web applications."
 dependencies = [
     "Jinja2>=3.0",
     "Werkzeug>=2.2.2",
     "click>=8.0",
     "importlib-metadata>=3.6.0; python_version < \"3.10\"",
@@ -217,33 +222,33 @@
 summary = "A pure-Python, bring-your-own-I/O implementation of HTTP/1.1"
 dependencies = [
     "typing-extensions; python_version < \"3.8\"",
 ]
 
 [[package]]
 name = "httpcore"
-version = "0.16.3"
+version = "0.17.2"
 requires_python = ">=3.7"
 summary = "A minimal low-level HTTP client."
 dependencies = [
     "anyio<5.0,>=3.0",
     "certifi",
     "h11<0.15,>=0.13",
     "sniffio==1.*",
 ]
 
 [[package]]
 name = "httpx"
-version = "0.23.3"
+version = "0.24.1"
 requires_python = ">=3.7"
 summary = "The next generation HTTP client."
 dependencies = [
     "certifi",
-    "httpcore<0.17.0,>=0.15.0",
-    "rfc3986[idna2008]<2,>=1.3",
+    "httpcore<0.18.0,>=0.15.0",
+    "idna",
     "sniffio",
 ]
 
 [[package]]
 name = "idna"
 version = "3.4"
 requires_python = ">=3.5"
@@ -257,15 +262,15 @@
 dependencies = [
     "typing-extensions>=3.6.4; python_version < \"3.8\"",
     "zipp>=0.5",
 ]
 
 [[package]]
 name = "importlib-resources"
-version = "5.10.2"
+version = "5.12.0"
 requires_python = ">=3.7"
 summary = "Read resources from Python packages"
 dependencies = [
     "zipp>=3.1.0; python_version < \"3.10\"",
 ]
 
 [[package]]
@@ -316,23 +321,23 @@
 [[package]]
 name = "ipython-genutils"
 version = "0.2.0"
 summary = "Vestigial utilities from IPython"
 
 [[package]]
 name = "ipywidgets"
-version = "8.0.4"
+version = "8.0.6"
 requires_python = ">=3.7"
 summary = "Jupyter interactive widgets"
 dependencies = [
     "ipykernel>=4.5.1",
     "ipython>=6.1.0",
-    "jupyterlab-widgets~=3.0",
+    "jupyterlab-widgets~=3.0.7",
     "traitlets>=4.3.1",
-    "widgetsnbextension~=4.0",
+    "widgetsnbextension~=4.0.7",
 ]
 
 [[package]]
 name = "isort"
 version = "5.11.5"
 requires_python = ">=3.7.0"
 summary = "A Python utility / library to sort Python imports."
@@ -401,38 +406,41 @@
     "pyzmq>=23.0",
     "tornado>=6.2",
     "traitlets",
 ]
 
 [[package]]
 name = "jupyter-console"
-version = "6.4.4"
+version = "6.6.3"
 requires_python = ">=3.7"
 summary = "Jupyter terminal console"
 dependencies = [
-    "ipykernel",
+    "ipykernel>=6.14",
     "ipython",
     "jupyter-client>=7.0.0",
-    "prompt-toolkit!=3.0.0,!=3.0.1,<3.1.0,>=2.0.0",
+    "jupyter-core!=5.0.*,>=4.12",
+    "prompt-toolkit>=3.0.30",
     "pygments",
+    "pyzmq>=17",
+    "traitlets>=5.4",
 ]
 
 [[package]]
 name = "jupyter-core"
 version = "4.12.0"
 requires_python = ">=3.7"
 summary = "Jupyter core package. A base package on which Jupyter projects rely."
 dependencies = [
     "pywin32>=1.0; sys_platform == \"win32\" and platform_python_implementation != \"PyPy\"",
     "traitlets",
 ]
 
 [[package]]
 name = "jupyter-server"
-version = "1.23.5"
+version = "1.24.0"
 requires_python = ">=3.7"
 summary = "The backend—i.e. core services, APIs, and REST endpoints—to Jupyter web applications."
 dependencies = [
     "Send2Trash",
     "anyio<4,>=3.1.0",
     "argon2-cffi",
     "jinja2",
@@ -454,31 +462,31 @@
 name = "jupyterlab-pygments"
 version = "0.2.2"
 requires_python = ">=3.7"
 summary = "Pygments theme using JupyterLab CSS variables"
 
 [[package]]
 name = "jupyterlab-widgets"
-version = "3.0.5"
+version = "3.0.7"
 requires_python = ">=3.7"
 summary = "Jupyter interactive widgets for JupyterLab"
 
 [[package]]
 name = "loguru"
-version = "0.6.0"
+version = "0.7.0"
 requires_python = ">=3.5"
 summary = "Python logging made (stupidly) simple"
 dependencies = [
     "colorama>=0.3.4; sys_platform == \"win32\"",
     "win32-setctime>=1.0.0; sys_platform == \"win32\"",
 ]
 
 [[package]]
 name = "markupsafe"
-version = "2.1.2"
+version = "2.1.3"
 requires_python = ">=3.7"
 summary = "Safely add untrusted strings to HTML/XML markup."
 
 [[package]]
 name = "matplotlib-inline"
 version = "0.1.6"
 requires_python = ">=3.5"
@@ -491,74 +499,75 @@
 name = "mccabe"
 version = "0.7.0"
 requires_python = ">=3.6"
 summary = "McCabe checker, plugin for flake8"
 
 [[package]]
 name = "mistune"
-version = "2.0.4"
+version = "2.0.5"
 summary = "A sane Markdown parser with useful plugins and renderers"
 
 [[package]]
 name = "mypy"
-version = "0.991"
+version = "1.3.0"
 requires_python = ">=3.7"
 summary = "Optional static typing for Python"
 dependencies = [
-    "mypy-extensions>=0.4.3",
+    "mypy-extensions>=1.0.0",
     "tomli>=1.1.0; python_version < \"3.11\"",
     "typed-ast<2,>=1.4.0; python_version < \"3.8\"",
     "typing-extensions>=3.10",
 ]
 
 [[package]]
 name = "mypy-extensions"
-version = "0.4.3"
-summary = "Experimental type system extensions for programs checked with the mypy typechecker."
+version = "1.0.0"
+requires_python = ">=3.5"
+summary = "Type system extensions for programs checked with the mypy type checker."
 
 [[package]]
 name = "nbclassic"
-version = "0.4.8"
+version = "1.0.0"
 requires_python = ">=3.7"
-summary = "A web-based notebook environment for interactive computing"
+summary = "Jupyter Notebook as a Jupyter Server extension."
 dependencies = [
     "Send2Trash>=1.8.0",
     "argon2-cffi",
     "ipykernel",
     "ipython-genutils",
     "jinja2",
     "jupyter-client>=6.1.1",
     "jupyter-core>=4.6.1",
     "jupyter-server>=1.8",
     "nbconvert>=5",
     "nbformat",
     "nest-asyncio>=1.5",
-    "notebook-shim>=0.1.0",
+    "notebook-shim>=0.2.3",
     "prometheus-client",
     "pyzmq>=17",
     "terminado>=0.8.3",
     "tornado>=6.1",
     "traitlets>=4.2.1",
 ]
 
 [[package]]
 name = "nbclient"
-version = "0.7.2"
+version = "0.7.4"
 requires_python = ">=3.7.0"
 summary = "A client library for executing notebooks. Formerly nbconvert's ExecutePreprocessor."
 dependencies = [
     "jupyter-client>=6.1.12",
     "jupyter-core!=5.0.*,>=4.12",
     "nbformat>=5.1",
     "traitlets>=5.3",
 ]
 
 [[package]]
 name = "nbconvert"
-version = "7.2.8"
+version = "7.4.0"
 requires_python = ">=3.7"
 summary = "Converting Jupyter Notebooks"
 dependencies = [
     "beautifulsoup4",
     "bleach",
     "defusedxml",
     "importlib-metadata>=3.6; python_version < \"3.10\"",
@@ -574,15 +583,15 @@
     "pygments>=2.4.1",
     "tinycss2",
     "traitlets>=5.0",
 ]
 
 [[package]]
 name = "nbformat"
-version = "5.7.3"
+version = "5.8.0"
 requires_python = ">=3.7"
 summary = "The Jupyter Notebook format"
 dependencies = [
     "fastjsonschema",
     "importlib-metadata>=3.6; python_version < \"3.8\"",
     "jsonschema>=2.6",
     "jupyter-core",
@@ -593,15 +602,15 @@
 name = "nest-asyncio"
 version = "1.5.6"
 requires_python = ">=3.5"
 summary = "Patch asyncio to allow nested event loops"
 
 [[package]]
 name = "notebook"
-version = "6.5.2"
+version = "6.5.4"
 requires_python = ">=3.7"
 summary = "A web-based notebook environment for interactive computing"
 dependencies = [
     "Send2Trash>=1.8.0",
     "argon2-cffi",
     "ipykernel",
     "ipython-genutils",
@@ -617,24 +626,24 @@
     "terminado>=0.8.3",
     "tornado>=6.1",
     "traitlets>=4.2.1",
 ]
 
 [[package]]
 name = "notebook-shim"
-version = "0.2.2"
+version = "0.2.3"
 requires_python = ">=3.7"
 summary = "A shim layer for notebook traits and config"
 dependencies = [
     "jupyter-server<3,>=1.8",
 ]
 
 [[package]]
 name = "packaging"
-version = "23.0"
+version = "23.1"
 requires_python = ">=3.7"
 summary = "Core utilities for Python packages"
 
 [[package]]
 name = "pandocfilters"
 version = "1.5.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
@@ -644,15 +653,15 @@
 name = "parso"
 version = "0.8.3"
 requires_python = ">=3.6"
 summary = "A Python Parser"
 
 [[package]]
 name = "pathspec"
-version = "0.10.3"
+version = "0.11.1"
 requires_python = ">=3.7"
 summary = "Utility library for gitignore style pattern matching of file paths."
 
 [[package]]
 name = "pexpect"
 version = "4.8.0"
 summary = "Pexpect allows easy control of interactive console applications."
@@ -669,48 +678,48 @@
 name = "pkgutil-resolve-name"
 version = "1.3.10"
 requires_python = ">=3.6"
 summary = "Resolve a name to an object."
 
 [[package]]
 name = "platformdirs"
-version = "2.6.2"
+version = "3.5.1"
 requires_python = ">=3.7"
 summary = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 dependencies = [
-    "typing-extensions>=4.4; python_version < \"3.8\"",
+    "typing-extensions>=4.5; python_version < \"3.8\"",
 ]
 
 [[package]]
 name = "pluggy"
 version = "1.0.0"
 requires_python = ">=3.6"
 summary = "plugin and hook calling mechanisms for python"
 dependencies = [
     "importlib-metadata>=0.12; python_version < \"3.8\"",
 ]
 
 [[package]]
 name = "prometheus-client"
-version = "0.15.0"
+version = "0.17.0"
 requires_python = ">=3.6"
 summary = "Python client for the Prometheus monitoring system."
 
 [[package]]
 name = "prompt-toolkit"
-version = "3.0.36"
-requires_python = ">=3.6.2"
+version = "3.0.38"
+requires_python = ">=3.7.0"
 summary = "Library for building powerful interactive command lines in Python"
 dependencies = [
     "wcwidth",
 ]
 
 [[package]]
 name = "psutil"
-version = "5.9.4"
+version = "5.9.5"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "Cross-platform lib for process and system monitoring in Python."
 
 [[package]]
 name = "ptyprocess"
 version = "0.7.0"
 summary = "Run a subprocess in a pseudo terminal"
@@ -725,15 +734,15 @@
 name = "pycparser"
 version = "2.21"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "C parser in Python"
 
 [[package]]
 name = "pydantic"
-version = "1.10.4"
+version = "1.10.8"
 requires_python = ">=3.7"
 summary = "Data validation and settings management using python type hints"
 dependencies = [
     "typing-extensions>=4.2.0",
 ]
 
 [[package]]
@@ -750,44 +759,43 @@
 name = "pyflakes"
 version = "2.5.0"
 requires_python = ">=3.6"
 summary = "passive checker of Python programs"
 
 [[package]]
 name = "pygments"
-version = "2.14.0"
-requires_python = ">=3.6"
+version = "2.15.1"
+requires_python = ">=3.7"
 summary = "Pygments is a syntax highlighting package written in Python."
 
 [[package]]
 name = "pyrsistent"
 version = "0.19.3"
 requires_python = ">=3.7"
 summary = "Persistent/Functional/Immutable data structures"
 
 [[package]]
 name = "pytest"
-version = "7.2.1"
+version = "7.3.1"
 requires_python = ">=3.7"
 summary = "pytest: simple powerful testing with Python"
 dependencies = [
-    "attrs>=19.2.0",
     "colorama; sys_platform == \"win32\"",
     "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
     "importlib-metadata>=0.12; python_version < \"3.8\"",
     "iniconfig",
     "packaging",
     "pluggy<2.0,>=0.12",
     "tomli>=1.0.0; python_version < \"3.11\"",
 ]
 
 [[package]]
 name = "pytest-cov"
-version = "4.0.0"
-requires_python = ">=3.6"
+version = "4.1.0"
+requires_python = ">=3.7"
 summary = "Pytest plugin for measuring coverage."
 dependencies = [
     "coverage[toml]>=5.2.1",
     "pytest>=4.6",
 ]
 
 [[package]]
@@ -797,80 +805,67 @@
 summary = "Extensions to the standard Python datetime module"
 dependencies = [
     "six>=1.5",
 ]
 
 [[package]]
 name = "pywin32"
-version = "305"
+version = "306"
 summary = "Python for Window Extensions"
 
 [[package]]
 name = "pywinpty"
 version = "2.0.10"
 requires_python = ">=3.7"
 summary = "Pseudo terminal support for Windows from Python."
 
 [[package]]
 name = "pyzmq"
-version = "25.0.0"
+version = "25.1.0"
 requires_python = ">=3.6"
 summary = "Python bindings for 0MQ"
 dependencies = [
     "cffi; implementation_name == \"pypy\"",
 ]
 
 [[package]]
 name = "qtconsole"
-version = "5.4.0"
+version = "5.4.3"
 requires_python = ">= 3.7"
 summary = "Jupyter Qt console"
 dependencies = [
     "ipykernel>=4.1",
     "ipython-genutils",
     "jupyter-client>=4.1",
     "jupyter-core",
+    "packaging",
     "pygments",
     "pyzmq>=17.1",
     "qtpy>=2.0.1",
     "traitlets!=5.2.1,!=5.2.2",
 ]
 
 [[package]]
 name = "qtpy"
-version = "2.3.0"
+version = "2.3.1"
 requires_python = ">=3.7"
 summary = "Provides an abstraction layer on top of the various Qt bindings (PyQt5/6 and PySide2/6)."
 dependencies = [
     "packaging",
 ]
 
 [[package]]
-name = "rfc3986"
-version = "1.5.0"
-summary = "Validating URI References per RFC 3986"
-
-[[package]]
-name = "rfc3986"
-version = "1.5.0"
-extras = ["idna2008"]
-summary = "Validating URI References per RFC 3986"
-dependencies = [
-    "idna",
-    "rfc3986==1.5.0",
-]
-
-[[package]]
 name = "send2trash"
-version = "1.8.0"
-summary = "Send file to trash natively under Mac OS X, Windows and Linux."
+version = "1.8.2"
+requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,>=2.7"
+summary = "Send file to trash natively under Mac OS X, Windows and Linux"
 
 [[package]]
 name = "setuptools"
-version = "66.1.1"
+version = "67.8.0"
 requires_python = ">=3.7"
 summary = "Easily download, build, install, upgrade, and uninstall Python packages"
 
 [[package]]
 name = "six"
 version = "1.16.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
@@ -885,16 +880,16 @@
 [[package]]
 name = "snowballstemmer"
 version = "2.2.0"
 summary = "This package provides 29 stemmers for 28 languages generated from Snowball algorithms."
 
 [[package]]
 name = "soupsieve"
-version = "2.3.2.post1"
-requires_python = ">=3.6"
+version = "2.4.1"
+requires_python = ">=3.7"
 summary = "A modern CSS selector implementation for Beautiful Soup."
 
 [[package]]
 name = "terminado"
 version = "0.17.1"
 requires_python = ">=3.7"
 summary = "Tornado websocket backend for the Xterm.js Javascript terminal emulator library."
@@ -929,27 +924,27 @@
 name = "tornado"
 version = "6.2"
 requires_python = ">= 3.7"
 summary = "Tornado is a Python web framework and asynchronous networking library, originally developed at FriendFeed."
 
 [[package]]
 name = "traitlets"
-version = "5.8.1"
+version = "5.9.0"
 requires_python = ">=3.7"
 summary = "Traitlets Python configuration system"
 
 [[package]]
 name = "typed-ast"
 version = "1.5.4"
 requires_python = ">=3.6"
 summary = "a fork of Python 2 and 3 ast modules with type comment support"
 
 [[package]]
 name = "typing-extensions"
-version = "4.4.0"
+version = "4.6.3"
 requires_python = ">=3.7"
 summary = "Backported and Experimental Type Hints for Python 3.7+"
 
 [[package]]
 name = "wcwidth"
 version = "0.2.6"
 summary = "Measures the displayed width of unicode strings in a terminal"
@@ -957,59 +952,61 @@
 [[package]]
 name = "webencodings"
 version = "0.5.1"
 summary = "Character encoding aliases for legacy web content"
 
 [[package]]
 name = "websocket-client"
-version = "1.4.2"
+version = "1.5.2"
 requires_python = ">=3.7"
 summary = "WebSocket client for Python with low level API options"
 
 [[package]]
 name = "websockets"
-version = "10.4"
+version = "11.0.3"
 requires_python = ">=3.7"
 summary = "An implementation of the WebSocket Protocol (RFC 6455 & 7692)"
 
 [[package]]
 name = "werkzeug"
-version = "2.2.2"
+version = "2.2.3"
 requires_python = ">=3.7"
 summary = "The comprehensive WSGI web application library."
 dependencies = [
     "MarkupSafe>=2.1.1",
 ]
 
 [[package]]
 name = "widgetsnbextension"
-version = "4.0.5"
+version = "4.0.7"
 requires_python = ">=3.7"
 summary = "Jupyter interactive widgets for Jupyter Notebook"
 
 [[package]]
 name = "win32-setctime"
 version = "1.1.0"
 requires_python = ">=3.5"
 summary = "A small Python utility to set file creation time on Windows"
 
 [[package]]
 name = "zipp"
-version = "3.11.0"
+version = "3.15.0"
 requires_python = ">=3.7"
 summary = "Backport of pathlib-compatible object wrapper for zip files"
 
 [metadata]
-lock_version = "4.1"
-content_hash = "sha256:5c5e2f205ebe6d36c6f312ef811d7c8d95a2d41350da1f1743f424ad8592e1e9"
+lock_version = "4.2"
+cross_platform = true
+groups = ["default", "dev"]
+content_hash = "sha256:fd5ce86dcb495ee28efdde0ddbd49b6e8ae6b974254e52b41c0c12feeae22f3b"
 
 [metadata.files]
-"anyio 3.6.2" = [
-    {url = "https://files.pythonhosted.org/packages/77/2b/b4c0b7a3f3d61adb1a1e0b78f90a94e2b6162a043880704b7437ef297cad/anyio-3.6.2-py3-none-any.whl", hash = "sha256:fbbe32bd270d2a2ef3ed1c5d45041250284e31fc0a4df4a5a6071842051a51e3"},
-    {url = "https://files.pythonhosted.org/packages/8b/94/6928d4345f2bc1beecbff03325cad43d320717f51ab74ab5a571324f4f5a/anyio-3.6.2.tar.gz", hash = "sha256:25ea0d673ae30af41a0c442f81cf3b38c7e79fdc7b60335a4c14e05eb0947421"},
+"anyio 3.7.0" = [
+    {url = "https://files.pythonhosted.org/packages/68/fe/7ce1926952c8a403b35029e194555558514b365ad77d75125f521a2bec62/anyio-3.7.0-py3-none-any.whl", hash = "sha256:eddca883c4175f14df8aedce21054bfca3adb70ffe76a9f607aef9d7fa2ea7f0"},
+    {url = "https://files.pythonhosted.org/packages/c6/b3/fefbf7e78ab3b805dec67d698dc18dd505af7a18a8dd08868c9b4fa736b5/anyio-3.7.0.tar.gz", hash = "sha256:275d9973793619a5374e1c89a4f4ad3f4b0a5510a2b5b939444bee8f4c4d37ce"},
 ]
 "appnope 0.1.3" = [
     {url = "https://files.pythonhosted.org/packages/41/4a/381783f26df413dde4c70c734163d88ca0550a1361cb74a1c68f47550619/appnope-0.1.3-py2.py3-none-any.whl", hash = "sha256:265a455292d0bd8a72453494fa24df5a11eb18373a60c7c0430889f22548605e"},
     {url = "https://files.pythonhosted.org/packages/6a/cd/355842c0db33192ac0fc822e2dcae835669ef317fe56c795fb55fcddb26f/appnope-0.1.3.tar.gz", hash = "sha256:02bd91c4de869fbb1e1c50aafc4098827a7a54ab2f39d9dcba6c9547ed920e24"},
 ]
 "argon2-cffi 21.3.0" = [
     {url = "https://files.pythonhosted.org/packages/3f/18/20bb5b6bf55e55d14558b57afc3d4476349ab90e0c43e60f27a7c2187289/argon2-cffi-21.3.0.tar.gz", hash = "sha256:d384164d944190a7dd7ef22c6aa3ff197da12962bd04b17f64d4e93d934dba5b"},
@@ -1034,47 +1031,60 @@
     {url = "https://files.pythonhosted.org/packages/dc/46/610263c404f33127878515819217aafd150906814624c31a6ad18a0a40fb/argon2_cffi_bindings-21.2.0-pp37-pypy37_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2c3e3cc67fdb7d82c4718f19b4e7a87123caf8a93fde7e23cf66ac0337d3cb3f"},
     {url = "https://files.pythonhosted.org/packages/ec/f7/378254e6dd7ae6f31fe40c8649eea7d4832a42243acaf0f1fff9083b2bed/argon2_cffi_bindings-21.2.0-cp36-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b746dba803a79238e925d9046a63aa26bf86ab2a2fe74ce6b009a1c3f5c8f2ae"},
     {url = "https://files.pythonhosted.org/packages/ed/55/f8ba268bc9005d0ca57a862e8f1b55bf1775e97a36bd30b0a8fb568c265c/argon2_cffi_bindings-21.2.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:5e00316dabdaea0b2dd82d141cc66889ced0cdcbfa599e8b471cf22c620c329a"},
     {url = "https://files.pythonhosted.org/packages/ee/0f/a2260a207f21ce2ff4cad00a417c31597f08eafb547e00615bcbf403d8ea/argon2_cffi_bindings-21.2.0-pp38-pypy38_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ed2937d286e2ad0cc79a7087d3c272832865f779430e0cc2b4f3718d3159b0cb"},
     {url = "https://files.pythonhosted.org/packages/f2/c6/e1ea7fc615ac7f9aaa4397e4ace245557d5bb25b4a594b06dccb2d90e05d/argon2_cffi_bindings-21.2.0-pp37-pypy37_pp73-macosx_10_9_x86_64.whl", hash = "sha256:3e385d1c39c520c08b53d63300c3ecc28622f076f4c2b0e6d7e796e9f6502194"},
     {url = "https://files.pythonhosted.org/packages/f4/64/bef937102280c7c92dd47dd9a67b6c76ef6a276f736c419ea538fa86adf8/argon2_cffi_bindings-21.2.0-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:93f9bf70084f97245ba10ee36575f0c3f1e7d7724d67d8e5b08e61787c320ed7"},
 ]
-"attrs 22.2.0" = [
-    {url = "https://files.pythonhosted.org/packages/21/31/3f468da74c7de4fcf9b25591e682856389b3400b4b62f201e65f15ea3e07/attrs-22.2.0.tar.gz", hash = "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"},
-    {url = "https://files.pythonhosted.org/packages/fb/6e/6f83bf616d2becdf333a1640f1d463fef3150e2e926b7010cb0f81c95e88/attrs-22.2.0-py3-none-any.whl", hash = "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836"},
+"attrs 23.1.0" = [
+    {url = "https://files.pythonhosted.org/packages/97/90/81f95d5f705be17872843536b1868f351805acf6971251ff07c1b8334dbb/attrs-23.1.0.tar.gz", hash = "sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015"},
+    {url = "https://files.pythonhosted.org/packages/f0/eb/fcb708c7bf5056045e9e98f62b93bd7467eb718b0202e7698eb11d66416c/attrs-23.1.0-py3-none-any.whl", hash = "sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04"},
 ]
 "backcall 0.2.0" = [
     {url = "https://files.pythonhosted.org/packages/4c/1c/ff6546b6c12603d8dd1070aa3c3d273ad4c07f5771689a7b69a550e8c951/backcall-0.2.0-py2.py3-none-any.whl", hash = "sha256:fbbce6a29f263178a1f7915c1940bde0ec2b2a967566fe1c65c1dfb7422bd255"},
     {url = "https://files.pythonhosted.org/packages/a2/40/764a663805d84deee23043e1426a9175567db89c8b3287b5c2ad9f71aa93/backcall-0.2.0.tar.gz", hash = "sha256:5cbdbf27be5e7cfadb448baf0aa95508f91f2bbc6c6437cd9cd06e2a4c215e1e"},
 ]
-"beautifulsoup4 4.11.1" = [
-    {url = "https://files.pythonhosted.org/packages/9c/d8/909c4089dbe4ade9f9705f143c9f13f065049a9d5e7d34c828aefdd0a97c/beautifulsoup4-4.11.1-py3-none-any.whl", hash = "sha256:58d5c3d29f5a36ffeb94f02f0d786cd53014cf9b3b3951d42e0080d8a9498d30"},
-    {url = "https://files.pythonhosted.org/packages/e8/b0/cd2b968000577ec5ce6c741a54d846dfa402372369b8b6861720aa9ecea7/beautifulsoup4-4.11.1.tar.gz", hash = "sha256:ad9aa55b65ef2808eb405f46cf74df7fcb7044d5cbc26487f96eb2ef2e436693"},
-]
-"black 22.12.0" = [
-    {url = "https://files.pythonhosted.org/packages/0c/51/1f7f93c0555eaf4cbb628e26ba026e3256174a45bd9397ff1ea7cf96bad5/black-22.12.0-py3-none-any.whl", hash = "sha256:436cc9167dd28040ad90d3b404aec22cedf24a6e4d7de221bec2730ec0c97bcf"},
-    {url = "https://files.pythonhosted.org/packages/4c/49/420dcfccba3215dc4e5790fa47572ef14129df1c5e95dd87b5ad30211b01/black-22.12.0-cp311-cp311-win_amd64.whl", hash = "sha256:7412e75863aa5c5411886804678b7d083c7c28421210180d67dfd8cf1221e1f4"},
-    {url = "https://files.pythonhosted.org/packages/4c/dd/cdb4e62a58e229ee757110a9dfb914a44e9d41be8becb41e085cb5df5d5b/black-22.12.0-cp38-cp38-win_amd64.whl", hash = "sha256:82d9fe8fee3401e02e79767016b4907820a7dc28d70d137eb397b92ef3cc5bfc"},
-    {url = "https://files.pythonhosted.org/packages/54/44/6d5f9af3c14da013754021e28eacc873e6ecbe877b2540e37346579398c8/black-22.12.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:77d86c9f3db9b1bf6761244bc0b3572a546f5fe37917a044e02f3166d5aafa7d"},
-    {url = "https://files.pythonhosted.org/packages/71/57/975782465cc6b514f2c972421e29b933dfbb51d4a95948a4e0e94f36ea38/black-22.12.0-cp310-cp310-win_amd64.whl", hash = "sha256:159a46a4947f73387b4d83e87ea006dbb2337eab6c879620a3ba52699b1f4351"},
-    {url = "https://files.pythonhosted.org/packages/79/d9/60852a6fc2f85374db20a9767dacfe50c2172eb8388f46018c8daf836995/black-22.12.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9eedd20838bd5d75b80c9f5487dbcb06836a43833a37846cf1d8c1cc01cef59d"},
-    {url = "https://files.pythonhosted.org/packages/a6/59/e873cc6807fb62c11131e5258ca15577a3b7452abad08dc49286cf8245e8/black-22.12.0.tar.gz", hash = "sha256:229351e5a18ca30f447bf724d007f890f97e13af070bb6ad4c0a441cd7596a2f"},
-    {url = "https://files.pythonhosted.org/packages/ba/32/954bcc56b2b3b4ef52a086e3c0bdbad88a38c9e739feb19dd2e6294cda42/black-22.12.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:101c69b23df9b44247bd88e1d7e90154336ac4992502d4197bdac35dd7ee3320"},
-    {url = "https://files.pythonhosted.org/packages/e9/e0/6aa02d14785c4039b38bfed6f9ee28a952b2d101c64fc97b15811fa8bd04/black-22.12.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d30b212bffeb1e252b31dd269dfae69dd17e06d92b87ad26e23890f3efea366f"},
-    {url = "https://files.pythonhosted.org/packages/eb/91/e0ccc36f8e1a00ed3c343741ca7ffe954e33cd2be0cada039845ff9e0539/black-22.12.0-cp37-cp37m-win_amd64.whl", hash = "sha256:1f58cbe16dfe8c12b7434e50ff889fa479072096d79f0a7f25e4ab8e94cd8350"},
-    {url = "https://files.pythonhosted.org/packages/f1/b7/6de002378cfe0b83beba72f0a7875dfb6005b2a214ac9f9ca689583069ef/black-22.12.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c116eed0efb9ff870ded8b62fe9f28dd61ef6e9ddd28d83d7d264a38417dcee2"},
-    {url = "https://files.pythonhosted.org/packages/f2/b9/06fe2dd83a2104d83c2b737f41aa5679f5a4395630005443ba4fa6fece8b/black-22.12.0-cp39-cp39-win_amd64.whl", hash = "sha256:559c7a1ba9a006226f09e4916060982fd27334ae1998e7a38b3f33a37f7a2148"},
-]
-"bleach 5.0.1" = [
-    {url = "https://files.pythonhosted.org/packages/c2/5d/d5d45a38163ede3342d6ac1ca01b5d387329daadf534a25718f9a9ba818c/bleach-5.0.1.tar.gz", hash = "sha256:0d03255c47eb9bd2f26aa9bb7f2107732e7e8fe195ca2f64709fcf3b0a4a085c"},
-    {url = "https://files.pythonhosted.org/packages/d4/87/508104336a2bc0c4cfdbdceedc0f44dc72da3abc0460c57e323ddd1b3257/bleach-5.0.1-py3-none-any.whl", hash = "sha256:085f7f33c15bd408dd9b17a4ad77c577db66d76203e5984b1bd59baeee948b2a"},
-]
-"certifi 2022.12.7" = [
-    {url = "https://files.pythonhosted.org/packages/37/f7/2b1b0ec44fdc30a3d31dfebe52226be9ddc40cd6c0f34ffc8923ba423b69/certifi-2022.12.7.tar.gz", hash = "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3"},
-    {url = "https://files.pythonhosted.org/packages/71/4c/3db2b8021bd6f2f0ceb0e088d6b2d49147671f25832fb17970e9b583d742/certifi-2022.12.7-py3-none-any.whl", hash = "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"},
+"beautifulsoup4 4.12.2" = [
+    {url = "https://files.pythonhosted.org/packages/57/f4/a69c20ee4f660081a7dedb1ac57f29be9378e04edfcb90c526b923d4bebc/beautifulsoup4-4.12.2-py3-none-any.whl", hash = "sha256:bd2520ca0d9d7d12694a53d44ac482d181b4ec1888909b035a3dbf40d0f57d4a"},
+    {url = "https://files.pythonhosted.org/packages/af/0b/44c39cf3b18a9280950ad63a579ce395dda4c32193ee9da7ff0aed547094/beautifulsoup4-4.12.2.tar.gz", hash = "sha256:492bbc69dca35d12daac71c4db1bfff0c876c00ef4a2ffacce226d4638eb72da"},
+]
+"black 23.3.0" = [
+    {url = "https://files.pythonhosted.org/packages/06/1e/273d610249f0335afb1ddb03664a03223f4826e3d1a95170a0142cb19fb4/black-23.3.0-cp39-cp39-win_amd64.whl", hash = "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb"},
+    {url = "https://files.pythonhosted.org/packages/12/4b/99c71d1cf1353edd5aff2700b8960f92e9b805c9dab72639b67dbb449d3a/black-23.3.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961"},
+    {url = "https://files.pythonhosted.org/packages/13/0a/ed8b66c299e896780e4528eed4018f5b084da3b9ba4ee48328550567d866/black-23.3.0-cp38-cp38-macosx_10_16_x86_64.whl", hash = "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5"},
+    {url = "https://files.pythonhosted.org/packages/13/25/cfa06788d0a936f2445af88f13604b5bcd5c9d050db618c718e6ebe66f74/black-23.3.0-cp39-cp39-macosx_10_16_arm64.whl", hash = "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30"},
+    {url = "https://files.pythonhosted.org/packages/21/14/d5a2bec5fb15f9118baab7123d344646fac0b1c6939d51c2b05259cd2d9c/black-23.3.0-cp38-cp38-macosx_10_16_universal2.whl", hash = "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331"},
+    {url = "https://files.pythonhosted.org/packages/24/eb/2d2d2c27cb64cfd073896f62a952a802cd83cf943a692a2f278525b57ca9/black-23.3.0-cp37-cp37m-macosx_10_16_x86_64.whl", hash = "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b"},
+    {url = "https://files.pythonhosted.org/packages/27/70/07aab2623cfd3789786f17e051487a41d5657258c7b1ef8f780512ffea9c/black-23.3.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9"},
+    {url = "https://files.pythonhosted.org/packages/29/b1/b584fc863c155653963039664a592b3327b002405043b7e761b9b0212337/black-23.3.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2"},
+    {url = "https://files.pythonhosted.org/packages/3c/d7/85f3d79f9e543402de2244c4d117793f262149e404ea0168841613c33e07/black-23.3.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab"},
+    {url = "https://files.pythonhosted.org/packages/3f/0d/81dd4194ce7057c199d4f28e4c2a885082d9d929e7a55c514b23784f7787/black-23.3.0-cp311-cp311-win_amd64.whl", hash = "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326"},
+    {url = "https://files.pythonhosted.org/packages/49/36/15d2122f90ff1cd70f06892ebda777b650218cf84b56b5916a993dc1359a/black-23.3.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2"},
+    {url = "https://files.pythonhosted.org/packages/49/d7/f3b7da6c772800f5375aeb050a3dcf682f0bbeb41d313c9c2820d0156e4e/black-23.3.0-cp39-cp39-macosx_10_16_x86_64.whl", hash = "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266"},
+    {url = "https://files.pythonhosted.org/packages/69/49/7e1f0cf585b0d607aad3f971f95982cc4208fc77f92363d632d23021ee57/black-23.3.0-cp311-cp311-macosx_10_16_x86_64.whl", hash = "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d"},
+    {url = "https://files.pythonhosted.org/packages/6d/b4/0f13ab7f5e364795ff82b76b0f9a4c9c50afda6f1e2feeb8b03fdd7ec57d/black-23.3.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c"},
+    {url = "https://files.pythonhosted.org/packages/ad/e7/4642b7f462381799393fbad894ba4b32db00870a797f0616c197b07129a9/black-23.3.0-py3-none-any.whl", hash = "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4"},
+    {url = "https://files.pythonhosted.org/packages/c0/53/42e312c17cfda5c8fc4b6b396a508218807a3fcbb963b318e49d3ddd11d5/black-23.3.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70"},
+    {url = "https://files.pythonhosted.org/packages/ca/44/eb41edd3f558a6139f09eee052dead4a7a464e563b822ddf236f5a8ee286/black-23.3.0-cp37-cp37m-win_amd64.whl", hash = "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925"},
+    {url = "https://files.pythonhosted.org/packages/ce/f4/2b0c6ac9e1f8584296747f66dd511898b4ebd51d6510dba118279bff53b6/black-23.3.0-cp38-cp38-macosx_10_16_arm64.whl", hash = "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27"},
+    {url = "https://files.pythonhosted.org/packages/d1/6e/5810b6992ed70403124c67e8b3f62858a32b35405177553f1a78ed6b6e31/black-23.3.0-cp38-cp38-win_amd64.whl", hash = "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8"},
+    {url = "https://files.pythonhosted.org/packages/d6/36/66370f5017b100225ec4950a60caeef60201a10080da57ddb24124453fba/black-23.3.0.tar.gz", hash = "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940"},
+    {url = "https://files.pythonhosted.org/packages/d7/6f/d3832960a3b646b333b7f0d80d336a3c123012e9d9d5dba4a622b2b6181d/black-23.3.0-cp311-cp311-macosx_10_16_arm64.whl", hash = "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6"},
+    {url = "https://files.pythonhosted.org/packages/db/f4/7908f71cc71da08df1317a3619f002cbf91927fb5d3ffc7723905a2113f7/black-23.3.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915"},
+    {url = "https://files.pythonhosted.org/packages/de/b4/76f152c5eb0be5471c22cd18380d31d188930377a1a57969073b89d6615d/black-23.3.0-cp310-cp310-win_amd64.whl", hash = "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c"},
+    {url = "https://files.pythonhosted.org/packages/eb/a5/17b40bfd9b607b69fa726b0b3a473d14b093dcd5191ea1a1dd664eccfee3/black-23.3.0-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b"},
+    {url = "https://files.pythonhosted.org/packages/fd/5b/fc2d7922c1a6bb49458d424b5be71d251f2d0dc97be9534e35d171bdc653/black-23.3.0-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"},
+]
+"bleach 6.0.0" = [
+    {url = "https://files.pythonhosted.org/packages/7e/e6/d5f220ca638f6a25557a611860482cb6e54b2d97f0332966b1b005742e1f/bleach-6.0.0.tar.gz", hash = "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414"},
+    {url = "https://files.pythonhosted.org/packages/ac/e2/dfcab68c9b2e7800c8f06b85c76e5f978d05b195a958daa9b1dda54a1db6/bleach-6.0.0-py3-none-any.whl", hash = "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"},
+]
+"certifi 2023.5.7" = [
+    {url = "https://files.pythonhosted.org/packages/93/71/752f7a4dd4c20d6b12341ed1732368546bc0ca9866139fe812f6009d9ac7/certifi-2023.5.7.tar.gz", hash = "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7"},
+    {url = "https://files.pythonhosted.org/packages/9d/19/59961b522e6757f0c9097e4493fa906031b95b3ebe9360b2c3083561a6b4/certifi-2023.5.7-py3-none-any.whl", hash = "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"},
 ]
 "cffi 1.15.1" = [
     {url = "https://files.pythonhosted.org/packages/00/05/23a265a3db411b0bfb721bf7a116c7cecaf3eb37ebd48a6ea4dfb0a3244d/cffi-1.15.1-cp27-cp27m-win_amd64.whl", hash = "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e"},
     {url = "https://files.pythonhosted.org/packages/03/7b/259d6e01a6083acef9d3c8c88990c97d313632bb28fa84d6ab2bb201140a/cffi-1.15.1-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405"},
     {url = "https://files.pythonhosted.org/packages/0e/65/0d7b5dad821ced4dcd43f96a362905a68ce71e6b5f5cfd2fada867840582/cffi-1.15.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e"},
     {url = "https://files.pythonhosted.org/packages/0e/e2/a23af3d81838c577571da4ff01b799b0c2bbde24bd924d97e228febae810/cffi-1.15.1-cp310-cp310-win_amd64.whl", hash = "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d"},
     {url = "https://files.pythonhosted.org/packages/10/72/617ee266192223a38b67149c830bd9376b69cf3551e1477abc72ff23ef8e/cffi-1.15.1-cp311-cp311-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9"},
@@ -1142,141 +1152,150 @@
     {url = "https://files.pythonhosted.org/packages/59/87/84326af34517fca8c58418d148f2403df25303e02736832403587318e9e8/click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
     {url = "https://files.pythonhosted.org/packages/c2/f1/df59e28c642d583f7dacffb1e0965d0e00b218e0186d7858ac5233dce840/click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
 ]
 "colorama 0.4.6" = [
     {url = "https://files.pythonhosted.org/packages/d1/d6/3965ed04c63042e047cb6a3e6ed1a63a35087b6a609aa3a15ed8ac56c221/colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {url = "https://files.pythonhosted.org/packages/d8/53/6f443c9a4a8358a93a6792e2acffb9d9d5cb0a5cfd8802644b7b1c9a02e4/colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
-"coverage 7.0.5" = [
-    {url = "https://files.pythonhosted.org/packages/01/01/8d17427fbeb0ee132111c543bfeea5ab403d6869812cf6085adc18debecf/coverage-7.0.5-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a9fed35ca8c6e946e877893bbac022e8563b94404a605af1d1e6accc7eb73289"},
-    {url = "https://files.pythonhosted.org/packages/02/d6/c095845877f235b52a7113e08e750a9210feabf059b71133e9349eccb836/coverage-7.0.5-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:95304068686545aa368b35dfda1cdfbbdbe2f6fe43de4a2e9baa8ebd71be46e2"},
-    {url = "https://files.pythonhosted.org/packages/03/ba/da1510983720f5196f4c8fe01489b6ce9c4fa661fe9aa9375611e639a8d7/coverage-7.0.5-cp37-cp37m-win32.whl", hash = "sha256:d8f3e2e0a1d6777e58e834fd5a04657f66affa615dae61dd67c35d1568c38882"},
-    {url = "https://files.pythonhosted.org/packages/06/45/d201ad5b5b7e44764769421fcd1a9cbb0fa3fc7bb4020d83f955e2a6fb2d/coverage-7.0.5-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ea76dbcad0b7b0deb265d8c36e0801abcddf6cc1395940a24e3595288b405ca0"},
-    {url = "https://files.pythonhosted.org/packages/0b/0c/c1f48457a7df79c53299d56e1632d1907cc8548fe158b2c839ad8e456584/coverage-7.0.5-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b8c56bec53d6e3154eaff6ea941226e7bd7cc0d99f9b3756c2520fc7a94e6d96"},
-    {url = "https://files.pythonhosted.org/packages/13/31/f4b97b92913e6dbffc11e1e575e01eb8fff7abaaf4b38b11208ecc362207/coverage-7.0.5-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d66187792bfe56f8c18ba986a0e4ae44856b1c645336bd2c776e3386da91e1dd"},
-    {url = "https://files.pythonhosted.org/packages/16/4b/25fffab188056faf56071b38b72e8e5ae74c7f7f5f8302a764f9f915512c/coverage-7.0.5-cp39-cp39-win_amd64.whl", hash = "sha256:949844af60ee96a376aac1ded2a27e134b8c8d35cc006a52903fc06c24a3296f"},
-    {url = "https://files.pythonhosted.org/packages/1d/87/65a9ac379bd840950efd5d69cf97584a4f21ef939c3d05a74edbd308aa2b/coverage-7.0.5-pp37.pp38.pp39-none-any.whl", hash = "sha256:b9727ac4f5cf2cbf87880a63870b5b9730a8ae3a4a360241a0fdaa2f71240ff0"},
-    {url = "https://files.pythonhosted.org/packages/28/7c/7574b64b81d1be6fe5fb5ce9364a6c82507d474678d44c2bd69b7f40ffe9/coverage-7.0.5-cp38-cp38-win_amd64.whl", hash = "sha256:4a950f83fd3f9bca23b77442f3a2b2ea4ac900944d8af9993743774c4fdc57af"},
-    {url = "https://files.pythonhosted.org/packages/29/1e/6cbbb64032ba687cc88f719556e63bb28555807ecbdf8aaedaff2e535f54/coverage-7.0.5-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:220e3fa77d14c8a507b2d951e463b57a1f7810a6443a26f9b7591ef39047b1b2"},
-    {url = "https://files.pythonhosted.org/packages/35/51/0dd2e96c0f2cbd08fca3277ab61728e9fa1e30b4a6fbf64ec112b86ac090/coverage-7.0.5-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:50a6adc2be8edd7ee67d1abc3cd20678987c7b9d79cd265de55941e3d0d56499"},
-    {url = "https://files.pythonhosted.org/packages/39/ee/06bf06e1670678934b60c818ce295dea7b9c361e1adc72b4651e933f959a/coverage-7.0.5-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:276f4cd0001cd83b00817c8db76730938b1ee40f4993b6a905f40a7278103b3a"},
-    {url = "https://files.pythonhosted.org/packages/3e/fc/80617dba15621700e9fee56ced5f728376a6f853e1e32181b63f64c0888a/coverage-7.0.5-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3c2155943896ac78b9b0fd910fb381186d0c345911f5333ee46ac44c8f0e43ab"},
-    {url = "https://files.pythonhosted.org/packages/4c/f1/c8c99bb9902df7a01ac80ca850a0fbf2c5d2bf25755841ffdb5d72c1b068/coverage-7.0.5-cp310-cp310-win32.whl", hash = "sha256:be9fcf32c010da0ba40bf4ee01889d6c737658f4ddff160bd7eb9cac8f094b21"},
-    {url = "https://files.pythonhosted.org/packages/53/6c/d206426bd4896df14f88581e47198e509a376f50e3ced18bce75f31aabb5/coverage-7.0.5-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:1caed2367b32cc80a2b7f58a9f46658218a19c6cfe5bc234021966dc3daa01f0"},
-    {url = "https://files.pythonhosted.org/packages/59/95/22de7c62c8e24b17cc5c337a0523e5e9c8cf63b0e8e10e3628863681875a/coverage-7.0.5-cp38-cp38-win32.whl", hash = "sha256:e4ce984133b888cc3a46867c8b4372c7dee9cee300335e2925e197bcd45b9e16"},
-    {url = "https://files.pythonhosted.org/packages/5a/79/7acd51daffd3e53f8a6f2f43543f686b46c206e6f36e2203ca2ca15d72ec/coverage-7.0.5-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:2a7f23bbaeb2a87f90f607730b45564076d870f1fb07b9318d0c21f36871932b"},
-    {url = "https://files.pythonhosted.org/packages/63/74/a65dc4de105d34240d7c46c246371471d64b5b163d1503f29108f1297a4d/coverage-7.0.5-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:66e50680e888840c0995f2ad766e726ce71ca682e3c5f4eee82272c7671d38a2"},
-    {url = "https://files.pythonhosted.org/packages/66/c9/08ed37cdf2101a6832dfe99307fdbf6d9d5abc2070105ee061b7385a1f80/coverage-7.0.5-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:17e01dd8666c445025c29684d4aabf5a90dc6ef1ab25328aa52bedaa95b65ad7"},
-    {url = "https://files.pythonhosted.org/packages/6c/f4/4f4011153af468e75f9f4708953daf56c6945b3f0bf3fb813d9747f3eefa/coverage-7.0.5-cp311-cp311-win_amd64.whl", hash = "sha256:1f66862d3a41674ebd8d1a7b6f5387fe5ce353f8719040a986551a545d7d83ea"},
-    {url = "https://files.pythonhosted.org/packages/71/56/29e6648e9c0542602d0989c4848e605a6e2b98af79c454b6fd1f14ed03ee/coverage-7.0.5-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:790e4433962c9f454e213b21b0fd4b42310ade9c077e8edcb5113db0818450cb"},
-    {url = "https://files.pythonhosted.org/packages/71/5e/55d1d143327306f793fce0cb34b2a4ab0d5a1559d632ca5e327a9f9bb848/coverage-7.0.5-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:d8d04e755934195bdc1db45ba9e040b8d20d046d04d6d77e71b3b34a8cc002d0"},
-    {url = "https://files.pythonhosted.org/packages/7a/a8/3b985e615a9a5c255ab2782aec1259e1dc5bce82bda76459d16e0795ce33/coverage-7.0.5-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:436e103950d05b7d7f55e39beeb4d5be298ca3e119e0589c0227e6d0b01ee8c7"},
-    {url = "https://files.pythonhosted.org/packages/7c/08/6e8508b6fdad45895daf46cf37a27e043e1162e1353b4f8940987bdaee1d/coverage-7.0.5-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ef14d75d86f104f03dea66c13188487151760ef25dd6b2dbd541885185f05f40"},
-    {url = "https://files.pythonhosted.org/packages/82/9c/ad0cd77d84de4e561c77905a735397f27abee1a526ca715d2ec7759047ae/coverage-7.0.5-cp37-cp37m-win_amd64.whl", hash = "sha256:9e662e6fc4f513b79da5d10a23edd2b87685815b337b1a30cd11307a6679148d"},
-    {url = "https://files.pythonhosted.org/packages/84/b3/992a6b222b14c99e6d4aa9f448c670a5f614648597499de6ddc11be839e3/coverage-7.0.5.tar.gz", hash = "sha256:051afcbd6d2ac39298d62d340f94dbb6a1f31de06dfaf6fcef7b759dd3860c45"},
-    {url = "https://files.pythonhosted.org/packages/87/f7/6259d91f3b3a0c38337e99b85a10ebfd3e1a15273452cee72151b281e57d/coverage-7.0.5-cp310-cp310-win_amd64.whl", hash = "sha256:cbfcba14a3225b055a28b3199c3d81cd0ab37d2353ffd7f6fd64844cebab31ad"},
-    {url = "https://files.pythonhosted.org/packages/88/88/1bfb18b78f068ffae4c87cb39b0351e6709ce9a655cfe6b0a7e397b669f8/coverage-7.0.5-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:30b5fec1d34cc932c1bc04017b538ce16bf84e239378b8f75220478645d11fca"},
-    {url = "https://files.pythonhosted.org/packages/8b/e4/ca474e48fe69f2307cf9f2bb775a86130fad765b38ba9b402469d44b7893/coverage-7.0.5-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:ecb0f73954892f98611e183f50acdc9e21a4653f294dfbe079da73c6378a6f47"},
-    {url = "https://files.pythonhosted.org/packages/9b/38/b407288f8142c3b14c3f36a145d1380e5750781b22997eb1b659f194b093/coverage-7.0.5-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:13250b1f0bd023e0c9f11838bdeb60214dd5b6aaf8e8d2f110c7e232a1bff83b"},
-    {url = "https://files.pythonhosted.org/packages/a4/3c/662aa204ff721bbad7321908013fca51ed6b64ae24e94c699f0789528111/coverage-7.0.5-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7b05ed4b35bf6ee790832f68932baf1f00caa32283d66cc4d455c9e9d115aafc"},
-    {url = "https://files.pythonhosted.org/packages/a4/dc/3671f11710feeb83fda4b2b7a70262c6bf7e32f8a43c31fa33b5d83bac0a/coverage-7.0.5-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:e057e74e53db78122a3979f908973e171909a58ac20df05c33998d52e6d35757"},
-    {url = "https://files.pythonhosted.org/packages/a5/da/f340fca24231ca2ac91807d2ea3596be6d4effab7b870c74949b9a92dbeb/coverage-7.0.5-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:54f7e9705e14b2c9f6abdeb127c390f679f6dbe64ba732788d3015f7f76ef637"},
-    {url = "https://files.pythonhosted.org/packages/a7/15/bbea207f612ba112536bcf7a4c57529738f11fcf41b307d62459ec788ca5/coverage-7.0.5-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:f26648e1b3b03b6022b48a9b910d0ae209e2d51f50441db5dce5b530fad6d9b1"},
-    {url = "https://files.pythonhosted.org/packages/a8/96/e88aeefcf6aa03996a685f0dd61100a0b6ffa0e371f8a3089827595c9913/coverage-7.0.5-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7a38362528a9115a4e276e65eeabf67dcfaf57698e17ae388599568a78dcb029"},
-    {url = "https://files.pythonhosted.org/packages/a8/98/e0308655f42fa5b1daf3574c79c32628936ed6fa11d8e8f3b970d185220a/coverage-7.0.5-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:29de916ba1099ba2aab76aca101580006adfac5646de9b7c010a0f13867cba45"},
-    {url = "https://files.pythonhosted.org/packages/ac/9a/5a0e4c17f105eb04caa7cd4e524a734badb6198c36617ac124002a68aa3b/coverage-7.0.5-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0ee30375b409d9a7ea0f30c50645d436b6f5dfee254edffd27e45a980ad2c7f4"},
-    {url = "https://files.pythonhosted.org/packages/b6/e0/1b5b5bf33eaba010395864415aaa5c036a3fb10780cc2c92b3a8e51f035b/coverage-7.0.5-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:7e109f1c9a3ece676597831874126555997c48f62bddbcace6ed17be3e372de8"},
-    {url = "https://files.pythonhosted.org/packages/b7/fc/7deab9d5d5af9d9ac360922d088250a644a2a2d0627d70a2043b76c260cc/coverage-7.0.5-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:2c407b1950b2d2ffa091f4e225ca19a66a9bd81222f27c56bd12658fc5ca1209"},
-    {url = "https://files.pythonhosted.org/packages/c0/7f/7875a6e6a2522e8b7bc683be78714badd4ac8b3d90b69fc2cadc20ca4d52/coverage-7.0.5-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:0a1890fca2962c4f1ad16551d660b46ea77291fba2cc21c024cd527b9d9c8809"},
-    {url = "https://files.pythonhosted.org/packages/c2/46/fb2e5ea06f34fbefc6d56a49508865c0d8268a7fa4645313d3a176a41161/coverage-7.0.5-cp39-cp39-win32.whl", hash = "sha256:ba3027deb7abf02859aca49c865ece538aee56dcb4871b4cced23ba4d5088904"},
-    {url = "https://files.pythonhosted.org/packages/c2/c1/daf9e61cb35b8c5b781f94b85941fbbc233502f3dfda864d83f4c677391b/coverage-7.0.5-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:c76a3075e96b9c9ff00df8b5f7f560f5634dffd1658bafb79eb2682867e94f78"},
-    {url = "https://files.pythonhosted.org/packages/c6/81/e01309e5ba812a767bfd3ef692a619ee459af4d9313e7244305561aa2341/coverage-7.0.5-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d254666d29540a72d17cc0175746cfb03d5123db33e67d1020e42dae611dc196"},
-    {url = "https://files.pythonhosted.org/packages/c7/47/39dda27c8eb0729762ccd3e9ca83d2b7a6e748872cc29533fae832d929a9/coverage-7.0.5-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:b69522b168a6b64edf0c33ba53eac491c0a8f5cc94fa4337f9c6f4c8f2f5296c"},
-    {url = "https://files.pythonhosted.org/packages/c8/f1/701995cc6a65dbc57b6cfcd60e4d2358735c6fcec877bd8f85963eb0c48d/coverage-7.0.5-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:f67472c09a0c7486e27f3275f617c964d25e35727af952869dd496b9b5b7f6a3"},
-    {url = "https://files.pythonhosted.org/packages/cc/55/40719c5b7b7503144ffcf55ead8d37c6e8ec2269293a11c5d7654caa5228/coverage-7.0.5-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:19245c249aa711d954623d94f23cc94c0fd65865661f20b7781210cb97c471c0"},
-    {url = "https://files.pythonhosted.org/packages/d0/eb/52b1585f1da59f25a2d0ef79988795fa46ab99b48d44df2e38e99c725a63/coverage-7.0.5-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:49640bda9bda35b057b0e65b7c43ba706fa2335c9a9896652aebe0fa399e80e6"},
-    {url = "https://files.pythonhosted.org/packages/ea/fe/5116a0d06a3f6b61d5f147e7d968cdd472b4213f497e3d600afea3ea2f1c/coverage-7.0.5-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:c18d47f314b950dbf24a41787ced1474e01ca816011925976d90a88b27c22b89"},
-    {url = "https://files.pythonhosted.org/packages/ed/38/150ae9c3ee2f9544a1c1c50a78c98364d4e6ce9025cd647b739ec3b776b7/coverage-7.0.5-cp311-cp311-win32.whl", hash = "sha256:52ab14b9e09ce052237dfe12d6892dd39b0401690856bcfe75d5baba4bfe2831"},
-    {url = "https://files.pythonhosted.org/packages/ed/75/fa4b613e2d4d8b0773ac21061cedd29a7a158ab9139c932011fdafc0cbc3/coverage-7.0.5-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:411d4ff9d041be08fdfc02adf62e89c735b9468f6d8f6427f8a14b6bb0a85095"},
-    {url = "https://files.pythonhosted.org/packages/ff/ff/cfb9b03d3673d24aae2a40397d812cde590e36f5e4aad3efa946910965c3/coverage-7.0.5-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b78729038abea6a5df0d2708dce21e82073463b2d79d10884d7d591e0f385ded"},
-]
-"debugpy 1.6.5" = [
-    {url = "https://files.pythonhosted.org/packages/01/d1/ca25645259d56eae64a4b4d330072b5aa8145cfb8cdcae50c1096a0ef826/debugpy-1.6.5-cp39-cp39-win32.whl", hash = "sha256:15bc5febe0edc79726517b1f8d57d7ac7c784567b5ba804aab8b1c9d07a57018"},
-    {url = "https://files.pythonhosted.org/packages/09/ae/b1cf75c44fd09570be433e481628fb7cc1c13715b5ce181d93197287ec25/debugpy-1.6.5-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:947c686e8adb46726f3d5f19854f6aebf66c2edb91225643c7f44b40b064a235"},
-    {url = "https://files.pythonhosted.org/packages/22/9a/610d08048464ac9a39238a9b07312052e3e6a1f6b6f2c6aa9e8daa6a7e68/debugpy-1.6.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8f3fab217fe7e2acb2d90732af1a871947def4e2b6654945ba1ebd94bd0bea26"},
-    {url = "https://files.pythonhosted.org/packages/27/bf/5fb58a315f33860448ebe6481ec6bf15d67fe783e1f80f6c0868fa284f4d/debugpy-1.6.5.zip", hash = "sha256:5e55e6c79e215239dd0794ee0bf655412b934735a58e9d705e5c544f596f1603"},
-    {url = "https://files.pythonhosted.org/packages/2b/65/d696eabc4f9e2b0e8704cbbd88d96327c16dfe134c6286b5f57ce388ba11/debugpy-1.6.5-cp310-cp310-win32.whl", hash = "sha256:62a06eb78378292ba6c427d861246574dc8b84471904973797b29dd33c7c2495"},
-    {url = "https://files.pythonhosted.org/packages/31/12/3304fea2f4b3a241fe60ee6459cc16f2e7b7ef1a197669106dc416053bc9/debugpy-1.6.5-cp39-cp39-win_amd64.whl", hash = "sha256:7e84d9e4420122384cb2cc762a00b4e17cbf998022890f89b195ce178f78ff47"},
-    {url = "https://files.pythonhosted.org/packages/3e/14/b96f86b17d1faaf61259ad01ff7d4e6b390d7de30fb074ef12e519cffd7c/debugpy-1.6.5-cp310-cp310-win_amd64.whl", hash = "sha256:9984fc00ab372c97f63786c400107f54224663ea293daab7b365a5b821d26309"},
-    {url = "https://files.pythonhosted.org/packages/4a/2a/1b7b12e720feea3e423c6f4f393e2fe4a872302265e34840534e4162d132/debugpy-1.6.5-cp38-cp38-win32.whl", hash = "sha256:377391341c4b86f403d93e467da8e2d05c22b683f08f9af3e16d980165b06b90"},
-    {url = "https://files.pythonhosted.org/packages/74/1c/6ee0a088c450f85654ae6e2b4b6f6175c2d626d3d14f2f325dc5138c1ff0/debugpy-1.6.5-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:500dd4a9ff818f5c52dddb4a608c7de5371c2d7d905c505eb745556c579a9f11"},
-    {url = "https://files.pythonhosted.org/packages/7a/59/c92fbbc9065fd907a3a2ddf67cbc846d73240a0c90eeb12cf69eacde5f1b/debugpy-1.6.5-cp37-cp37m-win_amd64.whl", hash = "sha256:b5a74ecebe5253344501d9b23f74459c46428b30437fa9254cfb8cb129943242"},
-    {url = "https://files.pythonhosted.org/packages/8a/02/a0d2c426729faf8c136a65c01fff638412b6c29d67b9a654a670445a87a2/debugpy-1.6.5-cp38-cp38-macosx_10_15_x86_64.whl", hash = "sha256:9e809ef787802c808995e5b6ade714a25fa187f892b41a412d418a15a9c4a432"},
-    {url = "https://files.pythonhosted.org/packages/8a/92/1cbba7515b8872e72d230a6b0784ff845767355a73fe9678e25ddd08a077/debugpy-1.6.5-cp37-cp37m-macosx_10_15_x86_64.whl", hash = "sha256:048368f121c08b00bbded161e8583817af5055982d2722450a69efe2051621c2"},
-    {url = "https://files.pythonhosted.org/packages/92/d5/b0f9b31b5fc902aa1611d0163652713b21661201f7008051fd5e512e851b/debugpy-1.6.5-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:17039e392d6f38388a68bd02c5f823b32a92142a851e96ba3ec52aeb1ce9d900"},
-    {url = "https://files.pythonhosted.org/packages/b6/75/67d59b76830c44527167008dde863b51c4c671d8ec23b6b61205bf383b28/debugpy-1.6.5-py2.py3-none-any.whl", hash = "sha256:8116e40a1cd0593bd2aba01d4d560ee08f018da8e8fbd4cbd24ff09b5f0e41ef"},
-    {url = "https://files.pythonhosted.org/packages/bb/51/01bb919203098f303a2e1fd17c6de6cc3baaa8519a90e41c5651134fbc18/debugpy-1.6.5-cp37-cp37m-win32.whl", hash = "sha256:0f9afcc8cad6424695f3356dc9a7406d5b18e37ee2e73f34792881a44b02cc50"},
-    {url = "https://files.pythonhosted.org/packages/bf/ca/b2a54608a5ab21fc9e0afa4d78f2e45c193f8147969c27d790666ed4a282/debugpy-1.6.5-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:696165f021a6a17da08163eaae84f3faf5d8be68fb78cd78488dd347e625279c"},
-    {url = "https://files.pythonhosted.org/packages/e5/de/155f5b533624f9e304c7f742d2fa4f456dd504016a27ebb8cb1d302f4b77/debugpy-1.6.5-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:74e4eca42055759032e3f1909d1374ba1d729143e0c2729bb8cb5e8b5807c458"},
-    {url = "https://files.pythonhosted.org/packages/f4/25/8d21b8a3346e4537a908040a63089cf788b9a009ac4e32ec7aaed343af08/debugpy-1.6.5-cp38-cp38-win_amd64.whl", hash = "sha256:286ae0c2def18ee0dc8a61fa76d51039ca8c11485b6ed3ef83e3efe8a23926ae"},
+"coverage 7.2.7" = [
+    {url = "https://files.pythonhosted.org/packages/01/24/be01e62a7bce89bcffe04729c540382caa5a06bee45ae42136c93e2499f5/coverage-7.2.7-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8"},
+    {url = "https://files.pythonhosted.org/packages/03/ec/6f30b4e0c96ce03b0e64aec46b4af2a8c49b70d1b5d0d69577add757b946/coverage-7.2.7-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a"},
+    {url = "https://files.pythonhosted.org/packages/04/d6/8cba3bf346e8b1a4fb3f084df7d8cea25a6b6c56aaca1f2e53829be17e9e/coverage-7.2.7-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d"},
+    {url = "https://files.pythonhosted.org/packages/04/fa/43b55101f75a5e9115259e8be70ff9279921cb6b17f04c34a5702ff9b1f7/coverage-7.2.7-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97"},
+    {url = "https://files.pythonhosted.org/packages/0d/31/340428c238eb506feb96d4fb5c9ea614db1149517f22cc7ab8c6035ef6d9/coverage-7.2.7-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050"},
+    {url = "https://files.pythonhosted.org/packages/0e/bc/7e3a31534fabb043269f14fb64e2bb2733f85d4cf39e5bbc71357c57553a/coverage-7.2.7-cp37-cp37m-win_amd64.whl", hash = "sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0"},
+    {url = "https://files.pythonhosted.org/packages/15/81/b108a60bc758b448c151e5abceed027ed77a9523ecbc6b8a390938301841/coverage-7.2.7-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01"},
+    {url = "https://files.pythonhosted.org/packages/1f/e9/d6730247d8dec2a3dddc520ebe11e2e860f0f98cee3639e23de6cf920255/coverage-7.2.7-cp310-cp310-win_amd64.whl", hash = "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850"},
+    {url = "https://files.pythonhosted.org/packages/22/c1/2f6c1b6f01a0996c9e067a9c780e1824351dbe17faae54388a4477e6d86f/coverage-7.2.7-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959"},
+    {url = "https://files.pythonhosted.org/packages/24/df/6765898d54ea20e3197a26d26bb65b084deefadd77ce7de946b9c96dfdc5/coverage-7.2.7-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4"},
+    {url = "https://files.pythonhosted.org/packages/28/d7/9a8de57d87f4bbc6f9a6a5ded1eaac88a89bf71369bb935dac3c0cf2893e/coverage-7.2.7-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5"},
+    {url = "https://files.pythonhosted.org/packages/29/8f/4fad1c2ba98104425009efd7eaa19af9a7c797e92d40cd2ec026fa1f58cb/coverage-7.2.7-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495"},
+    {url = "https://files.pythonhosted.org/packages/2b/86/3dbf9be43f8bf6a5ca28790a713e18902b2d884bc5fa9512823a81dff601/coverage-7.2.7-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1"},
+    {url = "https://files.pythonhosted.org/packages/3d/80/7060a445e1d2c9744b683dc935248613355657809d6c6b2716cdf4ca4766/coverage-7.2.7-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb"},
+    {url = "https://files.pythonhosted.org/packages/44/55/49f65ccdd4dfd6d5528e966b28c37caec64170c725af32ab312889d2f857/coverage-7.2.7-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e"},
+    {url = "https://files.pythonhosted.org/packages/45/8b/421f30467e69ac0e414214856798d4bc32da1336df745e49e49ae5c1e2a8/coverage-7.2.7.tar.gz", hash = "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59"},
+    {url = "https://files.pythonhosted.org/packages/4a/fb/78986d3022e5ccf2d4370bc43a5fef8374f092b3c21d32499dee8e30b7b6/coverage-7.2.7-cp38-cp38-win32.whl", hash = "sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e"},
+    {url = "https://files.pythonhosted.org/packages/61/90/c76b9462f39897ebd8714faf21bc985b65c4e1ea6dff428ea9dc711ed0dd/coverage-7.2.7-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6"},
+    {url = "https://files.pythonhosted.org/packages/61/af/5964b8d7d9a5c767785644d9a5a63cacba9a9c45cc42ba06d25895ec87be/coverage-7.2.7-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7"},
+    {url = "https://files.pythonhosted.org/packages/66/2e/c99fe1f6396d93551aa352c75410686e726cd4ea104479b9af1af22367ce/coverage-7.2.7-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250"},
+    {url = "https://files.pythonhosted.org/packages/67/a2/6fa66a50e6e894286d79a3564f42bd54a9bd27049dc0a63b26d9924f0aa3/coverage-7.2.7-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9"},
+    {url = "https://files.pythonhosted.org/packages/67/d7/cd8fe689b5743fffac516597a1222834c42b80686b99f5b44ef43ccc2a43/coverage-7.2.7-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe"},
+    {url = "https://files.pythonhosted.org/packages/67/fb/b3b1d7887e1ea25a9608b0776e480e4bbc303ca95a31fd585555ec4fff5a/coverage-7.2.7-pp37.pp38.pp39-none-any.whl", hash = "sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d"},
+    {url = "https://files.pythonhosted.org/packages/68/5f/d2bd0f02aa3c3e0311986e625ccf97fdc511b52f4f1a063e4f37b624772f/coverage-7.2.7-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a"},
+    {url = "https://files.pythonhosted.org/packages/69/8c/26a95b08059db1cbb01e4b0e6d40f2e9debb628c6ca86b78f625ceaf9bab/coverage-7.2.7-cp312-cp312-win32.whl", hash = "sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511"},
+    {url = "https://files.pythonhosted.org/packages/6e/ea/4a252dc77ca0605b23d477729d139915e753ee89e4c9507630e12ad64a80/coverage-7.2.7-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de"},
+    {url = "https://files.pythonhosted.org/packages/7a/05/084864fa4bbf8106f44fb72a56e67e0cd372d3bf9d893be818338c81af5d/coverage-7.2.7-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb"},
+    {url = "https://files.pythonhosted.org/packages/7b/e3/f552d5871943f747165b92a924055c5d6daa164ae659a13f9018e22f3990/coverage-7.2.7-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6"},
+    {url = "https://files.pythonhosted.org/packages/80/d7/67937c80b8fd4c909fdac29292bc8b35d9505312cff6bcab41c53c5b1df6/coverage-7.2.7-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f"},
+    {url = "https://files.pythonhosted.org/packages/88/8b/b0d9fe727acae907fa7f1c8194ccb6fe9d02e1c3e9001ecf74c741f86110/coverage-7.2.7-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9"},
+    {url = "https://files.pythonhosted.org/packages/88/da/495944ebf0ad246235a6bd523810d9f81981f9b81c6059ba1f56e943abe0/coverage-7.2.7-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9"},
+    {url = "https://files.pythonhosted.org/packages/8c/95/16eed713202406ca0a37f8ac259bbf144c9d24f9b8097a8e6ead61da2dbb/coverage-7.2.7-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"},
+    {url = "https://files.pythonhosted.org/packages/8d/d6/53e999ec1bf7498ca4bc5f3b8227eb61db39068d2de5dcc359dec5601b5a/coverage-7.2.7-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02"},
+    {url = "https://files.pythonhosted.org/packages/8f/a8/12cc7b261f3082cc299ab61f677f7e48d93e35ca5c3c2f7241ed5525ccea/coverage-7.2.7-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833"},
+    {url = "https://files.pythonhosted.org/packages/91/e8/469ed808a782b9e8305a08bad8c6fa5f8e73e093bda6546c5aec68275bff/coverage-7.2.7-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353"},
+    {url = "https://files.pythonhosted.org/packages/94/4e/d4e46a214ae857be3d7dc5de248ba43765f60daeb1ab077cb6c1536c7fba/coverage-7.2.7-cp310-cp310-win32.whl", hash = "sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818"},
+    {url = "https://files.pythonhosted.org/packages/9f/5c/d9760ac497c41f9c4841f5972d0edf05d50cad7814e86ee7d133ec4a0ac8/coverage-7.2.7-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d"},
+    {url = "https://files.pythonhosted.org/packages/a7/cd/3ce94ad9d407a052dc2a74fbeb1c7947f442155b28264eb467ee78dea812/coverage-7.2.7-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb"},
+    {url = "https://files.pythonhosted.org/packages/a9/0c/4a848ae663b47f1195abcb09a951751dd61f80b503303b9b9d768e0fd321/coverage-7.2.7-cp39-cp39-win_amd64.whl", hash = "sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27"},
+    {url = "https://files.pythonhosted.org/packages/b1/96/c12ed0dfd4ec587f3739f53eb677b9007853fd486ccb0e7d5512a27bab2e/coverage-7.2.7-cp311-cp311-win_amd64.whl", hash = "sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562"},
+    {url = "https://files.pythonhosted.org/packages/b1/d5/a8e276bc005e42114468d4fe03e0a9555786bc51cbfe0d20827a46c1565a/coverage-7.2.7-cp39-cp39-win32.whl", hash = "sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb"},
+    {url = "https://files.pythonhosted.org/packages/b4/bd/1b2331e3a04f4cc9b7b332b1dd0f3a1261dfc4114f8479bebfcc2afee9e8/coverage-7.2.7-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063"},
+    {url = "https://files.pythonhosted.org/packages/b7/00/14b00a0748e9eda26e97be07a63cc911108844004687321ddcc213be956c/coverage-7.2.7-cp312-cp312-win_amd64.whl", hash = "sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3"},
+    {url = "https://files.pythonhosted.org/packages/b8/9d/926fce7e03dbfc653104c2d981c0fa71f0572a9ebd344d24c573bd6f7c4f/coverage-7.2.7-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6"},
+    {url = "https://files.pythonhosted.org/packages/ba/92/69c0722882643df4257ecc5437b83f4c17ba9e67f15dc6b77bad89b6982e/coverage-7.2.7-cp311-cp311-win32.whl", hash = "sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a"},
+    {url = "https://files.pythonhosted.org/packages/bb/e9/88747b40c8fb4a783b40222510ce6d66170217eb05d7f46462c36b4fa8cc/coverage-7.2.7-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2"},
+    {url = "https://files.pythonhosted.org/packages/c1/49/4d487e2ad5d54ed82ac1101e467e8994c09d6123c91b2a962145f3d262c2/coverage-7.2.7-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f"},
+    {url = "https://files.pythonhosted.org/packages/c3/1c/6b3c9c363fb1433c79128e0d692863deb761b1b78162494abb9e5c328bc0/coverage-7.2.7-cp38-cp38-win_amd64.whl", hash = "sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c"},
+    {url = "https://files.pythonhosted.org/packages/c6/fa/529f55c9a1029c840bcc9109d5a15ff00478b7ff550a1ae361f8745f8ad5/coverage-7.2.7-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f"},
+    {url = "https://files.pythonhosted.org/packages/c6/fc/be19131010930a6cf271da48202c8cc1d3f971f68c02fb2d3a78247f43dc/coverage-7.2.7-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5"},
+    {url = "https://files.pythonhosted.org/packages/c8/e4/e6182e4697665fb594a7f4e4f27cb3a4dd00c2e3d35c5c706765de8c7866/coverage-7.2.7-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9"},
+    {url = "https://files.pythonhosted.org/packages/ca/0c/3dfeeb1006c44b911ee0ed915350db30325d01808525ae7cc8d57643a2ce/coverage-7.2.7-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2"},
+    {url = "https://files.pythonhosted.org/packages/d1/3a/67f5d18f911abf96857f6f7e4df37ca840e38179e2cc9ab6c0b9c3380f19/coverage-7.2.7-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2"},
+    {url = "https://files.pythonhosted.org/packages/d9/1d/cd467fceb62c371f9adb1d739c92a05d4e550246daa90412e711226bd320/coverage-7.2.7-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e"},
+    {url = "https://files.pythonhosted.org/packages/dd/ce/97c1dd6592c908425622fe7f31c017d11cf0421729b09101d4de75bcadc8/coverage-7.2.7-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5"},
+    {url = "https://files.pythonhosted.org/packages/de/a3/5a98dc9e239d0dc5f243ef5053d5b1bdcaa1dee27a691dfc12befeccf878/coverage-7.2.7-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f"},
+    {url = "https://files.pythonhosted.org/packages/e2/c0/73f139794c742840b9ab88e2e17fe14a3d4668a166ff95d812ac66c0829d/coverage-7.2.7-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd"},
+    {url = "https://files.pythonhosted.org/packages/e9/40/383305500d24122dbed73e505a4d6828f8f3356d1f68ab6d32c781754b81/coverage-7.2.7-cp37-cp37m-win32.whl", hash = "sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f"},
+    {url = "https://files.pythonhosted.org/packages/fe/57/e4f8ad64d84ca9e759d783a052795f62a9f9111585e46068845b1cb52c2b/coverage-7.2.7-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1"},
+    {url = "https://files.pythonhosted.org/packages/ff/d5/52fa1891d1802ab2e1b346d37d349cb41cdd4fd03f724ebbf94e80577687/coverage-7.2.7-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4"},
+]
+"debugpy 1.6.7" = [
+    {url = "https://files.pythonhosted.org/packages/0f/63/d07f5c023abf3192200344d494118f7a00168d67eec50cc16c9bf20a3333/debugpy-1.6.7-py2.py3-none-any.whl", hash = "sha256:53f7a456bc50706a0eaabecf2d3ce44c4d5010e46dfc65b6b81a518b42866267"},
+    {url = "https://files.pythonhosted.org/packages/11/c1/5185e404c8d0198f2e41721dcdec2a4da82938684546a7c6df55922fa044/debugpy-1.6.7-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:de86029696e1b3b4d0d49076b9eba606c226e33ae312a57a46dca14ff370894d"},
+    {url = "https://files.pythonhosted.org/packages/35/59/8c931ec27227fc2aace39566cb82b5df8e10ab03a3b230213383c87d3a25/debugpy-1.6.7-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:279d64c408c60431c8ee832dfd9ace7c396984fd7341fa3116aee414e7dcd88d"},
+    {url = "https://files.pythonhosted.org/packages/3c/70/6615731fb33f858986658428622156a08a8f6647ea7d33549a4cfe803456/debugpy-1.6.7-cp38-cp38-macosx_10_15_x86_64.whl", hash = "sha256:5224eabbbeddcf1943d4e2821876f3e5d7d383f27390b82da5d9558fd4eb30a9"},
+    {url = "https://files.pythonhosted.org/packages/5d/af/8fc131291aa6bb20bdbc07f3bbbe53785f366abf157928fcc00e992e71cc/debugpy-1.6.7-cp310-cp310-win32.whl", hash = "sha256:33edb4afa85c098c24cc361d72ba7c21bb92f501104514d4ffec1fb36e09c01a"},
+    {url = "https://files.pythonhosted.org/packages/67/bf/23c2add9b70a3bf5b0143bf054dc09e380316a1d28e1ace6cd7fc5be520a/debugpy-1.6.7-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:0679b7e1e3523bd7d7869447ec67b59728675aadfc038550a63a362b63029d2c"},
+    {url = "https://files.pythonhosted.org/packages/70/91/b64453cf09557d3e1502dcdaac53955cefbe856d0dd84be1c2e8eb67c9dd/debugpy-1.6.7-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bae1123dff5bfe548ba1683eb972329ba6d646c3a80e6b4c06cd1b1dd0205e9b"},
+    {url = "https://files.pythonhosted.org/packages/76/7d/e141516510764239c881273198ea3ef932d67c17ce8efa00d41654f6e34a/debugpy-1.6.7-cp39-cp39-win32.whl", hash = "sha256:d71b31117779d9a90b745720c0eab54ae1da76d5b38c8026c654f4a066b0130a"},
+    {url = "https://files.pythonhosted.org/packages/7e/59/d4491446423c601371033a699d00c17ffae573724ebfe1dcc997ccc80afc/debugpy-1.6.7-cp38-cp38-win32.whl", hash = "sha256:9cd10cf338e0907fdcf9eac9087faa30f150ef5445af5a545d307055141dd7a4"},
+    {url = "https://files.pythonhosted.org/packages/8e/b0/ed43b2d9a5e90b144e7a492308c9d4893946ca526e9dbf1d6466f4c6e2f4/debugpy-1.6.7-cp37-cp37m-macosx_10_15_x86_64.whl", hash = "sha256:38ed626353e7c63f4b11efad659be04c23de2b0d15efff77b60e4740ea685d07"},
+    {url = "https://files.pythonhosted.org/packages/92/d4/437fa53a5a0e5a04d77e12b7eeac1df003e33834f85ddd4513fe2df31e13/debugpy-1.6.7.zip", hash = "sha256:c4c2f0810fa25323abfdfa36cbbbb24e5c3b1a42cb762782de64439c575d67f2"},
+    {url = "https://files.pythonhosted.org/packages/97/b2/1b264a5985de53f3f9399eb3ea83dcc4b8d2126995e04cb318c806b1424e/debugpy-1.6.7-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e3876611d114a18aafef6383695dfc3f1217c98a9168c1aaf1a02b01ec7d8d1e"},
+    {url = "https://files.pythonhosted.org/packages/a8/9a/342ac3474d2c5f4bca261e084143a77f559431635272c8ded5c1ecd65202/debugpy-1.6.7-cp37-cp37m-win32.whl", hash = "sha256:dbe04e7568aa69361a5b4c47b4493d5680bfa3a911d1e105fbea1b1f23f3eb45"},
+    {url = "https://files.pythonhosted.org/packages/ac/7f/409fb252284681fc1703d9465b6c5c2c08612be3ffe3a5923be23a9ced69/debugpy-1.6.7-cp39-cp39-win_amd64.whl", hash = "sha256:c0ff93ae90a03b06d85b2c529eca51ab15457868a377c4cc40a23ab0e4e552a3"},
+    {url = "https://files.pythonhosted.org/packages/ae/24/1150e66a4dec62c16b34c6cc0ff8d6cfe89ac2a64112797d70cfe774e682/debugpy-1.6.7-cp38-cp38-win_amd64.whl", hash = "sha256:aaf6da50377ff4056c8ed470da24632b42e4087bc826845daad7af211e00faad"},
+    {url = "https://files.pythonhosted.org/packages/af/7e/61738aba4da0de74e797ca71013977ebd8d35f58b18e674da045efb30487/debugpy-1.6.7-cp37-cp37m-win_amd64.whl", hash = "sha256:f90a2d4ad9a035cee7331c06a4cf2245e38bd7c89554fe3b616d90ab8aab89cc"},
+    {url = "https://files.pythonhosted.org/packages/bb/27/6f8ba374ec748a70fedf61e87b9d08387a299f22458c4847c82b12bdd357/debugpy-1.6.7-cp310-cp310-win_amd64.whl", hash = "sha256:ed6d5413474e209ba50b1a75b2d9eecf64d41e6e4501977991cdc755dc83ab0f"},
+    {url = "https://files.pythonhosted.org/packages/ee/7e/7a0621b57788ee106932149eba7dc5c014d7212f95964638c04aadd98425/debugpy-1.6.7-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:b3e7ac809b991006ad7f857f016fa92014445085711ef111fdc3f74f66144096"},
 ]
 "decorator 5.1.1" = [
     {url = "https://files.pythonhosted.org/packages/66/0c/8d907af351aa16b42caae42f9d6aa37b900c67308052d10fdce809f8d952/decorator-5.1.1.tar.gz", hash = "sha256:637996211036b6385ef91435e4fae22989472f9d571faba8927ba8253acbc330"},
     {url = "https://files.pythonhosted.org/packages/d5/50/83c593b07763e1161326b3b8c6686f0f4b0f24d5526546bee538c89837d6/decorator-5.1.1-py3-none-any.whl", hash = "sha256:b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186"},
 ]
 "defusedxml 0.7.1" = [
     {url = "https://files.pythonhosted.org/packages/07/6c/aa3f2f849e01cb6a001cd8554a88d4c77c5c1a31c95bdf1cf9301e6d9ef4/defusedxml-0.7.1-py2.py3-none-any.whl", hash = "sha256:a352e7e428770286cc899e2542b6cdaedb2b4953ff269a210103ec58f6198a61"},
     {url = "https://files.pythonhosted.org/packages/0f/d5/c66da9b79e5bdb124974bfe172b4daf3c984ebd9c2a06e2b8a4dc7331c72/defusedxml-0.7.1.tar.gz", hash = "sha256:1bb3032db185915b62d7c6209c5a8792be6a32ab2fedacc84e01b52c51aa3e69"},
 ]
 "entrypoints 0.4" = [
     {url = "https://files.pythonhosted.org/packages/35/a8/365059bbcd4572cbc41de17fd5b682be5868b218c3c5479071865cab9078/entrypoints-0.4-py3-none-any.whl", hash = "sha256:f174b5ff827504fd3cd97cc3f8649f3693f51538c7e4bdf3ef002c8429d42f9f"},
     {url = "https://files.pythonhosted.org/packages/ea/8d/a7121ffe5f402dc015277d2d31eb82d2187334503a011c18f2e78ecbb9b2/entrypoints-0.4.tar.gz", hash = "sha256:b706eddaa9218a19ebcd67b56818f05bb27589b1ca9e8d797b74affad4ccacd4"},
 ]
-"exceptiongroup 1.1.0" = [
-    {url = "https://files.pythonhosted.org/packages/15/ab/dd27fb742b19a9d020338deb9ab9a28796524081bca880ac33c172c9a8f6/exceptiongroup-1.1.0.tar.gz", hash = "sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23"},
-    {url = "https://files.pythonhosted.org/packages/e8/14/9c6a7e5f12294ccd6975a45e02899ed25468cd7c2c86f3d9725f387f9f5f/exceptiongroup-1.1.0-py3-none-any.whl", hash = "sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e"},
-]
-"fastjsonschema 2.16.2" = [
-    {url = "https://files.pythonhosted.org/packages/7a/62/6df03bacda3544b5872d0b30f79c599ab84fc598858c77a77e1587d61ba3/fastjsonschema-2.16.2.tar.gz", hash = "sha256:01e366f25d9047816fe3d288cbfc3e10541daf0af2044763f3d0ade42476da18"},
-    {url = "https://files.pythonhosted.org/packages/e4/be/cf1b876348070a23cb0c3ebfee7a452ad3a91b07b456dade3bd514656009/fastjsonschema-2.16.2-py3-none-any.whl", hash = "sha256:21f918e8d9a1a4ba9c22e09574ba72267a6762d47822db9add95f6454e51cc1c"},
+"exceptiongroup 1.1.1" = [
+    {url = "https://files.pythonhosted.org/packages/61/97/17ed81b7a8d24d8f69b62c0db37abbd8c0042d4b3fc429c73dab986e7483/exceptiongroup-1.1.1-py3-none-any.whl", hash = "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e"},
+    {url = "https://files.pythonhosted.org/packages/cc/38/57f14ddc8e8baeddd8993a36fe57ce7b4ba174c35048b9a6d270bb01e833/exceptiongroup-1.1.1.tar.gz", hash = "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"},
+]
+"fastjsonschema 2.17.1" = [
+    {url = "https://files.pythonhosted.org/packages/a4/e1/cda97fa4447e138f1f0ccfdaf678fa247415f7e9f4942d856fd63c7d863c/fastjsonschema-2.17.1.tar.gz", hash = "sha256:f4eeb8a77cef54861dbf7424ac8ce71306f12cbb086c45131bcba2c6a4f726e3"},
+    {url = "https://files.pythonhosted.org/packages/d4/a1/b3816c7945742ee95e2fb68dd59aaa205c9ce53ffd90704f70c2207a7b4d/fastjsonschema-2.17.1-py3-none-any.whl", hash = "sha256:4b90b252628ca695280924d863fe37234eebadc29c5360d322571233dc9746e0"},
 ]
 "flake8 5.0.4" = [
     {url = "https://files.pythonhosted.org/packages/ad/00/9808c62b2d529cefc69ce4e4a1ea42c0f855effa55817b7327ec5b75e60a/flake8-5.0.4.tar.gz", hash = "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db"},
     {url = "https://files.pythonhosted.org/packages/cf/a0/b881b63a17a59d9d07f5c0cc91a29182c8e8a9aa2bde5b3b2b16519c02f4/flake8-5.0.4-py2.py3-none-any.whl", hash = "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"},
 ]
-"flake8-pyproject 1.2.2" = [
-    {url = "https://files.pythonhosted.org/packages/91/8a/607fc3cb97714873e3c333afb4927e0341cec2677a26ca0dc7e0e666f016/flake8_pyproject-1.2.2-py3-none-any.whl", hash = "sha256:52d412219e7db6227faa654675b1435947b11d49b453f3eced760f19bdd6f06a"},
+"flake8-pyproject 1.2.3" = [
+    {url = "https://files.pythonhosted.org/packages/5f/1d/635e86f9f3a96b7ea9e9f19b5efe17a987e765c39ca496e4a893bb999112/flake8_pyproject-1.2.3-py3-none-any.whl", hash = "sha256:6249fe53545205af5e76837644dc80b4c10037e73a0e5db87ff562d75fb5bd4a"},
 ]
-"flask 2.2.2" = [
-    {url = "https://files.pythonhosted.org/packages/0f/43/15f4f9ab225b0b25352412e8daa3d0e3d135fcf5e127070c74c3632c8b4c/Flask-2.2.2-py3-none-any.whl", hash = "sha256:b9c46cc36662a7949f34b52d8ec7bb59c0d74ba08ba6cb9ce9adc1d8676d9526"},
-    {url = "https://files.pythonhosted.org/packages/69/b6/53cfa30eed5aa7343daff36622843688ba8c6fe9829bb2b92e193ab1163f/Flask-2.2.2.tar.gz", hash = "sha256:642c450d19c4ad482f96729bd2a8f6d32554aa1e231f4f6b4e7e5264b16cca2b"},
+"flask 2.2.5" = [
+    {url = "https://files.pythonhosted.org/packages/5f/76/a4d2c4436dda4b0a12c71e075c508ea7988a1066b06a575f6afe4fecc023/Flask-2.2.5.tar.gz", hash = "sha256:edee9b0a7ff26621bd5a8c10ff484ae28737a2410d99b0bb9a6850c7fb977aa0"},
+    {url = "https://files.pythonhosted.org/packages/9f/1a/8b6d48162861009d1e017a9740431c78d860809773b66cac220a11aa3310/Flask-2.2.5-py3-none-any.whl", hash = "sha256:58107ed83443e86067e41eff4631b058178191a355886f8e479e347fa1285fdf"},
 ]
 "h11 0.14.0" = [
     {url = "https://files.pythonhosted.org/packages/95/04/ff642e65ad6b90db43e668d70ffb6736436c7ce41fcc549f4e9472234127/h11-0.14.0-py3-none-any.whl", hash = "sha256:e3fe4ac4b851c468cc8363d500db52c2ead036020723024a109d37346efaa761"},
     {url = "https://files.pythonhosted.org/packages/f5/38/3af3d3633a34a3316095b39c8e8fb4853a28a536e55d347bd8d8e9a14b03/h11-0.14.0.tar.gz", hash = "sha256:8f19fbbe99e72420ff35c00b27a34cb9937e902a8b810e2c88300c6f0a3b699d"},
 ]
-"httpcore 0.16.3" = [
-    {url = "https://files.pythonhosted.org/packages/04/7e/ef97af4623024e8159993b3114ce208de4f677098ae058ec5882a1bf7605/httpcore-0.16.3-py3-none-any.whl", hash = "sha256:da1fb708784a938aa084bde4feb8317056c55037247c787bd7e19eb2c2949dc0"},
-    {url = "https://files.pythonhosted.org/packages/61/42/5c456b02816845d163fab0f32936b6a5b649f3f915beff6f819f4f6c90b2/httpcore-0.16.3.tar.gz", hash = "sha256:c5d6f04e2fc530f39e0c077e6a30caa53f1451096120f1f38b954afd0b17c0cb"},
-]
-"httpx 0.23.3" = [
-    {url = "https://files.pythonhosted.org/packages/ac/a2/0260c0f5d73bdf06e8d3fc1013a82b9f0633dc21750c9e3f3cb1dba7bb8c/httpx-0.23.3-py3-none-any.whl", hash = "sha256:a211fcce9b1254ea24f0cd6af9869b3d29aba40154e947d2a07bb499b3e310d6"},
-    {url = "https://files.pythonhosted.org/packages/f5/50/04d5e8ee398a10c767a341a25f59ff8711ae3adf0143c7f8b45fc560d72d/httpx-0.23.3.tar.gz", hash = "sha256:9818458eb565bb54898ccb9b8b251a28785dd4a55afbc23d0eb410754fe7d0f9"},
+"httpcore 0.17.2" = [
+    {url = "https://files.pythonhosted.org/packages/4d/32/b908f673ccef12b6425b848a541264ee3d95f5f571f18f6ab0d8c311442e/httpcore-0.17.2-py3-none-any.whl", hash = "sha256:5581b9c12379c4288fe70f43c710d16060c10080617001e6b22a3b6dbcbefd36"},
+    {url = "https://files.pythonhosted.org/packages/b3/ad/7002a6f8e6ce0a246c991e00ba79b26ad06d307421a160214df24de5651f/httpcore-0.17.2.tar.gz", hash = "sha256:125f8375ab60036db632f34f4b627a9ad085048eef7cb7d2616fea0f739f98af"},
+]
+"httpx 0.24.1" = [
+    {url = "https://files.pythonhosted.org/packages/ec/91/e41f64f03d2a13aee7e8c819d82ee3aa7cdc484d18c0ae859742597d5aa0/httpx-0.24.1-py3-none-any.whl", hash = "sha256:06781eb9ac53cde990577af654bd990a4949de37a28bdb4a230d434f3a30b9bd"},
+    {url = "https://files.pythonhosted.org/packages/f8/2a/114d454cb77657dbf6a293e69390b96318930ace9cd96b51b99682493276/httpx-0.24.1.tar.gz", hash = "sha256:5853a43053df830c20f8110c5e69fe44d035d850b2dfe795e196f00fdb774bdd"},
 ]
 "idna 3.4" = [
     {url = "https://files.pythonhosted.org/packages/8b/e1/43beb3d38dba6cb420cefa297822eac205a277ab43e5ba5d5c46faf96438/idna-3.4.tar.gz", hash = "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4"},
     {url = "https://files.pythonhosted.org/packages/fc/34/3030de6f1370931b9dbb4dad48f6ab1015ab1d32447850b9fc94e60097be/idna-3.4-py3-none-any.whl", hash = "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"},
 ]
 "importlib-metadata 4.2.0" = [
     {url = "https://files.pythonhosted.org/packages/22/51/52442c59db26637681148c21f8984eed58c9db67053a0a4783a047010c98/importlib_metadata-4.2.0-py3-none-any.whl", hash = "sha256:057e92c15bc8d9e8109738a48db0ccb31b4d9d5cfbee5a8670879a30be66304b"},
     {url = "https://files.pythonhosted.org/packages/c7/7c/126a8686399ebe256b5e4343ea80b6f2ee91549969da2eef0bb2891b8d24/importlib_metadata-4.2.0.tar.gz", hash = "sha256:b7e52a1f8dec14a75ea73e0891f3060099ca1d8e6a462a4dff11c3e119ea1b31"},
 ]
-"importlib-resources 5.10.2" = [
-    {url = "https://files.pythonhosted.org/packages/2e/f8/be5c59ff2545362397cbc989f5cd3835326fc4092433d50dfaf21616bc71/importlib_resources-5.10.2.tar.gz", hash = "sha256:e4a96c8cc0339647ff9a5e0550d9f276fc5a01ffa276012b58ec108cfd7b8484"},
-    {url = "https://files.pythonhosted.org/packages/be/0f/bd3e7fa47cc43276051c557d3b2fe946664781d2ecf08b05d074e1a3ee59/importlib_resources-5.10.2-py3-none-any.whl", hash = "sha256:7d543798b0beca10b6a01ac7cafda9f822c54db9e8376a6bf57e0cbd74d486b6"},
+"importlib-resources 5.12.0" = [
+    {url = "https://files.pythonhosted.org/packages/38/71/c13ea695a4393639830bf96baea956538ba7a9d06fcce7cef10bfff20f72/importlib_resources-5.12.0-py3-none-any.whl", hash = "sha256:7b1deeebbf351c7578e09bf2f63fa2ce8b5ffec296e0d349139d43cca061a81a"},
+    {url = "https://files.pythonhosted.org/packages/4e/a2/3cab1de83f95dd15297c15bdc04d50902391d707247cada1f021bbfe2149/importlib_resources-5.12.0.tar.gz", hash = "sha256:4be82589bf5c1d7999aedf2a45159d10cb3ca4f19b2271f8792bc8e6da7b22f6"},
 ]
 "iniconfig 2.0.0" = [
     {url = "https://files.pythonhosted.org/packages/d7/4b/cbd8e699e64a6f16ca3a8220661b5f83792b3017d0f79807cb8708d33913/iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
     {url = "https://files.pythonhosted.org/packages/ef/a6/62565a6e1cf69e10f5727360368e451d4b7f58beeac6173dc9db836a5b46/iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
 ]
 "ipykernel 6.16.2" = [
     {url = "https://files.pythonhosted.org/packages/4f/ca/22431cf8ffa45438a5ab7d5e0ada45037b3622478ef45b231f29783a93a9/ipykernel-6.16.2.tar.gz", hash = "sha256:463f3d87a92e99969b1605cb7a5b4d7b36b7145a0e72d06e65918a6ddefbe630"},
@@ -1286,17 +1305,17 @@
     {url = "https://files.pythonhosted.org/packages/7c/6a/1f1365f4bf9fcb349fcaa5b61edfcefa721aa13ff37c5631296b12fab8e5/ipython-7.34.0-py3-none-any.whl", hash = "sha256:c175d2440a1caff76116eb719d40538fbb316e214eda85c5515c303aacbfb23e"},
     {url = "https://files.pythonhosted.org/packages/db/6c/3fcf0b8ee46656796099ac4b7b72497af5f090da3e43fd305f2a24c73915/ipython-7.34.0.tar.gz", hash = "sha256:af3bdb46aa292bce5615b1b2ebc76c2080c5f77f54bda2ec72461317273e7cd6"},
 ]
 "ipython-genutils 0.2.0" = [
     {url = "https://files.pythonhosted.org/packages/e8/69/fbeffffc05236398ebfcfb512b6d2511c622871dca1746361006da310399/ipython_genutils-0.2.0.tar.gz", hash = "sha256:eb2e116e75ecef9d4d228fdc66af54269afa26ab4463042e33785b887c628ba8"},
     {url = "https://files.pythonhosted.org/packages/fa/bc/9bd3b5c2b4774d5f33b2d544f1460be9df7df2fe42f352135381c347c69a/ipython_genutils-0.2.0-py2.py3-none-any.whl", hash = "sha256:72dd37233799e619666c9f639a9da83c34013a73e8bbc79a7a6348d93c61fab8"},
 ]
-"ipywidgets 8.0.4" = [
-    {url = "https://files.pythonhosted.org/packages/26/2a/47bf74e71f2c172136e3a101d8a222807ec5cabc10321dfa14f58fda1cbf/ipywidgets-8.0.4.tar.gz", hash = "sha256:c0005a77a47d77889cafed892b58e33b4a2a96712154404c6548ec22272811ea"},
-    {url = "https://files.pythonhosted.org/packages/f3/fc/bd076538811d63babf8ceea0ff3d8d024171569a47f5dba7757c5fd0462c/ipywidgets-8.0.4-py3-none-any.whl", hash = "sha256:ebb195e743b16c3947fe8827190fb87b4d00979c0fbf685afe4d2c4927059fa1"},
+"ipywidgets 8.0.6" = [
+    {url = "https://files.pythonhosted.org/packages/50/7d/2c8b7bba2b1c2b5d1299f22fa7853f09b573c84e63b62870c13a6ec11990/ipywidgets-8.0.6-py3-none-any.whl", hash = "sha256:a60bf8d2528997e05ac83fd19ea2fbe65f2e79fbe1b2b35779bdfc46c2941dcc"},
+    {url = "https://files.pythonhosted.org/packages/64/3c/00fe451a0571677a37e78515613f6578ba61462626354a98c17e1b4f9c68/ipywidgets-8.0.6.tar.gz", hash = "sha256:de7d779f2045d60de9f6c25f653fdae2dba57898e6a1284494b3ba20b6893bb8"},
 ]
 "isort 5.11.5" = [
     {url = "https://files.pythonhosted.org/packages/5f/f6/c55db45970fbd14de6ab72082f1b8a143c3a69aa031c1e0dd4b9ecc8d496/isort-5.11.5-py3-none-any.whl", hash = "sha256:ba1d72fb2595a01c7895a5128f9585a5cc4b6d395f1c8d514989b9a7eb2a8746"},
     {url = "https://files.pythonhosted.org/packages/67/63/18cc5c2f9084d3f91ce704f2b5c8e17bedd777244e7732c21a31992b0a78/isort-5.11.5.tar.gz", hash = "sha256:6be1f76a507cb2ecf16c7cf14a37e41609ca082330be4e3436a18ef74add55db"},
 ]
 "itsdangerous 2.1.2" = [
     {url = "https://files.pythonhosted.org/packages/68/5f/447e04e828f47465eeab35b5d408b7ebaaaee207f48b7136c5a7267a30ae/itsdangerous-2.1.2-py3-none-any.whl", hash = "sha256:2c2349112351b88699d8d4b6b075022c0808887cb7ad10069318a8b0bc88db44"},
@@ -1319,287 +1338,283 @@
     {url = "https://files.pythonhosted.org/packages/c9/a9/371d0b8fe37dd231cf4b2cff0a9f0f25e98f3a73c3771742444be27f2944/jupyter-1.0.0.tar.gz", hash = "sha256:d9dc4b3318f310e34c82951ea5d6683f67bed7def4b259fafbfe4f1beb1d8e5f"},
     {url = "https://files.pythonhosted.org/packages/fc/21/a372b73e3a498b41b92ed915ada7de2ad5e16631546329c03e484c3bf4e9/jupyter-1.0.0.zip", hash = "sha256:3e1f86076bbb7c8c207829390305a2b1fe836d471ed54be66a3b8c41e7f46cc7"},
 ]
 "jupyter-client 7.4.9" = [
     {url = "https://files.pythonhosted.org/packages/1e/33/71778cdd2c69445bcd3bb6029da2e43cc9b5cbbeef4f4982ef3aaf396650/jupyter_client-7.4.9.tar.gz", hash = "sha256:52be28e04171f07aed8f20e1616a5a552ab9fee9cbbe6c1896ae170c3880d392"},
     {url = "https://files.pythonhosted.org/packages/fd/a7/ef3b7c8b9d6730a21febdd0809084e4cea6d2a7e43892436adecdd0acbd4/jupyter_client-7.4.9-py3-none-any.whl", hash = "sha256:214668aaea208195f4c13d28eb272ba79f945fc0cf3f11c7092c20b2ca1980e7"},
 ]
-"jupyter-console 6.4.4" = [
-    {url = "https://files.pythonhosted.org/packages/1b/2f/acb5851aa3ed730f8cde5ec9eb0c0d9681681123f32c3b82d1536df1e937/jupyter_console-6.4.4.tar.gz", hash = "sha256:172f5335e31d600df61613a97b7f0352f2c8250bbd1092ef2d658f77249f89fb"},
-    {url = "https://files.pythonhosted.org/packages/8b/0c/f9382ca7b7499c8594a5158817a72c95b4c09a6c6f2de10553bfe8905924/jupyter_console-6.4.4-py3-none-any.whl", hash = "sha256:756df7f4f60c986e7bc0172e4493d3830a7e6e75c08750bbe59c0a5403ad6dee"},
+"jupyter-console 6.6.3" = [
+    {url = "https://files.pythonhosted.org/packages/bd/2d/e2fd31e2fc41c14e2bcb6c976ab732597e907523f6b2420305f9fc7fdbdb/jupyter_console-6.6.3.tar.gz", hash = "sha256:566a4bf31c87adbfadf22cdf846e3069b59a71ed5da71d6ba4d8aaad14a53539"},
+    {url = "https://files.pythonhosted.org/packages/ca/77/71d78d58f15c22db16328a476426f7ac4a60d3a5a7ba3b9627ee2f7903d4/jupyter_console-6.6.3-py3-none-any.whl", hash = "sha256:309d33409fcc92ffdad25f0bcdf9a4a9daa61b6f341177570fdac03de5352485"},
 ]
 "jupyter-core 4.12.0" = [
     {url = "https://files.pythonhosted.org/packages/02/8f/0e0ad6804c0a021a27410ec997626a7a955c20916454d0205f16eb83de4b/jupyter_core-4.12.0-py3-none-any.whl", hash = "sha256:a54672c539333258495579f6964144924e0aa7b07f7069947bef76d7ea5cb4c1"},
     {url = "https://files.pythonhosted.org/packages/8b/d9/0d18cbe8d0d2eb165dd0b42266f0e5e31b1f80c3a48031fbef1077c34521/jupyter_core-4.12.0.tar.gz", hash = "sha256:87f39d7642412ae8a52291cc68e71ac01dfa2c735df2701f8108251d51b4f460"},
 ]
-"jupyter-server 1.23.5" = [
-    {url = "https://files.pythonhosted.org/packages/77/d0/41f8ac982b49456fe93bd0b00efb49c2df1ac2bada8c92c3d4e702f80477/jupyter_server-1.23.5-py3-none-any.whl", hash = "sha256:d42e520af98af9fbb7f0fb0d069991054d88e4d2ee051eb7110aef35f3756cef"},
-    {url = "https://files.pythonhosted.org/packages/95/a9/053638b3798bf5bf4ae972946f6f0cf4a96ed88f07e53129bbecf7e5010d/jupyter_server-1.23.5.tar.gz", hash = "sha256:a2caa759e2a29ece1aad013c58215fe951f38317b97de462b921834955fe3fca"},
+"jupyter-server 1.24.0" = [
+    {url = "https://files.pythonhosted.org/packages/5b/ce/142bcb35ffe215d8880e968689ab733bd7976a6c20dae24b6782cce2219a/jupyter_server-1.24.0-py3-none-any.whl", hash = "sha256:c88ddbe862966ea1aea8c3ccb89a5903abd8fbcfe5cd14090ef549d403332c37"},
+    {url = "https://files.pythonhosted.org/packages/79/0c/ce06c97c52707bc0fed9461ed5624f1a5ee76dc772d7da2c0699395653af/jupyter_server-1.24.0.tar.gz", hash = "sha256:23368e8e214baf82b313d4c5a0d828ca73015e1a192ce3829bd74e62fab8d046"},
 ]
 "jupyterlab-pygments 0.2.2" = [
     {url = "https://files.pythonhosted.org/packages/69/8e/8ae01f052013ee578b297499d16fcfafb892927d8e41c1a0054d2f99a569/jupyterlab_pygments-0.2.2.tar.gz", hash = "sha256:7405d7fde60819d905a9fa8ce89e4cd830e318cdad22a0030f7a901da705585d"},
     {url = "https://files.pythonhosted.org/packages/c0/7e/c3d1df3ae9b41686e664051daedbd70eea2e1d2bd9d9c33e7e1455bc9f96/jupyterlab_pygments-0.2.2-py2.py3-none-any.whl", hash = "sha256:2405800db07c9f770863bcf8049a529c3dd4d3e28536638bd7c1c01d2748309f"},
 ]
-"jupyterlab-widgets 3.0.5" = [
-    {url = "https://files.pythonhosted.org/packages/a8/59/1c1a0ae2dc4586c08c372aaee6f5f765327564a753752a8df2574ea1aa31/jupyterlab_widgets-3.0.5.tar.gz", hash = "sha256:eeaecdeaf6c03afc960ddae201ced88d5979b4ca9c3891bcb8f6631af705f5ef"},
-    {url = "https://files.pythonhosted.org/packages/df/82/4576cbc07ebace8c7734fe08b2c2f9123b7ebecd29e932a3b839b6bee2cb/jupyterlab_widgets-3.0.5-py3-none-any.whl", hash = "sha256:a04a42e50231b355b7087e16a818f541e53589f7647144ea0344c4bf16f300e5"},
-]
-"loguru 0.6.0" = [
-    {url = "https://files.pythonhosted.org/packages/75/1f/d3818863e4be96bd641c4643c535a98f0fa2a12efa7c8ba35f763fa778ee/loguru-0.6.0.tar.gz", hash = "sha256:066bd06758d0a513e9836fd9c6b5a75bfb3fd36841f4b996bc60b547a309d41c"},
-    {url = "https://files.pythonhosted.org/packages/fe/21/e1d1da2586865a159fc73b611f36bdd50b6c4043cb6132d3d5e972988028/loguru-0.6.0-py3-none-any.whl", hash = "sha256:4e2414d534a2ab57573365b3e6d0234dfb1d84b68b7f3b948e6fb743860a77c3"},
-]
-"markupsafe 2.1.2" = [
-    {url = "https://files.pythonhosted.org/packages/02/2c/18d55e5df6a9ea33709d6c33e08cb2e07d39e20ad05d8c6fbf9c9bcafd54/MarkupSafe-2.1.2-cp310-cp310-win_amd64.whl", hash = "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156"},
-    {url = "https://files.pythonhosted.org/packages/04/cf/9464c3c41b7cdb8df660cda75676697e7fb49ce1be7691a1162fc88da078/MarkupSafe-2.1.2-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc"},
-    {url = "https://files.pythonhosted.org/packages/06/3b/d026c21cd1dbee89f41127e93113dcf5fa85c6660d108847760b59b3a66d/MarkupSafe-2.1.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4"},
-    {url = "https://files.pythonhosted.org/packages/0a/88/78cb3d95afebd183d8b04442685ab4c70cfc1138b850ba20e2a07aff2f53/MarkupSafe-2.1.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd"},
-    {url = "https://files.pythonhosted.org/packages/0d/15/82b108c697bec4c26c00aed6975b778cf0eac6cbb77598862b10550b7fcc/MarkupSafe-2.1.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03"},
-    {url = "https://files.pythonhosted.org/packages/19/00/3b8eb0093c885576a1ce7f2263e7b8c01e55b9977433f8246f57cd81b0be/MarkupSafe-2.1.2-cp311-cp311-win32.whl", hash = "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625"},
-    {url = "https://files.pythonhosted.org/packages/1f/20/76f6337f1e7238a626ab34405ddd634636011b2ff947dcbd8995f16a7776/MarkupSafe-2.1.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0"},
-    {url = "https://files.pythonhosted.org/packages/22/88/9c0cae2f5ada778182f2842b377dd273d6be689953345c10b165478831eb/MarkupSafe-2.1.2-cp39-cp39-win32.whl", hash = "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7"},
-    {url = "https://files.pythonhosted.org/packages/29/d2/243e6b860d97c18d848fc2bee2f39d102755a2b04a5ce4d018d839711b46/MarkupSafe-2.1.2-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba"},
-    {url = "https://files.pythonhosted.org/packages/30/3e/0a69a24adb38df83e2f6989c38d68627a5f27181c82ecaa1fd03d1236dca/MarkupSafe-2.1.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601"},
-    {url = "https://files.pythonhosted.org/packages/34/19/64b0abc021b22766e86efee32b0e2af684c4b731ce8ac1d519c791800c13/MarkupSafe-2.1.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036"},
-    {url = "https://files.pythonhosted.org/packages/37/b2/6f4d5cac75ba6fe9f17671304fe339ea45a73c5609b5f5e652aa79c915c8/MarkupSafe-2.1.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7"},
-    {url = "https://files.pythonhosted.org/packages/39/8d/5c5ce72deb8567ab48a18fbd99dc0af3dd651b6691b8570947e54a28e0f3/MarkupSafe-2.1.2-cp37-cp37m-win_amd64.whl", hash = "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666"},
-    {url = "https://files.pythonhosted.org/packages/3d/66/2f636ba803fd6eb4cee7b3106ae02538d1e84a7fb7f4f8775c6528a87d31/MarkupSafe-2.1.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323"},
-    {url = "https://files.pythonhosted.org/packages/41/54/6e88795c64ab5dcda31b06406c062c2740d1a64db18219d4e21fc90928c1/MarkupSafe-2.1.2-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c"},
-    {url = "https://files.pythonhosted.org/packages/46/0c/10ee33673c5e36fa3809cf136971f81d951ca38516188ee11a965d9b2fe9/MarkupSafe-2.1.2-cp39-cp39-win_amd64.whl", hash = "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed"},
-    {url = "https://files.pythonhosted.org/packages/48/cc/d027612e17b56088cfccd2c8e083518995fcb25a7b4f17fc146362a0499d/MarkupSafe-2.1.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"},
-    {url = "https://files.pythonhosted.org/packages/4b/34/dc837e5ad9e14634aac4342eb8b12a9be20a4f74f50cc0d765f7aa2fc1e3/MarkupSafe-2.1.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094"},
-    {url = "https://files.pythonhosted.org/packages/50/41/1442b693a40eb76d835ca2016e86a01479f17d7fd8288f9830f6790e366a/MarkupSafe-2.1.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3"},
-    {url = "https://files.pythonhosted.org/packages/52/36/b35c577c884ea352fc0c1eaed9ca4946ffc22cc9c3527a70408bfa9e9496/MarkupSafe-2.1.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f"},
-    {url = "https://files.pythonhosted.org/packages/56/0d/c9818629672a3368b773fa94597d79da77bdacc3186f097bb85023f785f6/MarkupSafe-2.1.2-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460"},
-    {url = "https://files.pythonhosted.org/packages/5a/94/d056bf5dbadf7f4b193ee2a132b3d49ffa1602371e3847518b2982045425/MarkupSafe-2.1.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6"},
-    {url = "https://files.pythonhosted.org/packages/5e/f6/8eb8a5692c1986b6e863877b0b8a83628aff14e5fbfaf11d9522b532bd9d/MarkupSafe-2.1.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1"},
-    {url = "https://files.pythonhosted.org/packages/66/21/dadb671aade8eb67ef96e0d8f90b1bd5e8cfb6ad9d8c7fa2c870ec0c257b/MarkupSafe-2.1.2-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619"},
-    {url = "https://files.pythonhosted.org/packages/76/b5/05ce70a3e31ecebcd3628cd180dc4761293aa496db85170fdc085ed2d79a/MarkupSafe-2.1.2-cp38-cp38-win32.whl", hash = "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2"},
-    {url = "https://files.pythonhosted.org/packages/77/26/af46880038c6eac3832e751298f1965f3a550f38d1e9ddaabd674860076b/MarkupSafe-2.1.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd"},
-    {url = "https://files.pythonhosted.org/packages/78/e6/91c9a20a943ea231c59024e181c4c5480097daf132428f2272670974637f/MarkupSafe-2.1.2-cp310-cp310-win32.whl", hash = "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603"},
-    {url = "https://files.pythonhosted.org/packages/79/e2/b818bf277fa6b01244943498cb2127372c01dde5eff7682837cc72740618/MarkupSafe-2.1.2-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d"},
-    {url = "https://files.pythonhosted.org/packages/7b/0f/0e99c2f342933c43af69849a6ba63f2eef54e14c6d0e10a26470fb6b40a9/MarkupSafe-2.1.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a"},
-    {url = "https://files.pythonhosted.org/packages/7c/e6/454df09f18e0ea34d189b447a9e1a9f66c2aa332b77fd5577ebc7ca14d42/MarkupSafe-2.1.2-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2"},
-    {url = "https://files.pythonhosted.org/packages/80/64/ccb65aadd71e7685caa69a885885a673e8748525a243fb26acea37201b44/MarkupSafe-2.1.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54"},
-    {url = "https://files.pythonhosted.org/packages/82/70/b3978786c7b576c25d84b009d2a20a11b5300d252fc3ce984e37b932e97c/MarkupSafe-2.1.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65"},
-    {url = "https://files.pythonhosted.org/packages/82/e3/4efcd74f10a7999783955aec36386f71082e6d7dafcc06b77b9df72b325a/MarkupSafe-2.1.2-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f"},
-    {url = "https://files.pythonhosted.org/packages/87/a1/d0f05a09c6c1aef89d1eea0ab0ff1ea897d4117d27f1571034a7e3ff515b/MarkupSafe-2.1.2-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a"},
-    {url = "https://files.pythonhosted.org/packages/93/ca/1c3ae0c6a5712d4ba98610cada03781ea0448436b17d1dcd4759115b15a1/MarkupSafe-2.1.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1"},
-    {url = "https://files.pythonhosted.org/packages/93/fa/d72f68f84f8537ee8aa3e0764d1eb11e5e025a5ca90c16e94a40f894c2fc/MarkupSafe-2.1.2-cp38-cp38-win_amd64.whl", hash = "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147"},
-    {url = "https://files.pythonhosted.org/packages/95/7e/68018b70268fb4a2a605e2be44ab7b4dd7ce7808adae6c5ef32e34f4b55a/MarkupSafe-2.1.2.tar.gz", hash = "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d"},
-    {url = "https://files.pythonhosted.org/packages/95/88/8c8cce021ac1b1eedde349c6a41f6c256da60babf95e572071361ff3f66b/MarkupSafe-2.1.2-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a"},
-    {url = "https://files.pythonhosted.org/packages/96/92/a873b4a7fa20c2e30bffe883bb560330f3b6ce03aaf278f75f96d161935b/MarkupSafe-2.1.2-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff"},
-    {url = "https://files.pythonhosted.org/packages/9d/80/8320f182d06a9b289b1a9f266f593feb91d3781c7e104bbe09e0c4c11439/MarkupSafe-2.1.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419"},
-    {url = "https://files.pythonhosted.org/packages/be/18/988e1913a40cc8eb725b1e073eacc130f7803a061577bdc0b9343eb3c696/MarkupSafe-2.1.2-cp37-cp37m-win32.whl", hash = "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859"},
-    {url = "https://files.pythonhosted.org/packages/c3/e5/42842a44bfd9ba2955c562b1139334a2f64cedb687e8969777fd07de42a9/MarkupSafe-2.1.2-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2"},
-    {url = "https://files.pythonhosted.org/packages/c7/0e/22d0c8e6ee84414e251bd1bc555b2705af6b3fb99f0ba1ead2a0f51d423b/MarkupSafe-2.1.2-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa"},
-    {url = "https://files.pythonhosted.org/packages/cf/c1/d7596976a868fe3487212a382cc121358a53dc8e8d85ff2ee2c3d3b40f04/MarkupSafe-2.1.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1"},
-    {url = "https://files.pythonhosted.org/packages/d1/10/ff89b23d4a24051c4e4f689b79ee06f230d7e9431445e24f5dd9d9a89730/MarkupSafe-2.1.2-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed"},
-    {url = "https://files.pythonhosted.org/packages/e3/a9/e366665c7eae59c9c9d34b747cd5a3994847719a2304e0c8dec8b604dd98/MarkupSafe-2.1.2-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013"},
-    {url = "https://files.pythonhosted.org/packages/e6/ff/d2378ca3cb3ac4a37af767b820b0f0bf3f5e9193a6acce0eefc379425c1c/MarkupSafe-2.1.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a"},
-    {url = "https://files.pythonhosted.org/packages/e9/c6/2da36728c1310f141395176556500aeedfdea8c2b02a3b72ba61b69280e8/MarkupSafe-2.1.2-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513"},
-    {url = "https://files.pythonhosted.org/packages/ea/60/2400ba59cf2465fa136487ee7299f52121a9d04b2cf8539ad43ad10e70e8/MarkupSafe-2.1.2-cp311-cp311-win_amd64.whl", hash = "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3"},
-    {url = "https://files.pythonhosted.org/packages/f9/aa/ebcd114deab08f892b1d70badda4436dbad1747f9e5b72cffb3de4c7129d/MarkupSafe-2.1.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65"},
+"jupyterlab-widgets 3.0.7" = [
+    {url = "https://files.pythonhosted.org/packages/46/98/e7ce879b7b5d4871b80e291be967d22e5e66fa43474c476a95fe6231f50d/jupyterlab_widgets-3.0.7-py3-none-any.whl", hash = "sha256:c73f8370338ec19f1bec47254752d6505b03601cbd5a67e6a0b184532f73a459"},
+    {url = "https://files.pythonhosted.org/packages/d4/68/ef3070afff437dc92562241294467112566d3b402d85bb9b32e3fd65352a/jupyterlab_widgets-3.0.7.tar.gz", hash = "sha256:c3a50ed5bf528a0c7a869096503af54702f86dda1db469aee1c92dc0c01b43ca"},
+]
+"loguru 0.7.0" = [
+    {url = "https://files.pythonhosted.org/packages/0c/1d/697cbb4ae54217784c1c4805696efb2fd7a1cbbe4827264a80a49e52b828/loguru-0.7.0.tar.gz", hash = "sha256:1612053ced6ae84d7959dd7d5e431a0532642237ec21f7fd83ac73fe539e03e1"},
+    {url = "https://files.pythonhosted.org/packages/71/bd/337f7a0cd2628c4c77512d78e26f93b13c327a2ddf2132001dd78c000bf4/loguru-0.7.0-py3-none-any.whl", hash = "sha256:b93aa30099fa6860d4727f1b81f8718e965bb96253fa190fab2077aaad6d15d3"},
+]
+"markupsafe 2.1.3" = [
+    {url = "https://files.pythonhosted.org/packages/03/06/e72e88f81f8c91d4f488d21712d2d403fd644e3172eaadc302094377bc22/MarkupSafe-2.1.3-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4"},
+    {url = "https://files.pythonhosted.org/packages/03/65/3473d2cb84bb2cda08be95b97fc4f53e6bcd701a2d50ba7b7c905e1e9273/MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636"},
+    {url = "https://files.pythonhosted.org/packages/10/b3/c2b0a61cc0e1d50dd8a1b663ba4866c667cb58fb35f12475001705001680/MarkupSafe-2.1.3-cp38-cp38-win32.whl", hash = "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5"},
+    {url = "https://files.pythonhosted.org/packages/12/b3/d9ed2c0971e1435b8a62354b18d3060b66c8cb1d368399ec0b9baa7c0ee5/MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52"},
+    {url = "https://files.pythonhosted.org/packages/20/1d/713d443799d935f4d26a4f1510c9e61b1d288592fb869845e5cc92a1e055/MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa"},
+    {url = "https://files.pythonhosted.org/packages/22/81/b5659e2b6ae1516495a22f87370419c1d79c8d853315e6cbe5172fc01a06/MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea"},
+    {url = "https://files.pythonhosted.org/packages/32/d4/ce98c4ca713d91c4a17c1a184785cc00b9e9c25699d618956c2b9999500a/MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9"},
+    {url = "https://files.pythonhosted.org/packages/3c/c8/74d13c999cbb49e3460bf769025659a37ef4a8e884de629720ab4e42dcdb/MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7"},
+    {url = "https://files.pythonhosted.org/packages/43/70/f24470f33b2035b035ef0c0ffebf57006beb2272cf3df068fc5154e04ead/MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc"},
+    {url = "https://files.pythonhosted.org/packages/43/ad/7246ae594aac948b17408c0ff0f9ff0bc470bdbe9c672a754310db64b237/MarkupSafe-2.1.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c"},
+    {url = "https://files.pythonhosted.org/packages/44/53/93405d37bb04a10c43b1bdd6f548097478d494d7eadb4b364e3e1337f0cc/MarkupSafe-2.1.3-cp311-cp311-win32.whl", hash = "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb"},
+    {url = "https://files.pythonhosted.org/packages/47/26/932140621773bfd4df3223fbdd9e78de3477f424f0d2987c313b1cb655ff/MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779"},
+    {url = "https://files.pythonhosted.org/packages/4d/e4/77bb622d6a37aeb51ee55857100986528b7f47d6dbddc35f9b404622ed50/MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc"},
+    {url = "https://files.pythonhosted.org/packages/4f/13/cf36eff21600fb21d5bd8c4c1b6ff0b7cc0ff37b955017210cfc6f367972/MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b"},
+    {url = "https://files.pythonhosted.org/packages/62/9b/4908a57acf39d8811836bc6776b309c2e07d63791485589acf0b6d7bc0c6/MarkupSafe-2.1.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b"},
+    {url = "https://files.pythonhosted.org/packages/68/8d/c33c43c499c19f4b51181e196c9a497010908fc22c5de33551e298aa6a21/MarkupSafe-2.1.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58"},
+    {url = "https://files.pythonhosted.org/packages/6a/86/654dc431513cd4417dfcead8102f22bece2d6abf2f584f0e1cc1524f7b94/MarkupSafe-2.1.3-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198"},
+    {url = "https://files.pythonhosted.org/packages/6d/7c/59a3248f411813f8ccba92a55feaac4bf360d29e2ff05ee7d8e1ef2d7dbf/MarkupSafe-2.1.3.tar.gz", hash = "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad"},
+    {url = "https://files.pythonhosted.org/packages/71/61/f5673d7aac2cf7f203859008bb3fc2b25187aa330067c5e9955e5c5ebbab/MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6"},
+    {url = "https://files.pythonhosted.org/packages/74/a3/54fc60ee2da3ab6d68b1b2daf4897297c597840212ee126e68a4eb89fcd7/MarkupSafe-2.1.3-cp38-cp38-win_amd64.whl", hash = "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc"},
+    {url = "https://files.pythonhosted.org/packages/7d/48/6ba4db436924698ca22109325969e00be459d417830dafec3c1001878b57/MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e"},
+    {url = "https://files.pythonhosted.org/packages/84/a8/c4aebb8a14a1d39d5135eb8233a0b95831cdc42c4088358449c3ed657044/MarkupSafe-2.1.3-cp310-cp310-win_amd64.whl", hash = "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559"},
+    {url = "https://files.pythonhosted.org/packages/8b/bb/72ca339b012054a84753accabe3258e0baf6e34bd0ab6e3670b9a65f679d/MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8"},
+    {url = "https://files.pythonhosted.org/packages/8d/66/4a46c7f1402e0377a8b220fd4b53cc4f1b2337ab0d97f06e23acd1f579d1/MarkupSafe-2.1.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee"},
+    {url = "https://files.pythonhosted.org/packages/96/e4/4db3b1abc5a1fe7295aa0683eafd13832084509c3b8236f3faf8dd4eff75/MarkupSafe-2.1.3-cp310-cp310-win32.whl", hash = "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431"},
+    {url = "https://files.pythonhosted.org/packages/9b/c1/9f44da5ca74f95116c644892152ca6514ecdc34c8297a3f40d886147863d/MarkupSafe-2.1.3-cp37-cp37m-win_amd64.whl", hash = "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24"},
+    {url = "https://files.pythonhosted.org/packages/a2/b2/624042cb58cc6b3529a6c3a7b7d230766e3ecb768cba118ba7befd18ed6f/MarkupSafe-2.1.3-cp39-cp39-win_amd64.whl", hash = "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba"},
+    {url = "https://files.pythonhosted.org/packages/a2/f7/9175ad1b8152092f7c3b78c513c1bdfe9287e0564447d1c2d3d1a2471540/MarkupSafe-2.1.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee"},
+    {url = "https://files.pythonhosted.org/packages/a6/56/f1d4ee39e898a9e63470cbb7fae1c58cce6874f25f54220b89213a47f273/MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f"},
+    {url = "https://files.pythonhosted.org/packages/a8/12/fd9ef3e09a7312d60467c71037283553ff2acfcd950159cd4c3ca9558af4/MarkupSafe-2.1.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2"},
+    {url = "https://files.pythonhosted.org/packages/ab/20/f59423543a8422cb8c69a579ebd0ef2c9dafa70cc8142b7372b5b4073caa/MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e"},
+    {url = "https://files.pythonhosted.org/packages/b2/0d/cbaade3ee8efbd5ce2fb72b48cc51479ebf3d4ce2c54dcb6557d3ea6a950/MarkupSafe-2.1.3-cp37-cp37m-win32.whl", hash = "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0"},
+    {url = "https://files.pythonhosted.org/packages/b2/27/07e5aa9f93314dc65ad2ad9b899656dee79b70a9425ee199dd5a4c4cf2cd/MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3"},
+    {url = "https://files.pythonhosted.org/packages/bb/82/f88ccb3ca6204a4536cf7af5abdad7c3657adac06ab33699aa67279e0744/MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac"},
+    {url = "https://files.pythonhosted.org/packages/be/bb/08b85bc194034efbf572e70c3951549c8eca0ada25363afc154386b5390a/MarkupSafe-2.1.3-cp311-cp311-win_amd64.whl", hash = "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686"},
+    {url = "https://files.pythonhosted.org/packages/bf/b7/c5ba9b7ad9ad21fc4a60df226615cf43ead185d328b77b0327d603d00cc5/MarkupSafe-2.1.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00"},
+    {url = "https://files.pythonhosted.org/packages/c0/c7/171f5ac6b065e1425e8fabf4a4dfbeca76fd8070072c6a41bd5c07d90d8b/MarkupSafe-2.1.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575"},
+    {url = "https://files.pythonhosted.org/packages/c9/80/f08e782943ee7ae6e9438851396d00a869f5b50ea8c6e1f40385f3e95771/MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d"},
+    {url = "https://files.pythonhosted.org/packages/d2/a1/4ae49dd1520c7b891ea4963258aab08fb2554c564781ecb2a9c4afdf9cb1/MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48"},
+    {url = "https://files.pythonhosted.org/packages/d5/c1/1177f712d4ab91eb67f79d763a7b5f9c5851ee3077d6b4eee15e23b6b93e/MarkupSafe-2.1.3-cp39-cp39-win32.whl", hash = "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"},
+    {url = "https://files.pythonhosted.org/packages/de/63/cb7e71984e9159ec5f45b5e81e896c8bdd0e45fe3fc6ce02ab497f0d790e/MarkupSafe-2.1.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e"},
+    {url = "https://files.pythonhosted.org/packages/de/e2/32c14301bb023986dff527a49325b6259cab4ebb4633f69de54af312fc45/MarkupSafe-2.1.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be"},
+    {url = "https://files.pythonhosted.org/packages/e5/dd/49576e803c0d974671e44fa78049217fcc68af3662a24f831525ed30e6c7/MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707"},
+    {url = "https://files.pythonhosted.org/packages/e6/5c/8ab8f67bbbbf90fe88f887f4fa68123435c5415531442e8aefef1e118d5c/MarkupSafe-2.1.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e"},
+    {url = "https://files.pythonhosted.org/packages/f4/a0/103f94793c3bf829a18d2415117334ece115aeca56f2df1c47fa02c6dbd6/MarkupSafe-2.1.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9"},
+    {url = "https://files.pythonhosted.org/packages/f7/9c/86cbd8e0e1d81f0ba420f20539dd459c50537c7751e28102dbfee2b6f28c/MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57"},
+    {url = "https://files.pythonhosted.org/packages/f8/33/e9e83b214b5f8d9a60b26e60051734e7657a416e5bce7d7f1c34e26badad/MarkupSafe-2.1.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0"},
+    {url = "https://files.pythonhosted.org/packages/fa/bb/12fb5964c4a766eb98155dd31ec070adc8a69a395564ffc1e7b34d91335a/MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155"},
+    {url = "https://files.pythonhosted.org/packages/fe/09/c31503cb8150cf688c1534a7135cc39bb9092f8e0e6369ec73494d16ee0e/MarkupSafe-2.1.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c"},
+    {url = "https://files.pythonhosted.org/packages/fe/21/2eff1de472ca6c99ec3993eab11308787b9879af9ca8bbceb4868cf4f2ca/MarkupSafe-2.1.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2"},
 ]
 "matplotlib-inline 0.1.6" = [
     {url = "https://files.pythonhosted.org/packages/d9/50/3af8c0362f26108e54d58c7f38784a3bdae6b9a450bab48ee8482d737f44/matplotlib-inline-0.1.6.tar.gz", hash = "sha256:f887e5f10ba98e8d2b150ddcf4702c1e5f8b3a20005eb0f74bfdbd360ee6f304"},
     {url = "https://files.pythonhosted.org/packages/f2/51/c34d7a1d528efaae3d8ddb18ef45a41f284eacf9e514523b191b7d0872cc/matplotlib_inline-0.1.6-py3-none-any.whl", hash = "sha256:f1f41aab5328aa5aaea9b16d083b128102f8712542f819fe7e6a420ff581b311"},
 ]
 "mccabe 0.7.0" = [
     {url = "https://files.pythonhosted.org/packages/27/1a/1f68f9ba0c207934b35b86a8ca3aad8395a3d6dd7921c0686e23853ff5a9/mccabe-0.7.0-py2.py3-none-any.whl", hash = "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"},
     {url = "https://files.pythonhosted.org/packages/e7/ff/0ffefdcac38932a54d2b5eed4e0ba8a408f215002cd178ad1df0f2806ff8/mccabe-0.7.0.tar.gz", hash = "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325"},
 ]
-"mistune 2.0.4" = [
-    {url = "https://files.pythonhosted.org/packages/3a/c7/b0a4413a4d9b7a4fda0d710fd90dba62375f0d0c4544e848dc7656757c0c/mistune-2.0.4-py2.py3-none-any.whl", hash = "sha256:182cc5ee6f8ed1b807de6b7bb50155df7b66495412836b9a74c8fbdfc75fe36d"},
-    {url = "https://files.pythonhosted.org/packages/cd/9b/0f98334812f548a5ee4399b76e33752a74fc7bb976f5efb34d962f03d585/mistune-2.0.4.tar.gz", hash = "sha256:9ee0a66053e2267aba772c71e06891fa8f1af6d4b01d5e84e267b4570d4d9808"},
-]
-"mypy 0.991" = [
-    {url = "https://files.pythonhosted.org/packages/0e/5c/fbe112ca73d4c6a9e65336f48099c60800514d8949b4129c093a84a28dc8/mypy-0.991.tar.gz", hash = "sha256:3c0165ba8f354a6d9881809ef29f1a9318a236a6d81c690094c5df32107bde06"},
-    {url = "https://files.pythonhosted.org/packages/14/05/5a4206e269268f4aecb1096bf2375a231c959987ccf3e31313221b8bc153/mypy-0.991-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:37bd02ebf9d10e05b00d71302d2c2e6ca333e6c2a8584a98c00e038db8121f05"},
-    {url = "https://files.pythonhosted.org/packages/28/9c/e1805f2fea93a92671f33b00dd577119f37e4a8b859d6f6ea62d3e9129fa/mypy-0.991-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:1c8cd4fb70e8584ca1ed5805cbc7c017a3d1a29fb450621089ffed3e99d1857f"},
-    {url = "https://files.pythonhosted.org/packages/33/20/c4c15c9e9b7929ef44e35e83c0bcc254c8bf5998bbef0954ae658288e8c6/mypy-0.991-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:b86ce2c1866a748c0f6faca5232059f881cda6dda2a893b9a8373353cfe3715a"},
-    {url = "https://files.pythonhosted.org/packages/39/05/7a7d58afc7d00e819e553ad2485a29141e14575e3b0c43b9da6f869ede4c/mypy-0.991-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bc9ec663ed6c8f15f4ae9d3c04c989b744436c16d26580eaa760ae9dd5d662eb"},
-    {url = "https://files.pythonhosted.org/packages/44/d0/81d47bffc80d0cff84174aab266adc3401e735e13c5613418e825c146986/mypy-0.991-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:7d17e0a9707d0772f4a7b878f04b4fd11f6f5bcb9b3813975a9b13c9332153ab"},
-    {url = "https://files.pythonhosted.org/packages/49/83/34d682a10604845d77a0e7dbde1d0e70f3784d0f67b0df11d2eaf7bb8360/mypy-0.991-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a12c56bf73cdab116df96e4ff39610b92a348cc99a1307e1da3c3768bbb5b135"},
-    {url = "https://files.pythonhosted.org/packages/4b/98/125e5d14222de8e92f44314f8df21a9c351b531b37c551526acd67486a7d/mypy-0.991-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:26efb2fcc6b67e4d5a55561f39176821d2adf88f2745ddc72751b7890f3194ad"},
-    {url = "https://files.pythonhosted.org/packages/5d/c8/fc9b7cd600330e8c9dbd52b499a76eeaf4b48969a605fb50415a9d361d5b/mypy-0.991-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:652b651d42f155033a1967739788c436491b577b6a44e4c39fb340d0ee7f0d70"},
-    {url = "https://files.pythonhosted.org/packages/6b/22/5e19d1a6f8e029296e7b2fa462d8753fb4365126684c2f840dcb1447e6e8/mypy-0.991-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6d7464bac72a85cb3491c7e92b5b62f3dcccb8af26826257760a552a5e244aa5"},
-    {url = "https://files.pythonhosted.org/packages/80/23/76e56e004acca691b4da4086a8c38bd67b7ae73536848dcab76cfed5c188/mypy-0.991-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:4307270436fd7694b41f913eb09210faff27ea4979ecbcd849e57d2da2f65305"},
-    {url = "https://files.pythonhosted.org/packages/87/ec/62fd00fa5d8ead3ecafed3eb99ee805911f41b11536c5940df1bcb2c845d/mypy-0.991-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:0c8f3be99e8a8bd403caa8c03be619544bc2c77a7093685dcf308c6b109426c6"},
-    {url = "https://files.pythonhosted.org/packages/89/76/7159258fdbf26a5ceef100b80a82d2f79b9066725a5daeb6383a8f773910/mypy-0.991-cp311-cp311-win_amd64.whl", hash = "sha256:3a700330b567114b673cf8ee7388e949f843b356a73b5ab22dd7cff4742a5297"},
-    {url = "https://files.pythonhosted.org/packages/90/a5/3a2c0c02e99a845318cc25556097d96eb8eb85fe53619ac8ff37b44acc46/mypy-0.991-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:3d80e36b7d7a9259b740be6d8d906221789b0d836201af4234093cae89ced0cd"},
-    {url = "https://files.pythonhosted.org/packages/91/27/716b1cfce990cb58dc92f6601852141bc25e1524c06b3f3a39b0de6d9210/mypy-0.991-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:c9166b3f81a10cdf9b49f2d594b21b31adadb3d5e9db9b834866c3258b695be3"},
-    {url = "https://files.pythonhosted.org/packages/97/e3/1da0f08c60f555c04b93eff4016611fa1858ea53111dbdc757a37c234042/mypy-0.991-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:641411733b127c3e0dab94c45af15fea99e4468f99ac88b39efb1ad677da5711"},
-    {url = "https://files.pythonhosted.org/packages/9b/b1/0d5f1549c2894fd9af744e886156870d98ea0b1784952989f10e51eb0030/mypy-0.991-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:1f7d1a520373e2272b10796c3ff721ea1a0712288cafaa95931e66aa15798813"},
-    {url = "https://files.pythonhosted.org/packages/ac/a6/e4d6dca539c637735d0d93f1eee3ac35cedfd9c047da7386b3a59e93f35b/mypy-0.991-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:5e80e758243b97b618cdf22004beb09e8a2de1af481382e4d84bc52152d1c476"},
-    {url = "https://files.pythonhosted.org/packages/af/9a/ee3b76f36e90ecb5e44dd2827bf5992d02c127192366a4c7864cfeab95b6/mypy-0.991-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:0cca5adf694af539aeaa6ac633a7afe9bbd760df9d31be55ab780b77ab5ae8bf"},
-    {url = "https://files.pythonhosted.org/packages/b1/30/24a92552a7c3df25db5a2e56ae359b4aa9bba6aebc8f0e25523a94e5c1e7/mypy-0.991-cp37-cp37m-win_amd64.whl", hash = "sha256:e62ebaad93be3ad1a828a11e90f0e76f15449371ffeecca4a0a0b9adc99abcef"},
-    {url = "https://files.pythonhosted.org/packages/b8/ab/aa2e02fce8ee8885fe98ee2a0549290e9de5caa28febc0cf243bfab020e7/mypy-0.991-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:d13674f3fb73805ba0c45eb6c0c3053d218aa1f7abead6e446d474529aafc372"},
-    {url = "https://files.pythonhosted.org/packages/bc/b2/6e71e47b259992dcd99d257ce452c0de3f711be713d048fe8f0fda9a9996/mypy-0.991-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:98e781cd35c0acf33eb0295e8b9c55cdbef64fcb35f6d3aa2186f289bed6e80d"},
-    {url = "https://files.pythonhosted.org/packages/ca/0d/da98f81e7c13a60111dc10a16cbf1b48dc8500df90a1fc959878a5981f49/mypy-0.991-cp39-cp39-win_amd64.whl", hash = "sha256:74e259b5c19f70d35fcc1ad3d56499065c601dfe94ff67ae48b85596b9ec1461"},
-    {url = "https://files.pythonhosted.org/packages/d7/f4/dcab9f3c5ed410caca1b9374dbb2b2caa778d225e32f174e266e20291edf/mypy-0.991-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:0714258640194d75677e86c786e80ccf294972cc76885d3ebbb560f11db0003d"},
-    {url = "https://files.pythonhosted.org/packages/df/bb/3cf400e05e30939a0fc58b34e0662d8abe8e206464665065b56cf2ca9a62/mypy-0.991-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:209ee89fbb0deed518605edddd234af80506aec932ad28d73c08f1400ef80a33"},
-    {url = "https://files.pythonhosted.org/packages/e3/84/188ddeaebfc8b5bbdcc3c7f05c09b61758540b2df84aad0146263d66960a/mypy-0.991-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:ac6e503823143464538efda0e8e356d871557ef60ccd38f8824a4257acc18d93"},
-    {url = "https://files.pythonhosted.org/packages/e7/a1/c503a15ad69ff133a76c159b8287f0eadc1f521d9796bf81f935886c98f6/mypy-0.991-py3-none-any.whl", hash = "sha256:de32edc9b0a7e67c2775e574cb061a537660e51210fbf6006b0b36ea695ae9bb"},
-    {url = "https://files.pythonhosted.org/packages/e9/7e/cc2de45afb46fee694bf285f91df3e227a3b0c671f775524814549c26556/mypy-0.991-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b8472f736a5bfb159a5e36740847808f6f5b659960115ff29c7cecec1741c648"},
-    {url = "https://files.pythonhosted.org/packages/f3/1d/cc67a674f1cd7f1c10619487a4245185f6f8f14cbd685b60709318e9ac27/mypy-0.991-cp310-cp310-win_amd64.whl", hash = "sha256:901c2c269c616e6cb0998b33d4adbb4a6af0ac4ce5cd078afd7bc95830e62c1c"},
-    {url = "https://files.pythonhosted.org/packages/f7/3a/19c01d59d24f1f36fabdeb61a286b4fc5e0456bf6211f5159ad5ebb5f735/mypy-0.991-cp38-cp38-win_amd64.whl", hash = "sha256:4175593dc25d9da12f7de8de873a33f9b2b8bdb4e827a7cae952e5b1a342e243"},
-]
-"mypy-extensions 0.4.3" = [
-    {url = "https://files.pythonhosted.org/packages/5c/eb/975c7c080f3223a5cdaff09612f3a5221e4ba534f7039db34c35d95fa6a5/mypy_extensions-0.4.3-py2.py3-none-any.whl", hash = "sha256:090fedd75945a69ae91ce1303b5824f428daf5a028d2f6ab8a299250a846f15d"},
-    {url = "https://files.pythonhosted.org/packages/63/60/0582ce2eaced55f65a4406fc97beba256de4b7a95a0034c6576458c6519f/mypy_extensions-0.4.3.tar.gz", hash = "sha256:2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8"},
-]
-"nbclassic 0.4.8" = [
-    {url = "https://files.pythonhosted.org/packages/0d/52/2fd9c7a81763d7e20cc28757d42ae25d8f0fcab2913092b2e239b906892a/nbclassic-0.4.8.tar.gz", hash = "sha256:c74d8a500f8e058d46b576a41e5bc640711e1032cf7541dde5f73ea49497e283"},
-    {url = "https://files.pythonhosted.org/packages/a6/85/2a240df7326b7311ebd926c12d7df5394aef2f9f76ffbb294079cc43960e/nbclassic-0.4.8-py3-none-any.whl", hash = "sha256:cbf05df5842b420d5cece0143462380ea9d308ff57c2dc0eb4d6e035b18fbfb3"},
-]
-"nbclient 0.7.2" = [
-    {url = "https://files.pythonhosted.org/packages/15/49/ea7a0c7e649c54883d76f5119a3e0be592d82a7df1a9b87124fa6663d9c7/nbclient-0.7.2-py3-none-any.whl", hash = "sha256:d97ac6257de2794f5397609df754fcbca1a603e94e924eb9b99787c031ae2e7c"},
-    {url = "https://files.pythonhosted.org/packages/19/ab/3508807c537cca591f85bb28bb914b9b64fd9f4dfa70e0847cf514c5fbd0/nbclient-0.7.2.tar.gz", hash = "sha256:884a3f4a8c4fc24bb9302f263e0af47d97f0d01fe11ba714171b320c8ac09547"},
-]
-"nbconvert 7.2.8" = [
-    {url = "https://files.pythonhosted.org/packages/21/be/5411c7d2e10f103bb760b8710955c594d2c9d9db04ecb51e763136beacfe/nbconvert-7.2.8-py3-none-any.whl", hash = "sha256:ac57f2812175441a883f50c8ff113133ca65fe7ae5a9f1e3da3bfd1a70dce2ee"},
-    {url = "https://files.pythonhosted.org/packages/78/10/f10deed3a5cd565c16d80088dbcb7eadd9f2f1f03061c98d4599100d4a45/nbconvert-7.2.8.tar.gz", hash = "sha256:ccedacde57a972836bfb46466485be29ed1364ed7c2f379f62bad47d340ece99"},
-]
-"nbformat 5.7.3" = [
-    {url = "https://files.pythonhosted.org/packages/21/ad/020fed74bfde983a3b70cc95843d6adbe59171aa9a3da5aab403aa722a17/nbformat-5.7.3-py3-none-any.whl", hash = "sha256:22a98a6516ca216002b0a34591af5bcb8072ca6c63910baffc901cfa07fefbf0"},
-    {url = "https://files.pythonhosted.org/packages/ce/42/fae44dfe70960c488e5b9b53c617dedd1c7932aff1962c59b2a923e82bb8/nbformat-5.7.3.tar.gz", hash = "sha256:4b021fca24d3a747bf4e626694033d792d594705829e5e35b14ee3369f9f6477"},
+"mistune 2.0.5" = [
+    {url = "https://files.pythonhosted.org/packages/9f/e5/780d22d19543f339aad583304f58002975b586757aa590cbe7bea5cc6f13/mistune-2.0.5-py2.py3-none-any.whl", hash = "sha256:bad7f5d431886fcbaf5f758118ecff70d31f75231b34024a1341120340a65ce8"},
+    {url = "https://files.pythonhosted.org/packages/fb/6b/d8013058fcdb0088b4130164fc961e15c50d30302f60a349c16bdfda9770/mistune-2.0.5.tar.gz", hash = "sha256:0246113cb2492db875c6be56974a7c893333bf26cd92891c85f63151cee09d34"},
+]
+"mypy 1.3.0" = [
+    {url = "https://files.pythonhosted.org/packages/09/7b/8eb0d648352c61b08cb364d278b5c12c3f1c5841724fdd2929d7172b7eaf/mypy-1.3.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:f9dca1e257d4cc129517779226753dbefb4f2266c4eaad610fc15c6a7e14283e"},
+    {url = "https://files.pythonhosted.org/packages/11/41/d24f93eefc89c650782bf1f9acfdb02a32f327b841058a5b0ce5857b60af/mypy-1.3.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:4c99c3ecf223cf2952638da9cd82793d8f3c0c5fa8b6ae2b2d9ed1e1ff51ba85"},
+    {url = "https://files.pythonhosted.org/packages/25/c7/4735f81858a727e170279144600881fe3299aa7589ed585af6b788ea4556/mypy-1.3.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:6e33bb8b2613614a33dff70565f4c803f889ebd2f859466e42b46e1df76018dd"},
+    {url = "https://files.pythonhosted.org/packages/2b/27/4a26f91301804969194ee0dc9393843f10566d7fdf192ce11fc0218a989d/mypy-1.3.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c1eb485cea53f4f5284e5baf92902cd0088b24984f4209e25981cc359d64448d"},
+    {url = "https://files.pythonhosted.org/packages/3c/5d/b87339c1fdfec7d13899cd7ad2ee992801695114c1cf9e1645da264cd437/mypy-1.3.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:74bc9b6e0e79808bf8678d7678b2ae3736ea72d56eede3820bd3849823e7f305"},
+    {url = "https://files.pythonhosted.org/packages/47/f6/25c154bb1c479f2047093f0580c2c35ffc1ff007d52b7e50020cca60c010/mypy-1.3.0-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:76ec771e2342f1b558c36d49900dfe81d140361dd0d2df6cd71b3db1be155409"},
+    {url = "https://files.pythonhosted.org/packages/4c/10/530d2df4d57f46f77b8211cf9bbe090baacff02e7076f21f1bf08148d541/mypy-1.3.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:ddae0f39ca146972ff6bb4399f3b2943884a774b8771ea0a8f50e971f5ea5ba8"},
+    {url = "https://files.pythonhosted.org/packages/55/e1/90487a3ea5a88b8f5c9d7fbf6f5fa7fcc8633d0132ce8364810a1da901c9/mypy-1.3.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:cbc07246253b9e3d7d74c9ff948cd0fd7a71afcc2b77c7f0a59c26e9395cb152"},
+    {url = "https://files.pythonhosted.org/packages/5b/fb/0b1c90c635319b98dd65c6d6d6347413e42397e94057993011eeedeffbd9/mypy-1.3.0-cp37-cp37m-win_amd64.whl", hash = "sha256:8c5979d0deb27e0f4479bee18ea0f83732a893e81b78e62e2dda3e7e518c92ee"},
+    {url = "https://files.pythonhosted.org/packages/6a/d0/4681d84878cecfd911752016ab30566366f6de7296fdc977b746eb68bf45/mypy-1.3.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:7d23370d2a6b7a71dc65d1266f9a34e4cde9e8e21511322415db4b26f46f6b8c"},
+    {url = "https://files.pythonhosted.org/packages/6a/d9/48de5203f4b6287a98fadcc47072b1bc69e3faaa39cba59a3a600b05a42c/mypy-1.3.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:6e42d29e324cdda61daaec2336c42512e59c7c375340bd202efa1fe0f7b8f8ca"},
+    {url = "https://files.pythonhosted.org/packages/7e/75/021af7f0683ea19b9ad6a436e1b5c7cb39899c0f7b31040fa69b2395421e/mypy-1.3.0-cp310-cp310-win_amd64.whl", hash = "sha256:a22435632710a4fcf8acf86cbd0d69f68ac389a3892cb23fbad176d1cddaf228"},
+    {url = "https://files.pythonhosted.org/packages/86/56/08c5ff6b2139f301d9aa56cb8e7b2a24d4faa6fc3e94234dfe7eeecc9c44/mypy-1.3.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:faff86aa10c1aa4a10e1a301de160f3d8fc8703b88c7e98de46b531ff1276a9a"},
+    {url = "https://files.pythonhosted.org/packages/88/0e/646696eb8fe7658b752009a495054a0214ae8e659e9cbcde8181f16ae999/mypy-1.3.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:658fe7b674769a0770d4b26cb4d6f005e88a442fe82446f020be8e5f5efb2fae"},
+    {url = "https://files.pythonhosted.org/packages/8d/c8/681f4a19c62aa71bdc9ad3a4bc9a0fb8846bd0b5a8bc1b29d261c8025f80/mypy-1.3.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:550a8b3a19bb6589679a7c3c31f64312e7ff482a816c96e0cecec9ad3a7564dd"},
+    {url = "https://files.pythonhosted.org/packages/90/b6/a2d2ba604982af6034e3fcad17a464a66127be47f07b4587beec76e8f80b/mypy-1.3.0-cp38-cp38-win_amd64.whl", hash = "sha256:44797d031a41516fcf5cbfa652265bb994e53e51994c1bd649ffcd0c3a7eccbf"},
+    {url = "https://files.pythonhosted.org/packages/b1/ce/8d87f684bb7e2a520cfa9cd17b8dc686a83143bb12a3e1ac4ad6d8d4825c/mypy-1.3.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:c5d2cc54175bab47011b09688b418db71403aefad07cbcd62d44010543fc143f"},
+    {url = "https://files.pythonhosted.org/packages/b1/e1/399e3dfeb2842e4a2634866e4ef8b69151d465b7a5ceb648d7f1296f17d0/mypy-1.3.0-cp39-cp39-win_amd64.whl", hash = "sha256:95d8d31a7713510685b05fbb18d6ac287a56c8f6554d88c19e73f724a445448a"},
+    {url = "https://files.pythonhosted.org/packages/b8/36/6628916f94bb0816e1719117e1962750413ab408f83673ce7d571caf3960/mypy-1.3.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:1c4c42c60a8103ead4c1c060ac3cdd3ff01e18fddce6f1016e08939647a0e703"},
+    {url = "https://files.pythonhosted.org/packages/ba/ac/1c280246fc0c5239409f31e1a321f178ba11a9c6e5eaaf6d56f9ff627cdf/mypy-1.3.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e86c2c6852f62f8f2b24cb7a613ebe8e0c7dc1402c61d36a609174f63e0ff017"},
+    {url = "https://files.pythonhosted.org/packages/c9/c5/f3e4ed59e08e3a728a15da198317edfcd13b7dc2215d52b5d85fce716285/mypy-1.3.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:87df44954c31d86df96c8bd6e80dfcd773473e877ac6176a8e29898bfb3501cb"},
+    {url = "https://files.pythonhosted.org/packages/cd/b9/6abe1cd8ac8e70f12f43eebe6427814f9d36142d331eae5cc5bba77585a2/mypy-1.3.0-cp311-cp311-win_amd64.whl", hash = "sha256:d0b6c62206e04061e27009481cb0ec966f7d6172b5b936f3ead3d74f29fe3dcf"},
+    {url = "https://files.pythonhosted.org/packages/d8/c6/de2e214a42b63d7ea0abef9f02a6da69cad6d532165bb7a8cc8291099a0c/mypy-1.3.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:473117e310febe632ddf10e745a355714e771ffe534f06db40702775056614c4"},
+    {url = "https://files.pythonhosted.org/packages/d9/79/82d452b409d7610944ba3a1a6079987d3ed6062cb8fe5c8850f26dafb6e0/mypy-1.3.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ebc95f8386314272bbc817026f8ce8f4f0d2ef7ae44f947c4664efac9adec929"},
+    {url = "https://files.pythonhosted.org/packages/e3/f7/1fed3b24abb75f244fa6bc60ea03cd9d3d8ad225a4cfda7533042fe6d831/mypy-1.3.0-py3-none-any.whl", hash = "sha256:a8763e72d5d9574d45ce5881962bc8e9046bf7b375b0abf031f3e6811732a897"},
+    {url = "https://files.pythonhosted.org/packages/f9/88/3bfe07521fb9e74b449cbc4367434067ec70bfd8a24c652fa3e0f9597389/mypy-1.3.0.tar.gz", hash = "sha256:e1f4d16e296f5135624b34e8fb741eb0eadedca90862405b1f1fde2040b9bd11"},
+]
+"mypy-extensions 1.0.0" = [
+    {url = "https://files.pythonhosted.org/packages/2a/e2/5d3f6ada4297caebe1a2add3b126fe800c96f56dbe5d1988a2cbe0b267aa/mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
+    {url = "https://files.pythonhosted.org/packages/98/a4/1ab47638b92648243faf97a5aeb6ea83059cc3624972ab6b8d2316078d3f/mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
+]
+"nbclassic 1.0.0" = [
+    {url = "https://files.pythonhosted.org/packages/84/ae/eaa71c0ed64e8ddc426a4c902e83d31c4925e9d3418d6b240dd5752b6e71/nbclassic-1.0.0-py3-none-any.whl", hash = "sha256:f99e4769b4750076cd4235c044b61232110733322384a94a63791d2e7beacc66"},
+    {url = "https://files.pythonhosted.org/packages/8b/11/6e6084bad2b2f8faa787bd5f72fd1171c741801a03872b518965d7653ba5/nbclassic-1.0.0.tar.gz", hash = "sha256:0ae11eb2319455d805596bf320336cda9554b41d99ab9a3c31bf8180bffa30e3"},
+]
+"nbclient 0.7.4" = [
+    {url = "https://files.pythonhosted.org/packages/c8/ee/b9351110fbbc8229863cbc54454f1db91f7836c730018d674a188ede5efd/nbclient-0.7.4.tar.gz", hash = "sha256:d447f0e5a4cfe79d462459aec1b3dc5c2e9152597262be8ee27f7d4c02566a0d"},
+    {url = "https://files.pythonhosted.org/packages/f3/97/d35da363d1df4a68f1b3d44335f80235487d7ca77d1f606b0c3523118f34/nbclient-0.7.4-py3-none-any.whl", hash = "sha256:c817c0768c5ff0d60e468e017613e6eae27b6fa31e43f905addd2d24df60c125"},
+]
+"nbconvert 7.4.0" = [
+    {url = "https://files.pythonhosted.org/packages/0f/24/a7f5d67535ebd13276a1113d1a20572053c5a9182c29651420b957d1226c/nbconvert-7.4.0.tar.gz", hash = "sha256:51b6c77b507b177b73f6729dba15676e42c4e92bcb00edc8cc982ee72e7d89d7"},
+    {url = "https://files.pythonhosted.org/packages/2f/90/79bf16b584f5150550b0c175ca7a6e88334226e9275cf16db13785105d73/nbconvert-7.4.0-py3-none-any.whl", hash = "sha256:af5064a9db524f9f12f4e8be7f0799524bd5b14c1adea37e34e83c95127cc818"},
+]
+"nbformat 5.8.0" = [
+    {url = "https://files.pythonhosted.org/packages/08/b7/8b964e977438037b57de31d312d67046e215295899107576e3708b0ea223/nbformat-5.8.0.tar.gz", hash = "sha256:46dac64c781f1c34dfd8acba16547024110348f9fc7eab0f31981c2a3dc48d1f"},
+    {url = "https://files.pythonhosted.org/packages/1d/f6/38f4694b5035306a8c2685e9e6ea7bf46ea344c03422d7131442ac9677c1/nbformat-5.8.0-py3-none-any.whl", hash = "sha256:d910082bd3e0bffcf07eabf3683ed7dda0727a326c446eeb2922abe102e65162"},
 ]
 "nest-asyncio 1.5.6" = [
     {url = "https://files.pythonhosted.org/packages/35/76/64c51c1cbe704ad79ef6ec82f232d1893b9365f2ff194111787dc91b004f/nest_asyncio-1.5.6.tar.gz", hash = "sha256:d267cc1ff794403f7df692964d1d2a3fa9418ffea2a3f6859a439ff482fef290"},
     {url = "https://files.pythonhosted.org/packages/e9/1a/6dd9ec31cfdb34cef8fea0055b593ee779a6f63c8e8038ad90d71b7f53c0/nest_asyncio-1.5.6-py3-none-any.whl", hash = "sha256:b9a953fb40dceaa587d109609098db21900182b16440652454a146cffb06e8b8"},
 ]
-"notebook 6.5.2" = [
-    {url = "https://files.pythonhosted.org/packages/41/15/a4285abb25c87dec3002cd7eab88320ef21448effdd3714840695aafab12/notebook-6.5.2.tar.gz", hash = "sha256:c1897e5317e225fc78b45549a6ab4b668e4c996fd03a04e938fe5e7af2bfffd0"},
-    {url = "https://files.pythonhosted.org/packages/db/40/2d321ba572dc9a94a090d92c9826291a1dcee1e05bc6c1d641ce419b701d/notebook-6.5.2-py3-none-any.whl", hash = "sha256:e04f9018ceb86e4fa841e92ea8fb214f8d23c1cedfde530cc96f92446924f0e4"},
-]
-"notebook-shim 0.2.2" = [
-    {url = "https://files.pythonhosted.org/packages/29/34/b3d57a23287c55fe964da403bb5457baacc2c0edc1fc3bf2739d4a958d90/notebook_shim-0.2.2-py3-none-any.whl", hash = "sha256:9c6c30f74c4fbea6fce55c1be58e7fd0409b1c681b075dcedceb005db5026949"},
-    {url = "https://files.pythonhosted.org/packages/98/29/3b1be2556ebb55053ffc2d2cac7bf2d611827a2cf23e1f34acc1c811d23f/notebook_shim-0.2.2.tar.gz", hash = "sha256:090e0baf9a5582ff59b607af523ca2db68ff216da0c69956b62cab2ef4fc9c3f"},
-]
-"packaging 23.0" = [
-    {url = "https://files.pythonhosted.org/packages/47/d5/aca8ff6f49aa5565df1c826e7bf5e85a6df852ee063600c1efa5b932968c/packaging-23.0.tar.gz", hash = "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"},
-    {url = "https://files.pythonhosted.org/packages/ed/35/a31aed2993e398f6b09a790a181a7927eb14610ee8bbf02dc14d31677f1c/packaging-23.0-py3-none-any.whl", hash = "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2"},
+"notebook 6.5.4" = [
+    {url = "https://files.pythonhosted.org/packages/52/1e/b555b6e33c962a605e2e85b6014f609d3e1c6a5ff48f7c2480376b430d96/notebook-6.5.4.tar.gz", hash = "sha256:517209568bd47261e2def27a140e97d49070602eea0d226a696f42a7f16c9a4e"},
+    {url = "https://files.pythonhosted.org/packages/7a/21/0e7683e7c4d51b8f6cc5df9bbd33fb2d1e114b9e5dcddeef96ebd8e86348/notebook-6.5.4-py3-none-any.whl", hash = "sha256:dd17e78aefe64c768737b32bf171c1c766666a21cc79a44d37a1700771cab56f"},
+]
+"notebook-shim 0.2.3" = [
+    {url = "https://files.pythonhosted.org/packages/ea/10/6c6c7adc0d61e72cfc4055d0671bbd12bdc6ffea86892e903bd2398b9019/notebook_shim-0.2.3.tar.gz", hash = "sha256:f69388ac283ae008cd506dda10d0288b09a017d822d5e8c7129a152cbd3ce7e9"},
+    {url = "https://files.pythonhosted.org/packages/f4/79/73250372e5bbab63018b41b02d5cc6b395655ec6c1254e477ef7c913aada/notebook_shim-0.2.3-py3-none-any.whl", hash = "sha256:a83496a43341c1674b093bfcebf0fe8e74cbe7eda5fd2bbc56f8e39e1486c0c7"},
+]
+"packaging 23.1" = [
+    {url = "https://files.pythonhosted.org/packages/ab/c3/57f0601a2d4fe15de7a553c00adbc901425661bf048f2a22dfc500caf121/packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
+    {url = "https://files.pythonhosted.org/packages/b9/6c/7c6658d258d7971c5eb0d9b69fa9265879ec9a9158031206d47800ae2213/packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 "pandocfilters 1.5.0" = [
     {url = "https://files.pythonhosted.org/packages/5e/a8/878258cffd53202a6cc1903c226cf09e58ae3df6b09f8ddfa98033286637/pandocfilters-1.5.0-py2.py3-none-any.whl", hash = "sha256:33aae3f25fd1a026079f5d27bdd52496f0e0803b3469282162bafdcbdf6ef14f"},
     {url = "https://files.pythonhosted.org/packages/62/42/c32476b110a2d25277be875b82b5669f2cdda7897c165bd22b78f366b3cb/pandocfilters-1.5.0.tar.gz", hash = "sha256:0b679503337d233b4339a817bfc8c50064e2eff681314376a47cb582305a7a38"},
 ]
 "parso 0.8.3" = [
     {url = "https://files.pythonhosted.org/packages/05/63/8011bd08a4111858f79d2b09aad86638490d62fbf881c44e434a6dfca87b/parso-0.8.3-py2.py3-none-any.whl", hash = "sha256:c001d4636cd3aecdaf33cbb40aebb59b094be2a74c556778ef5576c175e19e75"},
     {url = "https://files.pythonhosted.org/packages/a2/0e/41f0cca4b85a6ea74d66d2226a7cda8e41206a624f5b330b958ef48e2e52/parso-0.8.3.tar.gz", hash = "sha256:8c07be290bb59f03588915921e29e8a50002acaf2cdc5fa0e0114f91709fafa0"},
 ]
-"pathspec 0.10.3" = [
-    {url = "https://files.pythonhosted.org/packages/32/1a/6baf904503c3e943cae9605c9c88a43b964dea5b59785cf956091b341b08/pathspec-0.10.3.tar.gz", hash = "sha256:56200de4077d9d0791465aa9095a01d421861e405b5096955051deefd697d6f6"},
-    {url = "https://files.pythonhosted.org/packages/3c/29/c07c3a976dbe37c56e381e058c11e8738cb3a0416fc842a310461f8bb695/pathspec-0.10.3-py3-none-any.whl", hash = "sha256:3c95343af8b756205e2aba76e843ba9520a24dd84f68c22b9f93251507509dd6"},
+"pathspec 0.11.1" = [
+    {url = "https://files.pythonhosted.org/packages/95/60/d93628975242cc515ab2b8f5b2fc831d8be2eff32f5a1be4776d49305d13/pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
+    {url = "https://files.pythonhosted.org/packages/be/c8/551a803a6ebb174ec1c124e68b449b98a0961f0b737def601e3c1fbb4cfd/pathspec-0.11.1-py3-none-any.whl", hash = "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"},
 ]
 "pexpect 4.8.0" = [
     {url = "https://files.pythonhosted.org/packages/39/7b/88dbb785881c28a102619d46423cb853b46dbccc70d3ac362d99773a78ce/pexpect-4.8.0-py2.py3-none-any.whl", hash = "sha256:0b48a55dcb3c05f3329815901ea4fc1537514d6ba867a152b581d69ae3710937"},
     {url = "https://files.pythonhosted.org/packages/e5/9b/ff402e0e930e70467a7178abb7c128709a30dfb22d8777c043e501bc1b10/pexpect-4.8.0.tar.gz", hash = "sha256:fc65a43959d153d0114afe13997d439c22823a27cefceb5ff35c2178c6784c0c"},
 ]
 "pickleshare 0.7.5" = [
     {url = "https://files.pythonhosted.org/packages/9a/41/220f49aaea88bc6fa6cba8d05ecf24676326156c23b991e80b3f2fc24c77/pickleshare-0.7.5-py2.py3-none-any.whl", hash = "sha256:9649af414d74d4df115d5d718f82acb59c9d418196b7b4290ed47a12ce62df56"},
     {url = "https://files.pythonhosted.org/packages/d8/b6/df3c1c9b616e9c0edbc4fbab6ddd09df9535849c64ba51fcb6531c32d4d8/pickleshare-0.7.5.tar.gz", hash = "sha256:87683d47965c1da65cdacaf31c8441d12b8044cdec9aca500cd78fc2c683afca"},
 ]
 "pkgutil-resolve-name 1.3.10" = [
     {url = "https://files.pythonhosted.org/packages/70/f2/f2891a9dc37398696ddd945012b90ef8d0a034f0012e3f83c3f7a70b0f79/pkgutil_resolve_name-1.3.10.tar.gz", hash = "sha256:357d6c9e6a755653cfd78893817c0853af365dd51ec97f3d358a819373bbd174"},
     {url = "https://files.pythonhosted.org/packages/c9/5c/3d4882ba113fd55bdba9326c1e4c62a15e674a2501de4869e6bd6301f87e/pkgutil_resolve_name-1.3.10-py3-none-any.whl", hash = "sha256:ca27cc078d25c5ad71a9de0a7a330146c4e014c2462d9af19c6b828280649c5e"},
 ]
-"platformdirs 2.6.2" = [
-    {url = "https://files.pythonhosted.org/packages/c1/c7/9be9d651b93efce682b45142a6267034fc4215972780748618c02e236361/platformdirs-2.6.2-py3-none-any.whl", hash = "sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490"},
-    {url = "https://files.pythonhosted.org/packages/cf/4d/198b7e6c6c2b152f4f9f4cdf975d3590e33e63f1920f2d89af7f0390e6db/platformdirs-2.6.2.tar.gz", hash = "sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2"},
+"platformdirs 3.5.1" = [
+    {url = "https://files.pythonhosted.org/packages/89/7e/c6ff9ddcf93b9b36c90d88111c4db354afab7f9a58c7ac3257fa717f1268/platformdirs-3.5.1-py3-none-any.whl", hash = "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"},
+    {url = "https://files.pythonhosted.org/packages/9c/0e/ae9ef1049d4b5697e79250c4b2e72796e4152228e67733389868229c92bb/platformdirs-3.5.1.tar.gz", hash = "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f"},
 ]
 "pluggy 1.0.0" = [
     {url = "https://files.pythonhosted.org/packages/9e/01/f38e2ff29715251cf25532b9082a1589ab7e4f571ced434f98d0139336dc/pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
     {url = "https://files.pythonhosted.org/packages/a1/16/db2d7de3474b6e37cbb9c008965ee63835bba517e22cdb8c35b5116b5ce1/pluggy-1.0.0.tar.gz", hash = "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159"},
 ]
-"prometheus-client 0.15.0" = [
-    {url = "https://files.pythonhosted.org/packages/2e/5e/4225463cdac1098aac718b1d8adf8f9dc3d6aaea55f4f85a2f7d572b4f7c/prometheus_client-0.15.0-py3-none-any.whl", hash = "sha256:db7c05cbd13a0f79975592d112320f2605a325969b270a94b71dcabc47b931d2"},
-    {url = "https://files.pythonhosted.org/packages/ae/ae/04b27ea04f67f91f10b1379d8fd6729c41ac0bcefbb0af603850b3fa32e0/prometheus_client-0.15.0.tar.gz", hash = "sha256:be26aa452490cfcf6da953f9436e95a9f2b4d578ca80094b4458930e5f584ab1"},
-]
-"prompt-toolkit 3.0.36" = [
-    {url = "https://files.pythonhosted.org/packages/eb/37/791f1a6edd13c61cac85282368aa68cb0f3f164440fdf60032f2cc6ca34e/prompt_toolkit-3.0.36-py3-none-any.whl", hash = "sha256:aa64ad242a462c5ff0363a7b9cfe696c20d55d9fc60c11fd8e632d064804d305"},
-    {url = "https://files.pythonhosted.org/packages/fb/93/180be2342f89f16543ec4eb3f25083b5b84eba5378f68efff05409fb39a9/prompt_toolkit-3.0.36.tar.gz", hash = "sha256:3e163f254bef5a03b146397d7c1963bd3e2812f0964bb9a24e6ec761fd28db63"},
-]
-"psutil 5.9.4" = [
-    {url = "https://files.pythonhosted.org/packages/1d/80/e1502ba4ff65390bd17b4612010762075f64f5a0e7c28e889c4820bd95a9/psutil-5.9.4-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:3ff89f9b835100a825b14c2808a106b6fdcc4b15483141482a12c725e7f78549"},
-    {url = "https://files.pythonhosted.org/packages/25/6e/ba97809175c90cbdcd33b470e466ebf0854d15d1506e605cc0ddd284d5b6/psutil-5.9.4-cp36-abi3-win_amd64.whl", hash = "sha256:fd8522436a6ada7b4aad6638662966de0d61d241cb821239b2ae7013d41a43d4"},
-    {url = "https://files.pythonhosted.org/packages/3d/7d/d05864a69e452f003c0d77e728e155a89a2a26b09e64860ddd70ad64fb26/psutil-5.9.4.tar.gz", hash = "sha256:3d7f9739eb435d4b1338944abe23f49584bde5395f27487d2ee25ad9a8774a62"},
-    {url = "https://files.pythonhosted.org/packages/3e/af/fe14b984e8b0f778d502d387b789d846cb2fcc3989f63be942741266d8c8/psutil-5.9.4-cp36-abi3-win32.whl", hash = "sha256:149555f59a69b33f056ba1c4eb22bb7bf24332ce631c44a319cec09f876aaeff"},
-    {url = "https://files.pythonhosted.org/packages/53/ae/536719016fe9399187dbf52cdc65aef942f82b75924495918a2f701bcb77/psutil-5.9.4-cp27-cp27m-win32.whl", hash = "sha256:852dd5d9f8a47169fe62fd4a971aa07859476c2ba22c2254d4a1baa4e10b95ad"},
-    {url = "https://files.pythonhosted.org/packages/5a/37/ef88eed265d93bc28c681316f68762c5e04167519e5627a0187c8878b409/psutil-5.9.4-cp36-abi3-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:16653106f3b59386ffe10e0bad3bb6299e169d5327d3f187614b1cb8f24cf2e1"},
-    {url = "https://files.pythonhosted.org/packages/60/f8/b92fecd5297edcecda825a04dfde7cb0a2ecd178eb976cb5a7956e375c6a/psutil-5.9.4-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:c1ca331af862803a42677c120aff8a814a804e09832f166f226bfd22b56feee8"},
-    {url = "https://files.pythonhosted.org/packages/6e/c8/784968329c1c67c28cce91991ef9af8a8913aa5a3399a6a8954b1380572f/psutil-5.9.4-cp36-abi3-manylinux_2_12_x86_64.manylinux2010_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:54c0d3d8e0078b7666984e11b12b88af2db11d11249a8ac8920dd5ef68a66e08"},
-    {url = "https://files.pythonhosted.org/packages/79/26/f026804298b933b11640cc2d15155a545805df732e5ead3a2ad7cf45a38b/psutil-5.9.4-cp38-abi3-macosx_11_0_arm64.whl", hash = "sha256:6001c809253a29599bc0dfd5179d9f8a5779f9dffea1da0f13c53ee568115e1e"},
-    {url = "https://files.pythonhosted.org/packages/89/a8/dd2f0866a7e87de751fb5f7c6eca99cbb953c81be76e1814ab3c8c3b0908/psutil-5.9.4-cp27-cp27mu-manylinux2010_x86_64.whl", hash = "sha256:efeae04f9516907be44904cc7ce08defb6b665128992a56957abc9b61dca94b7"},
-    {url = "https://files.pythonhosted.org/packages/8e/6b/9a3a5471b74d92dc85bfd71a7f7a55e013b258d86b4c3826ace9d49f7b8c/psutil-5.9.4-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:68908971daf802203f3d37e78d3f8831b6d1014864d7a85937941bb35f09aefe"},
-    {url = "https://files.pythonhosted.org/packages/99/9c/7a5761f9d2e79e6f781db5b25eeb9e74c2dc533bc52ee4749cb055a32ce9/psutil-5.9.4-cp27-cp27m-win_amd64.whl", hash = "sha256:9120cd39dca5c5e1c54b59a41d205023d436799b1c8c4d3ff71af18535728e94"},
-    {url = "https://files.pythonhosted.org/packages/a5/73/35cea01aad1baf901c915dc95ea33a2f271c8ff8cf2f1c73b7f591f1bdf1/psutil-5.9.4-cp36-abi3-macosx_10_9_x86_64.whl", hash = "sha256:54d5b184728298f2ca8567bf83c422b706200bcbbfafdc06718264f9393cfeb7"},
-    {url = "https://files.pythonhosted.org/packages/ec/be/b8df2071eda861e65a1b2cec35770bb1f4523737e84a10aa41c53e39e9bc/psutil-5.9.4-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:6b92c532979bafc2df23ddc785ed116fced1f492ad90a6830cf24f4d1ea27d24"},
+"prometheus-client 0.17.0" = [
+    {url = "https://files.pythonhosted.org/packages/0e/01/bda72c3b5d4a0df411bceb88c4993d413dd9b7d3b3b68ab19171a09e7db1/prometheus_client-0.17.0.tar.gz", hash = "sha256:9c3b26f1535945e85b8934fb374678d263137b78ef85f305b1156c7c881cd11b"},
+    {url = "https://files.pythonhosted.org/packages/5b/62/75fc6f255e214ff0a8bd3267a0bd337521dd24f76cd593c10795e488f41b/prometheus_client-0.17.0-py3-none-any.whl", hash = "sha256:a77b708cf083f4d1a3fb3ce5c95b4afa32b9c521ae363354a4a910204ea095ce"},
+]
+"prompt-toolkit 3.0.38" = [
+    {url = "https://files.pythonhosted.org/packages/4b/bb/75cdcd356f57d17b295aba121494c2333d26bfff1a837e6199b8b83c415a/prompt_toolkit-3.0.38.tar.gz", hash = "sha256:23ac5d50538a9a38c8bde05fecb47d0b403ecd0662857a86f886f798563d5b9b"},
+    {url = "https://files.pythonhosted.org/packages/87/3f/1f5a0ff475ae6481f4b0d45d4d911824d3218b94ee2a97a8cb84e5569836/prompt_toolkit-3.0.38-py3-none-any.whl", hash = "sha256:45ea77a2f7c60418850331366c81cf6b5b9cf4c7fd34616f733c5427e6abbb1f"},
+]
+"psutil 5.9.5" = [
+    {url = "https://files.pythonhosted.org/packages/26/f2/dcd8a3cc9c9b1fcd7576a54e3603ce4d1f85672f2687a44050340f7d47b0/psutil-5.9.5-cp27-none-win_amd64.whl", hash = "sha256:8c5f7c5a052d1d567db4ddd231a9d27a74e8e4a9c3f44b1032762bd7b9fdcd42"},
+    {url = "https://files.pythonhosted.org/packages/3b/e4/fee119c206545fd37be1e5fa4eeb0c729a52ec2ade4f728ae1fd1acb2a3a/psutil-5.9.5-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:be8929ce4313f9f8146caad4272f6abb8bf99fc6cf59344a3167ecd74f4f203f"},
+    {url = "https://files.pythonhosted.org/packages/5f/da/de9d2342db0b7a96863ef84ab94ef1022eec78ece05aac253cddc494e1a7/psutil-5.9.5-cp27-cp27mu-manylinux2010_x86_64.whl", hash = "sha256:acf2aef9391710afded549ff602b5887d7a2349831ae4c26be7c807c0a39fac4"},
+    {url = "https://files.pythonhosted.org/packages/86/f3/23e4e4e7ec7855d506ed928756b04735c246b14d9f778ed7ffaae18d8043/psutil-5.9.5-cp36-abi3-win_amd64.whl", hash = "sha256:b258c0c1c9d145a1d5ceffab1134441c4c5113b2417fafff7315a917a026c3c9"},
+    {url = "https://files.pythonhosted.org/packages/89/fa/ab117fa86195050802207639f5daee857791daaabe9a996935b5b77dbe10/psutil-5.9.5-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:4aef137f3345082a3d3232187aeb4ac4ef959ba3d7c10c33dd73763fbc063da4"},
+    {url = "https://files.pythonhosted.org/packages/8d/24/ed6b6506f187def39887a91a68e58336eff4cf3e3d5a163ded58bee98624/psutil-5.9.5-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:ab8ed1a1d77c95453db1ae00a3f9c50227ebd955437bcf2a574ba8adbf6a74d5"},
+    {url = "https://files.pythonhosted.org/packages/99/f5/ec768e107445f18baa907509aaa0562a4d148a602bd97e8114d79bd6c84d/psutil-5.9.5-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:ea8518d152174e1249c4f2a1c89e3e6065941df2fa13a1ab45327716a23c2b48"},
+    {url = "https://files.pythonhosted.org/packages/9a/76/c0195c3443a725c24b3a479f57636dec89efe53d19d435d1752c5188f7de/psutil-5.9.5-cp36-abi3-macosx_10_9_x86_64.whl", hash = "sha256:3c6f686f4225553615612f6d9bc21f1c0e305f75d7d8454f9b46e901778e7217"},
+    {url = "https://files.pythonhosted.org/packages/af/4d/389441079ecef400e2551a3933224885a7bde6b8a4810091d628cdd75afe/psutil-5.9.5-cp36-abi3-manylinux_2_12_x86_64.manylinux2010_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:89518112647f1276b03ca97b65cc7f64ca587b1eb0278383017c2a0dcc26cbe4"},
+    {url = "https://files.pythonhosted.org/packages/cf/e3/6af6ec0cbe72f63e9a16d8b53590489e40ed0ff0c99b6a6f05d6af3bb80e/psutil-5.9.5-cp27-none-win32.whl", hash = "sha256:5b9b8cb93f507e8dbaf22af6a2fd0ccbe8244bf30b1baad6b3954e935157ae3f"},
+    {url = "https://files.pythonhosted.org/packages/d6/0f/96b7309212a926c1448366e9ce69b081ea79d63265bde33f11cc9cfc2c07/psutil-5.9.5.tar.gz", hash = "sha256:5410638e4df39c54d957fc51ce03048acd8e6d60abc0f5107af51e5fb566eb3c"},
+    {url = "https://files.pythonhosted.org/packages/e5/2e/56db2b45508ad484b3f22888b3e1adaaf09b8766eaa058ed0e4486c1abae/psutil-5.9.5-cp36-abi3-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7a7dd9997128a0d928ed4fb2c2d57e5102bb6089027939f3b722f3a210f9a8da"},
+    {url = "https://files.pythonhosted.org/packages/ed/98/2624954f83489ab13fde2b544baa337d5578c07eee304d320d9ba56e1b1f/psutil-5.9.5-cp38-abi3-macosx_11_0_arm64.whl", hash = "sha256:c607bb3b57dc779d55e1554846352b4e358c10fff3abf3514a7a6601beebdb30"},
+    {url = "https://files.pythonhosted.org/packages/fa/e0/e91277b1cabf5c3f2995c22314553f1be68b17444260101f365c5a5b6ba1/psutil-5.9.5-cp36-abi3-win32.whl", hash = "sha256:104a5cc0e31baa2bcf67900be36acde157756b9c44017b86b2c049f11957887d"},
 ]
 "ptyprocess 0.7.0" = [
     {url = "https://files.pythonhosted.org/packages/20/e5/16ff212c1e452235a90aeb09066144d0c5a6a8c0834397e03f5224495c4e/ptyprocess-0.7.0.tar.gz", hash = "sha256:5c5d0a3b48ceee0b48485e0c26037c0acd7d29765ca3fbb5cb3831d347423220"},
     {url = "https://files.pythonhosted.org/packages/22/a6/858897256d0deac81a172289110f31629fc4cee19b6f01283303e18c8db3/ptyprocess-0.7.0-py2.py3-none-any.whl", hash = "sha256:4b41f3967fce3af57cc7e94b888626c18bf37a083e3651ca8feeb66d492fef35"},
 ]
 "pycodestyle 2.9.1" = [
     {url = "https://files.pythonhosted.org/packages/67/e4/fc77f1039c34b3612c4867b69cbb2b8a4e569720b1f19b0637002ee03aff/pycodestyle-2.9.1-py2.py3-none-any.whl", hash = "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"},
     {url = "https://files.pythonhosted.org/packages/b6/83/5bcaedba1f47200f0665ceb07bcb00e2be123192742ee0edfb66b600e5fd/pycodestyle-2.9.1.tar.gz", hash = "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785"},
 ]
 "pycparser 2.21" = [
     {url = "https://files.pythonhosted.org/packages/5e/0b/95d387f5f4433cb0f53ff7ad859bd2c6051051cebbb564f139a999ab46de/pycparser-2.21.tar.gz", hash = "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"},
     {url = "https://files.pythonhosted.org/packages/62/d5/5f610ebe421e85889f2e55e33b7f9a6795bd982198517d912eb1c76e1a53/pycparser-2.21-py2.py3-none-any.whl", hash = "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9"},
 ]
-"pydantic 1.10.4" = [
-    {url = "https://files.pythonhosted.org/packages/02/6b/c4b5773bcc216652cc6a040eb32697f99770cf9274d8ad254e621eb3fdd1/pydantic-1.10.4-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:a9f2de23bec87ff306aef658384b02aa7c32389766af3c5dee9ce33e80222dfa"},
-    {url = "https://files.pythonhosted.org/packages/09/46/66c65d678e4c1b151c36bd61fd7ad9ebd1b48ecccc115d5dc77c1d7fe476/pydantic-1.10.4-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:05a81b006be15655b2a1bae5faa4280cf7c81d0e09fcb49b342ebf826abe5a72"},
-    {url = "https://files.pythonhosted.org/packages/12/74/797cf42ee7093e73f740224ee7f9d3faba6e5f674243078a51fc38ba7a78/pydantic-1.10.4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:51bdeb10d2db0f288e71d49c9cefa609bca271720ecd0c58009bd7504a0c464c"},
-    {url = "https://files.pythonhosted.org/packages/17/70/139ae58f5fa5e9000c63d49e1b74a256a74abf4064d7e9b236adc3e21251/pydantic-1.10.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:6dc1cc241440ed7ca9ab59d9929075445da6b7c94ced281b3dd4cfe6c8cff817"},
-    {url = "https://files.pythonhosted.org/packages/2d/c7/d284a73934b79077ff48c6e64f93dcf570660931c90bafbdadc9867bf929/pydantic-1.10.4-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:cd8702c5142afda03dc2b1ee6bc358b62b3735b2cce53fc77b31ca9f728e4bc8"},
-    {url = "https://files.pythonhosted.org/packages/35/b1/c574b4d47ba9565f5984cf406ce06764a07994b1608d89d53207a7f67c33/pydantic-1.10.4-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:f2f7eb6273dd12472d7f218e1fef6f7c7c2f00ac2e1ecde4db8824c457300416"},
-    {url = "https://files.pythonhosted.org/packages/36/78/1755a9fe87b0480775bce2e812049669adbe4b006787257d288806caa580/pydantic-1.10.4-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:990406d226dea0e8f25f643b370224771878142155b879784ce89f633541a024"},
-    {url = "https://files.pythonhosted.org/packages/49/0c/3cb9ddf7aba9a13c56585401ee7ea345ed583c2f848e783eec634c9726d3/pydantic-1.10.4-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:fdf8d759ef326962b4678d89e275ffc55b7ce59d917d9f72233762061fd04a2d"},
-    {url = "https://files.pythonhosted.org/packages/49/90/ff3dd0265279a2f0607995dfcd77720f0130918cf11ee9449b106d99b942/pydantic-1.10.4-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:572066051eeac73d23f95ba9a71349c42a3e05999d0ee1572b7860235b850cc6"},
-    {url = "https://files.pythonhosted.org/packages/4a/52/79167d367d0765effd60faef145c54a213a5feab7a5c97055fa368f25031/pydantic-1.10.4-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:8775d4ef5e7299a2f4699501077a0defdaac5b6c4321173bcb0f3c496fbadf85"},
-    {url = "https://files.pythonhosted.org/packages/4e/26/38b8e36129e1f9e4d5e4481cee0cbc49b778ac103777c50cb2fca714afbe/pydantic-1.10.4-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:eb992a1ef739cc7b543576337bebfc62c0e6567434e522e97291b251a41dad7f"},
-    {url = "https://files.pythonhosted.org/packages/53/17/34e54e352f6a3d304044e52d5ddd5cd621a62ec8fb7af08cc73af65dd3e1/pydantic-1.10.4.tar.gz", hash = "sha256:b9a3859f24eb4e097502a3be1fb4b2abb79b6103dd9e2e0edb70613a4459a648"},
-    {url = "https://files.pythonhosted.org/packages/54/7e/e111f6ff353af848d44bb4f40311c1ca7dfb284efbf8a41122a6091a0996/pydantic-1.10.4-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:d88c4c0e5c5dfd05092a4b271282ef0588e5f4aaf345778056fc5259ba098857"},
-    {url = "https://files.pythonhosted.org/packages/58/1b/0132040ef3e8ec0ce96142d4759bde9f16b52ab7eac5f2c1ce3a5b641f16/pydantic-1.10.4-py3-none-any.whl", hash = "sha256:4948f264678c703f3877d1c8877c4e3b2e12e549c57795107f08cf70c6ec7774"},
-    {url = "https://files.pythonhosted.org/packages/5f/05/faa76cdd1d58066678b104a8bfa2b657144b1996773d655e2d5abb72bfeb/pydantic-1.10.4-cp310-cp310-win_amd64.whl", hash = "sha256:7feb6a2d401f4d6863050f58325b8d99c1e56f4512d98b11ac64ad1751dc647d"},
-    {url = "https://files.pythonhosted.org/packages/67/f7/05de7f3998a365725ea26ed44ce242dfa4e7ddb4fd849fd36902ff0a6715/pydantic-1.10.4-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a48f1953c4a1d9bd0b5167ac50da9a79f6072c63c4cef4cf2a3736994903583e"},
-    {url = "https://files.pythonhosted.org/packages/6b/85/c3c30a050f04668dccf4ce8df015242a7ccaea8dface44b342f173f68991/pydantic-1.10.4-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:2b3ce5f16deb45c472dde1a0ee05619298c864a20cded09c4edd820e1454129f"},
-    {url = "https://files.pythonhosted.org/packages/6e/00/7e25a76d3629999587ea4f30b0b15f52a14a43c811a80168900005500f9b/pydantic-1.10.4-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2e82a6d37a95e0b1b42b82ab340ada3963aea1317fd7f888bb6b9dfbf4fff57c"},
-    {url = "https://files.pythonhosted.org/packages/6f/6a/a3b9a51b886eeee570ddb32ae64a8d2fd00cd25cb1daaf82260188d2d1e4/pydantic-1.10.4-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fdf88ab63c3ee282c76d652fc86518aacb737ff35796023fae56a65ced1a5978"},
-    {url = "https://files.pythonhosted.org/packages/7a/9c/3a9db59d67755033edb1588e6d412806fe8023ac5bdbf87a9b8806205bd7/pydantic-1.10.4-cp37-cp37m-win_amd64.whl", hash = "sha256:6e7124d6855b2780611d9f5e1e145e86667eaa3bd9459192c8dc1a097f5e9903"},
-    {url = "https://files.pythonhosted.org/packages/80/79/51583ea13a70715d497be473fc73596142d751dfae956a39b3a0196bc506/pydantic-1.10.4-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:d7b5a3821225f5c43496c324b0d6875fde910a1c2933d726a743ce328fbb2a8c"},
-    {url = "https://files.pythonhosted.org/packages/87/7e/aec14140cb0ee6b62b5777e9d28eea44813b4d590826ad518b7e197e1200/pydantic-1.10.4-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:983e720704431a6573d626b00662eb78a07148c9115129f9b4351091ec95ecc3"},
-    {url = "https://files.pythonhosted.org/packages/88/b4/123955cfb978fb9d2cfde7a92b588cffca5cb3772702a09e4ab5807574b1/pydantic-1.10.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:b5635de53e6686fe7a44b5cf25fcc419a0d5e5c1a1efe73d49d48fe7586db854"},
-    {url = "https://files.pythonhosted.org/packages/8a/97/8f789eb4ab68abe9541f5765dc7f533dbc3d6c9c94cd70d1b01e21759cf9/pydantic-1.10.4-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:55b1625899acd33229c4352ce0ae54038529b412bd51c4915349b49ca575258f"},
-    {url = "https://files.pythonhosted.org/packages/9e/85/13eb8a5121d1d37826118ac8d88fe856229aad43396a3680307eaee8c73e/pydantic-1.10.4-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:78cec42b95dbb500a1f7120bdf95c401f6abb616bbe8785ef09887306792e66e"},
-    {url = "https://files.pythonhosted.org/packages/ae/97/c9716e8060e3ed0bbd954258babe4c2f75092ca923972101d791230dcb7e/pydantic-1.10.4-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:9193d4f4ee8feca58bc56c8306bcb820f5c7905fd919e0750acdeeeef0615b28"},
-    {url = "https://files.pythonhosted.org/packages/ba/7f/47a90201dc4c11a514dfba59c689491d5018b83be21f682aa602c845c125/pydantic-1.10.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:a9a6747cac06c2beb466064dda999a13176b23535e4c496c9d48e6406f92d42d"},
-    {url = "https://files.pythonhosted.org/packages/d1/1a/44c9e2fa8d94cfb1d73352205960798d991a1236aec09d15bf702874ac64/pydantic-1.10.4-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:75d52162fe6b2b55964fbb0af2ee58e99791a3138588c482572bb6087953113a"},
-    {url = "https://files.pythonhosted.org/packages/d3/ab/0626c660fa632920c0a2623a07700adacb01986bd22a089f2669596096cd/pydantic-1.10.4-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:0b53e1d41e97063d51a02821b80538053ee4608b9a181c1005441f1673c55423"},
-    {url = "https://files.pythonhosted.org/packages/da/e9/82b5585bb1d8a01c6b597fe30ef078ca3939dbbd7c1f7f9a6501062889ec/pydantic-1.10.4-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b6f9d649892a6f54a39ed56b8dfd5e08b5f3be5f893da430bed76975f3735d15"},
-    {url = "https://files.pythonhosted.org/packages/db/2a/41d60a843328d91b12c6efd1a18b17606bd2ebe498647e75721a9317b433/pydantic-1.10.4-cp311-cp311-win_amd64.whl", hash = "sha256:6a05a9db1ef5be0fe63e988f9617ca2551013f55000289c671f71ec16f4985e3"},
-    {url = "https://files.pythonhosted.org/packages/de/d4/dcb8e4bc7777e2e0d79381cc4c63cda50e83e355fa10d64082c216905377/pydantic-1.10.4-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:301d626a59edbe5dfb48fcae245896379a450d04baeed50ef40d8199f2733b06"},
-    {url = "https://files.pythonhosted.org/packages/df/8d/c52f913e533b2e71a94e7f22148b449abf328c46a5b4a1da4d0e7e9f659e/pydantic-1.10.4-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:887ca463c3bc47103c123bc06919c86720e80e1214aab79e9b779cda0ff92a00"},
-    {url = "https://files.pythonhosted.org/packages/ea/45/86ec3475f45f02858808643f38700788c64bfef0896566936dc33a78d4ba/pydantic-1.10.4-cp39-cp39-win_amd64.whl", hash = "sha256:9cbdc268a62d9a98c56e2452d6c41c0263d64a2009aac69246486f01b4f594c4"},
-    {url = "https://files.pythonhosted.org/packages/ec/f2/c136265b246eb0411b293763e1b5e18a22de2d8d6a084e5c3d7b9e6e796e/pydantic-1.10.4-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:39f4a73e5342b25c2959529f07f026ef58147249f9b7431e1ba8414a36761f53"},
-    {url = "https://files.pythonhosted.org/packages/f4/09/6efdaefc6e967f03af3ae3d5e63575036598eb0c740a43a69a77be054a5f/pydantic-1.10.4-cp38-cp38-win_amd64.whl", hash = "sha256:4b05697738e7d2040696b0a66d9f0a10bec0efa1883ca75ee9e55baf511909d6"},
+"pydantic 1.10.8" = [
+    {url = "https://files.pythonhosted.org/packages/05/43/e39c6bf32695f2d568ebb2f6a3dd843c8e2edb57c77a4a911d517b5675b2/pydantic-1.10.8-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:35db5301b82e8661fa9c505c800d0990bc14e9f36f98932bb1d248c0ac5cada5"},
+    {url = "https://files.pythonhosted.org/packages/0b/39/afbca0ea8e766ccf04f224520b95ca29d5a18b680c0780609a2c39293f8b/pydantic-1.10.8-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:1243d28e9b05003a89d72e7915fdb26ffd1d39bdd39b00b7dbe4afae4b557f9d"},
+    {url = "https://files.pythonhosted.org/packages/13/dc/54ceed364e733f81596a4f113de2098221b3d39b4eb7abbffa64e681f243/pydantic-1.10.8-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:666bdf6066bf6dbc107b30d034615d2627e2121506c555f73f90b54a463d1f33"},
+    {url = "https://files.pythonhosted.org/packages/15/27/c35f6fefc782aebcff9991b28728f3855b1253ff757e6dee8e3ac3815cd0/pydantic-1.10.8-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:191ba419b605f897ede9892f6c56fb182f40a15d309ef0142212200a10af4c18"},
+    {url = "https://files.pythonhosted.org/packages/23/65/2aa13873e9e0084ecaec00fbe6c6096b65e1ab99ba66bdbf7e4e7c4cc915/pydantic-1.10.8.tar.gz", hash = "sha256:1410275520dfa70effadf4c21811d755e7ef9bb1f1d077a21958153a92c8d9ca"},
+    {url = "https://files.pythonhosted.org/packages/2d/a2/e3ac01dd929485a6280518d280d8cf313558c878c91d86b3a95b1702938b/pydantic-1.10.8-cp310-cp310-win_amd64.whl", hash = "sha256:ab523c31e22943713d80d8d342d23b6f6ac4b792a1e54064a8d0cf78fd64e800"},
+    {url = "https://files.pythonhosted.org/packages/36/60/b24bd42bdd385fee681cc1231ef1d423566d4e33e867df4d2bd08b531466/pydantic-1.10.8-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:6f2e754d5566f050954727c77f094e01793bcb5725b663bf628fa6743a5a9108"},
+    {url = "https://files.pythonhosted.org/packages/56/b5/903cd28ab9a3bf8cbfbe0a6a87d9463ceac7610193cd1d72bb1bdb276d01/pydantic-1.10.8-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f90c1e29f447557e9e26afb1c4dbf8768a10cc676e3781b6a577841ade126b85"},
+    {url = "https://files.pythonhosted.org/packages/57/ce/b3de85c397a03f1c8dadebe33fa81b195b6090c840a0333769fba00693fd/pydantic-1.10.8-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:1952526ba40b220b912cdc43c1c32bcf4a58e3f192fa313ee665916b26befb68"},
+    {url = "https://files.pythonhosted.org/packages/59/ab/1de0d5386a464ef527338d320216a2f41de416e204780e00baa0e5e3b807/pydantic-1.10.8-cp38-cp38-win_amd64.whl", hash = "sha256:6a82d6cda82258efca32b40040228ecf43a548671cb174a1e81477195ed3ed56"},
+    {url = "https://files.pythonhosted.org/packages/6b/15/3504de0fcb90336680916ea3fde845d01fa846c95ab4342c28d985c0d29d/pydantic-1.10.8-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:93e766b4a8226e0708ef243e843105bf124e21331694367f95f4e3b4a92bbb3f"},
+    {url = "https://files.pythonhosted.org/packages/6c/32/0755046e707a468fe276fd40df11d492a72d1cbcfa344091e3a46120131c/pydantic-1.10.8-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:c0ab53b609c11dfc0c060d94335993cc2b95b2150e25583bec37a49b2d6c6c3f"},
+    {url = "https://files.pythonhosted.org/packages/6c/f9/5edecae1914fc7dc6a566809a5242c97d63acfb92253b0bb885d890eb953/pydantic-1.10.8-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:42aa0c4b5c3025483240a25b09f3c09a189481ddda2ea3a831a9d25f444e03c1"},
+    {url = "https://files.pythonhosted.org/packages/6f/4d/7647a5f98fbcbb9bdb1e5a77eca931a1f83255c9aa14448794a0596b5a42/pydantic-1.10.8-cp37-cp37m-win_amd64.whl", hash = "sha256:16f8c3e33af1e9bb16c7a91fc7d5fa9fe27298e9f299cff6cb744d89d573d62c"},
+    {url = "https://files.pythonhosted.org/packages/77/ea/2b96534811f867bb53edaf2a3ca5037d8bcbceb05d5930bac5caa1fba573/pydantic-1.10.8-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:1ced8375969673929809d7f36ad322934c35de4af3b5e5b09ec967c21f9f7887"},
+    {url = "https://files.pythonhosted.org/packages/7a/ba/439e2bc693d3f464946159a76724efc570cef9f4e27303fa3b360b2f3ef7/pydantic-1.10.8-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ceb6a23bf1ba4b837d0cfe378329ad3f351b5897c8d4914ce95b85fba96da5a1"},
+    {url = "https://files.pythonhosted.org/packages/98/20/52707fc7dc91b6e580dbd30c4a6b88e426f61af9f2547bb52e880f09e67d/pydantic-1.10.8-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:12f7b0bf8553e310e530e9f3a2f5734c68699f42218bf3568ef49cd9b0e44df4"},
+    {url = "https://files.pythonhosted.org/packages/a7/27/80672dfb14e47293cca421580141ec923a1e5fe7283f775079e006b0be28/pydantic-1.10.8-cp311-cp311-win_amd64.whl", hash = "sha256:d532bf00f381bd6bc62cabc7d1372096b75a33bc197a312b03f5838b4fb84edd"},
+    {url = "https://files.pythonhosted.org/packages/b2/43/8eca9ebbfd861209365c5b9f982b113275eccd892e53ab7bde60a21439e8/pydantic-1.10.8-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:34d327c81e68a1ecb52fe9c8d50c8a9b3e90d3c8ad991bfc8f953fb477d42fb4"},
+    {url = "https://files.pythonhosted.org/packages/b8/45/538d65960c489a1aa9cbf1f54d4b911e1e838d557d2d2ccd1b6c8fa10f3b/pydantic-1.10.8-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:17aef11cc1b997f9d574b91909fed40761e13fac438d72b81f902226a69dac01"},
+    {url = "https://files.pythonhosted.org/packages/c1/37/d136df986c0a2d20f940d360fe472ae410fba46f55a73e872fd3168f4289/pydantic-1.10.8-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:0c6fafa0965b539d7aab0a673a046466d23b86e4b0e8019d25fd53f4df62c277"},
+    {url = "https://files.pythonhosted.org/packages/c4/f3/c5dc9f49783a6407487d20c9a32bca878ebf2df155b8d2858838d79b6d46/pydantic-1.10.8-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:bb14388ec45a7a0dc429e87def6396f9e73c8c77818c927b6a60706603d5f2ea"},
+    {url = "https://files.pythonhosted.org/packages/c5/58/71d48d4154e5845192f4ccc6c6ebcf6fa5286fa3bcb3c595aa18a5bf599d/pydantic-1.10.8-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:e82d4566fcd527eae8b244fa952d99f2ca3172b7e97add0b43e2d97ee77f81ab"},
+    {url = "https://files.pythonhosted.org/packages/ca/5b/8b2c49589c826bf2796fc523d77d46fed2e82585c87c812f289ce244c88b/pydantic-1.10.8-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2e4148e635994d57d834be1182a44bdb07dd867fa3c2d1b37002000646cc5459"},
+    {url = "https://files.pythonhosted.org/packages/cc/a4/354a73bb8a06df0df0bc74b5fbf3b9510ed4900185f86a00861dcfbe60c7/pydantic-1.10.8-py3-none-any.whl", hash = "sha256:7456eb22ed9aaa24ff3e7b4757da20d9e5ce2a81018c1b3ebd81a0b88a18f3b2"},
+    {url = "https://files.pythonhosted.org/packages/d8/7b/ca035af1833c6d047eeb328438a2ae402d03929be2055cd66294542a814d/pydantic-1.10.8-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:052d8654cb65174d6f9490cc9b9a200083a82cf5c3c5d3985db765757eb3b375"},
+    {url = "https://files.pythonhosted.org/packages/dc/92/3a09ec18592ca6fc96223b42ad20c8711847a8d2e1800779f9206c2fa6a2/pydantic-1.10.8-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:df7800cb1984d8f6e249351139667a8c50a379009271ee6236138a22a0c0f319"},
+    {url = "https://files.pythonhosted.org/packages/e2/21/e6f68631ec2f0470e28722d1ca352bac4f25aef6eb18b8e65ba3cd9ae8a2/pydantic-1.10.8-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7b1f6cb446470b7ddf86c2e57cd119a24959af2b01e552f60705910663af09a4"},
+    {url = "https://files.pythonhosted.org/packages/e6/dd/6f9ef794df128746581bd5886c6382a19f1729ff39f3d65e66e3b6751c7a/pydantic-1.10.8-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c33b60054b2136aef8cf190cd4c52a3daa20b2263917c49adad20eaf381e823b"},
+    {url = "https://files.pythonhosted.org/packages/e7/a3/329824b0e46edcb2c51f0fa73678f24aba083289697a0db3036f4f30e1ed/pydantic-1.10.8-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3e59417ba8a17265e632af99cc5f35ec309de5980c440c255ab1ca3ae96a3e0e"},
+    {url = "https://files.pythonhosted.org/packages/e8/b3/b748afd5f4fd8f640e08cf4828fa5c9da865353eade18b9c789726b1a0ce/pydantic-1.10.8-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f9613fadad06b4f3bc5db2653ce2f22e0de84a7c6c293909b48f6ed37b83c61f"},
+    {url = "https://files.pythonhosted.org/packages/e9/17/a840d0631a288a4400e23a9ec96d131bd07be820fe2c1d070995de6dfb61/pydantic-1.10.8-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:93e6bcfccbd831894a6a434b0aeb1947f9e70b7468f274154d03d71fabb1d7c6"},
+    {url = "https://files.pythonhosted.org/packages/fa/3b/279a13153350b688fb5eb557acf980059a21ffede20d9b6fbc5368778bf4/pydantic-1.10.8-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:84d80219c3f8d4cad44575e18404099c76851bc924ce5ab1c4c8bb5e2a2227d0"},
+    {url = "https://files.pythonhosted.org/packages/fb/46/723587abb4aecf82edcfaa213a827d61854ebcbf76b4818cbf59c8868f4e/pydantic-1.10.8-cp39-cp39-win_amd64.whl", hash = "sha256:66a703d1983c675a6e0fed8953b0971c44dba48a929a2000a493c3772eb61a5a"},
+    {url = "https://files.pythonhosted.org/packages/fe/26/66c9ac1e21a3bda4f5c10785b3ff199e12e2d1e984780a8bfa796bb4e2f0/pydantic-1.10.8-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:7d5b8641c24886d764a74ec541d2fc2c7fb19f6da2a4001e6d580ba4a38f7878"},
+    {url = "https://files.pythonhosted.org/packages/ff/b4/b56bd5f591969df63a260555a891bf953536eefcbe66b711b80f86acc3a4/pydantic-1.10.8-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:88f195f582851e8db960b4a94c3e3ad25692c1c1539e2552f3df7a9e972ef60e"},
 ]
 "pydocstyle 6.3.0" = [
     {url = "https://files.pythonhosted.org/packages/36/ea/99ddefac41971acad68f14114f38261c1f27dac0b3ec529824ebc739bdaa/pydocstyle-6.3.0-py3-none-any.whl", hash = "sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019"},
     {url = "https://files.pythonhosted.org/packages/e9/5c/d5385ca59fd065e3c6a5fe19f9bc9d5ea7f2509fa8c9c22fb6b2031dd953/pydocstyle-6.3.0.tar.gz", hash = "sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1"},
 ]
 "pyflakes 2.5.0" = [
     {url = "https://files.pythonhosted.org/packages/07/92/f0cb5381f752e89a598dd2850941e7f570ac3cb8ea4a344854de486db152/pyflakes-2.5.0.tar.gz", hash = "sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3"},
     {url = "https://files.pythonhosted.org/packages/dc/13/63178f59f74e53acc2165aee4b002619a3cfa7eeaeac989a9eb41edf364e/pyflakes-2.5.0-py2.py3-none-any.whl", hash = "sha256:4579f67d887f804e67edb544428f264b7b24f435b263c4614f384135cea553d2"},
 ]
-"pygments 2.14.0" = [
-    {url = "https://files.pythonhosted.org/packages/0b/42/d9d95cc461f098f204cd20c85642ae40fbff81f74c300341b8d0e0df14e0/Pygments-2.14.0-py3-none-any.whl", hash = "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"},
-    {url = "https://files.pythonhosted.org/packages/da/6a/c427c06913204e24de28de5300d3f0e809933f376e0b7df95194b2bb3f71/Pygments-2.14.0.tar.gz", hash = "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297"},
+"pygments 2.15.1" = [
+    {url = "https://files.pythonhosted.org/packages/34/a7/37c8d68532ba71549db4212cb036dbd6161b40e463aba336770e80c72f84/Pygments-2.15.1-py3-none-any.whl", hash = "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"},
+    {url = "https://files.pythonhosted.org/packages/89/6b/2114e54b290824197006e41be3f9bbe1a26e9c39d1f5fa20a6d62945a0b3/Pygments-2.15.1.tar.gz", hash = "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c"},
 ]
 "pyrsistent 0.19.3" = [
     {url = "https://files.pythonhosted.org/packages/07/d2/0e72806d668c001d13885e8d7c78fefa5a649c34ad9d77b90eb472096ae7/pyrsistent-0.19.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cc5d149f31706762c1f8bda2e8c4f8fead6e80312e3692619a75301d3dbb819a"},
     {url = "https://files.pythonhosted.org/packages/09/0a/cf855eb8b1dc98f20e3223c7262068918f22f5ad452a99588cf2e5e70e82/pyrsistent-0.19.3-cp37-cp37m-win32.whl", hash = "sha256:e8f2b814a3dc6225964fa03d8582c6e0b6650d68a232df41e3cc1b66a5d2f8d1"},
     {url = "https://files.pythonhosted.org/packages/0b/c0/5ba658ab88966a5a709e17739d1da02615b95e8210d52041d147f11da5da/pyrsistent-0.19.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:aeda827381f5e5d65cced3024126529ddc4289d944f75e090572c77ceb19adbf"},
     {url = "https://files.pythonhosted.org/packages/40/04/f1d7813d4cdb62ed58e75b53e2ef481b47081ab5ad2a104cd284fa507042/pyrsistent-0.19.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4c18264cb84b5e68e7085a43723f9e4c1fd1d935ab240ce02c0324a8e01ccb64"},
     {url = "https://files.pythonhosted.org/packages/4a/91/f8e546cbd5aeecce04a5e9d03c32f329c6b97a5514868c824bbe111cd697/pyrsistent-0.19.3-cp38-cp38-win32.whl", hash = "sha256:f0e7c4b2f77593871e918be000b96c8107da48444d57005b6a6bc61fb4331b2c"},
@@ -1622,164 +1637,160 @@
     {url = "https://files.pythonhosted.org/packages/d5/bf/6ed2d861e3e94c5e92dbb1399eef672fb6add6e824d8c0f4b55d9cd9e733/pyrsistent-0.19.3-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:b735e538f74ec31378f5a1e3886a26d2ca6351106b4dfde376a26fc32a044edc"},
     {url = "https://files.pythonhosted.org/packages/d8/95/374840c28274b2d660a49c81aee980543953c9c13bcfc9c8c22fb7737919/pyrsistent-0.19.3-cp37-cp37m-win_amd64.whl", hash = "sha256:c9bb60a40a0ab9aba40a59f68214eed5a29c6274c83b2cc206a359c4a89fa41b"},
     {url = "https://files.pythonhosted.org/packages/dc/c2/994b3e91f22b040fefbb3058d8622e3b45ab78dd1256599575bf36319b6d/pyrsistent-0.19.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:c4db1bd596fefd66b296a3d5d943c94f4fac5bcd13e99bffe2ba6a759d959a28"},
     {url = "https://files.pythonhosted.org/packages/de/9e/10c5bf794eec650a3aab1b4fb1f6824f53011d111ddfdce1459dc357408a/pyrsistent-0.19.3-cp311-cp311-win32.whl", hash = "sha256:64220c429e42a7150f4bfd280f6f4bb2850f95956bde93c6fda1b70507af6ef3"},
     {url = "https://files.pythonhosted.org/packages/ed/7b/7d032130a6838b179b46dff1ee88909c11d518a10ec9bc70c4b72c7c2f80/pyrsistent-0.19.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:20460ac0ea439a3e79caa1dbd560344b64ed75e85d8703943e0b66c2a6150e4a"},
     {url = "https://files.pythonhosted.org/packages/f4/43/183384edb4d2788374aa7663b82ace4afe4a0c1fbfee064875eb40ada95b/pyrsistent-0.19.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3a8cb235fa6d3fd7aae6a4f1429bbb1fec1577d978098da1252f0489937786f3"},
 ]
-"pytest 7.2.1" = [
-    {url = "https://files.pythonhosted.org/packages/cc/02/8f59bf194c9a1ceac6330850715e9ec11e21e2408a30a596c65d54cf4d2a/pytest-7.2.1-py3-none-any.whl", hash = "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5"},
-    {url = "https://files.pythonhosted.org/packages/e5/6c/f3a15217ac72912c28c5d7a7a8e87ff6d6475c9530595ae9f0f8dedd8dd8/pytest-7.2.1.tar.gz", hash = "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"},
-]
-"pytest-cov 4.0.0" = [
-    {url = "https://files.pythonhosted.org/packages/ea/70/da97fd5f6270c7d2ce07559a19e5bf36a76f0af21500256f005a69d9beba/pytest-cov-4.0.0.tar.gz", hash = "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"},
-    {url = "https://files.pythonhosted.org/packages/fe/1f/9ec0ddd33bd2b37d6ec50bb39155bca4fe7085fa78b3b434c05459a860e3/pytest_cov-4.0.0-py3-none-any.whl", hash = "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b"},
+"pytest 7.3.1" = [
+    {url = "https://files.pythonhosted.org/packages/1b/d1/72df649a705af1e3a09ffe14b0c7d3be1fd730da6b98beb4a2ed26b8a023/pytest-7.3.1-py3-none-any.whl", hash = "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362"},
+    {url = "https://files.pythonhosted.org/packages/ec/d9/36b65598f3d19d0a14d13dc87ad5fa42869ae53bb7471f619a30eaabc4bf/pytest-7.3.1.tar.gz", hash = "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"},
+]
+"pytest-cov 4.1.0" = [
+    {url = "https://files.pythonhosted.org/packages/7a/15/da3df99fd551507694a9b01f512a2f6cf1254f33601605843c3775f39460/pytest-cov-4.1.0.tar.gz", hash = "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6"},
+    {url = "https://files.pythonhosted.org/packages/a7/4b/8b78d126e275efa2379b1c2e09dc52cf70df16fc3b90613ef82531499d73/pytest_cov-4.1.0-py3-none-any.whl", hash = "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"},
 ]
 "python-dateutil 2.8.2" = [
     {url = "https://files.pythonhosted.org/packages/36/7a/87837f39d0296e723bb9b62bbb257d0355c7f6128853c78955f57342a56d/python_dateutil-2.8.2-py2.py3-none-any.whl", hash = "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"},
     {url = "https://files.pythonhosted.org/packages/4c/c4/13b4776ea2d76c115c1d1b84579f3764ee6d57204f6be27119f13a61d0a9/python-dateutil-2.8.2.tar.gz", hash = "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86"},
 ]
-"pywin32 305" = [
-    {url = "https://files.pythonhosted.org/packages/02/80/23fdb88f8a398dff615f10100cf54871fd8518e3eeea72c1a7d46af01bf9/pywin32-305-cp310-cp310-win_amd64.whl", hash = "sha256:73e819c6bed89f44ff1d690498c0a811948f73777e5f97c494c152b850fad478"},
-    {url = "https://files.pythonhosted.org/packages/05/19/e1f2d772c5437f37c7dbe88be56939de53f040674b6accf2c0369674873d/pywin32-305-cp310-cp310-win_arm64.whl", hash = "sha256:742eb905ce2187133a29365b428e6c3b9001d79accdc30aa8969afba1d8470f4"},
-    {url = "https://files.pythonhosted.org/packages/1e/28/89edde08f43d3c795a7a950368cb3c811f10ae7cc9f1b862f468c3697e8a/pywin32-305-cp39-cp39-win32.whl", hash = "sha256:9d968c677ac4d5cbdaa62fd3014ab241718e619d8e36ef8e11fb930515a1e918"},
-    {url = "https://files.pythonhosted.org/packages/22/da/344b3df042f42d9d775ae2030276b2992adab519c6d682393ddf356775f3/pywin32-305-cp311-cp311-win_amd64.whl", hash = "sha256:326f42ab4cfff56e77e3e595aeaf6c216712bbdd91e464d167c6434b28d65990"},
-    {url = "https://files.pythonhosted.org/packages/29/a9/44913e2b953a63404f992daa7608f8263fe8ac608dd8c717de5be9d53600/pywin32-305-cp37-cp37m-win_amd64.whl", hash = "sha256:109f98980bfb27e78f4df8a51a8198e10b0f347257d1e265bb1a32993d0c973d"},
-    {url = "https://files.pythonhosted.org/packages/2f/02/b7ffa4a3f6b7ddf8f08926fc9312856443ec446259d095ae80bbf5d06add/pywin32-305-cp39-cp39-win_amd64.whl", hash = "sha256:50768c6b7c3f0b38b7fb14dd4104da93ebced5f1a50dc0e834594bff6fbe1271"},
-    {url = "https://files.pythonhosted.org/packages/4b/af/7c7d46af6bf74a92ecaf674fe9f587912bd74a95eddd9304b4e16b37aa8b/pywin32-305-cp36-cp36m-win_amd64.whl", hash = "sha256:13362cc5aa93c2beaf489c9c9017c793722aeb56d3e5166dadd5ef82da021fe1"},
-    {url = "https://files.pythonhosted.org/packages/4b/e0/2b1513208a885267f5acef393eb6346062323751769630c071667c904dde/pywin32-305-cp37-cp37m-win32.whl", hash = "sha256:a55db448124d1c1484df22fa8bbcbc45c64da5e6eae74ab095b9ea62e6d00496"},
-    {url = "https://files.pythonhosted.org/packages/5c/63/ff5e909e6718ccf1b7f5b359b12bed40136c9f5d58b749662a592f4e7aa2/pywin32-305-cp36-cp36m-win32.whl", hash = "sha256:48d8b1659284f3c17b68587af047d110d8c44837736b8932c034091683e05863"},
-    {url = "https://files.pythonhosted.org/packages/65/e4/76dab43949fc3ba9aee8dc0635b299ad09df7813e81aa4adc88e27f463fe/pywin32-305-cp310-cp310-win32.whl", hash = "sha256:421f6cd86e84bbb696d54563c48014b12a23ef95a14e0bdba526be756d89f116"},
-    {url = "https://files.pythonhosted.org/packages/66/e8/0078d6042bf5bce7e2518b32cf1a0c1399a64f91fc280bb1cfda69fcdb35/pywin32-305-cp311-cp311-win32.whl", hash = "sha256:19ca459cd2e66c0e2cc9a09d589f71d827f26d47fe4a9d09175f6aa0256b51c2"},
-    {url = "https://files.pythonhosted.org/packages/6d/37/fb50f89e6f8a420f0f02adbb81cd85de6fd8a4d4c842b721b08bcd533987/pywin32-305-cp38-cp38-win_amd64.whl", hash = "sha256:56d7a9c6e1a6835f521788f53b5af7912090674bb84ef5611663ee1595860fc7"},
-    {url = "https://files.pythonhosted.org/packages/a2/df/cb14fa23ef0782e62df7b33ea2b926150de3b1d71d2713f434582f8a0024/pywin32-305-cp311-cp311-win_arm64.whl", hash = "sha256:4ecd404b2c6eceaca52f8b2e3e91b2187850a1ad3f8b746d0796a98b4cea04db"},
-    {url = "https://files.pythonhosted.org/packages/e3/c9/3ab2df149dc0e0b0ece0513e1650c7e7f26b61b05851853864aa95ff42b9/pywin32-305-cp38-cp38-win32.whl", hash = "sha256:9dd98384da775afa009bc04863426cb30596fd78c6f8e4e2e5bbf4edf8029504"},
+"pywin32 306" = [
+    {url = "https://files.pythonhosted.org/packages/08/dc/28c668097edfaf4eac4617ef7adf081b9cf50d254672fcf399a70f5efc41/pywin32-306-cp310-cp310-win32.whl", hash = "sha256:06d3420a5155ba65f0b72f2699b5bacf3109f36acbe8923765c22938a69dfc8d"},
+    {url = "https://files.pythonhosted.org/packages/0e/57/c3ec32b498f24a2392404d1f0fd29f47a3f7339d7d579df7a0560cff337c/pywin32-306-cp38-cp38-win32.whl", hash = "sha256:e4c092e2589b5cf0d365849e73e02c391c1349958c5ac3e9d5ccb9a28e017b3a"},
+    {url = "https://files.pythonhosted.org/packages/14/91/17e016d5923e178346aabda3dfec6629d1a26efe587d19667542105cf0a6/pywin32-306-cp312-cp312-win32.whl", hash = "sha256:383229d515657f4e3ed1343da8be101000562bf514591ff383ae940cad65458b"},
+    {url = "https://files.pythonhosted.org/packages/1c/43/e3444dc9a12f8365d9603c2145d16bf0a2f8180f343cf87be47f5579e547/pywin32-306-cp312-cp312-win_arm64.whl", hash = "sha256:5821ec52f6d321aa59e2db7e0a35b997de60c201943557d108af9d4ae1ec7040"},
+    {url = "https://files.pythonhosted.org/packages/1c/f7/24d8ed4fd9c43b90354df7764f81f0dd5e623f9a50f1538f90fe085d6dff/pywin32-306-cp39-cp39-win_amd64.whl", hash = "sha256:39b61c15272833b5c329a2989999dcae836b1eed650252ab1b7bfbe1d59f30f4"},
+    {url = "https://files.pythonhosted.org/packages/28/19/6b8f416ff02132c404042f251eb90a41d15abe677481fcff22077e943c6f/pywin32-306-cp37-cp37m-win32.whl", hash = "sha256:1c73ea9a0d2283d889001998059f5eaaba3b6238f767c9cf2833b13e6a685f65"},
+    {url = "https://files.pythonhosted.org/packages/7e/7f/419c4fcadcaa374a0ae41cbdf6c3a81452892dd6c523aea629d17e49146e/pywin32-306-cp39-cp39-win32.whl", hash = "sha256:e25fd5b485b55ac9c057f67d94bc203f3f6595078d1fb3b458c9c28b7153a802"},
+    {url = "https://files.pythonhosted.org/packages/7e/9e/ad6b1ae2a5ad1066dc509350e0fbf74d8d50251a51e420a2a8feaa0cecbd/pywin32-306-cp311-cp311-win_amd64.whl", hash = "sha256:a7639f51c184c0272e93f244eb24dafca9b1855707d94c192d4a0b4c01e1100e"},
+    {url = "https://files.pythonhosted.org/packages/80/e6/08192cb5728a6ffdb70ea990d9a1351b320d31a751bb463e652d9e05e7aa/pywin32-306-cp37-cp37m-win_amd64.whl", hash = "sha256:72c5f621542d7bdd4fdb716227be0dd3f8565c11b280be6315b06ace35487d36"},
+    {url = "https://files.pythonhosted.org/packages/83/1c/25b79fc3ec99b19b0a0730cc47356f7e2959863bf9f3cd314332bddb4f68/pywin32-306-cp312-cp312-win_amd64.whl", hash = "sha256:37257794c1ad39ee9be652da0462dc2e394c8159dfd913a8a4e8eb6fd346da0e"},
+    {url = "https://files.pythonhosted.org/packages/8b/1e/fc18ad83ca553e01b97aa8393ff10e33c1fb57801db05488b83282ee9913/pywin32-306-cp311-cp311-win32.whl", hash = "sha256:e65028133d15b64d2ed8f06dd9fbc268352478d4f9289e69c190ecd6818b6407"},
+    {url = "https://files.pythonhosted.org/packages/91/20/f744bff1da8f43388498503634378dbbefbe493e65675f2cc52f7185c2c2/pywin32-306-cp311-cp311-win_arm64.whl", hash = "sha256:70dba0c913d19f942a2db25217d9a1b726c278f483a919f1abfed79c9cf64d3a"},
+    {url = "https://files.pythonhosted.org/packages/d3/d6/891894edec688e72c2e308b3243fad98b4066e1839fd2fe78f04129a9d31/pywin32-306-cp310-cp310-win_amd64.whl", hash = "sha256:84f4471dbca1887ea3803d8848a1616429ac94a4a8d05f4bc9c5dcfd42ca99c8"},
+    {url = "https://files.pythonhosted.org/packages/fa/80/a6b22e031590cc5f4fcbd5bf4bcf63a9dabce9d59065f53add99a8caaec5/pywin32-306-cp38-cp38-win_amd64.whl", hash = "sha256:e8ac1ae3601bee6ca9f7cb4b5363bf1c0badb935ef243c4733ff9a393b1690c0"},
 ]
 "pywinpty 2.0.10" = [
     {url = "https://files.pythonhosted.org/packages/37/1a/39d71696107d00fe39a22cd6e512d868b46ddd47e687a22f3f0fc71e2cc7/pywinpty-2.0.10-cp37-none-win_amd64.whl", hash = "sha256:38cb924f2778b5751ef91a75febd114776b3af0ae411bc667be45dd84fc881d3"},
     {url = "https://files.pythonhosted.org/packages/98/3f/eedff7d7f4bc2bb828fa4ea137528f04941bfe6805d13f594c96624a2f93/pywinpty-2.0.10-cp311-none-win_amd64.whl", hash = "sha256:7ffbd66310b83e42028fc9df7746118978d94fba8c1ebf15a7c1275fdd80b28a"},
     {url = "https://files.pythonhosted.org/packages/a4/2e/7aabef8a774819d4851112388b6646bd65782adfcec6fbbf2e309ddb07fb/pywinpty-2.0.10-cp310-none-win_amd64.whl", hash = "sha256:4c7d06ad10f6e92bc850a467f26d98f4f30e73d2fe5926536308c6ae0566bc16"},
     {url = "https://files.pythonhosted.org/packages/ac/09/103cdc5913a8b89099ef8129dfc8f0e0cfdd900e764e3e5d9401256442c5/pywinpty-2.0.10-cp39-none-win_amd64.whl", hash = "sha256:3c46aef80dd50979aff93de199e4a00a8ee033ba7a03cadf0a91fed45f0c39d7"},
     {url = "https://files.pythonhosted.org/packages/c8/cf/c770e35321a5ad004cde0f6fab2a00db6bac2a69b1f0c7d9832d6090ad53/pywinpty-2.0.10-cp38-none-win_amd64.whl", hash = "sha256:902d79444b29ad1833b8d5c3c9aabdfd428f4f068504430df18074007c8c0de8"},
     {url = "https://files.pythonhosted.org/packages/d3/89/2b9113eabacfe3bbebcdf95c24772e2267c7b6b9fed6e35bffba2080a4c1/pywinpty-2.0.10.tar.gz", hash = "sha256:cdbb5694cf8c7242c2ecfaca35c545d31fa5d5814c3d67a4e628f803f680ebea"},
 ]
-"pyzmq 25.0.0" = [
-    {url = "https://files.pythonhosted.org/packages/00/b2/b83067a8af05bd8ebd9613046a0be15e7728219079cf0fbf17ec0fff0a40/pyzmq-25.0.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:656281d496aaf9ca4fd4cea84e6d893e3361057c4707bd38618f7e811759103c"},
-    {url = "https://files.pythonhosted.org/packages/02/5e/dae3cfb179ee0149c8b00f6400cd372fc6b738705f51db3e0f5b7384399a/pyzmq-25.0.0-cp39-cp39-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:9ca6db34b26c4d3e9b0728841ec9aa39484eee272caa97972ec8c8e231b20c7e"},
-    {url = "https://files.pythonhosted.org/packages/08/d7/6aec451d335d8f691993d63105009f508e4011bad0414ab4e6255b31798e/pyzmq-25.0.0-cp39-cp39-macosx_10_15_universal2.whl", hash = "sha256:62b9e80890c0d2408eb42d5d7e1fc62a5ce71be3288684788f74cf3e59ffd6e2"},
-    {url = "https://files.pythonhosted.org/packages/08/e4/0bcbfe6e6babd5ca35059383db4e310ea05e4d6de36be2813ed668606160/pyzmq-25.0.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:0a90b2480a26aef7c13cff18703ba8d68e181facb40f78873df79e6d42c1facc"},
-    {url = "https://files.pythonhosted.org/packages/09/c4/40133b9e77dd6737ec0b3a512a2927f428a93ba3e6cdd9315035c1bce579/pyzmq-25.0.0-cp37-cp37m-win_amd64.whl", hash = "sha256:cac602e02341eaaf4edfd3e29bd3fdef672e61d4e6dfe5c1d065172aee00acee"},
-    {url = "https://files.pythonhosted.org/packages/0c/29/b9344ce166b37bcdac4643a20007e1a5c50c3c9a37b93f8266835eadd99b/pyzmq-25.0.0-pp37-pypy37_pp73-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:28bcb2e66224a7ac2843eb632e4109d6b161479e7a2baf24e37210461485b4f1"},
-    {url = "https://files.pythonhosted.org/packages/0c/85/32a5d18f6ffea367538c70127eb9bc2e5122db6ec65b5b5c81584bc5457c/pyzmq-25.0.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:866eabf7c1315ef2e93e34230db7cbf672e0d7c626b37c11f7e870c8612c3dcc"},
-    {url = "https://files.pythonhosted.org/packages/10/70/4a8f4b8dfbbe5c73a56b9cdcdc17dbe82b03d95fb3cf64e90b66cbb68258/pyzmq-25.0.0-cp37-cp37m-win32.whl", hash = "sha256:02f5cb60a7da1edd5591a15efa654ffe2303297a41e1b40c3c8942f8f11fc17c"},
-    {url = "https://files.pythonhosted.org/packages/13/51/16b0b03dcd26e4613f458a2523d3803a65e26972f89fb91296b091870794/pyzmq-25.0.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:4d3d604fe0a67afd1aff906e54da557a5203368a99dcc50a70eef374f1d2abef"},
-    {url = "https://files.pythonhosted.org/packages/17/02/b8f15787b2a72cba595b5aa75c76c13683fcef017f22af09b7f65c8f288e/pyzmq-25.0.0-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:a1cd4a95f176cdc0ee0a82d49d5830f13ae6015d89decbf834c273bc33eeb3d3"},
-    {url = "https://files.pythonhosted.org/packages/1b/38/22c87e0b51fa7c940a6a07e662161479b145ac2748cee56b9a7df4d1479a/pyzmq-25.0.0-pp37-pypy37_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a0e7ef9ac807db50b4eb6f534c5dcc22f998f5dae920cc28873d2c1d080a4fc9"},
-    {url = "https://files.pythonhosted.org/packages/1f/32/29071fa17e17636636dfb7e7c6ee941790bcad5f7281561a68baea5c2bdb/pyzmq-25.0.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3594c0ff604e685d7e907860b61d0e10e46c74a9ffca168f6e9e50ea934ee440"},
-    {url = "https://files.pythonhosted.org/packages/23/54/83f2f9c86749ac10d17f37d51d29d1e80f83cd20b095e4283646ff36afc9/pyzmq-25.0.0-cp310-cp310-win32.whl", hash = "sha256:01d53958c787cfea34091fcb8ef36003dbb7913b8e9f8f62a0715234ebc98b70"},
-    {url = "https://files.pythonhosted.org/packages/29/f3/453d0971055fefe44b153b50db5ffdd569356618434846d42f9562df15a0/pyzmq-25.0.0-cp38-cp38-win_amd64.whl", hash = "sha256:b90bb8dfbbd138558f1f284fecfe328f7653616ff9a972433a00711d9475d1a9"},
-    {url = "https://files.pythonhosted.org/packages/32/d1/802e9e4243cf54399541baa3279bf2b2c08cbe911928c531fc7cd0aee7b2/pyzmq-25.0.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:85456f0d8f3268eecd63dede3b99d5bd8d3b306310c37d4c15141111d22baeaf"},
-    {url = "https://files.pythonhosted.org/packages/3b/06/af109f55f372e428d49d352228a6c14cd70946b20f36aa74185c2238d828/pyzmq-25.0.0-cp38-cp38-macosx_10_15_universal2.whl", hash = "sha256:e14df47c1265356715d3d66e90282a645ebc077b70b3806cf47efcb7d1d630cb"},
-    {url = "https://files.pythonhosted.org/packages/3f/fa/55c6f991e6eda6b79e4f7b3d940660ba47579fe9db5c966d92adf1b2110b/pyzmq-25.0.0-cp310-cp310-macosx_10_15_universal2.whl", hash = "sha256:2d05d904f03ddf1e0d83d97341354dfe52244a619b5a1440a5f47a5b3451e84e"},
-    {url = "https://files.pythonhosted.org/packages/41/a5/3fa528007e7f54fa4a6c76397ed994d7b82958bc1d641a7a1f692a0ff499/pyzmq-25.0.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:484c2c4ee02c1edc07039f42130bd16e804b1fe81c4f428e0042e03967f40c20"},
-    {url = "https://files.pythonhosted.org/packages/42/a8/14ef1a6526e709f81fb06aced32ba894098cf8037d21d5c243eb1aca95b5/pyzmq-25.0.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:8539216173135e9e89f6b1cc392e74e6b935b91e8c76106cf50e7a02ab02efe5"},
-    {url = "https://files.pythonhosted.org/packages/43/42/49d5ad17b3da40c5712f9eeb1452d507f9d534b520efa3eb9237990218ee/pyzmq-25.0.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:17e1cb97d573ea84d7cd97188b42ca6f611ab3ee600f6a75041294ede58e3d20"},
-    {url = "https://files.pythonhosted.org/packages/49/6a/8e85abffd399ecedeb5ca4e231c750e0ac7d2cac7dc08938d03f1bea4767/pyzmq-25.0.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:9a2d5e419bd39a1edb6cdd326d831f0120ddb9b1ff397e7d73541bf393294973"},
-    {url = "https://files.pythonhosted.org/packages/4a/58/7767b8311c2f28f52fecc2d561637ca19848d93c5bd27d633e70c9822099/pyzmq-25.0.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:293a7c2128690f496057f1f1eb6074f8746058d13588389981089ec45d8fdc77"},
-    {url = "https://files.pythonhosted.org/packages/4b/6b/f11212e1d0b1424f320e766383bcd53b9f62132ac313385589eeef37a918/pyzmq-25.0.0-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:5049e75cc99db65754a3da5f079230fb8889230cf09462ec972d884d1704a3ed"},
-    {url = "https://files.pythonhosted.org/packages/4b/c6/100d104d2924b20c906e358ab8253ec1cc8bf00a76e1c87e06c5fd5f7dd6/pyzmq-25.0.0-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:c48f257da280b3be6c94e05bd575eddb1373419dbb1a72c3ce64e88f29d1cd6d"},
-    {url = "https://files.pythonhosted.org/packages/51/aa/beee6940d0a19f48aea86616701a8b56706b72ee63d50484ebf0a8e68197/pyzmq-25.0.0-pp37-pypy37_pp73-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:a9c464cc508177c09a5a6122b67f978f20e2954a21362bf095a0da4647e3e908"},
-    {url = "https://files.pythonhosted.org/packages/53/42/c4f9a4a14fa4f10ef61a9f8d5d8587cb36e7109082a5ebaf2438cd8921bf/pyzmq-25.0.0-cp38-cp38-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:731b208bc9412deeb553c9519dca47136b5a01ca66667cafd8733211941b17e4"},
-    {url = "https://files.pythonhosted.org/packages/55/72/583bd1168ff88f52ffb82827a0498f59e0c2edbc844a74be86b3181cbfc0/pyzmq-25.0.0-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4046d03100aca266e70d54a35694cb35d6654cfbef633e848b3c4a8d64b9d187"},
-    {url = "https://files.pythonhosted.org/packages/55/7b/78a39bfcece02f6768952a951f013af60b42af525ebe1eef3d149af9d1e3/pyzmq-25.0.0-cp311-cp311-win32.whl", hash = "sha256:0282bba9aee6e0346aa27d6c69b5f7df72b5a964c91958fc9e0c62dcae5fdcdc"},
-    {url = "https://files.pythonhosted.org/packages/57/ac/67881ebf4380c7542d986e914829d32dabca027ac5a66087e5350644f3d8/pyzmq-25.0.0-cp38-cp38-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:b055a1cddf8035966ad13aa51edae5dc8f1bba0b5d5e06f7a843d8b83dc9b66b"},
-    {url = "https://files.pythonhosted.org/packages/5f/38/2665a604c359a779f6a4a091095ce57cd615b094c7d738c9dcad6df7b0ad/pyzmq-25.0.0-cp39-cp39-win32.whl", hash = "sha256:3670e8c5644768f214a3b598fe46378a4a6f096d5fb82a67dfd3440028460565"},
-    {url = "https://files.pythonhosted.org/packages/5f/47/194e743803010b7cd7dc6b461921e438abfa00a92700cf94af0750b327bf/pyzmq-25.0.0-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:ccb3e1a863222afdbda42b7ca8ac8569959593d7abd44f5a709177d6fa27d266"},
-    {url = "https://files.pythonhosted.org/packages/67/07/a78a31b9267ffb80319eda7eaa629fc95497be316ab18d5a58f560e18896/pyzmq-25.0.0-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:3100dddcada66ec5940ed6391ebf9d003cc3ede3d320748b2737553019f58230"},
-    {url = "https://files.pythonhosted.org/packages/67/ee/2319050b463e7e8dee5a2384a405816fbc51a558c88f11a3a436f079ad8a/pyzmq-25.0.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:af1fbfb7ad6ac0009ccee33c90a1d303431c7fb594335eb97760988727a37577"},
-    {url = "https://files.pythonhosted.org/packages/6a/93/7553f884201ee5d7da1455e6601b01898a26a6861cd864f009f7d432b6ec/pyzmq-25.0.0-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:2a73af6504e0d2805e926abf136ebf536735a13c22f709be7113c2ec65b4bec3"},
-    {url = "https://files.pythonhosted.org/packages/6c/1a/cd15043bf811ba492f512e481f8dcf223cb5bd6542cc5c10083c5ffd0a08/pyzmq-25.0.0-cp311-cp311-manylinux_2_28_x86_64.whl", hash = "sha256:4e295f7928a31ae0f657e848c5045ba6d693fe8921205f408ca3804b1b236968"},
-    {url = "https://files.pythonhosted.org/packages/74/7a/31d3b68d6dd7769736ee42d0558f901de6274c939d05425b71ee43a29490/pyzmq-25.0.0-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:00c94fd4c9dd3c95aace0c629a7fa713627a5c80c1819326b642adf6c4b8e2a2"},
-    {url = "https://files.pythonhosted.org/packages/77/6e/9ad415b182345a6cb477ea6e99e8d656a9b482d21dbf64db898a153527b2/pyzmq-25.0.0-pp37-pypy37_pp73-macosx_10_9_x86_64.whl", hash = "sha256:66509c48f7446b640eeae24b60c9c1461799a27b1b0754e438582e36b5af3315"},
-    {url = "https://files.pythonhosted.org/packages/77/9b/14de93488ac5ff111f3fcfdde9ea9e84906968282fddd2a265e07670cadb/pyzmq-25.0.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:4c25c95416133942280faaf068d0fddfd642b927fb28aaf4ab201a738e597c1e"},
-    {url = "https://files.pythonhosted.org/packages/7d/38/9d92d54501abbd98572c2e75c5e48157e2ae49f11edf9d11ce93777f9534/pyzmq-25.0.0-pp38-pypy38_pp73-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:5605621f2181f20b71f13f698944deb26a0a71af4aaf435b34dd90146092d530"},
-    {url = "https://files.pythonhosted.org/packages/7d/4d/65212414b17abbbd4a12110a5d32e64e9633700bae34e3b81e2ea17b2b0f/pyzmq-25.0.0-cp311-cp311-macosx_10_15_universal2.whl", hash = "sha256:e4bba04ea779a3d7ef25a821bb63fd0939142c88e7813e5bd9c6265a20c523a2"},
-    {url = "https://files.pythonhosted.org/packages/80/40/044fb4342b613ad45882dd3a1b7f34565885f5f12b833e9fb726e9cf55b4/pyzmq-25.0.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:75243e422e85a62f0ab7953dc315452a56b2c6a7e7d1a3c3109ac3cc57ed6b47"},
-    {url = "https://files.pythonhosted.org/packages/85/66/604961b4684a0e56b120b48185f700c8b5750bcb74df37b694054ea30eb1/pyzmq-25.0.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:60ecbfe7669d3808ffa8a7dd1487d6eb8a4015b07235e3b723d4b2a2d4de7203"},
-    {url = "https://files.pythonhosted.org/packages/87/da/96d981dc99ea4278d95642139ef25b08900a4db819b66b4ae3f9dd95cc3b/pyzmq-25.0.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:1f6116991568aac48b94d6d8aaed6157d407942ea385335a6ed313692777fb9d"},
-    {url = "https://files.pythonhosted.org/packages/8a/e5/96bfb6c6a630a4dfefb9a9a4de0b6339a124ff074d53b65d8ad7898ee14c/pyzmq-25.0.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9f72ea279b2941a5203e935a4588b9ba8a48aeb9a926d9dfa1986278bd362cb8"},
-    {url = "https://files.pythonhosted.org/packages/9b/72/9c6c6fa3da365a0acefd90a6e7a536cd8d9f891e5c77127be30be28d9a77/pyzmq-25.0.0-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:930e6ad4f2eaac31a3d0c2130619d25db754b267487ebc186c6ad18af2a74018"},
-    {url = "https://files.pythonhosted.org/packages/a6/19/0dad3c7298fd9085b699efeeeaedcf6d3b05f52eb01fac033b7d747e3a7a/pyzmq-25.0.0-cp311-cp311-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0645b5a2d2a06fd8eb738018490c514907f7488bf9359c6ee9d92f62e844b76f"},
-    {url = "https://files.pythonhosted.org/packages/ac/3a/fd0680f45a02bb24d40943e22f88ed28a4f292fa7fb96037b1cca37b50aa/pyzmq-25.0.0-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:f3f96d452e9580cb961ece2e5a788e64abaecb1232a80e61deffb28e105ff84a"},
-    {url = "https://files.pythonhosted.org/packages/b0/3c/0a309509141d670b70e126c6ba00f2d2dfe92649aacdc21dad48cd037e24/pyzmq-25.0.0-cp36-cp36m-win32.whl", hash = "sha256:926236ca003aec70574754f39703528947211a406f5c6c8b3e50eca04a9e87fc"},
-    {url = "https://files.pythonhosted.org/packages/b0/42/b4515c34658a0fc172edaf68982aa39b213c3677de7f56c2bc2a194d57ab/pyzmq-25.0.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:2754fa68da08a854f4816e05160137fa938a2347276471103d31e04bcee5365c"},
-    {url = "https://files.pythonhosted.org/packages/b0/df/5bfe59d286dd82fae92712f259c3b47926ec74d6708e9c27e5b424de24b7/pyzmq-25.0.0-cp38-cp38-win32.whl", hash = "sha256:6bf3842af37af43fa953e96074ebbb5315f6a297198f805d019d788a1021dbc8"},
-    {url = "https://files.pythonhosted.org/packages/b3/67/165b2b94bbbd2792896d095d49a1c148fc9eed7a387d2f09464959544e53/pyzmq-25.0.0-pp38-pypy38_pp73-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:0e8d00228db627ddd1b418c7afd81820b38575f237128c9650365f2dd6ac3443"},
-    {url = "https://files.pythonhosted.org/packages/b4/05/2e9aeb882648498c574d1a25a047acd03dc23b60016bb80085cbe78429e5/pyzmq-25.0.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:4725412e27612f0d7d7c2f794d89807ad0227c2fc01dd6146b39ada49c748ef9"},
-    {url = "https://files.pythonhosted.org/packages/b4/b9/0e2f77522c5e670abc4a8b95356522d0a6edd74f13821cdbbc3d0e64131d/pyzmq-25.0.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:531866c491aee5a1e967c286cfa470dffac1e2a203b1afda52d62b58782651e9"},
-    {url = "https://files.pythonhosted.org/packages/ba/0c/74ec9bd576d77adca6027fd7fb50f6bfad35ac1f72ca4bedfed2ac0bf69d/pyzmq-25.0.0-cp39-cp39-win_amd64.whl", hash = "sha256:e99629a976809fe102ef73e856cf4b2660acd82a412a51e80ba2215e523dfd0a"},
-    {url = "https://files.pythonhosted.org/packages/ba/75/6d49e003a07722166076764f6b9a6444a653a72a44912d93f14c21e8c09c/pyzmq-25.0.0-cp310-cp310-win_amd64.whl", hash = "sha256:58fc3ad5e1cfd2e6d24741fbb1e216b388115d31b0ca6670f894187f280b6ba6"},
-    {url = "https://files.pythonhosted.org/packages/c1/c5/531db8fdec6804a29bc6eaa914cc250d5f1f629f2db2b324fbccab03a348/pyzmq-25.0.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4cbb885f347eba7ab7681c450dee5b14aed9f153eec224ec0c3f299273d9241f"},
-    {url = "https://files.pythonhosted.org/packages/cb/4c/18a0ab6d3a5b41081c79cbb9e4086bea377e9f407a13b61853f6c2a5937d/pyzmq-25.0.0-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6136bfb0e5a9cf8c60c6ac763eb21f82940a77e6758ea53516c8c7074f4ff948"},
-    {url = "https://files.pythonhosted.org/packages/cf/75/3221b3999808566064bc94190678dc0058af651747279ed3eca159df550e/pyzmq-25.0.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:ac97e7d647d5519bcef48dd8d3d331f72975afa5c4496c95f6e854686f45e2d9"},
-    {url = "https://files.pythonhosted.org/packages/cf/89/9dbc5bc589a06e94d493b551177a0ebbe70f08b5ebdd49dddf212df869ff/pyzmq-25.0.0.tar.gz", hash = "sha256:f330a1a2c7f89fd4b0aa4dcb7bf50243bf1c8da9a2f1efc31daf57a2046b31f2"},
-    {url = "https://files.pythonhosted.org/packages/d1/b7/7e96fd2807992197a7eb383bfbc90950048260fd0aa51ae9c65caa9035f5/pyzmq-25.0.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:be05504af0619d1cffa500af1e0ede69fb683f301003851f5993b5247cc2c576"},
-    {url = "https://files.pythonhosted.org/packages/d4/9b/61d6cf04113855041cc22c1b66977657e7a323718eb89f4af54f4077212e/pyzmq-25.0.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:4a1bc30f0c18444d51e9b0d0dd39e3a4e7c53ee74190bebef238cd58de577ea9"},
-    {url = "https://files.pythonhosted.org/packages/d5/2e/e34c2187694d2fafc7237a6cf6267d9872c1524c965ca82b94d41fca9d62/pyzmq-25.0.0-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:81f99fb1224d36eb91557afec8cdc2264e856f3464500b55749020ce4c848ef2"},
-    {url = "https://files.pythonhosted.org/packages/d9/9a/fdd2cb5ebb01d48c7012b2c2eb0ddf677af534670650519b2fe2ac566e76/pyzmq-25.0.0-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:5050f5c50b58a6e38ccaf9263a356f74ef1040f5ca4030225d1cb1a858c5b7b6"},
-    {url = "https://files.pythonhosted.org/packages/da/3c/71ca87cf890ea30ea10862ea10db31838e054c296e775df2c8a50b6fd18d/pyzmq-25.0.0-cp310-cp310-manylinux_2_28_x86_64.whl", hash = "sha256:31e523d067ce44a04e876bed3ff9ea1ff8d1b6636d16e5fcace9d22f8c564369"},
-    {url = "https://files.pythonhosted.org/packages/dc/d2/432640692e3a1df103c9686c60fc973c63794911485f617cae697f781300/pyzmq-25.0.0-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:fc7c1421c5b1c916acf3128bf3cc7ea7f5018b58c69a6866d70c14190e600ce9"},
-    {url = "https://files.pythonhosted.org/packages/dd/f2/f3d56e4da8dbeff1aba3cb6a4ac694bcd3aae80af2b7df0fddc066a0590a/pyzmq-25.0.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b6f75b4b8574f3a8a0d6b4b52606fc75b82cb4391471be48ab0b8677c82f9ed4"},
-    {url = "https://files.pythonhosted.org/packages/df/58/5f5d88ada0e1059f6ac45412c86652f86821150cfeb225cf0bb94595aac5/pyzmq-25.0.0-cp36-cp36m-win_amd64.whl", hash = "sha256:94f0a7289d0f5c80807c37ebb404205e7deb737e8763eb176f4770839ee2a287"},
-    {url = "https://files.pythonhosted.org/packages/e8/07/d5ce55d1b93e16db0aa2344c5324c44e4cdc1c4f3e4ca24b8cce5f74bd56/pyzmq-25.0.0-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:e1081d7030a1229c8ff90120346fb7599b54f552e98fcea5170544e7c6725aab"},
-    {url = "https://files.pythonhosted.org/packages/eb/30/07fab0f1344cd32c739e3fa0e3f1a266350317e2f77e945f8eada47eae24/pyzmq-25.0.0-cp310-cp310-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2e7b87638ee30ab13230e37ce5331b3e730b1e0dda30120b9eeec3540ed292c8"},
-    {url = "https://files.pythonhosted.org/packages/f7/a2/17fa06423627a5e5e9902b7c77880824296c6fd479bbf4182ebcf10fd279/pyzmq-25.0.0-cp311-cp311-win_amd64.whl", hash = "sha256:526f884a27e8bba62fe1f4e07c62be2cfe492b6d432a8fdc4210397f8cf15331"},
-    {url = "https://files.pythonhosted.org/packages/f8/a2/85b36d137ef3b4f9806f6f21552c57c3dab592d540980fa8fd615a43f623/pyzmq-25.0.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:487305c2a011fdcf3db1f24e8814bb76d23bc4d2f46e145bc80316a59a9aa07d"},
-    {url = "https://files.pythonhosted.org/packages/f9/23/25dcac691eaf807e14bba4f3ba6a7777b2bba079bb6a1158c38614d2a801/pyzmq-25.0.0-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:20638121b0bdc80777ce0ec8c1f14f1ffec0697a1f88f0b564fa4a23078791c4"},
-    {url = "https://files.pythonhosted.org/packages/f9/51/9515efb57e6e46650d4dd78726fd1e5347e2b014ce94f482a12c1157d2d5/pyzmq-25.0.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:0a154ef810d44f9d28868be04641f837374a64e7449df98d9208e76c260c7ef1"},
-    {url = "https://files.pythonhosted.org/packages/f9/85/7a7b13f38287accea5bfdaf3e91daf8b017d6f2ed55ae17b7cfb3203293c/pyzmq-25.0.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:c21a5f4e54a807df5afdef52b6d24ec1580153a6bcf0607f70a6e1d9fa74c5c3"},
-    {url = "https://files.pythonhosted.org/packages/fd/79/b4fd6a902b5057ff9bd5de592550f6e8b91067b995dad4ccf37b07aa396d/pyzmq-25.0.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:183e18742be3621acf8908903f689ec520aee3f08449bfd29f583010ca33022b"},
-    {url = "https://files.pythonhosted.org/packages/fe/32/45d41f2e2316e534c004aea758500e17687afc36ec91e20137d8909538e1/pyzmq-25.0.0-cp39-cp39-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:610d2d112acd4e5501fac31010064a6c6efd716ceb968e443cae0059eb7b86de"},
-    {url = "https://files.pythonhosted.org/packages/fe/be/a0aa5e60693c0618f15ef8d1a0743ef8431d366b30b5bca41ea14f01391a/pyzmq-25.0.0-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:7877264aa851c19404b1bb9dbe6eed21ea0c13698be1eda3784aab3036d1c861"},
-]
-"qtconsole 5.4.0" = [
-    {url = "https://files.pythonhosted.org/packages/49/c6/345fffb3f6d8c9607deac4d5ff86e7ad9baf46171267585f5da10b3db890/qtconsole-5.4.0.tar.gz", hash = "sha256:57748ea2fd26320a0b77adba20131cfbb13818c7c96d83fafcb110ff55f58b35"},
-    {url = "https://files.pythonhosted.org/packages/cc/00/4133199dc738e7f497385af86e619f5c29592aaa4c1731fbbc3ec7bb7080/qtconsole-5.4.0-py3-none-any.whl", hash = "sha256:be13560c19bdb3b54ed9741a915aa701a68d424519e8341ac479a91209e694b2"},
-]
-"qtpy 2.3.0" = [
-    {url = "https://files.pythonhosted.org/packages/b0/96/4f3be023cee0261b1f6cd5d2f6c2a5abea8d8022fc66027da8792373a57e/QtPy-2.3.0.tar.gz", hash = "sha256:0603c9c83ccc035a4717a12908bf6bc6cb22509827ea2ec0e94c2da7c9ed57c5"},
-    {url = "https://files.pythonhosted.org/packages/ca/56/3dfbcf8a6808d2b3566b75759c48a281bcdc2b9547760e5d044e6ec7e33b/QtPy-2.3.0-py3-none-any.whl", hash = "sha256:8d6d544fc20facd27360ea189592e6135c614785f0dec0b4f083289de6beb408"},
-]
-"rfc3986 1.5.0" = [
-    {url = "https://files.pythonhosted.org/packages/79/30/5b1b6c28c105629cc12b33bdcbb0b11b5bb1880c6cfbd955f9e792921aa8/rfc3986-1.5.0.tar.gz", hash = "sha256:270aaf10d87d0d4e095063c65bf3ddbc6ee3d0b226328ce21e036f946e421835"},
-    {url = "https://files.pythonhosted.org/packages/c4/e5/63ca2c4edf4e00657584608bee1001302bbf8c5f569340b78304f2f446cb/rfc3986-1.5.0-py2.py3-none-any.whl", hash = "sha256:a86d6e1f5b1dc238b218b012df0aa79409667bb209e58da56d0b94704e712a97"},
-]
-"send2trash 1.8.0" = [
-    {url = "https://files.pythonhosted.org/packages/47/26/3435896d757335ea53dce5abf8d658ca80757a7a06258451b358f10232be/Send2Trash-1.8.0-py3-none-any.whl", hash = "sha256:f20eaadfdb517eaca5ce077640cb261c7d2698385a6a0f072a4a5447fd49fa08"},
-    {url = "https://files.pythonhosted.org/packages/49/2c/d990b8d5a7378dde856f5a82e36ed9d6061b5f2d00f39dc4317acd9538b4/Send2Trash-1.8.0.tar.gz", hash = "sha256:d2c24762fd3759860a0aff155e45871447ea58d2be6bdd39b5c8f966a0c99c2d"},
-]
-"setuptools 66.1.1" = [
-    {url = "https://files.pythonhosted.org/packages/3c/7b/00030a938499c8f8345be02ab5b7d748d359ea59c2f020b7b0a21b82f832/setuptools-66.1.1.tar.gz", hash = "sha256:ac4008d396bc9cd983ea483cb7139c0240a07bbc74ffb6232fceffedc6cf03a8"},
-    {url = "https://files.pythonhosted.org/packages/c2/8b/abb577ca6ab2c71814d535b1ed1464c5f4aaefe1a31bbeb85013eb9b2401/setuptools-66.1.1-py3-none-any.whl", hash = "sha256:6f590d76b713d5de4e49fe4fbca24474469f53c83632d5d0fd056f7ff7e8112b"},
+"pyzmq 25.1.0" = [
+    {url = "https://files.pythonhosted.org/packages/01/a7/6e28dec3ce5153066551d0ac229298628194f3f0150d535f84b698079675/pyzmq-25.1.0-pp37-pypy37_pp73-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:0c4fc2741e0513b5d5a12fe200d6785bbcc621f6f2278893a9ca7bed7f2efb7d"},
+    {url = "https://files.pythonhosted.org/packages/04/0b/bff5b6c1680e248bad2df8248a060645709fe2aef9689e9f7c81c587bad4/pyzmq-25.1.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f1e931d9a92f628858a50f5bdffdfcf839aebe388b82f9d2ccd5d22a38a789dc"},
+    {url = "https://files.pythonhosted.org/packages/04/15/b8ab292f0b74e0440547185fb67167c87454a2b3be429d64de569f7142a2/pyzmq-25.1.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:442d3efc77ca4d35bee3547a8e08e8d4bb88dadb54a8377014938ba98d2e074a"},
+    {url = "https://files.pythonhosted.org/packages/09/91/3848097505febfc464abfd4a3f41274de124e4e1c9f28da1326a85dd3d8b/pyzmq-25.1.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:3575699d7fd7c9b2108bc1c6128641a9a825a58577775ada26c02eb29e09c517"},
+    {url = "https://files.pythonhosted.org/packages/09/db/4c1351aa0ca08b7713002e0e8ab014ca42a83ca50d3c835e8b379d33e801/pyzmq-25.1.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2f666ae327a6899ff560d741681fdcdf4506f990595201ed39b44278c471ad98"},
+    {url = "https://files.pythonhosted.org/packages/14/bb/e18f866b0699bf5ea00f84daac1cf4a4557cea4fad96dd4a069b241dac9b/pyzmq-25.1.0-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:75217e83faea9edbc29516fc90c817bc40c6b21a5771ecb53e868e45594826b0"},
+    {url = "https://files.pythonhosted.org/packages/19/37/6aa1503e9e00a015abf80e999f8ecee699a485b873d1118667b98b9b6c03/pyzmq-25.1.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:be86a26415a8b6af02cd8d782e3a9ae3872140a057f1cadf0133de685185c02b"},
+    {url = "https://files.pythonhosted.org/packages/1b/43/16e6ee67582e7fcbe884b23d877c7eaf68b1c5fff0ab7a0c054eab2b8dc5/pyzmq-25.1.0-cp37-cp37m-win32.whl", hash = "sha256:95bd3a998d8c68b76679f6b18f520904af5204f089beebb7b0301d97704634dd"},
+    {url = "https://files.pythonhosted.org/packages/1b/91/94af7b477922e3a62e56c03ba7a89f74a8d9c36c5bc66e56651d2bda887e/pyzmq-25.1.0-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:01f06f33e12497dca86353c354461f75275a5ad9eaea181ac0dc1662da8074fa"},
+    {url = "https://files.pythonhosted.org/packages/20/e9/f16b101c6f4e2d93abeb50beb47f2c4ed333509700945003613c73c8942d/pyzmq-25.1.0-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:b324fa769577fc2c8f5efcd429cef5acbc17d63fe15ed16d6dcbac2c5eb00849"},
+    {url = "https://files.pythonhosted.org/packages/21/9b/b5a095f9ed610986c22cf59fce24bb985047a81ae48b4d6a39b4ffe116dd/pyzmq-25.1.0-pp38-pypy38_pp73-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:5e7fbcafa3ea16d1de1f213c226005fea21ee16ed56134b75b2dede5a2129e62"},
+    {url = "https://files.pythonhosted.org/packages/22/3e/3670e36c6f42e124492ddd2af550ca13bd4a9f1edd562e1ae7c35a1f230b/pyzmq-25.1.0-cp311-cp311-win32.whl", hash = "sha256:65346f507a815a731092421d0d7d60ed551a80d9b75e8b684307d435a5597425"},
+    {url = "https://files.pythonhosted.org/packages/26/81/aa471449e6641e72f7e8819ba4d8877523414734faa5b95a8b7eee964dfa/pyzmq-25.1.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:bad172aba822444b32eae54c2d5ab18cd7dee9814fd5c7ed026603b8cae2d05f"},
+    {url = "https://files.pythonhosted.org/packages/26/bb/80535157e8811095901f98688839092afb6dcaf2ff154aa8fa2e575f540d/pyzmq-25.1.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4a983c8694667fd76d793ada77fd36c8317e76aa66eec75be2653cef2ea72883"},
+    {url = "https://files.pythonhosted.org/packages/26/f5/a38810b94f023de1cf29c6ddad3a3e1af0f446716f3b011dd901c616bf4e/pyzmq-25.1.0-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:5873d6a60b778848ce23b6c0ac26c39e48969823882f607516b91fb323ce80e5"},
+    {url = "https://files.pythonhosted.org/packages/27/bb/a4d543592ed28075456033467d1649e4b81f7888d4d53b5dc2fbf47211b2/pyzmq-25.1.0-cp38-cp38-macosx_10_15_universal2.whl", hash = "sha256:3bed53f7218490c68f0e82a29c92335daa9606216e51c64f37b48eb78f1281f4"},
+    {url = "https://files.pythonhosted.org/packages/29/d4/632bb9ae332863c620564c00ba55d6937c801a99b02ecadab337b0e13139/pyzmq-25.1.0-pp37-pypy37_pp73-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:fc34fdd458ff77a2a00e3c86f899911f6f269d393ca5675842a6e92eea565bae"},
+    {url = "https://files.pythonhosted.org/packages/29/d9/6a12cae59202b85e65c8649c72099e126462aefca47a21a392317f080924/pyzmq-25.1.0-pp38-pypy38_pp73-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:adecf6d02b1beab8d7c04bc36f22bb0e4c65a35eb0b4750b91693631d4081c70"},
+    {url = "https://files.pythonhosted.org/packages/2f/53/fc7dbdd32e275aee0961e2a5bed1bb64223846f959fd6e0c9a39aab08eed/pyzmq-25.1.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:19d0383b1f18411d137d891cab567de9afa609b214de68b86e20173dc624c101"},
+    {url = "https://files.pythonhosted.org/packages/31/7e/47c490658a18e99485ec48e24326df7d264b9a7a15db5c692ef931d1b531/pyzmq-25.1.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:bdca18b94c404af6ae5533cd1bc310c4931f7ac97c148bbfd2cd4bdd62b96253"},
+    {url = "https://files.pythonhosted.org/packages/32/e4/ce4f94009f84c2a688082c2674d490d2e20e0c9058087f5358a2bf29ddf1/pyzmq-25.1.0-cp310-cp310-win_amd64.whl", hash = "sha256:5693dcc4f163481cf79e98cf2d7995c60e43809e325b77a7748d8024b1b7bcba"},
+    {url = "https://files.pythonhosted.org/packages/38/ed/250acfa9f9953a99fa3568f305688c4097e545df87d42d13f3dc3a25c5f2/pyzmq-25.1.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7e23a8c3b6c06de40bdb9e06288180d630b562db8ac199e8cc535af81f90e64b"},
+    {url = "https://files.pythonhosted.org/packages/3d/0b/5c1a99032dfb12d0b3619ab031d7fd9191fc6378926565f6d635f43ba26c/pyzmq-25.1.0-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8b697774ea8273e3c0460cf0bba16cd85ca6c46dfe8b303211816d68c492e132"},
+    {url = "https://files.pythonhosted.org/packages/3e/71/3f41e23f14b04b87776497d5d5150335e6d7e06debf1571fd5ca4c6ff82a/pyzmq-25.1.0-cp38-cp38-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:9301cf1d7fc1ddf668d0abbe3e227fc9ab15bc036a31c247276012abb921b5ff"},
+    {url = "https://files.pythonhosted.org/packages/3f/f5/fd2230639b14eed05a1d978bf456e2033afcf4bc8ebaff29e58cd3ae717c/pyzmq-25.1.0-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:5489738a692bc7ee9a0a7765979c8a572520d616d12d949eaffc6e061b82b4d1"},
+    {url = "https://files.pythonhosted.org/packages/40/2b/7ff4e0175a5029751fd52c6a1f57606f6c3bb0a420da52f3271a0c0599c3/pyzmq-25.1.0-cp38-cp38-win_amd64.whl", hash = "sha256:c66b7ff2527e18554030319b1376d81560ca0742c6e0b17ff1ee96624a5f1afd"},
+    {url = "https://files.pythonhosted.org/packages/46/99/588928fd4010f0ccfc3128ec96c70c201f8c3053fbbbcd4b09136d46ec83/pyzmq-25.1.0-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:48e5e59e77c1a83162ab3c163fc01cd2eebc5b34560341a67421b09be0891287"},
+    {url = "https://files.pythonhosted.org/packages/4d/73/1ed2c2a7f73b9d2d902c101612e5cf20c4db17e818336e4194a7f5676fcf/pyzmq-25.1.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:4a82faae00d1eed4809c2f18b37f15ce39a10a1c58fe48b60ad02875d6e13d80"},
+    {url = "https://files.pythonhosted.org/packages/53/17/6a70f84b79e361af34f6c99064ecf9e87112c4c48b9c7ea78f8e680b57d8/pyzmq-25.1.0-cp310-cp310-macosx_10_15_universal2.whl", hash = "sha256:1a6169e69034eaa06823da6a93a7739ff38716142b3596c180363dee729d713d"},
+    {url = "https://files.pythonhosted.org/packages/54/4a/2ebfd6ae510e89feb382714d7ff016892d6f08f24365888978bea91cf405/pyzmq-25.1.0-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:6581e886aec3135964a302a0f5eb68f964869b9efd1dbafdebceaaf2934f8a68"},
+    {url = "https://files.pythonhosted.org/packages/56/5f/e15a82d79527424ceda0bc4da7582881270b6e2e19624c7114fb1cc72857/pyzmq-25.1.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:c8398a1b1951aaa330269c35335ae69744be166e67e0ebd9869bdc09426f3871"},
+    {url = "https://files.pythonhosted.org/packages/56/fb/fef967daf8dfcb6fb63dbee60a33a7b203061fdfa4d5131fbcfaa08abcba/pyzmq-25.1.0-cp37-cp37m-win_amd64.whl", hash = "sha256:dbc466744a2db4b7ca05589f21ae1a35066afada2f803f92369f5877c100ef62"},
+    {url = "https://files.pythonhosted.org/packages/57/c1/cf092445d442805b2ae942c2a92ac431a2afe5ff56bbe937adfdc9cf41f5/pyzmq-25.1.0-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:f45808eda8b1d71308c5416ef3abe958f033fdbb356984fabbfc7887bed76b3f"},
+    {url = "https://files.pythonhosted.org/packages/5a/b6/3c2ddd09aa24352e4f6aade53e9b9a1816c0774c844f11b1a2f508ddc0be/pyzmq-25.1.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:69511d604368f3dc58d4be1b0bad99b61ee92b44afe1cd9b7bd8c5e34ea8248a"},
+    {url = "https://files.pythonhosted.org/packages/5d/68/c91c79e46809e8bd590bdde18a61ded6c95173461a459239a6bb79d8c351/pyzmq-25.1.0-cp38-cp38-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:ddbef8b53cd16467fdbfa92a712eae46dd066aa19780681a2ce266e88fbc7165"},
+    {url = "https://files.pythonhosted.org/packages/5d/b7/8ca362952b14734804f95190e0a7c517185d40fad1b9e217063e6bea6de5/pyzmq-25.1.0-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:9e68ae9864d260b18f311b68d29134d8776d82e7f5d75ce898b40a88df9db30f"},
+    {url = "https://files.pythonhosted.org/packages/5e/9e/32074bd8bcf2a5cf282d8817458fd5479c68b487b6c3a5d4627711ad38f5/pyzmq-25.1.0-cp310-cp310-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:97d984b1b2f574bc1bb58296d3c0b64b10e95e7026f8716ed6c0b86d4679843f"},
+    {url = "https://files.pythonhosted.org/packages/5f/d7/397af40b3e072bd5b4b4657962f64dfbe7b81c8bbf7a42affd510e8a1e1a/pyzmq-25.1.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:851fb2fe14036cfc1960d806628b80276af5424db09fe5c91c726890c8e6d943"},
+    {url = "https://files.pythonhosted.org/packages/64/9c/2b2614b0b86ff703b3a33ea5e044923bd7d100adc8c829d579a9b71ea9e7/pyzmq-25.1.0.tar.gz", hash = "sha256:80c41023465d36280e801564a69cbfce8ae85ff79b080e1913f6e90481fb8957"},
+    {url = "https://files.pythonhosted.org/packages/64/db/e19f69fe9b1a4e53f6382274f553358e2e7305d2a2b9d9db36087bf52d5e/pyzmq-25.1.0-cp310-cp310-win32.whl", hash = "sha256:be24a5867b8e3b9dd5c241de359a9a5217698ff616ac2daa47713ba2ebe30ad1"},
+    {url = "https://files.pythonhosted.org/packages/66/96/129706be681649f43bde93811416f566acfefcd3fb18156d5df349c360ab/pyzmq-25.1.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:3a522510e3434e12aff80187144c6df556bb06fe6b9d01b2ecfbd2b5bfa5c60c"},
+    {url = "https://files.pythonhosted.org/packages/66/f5/15db4c297957f049cd4dcd35eb7fbe9098a72489e0abdb289c529d7327cc/pyzmq-25.1.0-cp311-cp311-manylinux_2_28_x86_64.whl", hash = "sha256:cad9545f5801a125f162d09ec9b724b7ad9b6440151b89645241d0120e119dcc"},
+    {url = "https://files.pythonhosted.org/packages/73/4f/7ce249548ea059758365fef953eb69a592c9407478474c39f9e7ee791e58/pyzmq-25.1.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:d40682ac60b2a613d36d8d3a0cd14fbdf8e7e0618fbb40aa9fa7b796c9081584"},
+    {url = "https://files.pythonhosted.org/packages/77/3b/8861b96c17a8d9c672338e124f1f71ef759ffb7557438c1be4e5b7162c3d/pyzmq-25.1.0-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5af31493663cf76dd36b00dafbc839e83bbca8a0662931e11816d75f36155897"},
+    {url = "https://files.pythonhosted.org/packages/78/54/62b368a4287893140cb980786da07d95d86cd2bc075a802f1e70c45c83d2/pyzmq-25.1.0-cp38-cp38-win32.whl", hash = "sha256:33d5c8391a34d56224bccf74f458d82fc6e24b3213fc68165c98b708c7a69325"},
+    {url = "https://files.pythonhosted.org/packages/7c/65/bccec1eae7c0e089d90648f350e6c2ff40ccb8c6d1b929548f4cd304b1f7/pyzmq-25.1.0-cp311-cp311-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:332616f95eb400492103ab9d542b69d5f0ff628b23129a4bc0a2fd48da6e4e0b"},
+    {url = "https://files.pythonhosted.org/packages/80/b3/70a9d6af68d9fe34ec6444241267282d0740cc6fac3bb79c9c1ba472954a/pyzmq-25.1.0-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e21cc00e4debe8f54c3ed7b9fcca540f46eee12762a9fa56feb8512fd9057161"},
+    {url = "https://files.pythonhosted.org/packages/84/70/749d4ee05aa77aba900dc2105964c34a9d8ae3da7dc80fc97716e66ce54c/pyzmq-25.1.0-cp36-cp36m-win_amd64.whl", hash = "sha256:968b0c737797c1809ec602e082cb63e9824ff2329275336bb88bd71591e94a90"},
+    {url = "https://files.pythonhosted.org/packages/8b/e0/79d63c46e0481c89be7d93b69ff22f5ba59caef64c0c52552b2c0fdbb7d7/pyzmq-25.1.0-pp37-pypy37_pp73-macosx_10_9_x86_64.whl", hash = "sha256:4cb27ef9d3bdc0c195b2dc54fcb8720e18b741624686a81942e14c8b67cc61a6"},
+    {url = "https://files.pythonhosted.org/packages/8e/e0/452f4dd0a9a4725bceb836643c056614b0cd3aa291fd1bce76ba1d605704/pyzmq-25.1.0-cp39-cp39-win_amd64.whl", hash = "sha256:71c7b5896e40720d30cd77a81e62b433b981005bbff0cb2f739e0f8d059b5d99"},
+    {url = "https://files.pythonhosted.org/packages/94/3a/c3964c0a86c3535ae240799d3b7c8e13527e7a092080dda9012b1401fa86/pyzmq-25.1.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:90146ab578931e0e2826ee39d0c948d0ea72734378f1898939d18bc9c823fcf9"},
+    {url = "https://files.pythonhosted.org/packages/94/4b/1093172b73984b568d9f1a72bcd61793822fab40aa571f5d6ed9db6234cb/pyzmq-25.1.0-cp39-cp39-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:4c2fc7aad520a97d64ffc98190fce6b64152bde57a10c704b337082679e74f67"},
+    {url = "https://files.pythonhosted.org/packages/9a/d9/c52c13720b8724922af56b5af9ded75ee5b170821d915a1849655e19f9a6/pyzmq-25.1.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:108c96ebbd573d929740d66e4c3d1bdf31d5cde003b8dc7811a3c8c5b0fc173b"},
+    {url = "https://files.pythonhosted.org/packages/9c/4b/be619e68131f185850e5dfb7af6119f9a4edaf8ec15d36e4fc3bfe72fc9d/pyzmq-25.1.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:3830be8826639d801de9053cf86350ed6742c4321ba4236e4b5568528d7bfed7"},
+    {url = "https://files.pythonhosted.org/packages/a0/db/4e586c563b48dec09b8f7c2728b905e29db61af89b5c58e4eba9ad36fdec/pyzmq-25.1.0-cp311-cp311-win_amd64.whl", hash = "sha256:8b45d722046fea5a5694cba5d86f21f78f0052b40a4bbbbf60128ac55bfcc7b6"},
+    {url = "https://files.pythonhosted.org/packages/a1/87/92556ffa8fbe7dc497d847e39d5c46134f9ad047b23f5bcefc8fbd0c2c9c/pyzmq-25.1.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:831ba20b660b39e39e5ac8603e8193f8fce1ee03a42c84ade89c36a251449d80"},
+    {url = "https://files.pythonhosted.org/packages/a8/2e/fb4836e1a6d89d6e05d5058ed60e7be8aa3dfa41a022428a6d0c13784401/pyzmq-25.1.0-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:47b915ba666c51391836d7ed9a745926b22c434efa76c119f77bcffa64d2c50c"},
+    {url = "https://files.pythonhosted.org/packages/a9/85/6c4dc21d96f4e2bbc45f0e2bab843e6f3fa9d1817711cad8a222219e10f5/pyzmq-25.1.0-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:f0d9e7ba6a815a12c8575ba7887da4b72483e4cfc57179af10c9b937f3f9308f"},
+    {url = "https://files.pythonhosted.org/packages/b4/eb/23d3ebec493bc620a5760079ffa4244b92c2851ab621626a08d1b73391bc/pyzmq-25.1.0-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:5482f08d2c3c42b920e8771ae8932fbaa0a67dff925fc476996ddd8155a170f3"},
+    {url = "https://files.pythonhosted.org/packages/b7/cb/2a36d3eed310efb342fbb7b4adf6b05f46401c4b937154bd1c9b703314e0/pyzmq-25.1.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:58416db767787aedbfd57116714aad6c9ce57215ffa1c3758a52403f7c68cff5"},
+    {url = "https://files.pythonhosted.org/packages/b9/86/1d7b7704d8c82fe64da255fa0936964feec921550e3338bd554b7c184fe3/pyzmq-25.1.0-pp37-pypy37_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8751f9c1442624da391bbd92bd4b072def6d7702a9390e4479f45c182392ff78"},
+    {url = "https://files.pythonhosted.org/packages/bb/80/ae792378f98d6d0e39c975c334603d3d2535f7897707fe91f31d37f94fdb/pyzmq-25.1.0-cp311-cp311-macosx_10_15_universal2.whl", hash = "sha256:13bbe36da3f8aaf2b7ec12696253c0bf6ffe05f4507985a8844a1081db6ec22d"},
+    {url = "https://files.pythonhosted.org/packages/c5/2c/5a1d77e8112401b2189247acad9b10fc7adc79b8f2ad43e987bce8e89092/pyzmq-25.1.0-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f6d39e42a0aa888122d1beb8ec0d4ddfb6c6b45aecb5ba4013c27e2f28657765"},
+    {url = "https://files.pythonhosted.org/packages/ca/db/f9976803f1a660e753d0f2426065975bad5db8272fd5284efaf488dc0ce1/pyzmq-25.1.0-cp310-cp310-manylinux_2_28_x86_64.whl", hash = "sha256:cb6d161ae94fb35bb518b74bb06b7293299c15ba3bc099dccd6a5b7ae589aee3"},
+    {url = "https://files.pythonhosted.org/packages/d5/81/6e36c26c541845e3ee917deb1b96201eceab03e7bd04d345d8de24f793dc/pyzmq-25.1.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2f5efcc29056dfe95e9c9db0dfbb12b62db9c4ad302f812931b6d21dd04a9119"},
+    {url = "https://files.pythonhosted.org/packages/d7/ac/4856333a4fd737fb7cf75b62ec0b82a3a3bdce3a9211ed18288f9a645091/pyzmq-25.1.0-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:414b8beec76521358b49170db7b9967d6974bdfc3297f47f7d23edec37329b00"},
+    {url = "https://files.pythonhosted.org/packages/de/49/d94114d1f8b4f86dab28e86d6ca631060a482382524bca79d7aca8f631a2/pyzmq-25.1.0-cp36-cp36m-win32.whl", hash = "sha256:b5a07c4f29bf7cb0164664ef87e4aa25435dcc1f818d29842118b0ac1eb8e2b5"},
+    {url = "https://files.pythonhosted.org/packages/e4/21/7f80485903510a4c9583d41044a789976a2be0407d7c72c32e7a46afd090/pyzmq-25.1.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:2a21fec5c3cea45421a19ccbe6250c82f97af4175bc09de4d6dd78fb0cb4c200"},
+    {url = "https://files.pythonhosted.org/packages/e5/bb/25c22e1eb6182ad4fec43310087ffd46dba6676b86593e5a4d5b5ff24a7a/pyzmq-25.1.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:7018289b402ebf2b2c06992813523de61d4ce17bd514c4339d8f27a6f6809492"},
+    {url = "https://files.pythonhosted.org/packages/ed/6f/54f5b5dc3734d212b1b21c14d7df7cb0d40b8cb2b820c1ff8f36e9d7501d/pyzmq-25.1.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:1fc56a0221bdf67cfa94ef2d6ce5513a3d209c3dfd21fed4d4e87eca1822e3a3"},
+    {url = "https://files.pythonhosted.org/packages/f2/f5/43fabde73ffc6fdb39a80d3afb7d283ce64e861cc8a96fad34518d917391/pyzmq-25.1.0-cp39-cp39-macosx_10_15_universal2.whl", hash = "sha256:af56229ea6527a849ac9fb154a059d7e32e77a8cba27e3e62a1e38d8808cb1a5"},
+    {url = "https://files.pythonhosted.org/packages/f8/2a/952facb087422ac084b35674343cedeb7b517f8b41a7db0f71096eba3df5/pyzmq-25.1.0-cp39-cp39-win32.whl", hash = "sha256:4d67609b37204acad3d566bb7391e0ecc25ef8bae22ff72ebe2ad7ffb7847158"},
+    {url = "https://files.pythonhosted.org/packages/f9/39/647cb2c45c1d4db11cbc87c03d3e511e016e6d2f239630a1ab56c3588586/pyzmq-25.1.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:eb52e826d16c09ef87132c6e360e1879c984f19a4f62d8a935345deac43f3c12"},
+    {url = "https://files.pythonhosted.org/packages/fa/40/7729719e38324e5e9f2e77f6131fc253f063a3741eab170ef610196098e8/pyzmq-25.1.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:d6128d431b8dfa888bf51c22a04d48bcb3d64431caf02b3cb943269f17fd2994"},
+    {url = "https://files.pythonhosted.org/packages/fa/fb/a114ba641eb873c165106d3c8ee75eb49d6ea3204168808708d866de360d/pyzmq-25.1.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:154bddda2a351161474b36dba03bf1463377ec226a13458725183e508840df89"},
+    {url = "https://files.pythonhosted.org/packages/fd/12/0324dcb2554cd3f2ebb851ddbfbac27c4bb384394ba4a8978dec093fe71d/pyzmq-25.1.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:2b15247c49d8cbea695b321ae5478d47cffd496a2ec5ef47131a9e79ddd7e46c"},
+    {url = "https://files.pythonhosted.org/packages/ff/19/f027b4b9067a5398cbccc6322ca14a6b2c872b633ed6b2a09bb53c0cf0b7/pyzmq-25.1.0-cp39-cp39-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:0b6b42f7055bbc562f63f3df3b63e3dd1ebe9727ff0f124c3aa7bcea7b3a00f9"},
+]
+"qtconsole 5.4.3" = [
+    {url = "https://files.pythonhosted.org/packages/18/3b/7bdbb99256d1406ae6c8904355222c6dc010640e6be158830f48b7097b32/qtconsole-5.4.3-py3-none-any.whl", hash = "sha256:35fd6e87b1f6d1fd41801b07e69339f8982e76afd4fa8ef35595bc6036717189"},
+    {url = "https://files.pythonhosted.org/packages/6f/6c/0e20886d4024f8b0dec690f2be0206dbad3abab9b87fc90fba8b990c720a/qtconsole-5.4.3.tar.gz", hash = "sha256:5e4082a86a201796b2a5cfd4298352d22b158b51b57736531824715fc2a979dd"},
+]
+"qtpy 2.3.1" = [
+    {url = "https://files.pythonhosted.org/packages/51/9f/495736f9bbebc56b9f2ba3d95df1045fd367378254f799e86463b0037ab0/QtPy-2.3.1-py3-none-any.whl", hash = "sha256:5193d20e0b16e4d9d3bc2c642d04d9f4e2c892590bd1b9c92bfe38a95d5a2e12"},
+    {url = "https://files.pythonhosted.org/packages/ad/6b/0e753af1197f82d2359c9aa91cef8abaaef4c547396ffdc71ea6a889e52c/QtPy-2.3.1.tar.gz", hash = "sha256:a8c74982d6d172ce124d80cafd39653df78989683f760f2281ba91a6e7b9de8b"},
+]
+"send2trash 1.8.2" = [
+    {url = "https://files.pythonhosted.org/packages/4a/d2/d4b4d8b1564752b4e593c6d007426172b6574df5a7c07322feba010f5551/Send2Trash-1.8.2.tar.gz", hash = "sha256:c132d59fa44b9ca2b1699af5c86f57ce9f4c5eb56629d5d55fbb7a35f84e2312"},
+    {url = "https://files.pythonhosted.org/packages/a9/78/e4df1e080ed790acf3a704edf521006dd96b9841bd2e2a462c0d255e0565/Send2Trash-1.8.2-py3-none-any.whl", hash = "sha256:a384719d99c07ce1eefd6905d2decb6f8b7ed054025bb0e618919f945de4f679"},
+]
+"setuptools 67.8.0" = [
+    {url = "https://files.pythonhosted.org/packages/03/20/630783571e76e5fa5f3e9f29398ca3ace377207b8196b54e0ffdf09f12c1/setuptools-67.8.0.tar.gz", hash = "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"},
+    {url = "https://files.pythonhosted.org/packages/f5/2c/074ab1c5be9c7d523d8d6d69d1f46f450fe7f11713147dc9e779aa4ca4ea/setuptools-67.8.0-py3-none-any.whl", hash = "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f"},
 ]
 "six 1.16.0" = [
     {url = "https://files.pythonhosted.org/packages/71/39/171f1c67cd00715f190ba0b100d606d440a28c93c7714febeca8b79af85e/six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
     {url = "https://files.pythonhosted.org/packages/d9/5a/e7c31adbe875f2abbb91bd84cf2dc52d792b5a01506781dbcf25c91daf11/six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
 ]
 "sniffio 1.3.0" = [
     {url = "https://files.pythonhosted.org/packages/c3/a0/5dba8ed157b0136607c7f2151db695885606968d1fae123dc3391e0cfdbf/sniffio-1.3.0-py3-none-any.whl", hash = "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"},
     {url = "https://files.pythonhosted.org/packages/cd/50/d49c388cae4ec10e8109b1b833fd265511840706808576df3ada99ecb0ac/sniffio-1.3.0.tar.gz", hash = "sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101"},
 ]
 "snowballstemmer 2.2.0" = [
     {url = "https://files.pythonhosted.org/packages/44/7b/af302bebf22c749c56c9c3e8ae13190b5b5db37a33d9068652e8f73b7089/snowballstemmer-2.2.0.tar.gz", hash = "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1"},
     {url = "https://files.pythonhosted.org/packages/ed/dc/c02e01294f7265e63a7315fe086dd1df7dacb9f840a804da846b96d01b96/snowballstemmer-2.2.0-py2.py3-none-any.whl", hash = "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"},
 ]
-"soupsieve 2.3.2.post1" = [
-    {url = "https://files.pythonhosted.org/packages/16/e3/4ad79882b92617e3a4a0df1960d6bce08edfb637737ac5c3f3ba29022e25/soupsieve-2.3.2.post1-py3-none-any.whl", hash = "sha256:3b2503d3c7084a42b1ebd08116e5f81aadfaea95863628c80a3b774a11b7c759"},
-    {url = "https://files.pythonhosted.org/packages/f3/03/bac179d539362319b4779a00764e95f7542f4920084163db6b0fd4742d38/soupsieve-2.3.2.post1.tar.gz", hash = "sha256:fc53893b3da2c33de295667a0e19f078c14bf86544af307354de5fcf12a3f30d"},
+"soupsieve 2.4.1" = [
+    {url = "https://files.pythonhosted.org/packages/47/9e/780779233a615777fbdf75a4dee2af7a345f4bf74b42d4a5f836800b9d91/soupsieve-2.4.1.tar.gz", hash = "sha256:89d12b2d5dfcd2c9e8c22326da9d9aa9cb3dfab0a83a024f05704076ee8d35ea"},
+    {url = "https://files.pythonhosted.org/packages/49/37/673d6490efc51ec46d198c75903d99de59baffdd47aea3d071b80a9e4e89/soupsieve-2.4.1-py3-none-any.whl", hash = "sha256:1c1bfee6819544a3447586c889157365a27e10d88cde3ad3da0cf0ddf646feb8"},
 ]
 "terminado 0.17.1" = [
     {url = "https://files.pythonhosted.org/packages/55/be/748034192602b9fd69ba94544c1675ff18b039ed8f346ad783478e31144f/terminado-0.17.1.tar.gz", hash = "sha256:6ccbbcd3a4f8a25a5ec04991f39a0b8db52dfcd487ea0e578d977e6752380333"},
     {url = "https://files.pythonhosted.org/packages/84/a7/c7628d79651b8c8c775d27b374315a825141b5783512e82026fb210dd639/terminado-0.17.1-py3-none-any.whl", hash = "sha256:8650d44334eba354dd591129ca3124a6ba42c3d5b70df5051b6921d506fdaeae"},
 ]
 "tinycss2 1.2.1" = [
     {url = "https://files.pythonhosted.org/packages/75/be/24179dfaa1d742c9365cbd0e3f0edc5d3aa3abad415a2327c5a6ff8ca077/tinycss2-1.2.1.tar.gz", hash = "sha256:8cff3a8f066c2ec677c06dbc7b45619804a6938478d9d73c284b29d14ecb0627"},
@@ -1802,17 +1813,17 @@
     {url = "https://files.pythonhosted.org/packages/71/cc/c1342382484d0178a79029109c433e406a60095da1c3605ca966775a70e5/tornado-6.2-cp37-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ba09ef14ca9893954244fd872798b4ccb2367c165946ce2dd7376aebdde8e3ac"},
     {url = "https://files.pythonhosted.org/packages/cd/a4/761e45cea12b2af076d36240d464b371ab1231272948cdc49b7d81855c5c/tornado-6.2-cp37-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:5f8c52d219d4995388119af7ccaa0bcec289535747620116a58d830e7c25d8a8"},
     {url = "https://files.pythonhosted.org/packages/ec/01/93e63530851ba8ef9685f1a9b91e324b28d28323a6b67400114ea65c5110/tornado-6.2-cp37-abi3-win32.whl", hash = "sha256:5c87076709343557ef8032934ce5f637dbb552efa7b21d08e89ae7619ed0eb23"},
     {url = "https://files.pythonhosted.org/packages/f3/9e/225a41452f2d9418d89be5e32cf824c84fe1e639d350d6e8d49db5b7f73a/tornado-6.2.tar.gz", hash = "sha256:9b630419bde84ec666bfd7ea0a4cb2a8a651c2d5cccdbdd1972a0c859dfc3c13"},
     {url = "https://files.pythonhosted.org/packages/f9/51/6f63a166d9a3077be100cbb13dcbce434e5654daaaa7003b0a045b9f6edf/tornado-6.2-cp37-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:1d54d13ab8414ed44de07efecb97d4ef7c39f7438cf5e976ccd356bebb1b5fca"},
     {url = "https://files.pythonhosted.org/packages/fb/bd/074254a55bfc82d7a1886abbd803600ef01cbd76ee66bc30307b2724130b/tornado-6.2-cp37-abi3-macosx_10_9_universal2.whl", hash = "sha256:20f638fd8cc85f3cbae3c732326e96addff0a15e22d80f049e00121651e82e72"},
 ]
-"traitlets 5.8.1" = [
-    {url = "https://files.pythonhosted.org/packages/76/fa/bd160e08ac7f656d818a0e40ff88e1a302b07ad2384864fb288db3c812fa/traitlets-5.8.1-py3-none-any.whl", hash = "sha256:a1ca5df6414f8b5760f7c5f256e326ee21b581742114545b462b35ffe3f04861"},
-    {url = "https://files.pythonhosted.org/packages/be/58/2d930cfab2caca22c827229ca61aabd8102423f7e817805cba706dce1598/traitlets-5.8.1.tar.gz", hash = "sha256:32500888f5ff7bbf3b9267ea31748fa657aaf34d56d85e60f91dda7dc7f5785b"},
+"traitlets 5.9.0" = [
+    {url = "https://files.pythonhosted.org/packages/39/c3/205e88f02959712b62008502952707313640369144a7fded4cbc61f48321/traitlets-5.9.0.tar.gz", hash = "sha256:f6cde21a9c68cf756af02035f72d5a723bf607e862e7be33ece505abf4a3bad9"},
+    {url = "https://files.pythonhosted.org/packages/77/75/c28e9ef7abec2b7e9ff35aea3e0be6c1aceaf7873c26c95ae1f0d594de71/traitlets-5.9.0-py3-none-any.whl", hash = "sha256:9e6ec080259b9a5940c797d58b613b5e31441c2257b87c2e795c5228ae80d2d8"},
 ]
 "typed-ast 1.5.4" = [
     {url = "https://files.pythonhosted.org/packages/04/93/482d12fd3334b53ec4087e658ab161ab23affcf8b052166b4cf972ca673b/typed_ast-1.5.4-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:6778e1b2f81dfc7bc58e4b259363b83d2e509a65198e85d5700dfae4c6c8ff1c"},
     {url = "https://files.pythonhosted.org/packages/07/d2/d55702e8deba2c80282fea0df53130790d8f398648be589750954c2dcce4/typed_ast-1.5.4.tar.gz", hash = "sha256:39e21ceb7388e4bb37f4c679d72707ed46c2fbf2a5609b8b8ebc4b067d977df2"},
     {url = "https://files.pythonhosted.org/packages/0b/e7/8ec06fc870254889198f933a595f139b7871b24bab1116d6128440731ea9/typed_ast-1.5.4-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3e123d878ba170397916557d31c8f589951e353cc95fb7f24f6bb69adc1a8a97"},
     {url = "https://files.pythonhosted.org/packages/0f/59/430b86961d63278fcbced5ba72655ee93aa35e8e908bad4ff138480eb25d/typed_ast-1.5.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:669dd0c4167f6f2cd9f57041e03c3c2ebf9063d0757dc89f79ba1daa2bfca9d4"},
     {url = "https://files.pythonhosted.org/packages/1a/f6/dd891624aaf98b918d7012b9d01753d0192c4eb18cf33ce616c0e08f62ba/typed_ast-1.5.4-cp37-cp37m-win_amd64.whl", hash = "sha256:0261195c2062caf107831e92a76764c81227dae162c4f75192c0d489faf751a2"},
@@ -1832,110 +1843,111 @@
     {url = "https://files.pythonhosted.org/packages/ca/da/fbc14befbf19d69d05b4b8b019edbc6554d958037a821c6d5585767fe0ff/typed_ast-1.5.4-cp39-cp39-win_amd64.whl", hash = "sha256:0fdbcf2fef0ca421a3f5912555804296f0b0960f0418c440f5d6d3abb549f3e1"},
     {url = "https://files.pythonhosted.org/packages/cd/f3/188eede730be3f6ddb9a788cd6b7289207c5fceebbf8ae190f9716dd8c05/typed_ast-1.5.4-cp310-cp310-win_amd64.whl", hash = "sha256:a9916d2bb8865f973824fb47436fa45e1ebf2efd920f2b9f99342cb7fab93f72"},
     {url = "https://files.pythonhosted.org/packages/d8/4e/db9505b53c44d7bc324a3d2e09bdf82b0943d6e08b183ae382860f482a87/typed_ast-1.5.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:98f80dee3c03455e92796b58b98ff6ca0b2a6f652120c263efdba4d6c5e58f72"},
     {url = "https://files.pythonhosted.org/packages/dd/87/09764c19a60a192b935579c93a07e781f6a52def10b723c8c5748e69a863/typed_ast-1.5.4-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ed855bbe3eb3715fca349c80174cfcfd699c2f9de574d40527b8429acae23a66"},
     {url = "https://files.pythonhosted.org/packages/e3/7c/7407838e9c540031439f2948bce2763cdd6882ebb72cc0a25b763c10529e/typed_ast-1.5.4-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:183afdf0ec5b1b211724dfef3d2cad2d767cbefac291f24d69b00546c1837fb6"},
     {url = "https://files.pythonhosted.org/packages/f9/57/89ac0020d5ffc762487376d0c78e5d02af795657f18c411155b73de3c765/typed_ast-1.5.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:4879da6c9b73443f97e731b617184a596ac1235fe91f98d279a7af36c796da35"},
 ]
-"typing-extensions 4.4.0" = [
-    {url = "https://files.pythonhosted.org/packages/0b/8e/f1a0a5a76cfef77e1eb6004cb49e5f8d72634da638420b9ea492ce8305e8/typing_extensions-4.4.0-py3-none-any.whl", hash = "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"},
-    {url = "https://files.pythonhosted.org/packages/e3/a7/8f4e456ef0adac43f452efc2d0e4b242ab831297f1bac60ac815d37eb9cf/typing_extensions-4.4.0.tar.gz", hash = "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa"},
+"typing-extensions 4.6.3" = [
+    {url = "https://files.pythonhosted.org/packages/42/56/cfaa7a5281734dadc842f3a22e50447c675a1c5a5b9f6ad8a07b467bffe7/typing_extensions-4.6.3.tar.gz", hash = "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"},
+    {url = "https://files.pythonhosted.org/packages/5f/86/d9b1518d8e75b346a33eb59fa31bdbbee11459a7e2cc5be502fa779e96c5/typing_extensions-4.6.3-py3-none-any.whl", hash = "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26"},
 ]
 "wcwidth 0.2.6" = [
     {url = "https://files.pythonhosted.org/packages/20/f4/c0584a25144ce20bfcf1aecd041768b8c762c1eb0aa77502a3f0baa83f11/wcwidth-0.2.6-py2.py3-none-any.whl", hash = "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e"},
     {url = "https://files.pythonhosted.org/packages/5e/5f/1e4bd82a9cc1f17b2c2361a2d876d4c38973a997003ba5eb400e8a932b6c/wcwidth-0.2.6.tar.gz", hash = "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"},
 ]
 "webencodings 0.5.1" = [
     {url = "https://files.pythonhosted.org/packages/0b/02/ae6ceac1baeda530866a85075641cec12989bd8d31af6d5ab4a3e8c92f47/webencodings-0.5.1.tar.gz", hash = "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"},
     {url = "https://files.pythonhosted.org/packages/f4/24/2a3e3df732393fed8b3ebf2ec078f05546de641fe1b667ee316ec1dcf3b7/webencodings-0.5.1-py2.py3-none-any.whl", hash = "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78"},
 ]
-"websocket-client 1.4.2" = [
-    {url = "https://files.pythonhosted.org/packages/75/af/1d13b93e7a21aca7f8ab8645fcfcfad21fc39716dc9dce5dc2a97f73ff78/websocket-client-1.4.2.tar.gz", hash = "sha256:d6e8f90ca8e2dd4e8027c4561adeb9456b54044312dba655e7cae652ceb9ae59"},
-    {url = "https://files.pythonhosted.org/packages/78/d5/2b5719b738791cd798e8f097eba4bb093ff5efca5cef2f3d37a72daa111f/websocket_client-1.4.2-py3-none-any.whl", hash = "sha256:d6b06432f184438d99ac1f456eaf22fe1ade524c3dd16e661142dc54e9cba574"},
-]
-"websockets 10.4" = [
-    {url = "https://files.pythonhosted.org/packages/00/15/611ddaca66937f77aa5021e97c9bec61e6a30668b75db3707713b69b3b88/websockets-10.4-pp37-pypy37_pp73-macosx_10_9_x86_64.whl", hash = "sha256:82ff5e1cae4e855147fd57a2863376ed7454134c2bf49ec604dfe71e446e2193"},
-    {url = "https://files.pythonhosted.org/packages/03/e2/7784912651a299a5e060656e6368946ae4c1da63f01236f7d650e8070cf8/websockets-10.4-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:b343f521b047493dc4022dd338fc6db9d9282658862756b4f6fd0e996c1380e1"},
-    {url = "https://files.pythonhosted.org/packages/09/35/2b8ed52dc995507476ebbb7a91a0c5ed80fd80fa0a840f422ac25c722dbf/websockets-10.4-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:e23173580d740bf8822fd0379e4bf30aa1d5a92a4f252d34e893070c081050df"},
-    {url = "https://files.pythonhosted.org/packages/0c/56/b2d373ed19b4e7b6c5c7630d598ba10473fa6131e67e69590214ab18bc09/websockets-10.4-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:e0cb5cc6ece6ffa75baccfd5c02cffe776f3f5c8bf486811f9d3ea3453676ce8"},
-    {url = "https://files.pythonhosted.org/packages/0c/f0/195097822f8edc4ffa355f6463a1890928577517382c0baededc760f9397/websockets-10.4-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:fe10ddc59b304cb19a1bdf5bd0a7719cbbc9fbdd57ac80ed436b709fcf889106"},
-    {url = "https://files.pythonhosted.org/packages/14/88/81c08fb3418c5aedf3776333f29443599729509a4f673d6598dd769d3d6b/websockets-10.4-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:d58804e996d7d2307173d56c297cf7bc132c52df27a3efaac5e8d43e36c21c48"},
-    {url = "https://files.pythonhosted.org/packages/17/e4/3bdc2ea97d7da70d9f184051dcd40f27c849ded517ea9bab70df677a6b23/websockets-10.4-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:5c1289596042fad2cdceb05e1ebf7aadf9995c928e0da2b7a4e99494953b1b94"},
-    {url = "https://files.pythonhosted.org/packages/19/a3/02ce75ffca3ef147cc0f44647c67acb3171b5a09910b5b9f083b5ca395a6/websockets-10.4-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:90fcf8929836d4a0e964d799a58823547df5a5e9afa83081761630553be731f9"},
-    {url = "https://files.pythonhosted.org/packages/1c/4b/cab8fed34c3a29d4594ff77234f6e6b45feb35331f1c12fccf92ca5486dd/websockets-10.4-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:62e627f6b6d4aed919a2052efc408da7a545c606268d5ab5bfab4432734b82b4"},
-    {url = "https://files.pythonhosted.org/packages/1d/06/5ecd0434cf35f92ca9ce80e38a3ac9bf5422ace9488693c3900e2f1c7fa0/websockets-10.4-cp37-cp37m-win32.whl", hash = "sha256:8a5cc00546e0a701da4639aa0bbcb0ae2bb678c87f46da01ac2d789e1f2d2038"},
-    {url = "https://files.pythonhosted.org/packages/1e/76/163a18626001465a309bf74b6aeb301d7092e304637fe00f89d7efc75c44/websockets-10.4-cp310-cp310-win_amd64.whl", hash = "sha256:8dc96f64ae43dde92530775e9cb169979f414dcf5cff670455d81a6823b42089"},
-    {url = "https://files.pythonhosted.org/packages/20/7a/bd0ce7ac1cfafc76c84d6e8051bcbd0f7def8e45207230833bd6ff77a41d/websockets-10.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:ba089c499e1f4155d2a3c2a05d2878a3428cf321c848f2b5a45ce55f0d7d310c"},
-    {url = "https://files.pythonhosted.org/packages/25/a7/4e32f8edfc26339d8d170fe539e0b83a329c42d974dacfe07a0566390aef/websockets-10.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:33d69ca7612f0ddff3316b0c7b33ca180d464ecac2d115805c044bf0a3b0d032"},
-    {url = "https://files.pythonhosted.org/packages/27/bb/6327e8c7d4dd7d5b450b409a461be278968ce05c54da13da581ac87661db/websockets-10.4-cp311-cp311-win_amd64.whl", hash = "sha256:a7a240d7a74bf8d5cb3bfe6be7f21697a28ec4b1a437607bae08ac7acf5b4882"},
-    {url = "https://files.pythonhosted.org/packages/29/33/dd88aefeabc9dddb4f48c9e15c6c2554dfb6b4cf8d8f1b4de4d12ba997de/websockets-10.4-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:0cff816f51fb33c26d6e2b16b5c7d48eaa31dae5488ace6aae468b361f422b63"},
-    {url = "https://files.pythonhosted.org/packages/2b/cb/d394efe7b0ee6cdeffac28a1cb054e42f9f95974885ca3bcd6fceb0acde1/websockets-10.4-pp38-pypy38_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ff64a1d38d156d429404aaa84b27305e957fd10c30e5880d1765c9480bea490f"},
-    {url = "https://files.pythonhosted.org/packages/2e/dd/521f0574bed6d08ce5e0acd5893ae418c0a81ef55eb4c960aedac9cbd929/websockets-10.4-pp39-pypy39_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b627c266f295de9dea86bd1112ed3d5fafb69a348af30a2422e16590a8ecba13"},
-    {url = "https://files.pythonhosted.org/packages/33/3a/72c9d733d676447da2c89a35c694f779a9a360cff51ee0f90bb562d80cd4/websockets-10.4-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:7d27a7e34c313b3a7f91adcd05134315002aaf8540d7b4f90336beafaea6217c"},
-    {url = "https://files.pythonhosted.org/packages/36/8f/6dd75723ea67d54dec3a597ad781642c0febe8d51f233b95347981c0e549/websockets-10.4-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:9bc42e8402dc5e9905fb8b9649f57efcb2056693b7e88faa8fb029256ba9c68c"},
-    {url = "https://files.pythonhosted.org/packages/37/02/ef21ca4698c2fd950250e5ac397fd07b0c9f16bbd073d0ea64c25baef9c1/websockets-10.4-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:7c584f366f46ba667cfa66020344886cf47088e79c9b9d39c84ce9ea98aaa331"},
-    {url = "https://files.pythonhosted.org/packages/3e/a5/e4535867a96bb07000c54172e1be82cd0b3a95339244cac1d400f8ba9b64/websockets-10.4-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:185929b4808b36a79c65b7865783b87b6841e852ef5407a2fb0c03381092fa3b"},
-    {url = "https://files.pythonhosted.org/packages/47/4d/f2e28f112302d3bc794b74ae64656255161d8223f4d47bd17d40cbb3629e/websockets-10.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:56029457f219ade1f2fc12a6504ea61e14ee227a815531f9738e41203a429112"},
-    {url = "https://files.pythonhosted.org/packages/47/58/69435f1479acb56b3678905b5f2be57908a201c28465d4368d91f52cad76/websockets-10.4-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:dd9becd5fe29773d140d68d607d66a38f60e31b86df75332703757ee645b6faf"},
-    {url = "https://files.pythonhosted.org/packages/4a/39/3b6b64f775f1f4f5de6eb909d72f3f794f453730b5b3176fa5021ff334ba/websockets-10.4-pp37-pypy37_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c9b27d6c1c6cd53dc93614967e9ce00ae7f864a2d9f99fe5ed86706e1ecbf485"},
-    {url = "https://files.pythonhosted.org/packages/4d/6f/2388f9304cdaa0215b6388f837c6dbfe6d63ac1bba8c196e3b14eea1831e/websockets-10.4-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:38ea7b82bfcae927eeffc55d2ffa31665dc7fec7b8dc654506b8e5a518eb4d50"},
-    {url = "https://files.pythonhosted.org/packages/4e/8b/854b3625cc5130e4af8a10a7502c2f6c16d1bd107ff009394127a2f8abb3/websockets-10.4-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:40e826de3085721dabc7cf9bfd41682dadc02286d8cf149b3ad05bff89311e4f"},
-    {url = "https://files.pythonhosted.org/packages/57/d7/df17197565e8874f0a77f8211304169ad4f39ffa3e8c008a7b0bf187a238/websockets-10.4-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:f5fc088b7a32f244c519a048c170f14cf2251b849ef0e20cbbb0fdf0fdaf556f"},
-    {url = "https://files.pythonhosted.org/packages/5a/87/dea889793d2d0958be254fc86dac528d97de9354d16fcdbcbad259750014/websockets-10.4-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:00213676a2e46b6ebf6045bc11d0f529d9120baa6f58d122b4021ad92adabd41"},
-    {url = "https://files.pythonhosted.org/packages/5d/3c/fc1725524e48f624df77f5998b1c7070fdddec3ae67a2ffbc99ffd116269/websockets-10.4-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f55b5905705725af31ccef50e55391621532cd64fbf0bc6f4bac935f0fccec46"},
-    {url = "https://files.pythonhosted.org/packages/60/3a/6dccbe2725d13c398b90cbebeea684cda7792e6d874f96417db900556ad0/websockets-10.4-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:47a2964021f2110116cc1125b3e6d87ab5ad16dea161949e7244ec583b905bb4"},
-    {url = "https://files.pythonhosted.org/packages/62/76/c2411e634979cc6e812ef2a96aa295545cfcbc9566b298db09f3f4639d62/websockets-10.4-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:edc344de4dac1d89300a053ac973299e82d3db56330f3494905643bb68801269"},
-    {url = "https://files.pythonhosted.org/packages/63/f2/ec4c59b4f91936eb2a5ddcf2f7e57184acbce5122d5d83911c5a47f25144/websockets-10.4-cp38-cp38-win_amd64.whl", hash = "sha256:48c08473563323f9c9debac781ecf66f94ad5a3680a38fe84dee5388cf5acaf6"},
-    {url = "https://files.pythonhosted.org/packages/68/bd/c8bd8354fc629863a2db39c9182d40297f47dfb2ed3e178bc83041ce044b/websockets-10.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:bc0b82d728fe21a0d03e65f81980abbbcb13b5387f733a1a870672c5be26edab"},
-    {url = "https://files.pythonhosted.org/packages/68/ec/3267f8bbe8a4a5e181ab3fc67cc137f0966ab9e9a4da14ffc603f320b9e6/websockets-10.4-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:00c870522cdb69cd625b93f002961ffb0c095394f06ba8c48f17eef7c1541f96"},
-    {url = "https://files.pythonhosted.org/packages/71/93/5a4f408177e43d84274e1c08cbea3e50ad80db654dc25a0bba79dbdc00b4/websockets-10.4-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4f72e5cd0f18f262f5da20efa9e241699e0cf3a766317a17392550c9ad7b37d8"},
-    {url = "https://files.pythonhosted.org/packages/75/18/155c3582fd69b60d9c490fb0e64e37269c55d5873cbcb37f83e2d3feb078/websockets-10.4-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:389f8dbb5c489e305fb113ca1b6bdcdaa130923f77485db5b189de343a179393"},
-    {url = "https://files.pythonhosted.org/packages/77/65/d7c73e62cf19f068850ddab548837329dab9c023567f5834747f61cdc747/websockets-10.4-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:45ec8e75b7dbc9539cbfafa570742fe4f676eb8b0d3694b67dabe2f2ceed8aa6"},
-    {url = "https://files.pythonhosted.org/packages/85/dc/549a807a53c13fd4a8dac286f117a7a71260defea9ec0c05d6027f2ae273/websockets-10.4.tar.gz", hash = "sha256:eef610b23933c54d5d921c92578ae5f89813438fded840c2e9809d378dc765d3"},
-    {url = "https://files.pythonhosted.org/packages/86/8e/390e0e3db702c55d31ca3999c622bb3b8b480c306c1bdee6a2da44b13b1b/websockets-10.4-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:84bc2a7d075f32f6ed98652db3a680a17a4edb21ca7f80fe42e38753a58ee02b"},
-    {url = "https://files.pythonhosted.org/packages/88/00/9776e2626a30e3455a830665e50cf40f5d34a4134272b3138a637afa38a7/websockets-10.4-cp39-cp39-win_amd64.whl", hash = "sha256:bbccd847aa0c3a69b5f691a84d2341a4f8a629c6922558f2a70611305f902d74"},
-    {url = "https://files.pythonhosted.org/packages/88/97/d70e2d528b9ffe759134e5db6b1424b61cd61fd1c4471b178c76e01f41af/websockets-10.4-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:74de2b894b47f1d21cbd0b37a5e2b2392ad95d17ae983e64727e18eb281fe7cb"},
-    {url = "https://files.pythonhosted.org/packages/8a/1e/8f34d7ee924dc7a624c1e14f43209484cb5eccb58e892285d45551729a95/websockets-10.4-cp39-cp39-win32.whl", hash = "sha256:c94ae4faf2d09f7c81847c63843f84fe47bf6253c9d60b20f25edfd30fb12588"},
-    {url = "https://files.pythonhosted.org/packages/90/e1/22e43e9a1fbc9ddf4a0317b231e2e28eddfbe8804b7ca4a9f7fba7033b17/websockets-10.4-pp37-pypy37_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:942de28af58f352a6f588bc72490ae0f4ccd6dfc2bd3de5945b882a078e4e179"},
-    {url = "https://files.pythonhosted.org/packages/93/7b/72134e4c75002e311c072f0665fe45f7321d614c5c65181888faddd616e9/websockets-10.4-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2fc8709c00704194213d45e455adc106ff9e87658297f72d544220e32029cd3d"},
-    {url = "https://files.pythonhosted.org/packages/a0/92/aa8d1ba3a7e3e6cf6d5d1c929530a40138667ea60454bf5c0fff3b93cae2/websockets-10.4-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c57e4c1349fbe0e446c9fa7b19ed2f8a4417233b6984277cce392819123142d3"},
-    {url = "https://files.pythonhosted.org/packages/a1/6f/60e5f6e114b6077683d74da5df0d4af647a9e6d2a18b4698f577b2cb7c14/websockets-10.4-cp310-cp310-win32.whl", hash = "sha256:b029fb2032ae4724d8ae8d4f6b363f2cc39e4c7b12454df8df7f0f563ed3e61a"},
-    {url = "https://files.pythonhosted.org/packages/a1/f6/83da14582fbb0496c47a4c039bd6e802886a0c300e9795c0f839fd1498e3/websockets-10.4-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:ae5e95cfb53ab1da62185e23b3130e11d64431179debac6dc3c6acf08760e9b1"},
-    {url = "https://files.pythonhosted.org/packages/ab/41/ed2fecb228c1f25cea03fce4a22a86f7771a10875d5762e777e943bb7d68/websockets-10.4-cp37-cp37m-win_amd64.whl", hash = "sha256:a9f9a735deaf9a0cadc2d8c50d1a5bcdbae8b6e539c6e08237bc4082d7c13f28"},
-    {url = "https://files.pythonhosted.org/packages/b0/fc/a818cddc63589e12d5eff9b51a59aad82e2adf35279493248a3742c41f85/websockets-10.4-cp311-cp311-win32.whl", hash = "sha256:b9968694c5f467bf67ef97ae7ad4d56d14be2751000c1207d31bf3bb8860bae8"},
-    {url = "https://files.pythonhosted.org/packages/b1/8f/dbffb63e7da0ada24e9ef8802c439169e0ed9a7ef8f6049874e6cbfc7919/websockets-10.4-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b0d15c968ea7a65211e084f523151dbf8ae44634de03c801b8bd070b74e85033"},
-    {url = "https://files.pythonhosted.org/packages/b4/91/c460f5164af303b31f58362935f7b8ed1750e3b8fbcb900da4b0661532a8/websockets-10.4-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:931c039af54fc195fe6ad536fde4b0de04da9d5916e78e55405436348cfb0e56"},
-    {url = "https://files.pythonhosted.org/packages/bb/5c/7dc1f604688f43168ef17313055e048c755a29afde821f7e0b19bd3a180f/websockets-10.4-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d6a4162139374a49eb18ef5b2f4da1dd95c994588f5033d64e0bbfda4b6b6fcf"},
-    {url = "https://files.pythonhosted.org/packages/c5/01/145d2883dfeffedf541a7c95bb26f8d8b5ddca84a7c8f671ec3b878ae7cd/websockets-10.4-pp38-pypy38_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:09a1814bb15eff7069e51fed0826df0bc0702652b5cb8f87697d469d79c23576"},
-    {url = "https://files.pythonhosted.org/packages/c6/41/07f39745017af5381aeb6c1d8c6509aa1861193c948648d4aaf4d0637915/websockets-10.4-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:3d3cac3e32b2c8414f4f87c1b2ab686fa6284a980ba283617404377cd448f631"},
-    {url = "https://files.pythonhosted.org/packages/cc/19/2f003f9f81c0fab2eabb81d8fc2fce5fb5b5714f1b4abfe897cb209e031d/websockets-10.4-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:7d3f0b61c45c3fa9a349cf484962c559a8a1d80dae6977276df8fd1fa5e3cb8c"},
-    {url = "https://files.pythonhosted.org/packages/d1/60/0a6cb94e25b981e428c1cdcc2b0a406ac6e1dfc78d8a81c8a4ee7510e853/websockets-10.4-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:e789376b52c295c4946403bd0efecf27ab98f05319df4583d3c48e43c7342c2f"},
-    {url = "https://files.pythonhosted.org/packages/d1/c6/9489869aa591e6a8941b0af2302f8383e199e90477559a510713d41bfa45/websockets-10.4-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:f2c38d588887a609191d30e902df2a32711f708abfd85d318ca9b367258cfd0c"},
-    {url = "https://files.pythonhosted.org/packages/d4/1a/2e4afd95abd33bd6ad77042270f8eee3697e07cdd749c068bff08bba2022/websockets-10.4-pp37-pypy37_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d210abe51b5da0ffdbf7b43eed0cfdff8a55a1ab17abbec4301c9ff077dd0342"},
-    {url = "https://files.pythonhosted.org/packages/d5/5d/d0b039f0db0bb1fea93437721cf3cd8a244ad02a86960c38a3853d5e1fab/websockets-10.4-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8f38706e0b15d3c20ef6259fd4bc1700cd133b06c3c1bb108ffe3f8947be15fa"},
-    {url = "https://files.pythonhosted.org/packages/d6/7c/79ea4e7f56dfe7f703213000bbbd29b70cef2666698d98b66ce1af43caee/websockets-10.4-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0154f7691e4fe6c2b2bc275b5701e8b158dae92a1ab229e2b940efe11905dff4"},
-    {url = "https://files.pythonhosted.org/packages/d7/f9/f64ec37da654351b212e5534b0e31703ed80d2a6acb6b8c1b1373fafa876/websockets-10.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4c6d2264f485f0b53adf22697ac11e261ce84805c232ed5dbe6b1bcb84b00ff0"},
-    {url = "https://files.pythonhosted.org/packages/da/0b/a501ed176c69b51ca83f4186bad80bba9b59ab354fd8954d7d36cb2ec47f/websockets-10.4-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e3a686ecb4aa0d64ae60c9c9f1a7d5d46cab9bfb5d91a2d303d00e2cd4c4c5cc"},
-    {url = "https://files.pythonhosted.org/packages/e0/8d/7bffabd3f10a88cd68080669b33f407471283becf7e5cb4f0143b117211d/websockets-10.4-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:932af322458da7e4e35df32f050389e13d3d96b09d274b22a7aa1808f292fee4"},
-    {url = "https://files.pythonhosted.org/packages/e6/94/cb97e5a9d019e473a37317a740852850ef09e14c02621dd86a898ec90f7a/websockets-10.4-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:884be66c76a444c59f801ac13f40c76f176f1bfa815ef5b8ed44321e74f1600b"},
-    {url = "https://files.pythonhosted.org/packages/e9/48/a0751eafbeab06866fc70a66f7dfa08422cb96113af9138e526e7b106f14/websockets-10.4-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:dd500e0a5e11969cdd3320935ca2ff1e936f2358f9c2e61f100a1660933320ea"},
-    {url = "https://files.pythonhosted.org/packages/ec/ba/74b4b92cc41ffc4cfa791fb9f8e8ab7c4d9bf84e54a5bef12ab23eb54880/websockets-10.4-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:da39dd03d130162deb63da51f6e66ed73032ae62e74aaccc4236e30edccddbb0"},
-    {url = "https://files.pythonhosted.org/packages/f8/f0/437187175182beed10246f53ef9793a5f6e087ce71ee25b64fdb12e396e0/websockets-10.4-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:4239b6027e3d66a89446908ff3027d2737afc1a375f8fd3eea630a4842ec9a0c"},
-    {url = "https://files.pythonhosted.org/packages/f9/15/ab0e9155700d3037ffe4a146a719f3e68ee025c9d45d6a39b027e928db52/websockets-10.4-cp38-cp38-win32.whl", hash = "sha256:db3c336f9eda2532ec0fd8ea49fef7a8df8f6c804cdf4f39e5c5c0d4a4ad9a7a"},
-    {url = "https://files.pythonhosted.org/packages/fd/42/07f31d9f9e142b38cde8d3ea0c8ea1bacf9bc366f2f573eca57086e9f2a6/websockets-10.4-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:05a7233089f8bd355e8cbe127c2e8ca0b4ea55467861906b80d2ebc7db4d6b72"},
-]
-"werkzeug 2.2.2" = [
-    {url = "https://files.pythonhosted.org/packages/c8/27/be6ddbcf60115305205de79c29004a0c6bc53cec814f733467b1bb89386d/Werkzeug-2.2.2-py3-none-any.whl", hash = "sha256:f979ab81f58d7318e064e99c4506445d60135ac5cd2e177a2de0089bfd4c9bd5"},
-    {url = "https://files.pythonhosted.org/packages/f8/c1/1c8e539f040acd80f844c69a5ef8e2fccdf8b442dabb969e497b55d544e1/Werkzeug-2.2.2.tar.gz", hash = "sha256:7ea2d48322cc7c0f8b3a215ed73eabd7b5d75d0b50e31ab006286ccff9e00b8f"},
-]
-"widgetsnbextension 4.0.5" = [
-    {url = "https://files.pythonhosted.org/packages/46/d0/ef509e5b74d96821b4ec170b7785449e25a89ef0e781e80562e515f84678/widgetsnbextension-4.0.5.tar.gz", hash = "sha256:003f716d930d385be3fd9de42dd9bf008e30053f73bddde235d14fbeaeff19af"},
-    {url = "https://files.pythonhosted.org/packages/c2/1a/73574f7194184c8670b804171d7f43f56c586e5f8142a41f7a53f0998b6b/widgetsnbextension-4.0.5-py3-none-any.whl", hash = "sha256:eaaaf434fb9b08bd197b2a14ffe45ddb5ac3897593d43c69287091e5f3147bf7"},
+"websocket-client 1.5.2" = [
+    {url = "https://files.pythonhosted.org/packages/3f/f2/2624e12ef854ee667d92ac5dc7815932095e0852e5ff2b2bf57feda8a11b/websocket-client-1.5.2.tar.gz", hash = "sha256:c7d67c13b928645f259d9b847ab5b57fd2d127213ca41ebd880de1f553b7c23b"},
+    {url = "https://files.pythonhosted.org/packages/86/5c/2ebfbb7d4dbb7f35a1f70c40d003f7844d78945ac7c69757067ebaea9c78/websocket_client-1.5.2-py3-none-any.whl", hash = "sha256:f8c64e28cd700e7ba1f04350d66422b6833b82a796b525a51e740b8cc8dab4b1"},
+]
+"websockets 11.0.3" = [
+    {url = "https://files.pythonhosted.org/packages/03/28/3a51ffcf51ac45746639f83128908bbb1cd212aa631e42d15a7acebce5cb/websockets-11.0.3-pp37-pypy37_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e052b8467dd07d4943936009f46ae5ce7b908ddcac3fda581656b1b19c083d9b"},
+    {url = "https://files.pythonhosted.org/packages/0a/84/68b848a373493b58615d6c10e9e8ccbaadfd540f84905421739a807704f8/websockets-11.0.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aa5003845cdd21ac0dc6c9bf661c5beddd01116f6eb9eb3c8e272353d45b3288"},
+    {url = "https://files.pythonhosted.org/packages/0f/d8/a997d3546aef9cc995a1126f7d7ade96c0e16c1a0efb9d2d430aee57c925/websockets-11.0.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:619d9f06372b3a42bc29d0cd0354c9bb9fb39c2cbc1a9c5025b4538738dbffaf"},
+    {url = "https://files.pythonhosted.org/packages/14/fc/5cbbf439c925e1e184a0392ec477a30cee2fabc0e63807c1d4b6d570fb52/websockets-11.0.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:b30c6590146e53149f04e85a6e4fcae068df4289e31e4aee1fdf56a0dead8f97"},
+    {url = "https://files.pythonhosted.org/packages/16/49/ae616bd221efba84a3d78737b417f704af1ffa36f40dcaba5eb954dd4753/websockets-11.0.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:e848f46a58b9fcf3d06061d17be388caf70ea5b8cc3466251963c8345e13f7eb"},
+    {url = "https://files.pythonhosted.org/packages/19/d3/2ea3f95d83033675144b0848a0ae2e4998b3f763da09ec3df6bce97ea4e6/websockets-11.0.3-cp37-cp37m-win32.whl", hash = "sha256:e590228200fcfc7e9109509e4d9125eace2042fd52b595dd22bbc34bb282307f"},
+    {url = "https://files.pythonhosted.org/packages/1b/3d/3dc77699fa4d003f2e810c321592f80f62b81d7b78483509de72ffe581fd/websockets-11.0.3-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:0ee68fe502f9031f19d495dae2c268830df2760c0524cbac5d759921ba8c8e82"},
+    {url = "https://files.pythonhosted.org/packages/20/62/5c6039c4069912adb27889ddd000403a2de9e0fe6aebe439b4e6b128a6b8/websockets-11.0.3-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:e6316827e3e79b7b8e7d8e3b08f4e331af91a48e794d5d8b099928b6f0b85f20"},
+    {url = "https://files.pythonhosted.org/packages/25/25/48540419005d07ed2d368a7eafb44ed4f33a2691ae4c210850bf31123c4a/websockets-11.0.3-cp38-cp38-win_amd64.whl", hash = "sha256:03aae4edc0b1c68498f41a6772d80ac7c1e33c06c6ffa2ac1c27a07653e79d6f"},
+    {url = "https://files.pythonhosted.org/packages/27/e9/605b0618d0864e9be7c2a78f22bff57aba9cf56b9fccde3205db9023ae22/websockets-11.0.3-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:92b2065d642bf8c0a82d59e59053dd2fdde64d4ed44efe4870fa816c1232647b"},
+    {url = "https://files.pythonhosted.org/packages/30/a5/d641f2a9a4b4079cfddbb0726fc1b914be76a610aaedb45e4760899a4ce1/websockets-11.0.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:bee9fcb41db2a23bed96c6b6ead6489702c12334ea20a297aa095ce6d31370d0"},
+    {url = "https://files.pythonhosted.org/packages/32/2c/ab8ea64e9a7d8bf62a7ea7a037fb8d328d8bd46dbfe083787a9d452a148e/websockets-11.0.3-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b67c6f5e5a401fc56394f191f00f9b3811fe843ee93f4a70df3c389d1adf857d"},
+    {url = "https://files.pythonhosted.org/packages/36/19/0da435afb26a6c47c0c045a82e414912aa2ac10de5721276a342bd9fdfee/websockets-11.0.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:332d126167ddddec94597c2365537baf9ff62dfcc9db4266f263d455f2f031cb"},
+    {url = "https://files.pythonhosted.org/packages/38/30/01a10fbf4cc1e7ffa07be9b0401501918fc9433d71fb7da4cfcef3bd26ca/websockets-11.0.3-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8531fdcad636d82c517b26a448dcfe62f720e1922b33c81ce695d0edb91eb931"},
+    {url = "https://files.pythonhosted.org/packages/38/ed/b8b133416536b6816e480594864e5950051db522714623eefc9e5275ec04/websockets-11.0.3-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:6505c1b31274723ccaf5f515c1824a4ad2f0d191cec942666b3d0f3aa4cb4007"},
+    {url = "https://files.pythonhosted.org/packages/44/a8/66c3a66b70b01a6c55fde486298766177fa11dd0d3a2c1cfc6820f25b4dc/websockets-11.0.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2529338a6ff0eb0b50c7be33dc3d0e456381157a31eefc561771ee431134a97f"},
+    {url = "https://files.pythonhosted.org/packages/47/96/9d5749106ff57629b54360664ae7eb9afd8302fad1680ead385383e33746/websockets-11.0.3-py3-none-any.whl", hash = "sha256:6681ba9e7f8f3b19440921e99efbb40fc89f26cd71bf539e45d8c8a25c976dc6"},
+    {url = "https://files.pythonhosted.org/packages/58/05/2efb520317340ece74bfc4d88e8f011dd71a4e6c263000bfffb71a343685/websockets-11.0.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e1a99a7a71631f0efe727c10edfba09ea6bee4166a6f9c19aafb6c0b5917d09c"},
+    {url = "https://files.pythonhosted.org/packages/58/0a/7570e15661a0a546c3a1152d95fe8c05480459bab36247f0acbf41f01a41/websockets-11.0.3-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bceab846bac555aff6427d060f2fcfff71042dba6f5fca7dc4f75cac815e57ca"},
+    {url = "https://files.pythonhosted.org/packages/58/68/9403771de1b1c21a2e878e4841815af8c9f8893b094654934e2a5ee4dbc8/websockets-11.0.3-cp38-cp38-win32.whl", hash = "sha256:f61bdb1df43dc9c131791fbc2355535f9024b9a04398d3bd0684fc16ab07df74"},
+    {url = "https://files.pythonhosted.org/packages/66/89/799f595c67b97a8a17e13d2764e088f631616bd95668aaa4c04b7cada136/websockets-11.0.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:df41b9bc27c2c25b486bae7cf42fccdc52ff181c8c387bfd026624a491c2671b"},
+    {url = "https://files.pythonhosted.org/packages/6b/ca/65d6986665888494eca4d5435a9741c822022996f0f4200c57ce4b9242f7/websockets-11.0.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:660e2d9068d2bedc0912af508f30bbeb505bbbf9774d98def45f68278cea20d3"},
+    {url = "https://files.pythonhosted.org/packages/70/fc/71377f36ef3049f3bc7db7c0f3a7696929d5f836d7a18777131d994192a9/websockets-11.0.3-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:34fd59a4ac42dff6d4681d8843217137f6bc85ed29722f2f7222bd619d15e95b"},
+    {url = "https://files.pythonhosted.org/packages/72/89/0d150939f2e592ed78c071d69237ac1c872462cc62a750c5f592f3d4ab18/websockets-11.0.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:97b52894d948d2f6ea480171a27122d77af14ced35f62e5c892ca2fae9344311"},
+    {url = "https://files.pythonhosted.org/packages/78/b2/df5452031b02b857851139806308f2af7c749069e25bfe15f2d559ade6e7/websockets-11.0.3-pp37-pypy37_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0ac56b661e60edd453585f4bd68eb6a29ae25b5184fd5ba51e97652580458998"},
+    {url = "https://files.pythonhosted.org/packages/82/3c/00f051abcf88aec5e952a8840076749b0b26a30c219dcae8ba70200998aa/websockets-11.0.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:86d2a77fd490ae3ff6fae1c6ceaecad063d3cc2320b44377efdde79880e11526"},
+    {url = "https://files.pythonhosted.org/packages/89/8f/707a05d5725f956c78d252a5fd73b89fa3ac57dd3959381c2d1acb41cb13/websockets-11.0.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:01f5567d9cf6f502d655151645d4e8b72b453413d3819d2b6f1185abc23e82dd"},
+    {url = "https://files.pythonhosted.org/packages/8a/77/a04d2911f6e2b9e781ce7ffc1e8516b54b85f985369eec8c853fd619d8e8/websockets-11.0.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:69269f3a0b472e91125b503d3c0b3566bda26da0a3261c49f0027eb6075086d1"},
+    {url = "https://files.pythonhosted.org/packages/8a/bd/a5e5973899d78d44a540f50a9e30b01c6771e8bf7883204ee762060cf95a/websockets-11.0.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:4841ed00f1026dfbced6fca7d963c4e7043aa832648671b5138008dc5a8f6d99"},
+    {url = "https://files.pythonhosted.org/packages/8b/97/34178f5f7c29e679372d597cebfeff2aa45991d741d938117d4616e81a74/websockets-11.0.3-pp39-pypy39_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1d5023a4b6a5b183dc838808087033ec5df77580485fc533e7dab2567851b0a4"},
+    {url = "https://files.pythonhosted.org/packages/8c/a8/e81533499f84ef6cdd95d11d5b05fa827c0f097925afd86f16e6a2631d8e/websockets-11.0.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:b58cbf0697721120866820b89f93659abc31c1e876bf20d0b3d03cef14faf84d"},
+    {url = "https://files.pythonhosted.org/packages/8f/7b/4d4ecd29be7d08486e38f987a6603c491296d1e33fe55127d79aebb0333e/websockets-11.0.3-cp310-cp310-win32.whl", hash = "sha256:2d903ad4419f5b472de90cd2d40384573b25da71e33519a67797de17ef849b69"},
+    {url = "https://files.pythonhosted.org/packages/8f/f2/8a3eb016be19743c7eb9e67c855df0fdfa5912534ffaf83a05b62667d761/websockets-11.0.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:8c82f11964f010053e13daafdc7154ce7385ecc538989a354ccc7067fd7028fd"},
+    {url = "https://files.pythonhosted.org/packages/94/8c/266155c14b7a26deca6fa4c4d5fd15b0ab32725d78a2acfcf6b24943585d/websockets-11.0.3-cp37-cp37m-win_amd64.whl", hash = "sha256:b16fff62b45eccb9c7abb18e60e7e446998093cdcb50fed33134b9b6878836de"},
+    {url = "https://files.pythonhosted.org/packages/98/a7/0ed69892981351e5acf88fac0ff4c801fabca2c3bdef9fca4c7d3fde8c53/websockets-11.0.3-cp310-cp310-win_amd64.whl", hash = "sha256:1d2256283fa4b7f4c7d7d3e84dc2ece74d341bce57d5b9bf385df109c2a1a82f"},
+    {url = "https://files.pythonhosted.org/packages/99/23/43071c989c0f87f612e7bccee98d00b04bddd3aca0cdc1ffaf31f6f8a4b4/websockets-11.0.3-pp38-pypy38_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c114e8da9b475739dde229fd3bc6b05a6537a88a578358bc8eb29b4030fac9c9"},
+    {url = "https://files.pythonhosted.org/packages/9a/6e/0fd7274042f46acb589161407f4b505b44c68d369437ce919bae1fa9b8c4/websockets-11.0.3-cp39-cp39-win32.whl", hash = "sha256:c7f3cb904cce8e1be667c7e6fef4516b98d1a6a0635a58a57528d577ac18a128"},
+    {url = "https://files.pythonhosted.org/packages/a0/1a/3da73e69ebc00649d11ed836541c92c1a2df0b8a8aa641a2c8746e7c2b9c/websockets-11.0.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3580dd9c1ad0701169e4d6fc41e878ffe05e6bdcaf3c412f9d559389d0c9e016"},
+    {url = "https://files.pythonhosted.org/packages/a0/39/acc3d4b15c5207ef7cca823c37eca8c74e3e1a1a63a397798986be3bdef7/websockets-11.0.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:68b977f21ce443d6d378dbd5ca38621755f2063d6fdb3335bda981d552cfff86"},
+    {url = "https://files.pythonhosted.org/packages/a6/1b/5c83c40f8d3efaf0bb2fdf05af94fb920f74842b7aaf31d7598e3ee44d58/websockets-11.0.3-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:dcacf2c7a6c3a84e720d1bb2b543c675bf6c40e460300b628bab1b1efc7c034c"},
+    {url = "https://files.pythonhosted.org/packages/a6/9c/2356ecb952fd3992b73f7a897d65e57d784a69b94bb8d8fd5f97531e5c02/websockets-11.0.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:279e5de4671e79a9ac877427f4ac4ce93751b8823f276b681d04b2156713b9dd"},
+    {url = "https://files.pythonhosted.org/packages/a7/8c/7100e9cf310fe1d83d1ae1322203f4eb2b767a7c2b301c1e70db6270306f/websockets-11.0.3-pp37-pypy37_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:de36fe9c02995c7e6ae6efe2e205816f5f00c22fd1fbf343d4d18c3d5ceac2f5"},
+    {url = "https://files.pythonhosted.org/packages/a7/f7/1e852351e8073c32885172a6bef64c95d14c13ff3634b01d4a1086321491/websockets-11.0.3-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:9d9acd80072abcc98bd2c86c3c9cd4ac2347b5a5a0cae7ed5c0ee5675f86d9af"},
+    {url = "https://files.pythonhosted.org/packages/a9/5e/b25c60067d700e811dccb4e3c318eeadd3a19d8b3620de9f97434af777a7/websockets-11.0.3-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:def07915168ac8f7853812cc593c71185a16216e9e4fa886358a17ed0fd9fcf6"},
+    {url = "https://files.pythonhosted.org/packages/b2/ec/56bdd12d847e4fc2d0a7ba2d7f1476f79cda50599d11ffb6080b86f21ef1/websockets-11.0.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ffd7dcaf744f25f82190856bc26ed81721508fc5cbf2a330751e135ff1283564"},
+    {url = "https://files.pythonhosted.org/packages/b5/94/ac47552208583d5dbcce468430c1eb2ae18962f6b3a694a2b7727cc60d4a/websockets-11.0.3-cp311-cp311-win32.whl", hash = "sha256:e1459677e5d12be8bbc7584c35b992eea142911a6236a3278b9b5ce3326f282c"},
+    {url = "https://files.pythonhosted.org/packages/b5/a8/8900184ab0b06b6e620ba7e92cf2faa5caa9ba86e148541b8fff1c7b6646/websockets-11.0.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:9f59a3c656fef341a99e3d63189852be7084c0e54b75734cde571182c087b152"},
+    {url = "https://files.pythonhosted.org/packages/b6/96/0d586c25d043aeab9457dad8e407251e3baf314d871215f91847e7b995c4/websockets-11.0.3-pp38-pypy38_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e063b1865974611313a3849d43f2c3f5368093691349cf3c7c8f8f75ad7cb280"},
+    {url = "https://files.pythonhosted.org/packages/b9/6b/26b28115b46e23e74ede76d95792eedfe8c58b21f4daabfff1e9f159c8fe/websockets-11.0.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d67ac60a307f760c6e65dad586f556dde58e683fab03323221a4e530ead6f74d"},
+    {url = "https://files.pythonhosted.org/packages/ba/6c/5c0322b2875e8395e6bf0eff11f43f3e25da7ef5b12f4d908cd3a19ea841/websockets-11.0.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:54c6e5b3d3a8936a4ab6870d46bdd6ec500ad62bde9e44462c32d18f1e9a8e54"},
+    {url = "https://files.pythonhosted.org/packages/c0/21/cb9dfbbea8dc0ad89ced52630e7e61edb425fb9fdc6002f8d0c5dd26b94b/websockets-11.0.3-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:777354ee16f02f643a4c7f2b3eff8027a33c9861edc691a2003531f5da4f6bc8"},
+    {url = "https://files.pythonhosted.org/packages/c0/a8/a8a582ebeeecc8b5f332997d44c57e241748f8a9856e06a38a5a13b30796/websockets-11.0.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c1f0524f203e3bd35149f12157438f406eff2e4fb30f71221c8a5eceb3617b6b"},
+    {url = "https://files.pythonhosted.org/packages/c4/5b/60eccd7e9703bbe93fc4167d1e7ada7e8e8e51544122198d63fd8e3460b7/websockets-11.0.3-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:fb06eea71a00a7af0ae6aefbb932fb8a7df3cb390cc217d51a9ad7343de1b8d0"},
+    {url = "https://files.pythonhosted.org/packages/c4/f5/15998b164c183af0513bba744b51ecb08d396ff86c0db3b55d62624d1f15/websockets-11.0.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:1fdf26fa8a6a592f8f9235285b8affa72748dc12e964a5518c6c5e8f916716f7"},
+    {url = "https://files.pythonhosted.org/packages/c6/91/f36454b87edf10a95be9c7212d2dcb8c606ddbf7a183afdc498933acdd19/websockets-11.0.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:1553cb82942b2a74dd9b15a018dce645d4e68674de2ca31ff13ebc2d9f283788"},
+    {url = "https://files.pythonhosted.org/packages/c9/fb/ae5ed4be3514287cf8f6c348c87e1392a6e3f4d6eadae75c18847a2f84b6/websockets-11.0.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7622a89d696fc87af8e8d280d9b421db5133ef5b29d3f7a1ce9f1a7bf7fcfa11"},
+    {url = "https://files.pythonhosted.org/packages/ca/20/25211be61d50189650fb0ec6084b6d6339f5c7c6436a6c217608dcb553e4/websockets-11.0.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:4b253869ea05a5a073ebfdcb5cb3b0266a57c3764cf6fe114e4cd90f4bfa5f5e"},
+    {url = "https://files.pythonhosted.org/packages/d1/ec/7e2b9bebc2e9b4a48404144106bbc6a7ace781feeb0e6a3829551e725fa5/websockets-11.0.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:8a34e13a62a59c871064dfd8ffb150867e54291e46d4a7cf11d02c94a5275bae"},
+    {url = "https://files.pythonhosted.org/packages/d8/3b/2ed38e52eed4cf277f9df5f0463a99199a04d9e29c9e227cfafa57bd3993/websockets-11.0.3.tar.gz", hash = "sha256:88fc51d9a26b10fc331be344f1781224a375b78488fc343620184e95a4b27016"},
+    {url = "https://files.pythonhosted.org/packages/d9/36/5741e62ccf629c8e38cc20f930491f8a33ce7dba972cae93dba3d6f02552/websockets-11.0.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6f1a3f10f836fab6ca6efa97bb952300b20ae56b409414ca85bff2ad241d2a61"},
+    {url = "https://files.pythonhosted.org/packages/de/0e/d7274e4d41d7b34f204744c27a23707be2ecefaf6f7df2145655f086ecd7/websockets-11.0.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:41f696ba95cd92dc047e46b41b26dd24518384749ed0d99bea0a941ca87404c4"},
+    {url = "https://files.pythonhosted.org/packages/e1/76/88640f8aeac7eb0d058b913e7bb72682f8d569db44c7d30e576ec4777ce1/websockets-11.0.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:3ccc8a0c387629aec40f2fc9fdcb4b9d5431954f934da3eaf16cdc94f67dbfac"},
+    {url = "https://files.pythonhosted.org/packages/e1/7c/0ad6e7ef0a054d73092f616d20d3d9bd3e1b837554cb20a52d8dd9f5b049/websockets-11.0.3-cp311-cp311-win_amd64.whl", hash = "sha256:e7837cb169eca3b3ae94cc5787c4fed99eef74c0ab9506756eea335e0d6f3ed8"},
+    {url = "https://files.pythonhosted.org/packages/e2/2f/3ad8ac4a9dc9d685e098e534180a36ed68fe2e85e82e225e00daec86bb94/websockets-11.0.3-pp37-pypy37_pp73-macosx_10_9_x86_64.whl", hash = "sha256:f2e58f2c36cc52d41f2659e4c0cbf7353e28c8c9e63e30d8c6d3494dc9fdedcf"},
+    {url = "https://files.pythonhosted.org/packages/e9/26/1dfaa81788f61c485b4d65f1b28a19615e39f9c45100dce5e2cbf5ad1352/websockets-11.0.3-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:f467ba0050b7de85016b43f5a22b46383ef004c4f672148a8abf32bc999a87f0"},
+    {url = "https://files.pythonhosted.org/packages/eb/fb/2af7fc3ce2c3f1378d48a15802b4ff2caf6c0dfac13291e73c557caf04f7/websockets-11.0.3-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:42cc5452a54a8e46a032521d7365da775823e21bfba2895fb7b77633cce031bb"},
+    {url = "https://files.pythonhosted.org/packages/ec/3f/0c5cae14e9e86401105833383405787ae4caddd476a8fc5561259253dab7/websockets-11.0.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1a073fc9ab1c8aff37c99f11f1641e16da517770e31a37265d2755282a5d28aa"},
+    {url = "https://files.pythonhosted.org/packages/ed/45/466944e00b324ae3a1fddb305b4abf641f582e131548f07bcd970971b154/websockets-11.0.3-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:ed058398f55163a79bb9f06a90ef9ccc063b204bb346c4de78efc5d15abfe602"},
+    {url = "https://files.pythonhosted.org/packages/f3/82/2d1f3395d47fab65fa8b801e2251b324300ed8db54753b6fb7919cef0c11/websockets-11.0.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:84d27a4832cc1a0ee07cdcf2b0629a8a72db73f4cf6de6f0904f6661227f256f"},
+    {url = "https://files.pythonhosted.org/packages/f4/3f/65dfa50084a06ab0a05f3ca74195c2c17a1c075b8361327d831ccce0a483/websockets-11.0.3-cp39-cp39-win_amd64.whl", hash = "sha256:c792ea4eabc0159535608fc5658a74d1a81020eb35195dd63214dcf07556f67e"},
+]
+"werkzeug 2.2.3" = [
+    {url = "https://files.pythonhosted.org/packages/02/3c/baaebf3235c87d61d6593467056d5a8fba7c75ac838b8d100a5e64eba7a0/Werkzeug-2.2.3.tar.gz", hash = "sha256:2e1ccc9417d4da358b9de6f174e3ac094391ea1d4fbef2d667865d819dfd0afe"},
+    {url = "https://files.pythonhosted.org/packages/f6/f8/9da63c1617ae2a1dec2fbf6412f3a0cfe9d4ce029eccbda6e1e4258ca45f/Werkzeug-2.2.3-py3-none-any.whl", hash = "sha256:56433961bc1f12533306c624f3be5e744389ac61d722175d543e1751285da612"},
+]
+"widgetsnbextension 4.0.7" = [
+    {url = "https://files.pythonhosted.org/packages/2e/f0/6e3a0d9c1ef015322cad1dd2191c338349b41151e4dc5e7ae984700c9dd2/widgetsnbextension-4.0.7-py3-none-any.whl", hash = "sha256:be3228a73bbab189a16be2d4a3cd89ecbd4e31948bfdc64edac17dcdee3cd99c"},
+    {url = "https://files.pythonhosted.org/packages/5b/19/df018c3ab363969cffb9ee38cbff0187634137335de0e083cad8c94bb130/widgetsnbextension-4.0.7.tar.gz", hash = "sha256:ea67c17a7cd4ae358f8f46c3b304c40698bc0423732e3f273321ee141232c8be"},
 ]
 "win32-setctime 1.1.0" = [
     {url = "https://files.pythonhosted.org/packages/0a/e6/a7d828fef907843b2a5773ebff47fb79ac0c1c88d60c0ca9530ee941e248/win32_setctime-1.1.0-py3-none-any.whl", hash = "sha256:231db239e959c2fe7eb1d7dc129f11172354f98361c4fa2d6d2d7e278baa8aad"},
     {url = "https://files.pythonhosted.org/packages/6b/dd/f95a13d2b235a28d613ba23ebad55191514550debb968b46aab99f2e3a30/win32_setctime-1.1.0.tar.gz", hash = "sha256:15cf5750465118d6929ae4de4eb46e8edae9a5634350c01ba582df868e932cb2"},
 ]
-"zipp 3.11.0" = [
-    {url = "https://files.pythonhosted.org/packages/8e/b3/8b16a007184714f71157b1a71bbe632c5d66dd43bc8152b3c799b13881e1/zipp-3.11.0.tar.gz", hash = "sha256:a7a22e05929290a67401440b39690ae6563279bced5f314609d9d03798f56766"},
-    {url = "https://files.pythonhosted.org/packages/d8/20/256eb3f3f437c575fb1a2efdce5e801a5ce3162ea8117da96c43e6ee97d8/zipp-3.11.0-py3-none-any.whl", hash = "sha256:83a28fcb75844b5c0cdaf5aa4003c2d728c77e05f5aeabe8e95e56727005fbaa"},
+"zipp 3.15.0" = [
+    {url = "https://files.pythonhosted.org/packages/00/27/f0ac6b846684cecce1ee93d32450c45ab607f65c2e0255f0092032d91f07/zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
+    {url = "https://files.pythonhosted.org/packages/5b/fa/c9e82bbe1af6266adf08afb563905eb87cab83fde00a0a08963510621047/zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
 ]
```

### Comparing `saxo_apy-0.2.4/samples/01_getting_started.ipynb` & `saxo_apy-0.2.5/samples/01_getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/samples/02_advanced_login.ipynb` & `saxo_apy-0.2.5/samples/02_advanced_login.ipynb`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/samples/03_session_management.ipynb` & `saxo_apy-0.2.5/samples/03_session_management.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998611111111111%*

 * *Differences: {"'cells'": "{4: {'source': {delete: [5]}}}"}*

```diff
@@ -79,15 +79,14 @@
             "outputs": [],
             "source": [
                 "client = SaxoOpenAPIClient()\n",
                 "client.login()\n",
                 "\n",
                 "\n",
                 "async def main() -> None:\n",
-                "\n",
                 "    # do all kinds of application logic here\n",
                 "    # make sure nothing in here is looping/blocking otherwise the refresh call won't be reached\n",
                 "\n",
                 "    # ensure that asyncio schedules the refresh loop\n",
                 "    asyncio.ensure_future(client.async_refresh())\n",
                 "\n",
                 "\n",
```

### Comparing `saxo_apy-0.2.4/samples/04_debugging_and_logging.ipynb` & `saxo_apy-0.2.5/samples/04_debugging_and_logging.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986288265306122%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, '\\n')]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.3'}}"}*

```diff
@@ -14,14 +14,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from saxo_apy import SaxoOpenAPIClient\n",
                 "\n",
+                "\n",
                 "client = SaxoOpenAPIClient(\n",
                 "    log_sink=\"log.txt\",  # controls the file to append logs to (will not override existing file!)\n",
                 "    log_level=\"DEBUG\",  # controls the level of log messages to be written to the file (default is DEBUG)\n",
                 ")"
             ]
         },
         {
@@ -134,15 +135,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.1 (main, Dec 23 2022, 09:28:24) [Clang 14.0.0 (clang-1400.0.29.202)]"
+            "version": "3.11.3"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "3f753197f020b6236bb06be37c192ff4bc0da2ccc1bf66f005a7556bcabdf016"
             }
         }
```

### Comparing `saxo_apy-0.2.4/samples/05_price_alerts_crud.ipynb` & `saxo_apy-0.2.5/samples/05_price_alerts_crud.ipynb`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/samples/06_instrument_search.ipynb` & `saxo_apy-0.2.5/samples/06_instrument_search.ipynb`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/samples/07_pricing_and_orders.ipynb` & `saxo_apy-0.2.5/samples/07_pricing_and_orders.ipynb`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/samples/README.md` & `saxo_apy-0.2.5/samples/README.md`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/samples/s01_async_requests.py` & `saxo_apy-0.2.5/samples/s01_async_requests.py`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/samples/s02_streaming_prices.py` & `saxo_apy-0.2.5/samples/s02_streaming_prices.py`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/saxo_apy/client.py` & `saxo_apy-0.2.5/saxo_apy/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -169,15 +169,15 @@
                 except ValidationError as e:
                     print(f"❌ failed to parse provided url due to error(s): {e}")
                 except KeyboardInterrupt:
                     logger.warning("keyboard interrupt received - shutting down")
                     print("🛑 operation interrupted by user - shutting down")
                     return
 
-        self.get_tokens(auth_code=_auth_code)
+        self._get_tokens(auth_code=_auth_code)
 
         assert self._token_data
 
         env = self._app_config.env.value  # type: ignore[union-attr]
         perm = "WRITE / TRADE" if self._token_data.write_permission else "READ"
 
         print(
@@ -220,15 +220,15 @@
 
         Automatically updates htt_session headers with new token and sends PUT request
         for the streaming websocket connection (if available).
         """
         logger.debug("refreshing API session")
         assert self.logged_in
 
-        self.get_tokens()
+        self._get_tokens()
         assert self._token_data
 
         if self.streaming_connection:
             logger.debug(f"found streaming connection with context_id: {self.streaming_context_id} - re-authorizing")
             self.put(
                 "/streamingws/authorize",
                 params={"ContextId": self.streaming_context_id},
@@ -246,15 +246,15 @@
                 f"{unix_seconds_to_datetime(int(time()) + delay)}"
             )
             await asyncio.sleep(delay)
             logger.debug("async refresh delay has passed - kicking off refresh")
             self.refresh()
         logger.debug("async refresh stopped as the client is no longer logged in")
 
-    def get_tokens(self, auth_code: Optional[AuthorizationCode] = None) -> None:
+    def _get_tokens(self, auth_code: Optional[AuthorizationCode] = None) -> None:
         """Retrieve a new token pair by exercising a refresh token or auth code."""
         authorization_param = "code" if auth_code else "refresh_token"
         grant_type = "authorization_code" if auth_code else "refresh_token"
         logger.debug(f"exercising authorization with grant type: {grant_type}")
 
         request_id = token_urlsafe(ID_NUM_BYTES)
 
@@ -303,17 +303,20 @@
         This connection is used to receive messages from the OpenAPI Streaming Service.
         """
         assert self.logged_in
 
         if self.streaming_connection:
             raise RuntimeError("streaming connection already created")
 
+        assert self._token_data  # assert for mypy
+        assert self._token_data.access_token
+
         self.streaming_context_id = token_urlsafe(ID_NUM_BYTES)
         url = f"{self._app_config.streaming_url}/connect?contextId={self.streaming_context_id}"
-        headers = {"Authorization": f"Bearer {self._token_data.access_token}"}  # type: ignore[union-attr]
+        headers = {"Authorization": f"Bearer {self._token_data.access_token}"}
         self.streaming_connection = ws_client.connect(url, extra_headers=headers)
 
     def get(self, path: str, params: Optional[Dict] = None) -> Dict:
         """Send GET request to OpenAPI and handle response."""
         response = handle_api_response(self.openapi_request("GET", path, params))
         return response.json()
 
@@ -375,19 +378,23 @@
             logger.debug("prepended '/' to request path as it is not provided")
             _path = "/" + path
         else:
             _path = path
 
         request_id = token_urlsafe(ID_NUM_BYTES)
 
+        assert self._app_config.env  # assert for mypy
+        assert self._token_data
+        assert self._token_data.access_token
+
         headers = {
             "x-request-id": f"saxo-apy/{VERSION}/{self.client_session_id}/{request_id}",
-            "x-openapi-env": self._app_config.env.value,  # type: ignore[union-attr]
+            "x-openapi-env": self._app_config.env.value,
             "x-client-timestamp": datetime.utcnow().isoformat(),
-            "authorization": f"Bearer {self._token_data.access_token}",  # type: ignore[union-attr]
+            "authorization": f"Bearer {self._token_data.access_token}",
         }
 
         logger.debug(f"performing request with id: {request_id} - {method} {_path}, {params=}, {data=}")
 
         response = self._http_client.request(
             method,
             path,
@@ -407,34 +414,40 @@
     def api_base_url(self) -> HttpsUrl:
         """Retrieve base URL to construct requests with."""
         return self._app_config.api_base_url
 
     @property
     def streaming_url(self) -> HttpsUrl:
         """Retrieve streaming URL to set up websocket connection."""
-        return self._app_config.streaming_url  # type: ignore[return-value]
+        assert self._app_config.streaming_url  # set on init, assert for mypy
+        return self._app_config.streaming_url
 
     @property
     def logged_in(self) -> bool:
         """Check if the client is connected with a valid session to OpenAPI.
 
         If no token data is available, the client is not logged in (yet).
         If the access token has expired, the client is effectively disconnected.
         """
         if not self._token_data:
             raise NotLoggedInError("no active session found - connect the client with '.login()'")
+        assert self._token_data.access_token_expiry
         if time() > self._token_data.access_token_expiry:
             raise TokenExpiredError("access token has expired - reconnect the client with '.login()'")
         return True
 
     @property
     def access_token_expiry(self) -> datetime:
         """Retrieve human-readable access token expiry."""
         assert self.logged_in
-        return unix_seconds_to_datetime(self._token_data.access_token_expiry)  # type: ignore[union-attr]
+        assert self._token_data  # this is already checked by logged_in property but mypy doesn't know...
+        assert self._token_data.access_token_expiry
+        return unix_seconds_to_datetime(self._token_data.access_token_expiry)
 
     @property
     def time_to_expiry(self) -> int:
         """Retrieve time in seconds until access token expires."""
         assert self.logged_in
-        token_expiry = self._token_data.access_token_expiry  # type: ignore[union-attr]
+        assert self._token_data  # this is already checked by logged_in property but mypy doesn't know...
+        assert self._token_data.access_token_expiry
+        token_expiry = self._token_data.access_token_expiry
         return token_expiry - int(time())
```

### Comparing `saxo_apy-0.2.4/saxo_apy/models.py` & `saxo_apy-0.2.5/saxo_apy/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,20 +130,20 @@
 
     access_token: str
     token_type: str
     expires_in: int
     refresh_token: RefreshToken
     refresh_token_expires_in: int
     base_uri: Optional[HttpsUrl]
-    access_token_expiry: int
-    refresh_token_expiry: int
-    client_key: str
-    user_key: str
-    session_id: str
-    write_permission: bool
+    access_token_expiry: Optional[int] = None
+    refresh_token_expiry: Optional[int] = None
+    client_key: Optional[str] = None
+    user_key: Optional[str] = None
+    session_id: Optional[str] = None
+    write_permission: Optional[bool] = None
 
     @root_validator(pre=True)
     def set_fields_from_token_payload(cls, values: Dict) -> Dict:
         """Set fields from token claims."""
         token_bytes = values["access_token"].encode("utf-8")
         payload = token_bytes.split(b".")[1]
         padded = payload + b"=" * divmod(len(payload), 4)[1]
```

### Comparing `saxo_apy-0.2.4/saxo_apy/redirect_server.py` & `saxo_apy-0.2.5/saxo_apy/redirect_server.py`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/saxo_apy/utils.py` & `saxo_apy-0.2.5/saxo_apy/utils.py`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/tests/test_client.py` & `saxo_apy-0.2.5/tests/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 from saxo_apy.client import SaxoOpenAPIClient
 from saxo_apy.models import (
     LIVE_STREAMING_URL,
     SIM_STREAMING_URL,
     APIEnvironment,
     NotLoggedInError,
     OpenAPIAppConfig,
+    RefreshToken,
     TokenData,
     TokenExpiredError,
 )
 
 from .fixtures.models import DUMMY_ACCESS_TOKEN, DUMMY_LIVE_CONFIG, DUMMY_SIM_CONFIG
 
 DUMMY_TOKEN_DATA = TokenData(
     access_token=DUMMY_ACCESS_TOKEN,
     token_type="Bearer",
     expires_in=1200,
-    refresh_token="12341234-1234-1234-1234-123412341234",
+    refresh_token=RefreshToken("12341234-1234-1234-1234-123412341234"),
     refresh_token_expires_in=3600,
     base_uri=None,
-    redirect_url="https://localhost:12321/redirect",
 )
 
 
 @mark.parametrize(
     "config, env",
     [
         (DUMMY_SIM_CONFIG, APIEnvironment.SIM),
```

### Comparing `saxo_apy-0.2.4/tests/test_models.py` & `saxo_apy-0.2.5/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/tests/test_utils.py` & `saxo_apy-0.2.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/tests/fixtures/dummy_app_config_live.json` & `saxo_apy-0.2.5/tests/fixtures/dummy_app_config_live.json`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/tests/fixtures/dummy_app_config_sim.json` & `saxo_apy-0.2.5/tests/fixtures/dummy_app_config_sim.json`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/tests/fixtures/models.py` & `saxo_apy-0.2.5/tests/fixtures/models.py`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/LICENSE` & `saxo_apy-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.4/README.md` & `saxo_apy-0.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 00000d70: 696f 6e73 2066 6f72 2074 6865 2061 7070  ions for the app
 00000d80: 2069 6620 796f 7520 7761 6e74 2074 6f20   if you want to 
 00000d90: 2777 7269 7465 2720 746f 2079 6f75 7220  'write' to your 
 00000da0: 6163 636f 756e 7420 2861 6e64 2070 6c61  account (and pla
 00000db0: 6365 206f 7264 6572 7329 0a0a 2323 2044  ce orders)..## D
 00000dc0: 6570 656e 6465 6e63 6965 730a 0a54 6869  ependencies..Thi
 00000dd0: 7320 7061 636b 6167 6520 7265 7175 6972  s package requir
-00000de0: 6573 2034 2064 6570 656e 6465 6e63 6965  es 4 dependencie
+00000de0: 6573 2035 2064 6570 656e 6465 6e63 6965  es 5 dependencie
 00000df0: 733a 0a0a 2d20 6070 7964 616e 7469 6360  s:..- `pydantic`
 00000e00: 2c20 666f 7220 7061 7273 696e 6720 636f  , for parsing co
 00000e10: 6e66 6967 2061 6e64 204a 534f 4e20 7265  nfig and JSON re
 00000e20: 7370 6f6e 7365 7320 0a2d 2060 466c 6173  sponses .- `Flas
 00000e30: 6b60 2c20 746f 2072 756e 2061 206c 6f63  k`, to run a loc
 00000e40: 616c 2073 6572 7665 7220 616e 6420 6361  al server and ca
 00000e50: 7463 6820 7468 6520 6361 6c6c 6261 636b  tch the callback
```

### Comparing `saxo_apy-0.2.4/pyproject.toml` & `saxo_apy-0.2.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "saxo-apy"
 description = "A lightweight Python client for hassle-free tinkering with Saxo OpenAPI."
 authors = [
     {name = "Gid", email = "giddevanderven@gmail.com"},
 ]
 dependencies = [
-    "httpx~=0.23",
-    "pydantic~=1.10",
-    "flask~=2.2",
-    "websockets~=10.4",
-    "loguru~=0.6",
+    "httpx>=0.24.1",
+    "pydantic>=1.10.8",
+    "flask>=2.2.5",
+    "websockets>=11.0.3",
+    "loguru>=0.7.0",
 ]
 requires-python = ">=3.7"
 readme = "README.md"
 license = {text = "MIT"}
 dynamic = ["version"]
 
 [tool.pdm]
 [tool.pdm.dev-dependencies]
 dev = [
-    "mypy~=0.991",
-    "black[jupyter]~=22.12",
-    "pydocstyle~=6.3",
-    "pytest~=7.2",
-    "pytest-cov~=4.0",
-    "jupyter~=1.0",
-    "isort~=5.11",
-    "flake8~=5.0",
-    "flake8-pyproject~=1.2",
+    "mypy>=1.3.0",
+    "black[jupyter]>=23.3.0",
+    "pydocstyle>=6.3.0",
+    "pytest>=7.3.1",
+    "pytest-cov>=4.1.0",
+    "jupyter>=1.0.0",
+    "isort>=5.11.5",
+    "flake8>=5.0.4",
+    "flake8-pyproject>=1.2.3",
 ]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
```

### Comparing `saxo_apy-0.2.4/PKG-INFO` & `saxo_apy-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: saxo-apy
-Version: 0.2.4
+Version: 0.2.5
 Summary: A lightweight Python client for hassle-free tinkering with Saxo OpenAPI.
 Author-email: Gid <giddevanderven@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.7
-Requires-Dist: flask~=2.2
-Requires-Dist: httpx~=0.23
-Requires-Dist: loguru~=0.6
-Requires-Dist: pydantic~=1.10
-Requires-Dist: websockets~=10.4
+Requires-Dist: flask>=2.2.5
+Requires-Dist: httpx>=0.24.1
+Requires-Dist: loguru>=0.7.0
+Requires-Dist: pydantic>=1.10.8
+Requires-Dist: websockets>=11.0.3
 Description-Content-Type: text/markdown
 
 ```
    _____         __   __  ____                   _____  __     __
   / ____|   /\   \ \ / / / __ \            /\   |  __ \ \ \   / /
  | (___    /  \   \ V / | |  | |  ____    /  \  | |__) | \ \_/ / 
   \___ \  / /\ \   ) (  | |  | | |____|  / /\ \ |  ___/   \   /  
@@ -87,15 +87,15 @@
     - [Create a free developer account](https://www.developer.saxo/accounts/sim/signup) if you don't have one already.
     - Ensure the application is set up with `Grant Type: Code` as authentication flow.
     - At least 1 localhost redirect needs to be defined such as `http://localhost:12321/redirect` (for development/testing purposes)
     - (Optional) enable trading permissions for the app if you want to 'write' to your account (and place orders)
 
 ## Dependencies
 
-This package requires 4 dependencies:
+This package requires 5 dependencies:
 
 - `pydantic`, for parsing config and JSON responses 
 - `Flask`, to run a local server and catch the callback from Saxo SSO
 - `httpx`, for sending requests to OpenAPI and managing the client session
 - `websockets`, for setting up a websocket connection to Saxo's streaming service
 - `loguru`, to handle logging
```

