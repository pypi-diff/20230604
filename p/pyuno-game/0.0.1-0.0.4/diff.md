# Comparing `tmp/pyuno-game-0.0.1.tar.gz` & `tmp/pyuno-game-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuno-game-0.0.1.tar", last modified: Thu Jun  1 16:46:56 2023, max compression
+gzip compressed data, was "pyuno-game-0.0.4.tar", last modified: Sun Jun  4 08:01:59 2023, max compression
```

## Comparing `pyuno-game-0.0.1.tar` & `pyuno-game-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:46:56.331327 pyuno-game-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 16:46:42.000000 pyuno-game-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-01 16:46:56.331327 pyuno-game-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 16:46:42.000000 pyuno-game-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-01 16:46:42.000000 pyuno-game-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:46:56.331327 pyuno-game-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:46:56.327327 pyuno-game-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:46:56.331327 pyuno-game-0.0.1/src/pyuno_game.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-01 16:46:56.000000 pyuno-game-0.0.1/src/pyuno_game.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-01 16:46:56.000000 pyuno-game-0.0.1/src/pyuno_game.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:46:56.000000 pyuno-game-0.0.1/src/pyuno_game.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 16:46:56.000000 pyuno-game-0.0.1/src/pyuno_game.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:46:56.331327 pyuno-game-0.0.1/src/uno/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 16:46:42.000000 pyuno-game-0.0.1/src/uno/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:46:56.331327 pyuno-game-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 16:46:42.000000 pyuno-game-0.0.1/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:01:59.550068 pyuno-game-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-04 08:01:50.000000 pyuno-game-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-04 08:01:59.550068 pyuno-game-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-04 08:01:50.000000 pyuno-game-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-04 08:01:50.000000 pyuno-game-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 08:01:59.550068 pyuno-game-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:01:59.546068 pyuno-game-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:01:59.550068 pyuno-game-0.0.4/src/pyuno_game.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-04 08:01:59.000000 pyuno-game-0.0.4/src/pyuno_game.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-04 08:01:59.000000 pyuno-game-0.0.4/src/pyuno_game.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 08:01:59.000000 pyuno-game-0.0.4/src/pyuno_game.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-04 08:01:59.000000 pyuno-game-0.0.4/src/pyuno_game.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:01:59.550068 pyuno-game-0.0.4/src/uno/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 08:01:50.000000 pyuno-game-0.0.4/src/uno/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:01:59.550068 pyuno-game-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-04 08:01:50.000000 pyuno-game-0.0.4/tests/test_placeholder.py
```

### Comparing `pyuno-game-0.0.1/LICENSE` & `pyuno-game-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuno-game-0.0.1/pyproject.toml` & `pyuno-game-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyuno-game"
-version = "0.0.1"
+version = "0.0.4"
 description = "A uno game"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "Dorapower", email = "thatisluo@outlook.com"}
 ]
 keywords = [
```

