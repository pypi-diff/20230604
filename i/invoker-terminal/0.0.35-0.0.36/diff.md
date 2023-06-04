# Comparing `tmp/invoker_terminal-0.0.35.tar.gz` & `tmp/invoker_terminal-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invoker_terminal-0.0.35.tar", last modified: Sat Jun  3 15:00:51 2023, max compression
+gzip compressed data, was "invoker_terminal-0.0.36.tar", last modified: Sun Jun  4 12:42:24 2023, max compression
```

## Comparing `invoker_terminal-0.0.35.tar` & `invoker_terminal-0.0.36.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:51.530114 invoker_terminal-0.0.35/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-03 15:00:51.530114 invoker_terminal-0.0.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:51.510113 invoker_terminal-0.0.35/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:51.514114 invoker_terminal-0.0.35/invoker_terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/ast_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:51.522114 invoker_terminal-0.0.35/invoker_terminal/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/commands/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/commands/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/commands/ipfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/commands/new_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/commands/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/commands/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:51.522114 invoker_terminal-0.0.35/invoker_terminal/cores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/cores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/cores/anchor.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/cores/invoker_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/cores/ipfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/cores/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:51.522114 invoker_terminal-0.0.35/invoker_terminal/idl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/idl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/idl/invoker_network_market.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:51.526114 invoker_terminal-0.0.35/invoker_terminal/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/inputs/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/inputs/fileinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/inputs/inputbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/inputs/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/inputs/rangeinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/inputs/selectinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/inputs/textinput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:51.526114 invoker_terminal-0.0.35/invoker_terminal/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/outputs/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:51.526114 invoker_terminal-0.0.35/invoker_terminal/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/storage/deployed_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/storage/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:51.530114 invoker_terminal-0.0.35/invoker_terminal/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/templates/Dockerfile_template
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/templates/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/templates/requirements.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/invoker_terminal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:51.518113 invoker_terminal-0.0.35/invoker_terminal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-03 15:00:51.000000 invoker_terminal-0.0.35/invoker_terminal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-03 15:00:51.000000 invoker_terminal-0.0.35/invoker_terminal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:00:51.000000 invoker_terminal-0.0.35/invoker_terminal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-03 15:00:51.000000 invoker_terminal-0.0.35/invoker_terminal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-03 15:00:51.000000 invoker_terminal-0.0.35/invoker_terminal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-03 15:00:51.000000 invoker_terminal-0.0.35/invoker_terminal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 15:00:51.530114 invoker_terminal-0.0.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:51.530114 invoker_terminal-0.0.35/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-03 15:00:36.000000 invoker_terminal-0.0.35/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.627195 invoker_terminal-0.0.36/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-04 12:42:24.627195 invoker_terminal-0.0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.619195 invoker_terminal-0.0.36/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.619195 invoker_terminal-0.0.36/invoker_terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/ast_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/ipfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/new_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/commands/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/cores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cores/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cores/invoker_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cores/ipfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cores/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/cores/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/idl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/idl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/idl/invoker_network_market.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/fileinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/inputbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/rangeinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/selectinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/inputs/textinput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/outputs/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/storage/deployed_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/storage/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/templates/Dockerfile_template
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/templates/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/templates/requirements.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/invoker_terminal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.623195 invoker_terminal-0.0.36/invoker_terminal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-04 12:42:24.000000 invoker_terminal-0.0.36/invoker_terminal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-04 12:42:24.000000 invoker_terminal-0.0.36/invoker_terminal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:42:24.000000 invoker_terminal-0.0.36/invoker_terminal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-04 12:42:24.000000 invoker_terminal-0.0.36/invoker_terminal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-04 12:42:24.000000 invoker_terminal-0.0.36/invoker_terminal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-04 12:42:24.000000 invoker_terminal-0.0.36/invoker_terminal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 12:42:24.627195 invoker_terminal-0.0.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:24.627195 invoker_terminal-0.0.36/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-04 12:42:10.000000 invoker_terminal-0.0.36/tests/test_base.py
```

### Comparing `invoker_terminal-0.0.35/HISTORY.md` & `invoker_terminal-0.0.36/HISTORY.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Add testexecutor. [The Invoker]
+- Release: version  🚀 [The Invoker]
 - Release: version  🚀 [The Invoker]
 - V0.0.35. [The Invoker]
 - Bump v0.0.34. [The Invoker]
 - Release: version  🚀 [The Invoker]
 - Fix version. [The Invoker]
 - Release: version  🚀 [The Invoker]
 - Add invoke to configless commands. [The Invoker]
```

### Comparing `invoker_terminal-0.0.35/LICENSE` & `invoker_terminal-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/PKG-INFO` & `invoker_terminal-0.0.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoker_terminal
-Version: 0.0.35
+Version: 0.0.36
 Summary: Awesome invoker_terminal created by m00dy
 Home-page: https://github.com/m00dy/invoker-terminal/
 Author: m00dy
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `invoker_terminal-0.0.35/README.md` & `invoker_terminal-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/ast_check.py` & `invoker_terminal-0.0.36/invoker_terminal/ast_check.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/cli.py` & `invoker_terminal-0.0.36/invoker_terminal/cli.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/client.py` & `invoker_terminal-0.0.36/invoker_terminal/client.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/commands/build.py` & `invoker_terminal-0.0.36/invoker_terminal/commands/build.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/commands/daemon.py` & `invoker_terminal-0.0.36/invoker_terminal/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/commands/deploy.py` & `invoker_terminal-0.0.36/invoker_terminal/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/commands/init.py` & `invoker_terminal-0.0.36/invoker_terminal/commands/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     config["system"]["docker_url"] = str(docker_url)
     config["system"]["docker_sock"] = str(docker_sock)
     config["system"]["xml_rpc_addr"] = str(xml_rpc_addr)
     config["system"]["xml_rpc_port"] = str(xml_rpc_port)
     config["system"]["tmp_folder"] = str(tmp_folder)
     config["system"]["log_level"] = str(20)
     config["system"]["wallet"] = generatewallet().to_json()
+    config["system"]["gpu_enabled"] = "False"
     config["local"] = {}
     config["local"]["rpc_url"] = local_rpc_url
     config["local"]["websocket_url"] = local_websocket_url
     config["dev"] = {}
     config["dev"]["rpc_url"] = dev_rpc_url
     config["dev"]["websocket_url"] = dev_websocket_url
     config["mainnet"] = {}
```

### Comparing `invoker_terminal-0.0.35/invoker_terminal/commands/new_task.py` & `invoker_terminal-0.0.36/invoker_terminal/commands/new_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 import os
 
 DOCKERFILE_FILE = (
     os.path.dirname(__file__) + "/../templates/Dockerfile_template"
 )
 MODEL_FILE = os.path.dirname(__file__) + "/../templates/model.py"
+REQ_FILE = os.path.dirname(__file__) + "/../templates/requirements.yaml"
 
 model_template = open(MODEL_FILE).read()
 dockerfile_template = open(DOCKERFILE_FILE).read()
-
+req_template = open(REQ_FILE).read()
 
 def cmd_new_task(args, config):
     cwd = os.getcwd()
     name = str(input("Enter model name: "))
     print(name)
     print(cwd)
     if os.path.isdir(name):
@@ -31,10 +32,14 @@
         f.write(dockerfile_template)
         f.close()
 
         # modelpy
         f = open(newpath + "/model.py", "w")
         f.write(model_template)
         f.close()
+        
+        f = open(newpath + "requirements.yaml", "w")
+        f.write(req_template)
+        f.close()
 
     # name = input('What is the task name? (must be unique)\n')
     # print(name)
```

### Comparing `invoker_terminal-0.0.35/invoker_terminal/commands/status.py` & `invoker_terminal-0.0.36/invoker_terminal/commands/status.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/commands/wallet.py` & `invoker_terminal-0.0.36/invoker_terminal/commands/wallet.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/constants.py` & `invoker_terminal-0.0.36/invoker_terminal/constants.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/cores/anchor.py` & `invoker_terminal-0.0.36/invoker_terminal/cores/anchor.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/cores/invoker_init.py` & `invoker_terminal-0.0.36/invoker_terminal/cores/invoker_init.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/cores/ipfs.py` & `invoker_terminal-0.0.36/invoker_terminal/cores/ipfs.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/idl/invoker_network_market.json` & `invoker_terminal-0.0.36/invoker_terminal/idl/invoker_network_market.json`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/inputs/decorators.py` & `invoker_terminal-0.0.36/invoker_terminal/inputs/decorators.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/inputs/numberinput.py` & `invoker_terminal-0.0.36/invoker_terminal/inputs/numberinput.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/inputs/rangeinput.py` & `invoker_terminal-0.0.36/invoker_terminal/inputs/rangeinput.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/inputs/textinput.py` & `invoker_terminal-0.0.36/invoker_terminal/inputs/textinput.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/outputs/output.py` & `invoker_terminal-0.0.36/invoker_terminal/outputs/output.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/server.py` & `invoker_terminal-0.0.36/invoker_terminal/server.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/storage/deployed_models.py` & `invoker_terminal-0.0.36/invoker_terminal/storage/deployed_models.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/templates/Dockerfile_template` & `invoker_terminal-0.0.36/invoker_terminal/templates/Dockerfile_template`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/templates/model.py` & `invoker_terminal-0.0.36/invoker_terminal/templates/model.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal/utils.py` & `invoker_terminal-0.0.36/invoker_terminal/utils.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.35/invoker_terminal.egg-info/PKG-INFO` & `invoker_terminal-0.0.36/invoker_terminal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoker-terminal
-Version: 0.0.35
+Version: 0.0.36
 Summary: Awesome invoker_terminal created by m00dy
 Home-page: https://github.com/m00dy/invoker-terminal/
 Author: m00dy
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `invoker_terminal-0.0.35/invoker_terminal.egg-info/SOURCES.txt` & `invoker_terminal-0.0.36/invoker_terminal.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 invoker_terminal/commands/status.py
 invoker_terminal/commands/test.py
 invoker_terminal/commands/wallet.py
 invoker_terminal/cores/__init__.py
 invoker_terminal/cores/anchor.py
 invoker_terminal/cores/invoker_init.py
 invoker_terminal/cores/ipfs.py
+invoker_terminal/cores/test_executor.py
 invoker_terminal/cores/wallet.py
 invoker_terminal/idl/__init__.py
 invoker_terminal/idl/invoker_network_market.json
 invoker_terminal/inputs/__init__.py
 invoker_terminal/inputs/decorators.py
 invoker_terminal/inputs/fileinput.py
 invoker_terminal/inputs/inputbase.py
```

### Comparing `invoker_terminal-0.0.35/setup.py` & `invoker_terminal-0.0.36/setup.py`

 * *Files identical despite different names*

