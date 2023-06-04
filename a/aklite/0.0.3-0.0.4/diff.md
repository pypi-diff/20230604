# Comparing `tmp/aklite-0.0.3.tar.gz` & `tmp/aklite-0.0.4.tar.gz`

## Comparing `aklite-0.0.3.tar` & `aklite-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aklite-0.0.3/.readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 aklite-0.0.3/requirements-dev.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aklite-0.0.3/requirements.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 aklite-0.0.3/docs/requirements.txt
--rw-r--r--   0        0        0     7085 2020-02-02 00:00:00.000000 aklite-0.0.3/docs/locales/zh_CN/LC_MESSAGES/index.po
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 aklite-0.0.3/docs/locales/zh_CN/LC_MESSAGES/notebooks/stock.po
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 aklite-0.0.3/docs/source/conf.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 aklite-0.0.3/docs/source/index.rst
--rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 aklite-0.0.3/docs/source/notebooks/stock.ipynb
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 aklite-0.0.3/src/aklite/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aklite-0.0.3/src/aklite/stock/__init__.py
--rw-r--r--   0        0        0     6957 2020-02-02 00:00:00.000000 aklite-0.0.3/src/aklite/stock/stock_hist_em.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 aklite-0.0.3/tests/test_ak.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 aklite-0.0.3/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 aklite-0.0.3/LICENSE
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 aklite-0.0.3/README.md
--rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 aklite-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 aklite-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aklite-0.0.4/.readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 aklite-0.0.4/requirements-dev.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aklite-0.0.4/requirements.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 aklite-0.0.4/docs/requirements.txt
+-rw-r--r--   0        0        0     7085 2020-02-02 00:00:00.000000 aklite-0.0.4/docs/locales/zh_CN/LC_MESSAGES/index.po
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 aklite-0.0.4/docs/locales/zh_CN/LC_MESSAGES/notebooks/stock.po
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 aklite-0.0.4/docs/source/conf.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 aklite-0.0.4/docs/source/index.rst
+-rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 aklite-0.0.4/docs/source/notebooks/stock.ipynb
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 aklite-0.0.4/src/aklite/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aklite-0.0.4/src/aklite/stock/__init__.py
+-rw-r--r--   0        0        0     6957 2020-02-02 00:00:00.000000 aklite-0.0.4/src/aklite/stock/stock_hist_em.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 aklite-0.0.4/tests/test_ak.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 aklite-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 aklite-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 aklite-0.0.4/README.md
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 aklite-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 aklite-0.0.4/PKG-INFO
```

### Comparing `aklite-0.0.3/docs/locales/zh_CN/LC_MESSAGES/index.po` & `aklite-0.0.4/docs/locales/zh_CN/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `aklite-0.0.3/docs/locales/zh_CN/LC_MESSAGES/notebooks/stock.po` & `aklite-0.0.4/docs/locales/zh_CN/LC_MESSAGES/notebooks/stock.po`

 * *Files identical despite different names*

### Comparing `aklite-0.0.3/docs/source/conf.py` & `aklite-0.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aklite-0.0.3/docs/source/index.rst` & `aklite-0.0.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `aklite-0.0.3/docs/source/notebooks/stock.ipynb` & `aklite-0.0.4/docs/source/notebooks/stock.ipynb`

 * *Files identical despite different names*

### Comparing `aklite-0.0.3/src/aklite/stock/stock_hist_em.py` & `aklite-0.0.4/src/aklite/stock/stock_hist_em.py`

 * *Files identical despite different names*

### Comparing `aklite-0.0.3/LICENSE` & `aklite-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aklite-0.0.3/README.md` & `aklite-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aklite-0.0.3/pyproject.toml` & `aklite-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "pandas>=2.0.0,<3",
-    "requests>=2.31.0,<3",
+    "httpx>=0.24.1,<1",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/jindaxiang/aklite"
 Documentation = "https://aklite.readthedocs.io"
```

### Comparing `aklite-0.0.3/PKG-INFO` & `aklite-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aklite
-Version: 0.0.3
+Version: 0.0.4
 Summary: AKLite is lite version fo AKShare
 Project-URL: Homepage, https://github.com/jindaxiang/aklite
 Project-URL: Documentation, https://aklite.readthedocs.io
 Author-email: Albert King <albertandking@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -30,16 +30,16 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
+Requires-Dist: httpx<1,>=0.24.1
 Requires-Dist: pandas<3,>=2.0.0
-Requires-Dist: requests<3,>=2.31.0
 Provides-Extra: all
 Requires-Dist: httpx<1,>=0.24.1; extra == 'all'
 Requires-Dist: pandas<3,>=2.0.0; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev'
 Requires-Dist: ruff==0.0.138; extra == 'dev'
 Requires-Dist: uvicorn[standard]<0.21.0,>=0.12.0; extra == 'dev'
```

