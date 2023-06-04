# Comparing `tmp/awschains-0.0.2.tar.gz` & `tmp/awschains-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awschains-0.0.2.tar", last modified: Sun May 28 01:17:24 2023, max compression
+gzip compressed data, was "awschains-0.0.3.tar", last modified: Sun Jun  4 12:47:15 2023, max compression
```

## Comparing `awschains-0.0.2.tar` & `awschains-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:17:24.823674 awschains-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:17:24.819674 awschains-0.0.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-28 01:17:15.000000 awschains-0.0.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-28 01:17:15.000000 awschains-0.0.2/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-28 01:17:15.000000 awschains-0.0.2/.devcontainer/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:17:24.815674 awschains-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:17:24.819674 awschains-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-28 01:17:15.000000 awschains-0.0.2/.github/workflows/pre-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-28 01:17:15.000000 awschains-0.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-28 01:17:15.000000 awschains-0.0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-28 01:17:15.000000 awschains-0.0.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:17:24.819674 awschains-0.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-28 01:17:15.000000 awschains-0.0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 01:17:15.000000 awschains-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-05-28 01:17:24.823674 awschains-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-28 01:17:15.000000 awschains-0.0.2/README.ja.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-28 01:17:15.000000 awschains-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-28 01:17:15.000000 awschains-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-28 01:17:15.000000 awschains-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 01:17:24.823674 awschains-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:17:24.815674 awschains-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:17:24.819674 awschains-0.0.2/src/awschains/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-28 01:17:24.000000 awschains-0.0.2/src/awschains/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-28 01:17:15.000000 awschains-0.0.2/src/awschains/dynamochain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:17:24.819674 awschains-0.0.2/src/awschains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-05-28 01:17:24.000000 awschains-0.0.2/src/awschains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-28 01:17:24.000000 awschains-0.0.2/src/awschains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 01:17:24.000000 awschains-0.0.2/src/awschains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-28 01:17:24.000000 awschains-0.0.2/src/awschains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-28 01:17:24.000000 awschains-0.0.2/src/awschains.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:17:24.819674 awschains-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-28 01:17:15.000000 awschains-0.0.2/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:17:24.819674 awschains-0.0.2/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-28 01:17:15.000000 awschains-0.0.2/test/data/expected_delete.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-28 01:17:15.000000 awschains-0.0.2/test/data/expected_get.json
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-28 01:17:15.000000 awschains-0.0.2/test/data/expected_query1.json
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-28 01:17:15.000000 awschains-0.0.2/test/data/expected_query2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-28 01:17:15.000000 awschains-0.0.2/test/data/expected_scan.json
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-28 01:17:15.000000 awschains-0.0.2/test/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:17:24.819674 awschains-0.0.2/test/database/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-28 01:17:15.000000 awschains-0.0.2/test/database/database.json
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-28 01:17:15.000000 awschains-0.0.2/test/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:47:15.197044 awschains-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:47:15.193044 awschains-0.0.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-04 12:47:03.000000 awschains-0.0.3/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-04 12:47:03.000000 awschains-0.0.3/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-04 12:47:03.000000 awschains-0.0.3/.devcontainer/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:47:15.193044 awschains-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:47:15.193044 awschains-0.0.3/.github/workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-06-04 12:47:03.000000 awschains-0.0.3/.github/workflows/guard_branch.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-04 12:47:03.000000 awschains-0.0.3/.github/workflows/pre-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-04 12:47:03.000000 awschains-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-04 12:47:03.000000 awschains-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-04 12:47:03.000000 awschains-0.0.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:47:15.193044 awschains-0.0.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-04 12:47:03.000000 awschains-0.0.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 12:47:03.000000 awschains-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-06-04 12:47:15.197044 awschains-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-04 12:47:03.000000 awschains-0.0.3/README.ja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-04 12:47:03.000000 awschains-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-04 12:47:03.000000 awschains-0.0.3/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-04 12:47:03.000000 awschains-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-04 12:47:03.000000 awschains-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 12:47:15.197044 awschains-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:47:15.193044 awschains-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:47:15.193044 awschains-0.0.3/src/awschains/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 12:47:15.000000 awschains-0.0.3/src/awschains/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-04 12:47:03.000000 awschains-0.0.3/src/awschains/dynamochain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:47:15.197044 awschains-0.0.3/src/awschains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-06-04 12:47:15.000000 awschains-0.0.3/src/awschains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-04 12:47:15.000000 awschains-0.0.3/src/awschains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:47:15.000000 awschains-0.0.3/src/awschains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-04 12:47:15.000000 awschains-0.0.3/src/awschains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-04 12:47:15.000000 awschains-0.0.3/src/awschains.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:47:15.197044 awschains-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-04 12:47:03.000000 awschains-0.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:47:15.197044 awschains-0.0.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-04 12:47:03.000000 awschains-0.0.3/tests/data/expected_delete1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-04 12:47:03.000000 awschains-0.0.3/tests/data/expected_get.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-04 12:47:03.000000 awschains-0.0.3/tests/data/expected_put1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-04 12:47:03.000000 awschains-0.0.3/tests/data/expected_put2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-04 12:47:03.000000 awschains-0.0.3/tests/data/expected_put3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-04 12:47:03.000000 awschains-0.0.3/tests/data/expected_query1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-04 12:47:03.000000 awschains-0.0.3/tests/data/expected_query2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-04 12:47:03.000000 awschains-0.0.3/tests/data/expected_scan1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-04 12:47:03.000000 awschains-0.0.3/tests/data/expected_scan2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-04 12:47:03.000000 awschains-0.0.3/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:47:15.197044 awschains-0.0.3/tests/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-04 12:47:03.000000 awschains-0.0.3/tests/database/database.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-06-04 12:47:03.000000 awschains-0.0.3/tests/test_wrapper.py
```

### Comparing `awschains-0.0.2/.github/workflows/pre-release.yml` & `awschains-0.0.3/.github/workflows/release.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-name: Pre Release
+name: Release
 
 on:
   push:
     tags:
-      - "v[0-9]+.[0-9]+.[0-9]+.beta.[0-9]+"
+      - "v[0-9]+.[0-9]+.[0-9]+"
 
   workflow_dispatch:
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+
+      - name: Check tagged branch
+        working-directory: .github/workflows
+        run: ./guard_branch.sh production ${{ github.ref_name }}
 
       - name: Build module
         run: |
           pip install build
           python -m build
 
-      - name: Publish package distributions to TestPyPI
+      - name: Publish package distributions to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-          repository-url: https://test.pypi.org/legacy/
+          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `awschains-0.0.2/.gitignore` & `awschains-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `awschains-0.0.2/LICENSE` & `awschains-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `awschains-0.0.2/PKG-INFO` & `awschains-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awschains
-Version: 0.0.2
+Version: 0.0.3
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
```

### Comparing `awschains-0.0.2/README.ja.md` & `awschains-0.0.3/README.ja.md`

 * *Files identical despite different names*

### Comparing `awschains-0.0.2/README.md` & `awschains-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `awschains-0.0.2/pyproject.toml` & `awschains-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `awschains-0.0.2/requirements.txt` & `awschains-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `awschains-0.0.2/src/awschains/dynamochain.py` & `awschains-0.0.3/src/awschains/dynamochain.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import operator
-
+from conditions import ChainsConditionBuilder
 
 class DynamoChain:
     def __init__(self, table) -> None:
         self._table = table
         self._query = {}
         self._operator = operator.and_
 
@@ -67,48 +67,68 @@
             self._query["Key"] = {key: value}
         return self
 
     def consistent_read(self, cr=True):
         self._query["ConsistentRead"] = cr
         return self
 
+    def projection(self, pe):
+        if "ProjectionExpression" in self._query:
+            self._query["ProjectionExpression"] += ',' + pe
+        else:
+            self._query["ProjectionExpression"] = pe
+        return self
+
+    def condition(self, ce):
+        if "ConditionExpression" in self._query:
+            self._query["ConditionExpression"] = self._operator(
+                self._query["ConditionExpression"], ce
+            )
+        else:
+            self._query["ConditionExpression"] = ce
+        return self
+
     # Last Method
     def count(self):
         self._query["Select"] = "COUNT"
-        resp = self._table.scan(**self._query)
+        resp = self._table.scan(**ChainsConditionBuilder(self._query).query)
         self._check_next_query(resp)
         count = resp["Count"]
         return count
 
     def count_all(self):
         resp = self.count()
         while not self.done:
             resp += self.count()
         return resp
 
     def scan(self):
-        resp = self._table.scan(**self._query)
+        resp = self._table.scan(**ChainsConditionBuilder(self._query).query)
         self._check_next_query(resp)
         return resp["Items"]
 
     def scan_all(self):
         resp = self.scan()
         while not self.done:
             resp += self.scan()
         return resp
 
     def query(self):
-        resp = self._table.query(**self._query)
+        resp = self._table.query(**ChainsConditionBuilder(self._query).query)
         self._check_next_query(resp)
         return resp["Items"]
 
     def query_all(self):
         resp = self.query()
         while not self.done:
             resp += self.query()
         return resp
 
     def delete(self):
-        self._table.delete_item(**self._query)
+        self._table.delete_item(**ChainsConditionBuilder(self._query).query)
 
     def get(self):
-        return self._table.get_item(**self._query)["Item"]
+        return self._table.get_item(**ChainsConditionBuilder(self._query).query)["Item"]
+
+    def put(self, item):
+        self._query["Item"] = item
+        self._table.put_item(**ChainsConditionBuilder(self._query).query)
```

### Comparing `awschains-0.0.2/src/awschains.egg-info/PKG-INFO` & `awschains-0.0.3/src/awschains.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awschains
-Version: 0.0.2
+Version: 0.0.3
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
```

### Comparing `awschains-0.0.2/src/awschains.egg-info/SOURCES.txt` & `awschains-0.0.3/src/awschains.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 .gitignore
 LICENSE
 README.ja.md
 README.md
+conditions.py
 pyproject.toml
 requirements.txt
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .devcontainer/docker-compose.yml
+.github/workflows/guard_branch.sh
 .github/workflows/pre-release.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
 .vscode/settings.json
 src/awschains/_version.py
 src/awschains/dynamochain.py
 src/awschains.egg-info/PKG-INFO
 src/awschains.egg-info/SOURCES.txt
 src/awschains.egg-info/dependency_links.txt
 src/awschains.egg-info/requires.txt
 src/awschains.egg-info/top_level.txt
-test/conftest.py
-test/data.py
-test/test_wrapper.py
-test/data/expected_delete.json
-test/data/expected_get.json
-test/data/expected_query1.json
-test/data/expected_query2.json
-test/data/expected_scan.json
-test/database/database.json
+tests/conftest.py
+tests/data.py
+tests/test_wrapper.py
+tests/data/expected_delete1.json
+tests/data/expected_get.json
+tests/data/expected_put1.json
+tests/data/expected_put2.json
+tests/data/expected_put3.json
+tests/data/expected_query1.json
+tests/data/expected_query2.json
+tests/data/expected_scan1.json
+tests/data/expected_scan2.json
+tests/database/database.json
```

### Comparing `awschains-0.0.2/test/data/expected_delete.json` & `awschains-0.0.3/tests/data/expected_delete1.json`

 * *Files identical despite different names*

### Comparing `awschains-0.0.2/test/data/expected_query1.json` & `awschains-0.0.3/tests/data/expected_query1.json`

 * *Files identical despite different names*

### Comparing `awschains-0.0.2/test/data/expected_scan.json` & `awschains-0.0.3/tests/data/expected_scan1.json`

 * *Files identical despite different names*

### Comparing `awschains-0.0.2/test/data.py` & `awschains-0.0.3/tests/data.py`

 * *Files identical despite different names*

### Comparing `awschains-0.0.2/test/database/database.json` & `awschains-0.0.3/tests/database/database.json`

 * *Files identical despite different names*

