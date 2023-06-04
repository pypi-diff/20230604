# Comparing `tmp/llm_explorer-0.0.6.tar.gz` & `tmp/llm_explorer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_explorer-0.0.6.tar", last modified: Sat Jun  3 23:21:32 2023, max compression
+gzip compressed data, was "llm_explorer-0.0.7.tar", last modified: Sun Jun  4 06:01:21 2023, max compression
```

## Comparing `llm_explorer-0.0.6.tar` & `llm_explorer-0.0.7.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/.gitcommit
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/DockerFile
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.749652 llm_explorer-0.0.6/llm_explorer/
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/agents/
--rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/chains/
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/databases/adbddl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/indexes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/indexes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/indexes/vectorstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/interfaces/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/llm/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/templates/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/templates/chains.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/templates/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/templates/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/llm_explorer/ui/lang.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/llm_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 23:21:32.000000 llm_explorer-0.0.6/llm_explorer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/pages/pandas_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/pip.conf
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-03 23:21:32.753651 llm_explorer-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-03 23:21:22.000000 llm_explorer-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.065228 llm_explorer-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/.gitcommit
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/DockerFile
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-04 06:01:21.065228 llm_explorer-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.057228 llm_explorer-0.0.7/llm_explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/auth/access.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/databases/adbddl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/indexes/vectorstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/interfaces/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.065228 llm_explorer-0.0.7/llm_explorer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/templates/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/templates/chains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/templates/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/templates/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.065228 llm_explorer-0.0.7/llm_explorer/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/ui/lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.065228 llm_explorer-0.0.7/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/pages/pandas_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/pip.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-04 06:01:21.065228 llm_explorer-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/setup.py
```

### Comparing `llm_explorer-0.0.6/.gitignore` & `llm_explorer-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/CODE_OF_CONDUCT.md` & `llm_explorer-0.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/CONTRIBUTING.rst` & `llm_explorer-0.0.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/LICENSE` & `llm_explorer-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/Makefile` & `llm_explorer-0.0.7/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 SHELL=/bin/bash
 devops_state = main
 working_dir = `pwd`
 datadog_api_key = ""
 
 install: install_python_dependencies
 
+local_build_and_deploy: 
+	pip uninstall llm_explorer -y \
+	&& python setup.py install \
+	&& llm_explorer
+
 package_build:
 	python -m build
 
 package_list:
 	unzip -l dist/*.whl  
 
 set_env:
```

### Comparing `llm_explorer-0.0.6/PKG-INFO` & `llm_explorer-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_explorer
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes
 Home-page: https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm_explorer-0.0.6/README.md` & `llm_explorer-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/SECURITY.md` & `llm_explorer-0.0.7/SECURITY.md`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer/__init__.py` & `llm_explorer-0.0.7/llm_explorer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 PAGE_ICON: str = "🤖🎯"
 LANG_EN: str = "En"
 LANG_RU: str = "Ru"
 LANG_ES: str = "Es"
 
 import streamlit as st
 
-from .ui import about
+from llm_explorer.ui import about
 
 st.set_page_config(
     page_title=PAGE_TITLE,
     page_icon=PAGE_ICON,
     layout="centered",
     initial_sidebar_state="auto",
     menu_items={
@@ -20,18 +20,18 @@
     },
 )
 
 from pathlib import Path
 
 from dotenv import find_dotenv, load_dotenv
 
-from .chains import ExplorerConversationChain
-from .chat import chat_loop
-from .interfaces import frontend as it
-from .ui.lang import en, es
+from llm_explorer.chains import ExplorerConversationChain
+from llm_explorer.chat import chat_loop
+from llm_explorer.interfaces import frontend as it
+from llm_explorer.ui.lang import en, es
 
 
 def auth():
     import streamlit_authenticator as stauth
     import yaml
     from yaml.loader import SafeLoader
```

### Comparing `llm_explorer-0.0.6/llm_explorer/agents/__init__.py` & `llm_explorer-0.0.7/llm_explorer/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer/chains/__init__.py` & `llm_explorer-0.0.7/llm_explorer/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer/chat/__init__.py` & `llm_explorer-0.0.7/llm_explorer/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer/databases/adbddl.py` & `llm_explorer-0.0.7/llm_explorer/databases/adbddl.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer/indexes/vectorstore.py` & `llm_explorer-0.0.7/llm_explorer/indexes/vectorstore.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer/interfaces/frontend.py` & `llm_explorer-0.0.7/llm_explorer/interfaces/frontend.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer/llm/__init__.py` & `llm_explorer-0.0.7/llm_explorer/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer/templates/agents.py` & `llm_explorer-0.0.7/llm_explorer/templates/agents.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer/templates/chains.py` & `llm_explorer-0.0.7/llm_explorer/templates/chains.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer/templates/prompt.py` & `llm_explorer-0.0.7/llm_explorer/templates/prompt.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer/templates/ui.py` & `llm_explorer-0.0.7/llm_explorer/templates/ui.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer/ui/__init__.py` & `llm_explorer-0.0.7/llm_explorer/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer/ui/lang.py` & `llm_explorer-0.0.7/llm_explorer/ui/lang.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/llm_explorer.egg-info/PKG-INFO` & `llm_explorer-0.0.7/llm_explorer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-explorer
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes
 Home-page: https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm_explorer-0.0.6/llm_explorer.egg-info/SOURCES.txt` & `llm_explorer-0.0.7/llm_explorer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 CONTRIBUTING.rst
 DockerFile
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 SECURITY.md
-app.py
 main.py
 package.json
 pip.conf
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 llm_explorer/__init__.py
+llm_explorer/app.py
 llm_explorer.egg-info/PKG-INFO
 llm_explorer.egg-info/SOURCES.txt
 llm_explorer.egg-info/dependency_links.txt
 llm_explorer.egg-info/entry_points.txt
 llm_explorer.egg-info/not-zip-safe
 llm_explorer.egg-info/requires.txt
 llm_explorer.egg-info/top_level.txt
 llm_explorer/agents/__init__.py
 llm_explorer/auth/__init__.py
+llm_explorer/auth/access.yaml
 llm_explorer/chains/__init__.py
 llm_explorer/chat/__init__.py
 llm_explorer/databases/__init__.py
 llm_explorer/databases/adbddl.py
 llm_explorer/indexes/__init__.py
 llm_explorer/indexes/vectorstore.py
 llm_explorer/interfaces/__init__.py
```

### Comparing `llm_explorer-0.0.6/llm_explorer.egg-info/requires.txt` & `llm_explorer-0.0.7/llm_explorer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/requirements.txt` & `llm_explorer-0.0.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.6/setup.py` & `llm_explorer-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 version = "#{PKG_VAR_SETUP}#"
 package_name = "llm_explorer"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 if "PKGVARSETUP" in package_env:
-    version = "0.0.6"
+    version = "0.0.7"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 # Check if any letters were found
 if len(package_env) > 0:
     package_name += f"_{package_env}"
 
@@ -64,15 +64,16 @@
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.10",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     install_requires=required,
     package_data={
-        "": ["*.json"],
+        "": ["*.json", "*.yaml", ".sql", ".csv", ".txt", ".md", ".html", ".css"],
     },
+    py_modules=['main'],
     entry_points={
         "console_scripts": [
-            "llm_explorer=app:main",
+            "llm_explorer=main:main",
         ],
     },
 )
```

