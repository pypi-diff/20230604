# Comparing `tmp/codex-chat-notebook-0.1.4.tar.gz` & `tmp/codex-chat-notebook-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codex-chat-notebook-0.1.4.tar", last modified: Tue Apr 26 19:26:17 2022, max compression
+gzip compressed data, was "codex-chat-notebook-0.1.5.tar", last modified: Sun Jun  4 21:47:10 2023, max compression
```

## Comparing `codex-chat-notebook-0.1.4.tar` & `codex-chat-notebook-0.1.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 19:26:17.663546 codex-chat-notebook-0.1.4/
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 19:26:17.659546 codex-chat-notebook-0.1.4/.github/
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 19:26:17.663546 codex-chat-notebook-0.1.4/.github/workflows/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1417 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.4/.github/workflows/build.yml
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1450 2021-11-28 18:14:12.000000 codex-chat-notebook-0.1.4/.gitignore
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      101 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.4/.prettierignore
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       79 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.4/.prettierrc
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1510 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.4/LICENSE
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      443 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.4/MANIFEST.in
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3055 2022-04-26 19:26:17.663546 codex-chat-notebook-0.1.4/PKG-INFO
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1987 2021-11-28 20:05:42.000000 codex-chat-notebook-0.1.4/README.md
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 19:26:17.663546 codex-chat-notebook-0.1.4/binder/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      516 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.4/binder/environment.yml
--rwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)     1266 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.4/binder/postBuild
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 19:26:17.663546 codex-chat-notebook-0.1.4/codex-chat-notebook/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      318 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/__init__.py
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      441 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/_version.py
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 19:26:17.663546 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2159 2022-04-26 19:26:16.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/package.json
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 19:26:17.663546 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2674 2022-04-26 19:26:16.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/223.b54a1552aec55f828dd0.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      852 2022-04-26 19:26:16.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/223.b54a1552aec55f828dd0.js.LICENSE.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)    20996 2022-04-26 19:26:16.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/267.a5477cedb5aecf90b318.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)    11549 2022-04-26 19:26:16.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/597.6a0e30da9896849c3b2d.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     5387 2022-04-26 19:26:16.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/747.c7879d7e9587a1c6296d.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)    20325 2022-04-26 19:26:16.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/905.fd54bc0b4a42205403dc.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2674 2022-04-26 19:26:16.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/927.21eeae7dfef6ffcebedc.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      852 2022-04-26 19:26:16.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/927.21eeae7dfef6ffcebedc.js.LICENSE.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     8227 2022-04-26 19:26:16.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/remoteEntry.ee0fc643ff265d1ca186.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      162 2022-04-26 19:26:15.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/style.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     5308 2022-04-26 19:26:16.000000 codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/third-party-licenses.json
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 19:26:17.663546 codex-chat-notebook-0.1.4/codex-prompt-repository/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      968 2021-11-28 22:14:30.000000 codex-chat-notebook-0.1.4/codex-prompt-repository/default.md
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1407 2021-11-28 22:40:20.000000 codex-chat-notebook-0.1.4/codex-prompt-repository/image-analysis.md
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      563 2021-11-28 22:41:54.000000 codex-chat-notebook-0.1.4/codex-prompt-repository/index.json
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 19:26:17.663546 codex-chat-notebook-0.1.4/codex_chat_notebook.egg-info/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3055 2022-04-26 19:26:17.000000 codex-chat-notebook-0.1.4/codex_chat_notebook.egg-info/PKG-INFO
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1537 2022-04-26 19:26:17.000000 codex-chat-notebook-0.1.4/codex_chat_notebook.egg-info/SOURCES.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)        1 2022-04-26 19:26:17.000000 codex-chat-notebook-0.1.4/codex_chat_notebook.egg-info/dependency_links.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)        1 2021-11-28 18:18:06.000000 codex-chat-notebook-0.1.4/codex_chat_notebook.egg-info/not-zip-safe
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       16 2022-04-26 19:26:17.000000 codex-chat-notebook-0.1.4/codex_chat_notebook.egg-info/requires.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       20 2022-04-26 19:26:17.000000 codex-chat-notebook-0.1.4/codex_chat_notebook.egg-info/top_level.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      199 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.4/install.json
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 19:26:17.663546 codex-chat-notebook-0.1.4/lib/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)    19906 2022-04-26 19:23:17.000000 codex-chat-notebook-0.1.4/lib/index.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)   248060 2022-04-26 19:26:01.000000 codex-chat-notebook-0.1.4/package-lock.json
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2017 2022-04-26 19:25:56.000000 codex-chat-notebook-0.1.4/package.json
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      165 2021-11-28 18:30:06.000000 codex-chat-notebook-0.1.4/publish.sh
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      145 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.4/pyproject.toml
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       38 2022-04-26 19:26:17.663546 codex-chat-notebook-0.1.4/setup.cfg
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2621 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.4/setup.py
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 19:26:17.663546 codex-chat-notebook-0.1.4/style/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       78 2022-04-26 19:25:44.000000 codex-chat-notebook-0.1.4/style/base.css
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       25 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.4/style/index.css
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       21 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.4/style/index.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1498 2022-04-26 19:20:56.000000 codex-chat-notebook-0.1.4/style/robot.svg
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)   227401 2021-11-22 08:12:04.000000 codex-chat-notebook-0.1.4/yarn.lock
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-04 21:47:10.025466 codex-chat-notebook-0.1.5/
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-04 21:47:10.021466 codex-chat-notebook-0.1.5/.github/
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-04 21:47:10.021466 codex-chat-notebook-0.1.5/.github/workflows/
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1417 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.5/.github/workflows/build.yml
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1450 2021-11-28 18:14:12.000000 codex-chat-notebook-0.1.5/.gitignore
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      101 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.5/.prettierignore
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       79 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.5/.prettierrc
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1510 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.5/LICENSE
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      443 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.5/MANIFEST.in
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3054 2023-06-04 21:47:10.025466 codex-chat-notebook-0.1.5/PKG-INFO
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1987 2021-11-28 20:05:42.000000 codex-chat-notebook-0.1.5/README.md
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-04 21:47:10.021466 codex-chat-notebook-0.1.5/binder/
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      516 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.5/binder/environment.yml
+-rwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)     1266 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.5/binder/postBuild
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-04 21:47:10.021466 codex-chat-notebook-0.1.5/codex-chat-notebook/
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      318 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/__init__.py
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      441 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/_version.py
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-04 21:47:10.021466 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2155 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/package.json
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-04 21:47:10.025466 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2674 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/223.b54a1552aec55f828dd0.js
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      852 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/223.b54a1552aec55f828dd0.js.LICENSE.txt
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)    12799 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/412.a2835a83deddc2445136.js
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)    48836 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/485.461f1ffaed83f67adf0b.js
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     5387 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/747.c7879d7e9587a1c6296d.js
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)    20325 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/905.5c83ee4c20235cca8264.js
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2674 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/927.21eeae7dfef6ffcebedc.js
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      852 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/927.21eeae7dfef6ffcebedc.js.LICENSE.txt
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     8219 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/remoteEntry.917c6c06846d04d0cc6e.js
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      162 2023-06-04 21:47:08.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/style.js
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     7675 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/third-party-licenses.json
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-04 21:47:10.025466 codex-chat-notebook-0.1.5/codex-prompt-repository/
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3343 2022-04-26 19:26:35.000000 codex-chat-notebook-0.1.5/codex-prompt-repository/cellpose-image-segmentation.md
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      968 2021-11-28 22:14:30.000000 codex-chat-notebook-0.1.5/codex-prompt-repository/default.md
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1407 2021-11-28 22:40:20.000000 codex-chat-notebook-0.1.5/codex-prompt-repository/image-analysis.md
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      834 2022-04-26 19:26:35.000000 codex-chat-notebook-0.1.5/codex-prompt-repository/index.json
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-04 21:47:10.025466 codex-chat-notebook-0.1.5/codex_chat_notebook.egg-info/
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3054 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex_chat_notebook.egg-info/PKG-INFO
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1574 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex_chat_notebook.egg-info/SOURCES.txt
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)        1 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex_chat_notebook.egg-info/dependency_links.txt
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)        1 2021-11-28 18:18:06.000000 codex-chat-notebook-0.1.5/codex_chat_notebook.egg-info/not-zip-safe
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       16 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex_chat_notebook.egg-info/requires.txt
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       20 2023-06-04 21:47:09.000000 codex-chat-notebook-0.1.5/codex_chat_notebook.egg-info/top_level.txt
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      199 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.5/install.json
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-04 21:47:10.025466 codex-chat-notebook-0.1.5/lib/
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)    21849 2023-06-04 21:42:39.000000 codex-chat-notebook-0.1.5/lib/index.js
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2013 2023-06-04 21:08:36.000000 codex-chat-notebook-0.1.5/package.json
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      165 2021-11-28 18:30:06.000000 codex-chat-notebook-0.1.5/publish.sh
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      145 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.5/pyproject.toml
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       38 2023-06-04 21:47:10.025466 codex-chat-notebook-0.1.5/setup.cfg
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2621 2021-11-28 18:11:07.000000 codex-chat-notebook-0.1.5/setup.py
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-04 21:47:10.025466 codex-chat-notebook-0.1.5/style/
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       78 2022-04-26 19:25:44.000000 codex-chat-notebook-0.1.5/style/base.css
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       25 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.5/style/index.css
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       21 2021-11-21 20:08:06.000000 codex-chat-notebook-0.1.5/style/index.js
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1498 2022-04-26 19:20:56.000000 codex-chat-notebook-0.1.5/style/robot.svg
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)   227517 2023-06-04 20:38:09.000000 codex-chat-notebook-0.1.5/yarn.lock
```

### Comparing `codex-chat-notebook-0.1.4/.github/workflows/build.yml` & `codex-chat-notebook-0.1.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/.gitignore` & `codex-chat-notebook-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/LICENSE` & `codex-chat-notebook-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/PKG-INFO` & `codex-chat-notebook-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codex-chat-notebook
-Version: 0.1.4
+Version: 0.1.5
 Summary: Doing data science without programming skills by chatting with OpenAI Codex
 Home-page: https://github.com/oeway/codex-chat-notebook
 Author: Wei Ouyang
 Author-email: oeway007@gmail.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -93,8 +93,7 @@
 ```
 
 ```
 pip install jupyter_packaging
 npm run install:extension
 jupyter lab
 ```
-
```

### Comparing `codex-chat-notebook-0.1.4/README.md` & `codex-chat-notebook-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/binder/environment.yml` & `codex-chat-notebook-0.1.5/binder/environment.yml`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/binder/postBuild` & `codex-chat-notebook-0.1.5/binder/postBuild`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/package.json` & `codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9635141093474426%*

 * *Differences: {"'dependencies'": "{'openai': '^3.2.1', delete: ['openai-api']}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.917c6c06846d04d0cc6e.js'}}",*

 * * "'version'": "'0.1.5'"}*

```diff
@@ -8,15 +8,15 @@
     },
     "dependencies": {
         "@jupyterlab/application": "^3.2.4",
         "@jupyterlab/apputils": "^3.2.4",
         "@jupyterlab/docregistry": "^3.2.4",
         "@jupyterlab/notebook": "^3.2.4",
         "@phosphor/disposable": "^1.3.1",
-        "openai-api": "^1.2.6"
+        "openai": "^3.2.1"
     },
     "description": "Doing data science without programming skills by chatting with OpenAI Codex",
     "devDependencies": {
         "@jupyterlab/builder": "^3.0.0",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2"
     },
@@ -24,15 +24,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/oeway/codex-chat-notebook",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ee0fc643ff265d1ca186.js",
+            "load": "static/remoteEntry.917c6c06846d04d0cc6e.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "codex-chat-notebook/labextension"
     },
     "keywords": [
         "jupyter",
@@ -61,9 +61,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
-    "version": "0.1.4"
+    "version": "0.1.5"
 }
```

### Comparing `codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/223.b54a1552aec55f828dd0.js` & `codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/223.b54a1552aec55f828dd0.js`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/223.b54a1552aec55f828dd0.js.LICENSE.txt` & `codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/223.b54a1552aec55f828dd0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/597.6a0e30da9896849c3b2d.js` & `codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/412.a2835a83deddc2445136.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,243 +1,277 @@
 "use strict";
 (self.webpackChunkcodex_chat_notebook = self.webpackChunkcodex_chat_notebook || []).push([
-    [597], {
-        1568: (t, e, o) => {
-            o.r(e), o.d(e, {
-                default: () => u
+    [412], {
+        1568: (e, t, o) => {
+            o.r(t), o.d(t, {
+                default: () => p
             });
-            var n = o(9321),
+            var n = o(6825),
                 s = o(2138),
                 i = o(3706),
-                l = o(7023),
-                a = o.n(l),
-                c = o(7905),
-                r = o(9628),
-                h = o(608);
-            class d {
-                constructor(t) {
-                    t.currentChanged.connect((t => {
-                        this.notebook = t.currentWidget.children()._source[2]
+                l = o(3931),
+                a = o(7905),
+                c = o(4198),
+                r = o(608);
+            class h {
+                constructor(e) {
+                    e.currentChanged.connect((e => {
+                        this.notebook = e.currentWidget.children()._source[2]
                     }))
                 }
-                createNew(t, e) {
-                    const o = t.content;
-                    this.notebook = o, o._sessionContex = e.sessionContext;
+                createNew(e, t) {
+                    const o = e.content;
+                    this.notebook = o, o._sessionContex = t.sessionContext;
                     let i = new n.ToolbarButton({
                         iconClass: "jp-RobotIcon",
                         onClick: () => {
                             console.log(`Notebook "${o.title.label}" is now activated as the current chat notebook!`)
                         },
-                        tooltip: "Codex Chat Notebook is enabled"
+                        tooltip: "Chat Notebook is enabled"
                     });
-                    return t.toolbar.insertItem(0, "activate", i), new s.DisposableDelegate((() => {
+                    return e.toolbar.insertItem(0, "activate", i), new s.DisposableDelegate((() => {
                         i.dispose(), this.notebook === o && (this.notebook = null)
                     }))
                 }
-                getState(t) {
+                getState(e) {
                     return {
-                        wasFocused: t.node.contains(document.activeElement),
-                        activeCell: t.activeCell
+                        wasFocused: e.node.contains(document.activeElement),
+                        activeCell: e.activeCell
                     }
                 }
-                handleState(t, e, o = !1) {
+                handleState(e, t, o = !1) {
                     const {
                         activeCell: n,
                         node: s
-                    } = t;
-                    (e.wasFocused || "edit" === t.mode) && t.activate(), o && n && h.ElementExt.scrollIntoViewIfNeeded(s, n.node)
+                    } = e;
+                    (t.wasFocused || "edit" === e.mode) && e.activate(), o && n && r.ElementExt.scrollIntoViewIfNeeded(s, n.node)
                 }
-                getCodeHistory(t, e) {
+                getCodeHistory(e, t) {
                     const o = this.notebook.model.cells,
                         n = [];
                     let s = !0;
                     for (let i = 0; i < o.length && !(i > this.notebook.activeCellIndex); i++) {
                         const l = o.get(i);
-                        if ("code" === l.type) s ? (n.push(`\n"""\n${t}\n"""\n${l.value.text}\n${e}`), s = !1) : n.push(l.value.text);
+                        if ("code" === l.type) s ? (n.push({
+                            role: "assistant",
+                            content: `\n"""\n${e}\n"""\n${l.value.text}\n${t}`
+                        }), s = !1) : n.push({
+                            role: "assistant",
+                            content: l.value.text
+                        });
                         else if ("markdown" === l.type) {
                             let o = "";
                             const i = l.value.text.split("\n");
                             if (o += "## " + i[0].replace(/^(\#+\s)/, ""), s || i.length > 1) {
                                 let n, l;
-                                l = s ? t : "", n = i.length > 1 ? i.slice(1).join("\n") : "", o += `\n"""\n${l}\n${n}\n"""`, s && (o += `\n${e}`, s = !1)
+                                l = s ? e : "", n = i.length > 1 ? i.slice(1).join("\n") : "", o += `\n"""\n${l}\n${n}\n"""`, s && (o += `\n${t}`, s = !1)
                             }
-                            n.push(o)
+                            n.push({
+                                role: "user",
+                                content: o
+                            })
                         }
                     }
                     return n
                 }
-                addCell(t, e) {
+                addCell(e, t) {
                     const o = this.notebook;
                     if (!o.model) return;
                     const n = this.getState(o),
                         s = o.model,
                         i = s.contentFactory.createMarkdownCell({});
-                    i.value.text = t, s.cells.insert(o.activeCellIndex + 1, i);
+                    i.value.text = e, s.cells.insert(o.activeCellIndex + 1, i);
                     const l = s.contentFactory.createCodeCell({});
-                    l.value.text = e, s.cells.insert(o.activeCellIndex + 2, l), o.activeCellIndex += 2, this.notebook.lastCellIndex = o.activeCellIndex, this.notebook.lastCellNumber = 2, o.deselectAll(), this.handleState(o, n, !0), setTimeout((async () => {
+                    l.value.text = t, s.cells.insert(o.activeCellIndex + 2, l), o.activeCellIndex += 2, this.notebook.lastCellIndex = o.activeCellIndex, this.notebook.lastCellNumber = 2, o.deselectAll(), this.handleState(o, n, !0), setTimeout((async () => {
                         try {
-                            const t = await c.v.run(this.notebook, this.notebook._sessionContex);
-                            console.log(t)
-                        } catch (t) {
-                            console.error(t)
+                            const e = await a.v.run(this.notebook, this.notebook._sessionContex);
+                            console.log(e)
+                        } catch (e) {
+                            console.error(e)
                         }
                     }), 0)
                 }
-                addMarkdown(t) {
-                    const e = this.notebook;
-                    if (!e.model) return;
-                    const o = this.getState(e),
+                addMarkdown(e) {
+                    const t = this.notebook;
+                    if (!t.model) return;
+                    const o = this.getState(t),
                         n = model.contentFactory.createMarkdownCell({});
-                    n.value.text = t, model.cells.insert(e.activeCellIndex + 1, n), e.activeCellIndex += 1, this.notebook.lastCellIndex = e.activeCellIndex, this.notebook.lastCellNumber = 1, e.deselectAll(), this.handleState(e, o, !0)
+                    n.value.text = e, model.cells.insert(t.activeCellIndex + 1, n), t.activeCellIndex += 1, this.notebook.lastCellIndex = t.activeCellIndex, this.notebook.lastCellNumber = 1, t.deselectAll(), this.handleState(t, o, !0)
                 }
                 runCell() {
-                    notebook.model && notebook.activeCell && c.v.run(this.notebook, this.notebook._sessionContex)
+                    notebook.model && notebook.activeCell && a.v.run(this.notebook, this.notebook._sessionContex)
                 }
                 runAllCells() {
-                    c.v.runAll(this.notebook, this.notebook._sessionContex)
+                    a.v.runAll(this.notebook, this.notebook._sessionContex)
                 }
                 undoCell() {
-                    let t = "";
+                    let e = "";
                     if (this.notebook.lastCellNumber && this.notebook.lastCellNumber > 0) {
-                        for (let e = 0; e < this.notebook.lastCellNumber; e++) {
-                            const e = this.notebook.model.cells.get(this.notebook.activeCellIndex);
-                            e && "markdown" === e.type && e.value.text.trim().startsWith("# ") && (t = e.value.text.trim().replace(/^(\#+\s)/, "")), c.v.cut(this.notebook), this.notebook.activeCellIndex = this.notebook.lastCellIndex - (this.notebook.lastCellNumber - 1)
+                        for (let t = 0; t < this.notebook.lastCellNumber; t++) {
+                            const t = this.notebook.model.cells.get(this.notebook.activeCellIndex);
+                            t && "markdown" === t.type && t.value.text.trim().startsWith("# ") && (e = t.value.text.trim().replace(/^(\#+\s)/, "")), a.v.cut(this.notebook), this.notebook.activeCellIndex = this.notebook.lastCellIndex - (this.notebook.lastCellNumber - 1)
                         }
                         this.notebook.lastCellIndex = 0, this.notebook.lastCellNumber = 0, this.notebook.activeCellIndex -= 1
                     } else {
-                        const e = this.notebook.model.cells.get(this.notebook.activeCellIndex);
-                        e && "markdown" === e.type && e.value.text.trim().startsWith("# ") && (t = e.value.text.trim().replace(/^(\#+\s)/, "")), c.v.cut(this.notebook), this.notebook.activeCellIndex -= 1
+                        const t = this.notebook.model.cells.get(this.notebook.activeCellIndex);
+                        t && "markdown" === t.type && t.value.text.trim().startsWith("# ") && (e = t.value.text.trim().replace(/^(\#+\s)/, "")), a.v.cut(this.notebook), this.notebook.activeCellIndex -= 1
                     }
-                    return t
+                    return e
                 }
             }
-            async function p(t, e) {
-                e = t.base_url.replace(/\/$/, "") + "/" + e;
-                const o = await fetch(e),
+            async function d(e, t) {
+                t = e.base_url.replace(/\/$/, "") + "/" + t;
+                const o = await fetch(t),
                     n = (await o.text()).split("\n");
                 let s = "prompt",
                     i = "",
                     l = "";
-                for (let t = 0; t < n.length; t++)
+                for (let e = 0; e < n.length; e++)
                     if ("prompt" === s) {
-                        if (n[t].startsWith("-----")) {
+                        if (n[e].startsWith("-----")) {
                             s = "code";
                             continue
                         }
-                        i += n[t] + "\n"
+                        i += n[e] + "\n"
                     } else {
-                        const e = n[t].replace(/```/g, "");
-                        "" !== e.trim() && (l += e + "\n")
+                        const t = n[e].replace(/```/g, "");
+                        "" !== t.trim() && (l += t + "\n")
                     } return {
                     prefix: i.trim(),
                     examples: l.trim()
                 }
             }
-            const u = {
+            const p = {
                 id: "codex-chat-notebook",
                 autoStart: !0,
-                requires: [r.INotebookTracker],
-                activate: function(t, e) {
-                    const o = new d(e);
-                    t.docRegistry.addWidgetExtension("Notebook", o), console.log("JupyterLab extension codex-chat-notebook is activated!");
+                requires: [c.INotebookTracker],
+                activate: function(e, t) {
+                    const o = new h(t);
+                    e.docRegistry.addWidgetExtension("Notebook", o), console.log("JupyterLab extension codex-chat-notebook is activated!");
                     class n extends i.Widget {
                         constructor() {
-                            super(), this.addClass("content"), this.id = "tutorial", this.title.label = "Codex Chat Notebook", this.title.closable = !0, this.createNode()
+                            super(), this.addClass("content"), this.id = "tutorial", this.title.label = "Chat Notebook", this.title.closable = !0, this.createNode()
                         }
                         setupSpeech() {
                             if ("webkitSpeechRecognition" in window) {
-                                let t = new webkitSpeechRecognition,
-                                    e = "",
+                                let e = new webkitSpeechRecognition,
+                                    t = "",
                                     o = !1;
-                                t.continuous = !0, t.interimResults = !0, t.lang = "en-US", this.speechButton.style.background = "", t.onstart = () => {
-                                    o = !0, e = "", this.speechButton.style.background = "greenyellow"
-                                }, t.onerror = () => {
+                                e.continuous = !0, e.interimResults = !0, e.lang = "en-US", this.speechButton.style.background = "", e.onstart = () => {
+                                    o = !0, t = "", this.speechButton.style.background = "greenyellow"
+                                }, e.onerror = () => {
                                     o = !1, this.speechButton.style.background = "red", console.log("Speech Recognition Error")
-                                }, t.onend = () => {
+                                }, e.onend = () => {
                                     o = !1, this.speechButton.style.background = "", console.log("Speech Recognition Ended")
-                                }, t.onresult = t => {
+                                }, e.onresult = e => {
                                     let o = "";
-                                    for (let n = t.resultIndex; n < t.results.length; ++n) t.results[n].isFinal ? (e += t.results[n][0].transcript, this.inputBox.value = e) : (o += t.results[n][0].transcript, this.inputBox.value = o)
-                                }, this.speechRecognition = t, this.speechButton.onclick = () => {
-                                    o ? t.stop() : t.start()
+                                    for (let n = e.resultIndex; n < e.results.length; ++n) e.results[n].isFinal ? (t += e.results[n][0].transcript, this.inputBox.value = t) : (o += e.results[n][0].transcript, this.inputBox.value = o)
+                                }, this.speechRecognition = e, this.speechButton.onclick = () => {
+                                    o ? e.stop() : e.start()
                                 }
                             } else console.error("Speech Recognition Not Available"), this.speechButton.style.display = "none"
                         }
                         async createNode() {
-                            let t;
                             this.repo = await async function() {
-                                const t = await fetch("https://raw.githubusercontent.com/oeway/codex-chat-notebook/master/codex-prompt-repository/index.json");
-                                return await t.json()
-                            }(), this.node.innerHTML = '<h2 style="color: slategrey;font-family: monospace;">Codex Chat Notebook</h2><p>Built with OpenAI Codex, by Wei Ouyang</p>', this.node.style.padding = "10px", this.node.style.background = "white", this.node.style.height = "100%", this.node.style.overflow = "auto", this.tokenInput = document.createElement("input"), this.tokenInput.style.display = "block", this.tokenInput.style.width = "100%", this.tokenInput.style.color = "gray", this.tokenInput.type = "password", this.tokenInput.placeholder = "OpenAI API token", this.tokenInput.title = "OpenAI API token", this.promptSelect = document.createElement("select"), this.promptSelect.style.display = "block", this.promptSelect.style.width = "100%", this.promptSelect.style.marginTop = "10px", this.promptSelect.style.color = "black", this.promptSelect.title = "Prompt", this.promptDetails = document.createElement("p"), this.promptDetails.style.display = "block", this.promptDetails.style.width = "100%", this.promptDetails.style.color = "gray", this.repo.items.forEach((t => {
-                                const e = document.createElement("option");
-                                e.value = t.source, e.title = t.description, e.innerText = t.name, this.promptSelect.appendChild(e)
-                            })), this.inputBox = document.createElement("textarea"), this.inputBox.style.marginTop = "10px", this.inputBox.style.display = "block", this.inputBox.style.width = "100%", this.inputBox.style.height = "6rem", this.inputBox.style.fontSize = "16px", this.speechButton = document.createElement("button"), this.speechButton.innerHTML = "Voice", this.speechButton.style.width = "50%", this.speechButton.style.height = "20px", this.speechButton.style.fontSize = "16px", this.speechButton.style.display = "inline-block", this.speechButton.classList.add("bp3-button", "bp3-minimal", "jp-ToolbarButtonComponent", "minimal", "jp-Button"), this.undoButton = document.createElement("button"), this.undoButton.style.width = "50%", this.undoButton.style.height = "20px", this.undoButton.style.fontSize = "16px", this.undoButton.innerHTML = "Undo", this.undoButton.style.display = "inline-block", this.undoButton.classList.add("bp3-button", "bp3-minimal", "jp-ToolbarButtonComponent", "minimal", "jp-Button"), this.executeButton = document.createElement("button"), this.executeButton.innerHTML = "Execute", this.executeButton.style.display = "block", this.executeButton.style.background = "lavender", this.executeButton.style.fontSize = "16px", this.executeButton.style.width = "100%", this.executeButton.classList.add("bp3-button", "bp3-minimal", "jp-ToolbarButtonComponent", "minimal", "jp-Button"), this.node.appendChild(this.tokenInput), this.node.appendChild(this.promptSelect), this.node.appendChild(this.promptDetails), this.node.appendChild(this.inputBox), this.node.appendChild(this.speechButton), this.node.appendChild(this.undoButton), this.node.appendChild(this.executeButton), this.requestedCodeElm = document.createElement("pre"), this.requestedCodeElm.style.color = "gray", this.respondCodeElm = document.createElement("pre"), this.respondCodeElm.style.color = "blue", this.node.appendChild(this.respondCodeElm), this.node.appendChild(this.requestedCodeElm);
-                            const e = localStorage.getItem("openai-token");
-                            e && (t = new(a())(e), this.tokenInput.value = e), this.tokenInput.onchange = () => {
-                                t = new(a())(this.tokenInput.value), localStorage.setItem("openai-token", this.tokenInput.value)
-                            }, this.promptPrefix = '# Generate code for Jupyter notebooks\nI start with an empty jupyter notebook with Python 3 kernel, and incrementally add instructions for each cell. The instructions are comment string starts with "##" (with additional details are provided as quoted with """) the lines after the instructions or details should be a generated executable Python 3 code block or empty.\nThe instructions are given by a human via a speech-to-text program in a noisy environment, therefore the text maybe confusing and requires correction but the general context is using python for data analysis.\nThe result of each code block should be printed or displayed in the notebook.\n\nIn the following cases, it should generate a special command string instead of a python code block:\n - To cancel or undo last cell, generate "%undo"\n - To execute all the cells, generate "%run-all"\n - To execute the current or active cell, generate "%run"\n', this.codeExamples = '## Print hello world\nprint("Hello world")\n', p(this.repo, this.promptSelect.value).then((t => {
-                                this.promptPrefix = t.prefix, this.codeExamples = t.examples
+                                const e = await fetch("https://raw.githubusercontent.com/oeway/codex-chat-notebook/master/codex-prompt-repository/index.json");
+                                return await e.json()
+                            }(), this.node.innerHTML = '<h2 style="color: slategrey;font-family: monospace;">Chat Notebook</h2><p>Built with LLM from OpenAI, by Wei Ouyang</p>', this.node.style.padding = "10px", this.node.style.background = "white", this.node.style.height = "100%", this.node.style.overflow = "auto", this.modelSelect = document.createElement("select"), this.modelSelect.style.display = "block", this.modelSelect.style.width = "100%", this.modelSelect.style.marginTop = "10px", this.modelSelect.style.color = "black", this.modelSelect.title = "Model", this.tokenInput = document.createElement("input"), this.tokenInput.style.display = "block", this.tokenInput.style.width = "100%", this.tokenInput.style.color = "gray", this.tokenInput.type = "password", this.tokenInput.placeholder = "OpenAI API token", this.tokenInput.title = "OpenAI API token", this.promptSelect = document.createElement("select"), this.promptSelect.style.display = "block", this.promptSelect.style.width = "100%", this.promptSelect.style.marginTop = "10px", this.promptSelect.style.color = "black", this.promptSelect.title = "Prompt", this.promptDetails = document.createElement("p"), this.promptDetails.style.display = "block", this.promptDetails.style.width = "100%", this.promptDetails.style.color = "gray", this.repo.items.forEach((e => {
+                                const t = document.createElement("option");
+                                t.value = e.source, t.title = e.description, t.innerText = e.name, this.promptSelect.appendChild(t)
+                            })), this.inputBox = document.createElement("textarea"), this.inputBox.style.marginTop = "10px", this.inputBox.style.display = "block", this.inputBox.style.width = "100%", this.inputBox.style.height = "6rem", this.inputBox.style.fontSize = "16px", this.speechButton = document.createElement("button"), this.speechButton.innerHTML = "Voice", this.speechButton.style.width = "50%", this.speechButton.style.height = "20px", this.speechButton.style.fontSize = "16px", this.speechButton.style.display = "inline-block", this.speechButton.classList.add("bp3-button", "bp3-minimal", "jp-ToolbarButtonComponent", "minimal", "jp-Button"), this.undoButton = document.createElement("button"), this.undoButton.style.width = "50%", this.undoButton.style.height = "20px", this.undoButton.style.fontSize = "16px", this.undoButton.innerHTML = "Undo", this.undoButton.style.display = "inline-block", this.undoButton.classList.add("bp3-button", "bp3-minimal", "jp-ToolbarButtonComponent", "minimal", "jp-Button"), this.executeButton = document.createElement("button"), this.executeButton.innerHTML = "Execute", this.executeButton.style.display = "block", this.executeButton.style.background = "lavender", this.executeButton.style.fontSize = "16px", this.executeButton.style.width = "100%", this.executeButton.classList.add("bp3-button", "bp3-minimal", "jp-ToolbarButtonComponent", "minimal", "jp-Button"), this.node.appendChild(this.modelSelect), this.node.appendChild(this.tokenInput), this.node.appendChild(this.promptSelect), this.node.appendChild(this.promptDetails), this.node.appendChild(this.inputBox), this.node.appendChild(this.speechButton), this.node.appendChild(this.undoButton), this.node.appendChild(this.executeButton), this.requestedCodeElm = document.createElement("pre"), this.requestedCodeElm.style.color = "gray", this.respondCodeElm = document.createElement("pre"), this.respondCodeElm.style.color = "blue", this.node.appendChild(this.respondCodeElm), this.node.appendChild(this.requestedCodeElm);
+                            const e = () => {
+                                fetch("https://api.openai.com/v1/models", {
+                                    method: "GET",
+                                    headers: {
+                                        Authorization: "Bearer " + this.tokenInput.value,
+                                        "Content-Type": "application/json"
+                                    }
+                                }).then((e => e.json())).then((e => {
+                                    e.data.forEach((e => {
+                                        let t = document.createElement("option");
+                                        t.text = e.id, t.value = e.id, this.modelSelect.add(t), this.modelSelect.value = localStorage.getItem("openai-model") || "gpt-3.5-turbo"
+                                    }))
+                                })).catch((e => {
+                                    console.error("Error:", e)
+                                }))
+                            };
+                            let t;
+                            this.modelSelect.onchange = () => {
+                                localStorage.setItem("openai-model", this.modelSelect.value)
+                            };
+                            const n = localStorage.getItem("openai-token");
+                            if (n) {
+                                const o = new l.Configuration({
+                                    apiKey: n
+                                });
+                                t = new l.OpenAIApi(o), this.tokenInput.value = n, e()
+                            }
+                            this.tokenInput.onchange = () => {
+                                const o = new l.Configuration({
+                                    apiKey: this.tokenInput.value
+                                });
+                                t = new l.OpenAIApi(o), localStorage.setItem("openai-token", this.tokenInput.value), e()
+                            }, this.promptPrefix = '# Generate code for Jupyter notebooks\nI start with an empty jupyter notebook with Python 3 kernel, and incrementally add instructions for each cell. The instructions are comment string starts with "##" (with additional details are provided as quoted with """) the lines after the instructions or details should be a generated executable Python 3 code block or empty.\nThe instructions are given by a human via a speech-to-text program in a noisy environment, therefore the text maybe confusing and requires correction but the general context is using python for data analysis.\nThe result of each code block should be printed or displayed in the notebook.\n\nFor all the instructions, the generated code should be as simple as possible, and the code should be able to run in the current notebook.\nIf you are not sure about the instructions, you can ask for clarification by adding a comment line starts with "##?" and the details of the question.\n\nIn the following cases, it should generate a special command string instead of a python code block:\n - To cancel or undo last cell, generate "%undo"\n - To execute all the cells, generate "%run-all"\n - To execute the current or active cell, generate "%run"\n', this.codeExamples = '## Print hello world\nprint("Hello world")\n', d(this.repo, this.promptSelect.value).then((e => {
+                                this.promptPrefix = e.prefix, this.codeExamples = e.examples
                             })), this.promptSelect.onchange = () => {
                                 this.selectedPrompt = this.promptSelect.value;
-                                const t = this.repo.items.find((t => t.source === this.selectedPrompt));
-                                this.promptSelect.title = "Select a prompt template for your task.", this.promptDetails.innerHTML = t.description, p(this.repo, this.selectedPrompt).then((t => {
-                                    this.promptPrefix = t.prefix, this.codeExamples = t.examples
-                                })).catch((t => {
-                                    console.error(t), alert("Failed to fetch prompt: " + this.selectedPrompt)
+                                const e = this.repo.items.find((e => e.source === this.selectedPrompt));
+                                this.promptSelect.title = "Select a prompt template for your task.", this.promptDetails.innerHTML = e.description, d(this.repo, this.selectedPrompt).then((e => {
+                                    this.promptPrefix = e.prefix, this.codeExamples = e.examples
+                                })).catch((e => {
+                                    console.error(e), alert("Failed to fetch prompt: " + this.selectedPrompt)
                                 }))
                             }, this.executeButton.onclick = async () => {
                                 this.respondCodeElm.innerHTML = "", this.speechRecognition && this.speechRecognition.stop();
                                 const e = (n = this.inputBox.value.trim()) && n[0].toUpperCase() + n.slice(1);
                                 var n;
                                 if (e.length <= 0) return;
                                 const s = e.split("\n");
                                 let i = "## " + s[0].replace(/^(\#+\s)/, "");
                                 s.length > 1 && (i += '\n"""\n' + s.slice(1).join("\n") + '\n"""');
-                                const l = o.getCodeHistory(this.promptPrefix, this.codeExamples).join("\n") + `\n${i}\n`;
-                                this.requestedCodeElm.innerHTML = "==== Request Prompt ====\n" + l, this.executeButton.style.background = "LightGoldenRodYellow";
+                                const l = o.getCodeHistory("", this.codeExamples);
+                                l.unshift({
+                                    role: "system",
+                                    content: this.promptPrefix
+                                }), l.push({
+                                    role: "user",
+                                    content: i
+                                }), this.requestedCodeElm.innerHTML = "==== Request Prompt ====\n" + l.map((e => e.content)).join("\n"), this.executeButton.style.background = "LightGoldenRodYellow";
                                 try {
-                                    const n = await t.complete({
-                                        engine: "davinci-codex",
-                                        prompt: l,
-                                        maxTokens: 500,
-                                        temperature: .1,
-                                        topP: 1,
-                                        presencePenalty: 0,
-                                        frequencyPenalty: 0,
-                                        bestOf: 1,
-                                        n: 1,
-                                        stream: !1,
-                                        stop: ["## "]
+                                    const n = await t.createChatCompletion({
+                                        model: this.modelSelect.value,
+                                        messages: l,
+                                        temperature: .1
                                     });
                                     console.log(n.data);
-                                    const s = n.data.choices[0].text.trim();
+                                    const s = n.data.choices[0].message.content.trim();
                                     if (this.respondCodeElm.innerHTML = "==== Generated Code ====\n\n" + s, s.startsWith("%undo")) this.undoButton.onclick();
                                     else if (s.startsWith("%run")) o.runCell();
                                     else if (s.startsWith("%run-all")) o.runAllCells();
                                     else if (s.startsWith("%markdown")) {
-                                        const t = s.substring(10);
-                                        o.addMarkdown(t)
+                                        const e = s.substring(10);
+                                        o.addMarkdown(e)
                                     } else o.addCell("# " + e.trim(), s)
-                                } catch (t) {
-                                    console.error(t), alert(`Failed to execute: ${t}`)
+                                } catch (e) {
+                                    console.error(e), alert(`Failed to execute: ${e}`)
                                 }
                                 this.executeButton.style.background = "lavender", this.inputBox.value = ""
                             }, this.undoButton.onclick = async () => {
                                 if (this.speechRecognition && this.speechRecognition.stop(), this.inputBox.value.trim().length > 0) this.inputBox.value = "";
                                 else {
-                                    const t = o.undoCell();
-                                    this.inputBox.value = t.split("\n")[0]
+                                    const e = o.undoCell();
+                                    this.inputBox.value = e.split("\n")[0]
                                 }
-                            }, this.inputBox.addEventListener("keydown", (t => {
-                                "Enter" != t.key || t.shiftKey || (this.executeButton.onclick(), t.preventDefault())
+                            }, this.inputBox.addEventListener("keydown", (e => {
+                                "Enter" != e.key || e.shiftKey || (this.executeButton.onclick(), e.preventDefault())
                             })), this.setupSpeech()
                         }
                     }
                     const s = new i.Panel;
-                    s.id = "Codex-Chat-Panel", s.title.iconClass = "jp-RobotIcon", s.addWidget(new n), t.shell.add(s, "left", {
+                    s.id = "Codex-Chat-Panel", s.title.iconClass = "jp-RobotIcon", s.addWidget(new n), e.shell.add(s, "left", {
                         rank: 1
                     })
                 }
             }
         }
     }
 ]);
```

### Comparing `codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/747.c7879d7e9587a1c6296d.js` & `codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/747.c7879d7e9587a1c6296d.js`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/905.fd54bc0b4a42205403dc.js` & `codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/905.5c83ee4c20235cca8264.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 "use strict";
 (self.webpackChunkcodex_chat_notebook = self.webpackChunkcodex_chat_notebook || []).push([
     [905], {
         7905: (e, t, l) => {
             l.d(t, {
                 v: () => m
             });
-            var n = l(9321),
-                o = l(4166),
-                i = l(3468),
+            var n = l(6825),
+                o = l(4309),
+                i = l(8369),
                 d = l(9850),
                 c = l(1797),
                 a = l(608),
                 r = l(6168),
                 s = l(6271);
             const u = "application/vnd.jupyter.cells",
                 g = "jp-mod-sideBySide";
```

### Comparing `codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/927.21eeae7dfef6ffcebedc.js` & `codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/927.21eeae7dfef6ffcebedc.js`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/927.21eeae7dfef6ffcebedc.js.LICENSE.txt` & `codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/927.21eeae7dfef6ffcebedc.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/remoteEntry.ee0fc643ff265d1ca186.js` & `codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/remoteEntry.917c6c06846d04d0cc6e.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, o, n, a, i, l, u, s, d, c, f, p, h, v, b, m, g, y, w, k, S = {
+    var e, r, t, o, n, a, i, l, u, d, s, f, c, p, h, v, b, m, g, y, w, k, S = {
             1315: (e, r, t) => {
                 var o = {
-                        "./index": () => Promise.all([t.e(905), t.e(160), t.e(597)]).then((() => () => t(1568))),
-                        "./extension": () => Promise.all([t.e(905), t.e(160), t.e(597)]).then((() => () => t(1568))),
+                        "./index": () => Promise.all([t.e(905), t.e(160), t.e(412)]).then((() => () => t(1568))),
+                        "./extension": () => Promise.all([t.e(905), t.e(160), t.e(412)]).then((() => () => t(1568))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -45,57 +45,57 @@
         for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
         160: "393e1e430ddc2ca76517",
         223: "b54a1552aec55f828dd0",
-        267: "a5477cedb5aecf90b318",
-        597: "6a0e30da9896849c3b2d",
+        412: "a2835a83deddc2445136",
+        485: "461f1ffaed83f67adf0b",
         747: "c7879d7e9587a1c6296d",
-        905: "fd54bc0b4a42205403dc",
+        905: "5c83ee4c20235cca8264",
         927: "21eeae7dfef6ffcebedc"
     } [e] + ".js?v=" + {
         160: "393e1e430ddc2ca76517",
         223: "b54a1552aec55f828dd0",
-        267: "a5477cedb5aecf90b318",
-        597: "6a0e30da9896849c3b2d",
+        412: "a2835a83deddc2445136",
+        485: "461f1ffaed83f67adf0b",
         747: "c7879d7e9587a1c6296d",
-        905: "fd54bc0b4a42205403dc",
+        905: "5c83ee4c20235cca8264",
         927: "21eeae7dfef6ffcebedc"
     } [e], x.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "codex-chat-notebook:", x.l = (t, o, n, a) => {
         if (e[t]) e[t].push(o);
         else {
             var i, l;
             if (void 0 !== n)
-                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
-                    var d = u[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
-                        i = d;
+                for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
+                    var s = u[d];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
+                        i = s;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [o];
-            var c = (r, o) => {
-                    i.onerror = i.onload = null, clearTimeout(f);
+            var f = (r, o) => {
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(o))), r) return r(o)
                 },
-                f = setTimeout(c.bind(null, void 0, {
+                c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, x.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -117,15 +117,15 @@
                         (!l || !l.loaded && (!o != !l.eager ? o : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!o
                         })
                     },
                     u = [];
-                return "default" === t && (l("@phosphor/disposable", "1.10.1", (() => Promise.all([x.e(160), x.e(223)]).then((() => () => x(1223))))), l("codex-chat-notebook", "0.1.4", (() => Promise.all([x.e(905), x.e(160), x.e(597)]).then((() => () => x(1568))))), l("openai-api", "1.2.6", (() => x.e(267).then((() => () => x(9267)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@phosphor/disposable", "1.10.1", (() => Promise.all([x.e(160), x.e(223)]).then((() => () => x(1223))))), l("codex-chat-notebook", "0.1.5", (() => Promise.all([x.e(905), x.e(160), x.e(412)]).then((() => () => x(1568))))), l("openai", "3.2.1", (() => x.e(485).then((() => () => x(6485)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -174,85 +174,85 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var o = e[0],
                 n = o < 0;
             n && (o = -o - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var s, d, c = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !u || ("u" == c ? l > o && !n : "" == c != n);
-                if ("u" == d) {
-                    if (!u || "u" != c) return !1
+                var d, s, f = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !u || ("u" == f ? l > o && !n : "" == f != n);
+                if ("u" == s) {
+                    if (!u || "u" != f) return !1
                 } else if (u)
-                    if (c == d)
+                    if (f == s)
                         if (l <= o) {
-                            if (s != e[l]) return !1
+                            if (d != e[l]) return !1
                         } else {
-                            if (n ? s > e[l] : s < e[l]) return !1;
-                            s != e[l] && (u = !1)
+                            if (n ? d > e[l] : d < e[l]) return !1;
+                            d != e[l] && (u = !1)
                         }
-                else if ("s" != c && "n" != c) {
+                else if ("s" != f && "n" != f) {
                     if (n || l <= o) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= o || d < c != n) return !1;
+                    if (l <= o || s < f != n) return !1;
                     u = !1
-                } else "s" != c && "n" != c && (u = !1, l--)
+                } else "s" != f && "n" != f && (u = !1, l--)
             }
         }
-        var f = [],
-            p = f.pop.bind(f);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            f.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = x.S[e];
         if (!t || !x.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || o(e, r) ? r : e), 0)) && t[r]
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && o(e, r) ? r : e), 0)
-    }, s = (e, r, t) => "Unsatisfied version " + r + " of shared singleton module " + e + " (required " + n(t) + ")", d = (e, r, t, o) => {
+    }, d = (e, r, t) => "Unsatisfied version " + r + " of shared singleton module " + e + " (required " + n(t) + ")", s = (e, r, t, o) => {
         var n = u(e, t);
-        return a(o, n) || "undefined" != typeof console && console.warn && console.warn(s(t, n, o)), h(e[t][n])
-    }, c = (e, r, t) => {
+        return a(o, n) || "undefined" != typeof console && console.warn && console.warn(d(t, n, o)), h(e[t][n])
+    }, f = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !a(t, r) || e && !o(e, r) ? e : r), 0)) && n[r]
-    }, f = (e, r, t, o) => {
+    }, c = (e, r, t, o) => {
         var a = e[t];
         return "No satisfying version (" + n(o) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
     }, p = (e, r, t, o) => {
-        "undefined" != typeof console && console.warn && console.warn(f(e, r, t, o))
+        "undefined" != typeof console && console.warn && console.warn(c(e, r, t, o))
     }, h = e => (e.loaded = 1, e.get()), b = (v = e => function(r, t, o, n) {
         var a = x.I(r);
         return a && a.then ? a.then(e.bind(e, r, x.S[r], t, o, n)) : e(r, x.S[r], t, o, n)
-    })(((e, r, t, o) => (i(e, t), h(c(r, t, o) || p(r, e, t, o) || l(r, t))))), m = v(((e, r, t, o) => (i(e, t), d(r, 0, t, o)))), g = v(((e, r, t, o, n) => {
-        var a = r && x.o(r, t) && c(r, t, o);
+    })(((e, r, t, o) => (i(e, t), h(f(r, t, o) || p(r, e, t, o) || l(r, t))))), m = v(((e, r, t, o) => (i(e, t), s(r, 0, t, o)))), g = v(((e, r, t, o, n) => {
+        var a = r && x.o(r, t) && f(r, t, o);
         return a ? h(a) : n()
     })), y = {}, w = {
         6168: () => m("default", "@lumino/signaling", [1, 1, 4, 3]),
         9850: () => m("default", "@lumino/algorithm", [1, 1, 3, 3]),
         608: () => m("default", "@lumino/domutils", [1, 1, 2, 3]),
         1797: () => m("default", "@lumino/coreutils", [1, 1, 5, 3]),
         2138: () => g("default", "@phosphor/disposable", [1, 1, 3, 1], (() => x.e(927).then((() => () => x(1223))))),
-        3468: () => m("default", "@jupyterlab/translation", [1, 3, 3, 4]),
         3706: () => m("default", "@lumino/widgets", [1, 1, 19, 0]),
-        4166: () => b("default", "@jupyterlab/cells", [1, 3, 3, 4]),
+        3931: () => g("default", "openai", [1, 3, 2, 1], (() => x.e(485).then((() => () => x(6485))))),
+        4198: () => m("default", "@jupyterlab/notebook", [1, 3, 2, 4]),
+        4309: () => b("default", "@jupyterlab/cells", [1, 3, 2, 4]),
         6271: () => m("default", "react", [1, 17, 0, 1]),
-        7023: () => g("default", "openai-api", [1, 1, 2, 6], (() => x.e(267).then((() => () => x(9267))))),
-        9321: () => m("default", "@jupyterlab/apputils", [1, 3, 3, 4]),
-        9628: () => m("default", "@jupyterlab/notebook", [1, 3, 3, 4])
+        6825: () => m("default", "@jupyterlab/apputils", [1, 3, 2, 4]),
+        8369: () => m("default", "@jupyterlab/translation", [1, 3, 2, 4])
     }, k = {
         160: [6168, 9850],
-        597: [608, 1797, 2138, 3468, 3706, 4166, 6271, 7023, 9321, 9628]
+        412: [608, 1797, 2138, 3706, 3931, 4198, 4309, 6271, 6825, 8369]
     }, x.f.consumes = (e, r) => {
         x.o(k, e) && k[e].forEach((e => {
             if (x.o(y, e)) return r.push(y[e]);
             var t = r => {
                     y[e] = 0, x.m[e] = t => {
                         delete x.c[e], t.exports = r()
                     }
```

### Comparing `codex-chat-notebook-0.1.4/codex-chat-notebook/labextension/static/third-party-licenses.json` & `codex-chat-notebook-0.1.5/codex-chat-notebook/labextension/static/third-party-licenses.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8984375%*

 * *Differences: {"'packages'": "{2: {'versionInfo': '0.26.1'}, 5: {'name': 'openai', 'versionInfo': '3.2.1', "*

 * *               "'licenseId': 'MIT', 'extractedText': 'The MIT License\\n\\nCopyright (c) OpenAI "*

 * *               '(https://openai.com)\\n\\nPermission is hereby granted, free of charge, to any '*

 * *               'person obtaining a copy\\nof this software and associated documentation files (the '*

 * *               '"Software"), to deal\\nin the Software without restriction, including without '*

 * *               'limitatio […]*

```diff
@@ -12,27 +12,33 @@
             "name": "@lumino/disposable",
             "versionInfo": "1.10.1"
         },
         {
             "extractedText": "Copyright (c) 2014-present Matt Zabriskie\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "axios",
-            "versionInfo": "0.21.4"
+            "versionInfo": "0.26.1"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "5.2.7"
         },
         {
-            "extractedText": "",
-            "licenseId": "ISC",
-            "name": "openai-api",
-            "versionInfo": "1.2.6"
+            "extractedText": "Copyright (c) 2012 Felix Geisend\u00f6rfer (felix@debuggable.com) and contributors\n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n of this software and associated documentation files (the \"Software\"), to deal\n in the Software without restriction, including without limitation the rights\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n copies of the Software, and to permit persons to whom the Software is\n furnished to do so, subject to the following conditions:\n\n The above copyright notice and this permission notice shall be included in\n all copies or substantial portions of the Software.\n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\n IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\n FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\n AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\n LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\n OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\n THE SOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "form-data",
+            "versionInfo": "4.0.0"
+        },
+        {
+            "extractedText": "The MIT License\n\nCopyright (c) OpenAI (https://openai.com)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "openai",
+            "versionInfo": "3.2.1"
         },
         {
             "extractedText": "(The MIT License)\n\nCopyright (c) 2013 Roman Shtylman <shtylman@gmail.com>\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "process",
             "versionInfo": "0.11.10"
         },
```

### Comparing `codex-chat-notebook-0.1.4/codex-prompt-repository/default.md` & `codex-chat-notebook-0.1.5/codex-prompt-repository/default.md`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/codex-prompt-repository/image-analysis.md` & `codex-chat-notebook-0.1.5/codex-prompt-repository/image-analysis.md`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/codex_chat_notebook.egg-info/PKG-INFO` & `codex-chat-notebook-0.1.5/codex_chat_notebook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codex-chat-notebook
-Version: 0.1.4
+Version: 0.1.5
 Summary: Doing data science without programming skills by chatting with OpenAI Codex
 Home-page: https://github.com/oeway/codex-chat-notebook
 Author: Wei Ouyang
 Author-email: oeway007@gmail.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -93,8 +93,7 @@
 ```
 
 ```
 pip install jupyter_packaging
 npm run install:extension
 jupyter lab
 ```
-
```

### Comparing `codex-chat-notebook-0.1.4/codex_chat_notebook.egg-info/SOURCES.txt` & `codex-chat-notebook-0.1.5/codex_chat_notebook.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 .gitignore
 .prettierignore
 .prettierrc
 LICENSE
 MANIFEST.in
 README.md
 install.json
-package-lock.json
 package.json
 publish.sh
 pyproject.toml
 setup.py
 yarn.lock
 .github/workflows/build.yml
 binder/environment.yml
 binder/postBuild
 codex-chat-notebook/__init__.py
 codex-chat-notebook/_version.py
 codex-chat-notebook/labextension/package.json
 codex-chat-notebook/labextension/static/223.b54a1552aec55f828dd0.js
 codex-chat-notebook/labextension/static/223.b54a1552aec55f828dd0.js.LICENSE.txt
-codex-chat-notebook/labextension/static/267.a5477cedb5aecf90b318.js
-codex-chat-notebook/labextension/static/597.6a0e30da9896849c3b2d.js
+codex-chat-notebook/labextension/static/412.a2835a83deddc2445136.js
+codex-chat-notebook/labextension/static/485.461f1ffaed83f67adf0b.js
 codex-chat-notebook/labextension/static/747.c7879d7e9587a1c6296d.js
-codex-chat-notebook/labextension/static/905.fd54bc0b4a42205403dc.js
+codex-chat-notebook/labextension/static/905.5c83ee4c20235cca8264.js
 codex-chat-notebook/labextension/static/927.21eeae7dfef6ffcebedc.js
 codex-chat-notebook/labextension/static/927.21eeae7dfef6ffcebedc.js.LICENSE.txt
-codex-chat-notebook/labextension/static/remoteEntry.ee0fc643ff265d1ca186.js
+codex-chat-notebook/labextension/static/remoteEntry.917c6c06846d04d0cc6e.js
 codex-chat-notebook/labextension/static/style.js
 codex-chat-notebook/labextension/static/third-party-licenses.json
+codex-prompt-repository/cellpose-image-segmentation.md
 codex-prompt-repository/default.md
 codex-prompt-repository/image-analysis.md
 codex-prompt-repository/index.json
 codex_chat_notebook.egg-info/PKG-INFO
 codex_chat_notebook.egg-info/SOURCES.txt
 codex_chat_notebook.egg-info/dependency_links.txt
 codex_chat_notebook.egg-info/not-zip-safe
```

### Comparing `codex-chat-notebook-0.1.4/lib/index.js` & `codex-chat-notebook-0.1.5/lib/index.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,18 @@
 } from '@phosphor/disposable';
 
 import {
     Widget,
     Panel
 } from '@lumino/widgets';
 
-import OpenAI from 'openai-api';
+import {
+    Configuration,
+    OpenAIApi
+} from "openai";
 
 import {
     NotebookActions
 } from '@jupyterlab/notebook/lib/actions';
 
 import {
     INotebookTracker
@@ -32,14 +35,17 @@
 }
 
 const promptPrefix = `# Generate code for Jupyter notebooks
 I start with an empty jupyter notebook with Python 3 kernel, and incrementally add instructions for each cell. The instructions are comment string starts with "##" (with additional details are provided as quoted with """) the lines after the instructions or details should be a generated executable Python 3 code block or empty.
 The instructions are given by a human via a speech-to-text program in a noisy environment, therefore the text maybe confusing and requires correction but the general context is using python for data analysis.
 The result of each code block should be printed or displayed in the notebook.
 
+For all the instructions, the generated code should be as simple as possible, and the code should be able to run in the current notebook.
+If you are not sure about the instructions, you can ask for clarification by adding a comment line starts with "##?" and the details of the question.
+
 In the following cases, it should generate a special command string instead of a python code block:
  - To cancel or undo last cell, generate "%undo"
  - To execute all the cells, generate "%run-all"
  - To execute the current or active cell, generate "%run"
 `
 const codeExamples = `## Print hello world
 print("Hello world")
@@ -60,15 +66,15 @@
         notebook._sessionContex = context.sessionContext;
         let callback = () => {
             console.log(`Notebook "${notebook.title.label}" is now activated as the current chat notebook!`)
         };
         let button = new ToolbarButton({
             iconClass: 'jp-RobotIcon',
             onClick: callback,
-            tooltip: 'Codex Chat Notebook is enabled'
+            tooltip: 'Chat Notebook is enabled'
         });
         panel.toolbar.insertItem(0, 'activate', button);
 
         return new DisposableDelegate(() => {
             button.dispose();
             if (this.notebook === notebook) {
                 this.notebook = null;
@@ -113,18 +119,24 @@
         const history = [];
         let firstMarkdown = true;
         for (let i = 0; i < cells.length; i++) {
             if (i > this.notebook.activeCellIndex) break;
             const cell = cells.get(i);
             if (cell.type === 'code') {
                 if (firstMarkdown) {
-                    history.push(`\n"""\n${promptPrefix}\n"""\n${cell.value.text}\n${codeExamples}`)
+                    history.push({
+                        "role": "assistant",
+                        "content": `\n"""\n${promptPrefix}\n"""\n${cell.value.text}\n${codeExamples}`
+                    })
                     firstMarkdown = false;
                 } else {
-                    history.push(cell.value.text)
+                    history.push({
+                        "role": "assistant",
+                        "content": cell.value.text
+                    })
                 }
             } else if (cell.type === 'markdown') {
                 const text = cell.value.text;
                 let newText = "";
                 // add ## before each line in the text
                 const lines = text.split('\n');
                 newText += '## ' + lines[0].replace(/^(\#+\s)/, "");
@@ -143,15 +155,18 @@
                     if (firstMarkdown) {
                         newText += `\n${codeExamples}`;
                         firstMarkdown = false;
                     }
                 }
                 // remove leading # and add ##
                 // newText = lines.map(line => '## ' + line.replace(/^(\#+\s)/,"")).join('\n');
-                history.push(newText)
+                history.push({
+                    "role": "user",
+                    "content": newText
+                })
             }
         }
         return history
     }
 
     addCell(doc, code) {
         const notebook = this.notebook;
@@ -292,15 +307,15 @@
         );
 
         class ContentWidget extends Widget {
             constructor() {
                 super();
                 this.addClass('content');
                 this.id = 'tutorial'
-                this.title.label = 'Codex Chat Notebook'
+                this.title.label = 'Chat Notebook'
                 this.title.closable = true;
                 this.createNode()
             }
 
             setupSpeech() {
                 if ("webkitSpeechRecognition" in window) {
                     let speechRecognition = new webkitSpeechRecognition();
@@ -358,19 +373,25 @@
                     this.speechButton.style.display = "none";
                 }
             }
 
             async createNode() {
                 this.repo = await fetchPromptRepo()
 
-                this.node.innerHTML = `<h2 style="color: slategrey;font-family: monospace;">Codex Chat Notebook</h2><p>Built with OpenAI Codex, by Wei Ouyang</p>`
+                this.node.innerHTML = `<h2 style="color: slategrey;font-family: monospace;">Chat Notebook</h2><p>Built with LLM from OpenAI, by Wei Ouyang</p>`
                 this.node.style.padding = "10px"
                 this.node.style.background = "white";
                 this.node.style.height = "100%";
                 this.node.style.overflow = "auto";
+                this.modelSelect = document.createElement('select')
+                this.modelSelect.style.display = "block";
+                this.modelSelect.style.width = "100%";
+                this.modelSelect.style.marginTop = "10px";
+                this.modelSelect.style.color = "black";
+                this.modelSelect.title = "Model";
                 this.tokenInput = document.createElement('input')
                 this.tokenInput.style.display = "block";
                 this.tokenInput.style.width = "100%";
                 this.tokenInput.style.color = "gray";
                 this.tokenInput.type = "password";
                 this.tokenInput.placeholder = "OpenAI API token";
                 this.tokenInput.title = "OpenAI API token";
@@ -417,14 +438,15 @@
                 this.executeButton.innerHTML = 'Execute'
                 this.executeButton.style.display = "block";
                 this.executeButton.style.background = "lavender";
                 this.executeButton.style.fontSize = "16px";
                 this.executeButton.style.width = "100%";
                 this.executeButton.classList.add("bp3-button", "bp3-minimal", "jp-ToolbarButtonComponent", "minimal", "jp-Button")
 
+                this.node.appendChild(this.modelSelect)
                 this.node.appendChild(this.tokenInput)
                 this.node.appendChild(this.promptSelect)
                 this.node.appendChild(this.promptDetails)
                 this.node.appendChild(this.inputBox)
                 this.node.appendChild(this.speechButton)
                 this.node.appendChild(this.undoButton)
                 this.node.appendChild(this.executeButton)
@@ -432,23 +454,59 @@
                 this.requestedCodeElm = document.createElement('pre')
                 this.requestedCodeElm.style.color = 'gray'
                 this.respondCodeElm = document.createElement('pre')
                 this.respondCodeElm.style.color = 'blue'
                 this.node.appendChild(this.respondCodeElm)
                 this.node.appendChild(this.requestedCodeElm)
 
+                const updateModels = () => {
+                    fetch('https://api.openai.com/v1/models', {
+                            method: 'GET',
+                            headers: {
+                                'Authorization': 'Bearer ' + this.tokenInput.value,
+                                'Content-Type': 'application/json'
+                            }
+                        })
+                        .then(response => response.json())
+                        .then(data => {
+                            data.data.forEach(model => {
+                                let option = document.createElement('option');
+                                option.text = model.id;
+                                option.value = model.id;
+                                this.modelSelect.add(option);
+
+                                this.modelSelect.value = localStorage.getItem('openai-model') || 'gpt-3.5-turbo';
+                            });
+                        })
+                        .catch((error) => {
+                            console.error('Error:', error);
+                        });
+                }
+
+                this.modelSelect.onchange = () => {
+                    localStorage.setItem('openai-model', this.modelSelect.value);
+                }
+
                 let openai;
                 const lastToken = localStorage.getItem('openai-token');
                 if (lastToken) {
-                    openai = new OpenAI(lastToken);
+                    const configuration = new Configuration({
+                        apiKey: lastToken,
+                    });
+                    openai = new OpenAIApi(configuration);
                     this.tokenInput.value = lastToken;
+                    updateModels();
                 }
                 this.tokenInput.onchange = () => {
-                    openai = new OpenAI(this.tokenInput.value);
+                    const configuration = new Configuration({
+                        apiKey: this.tokenInput.value,
+                    });
+                    openai = new OpenAIApi(configuration);
                     localStorage.setItem('openai-token', this.tokenInput.value);
+                    updateModels();
                 }
                 // set the default prompt
                 this.promptPrefix = promptPrefix;
                 this.codeExamples = codeExamples;
                 fetchPrompt(this.repo, this.promptSelect.value).then(result => {
                     this.promptPrefix = result.prefix;
                     this.codeExamples = result.examples;
@@ -475,33 +533,35 @@
                     if (this.speechRecognition) this.speechRecognition.stop();
                     const command = capitalize(this.inputBox.value.trim())
                     if (command.length <= 0) return;
                     const lines = command.split('\n');
 
                     let formatedCommand = '## ' + lines[0].replace(/^(\#+\s)/, "");
                     if (lines.length > 1) formatedCommand += '\n"""\n' + lines.slice(1).join('\n') + '\n"""'
-                    const prompt = nbExt.getCodeHistory(this.promptPrefix, this.codeExamples).join('\n') + `\n${formatedCommand}\n`
-                    this.requestedCodeElm.innerHTML = "==== Request Prompt ====\n" + prompt
+
+                    const messages = nbExt.getCodeHistory("", this.codeExamples)
+                    messages.unshift({
+                        role: 'system',
+                        content: this.promptPrefix
+                    })
+                    messages.push({
+                        role: 'user',
+                        content: formatedCommand
+                    })
+                    this.requestedCodeElm.innerHTML = "==== Request Prompt ====\n" + messages.map((x) => x.content).join('\n')
                     this.executeButton.style.background = "LightGoldenRodYellow";
                     try {
-                        const gptResponse = await openai.complete({
-                            engine: 'davinci-codex',
-                            prompt,
-                            maxTokens: 500,
+                        const gptResponse = await openai.createChatCompletion({
+                            model: this.modelSelect.value,
+                            messages: messages,
                             temperature: 0.1,
-                            topP: 1,
-                            presencePenalty: 0,
-                            frequencyPenalty: 0,
-                            bestOf: 1,
-                            n: 1,
-                            stream: false,
-                            stop: ['## ']
                         });
+
                         console.log(gptResponse.data);
-                        const completion = gptResponse.data.choices[0].text.trim()
+                        const completion = gptResponse.data.choices[0].message['content'].trim()
                         this.respondCodeElm.innerHTML = "==== Generated Code ====\n\n" + completion
                         if (completion.startsWith('%undo')) {
                             this.undoButton.onclick();
                         } else if (completion.startsWith('%run')) {
                             nbExt.runCell()
                         } else if (completion.startsWith('%run-all')) {
                             nbExt.runAllCells()
```

### Comparing `codex-chat-notebook-0.1.4/package.json` & `codex-chat-notebook-0.1.5/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'dependencies'": "{'openai': '^3.2.1', delete: ['openai-api']}", "'version'": "'0.1.5'"}*

```diff
@@ -8,15 +8,15 @@
     },
     "dependencies": {
         "@jupyterlab/application": "^3.2.4",
         "@jupyterlab/apputils": "^3.2.4",
         "@jupyterlab/docregistry": "^3.2.4",
         "@jupyterlab/notebook": "^3.2.4",
         "@phosphor/disposable": "^1.3.1",
-        "openai-api": "^1.2.6"
+        "openai": "^3.2.1"
     },
     "description": "Doing data science without programming skills by chatting with OpenAI Codex",
     "devDependencies": {
         "@jupyterlab/builder": "^3.0.0",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2"
     },
@@ -56,9 +56,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
-    "version": "0.1.4"
+    "version": "0.1.5"
 }
```

### Comparing `codex-chat-notebook-0.1.4/setup.py` & `codex-chat-notebook-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/style/robot.svg` & `codex-chat-notebook-0.1.5/style/robot.svg`

 * *Files identical despite different names*

### Comparing `codex-chat-notebook-0.1.4/yarn.lock` & `codex-chat-notebook-0.1.5/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1245,20 +1245,20 @@
   integrity sha1-tG6JCTSpWR8tL2+G1+ap8bP+dqg=
 
 aws4@^1.8.0:
   version "1.11.0"
   resolved "https://registry.yarnpkg.com/aws4/-/aws4-1.11.0.tgz#d61f46d83b2519250e2784daf5b09479a8b41c59"
   integrity sha512-xh1Rl34h6Fi1DC2WWKfxUTVqRsNnr6LsKz2+hfwDxQJWmrx8+c7ylaqBMcHfl1U1r2dsifOvKX3LQuLNZ+XSvA==
 
-axios@^0.21.1:
-  version "0.21.4"
-  resolved "https://registry.yarnpkg.com/axios/-/axios-0.21.4.tgz#c67b90dc0568e5c1cf2b0b858c43ba28e2eda575"
-  integrity sha512-ut5vewkiu8jjGBdqpM44XxjuCjq9LAKeHVmoVfHVzy8eHgxxq8SbAVQNovDA8mVi05kP0Ea/n/UzcSHcTJQfNg==
+axios@^0.26.0:
+  version "0.26.1"
+  resolved "https://registry.yarnpkg.com/axios/-/axios-0.26.1.tgz#1ede41c51fcf51bbbd6fd43669caaa4f0495aaa9"
+  integrity sha512-fPwcX4EvnSHuInCMItEhAGnaSEXRBjtzh9fOtsE6E1G6p7vl7edEeZe11QHf18+6+9gR5PbKV/sGKNaD8YaMeA==
   dependencies:
-    follow-redirects "^1.14.0"
+    follow-redirects "^1.14.8"
 
 balanced-match@^1.0.0:
   version "1.0.2"
   resolved "https://registry.yarnpkg.com/balanced-match/-/balanced-match-1.0.2.tgz#e83e3a7e3f300b34cb9d87f615fa0cbf357690ee"
   integrity sha512-3oSeUO0TMV67hN1AmbXsK4yaqU7tjiHlbxRDZOpH0KW9+CeX4bRAaX0Anxt0tx2MrpRpWwQaPwIlISEJhYU5Pw==
 
 base64-js@^1.3.1:
@@ -1525,15 +1525,15 @@
   integrity sha512-dOy+3AuW3a2wNbZHIuMZpTcgjGuLU/uBL/ubcZF9OXbDo8ff4O8yVp5Bf0efS8uEoYo5q4Fx7dY9OgQGXgAsQA==
 
 colorette@^2.0.14:
   version "2.0.16"
   resolved "https://registry.yarnpkg.com/colorette/-/colorette-2.0.16.tgz#713b9af84fdb000139f04546bd4a93f62a5085da"
   integrity sha512-hUewv7oMjCp+wkBv5Rm0v87eJhq4woh5rSR+42YSQJKecCqgIqNkZ6lAlQms/BwHPJA5NKMRlpxPRv0n8HQW6g==
 
-combined-stream@^1.0.6, combined-stream@~1.0.6:
+combined-stream@^1.0.6, combined-stream@^1.0.8, combined-stream@~1.0.6:
   version "1.0.8"
   resolved "https://registry.yarnpkg.com/combined-stream/-/combined-stream-1.0.8.tgz#c3d45a8b34fd730631a110a8a2520682b31d5a7f"
   integrity sha512-FQN4MRfuJeHf7cBbBMJFXhKSDq+2kAArBlmRBvcvFE5BB1HZKXtSFASDhdlz9zOYwxh8lDdnvmMOe/+5cdoEdg==
   dependencies:
     delayed-stream "~1.0.0"
 
 commander@^2.20.0:
@@ -1882,19 +1882,14 @@
   resolved "https://registry.yarnpkg.com/domutils/-/domutils-2.8.0.tgz#4437def5db6e2d1f5d6ee859bd95ca7d02048135"
   integrity sha512-w96Cjofp72M5IIhpjgobBimYEfoPjx1Vx0BSX9P30WBdZW2WIKU0T1Bd0kz2eNZ9ikjKgHbEyKx8BB6H1L3h3A==
   dependencies:
     dom-serializer "^1.0.1"
     domelementtype "^2.2.0"
     domhandler "^4.2.0"
 
-dotenv@^8.2.0:
-  version "8.6.0"
-  resolved "https://registry.yarnpkg.com/dotenv/-/dotenv-8.6.0.tgz#061af664d19f7f4d8fc6e4ff9b584ce237adcb8b"
-  integrity sha512-IrPdXQsk2BbzvCBGBOTmmSH5SodmqZNt4ERAZDmW4CT+tL8VtvinqywuANaFu4bOMWki16nqf0e4oC0QIaDr/g==
-
 duplexer3@^0.1.4:
   version "0.1.4"
   resolved "https://registry.yarnpkg.com/duplexer3/-/duplexer3-0.1.4.tgz#ee01dd1cac0ed3cbc7fdbea37dc0a8f1ce002ce2"
   integrity sha1-7gHdHKwO08vH/b6jfcCo8c4ALOI=
 
 duplicate-package-checker-webpack-plugin@^3.0.0:
   version "3.0.0"
@@ -2315,24 +2310,33 @@
     path-exists "^4.0.0"
 
 flatstr@^1.0.12:
   version "1.0.12"
   resolved "https://registry.yarnpkg.com/flatstr/-/flatstr-1.0.12.tgz#c2ba6a08173edbb6c9640e3055b95e287ceb5931"
   integrity sha512-4zPxDyhCyiN2wIAtSLI6gc82/EjqZc1onI4Mz/l0pWrAlsSfYH/2ZIcU+e3oA2wDwbzIWNKwa23F8rh6+DRWkw==
 
-follow-redirects@^1.14.0:
-  version "1.14.5"
-  resolved "https://registry.yarnpkg.com/follow-redirects/-/follow-redirects-1.14.5.tgz#f09a5848981d3c772b5392309778523f8d85c381"
-  integrity sha512-wtphSXy7d4/OR+MvIFbCVBDzZ5520qV8XfPklSN5QtxuMUJZ+b0Wnst1e1lCDocfzuCkHqj8k0FpZqO+UIaKNA==
+follow-redirects@^1.14.8:
+  version "1.15.2"
+  resolved "https://registry.yarnpkg.com/follow-redirects/-/follow-redirects-1.15.2.tgz#b460864144ba63f2681096f274c4e57026da2c13"
+  integrity sha512-VQLG33o04KaQ8uYi2tVNbdrWp1QWxNNea+nmIB4EVM28v0hmP17z7aG1+wAkNzVq4KeXTq3221ye5qTJP91JwA==
 
 forever-agent@~0.6.1:
   version "0.6.1"
   resolved "https://registry.yarnpkg.com/forever-agent/-/forever-agent-0.6.1.tgz#fbc71f0c41adeb37f96c577ad1ed42d8fdacca91"
   integrity sha1-+8cfDEGt6zf5bFd60e1C2P2sypE=
 
+form-data@^4.0.0:
+  version "4.0.0"
+  resolved "https://registry.yarnpkg.com/form-data/-/form-data-4.0.0.tgz#93919daeaf361ee529584b9b31664dc12c9fa452"
+  integrity sha512-ETEklSGi5t0QMZuiXoA/Q6vcnxcLQP5vdugSpuAyi6SVGi2clPPp+xgEhuMaHC+zGgn31Kd235W35f7Hykkaww==
+  dependencies:
+    asynckit "^0.4.0"
+    combined-stream "^1.0.8"
+    mime-types "^2.1.12"
+
 form-data@~2.3.2:
   version "2.3.3"
   resolved "https://registry.yarnpkg.com/form-data/-/form-data-2.3.3.tgz#dcce52c05f644f298c6a7ab936bd724ceffbf3a6"
   integrity sha512-1lLKB2Mu3aGP1Q/2eCOx0fNbRMe7XdwktwOruhfqqd0rIJWwN4Dh+E3hrPSlDCXnSR7UtZ1N38rVXm+6+MEhJQ==
   dependencies:
     asynckit "^0.4.0"
     combined-stream "^1.0.6"
@@ -3626,21 +3630,21 @@
 onetime@^5.1.0, onetime@^5.1.2:
   version "5.1.2"
   resolved "https://registry.yarnpkg.com/onetime/-/onetime-5.1.2.tgz#d0e96ebb56b07476df1dd9c4806e5237985ca45e"
   integrity sha512-kbpaSSGJTWdAY5KPVeMOKXSrPtr8C8C7wodJbcsd51jRnmD+GZu8Y0VoU6Dm5Z4vWr0Ig/1NKuWRKf7j5aaYSg==
   dependencies:
     mimic-fn "^2.1.0"
 
-openai-api@^1.2.6:
-  version "1.2.6"
-  resolved "https://registry.yarnpkg.com/openai-api/-/openai-api-1.2.6.tgz#4821a0072c816edfef4a936ba7688239f2048606"
-  integrity sha512-8wZ3ghZQLCaNnbcfkL2E6IRqy4mDyNFSZ7/ChIldBXshtNLLth8cTyqp6qIXT+MiSssE2vXcQn18mFigXCLZBQ==
+openai@^3.2.1:
+  version "3.2.1"
+  resolved "https://registry.yarnpkg.com/openai/-/openai-3.2.1.tgz#1fa35bdf979cbde8453b43f2dd3a7d401ee40866"
+  integrity sha512-762C9BNlJPbjjlWZi4WYK9iM2tAVAv0uUp1UmI34vb0CN5T2mjB/qM6RYBmNKMh/dN9fC+bxqPwWJZUTWW052A==
   dependencies:
-    axios "^0.21.1"
-    dotenv "^8.2.0"
+    axios "^0.26.0"
+    form-data "^4.0.0"
 
 optionator@^0.8.1:
   version "0.8.3"
   resolved "https://registry.yarnpkg.com/optionator/-/optionator-0.8.3.tgz#84fa1d036fe9d3c7e21d99884b601167ec8fb495"
   integrity sha512-+IW9pACdk3XWmmTXG8m3upGUJst5XRGzxMRjXzAuJ1XnIFNvfhjjIuYkDvysnPQ7qzqVzLt78BCruntqRhWQbA==
   dependencies:
     deep-is "~0.1.3"
```

