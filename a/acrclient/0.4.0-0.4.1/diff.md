# Comparing `tmp/acrclient-0.4.0.tar.gz` & `tmp/acrclient-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acrclient-0.4.0.tar", max compression
+gzip compressed data, was "acrclient-0.4.1.tar", max compression
```

## Comparing `acrclient-0.4.0.tar` & `acrclient-0.4.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2287 2023-05-19 10:37:11.721984 acrclient-0.4.0/README.md
--rw-r--r--   0        0        0      307 2023-05-19 10:37:11.721984 acrclient-0.4.0/acrclient/__init__.py
--rw-r--r--   0        0        0     4983 2023-05-19 10:37:11.721984 acrclient-0.4.0/acrclient/client.py
--rw-r--r--   0        0        0      664 2023-05-19 10:37:11.721984 acrclient-0.4.0/acrclient/models.py
--rw-r--r--   0        0        0        0 2023-05-19 10:37:11.721984 acrclient-0.4.0/acrclient/py.typed
--rw-r--r--   0        0        0     1672 2023-05-19 10:37:37.377805 acrclient-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 acrclient-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2287 2023-06-04 20:54:09.005451 acrclient-0.4.1/README.md
+-rw-r--r--   0        0        0      307 2023-06-04 20:54:09.005451 acrclient-0.4.1/acrclient/__init__.py
+-rw-r--r--   0        0        0     4983 2023-06-04 20:54:09.005451 acrclient-0.4.1/acrclient/client.py
+-rw-r--r--   0        0        0      664 2023-06-04 20:54:09.005451 acrclient-0.4.1/acrclient/models.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:54:09.005451 acrclient-0.4.1/acrclient/py.typed
+-rw-r--r--   0        0        0     1706 2023-06-04 20:54:26.917651 acrclient-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3014 1970-01-01 00:00:00.000000 acrclient-0.4.1/PKG-INFO
```

### Comparing `acrclient-0.4.0/README.md` & `acrclient-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `acrclient-0.4.0/acrclient/client.py` & `acrclient-0.4.1/acrclient/client.py`

 * *Files identical despite different names*

### Comparing `acrclient-0.4.0/acrclient/models.py` & `acrclient-0.4.1/acrclient/models.py`

 * *Files identical despite different names*

### Comparing `acrclient-0.4.0/pyproject.toml` & `acrclient-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "acrclient"
-version = "v0.4.0"
+version = "v0.4.1"
 description = "API wrapper for the v2 ACRCloud API"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-v3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -13,14 +13,15 @@
 packages = [
     { include = "acrclient"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = ">=2.28.2"
+cachecontrol = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 wheel = "^0.40.0"
 types-requests = "^2.28.11"
 flake8 = "^6.0.0"
@@ -31,15 +32,15 @@
 requests-mock = "^1.10.0"
 black = "^23.3.0"
 isort = "^5.11.4"
 Markdown = "^3.3"
 pytest-mypy = "^0.10.3"
 pytest-pylint = "^0.19.0"
 pytest-random-order = "^1.1.0"
-mkdocstrings = {extras = ["python"], version = "^0.21.2"}
+mkdocstrings = {extras = ["python"], version = ">=0.21.2,<0.23.0"}
 mkdocs-material = "^9.1"
 mkdocs = "^1.4.2"
 mkdocs-gen-files = "^0.5.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
```

### Comparing `acrclient-0.4.0/PKG-INFO` & `acrclient-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: acrclient
-Version: 0.4.0
+Version: 0.4.1
 Summary: API wrapper for the v2 ACRCloud API
 License: AGPL-v3
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: cachecontrol (>=0.13.0,<0.14.0)
 Requires-Dist: requests (>=2.28.2)
 Description-Content-Type: text/markdown
 
 # Python ACR Client module
 
 Contains a simple client for calling the v2 endpoints of the [ACRCloud](https://www.acrcloud.com) API.
```

