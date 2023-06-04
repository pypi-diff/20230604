# Comparing `tmp/fastapi_opa-1.4.4.tar.gz` & `tmp/fastapi_opa-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_opa-1.4.4.tar", max compression
+gzip compressed data, was "fastapi_opa-1.4.5.tar", max compression
```

## Comparing `fastapi_opa-1.4.4.tar` & `fastapi_opa-1.4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-05-24 09:09:19.494956 fastapi_opa-1.4.4/LICENSE
--rw-r--r--   0        0        0     7438 2023-05-24 09:09:19.494956 fastapi_opa-1.4.4/README.md
--rw-r--r--   0        0        0      122 2023-05-24 09:09:19.498956 fastapi_opa-1.4.4/fastapi_opa/__init__.py
--rw-r--r--   0        0        0      124 2023-05-24 09:09:19.498956 fastapi_opa-1.4.4/fastapi_opa/auth/__init__.py
--rw-r--r--   0        0        0     1019 2023-05-24 09:09:19.498956 fastapi_opa-1.4.4/fastapi_opa/auth/auth_api_key.py
--rw-r--r--   0        0        0      709 2023-05-24 09:09:19.498956 fastapi_opa-1.4.4/fastapi_opa/auth/auth_interface.py
--rw-r--r--   0        0        0     8855 2023-05-24 09:33:14.226654 fastapi_opa-1.4.4/fastapi_opa/auth/auth_oidc.py
--rw-r--r--   0        0        0     5433 2023-05-24 09:09:19.498956 fastapi_opa-1.4.4/fastapi_opa/auth/auth_saml.py
--rw-r--r--   0        0        0      328 2023-05-24 09:09:19.498956 fastapi_opa-1.4.4/fastapi_opa/auth/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-24 09:09:19.498956 fastapi_opa-1.4.4/fastapi_opa/opa/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 09:09:19.498956 fastapi_opa-1.4.4/fastapi_opa/opa/enrichment/__init__.py
--rw-r--r--   0        0        0     3771 2023-05-24 09:09:19.498956 fastapi_opa-1.4.4/fastapi_opa/opa/enrichment/graphql_enrichment.py
--rw-r--r--   0        0        0     1107 2023-05-24 09:09:19.498956 fastapi_opa-1.4.4/fastapi_opa/opa/opa_config.py
--rw-r--r--   0        0        0     5468 2023-05-24 09:33:14.226654 fastapi_opa-1.4.4/fastapi_opa/opa/opa_middleware.py
--rw-r--r--   0        0        0     1438 2023-05-24 09:33:14.230654 fastapi_opa-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     8616 1970-01-01 00:00:00.000000 fastapi_opa-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-24 09:09:19.494956 fastapi_opa-1.4.5/LICENSE
+-rw-r--r--   0        0        0     7438 2023-05-24 09:09:19.494956 fastapi_opa-1.4.5/README.md
+-rw-r--r--   0        0        0      122 2023-05-24 09:09:19.498956 fastapi_opa-1.4.5/fastapi_opa/__init__.py
+-rw-r--r--   0        0        0      124 2023-05-24 09:09:19.498956 fastapi_opa-1.4.5/fastapi_opa/auth/__init__.py
+-rw-r--r--   0        0        0     1019 2023-05-24 09:09:19.498956 fastapi_opa-1.4.5/fastapi_opa/auth/auth_api_key.py
+-rw-r--r--   0        0        0      709 2023-05-24 09:09:19.498956 fastapi_opa-1.4.5/fastapi_opa/auth/auth_interface.py
+-rw-r--r--   0        0        0     8855 2023-05-24 09:33:14.226654 fastapi_opa-1.4.5/fastapi_opa/auth/auth_oidc.py
+-rw-r--r--   0        0        0     5433 2023-05-24 09:09:19.498956 fastapi_opa-1.4.5/fastapi_opa/auth/auth_saml.py
+-rw-r--r--   0        0        0      328 2023-05-24 09:09:19.498956 fastapi_opa-1.4.5/fastapi_opa/auth/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:09:19.498956 fastapi_opa-1.4.5/fastapi_opa/opa/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:09:19.498956 fastapi_opa-1.4.5/fastapi_opa/opa/enrichment/__init__.py
+-rw-r--r--   0        0        0     3771 2023-05-24 09:09:19.498956 fastapi_opa-1.4.5/fastapi_opa/opa/enrichment/graphql_enrichment.py
+-rw-r--r--   0        0        0     1107 2023-05-24 09:09:19.498956 fastapi_opa-1.4.5/fastapi_opa/opa/opa_config.py
+-rw-r--r--   0        0        0     5468 2023-05-24 09:33:14.226654 fastapi_opa-1.4.5/fastapi_opa/opa/opa_middleware.py
+-rw-r--r--   0        0        0     1238 2023-06-04 07:27:01.100916 fastapi_opa-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     8575 1970-01-01 00:00:00.000000 fastapi_opa-1.4.5/PKG-INFO
```

### Comparing `fastapi_opa-1.4.4/LICENSE` & `fastapi_opa-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_opa-1.4.4/README.md` & `fastapi_opa-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_opa-1.4.4/fastapi_opa/auth/auth_api_key.py` & `fastapi_opa-1.4.5/fastapi_opa/auth/auth_api_key.py`

 * *Files identical despite different names*

### Comparing `fastapi_opa-1.4.4/fastapi_opa/auth/auth_interface.py` & `fastapi_opa-1.4.5/fastapi_opa/auth/auth_interface.py`

 * *Files identical despite different names*

### Comparing `fastapi_opa-1.4.4/fastapi_opa/auth/auth_oidc.py` & `fastapi_opa-1.4.5/fastapi_opa/auth/auth_oidc.py`

 * *Files identical despite different names*

### Comparing `fastapi_opa-1.4.4/fastapi_opa/auth/auth_saml.py` & `fastapi_opa-1.4.5/fastapi_opa/auth/auth_saml.py`

 * *Files identical despite different names*

### Comparing `fastapi_opa-1.4.4/fastapi_opa/opa/enrichment/graphql_enrichment.py` & `fastapi_opa-1.4.5/fastapi_opa/opa/enrichment/graphql_enrichment.py`

 * *Files identical despite different names*

### Comparing `fastapi_opa-1.4.4/fastapi_opa/opa/opa_config.py` & `fastapi_opa-1.4.5/fastapi_opa/opa/opa_config.py`

 * *Files identical despite different names*

### Comparing `fastapi_opa-1.4.4/fastapi_opa/opa/opa_middleware.py` & `fastapi_opa-1.4.5/fastapi_opa/opa/opa_middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_opa-1.4.4/pyproject.toml` & `fastapi_opa-1.4.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-opa"
-version = "1.4.4"
+version = "1.4.5"
 description = "Fastapi OPA middleware incl. auth flow."
 authors = ["Matthias Osswald <info@busykoala.io>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/busykoala/fastapi-opa"
 keywords = ["fastapi", "oidc", "authentication", "authorization", "saml"]
 exclude = ["fastapi_opa/example_oidc.py", "fastapi_opa/example_saml.py"]
@@ -14,20 +14,17 @@
 fastapi = ">= 0.65.2"
 itsdangerous = "*"
 requests = "*"
 PyJWT = {extras = ["crypto"], version = ">= 2.4"}
 graphene = {version = "^2", optional = true}
 python3-saml = {version = "*", optional = true}
 python-multipart = {version = "*", optional = true}
-# transitive overrides
-importlib-metadata = "< 5.0"  # https://importlib-metadata.readthedocs.io/en/latest/history.html
-
 
 [tool.poetry.dev-dependencies]
-flake9 = "*"
+flake8 = "*"
 black = "*"
 isort = "*"
 bandit = "*"
 pytest = "*"
 pytest-mock = "*"
 mock = "*"
 freezegun = "*"
@@ -44,16 +41,11 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line_length = 79
 
-[tool.flake8]
-max-complexity = 15
-max-line-length = 79
-extend-ignore = "E203"
-
 [tool.isort]
 line_length = 79
 include_trailing_comma = true
 force_single_line = true
```

### Comparing `fastapi_opa-1.4.4/PKG-INFO` & `fastapi_opa-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-opa
-Version: 1.4.4
+Version: 1.4.5
 Summary: Fastapi OPA middleware incl. auth flow.
 Home-page: https://github.com/busykoala/fastapi-opa
 License: GPL-3.0-or-later
 Keywords: fastapi,oidc,authentication,authorization,saml
 Author: Matthias Osswald
 Author-email: info@busykoala.io
 Requires-Python: >=3.7,<4.0
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: graphql
 Provides-Extra: saml
 Requires-Dist: PyJWT[crypto] (>=2.4)
 Requires-Dist: fastapi (>=0.65.2)
 Requires-Dist: graphene (>=2,<3) ; extra == "graphql"
-Requires-Dist: importlib-metadata (<5.0)
 Requires-Dist: itsdangerous
 Requires-Dist: python-multipart ; extra == "saml"
 Requires-Dist: python3-saml ; extra == "saml"
 Requires-Dist: requests
 Project-URL: Repository, https://github.com/busykoala/fastapi-opa
 Description-Content-Type: text/markdown
```

