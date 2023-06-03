# Comparing `tmp/llm_explorer-0.0.5.tar.gz` & `tmp/llm_explorer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_explorer-0.0.5.tar", last modified: Sat Jun  3 22:31:49 2023, max compression
+gzip compressed data, was "llm_explorer-0.0.6.tar", last modified: Sat Jun  3 23:21:32 2023, max compression
```

## Comparing `llm_explorer-0.0.5.tar` & `llm_explorer-0.0.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.469982 llm_explorer-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/.gitcommit
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/DockerFile
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-03 22:31:49.469982 llm_explorer-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/agents/
--rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/chains/
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/databases/adbddl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/indexes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/indexes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/indexes/vectorstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/interfaces/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/llm/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.469982 llm_explorer-0.0.5/llm_explorer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/templates/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/templates/chains.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/templates/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/templates/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.469982 llm_explorer-0.0.5/llm_explorer/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/ui/lang.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.469982 llm_explorer-0.0.5/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/pages/pandas_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/pip.conf
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-03 22:31:49.469982 llm_explorer-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/.gitcommit
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/DockerFile
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.749652 llm_explorer-0.0.6/llm_explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/databases/adbddl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/indexes/vectorstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/interfaces/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/templates/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/templates/chains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/templates/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/templates/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/ui/lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/pages/pandas_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/pip.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/setup.py
```

### Comparing `llm_explorer-0.0.5/.gitignore` & `llm_explorer-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/CODE_OF_CONDUCT.md` & `llm_explorer-0.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/CONTRIBUTING.rst` & `llm_explorer-0.0.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/LICENSE` & `llm_explorer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/Makefile` & `llm_explorer-0.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/PKG-INFO` & `llm_explorer-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_explorer
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes
 Home-page: https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm_explorer-0.0.5/README.md` & `llm_explorer-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/SECURITY.md` & `llm_explorer-0.0.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/__init__.py` & `llm_explorer-0.0.6/llm_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/agents/__init__.py` & `llm_explorer-0.0.6/llm_explorer/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/chains/__init__.py` & `llm_explorer-0.0.6/llm_explorer/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/chat/__init__.py` & `llm_explorer-0.0.6/llm_explorer/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/databases/adbddl.py` & `llm_explorer-0.0.6/llm_explorer/databases/adbddl.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/indexes/vectorstore.py` & `llm_explorer-0.0.6/llm_explorer/indexes/vectorstore.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/interfaces/frontend.py` & `llm_explorer-0.0.6/llm_explorer/interfaces/frontend.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/llm/__init__.py` & `llm_explorer-0.0.6/llm_explorer/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/templates/agents.py` & `llm_explorer-0.0.6/llm_explorer/templates/agents.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/templates/chains.py` & `llm_explorer-0.0.6/llm_explorer/templates/chains.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/templates/prompt.py` & `llm_explorer-0.0.6/llm_explorer/templates/prompt.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/templates/ui.py` & `llm_explorer-0.0.6/llm_explorer/templates/ui.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/ui/__init__.py` & `llm_explorer-0.0.6/llm_explorer/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer/ui/lang.py` & `llm_explorer-0.0.6/llm_explorer/ui/lang.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer.egg-info/PKG-INFO` & `llm_explorer-0.0.6/llm_explorer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-explorer
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes
 Home-page: https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm_explorer-0.0.5/llm_explorer.egg-info/SOURCES.txt` & `llm_explorer-0.0.6/llm_explorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/llm_explorer.egg-info/requires.txt` & `llm_explorer-0.0.6/llm_explorer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/requirements.txt` & `llm_explorer-0.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.5/setup.py` & `llm_explorer-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 version = "#{PKG_VAR_SETUP}#"
 package_name = "llm_explorer"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 if "PKGVARSETUP" in package_env:
-    version = "0.0.5"
+    version = "0.0.6"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 # Check if any letters were found
 if len(package_env) > 0:
     package_name += f"_{package_env}"
 
@@ -68,11 +68,11 @@
     ],
     install_requires=required,
     package_data={
         "": ["*.json"],
     },
     entry_points={
         "console_scripts": [
-            "llm_explorer=llm_explorer:main",
+            "llm_explorer=app:main",
         ],
     },
 )
```

