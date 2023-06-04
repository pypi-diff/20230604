# Comparing `tmp/aklite-0.0.2.tar.gz` & `tmp/aklite-0.0.3.tar.gz`

## Comparing `aklite-0.0.2.tar` & `aklite-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aklite-0.0.2/.readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 aklite-0.0.2/requirements-dev.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aklite-0.0.2/requirements.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 aklite-0.0.2/docs/requirements.txt
--rw-r--r--   0        0        0     7085 2020-02-02 00:00:00.000000 aklite-0.0.2/docs/locales/zh_CN/LC_MESSAGES/index.po
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 aklite-0.0.2/docs/locales/zh_CN/LC_MESSAGES/notebooks/stock.po
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 aklite-0.0.2/docs/source/conf.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 aklite-0.0.2/docs/source/index.rst
--rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 aklite-0.0.2/docs/source/notebooks/stock.ipynb
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 aklite-0.0.2/src/aklite/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aklite-0.0.2/src/aklite/stock/__init__.py
--rw-r--r--   0        0        0     6957 2020-02-02 00:00:00.000000 aklite-0.0.2/src/aklite/stock/stock_hist_em.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 aklite-0.0.2/tests/test_ak.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 aklite-0.0.2/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 aklite-0.0.2/LICENSE
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aklite-0.0.2/README.md
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 aklite-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 aklite-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aklite-0.0.3/.readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 aklite-0.0.3/requirements-dev.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aklite-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 aklite-0.0.3/docs/requirements.txt
+-rw-r--r--   0        0        0     7085 2020-02-02 00:00:00.000000 aklite-0.0.3/docs/locales/zh_CN/LC_MESSAGES/index.po
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 aklite-0.0.3/docs/locales/zh_CN/LC_MESSAGES/notebooks/stock.po
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 aklite-0.0.3/docs/source/conf.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 aklite-0.0.3/docs/source/index.rst
+-rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 aklite-0.0.3/docs/source/notebooks/stock.ipynb
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 aklite-0.0.3/src/aklite/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aklite-0.0.3/src/aklite/stock/__init__.py
+-rw-r--r--   0        0        0     6957 2020-02-02 00:00:00.000000 aklite-0.0.3/src/aklite/stock/stock_hist_em.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 aklite-0.0.3/tests/test_ak.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 aklite-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 aklite-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 aklite-0.0.3/README.md
+-rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 aklite-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 aklite-0.0.3/PKG-INFO
```

### Comparing `aklite-0.0.2/docs/locales/zh_CN/LC_MESSAGES/index.po` & `aklite-0.0.3/docs/locales/zh_CN/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `aklite-0.0.2/docs/locales/zh_CN/LC_MESSAGES/notebooks/stock.po` & `aklite-0.0.3/docs/locales/zh_CN/LC_MESSAGES/notebooks/stock.po`

 * *Files identical despite different names*

### Comparing `aklite-0.0.2/docs/source/conf.py` & `aklite-0.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aklite-0.0.2/docs/source/index.rst` & `aklite-0.0.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `aklite-0.0.2/docs/source/notebooks/stock.ipynb` & `aklite-0.0.3/docs/source/notebooks/stock.ipynb`

 * *Files identical despite different names*

### Comparing `aklite-0.0.2/src/aklite/stock/stock_hist_em.py` & `aklite-0.0.3/src/aklite/stock/stock_hist_em.py`

 * *Files identical despite different names*

### Comparing `aklite-0.0.2/LICENSE` & `aklite-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aklite-0.0.2/README.md` & `aklite-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ## Introduction
 
 AKLite is a lite version of AKShare, which will be used in the future to support the AKShare project.
 
 AKLite Features:
 1. Small, fast and powerful
-2. high performance
-3. easy to ues
+2. High performance
+3. Easy to ues
 
 ## Installation
 
 ```shell
-pip install aklite
+pip install aklite --upgrade -i https://pypi.org/simple
 ```
 
 ## Usage
 
 ```python
 import aklite as ai
 
@@ -58,9 +58,7 @@
 
 ## Publish
 
 ```shell
 hatch build
 hatch publish
 ```
-
-
```

### Comparing `aklite-0.0.2/pyproject.toml` & `aklite-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 dev = [
     "ruff ==0.0.138",
     "uvicorn[standard] >=0.12.0,<0.21.0",
     "pre-commit >=2.17.0,<3.0.0",
 ]
 all = [
     "pandas>=2.0.0,<3",
-    "requests>=2.31.0,<3",
+    "httpx>=0.24.1,<1",
 ]
 
 [tool.hatch.version]
 path = "./src/aklite/__init__.py"
 
 [tool.isort]
 profile = "black"
```

### Comparing `aklite-0.0.2/PKG-INFO` & `aklite-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aklite
-Version: 0.0.2
+Version: 0.0.3
 Summary: AKLite is lite version fo AKShare
 Project-URL: Homepage, https://github.com/jindaxiang/aklite
 Project-URL: Documentation, https://aklite.readthedocs.io
 Author-email: Albert King <albertandking@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -33,16 +33,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: pandas<3,>=2.0.0
 Requires-Dist: requests<3,>=2.31.0
 Provides-Extra: all
+Requires-Dist: httpx<1,>=0.24.1; extra == 'all'
 Requires-Dist: pandas<3,>=2.0.0; extra == 'all'
-Requires-Dist: requests<3,>=2.31.0; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev'
 Requires-Dist: ruff==0.0.138; extra == 'dev'
 Requires-Dist: uvicorn[standard]<0.21.0,>=0.12.0; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
@@ -77,21 +77,21 @@
 
 ## Introduction
 
 AKLite is a lite version of AKShare, which will be used in the future to support the AKShare project.
 
 AKLite Features:
 1. Small, fast and powerful
-2. high performance
-3. easy to ues
+2. High performance
+3. Easy to ues
 
 ## Installation
 
 ```shell
-pip install aklite
+pip install aklite --upgrade -i https://pypi.org/simple
 ```
 
 ## Usage
 
 ```python
 import aklite as ai
 
@@ -135,9 +135,7 @@
 
 ## Publish
 
 ```shell
 hatch build
 hatch publish
 ```
-
-
```

