# Comparing `tmp/invoker_terminal-0.0.36.tar.gz` & `tmp/invoker_terminal-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invoker_terminal-0.0.36.tar", last modified: Sun Jun  4 12:42:24 2023, max compression
+gzip compressed data, was "invoker_terminal-0.0.37.tar", last modified: Sun Jun  4 14:42:29 2023, max compression
```

## Comparing `invoker_terminal-0.0.36.tar` & `invoker_terminal-0.0.37.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.627195 invoker_terminal-0.0.36/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-04 12:42:24.627195 invoker_terminal-0.0.36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.619195 invoker_terminal-0.0.36/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.619195 invoker_terminal-0.0.36/invoker_terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/ast_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/ipfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/new_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/cores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cores/anchor.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cores/invoker_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cores/ipfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cores/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cores/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/idl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/idl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/idl/invoker_network_market.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/fileinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/inputbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/rangeinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/selectinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/textinput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/outputs/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/storage/deployed_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/storage/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/templates/Dockerfile_template
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/templates/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/templates/requirements.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-04 12:42:24.000000 invoker_terminal-0.0.36/invoker_terminal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-04 12:42:24.000000 invoker_terminal-0.0.36/invoker_terminal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:42:24.000000 invoker_terminal-0.0.36/invoker_terminal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-04 12:42:24.000000 invoker_terminal-0.0.36/invoker_terminal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-04 12:42:24.000000 invoker_terminal-0.0.36/invoker_terminal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-04 12:42:24.000000 invoker_terminal-0.0.36/invoker_terminal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 12:42:24.627195 invoker_terminal-0.0.36/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.627195 invoker_terminal-0.0.36/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:29.742251 invoker_terminal-0.0.37/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-04 14:42:29.742251 invoker_terminal-0.0.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:29.738251 invoker_terminal-0.0.37/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:29.738251 invoker_terminal-0.0.37/invoker_terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/ast_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:29.738251 invoker_terminal-0.0.37/invoker_terminal/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/commands/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/commands/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/commands/ipfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/commands/new_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/commands/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/commands/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:29.738251 invoker_terminal-0.0.37/invoker_terminal/cores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/cores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/cores/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/cores/invoker_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/cores/ipfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/cores/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/cores/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:29.738251 invoker_terminal-0.0.37/invoker_terminal/idl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/idl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/idl/invoker_network_market.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:29.742251 invoker_terminal-0.0.37/invoker_terminal/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/inputs/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/inputs/fileinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/inputs/inputbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/inputs/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/inputs/rangeinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/inputs/selectinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/inputs/textinput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:29.742251 invoker_terminal-0.0.37/invoker_terminal/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/outputs/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13149 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:29.742251 invoker_terminal-0.0.37/invoker_terminal/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/storage/deployed_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/storage/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:29.742251 invoker_terminal-0.0.37/invoker_terminal/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/templates/Dockerfile_template
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/templates/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/templates/requirements.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/invoker_terminal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:29.738251 invoker_terminal-0.0.37/invoker_terminal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-04 14:42:29.000000 invoker_terminal-0.0.37/invoker_terminal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-04 14:42:29.000000 invoker_terminal-0.0.37/invoker_terminal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 14:42:29.000000 invoker_terminal-0.0.37/invoker_terminal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-04 14:42:29.000000 invoker_terminal-0.0.37/invoker_terminal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-04 14:42:29.000000 invoker_terminal-0.0.37/invoker_terminal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-04 14:42:29.000000 invoker_terminal-0.0.37/invoker_terminal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 14:42:29.742251 invoker_terminal-0.0.37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:29.742251 invoker_terminal-0.0.37/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-04 14:42:13.000000 invoker_terminal-0.0.37/tests/test_base.py
```

### Comparing `invoker_terminal-0.0.36/HISTORY.md` & `invoker_terminal-0.0.37/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Enable async gpu acceleration. [The Invoker]
+- Release: version  🚀 [The Invoker]
 - Add testexecutor. [The Invoker]
 - Release: version  🚀 [The Invoker]
 - Release: version  🚀 [The Invoker]
 - V0.0.35. [The Invoker]
 - Bump v0.0.34. [The Invoker]
 - Release: version  🚀 [The Invoker]
 - Fix version. [The Invoker]
```

### Comparing `invoker_terminal-0.0.36/LICENSE` & `invoker_terminal-0.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/PKG-INFO` & `invoker_terminal-0.0.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoker_terminal
-Version: 0.0.36
+Version: 0.0.37
 Summary: Awesome invoker_terminal created by m00dy
 Home-page: https://github.com/m00dy/invoker-terminal/
 Author: m00dy
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `invoker_terminal-0.0.36/README.md` & `invoker_terminal-0.0.37/README.md`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/ast_check.py` & `invoker_terminal-0.0.37/invoker_terminal/ast_check.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/cli.py` & `invoker_terminal-0.0.37/invoker_terminal/cli.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/client.py` & `invoker_terminal-0.0.37/invoker_terminal/client.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/commands/build.py` & `invoker_terminal-0.0.37/invoker_terminal/commands/build.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/commands/daemon.py` & `invoker_terminal-0.0.37/invoker_terminal/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/commands/deploy.py` & `invoker_terminal-0.0.37/invoker_terminal/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/commands/init.py` & `invoker_terminal-0.0.37/invoker_terminal/commands/init.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/commands/new_task.py` & `invoker_terminal-0.0.37/invoker_terminal/commands/new_task.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/commands/status.py` & `invoker_terminal-0.0.37/invoker_terminal/commands/status.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/commands/wallet.py` & `invoker_terminal-0.0.37/invoker_terminal/commands/wallet.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/constants.py` & `invoker_terminal-0.0.37/invoker_terminal/constants.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/cores/anchor.py` & `invoker_terminal-0.0.37/invoker_terminal/cores/anchor.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/cores/invoker_init.py` & `invoker_terminal-0.0.37/invoker_terminal/cores/invoker_init.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/cores/ipfs.py` & `invoker_terminal-0.0.37/invoker_terminal/cores/ipfs.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/cores/test_executor.py` & `invoker_terminal-0.0.37/invoker_terminal/cores/test_executor.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/idl/invoker_network_market.json` & `invoker_terminal-0.0.37/invoker_terminal/idl/invoker_network_market.json`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/inputs/decorators.py` & `invoker_terminal-0.0.37/invoker_terminal/inputs/decorators.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/inputs/numberinput.py` & `invoker_terminal-0.0.37/invoker_terminal/inputs/numberinput.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/inputs/rangeinput.py` & `invoker_terminal-0.0.37/invoker_terminal/inputs/rangeinput.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/inputs/textinput.py` & `invoker_terminal-0.0.37/invoker_terminal/inputs/textinput.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/outputs/output.py` & `invoker_terminal-0.0.37/invoker_terminal/outputs/output.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/server.py` & `invoker_terminal-0.0.37/invoker_terminal/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 import atexit
 import json
 import os
 import threading
 import time
 import traceback
 import uuid
+import shutil
 from multiprocessing import current_process
 from pathlib import Path
 from struct import pack_into
 from xmlrpc.server import (
     SimpleXMLRPCRequestHandler,
     SimpleXMLRPCServer,
 )
 
+import docker
 import aiodocker
 import aiohttp
 import websockets
 from nacl.encoding import Base64Encoder
 from nacl.signing import SigningKey
 from solana.rpc.websocket_api import connect
 from solders.pubkey import Pubkey
@@ -77,31 +79,39 @@
     id = uuid.uuid4()
     host_url = os.path.join(cf["system"]["tmp_folder"], str(id))
     Path(host_url).mkdir(parents=True, exist_ok=True)
     logger.info("Host url {}".format(host_url))
     with open("{}/input.zip".format(host_url), "wb") as f:
         f.write(input)
 
-    docker = aiodocker.Docker(cf["system"]["docker_url"])
+    device_requests = []
+    gpu_enabled = cf["system"].get("gpu_enabled", False)
+    if gpu_enabled != "False" and gpu_enabled != False:
+        device_requests = [docker.types.DeviceRequest(count=-1, capabilities=[['gpu']])]
+    #async docker client -> docker_
+    docker_ = aiodocker.Docker(cf["system"]["docker_url"])
     container_config = {
         "Image": "{}".format(image_id),
-        "HostConfig": {"Binds": [f"{host_url}:/invoker"]},
+        "HostConfig": {
+            "Binds": [f"{host_url}:/invoker"],
+            "DeviceRequests": device_requests
+            }
     }
+    logger.info("Device Requests {}".format(device_requests))
     logger.info("Container ID {}".format(str(id)))
     logger.info("Container Config {}".format(container_config))
-    container = await docker.containers.create_or_replace(
+    container = await docker_.containers.create_or_replace(
         str(id), container_config
     )
     await container.start()
     await container.wait()
     await container.delete(force=True)
-    await docker.close()
+    await docker_.close()
     output = open("{}/output.zip".format(host_url), "rb").read()
-    # todo
-    # delete host mount point here
+    shutil.rmtree(host_url)
     return output
 
 
 async def heart_beat(cf, model: DeployedModel):
     HEARTBEAT_INTERVAL = 15
     logger = logging.getLogger("HeartBeat")
     keystr = cf["system"]["wallet"]
```

### Comparing `invoker_terminal-0.0.36/invoker_terminal/storage/deployed_models.py` & `invoker_terminal-0.0.37/invoker_terminal/storage/deployed_models.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/templates/Dockerfile_template` & `invoker_terminal-0.0.37/invoker_terminal/templates/Dockerfile_template`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/templates/model.py` & `invoker_terminal-0.0.37/invoker_terminal/templates/model.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal/utils.py` & `invoker_terminal-0.0.37/invoker_terminal/utils.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/invoker_terminal.egg-info/PKG-INFO` & `invoker_terminal-0.0.37/invoker_terminal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoker-terminal
-Version: 0.0.36
+Version: 0.0.37
 Summary: Awesome invoker_terminal created by m00dy
 Home-page: https://github.com/m00dy/invoker-terminal/
 Author: m00dy
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `invoker_terminal-0.0.36/invoker_terminal.egg-info/SOURCES.txt` & `invoker_terminal-0.0.37/invoker_terminal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.36/setup.py` & `invoker_terminal-0.0.37/setup.py`

 * *Files identical despite different names*

