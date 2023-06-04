# Comparing `tmp/silverback-0.1.0a1.tar.gz` & `tmp/silverback-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverback-0.1.0a1.tar", last modified: Sat Feb 11 18:58:37 2023, max compression
+gzip compressed data, was "silverback-0.1.0b1.tar", last modified: Sun Jun  4 21:51:02 2023, max compression
```

## Comparing `silverback-0.1.0a1.tar` & `silverback-0.1.0b1.tar`

### file list

```diff
@@ -1,38 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 18:58:37.785502 silverback-0.1.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 18:58:37.785502 silverback-0.1.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 18:58:37.785502 silverback-0.1.0a1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 18:58:37.785502 silverback-0.1.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-02-11 18:57:43.000000 silverback-0.1.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-02-11 18:57:43.000000 silverback-0.1.0a1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-02-11 18:57:43.000000 silverback-0.1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-02-11 18:58:37.785502 silverback-0.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-02-11 18:57:43.000000 silverback-0.1.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-11 18:57:43.000000 silverback-0.1.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-11 18:58:37.785502 silverback-0.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-02-11 18:57:43.000000 silverback-0.1.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 18:58:37.785502 silverback-0.1.0a1/silverback/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-11 18:57:43.000000 silverback-0.1.0a1/silverback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 18:57:43.000000 silverback-0.1.0a1/silverback/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-11 18:58:37.000000 silverback-0.1.0a1/silverback/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 18:58:37.785502 silverback-0.1.0a1/silverback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-02-11 18:58:37.000000 silverback-0.1.0a1/silverback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-11 18:58:37.000000 silverback-0.1.0a1/silverback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 18:58:37.000000 silverback-0.1.0a1/silverback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 18:58:37.000000 silverback-0.1.0a1/silverback.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-11 18:58:37.000000 silverback-0.1.0a1/silverback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-11 18:58:37.000000 silverback-0.1.0a1/silverback.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 18:58:37.785502 silverback-0.1.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 18:57:43.000000 silverback-0.1.0a1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:51:02.301558 silverback-0.1.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:51:02.297558 silverback-0.1.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:51:02.297558 silverback-0.1.0b1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:51:02.301558 silverback-0.1.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-04 21:49:56.000000 silverback-0.1.0b1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-04 21:49:56.000000 silverback-0.1.0b1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-04 21:49:56.000000 silverback-0.1.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-04 21:51:02.301558 silverback-0.1.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-04 21:49:56.000000 silverback-0.1.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-04 21:49:56.000000 silverback-0.1.0b1/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-04 21:49:56.000000 silverback-0.1.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-04 21:51:02.301558 silverback-0.1.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-04 21:49:56.000000 silverback-0.1.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:51:02.301558 silverback-0.1.0b1/silverback/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-04 21:49:56.000000 silverback-0.1.0b1/silverback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-04 21:49:56.000000 silverback-0.1.0b1/silverback/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-04 21:49:56.000000 silverback-0.1.0b1/silverback/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-04 21:49:56.000000 silverback-0.1.0b1/silverback/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-04 21:49:56.000000 silverback-0.1.0b1/silverback/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-04 21:49:56.000000 silverback-0.1.0b1/silverback/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 21:49:56.000000 silverback-0.1.0b1/silverback/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-04 21:49:56.000000 silverback-0.1.0b1/silverback/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-04 21:49:56.000000 silverback-0.1.0b1/silverback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-04 21:49:56.000000 silverback-0.1.0b1/silverback/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-04 21:51:01.000000 silverback-0.1.0b1/silverback/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:51:02.301558 silverback-0.1.0b1/silverback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-04 21:51:01.000000 silverback-0.1.0b1/silverback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-04 21:51:02.000000 silverback-0.1.0b1/silverback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:51:01.000000 silverback-0.1.0b1/silverback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-04 21:51:01.000000 silverback-0.1.0b1/silverback.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:51:01.000000 silverback-0.1.0b1/silverback.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-04 21:51:01.000000 silverback-0.1.0b1/silverback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 21:51:01.000000 silverback-0.1.0b1/silverback.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:51:02.301558 silverback-0.1.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 21:49:56.000000 silverback-0.1.0b1/tests/__init__.py
```

### Comparing `silverback-0.1.0a1/.github/ISSUE_TEMPLATE/bug.md` & `silverback-0.1.0b1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/.github/ISSUE_TEMPLATE/feature.md` & `silverback-0.1.0b1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/.github/ISSUE_TEMPLATE/work-item.md` & `silverback-0.1.0b1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/.github/release-drafter.yml` & `silverback-0.1.0b1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/.github/workflows/codeql.yaml` & `silverback-0.1.0b1/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/.github/workflows/commitlint.yaml` & `silverback-0.1.0b1/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/.github/workflows/prtitle.yaml` & `silverback-0.1.0b1/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/.github/workflows/publish.yaml` & `silverback-0.1.0b1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/.github/workflows/test.yaml` & `silverback-0.1.0b1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/.gitignore` & `silverback-0.1.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/.pre-commit-config.yaml` & `silverback-0.1.0b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/CONTRIBUTING.md` & `silverback-0.1.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/LICENSE` & `silverback-0.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/PKG-INFO` & `silverback-0.1.0b1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.1.0a1
+Version: 0.1.0b1
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/SilverBackLtd/sdk
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
         
@@ -32,15 +32,21 @@
         git clone https://github.com/SilverBackLtd/sdk.git silverback
         cd silverback
         python3 setup.py install
         ```
         
         ## Quick Usage
         
-        TODO: Describe library overview in code
+        Checkout [the example](./example.py) to see how to use the library.
+        
+        To run your bot against a live network, this SDK includes a simple runner you can use via:
+        
+        ```sh
+        $ silverback run "example:app" --network :mainnet:alchemy
+        ```
         
         ## Development
         
         This project is in development and should be considered a beta.
         Things might not be in their final state and breaking changes may occur.
         Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `silverback-0.1.0a1/README.md` & `silverback-0.1.0b1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 git clone https://github.com/SilverBackLtd/sdk.git silverback
 cd silverback
 python3 setup.py install
 ```
 
 ## Quick Usage
 
-TODO: Describe library overview in code
+Checkout [the example](./example.py) to see how to use the library.
+
+To run your bot against a live network, this SDK includes a simple runner you can use via:
+
+```sh
+$ silverback run "example:app" --network :mainnet:alchemy
+```
 
 ## Development
 
 This project is in development and should be considered a beta.
 Things might not be in their final state and breaking changes may occur.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `silverback-0.1.0a1/pyproject.toml` & `silverback-0.1.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silverback-0.1.0a1/setup.py` & `silverback-0.1.0b1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,19 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/SilverBackLtd/sdk",
     include_package_data=True,
     install_requires=[
         "eth-ape>=0.6.0,<1.0",
+        "taskiq[metrics]>=0.6.0,<0.7.0",
     ],
+    entry_points={
+        "console_scripts": ["silverback=silverback._cli:cli"],
+    },
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["silverback"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
```

### Comparing `silverback-0.1.0a1/silverback.egg-info/PKG-INFO` & `silverback-0.1.0b1/silverback.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.1.0a1
+Version: 0.1.0b1
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/SilverBackLtd/sdk
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
         
@@ -32,15 +32,21 @@
         git clone https://github.com/SilverBackLtd/sdk.git silverback
         cd silverback
         python3 setup.py install
         ```
         
         ## Quick Usage
         
-        TODO: Describe library overview in code
+        Checkout [the example](./example.py) to see how to use the library.
+        
+        To run your bot against a live network, this SDK includes a simple runner you can use via:
+        
+        ```sh
+        $ silverback run "example:app" --network :mainnet:alchemy
+        ```
         
         ## Development
         
         This project is in development and should be considered a beta.
         Things might not be in their final state and breaking changes may occur.
         Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `silverback-0.1.0a1/silverback.egg-info/requires.txt` & `silverback-0.1.0b1/silverback.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 eth-ape<1.0,>=0.6.0
+taskiq[metrics]<0.7.0,>=0.6.0
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 black>=22.12.0
```

