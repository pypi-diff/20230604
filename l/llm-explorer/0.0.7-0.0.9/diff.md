# Comparing `tmp/llm_explorer-0.0.7.tar.gz` & `tmp/llm_explorer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_explorer-0.0.7.tar", last modified: Sun Jun  4 06:01:21 2023, max compression
+gzip compressed data, was "llm_explorer-0.0.9.tar", last modified: Sun Jun  4 07:10:33 2023, max compression
```

## Comparing `llm_explorer-0.0.7.tar` & `llm_explorer-0.0.9.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.065228 llm_explorer-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/.gitcommit
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/DockerFile
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-04 06:01:21.065228 llm_explorer-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.057228 llm_explorer-0.0.7/llm_explorer/
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/agents/
--rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/auth/access.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/chains/
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/databases/adbddl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/indexes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/indexes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/indexes/vectorstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/interfaces/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer/llm/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.065228 llm_explorer-0.0.7/llm_explorer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/templates/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/templates/chains.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/templates/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/templates/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.065228 llm_explorer-0.0.7/llm_explorer/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/llm_explorer/ui/lang.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.061228 llm_explorer-0.0.7/llm_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 06:01:21.000000 llm_explorer-0.0.7/llm_explorer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:21.065228 llm_explorer-0.0.7/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/pages/pandas_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/pip.conf
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-04 06:01:21.065228 llm_explorer-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-04 06:01:10.000000 llm_explorer-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.247287 llm_explorer-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/.gitcommit
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/DockerFile
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-04 07:10:33.247287 llm_explorer-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.243287 llm_explorer-0.0.9/llm_explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.243287 llm_explorer-0.0.9/llm_explorer/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.243287 llm_explorer-0.0.9/llm_explorer/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.243287 llm_explorer-0.0.9/llm_explorer/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.243287 llm_explorer-0.0.9/llm_explorer/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.243287 llm_explorer-0.0.9/llm_explorer/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/databases/adbddl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.247287 llm_explorer-0.0.9/llm_explorer/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/indexes/vectorstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.247287 llm_explorer-0.0.9/llm_explorer/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/interfaces/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.247287 llm_explorer-0.0.9/llm_explorer/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.247287 llm_explorer-0.0.9/llm_explorer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/templates/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/templates/chains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/templates/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/templates/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.247287 llm_explorer-0.0.9/llm_explorer/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/llm_explorer/ui/lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.243287 llm_explorer-0.0.9/llm_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-04 07:10:33.000000 llm_explorer-0.0.9/llm_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-04 07:10:33.000000 llm_explorer-0.0.9/llm_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 07:10:33.000000 llm_explorer-0.0.9/llm_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-04 07:10:33.000000 llm_explorer-0.0.9/llm_explorer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 07:10:33.000000 llm_explorer-0.0.9/llm_explorer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-04 07:10:33.000000 llm_explorer-0.0.9/llm_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 07:10:33.000000 llm_explorer-0.0.9/llm_explorer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:33.247287 llm_explorer-0.0.9/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/pages/pandas_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/pip.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-04 07:10:33.247287 llm_explorer-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-04 07:10:22.000000 llm_explorer-0.0.9/setup.py
```

### Comparing `llm_explorer-0.0.7/.gitignore` & `llm_explorer-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/CODE_OF_CONDUCT.md` & `llm_explorer-0.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/CONTRIBUTING.rst` & `llm_explorer-0.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/LICENSE` & `llm_explorer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/Makefile` & `llm_explorer-0.0.9/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 SHELL=/bin/bash
 devops_state = main
 working_dir = `pwd`
 datadog_api_key = ""
 
-install: install_python_dependencies
+install: local_build_and_deploy
 
 local_build_and_deploy: 
 	pip uninstall llm_explorer -y \
 	&& python setup.py install \
 	&& llm_explorer
 
 package_build:
```

### Comparing `llm_explorer-0.0.7/PKG-INFO` & `llm_explorer-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: llm_explorer
-Version: 0.0.7
+Version: 0.0.9
 Summary: A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes
-Home-page: https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git
+Home-page: https://github.com/Occlusion-Solutions/llm_explorer.git
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,62 +16,74 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Occlusion LLM Explorer
 
 [![CodeQL](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/github-code-scanning/codeql) [![python-ci](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-ci.yml/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-ci.yml) [![python-cd](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-cd.yml/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-cd.yml) [![PyPI version](https://badge.fury.io/py/llm-explorer.svg)](https://badge.fury.io/py/llm-explorer)
 
-
 **Lakehouse Analytics &amp; Advanced ML**
 ![llm_explorer_sample](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/assets/11726633/f6a5753d-681c-418f-babb-0a2df74dd4d8)
 
 ## Setup
-**Important** This package requires **Open AI & HuggingFace API key**
 
-### PyPi
+**Important** This package requires **Open AI & HuggingFace API key**. Remember to run from a folder with the `.streamlit/secrets.toml` file.
+See [here](https://beta.openai.com/docs/developer-quickstart/your-api-keys) and [here](https://huggingface.co/docs/hub/quicktour.html#authentication) for more details.
+
+### Quick Install
+
 ```shell
 python -m pip install llm-explorer
 ```
 
 ```shell
-touch main.py
+llm_explorer
 ```
 
-```python
-from llm_explorer import main
+Initial load could take some time as it downloads the model and the tokenizer. Remember to include the secrets.toml file under .streamlit/ folder.
 
-if __name__ == "__main__":
-    main()
-```
+### Build from source
+
+Clone the repository
 
 ```shell
-python -m streamlit run main.py
+git clone https://github.com/Occlusion-Solutions/llm_explorer.git
 ```
 
-Initial load could take some time as it downloads the model and the tokenizer. Remember to include the secrets.toml file under .streamlit/ folder.
+Install the package
 
+``` shell
+cd llm_explorer && make install
+```
 
-### Build from source
-Create a virtual environment
+Run the package
+
+```shell
+llm_explorer
+```
+
+### Build manaually
+
+After cloning, ceate a virtual environment
 
 ```shell
-conda create -n occlusion python=3.10
-conda activate occlusion
+conda create -n llm_explorer python=3.10
+conda activate llm_explorer
 ```
 
 Install the requirements
 
 ```shell
 pip install -r requirements.txt
 ```
 
-Run the main.py script using streamlit:
+Run the python installation
 
 ```shell
-python -m streamlit run main.py
+python setup.py install
+llm_explorer
 ```
 
 ## Usage
 
 Use the `demo@occlusion.solutions` user and `DEMO@occlusion` password to login.
 
 The deployment requires a secrets.toml file created under .streamlit/:
@@ -91,14 +103,28 @@
 
 [connections.databricks]
 server_hostname="your databricks host"
 http_path="http path under cluster JDBC/ODBC connectivity"
 access_token="your databricks access token"
 ```
 
+## Run Modes
+
+### Chain
+
+An assistant Query engine, that is asked naturally with table references and helps in the query generation. The execution of the queries is manual
+
+### Agent
+
+It uses the pandas agent to generate the queries and execute them. It is a more natural way of querying the data and it operates autonomously until it thinks it finds and answer.
+
+### Chat
+
+It uses the HuggingFace Transformers Agent chat to operate in a conversational way.
+
 ## Lakehouse Agent Sample
 
 Agent is queried for the top 10 producing wells. It identifies the tables it has access to and understands that the request could be satified by the padalloc table. It then creates a query that returns the top 10 producing assets and return the results.
 
 ```shell
 
 > Entering new AgentExecutor chain...
```

### Comparing `llm_explorer-0.0.7/README.md` & `llm_explorer-0.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 # Occlusion LLM Explorer
 
 [![CodeQL](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/github-code-scanning/codeql) [![python-ci](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-ci.yml/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-ci.yml) [![python-cd](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-cd.yml/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-cd.yml) [![PyPI version](https://badge.fury.io/py/llm-explorer.svg)](https://badge.fury.io/py/llm-explorer)
 
-
 **Lakehouse Analytics &amp; Advanced ML**
 ![llm_explorer_sample](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/assets/11726633/f6a5753d-681c-418f-babb-0a2df74dd4d8)
 
 ## Setup
-**Important** This package requires **Open AI & HuggingFace API key**
 
-### PyPi
+**Important** This package requires **Open AI & HuggingFace API key**. Remember to run from a folder with the `.streamlit/secrets.toml` file.
+See [here](https://beta.openai.com/docs/developer-quickstart/your-api-keys) and [here](https://huggingface.co/docs/hub/quicktour.html#authentication) for more details.
+
+### Quick Install
+
 ```shell
 python -m pip install llm-explorer
 ```
 
 ```shell
-touch main.py
+llm_explorer
 ```
 
-```python
-from llm_explorer import main
+Initial load could take some time as it downloads the model and the tokenizer. Remember to include the secrets.toml file under .streamlit/ folder.
 
-if __name__ == "__main__":
-    main()
-```
+### Build from source
+
+Clone the repository
 
 ```shell
-python -m streamlit run main.py
+git clone https://github.com/Occlusion-Solutions/llm_explorer.git
 ```
 
-Initial load could take some time as it downloads the model and the tokenizer. Remember to include the secrets.toml file under .streamlit/ folder.
+Install the package
 
+``` shell
+cd llm_explorer && make install
+```
 
-### Build from source
-Create a virtual environment
+Run the package
+
+```shell
+llm_explorer
+```
+
+### Build manaually
+
+After cloning, ceate a virtual environment
 
 ```shell
-conda create -n occlusion python=3.10
-conda activate occlusion
+conda create -n llm_explorer python=3.10
+conda activate llm_explorer
 ```
 
 Install the requirements
 
 ```shell
 pip install -r requirements.txt
 ```
 
-Run the main.py script using streamlit:
+Run the python installation
 
 ```shell
-python -m streamlit run main.py
+python setup.py install
+llm_explorer
 ```
 
 ## Usage
 
 Use the `demo@occlusion.solutions` user and `DEMO@occlusion` password to login.
 
 The deployment requires a secrets.toml file created under .streamlit/:
@@ -73,14 +85,28 @@
 
 [connections.databricks]
 server_hostname="your databricks host"
 http_path="http path under cluster JDBC/ODBC connectivity"
 access_token="your databricks access token"
 ```
 
+## Run Modes
+
+### Chain
+
+An assistant Query engine, that is asked naturally with table references and helps in the query generation. The execution of the queries is manual
+
+### Agent
+
+It uses the pandas agent to generate the queries and execute them. It is a more natural way of querying the data and it operates autonomously until it thinks it finds and answer.
+
+### Chat
+
+It uses the HuggingFace Transformers Agent chat to operate in a conversational way.
+
 ## Lakehouse Agent Sample
 
 Agent is queried for the top 10 producing wells. It identifies the tables it has access to and understands that the request could be satified by the padalloc table. It then creates a query that returns the top 10 producing assets and return the results.
 
 ```shell
 
 > Entering new AgentExecutor chain...
```

### Comparing `llm_explorer-0.0.7/SECURITY.md` & `llm_explorer-0.0.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer/__init__.py` & `llm_explorer-0.0.9/llm_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer/agents/__init__.py` & `llm_explorer-0.0.9/llm_explorer/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer/chains/__init__.py` & `llm_explorer-0.0.9/llm_explorer/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer/chat/__init__.py` & `llm_explorer-0.0.9/llm_explorer/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer/databases/adbddl.py` & `llm_explorer-0.0.9/llm_explorer/databases/adbddl.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer/indexes/vectorstore.py` & `llm_explorer-0.0.9/llm_explorer/indexes/vectorstore.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,20 +28,20 @@
         }
         vectorstore_strategy = self.kwargs.get("vectorstore", "chroma")
         return set_vectorstore_strategies[vectorstore_strategy]()
 
 
 @st.cache_resource
 def load_chroma_vectorstore():
-    return Chroma(persist_directory="croma_index", embedding_function=embeddings)
+    return Chroma(persist_directory="llm_explorer/indexes/croma_index", embedding_function=embeddings)
 
 
 @st.cache_resource
 def load_faiss_vectorstore():
-    return FAISS.load_local("indexes/faiss_index", embeddings)
+    return FAISS.load_local("llm_explorer/indexes/faiss_index", embeddings)
 
 
 def faiss_metadata_index_loader(
     metadata_path: str = "llm_explorer/indexes/metadata/schema.md",
     page_content_column: str = "y",
 ):
     loader = UnstructuredMarkdownLoader(metadata_path)
```

### Comparing `llm_explorer-0.0.7/llm_explorer/interfaces/frontend.py` & `llm_explorer-0.0.9/llm_explorer/interfaces/frontend.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer/llm/__init__.py` & `llm_explorer-0.0.9/llm_explorer/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer/templates/agents.py` & `llm_explorer-0.0.9/llm_explorer/templates/agents.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer/templates/chains.py` & `llm_explorer-0.0.9/llm_explorer/templates/chains.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer/templates/prompt.py` & `llm_explorer-0.0.9/llm_explorer/templates/prompt.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer/templates/ui.py` & `llm_explorer-0.0.9/llm_explorer/templates/ui.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer/ui/__init__.py` & `llm_explorer-0.0.9/llm_explorer/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer/ui/lang.py` & `llm_explorer-0.0.9/llm_explorer/ui/lang.py`

 * *Files identical despite different names*

### Comparing `llm_explorer-0.0.7/llm_explorer.egg-info/PKG-INFO` & `llm_explorer-0.0.9/llm_explorer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: llm-explorer
-Version: 0.0.7
+Version: 0.0.9
 Summary: A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes
-Home-page: https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git
+Home-page: https://github.com/Occlusion-Solutions/llm_explorer.git
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,62 +16,74 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Occlusion LLM Explorer
 
 [![CodeQL](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/github-code-scanning/codeql) [![python-ci](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-ci.yml/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-ci.yml) [![python-cd](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-cd.yml/badge.svg)](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/actions/workflows/python-cd.yml) [![PyPI version](https://badge.fury.io/py/llm-explorer.svg)](https://badge.fury.io/py/llm-explorer)
 
-
 **Lakehouse Analytics &amp; Advanced ML**
 ![llm_explorer_sample](https://github.com/Occlusion-Solutions/occlussion_llm_explorer/assets/11726633/f6a5753d-681c-418f-babb-0a2df74dd4d8)
 
 ## Setup
-**Important** This package requires **Open AI & HuggingFace API key**
 
-### PyPi
+**Important** This package requires **Open AI & HuggingFace API key**. Remember to run from a folder with the `.streamlit/secrets.toml` file.
+See [here](https://beta.openai.com/docs/developer-quickstart/your-api-keys) and [here](https://huggingface.co/docs/hub/quicktour.html#authentication) for more details.
+
+### Quick Install
+
 ```shell
 python -m pip install llm-explorer
 ```
 
 ```shell
-touch main.py
+llm_explorer
 ```
 
-```python
-from llm_explorer import main
+Initial load could take some time as it downloads the model and the tokenizer. Remember to include the secrets.toml file under .streamlit/ folder.
 
-if __name__ == "__main__":
-    main()
-```
+### Build from source
+
+Clone the repository
 
 ```shell
-python -m streamlit run main.py
+git clone https://github.com/Occlusion-Solutions/llm_explorer.git
 ```
 
-Initial load could take some time as it downloads the model and the tokenizer. Remember to include the secrets.toml file under .streamlit/ folder.
+Install the package
 
+``` shell
+cd llm_explorer && make install
+```
 
-### Build from source
-Create a virtual environment
+Run the package
+
+```shell
+llm_explorer
+```
+
+### Build manaually
+
+After cloning, ceate a virtual environment
 
 ```shell
-conda create -n occlusion python=3.10
-conda activate occlusion
+conda create -n llm_explorer python=3.10
+conda activate llm_explorer
 ```
 
 Install the requirements
 
 ```shell
 pip install -r requirements.txt
 ```
 
-Run the main.py script using streamlit:
+Run the python installation
 
 ```shell
-python -m streamlit run main.py
+python setup.py install
+llm_explorer
 ```
 
 ## Usage
 
 Use the `demo@occlusion.solutions` user and `DEMO@occlusion` password to login.
 
 The deployment requires a secrets.toml file created under .streamlit/:
@@ -91,14 +103,28 @@
 
 [connections.databricks]
 server_hostname="your databricks host"
 http_path="http path under cluster JDBC/ODBC connectivity"
 access_token="your databricks access token"
 ```
 
+## Run Modes
+
+### Chain
+
+An assistant Query engine, that is asked naturally with table references and helps in the query generation. The execution of the queries is manual
+
+### Agent
+
+It uses the pandas agent to generate the queries and execute them. It is a more natural way of querying the data and it operates autonomously until it thinks it finds and answer.
+
+### Chat
+
+It uses the HuggingFace Transformers Agent chat to operate in a conversational way.
+
 ## Lakehouse Agent Sample
 
 Agent is queried for the top 10 producing wells. It identifies the tables it has access to and understands that the request could be satified by the padalloc table. It then creates a query that returns the top 10 producing assets and return the results.
 
 ```shell
 
 > Entering new AgentExecutor chain...
```

### Comparing `llm_explorer-0.0.7/llm_explorer.egg-info/SOURCES.txt` & `llm_explorer-0.0.9/llm_explorer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 llm_explorer.egg-info/dependency_links.txt
 llm_explorer.egg-info/entry_points.txt
 llm_explorer.egg-info/not-zip-safe
 llm_explorer.egg-info/requires.txt
 llm_explorer.egg-info/top_level.txt
 llm_explorer/agents/__init__.py
 llm_explorer/auth/__init__.py
-llm_explorer/auth/access.yaml
 llm_explorer/chains/__init__.py
 llm_explorer/chat/__init__.py
 llm_explorer/databases/__init__.py
 llm_explorer/databases/adbddl.py
 llm_explorer/indexes/__init__.py
 llm_explorer/indexes/vectorstore.py
 llm_explorer/interfaces/__init__.py
```

### Comparing `llm_explorer-0.0.7/llm_explorer.egg-info/requires.txt` & `llm_explorer-0.0.9/llm_explorer.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -160,7 +160,8 @@
 sentencepiece
 opencv-python
 sqlalchemy-databricks
 transformers
 huggingface_hub
 streamlit-authenticator
 tabulate
+black
```

### Comparing `llm_explorer-0.0.7/requirements.txt` & `llm_explorer-0.0.9/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -162,8 +162,9 @@
 sentencepiece 
 opencv-python
 sqlalchemy-databricks
 transformers
 #--extra-index-url https://github.com/huggingface/transformers@v4.29.0
 huggingface_hub
 streamlit-authenticator
-tabulate
+tabulate
+black
```

### Comparing `llm_explorer-0.0.7/setup.py` & `llm_explorer-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 import sys
-
+import glob
 from setuptools import find_packages, setup
 
 if sys.version_info < (3, 6):
     print("Error: llm_explorer does not support this version of Python.")
     print("Please upgrade to Python 3.6 or higher.")
     sys.exit(1)
 
@@ -23,57 +23,70 @@
 
 version = "#{PKG_VAR_SETUP}#"
 package_name = "llm_explorer"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 if "PKGVARSETUP" in package_env:
-    version = "0.0.7"
+    version = "0.0.9"
 
 package_env = re.sub(r"[^a-zA-Z]", "", version)
 
 # Check if any letters were found
 if len(package_env) > 0:
     package_name += f"_{package_env}"
 
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
+
+def prepare_data_files(directory, extensions):
+    files = []
+    for ext in extensions:
+        files.extend(glob.glob(f'{directory}/*.{ext}'))
+    return files
+
+
+data_files_structure = [
+    ('llm_explorer', prepare_data_files('llm_explorer', ['csv', 'sql', 'txt', 'md', 'html', 'css', 'json', 'yaml', 'faiss', 'pkl'])),
+]
+
 print(package_name, version)
 setup(
     name=package_name,
     version=version,
     author="Carlos D. Escobar-Valbuena",
     author_email="carlosdavidescobar@gmail.com",
     description="A Lakehouse LLM Explorer. Wrapper for spark, databricks and langchain processes",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
-    packages=find_packages(where="."),
+    packages=find_packages(),
     include_package_data=True,
     setup_requires=["setuptools", "wheel"],
     tests_require=["pytest"],
     python_requires=">=3.10",
     nstall_requires=required,
     test_suite="tests",
     zip_safe=False,
-    url="https://github.com/Occlusion-Solutions/occlussion_llm_explorer.git",
+    url="https://github.com/Occlusion-Solutions/llm_explorer.git",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.10",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     install_requires=required,
     package_data={
-        "": ["*.json", "*.yaml", ".sql", ".csv", ".txt", ".md", ".html", ".css"],
+        "llm_explorer": ["*.json", "*.yaml", "*.sql", "*.csv", "*.txt", "*.md", "*.html", "*.css", "*.pkl", "*.faiss"],
     },
+    data_files=data_files_structure,
     py_modules=['main'],
     entry_points={
         "console_scripts": [
             "llm_explorer=main:main",
         ],
     },
 )
```

