# Comparing `tmp/llm_explorer-0.0.4.tar.gz` & `tmp/llm_explorer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_explorer-0.0.4.tar", last modified: Sat Jun  3 16:56:06 2023, max compression
+gzip compressed data, was "llm_explorer-0.0.5.tar", last modified: Sat Jun  3 22:31:49 2023, max compression
```

## Comparing `llm_explorer-0.0.4.tar` & `llm_explorer-0.0.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.082532 llm_explorer-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/.gitcommit
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/DockerFile
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-03 16:56:06.082532 llm_explorer-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.074532 llm_explorer-0.0.4/llm_explorer/
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/agents/
--rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/chains/
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/databases/adbddl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/indexes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/indexes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/indexes/vectorstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/interfaces/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/llm/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/templates/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/templates/chains.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/templates/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/templates/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.082532 llm_explorer-0.0.4/llm_explorer/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/llm_explorer/ui/lang.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.078532 llm_explorer-0.0.4/llm_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 16:56:06.000000 llm_explorer-0.0.4/llm_explorer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:56:06.082532 llm_explorer-0.0.4/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/pages/pandas_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/pip.conf
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-03 16:56:06.082532 llm_explorer-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 16:55:53.000000 llm_explorer-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.469982 llm_explorer-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/.gitcommit
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/DockerFile
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-03 22:31:49.469982 llm_explorer-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/databases/adbddl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/indexes/vectorstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/interfaces/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.469982 llm_explorer-0.0.5/llm_explorer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/templates/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/templates/chains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/templates/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/templates/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.469982 llm_explorer-0.0.5/llm_explorer/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/llm_explorer/ui/lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.465982 llm_explorer-0.0.5/llm_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 22:31:49.000000 llm_explorer-0.0.5/llm_explorer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:49.469982 llm_explorer-0.0.5/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/pages/pandas_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/pip.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-03 22:31:49.469982 llm_explorer-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 22:31:38.000000 llm_explorer-0.0.5/setup.py
```

### Comparing `llm_explorer-0.0.4/.gitignore` & `llm_explorer-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/CODE_OF_CONDUCT.md` & `llm_explorer-0.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/CONTRIBUTING.rst` & `llm_explorer-0.0.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/LICENSE` & `llm_explorer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/Makefile` & `llm_explorer-0.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/README.md` & `llm_explorer-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,37 @@
+Metadata-Version: 2.1
+Name: llm_explorer
+Version: 0.0.5
+Summary: A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes
+Home-page: https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git
+Author: Carlos D. Escobar-Valbuena
+Author-email: carlosdavidescobar@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Occlusion LLM Explorer
 
 [![CodeQL](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/github-code-scanning/codeql) [![python-ci](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-ci.yml/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-ci.yml) [![python-cd](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-cd.yml/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-cd.yml) [![PyPI version](https://badge.fury.io/py/llm-explorer.svg)](https://badge.fury.io/py/llm-explorer)
 
 
 **Lakehouse Analytics &amp; Advanced ML**
-![llm_explorer_sample.png](/docs/.attachments/llm_explorer_sample.png)
+![llm_explorer_sample](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/assets/11726633/f6a5753d-681c-418f-babb-0a2df74dd4d8)
 
 ## Setup
 **Important** This package requires **Open AI & HuggingFace API key**
 
-### Pypi
+### PyPi
 ```shell
 python -m pip install llm-explorer
 ```
 
 ```shell
 touch main.py
 ```
@@ -81,47 +99,30 @@
 
 Agent is queried for the top 10 producing wells. It identifies the tables it has access to and understands that the request could be satified by the padalloc table. It then creates a query that returns the top 10 producing assets and return the results.
 
 ```shell
 
 > Entering new AgentExecutor chain...
 
-Observation: microchip_logs, padalloc
+Observation: logs, wells
 Thought: I should look at the schema of the microchip_logs and padalloc tables to see what columns I can use.
 
 Action: schema_sql_db
-Action Input: "microchip_logs, padalloc"
-Observation: 
-CREATE TABLE `microchip_logs` (
-        `file_path` STRING, 
-        `content` STRING
-)
-
-
-CREATE TABLE `padalloc` (
-        `ZONE_CODE` STRING, 
-        `ZONE_NAME` STRING, 
-        `ZONE_HID` DECIMAL, 
-        `WELL_HID` DECIMAL, 
-        `WELL_CODE` STRING, 
-        `PROD_DATE` TIMESTAMP, 
-        `PROD_GAS_VOLUME_MCF` DECIMAL, 
-        `PROD_OIL_VOLUME_BBL` DECIMAL, 
-        `PROD_WATER_VOLUME_BBL` DECIMAL, 
-        `ALLOCATED_FLAG` STRING, 
-        `SALE_GAS_VOLUME_MCF` DECIMAL, 
-        `SALE_OIL_VOLUME_BBL` DECIMAL, 
-        `LGL_VOLUME_MCF` DECIMAL, 
-        `OTHER_USES_GAS_MCF` DECIMAL
-)
-
+Action Input: "wells"
+Observation: DDL
 Thought: I should query the padalloc table to get the top 10 producing wells.
 
 Action: query_sql_db
 Action Input: "SELECT WELL_CODE, SUM(PROD_GAS_VOLUME_MCF) AS total_gas_volume_mcf FROM padalloc GROUP BY WELL_CODE ORDER BY total_gas_volume_mcf DESC LIMIT 10"
-Observation: [('1222344             ', Decimal('8429191.6172')), ('1212560             ', Decimal('8211108.4867')), ('1222345             ', Decimal('8163411.9976')), ('1212503             ', Decimal('6621501.8683')), ('1222335             ', Decimal('4773668.6216')), ('1222340             ', Decimal('4276560.8228')), ('1222338             ', Decimal('4153258.1434')), ('1222367             ', Decimal('4018012.2406')), ('1220189             ', Decimal('3965394.4453')), ('1222352             ', Decimal('3786076.4127'))]
+Observation: results_dataframe
 Thought: I now know the top 10 producing wells.
 
 Final Answer: The top 10 producing wells are 1222344, 1212560, 1222345, 1212503, 1222335, 1222340, 1222338, 1222367, 1220189, and 1222352.
 
 > Finished chain.
-```
+```
+
+## Attribution
+
+This is an adapted implementation from the GitHub repository. See the contibutions list for more details:
+
+https://github.com/kaarthik108/snowChat
```

### Comparing `llm_explorer-0.0.4/SECURITY.md` & `llm_explorer-0.0.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/__init__.py` & `llm_explorer-0.0.5/llm_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/agents/__init__.py` & `llm_explorer-0.0.5/llm_explorer/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/chains/__init__.py` & `llm_explorer-0.0.5/llm_explorer/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/chat/__init__.py` & `llm_explorer-0.0.5/llm_explorer/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/databases/adbddl.py` & `llm_explorer-0.0.5/llm_explorer/databases/adbddl.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/indexes/vectorstore.py` & `llm_explorer-0.0.5/llm_explorer/indexes/vectorstore.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/interfaces/frontend.py` & `llm_explorer-0.0.5/llm_explorer/interfaces/frontend.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/llm/__init__.py` & `llm_explorer-0.0.5/llm_explorer/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/templates/agents.py` & `llm_explorer-0.0.5/llm_explorer/templates/agents.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/templates/chains.py` & `llm_explorer-0.0.5/llm_explorer/templates/chains.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/templates/prompt.py` & `llm_explorer-0.0.5/llm_explorer/templates/prompt.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/templates/ui.py` & `llm_explorer-0.0.5/llm_explorer/templates/ui.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/ui/__init__.py` & `llm_explorer-0.0.5/llm_explorer/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer/ui/lang.py` & `llm_explorer-0.0.5/llm_explorer/ui/lang.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer.egg-info/SOURCES.txt` & `llm_explorer-0.0.5/llm_explorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/llm_explorer.egg-info/requires.txt` & `llm_explorer-0.0.5/llm_explorer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/requirements.txt` & `llm_explorer-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.4/setup.py` & `llm_explorer-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 version = "#{PKG_VAR_SETUP}#"
 package_name = "llm_explorer"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 if "PKGVARSETUP" in package_env:
-    version = "0.0.4"
+    version = "0.0.5"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 # Check if any letters were found
 if len(package_env) > 0:
     package_name += f"_{package_env}"
```

