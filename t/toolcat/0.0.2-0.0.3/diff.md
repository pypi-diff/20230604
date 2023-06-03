# Comparing `tmp/toolcat-0.0.2.tar.gz` & `tmp/toolcat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolcat-0.0.2.tar", max compression
+gzip compressed data, was "toolcat-0.0.3.tar", max compression
```

## Comparing `toolcat-0.0.2.tar` & `toolcat-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1211 2023-06-03 18:15:32.691464 toolcat-0.0.2/LICENSE
--rw-r--r--   0        0        0      451 2023-06-03 18:16:59.725937 toolcat-0.0.2/README.md
--rw-r--r--   0        0        0     1103 2023-06-03 19:37:27.014602 toolcat-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       24 2023-06-03 18:15:32.694245 toolcat-0.0.2/src/toolcat/__init__.py
--rw-r--r--   0        0        0      607 2023-06-03 18:52:10.387158 toolcat-0.0.2/src/toolcat/project.py
--rw-r--r--   0        0        0     1096 2023-06-03 19:12:14.817042 toolcat-0.0.2/src/toolcat/projects_test.py
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 toolcat-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-06-03 18:15:32.691464 toolcat-0.0.3/LICENSE
+-rw-r--r--   0        0        0      182 2023-06-03 20:00:15.609596 toolcat-0.0.3/README.md
+-rw-r--r--   0        0        0     1125 2023-06-03 23:04:17.520301 toolcat-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-03 18:15:32.694245 toolcat-0.0.3/src/toolcat/__init__.py
+-rw-r--r--   0        0        0     2382 2023-06-03 23:01:48.937333 toolcat-0.0.3/src/toolcat/database.py
+-rw-r--r--   0        0        0     1400 2023-06-03 23:01:51.316471 toolcat-0.0.3/src/toolcat/database_test.py
+-rw-r--r--   0        0        0      607 2023-06-03 18:52:10.387158 toolcat-0.0.3/src/toolcat/project.py
+-rw-r--r--   0        0        0     1096 2023-06-03 19:12:14.817042 toolcat-0.0.3/src/toolcat/projects_test.py
+-rw-r--r--   0        0        0      722 1970-01-01 00:00:00.000000 toolcat-0.0.3/PKG-INFO
```

### Comparing `toolcat-0.0.2/LICENSE` & `toolcat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.2/pyproject.toml` & `toolcat-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 [tool.mypy]
 ignore_missing_imports = true
 # https://stackoverflow.com/questions/62265366/does-mypy-only-type-check-a-function-if-it-declares-a-return-type
 check_untyped_defs = true
 
 [tool.poetry]
 name = "toolcat"
-version = "0.0.2"
+version = "0.0.3"
 description = "Essential Libraries and Tools for Streamlined Development"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicence"
 readme = "README.md"
 packages = [{ include = "toolcat", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 toml = "^0.10.2"
+sqlalchemy = "2.0.15"
 
 [tool.poetry.group.dev.dependencies]
 bandit = { extras = ["toml"], version = "^1.7.5" }
 behave = "^1.2.6"
 black = "^23.3.0"
 coverage = "^7.2.5"
 flake8 = "^6.0.0"
```

### Comparing `toolcat-0.0.2/src/toolcat/project.py` & `toolcat-0.0.3/src/toolcat/project.py`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.2/src/toolcat/projects_test.py` & `toolcat-0.0.3/src/toolcat/projects_test.py`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.2/PKG-INFO` & `toolcat-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 Metadata-Version: 2.1
 Name: toolcat
-Version: 0.0.2
+Version: 0.0.3
 Summary: Essential Libraries and Tools for Streamlined Development
 License: The Unlicence
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: sqlalchemy (==2.0.15)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Tool Cat
 
 Essential Libraries and Tools for Streamlined Development
 
 ## Requirements
 
 You will need the following installed in your machine.
 
 - [Poetry](https://python-poetry.org)
-- [Poetry Plugin: Export](https://github.com/python-poetry/poetry-plugin-export)
-- [Poetry Plugin: up](https://github.com/MousaZeidBaker/poetry-plugin-up)
-
-## How to update all dependencies
-
-Just run in your project directory:
-
-```bash
- poetry up --pinned --latest
-```
```

