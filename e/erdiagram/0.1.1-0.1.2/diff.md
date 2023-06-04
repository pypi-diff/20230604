# Comparing `tmp/erdiagram-0.1.1.tar.gz` & `tmp/erdiagram-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdiagram-0.1.1.tar", last modified: Mon Oct 10 16:10:20 2022, max compression
+gzip compressed data, was "erdiagram-0.1.2.tar", last modified: Sun Jun  4 19:32:47 2023, max compression
```

## Comparing `erdiagram-0.1.1.tar` & `erdiagram-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     2249 2022-10-10 15:23:20.164763 erdiagram-0.1.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     1196 2022-10-10 15:23:20.164838 erdiagram-0.1.1/.gitignore
--rw-r--r--   0        0        0     1613 2022-10-10 15:23:20.164911 erdiagram-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2022-10-10 15:23:20.165004 erdiagram-0.1.1/LICENSE
--rw-r--r--   0        0        0      101 2022-10-10 15:23:20.165058 erdiagram-0.1.1/README.md
--rw-r--r--   0        0        0       51 2022-10-10 15:23:20.165140 erdiagram-0.1.1/docs/api.md
--rw-r--r--   0        0        0       12 2022-10-10 15:23:20.165192 erdiagram-0.1.1/docs/changelog.md
--rw-r--r--   0        0        0      104 2022-10-10 15:23:20.165248 erdiagram-0.1.1/docs/index.md
--rw-r--r--   0        0        0      448 2022-10-10 15:46:41.635436 erdiagram-0.1.1/erdiagram/__init__.py
--rw-r--r--   0        0        0    16735 2022-10-10 15:44:07.493244 erdiagram-0.1.1/erdiagram/_sqlalchemy.py
--rw-r--r--   0        0        0      317 2022-10-10 15:23:20.165529 erdiagram-0.1.1/erdiagram/_utils.py
--rw-r--r--   0        0        0      153 2022-10-10 15:23:20.165588 erdiagram-0.1.1/lamin-project.yaml
--rw-r--r--   0        0        0      652 2022-10-10 15:23:20.165650 erdiagram-0.1.1/noxfile.py
--rw-r--r--   0        0        0      602 2022-10-10 15:44:07.493602 erdiagram-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4619 2022-10-10 15:23:20.165820 erdiagram-0.1.1/tests/test_schema_graph.py
--rw-r--r--   0        0        0     2937 2022-10-10 15:23:20.165888 erdiagram-0.1.1/tests/test_uml_graph.py
--rw-r--r--   0        0        0      979 2022-10-10 15:23:20.165960 erdiagram-0.1.1/tests/utils.py
--rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 erdiagram-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2249 2023-06-04 19:31:04.419685 erdiagram-0.1.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1196 2023-06-04 19:31:04.419771 erdiagram-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1613 2023-06-04 19:31:04.419846 erdiagram-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-06-04 19:31:04.419964 erdiagram-0.1.2/LICENSE
+-rw-r--r--   0        0        0      146 2023-06-04 19:31:04.420030 erdiagram-0.1.2/README.md
+-rw-r--r--   0        0        0       51 2023-06-04 19:31:04.420113 erdiagram-0.1.2/docs/api.md
+-rw-r--r--   0        0        0       12 2023-06-04 19:31:04.420167 erdiagram-0.1.2/docs/changelog.md
+-rw-r--r--   0        0        0      104 2023-06-04 19:31:04.420226 erdiagram-0.1.2/docs/index.md
+-rw-r--r--   0        0        0      448 2023-06-04 19:32:01.529520 erdiagram-0.1.2/erdiagram/__init__.py
+-rw-r--r--   0        0        0    17998 2023-06-04 19:31:04.420457 erdiagram-0.1.2/erdiagram/_sqlalchemy.py
+-rw-r--r--   0        0        0      317 2023-06-04 19:31:04.420551 erdiagram-0.1.2/erdiagram/_utils.py
+-rw-r--r--   0        0        0      153 2023-06-04 19:31:04.420634 erdiagram-0.1.2/lamin-project.yaml
+-rw-r--r--   0        0        0      652 2023-06-04 19:31:04.420706 erdiagram-0.1.2/noxfile.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:31:04.420771 erdiagram-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4619 2023-06-04 19:31:04.420896 erdiagram-0.1.2/tests/test_schema_graph.py
+-rw-r--r--   0        0        0     2937 2023-06-04 19:31:04.420970 erdiagram-0.1.2/tests/test_uml_graph.py
+-rw-r--r--   0        0        0      979 2023-06-04 19:31:04.421028 erdiagram-0.1.2/tests/utils.py
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 erdiagram-0.1.2/PKG-INFO
```

### Comparing `erdiagram-0.1.1/.github/workflows/build.yml` & `erdiagram-0.1.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `erdiagram-0.1.1/.gitignore` & `erdiagram-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `erdiagram-0.1.1/.pre-commit-config.yaml` & `erdiagram-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `erdiagram-0.1.1/LICENSE` & `erdiagram-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `erdiagram-0.1.1/erdiagram/_sqlalchemy.py` & `erdiagram-0.1.2/erdiagram/_sqlalchemy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,34 @@
-"""Draw diagrams for SQLAlchemy.
+"""Draw diagrams for SQLAlchemy."""
+# This is largely a re-formatted version of `sqlalchemy_schemadisplay`, which is MIT licensed.
 
-This is a re-formatted version of `sqlalchemy_schemadisplay`, which is MIT licensed.
+# The original source code & copyright is available from the link below and after the link:
+# https://github.com/fschulze/sqlalchemy_schemadisplay
+
+# This is the MIT license: http://www.opensource.org/licenses/mit-license.php
+
+# Copyright (c) 2010-2014 Ants Aasma and contributors.
+# SQLAlchemy is a trademark of Michael Bayer.
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this
+# software and associated documentation files (the "Software"), to deal in the Software
+# without restriction, including without limitation the rights to use, copy, modify, merge,
+# publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons
+# to whom the Software is furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all copies or
+# substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
+# INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
+# PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE
+# FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+# OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+# DEALINGS IN THE SOFTWARE.
 
-The original source code & copyright is available from the link below:
-https://github.com/fschulze/sqlalchemy_schemadisplay
-"""
 import types
 
 import pydot
 from sqlalchemy import ForeignKeyConstraint, text
 from sqlalchemy.dialects.postgresql.base import PGDialect
 from sqlalchemy.orm.properties import RelationshipProperty
```

### Comparing `erdiagram-0.1.1/noxfile.py` & `erdiagram-0.1.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `erdiagram-0.1.1/pyproject.toml` & `erdiagram-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 [project]
 name = "erdiagram"
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
-    "nbproject",
     "pydot",
     "sqlalchemy",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/erdiagram"
```

### Comparing `erdiagram-0.1.1/tests/test_schema_graph.py` & `erdiagram-0.1.2/tests/test_schema_graph.py`

 * *Files identical despite different names*

### Comparing `erdiagram-0.1.1/tests/test_uml_graph.py` & `erdiagram-0.1.2/tests/test_uml_graph.py`

 * *Files identical despite different names*

### Comparing `erdiagram-0.1.1/tests/utils.py` & `erdiagram-0.1.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `erdiagram-0.1.1/PKG-INFO` & `erdiagram-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: erdiagram
-Version: 0.1.1
+Version: 0.1.2
 Summary: Make diagrams for SQLAlchemy.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: nbproject
 Requires-Dist: pydot
 Requires-Dist: sqlalchemy
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbmake ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/erdiagram
 Provides-Extra: dev
 Provides-Extra: test
 
 # ERdiagram: Entity relationship diagrams for SQLalchemy
 
-Read the [docs](https://lamin.ai/docs/db).
+This package is heavily based on: https://github.com/fschulze/sqlalchemy_schemadisplay.
```

