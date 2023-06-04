# Comparing `tmp/circuitpython-display_ht16k33-0.4.1.tar.gz` & `tmp/circuitpython-display_ht16k33-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-display_ht16k33-0.4.1.tar", last modified: Wed May 31 23:35:04 2023, max compression
+gzip compressed data, was "circuitpython-display_ht16k33-0.4.2.tar", last modified: Sun Jun  4 20:23:35 2023, max compression
```

## Comparing `circuitpython-display_ht16k33-0.4.1.tar` & `circuitpython-display_ht16k33-0.4.2.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.720842 circuitpython-display_ht16k33-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.708842 circuitpython-display_ht16k33-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.712842 circuitpython-display_ht16k33-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-31 23:35:04.720842 circuitpython-display_ht16k33-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.712842 circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-31 23:35:04.000000 circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-31 23:35:04.000000 circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:35:04.000000 circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 23:35:04.000000 circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 23:35:04.000000 circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.716842 circuitpython-display_ht16k33-0.4.1/display_ht16k33/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/display_ht16k33/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/display_ht16k33/ht16k33.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/display_ht16k33/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    30459 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/display_ht16k33/segments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.716842 circuitpython-display_ht16k33-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)  1981287 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/7mwahe.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.720842 circuitpython-display_ht16k33-0.4.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/font5x8.bin
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    48491 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/segments.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.720842 circuitpython-display_ht16k33-0.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_advanced_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_segments_14x4.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_segments_count_down.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_segments_custom_chars.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_segments_marquee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_segments_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:35:04.720842 circuitpython-display_ht16k33-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:23:35.474637 circuitpython-display_ht16k33-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:23:35.462637 circuitpython-display_ht16k33-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:23:35.466637 circuitpython-display_ht16k33-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-06-04 20:23:35.474637 circuitpython-display_ht16k33-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:23:35.466637 circuitpython-display_ht16k33-0.4.2/circuitpython_display_ht16k33.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-06-04 20:23:35.000000 circuitpython-display_ht16k33-0.4.2/circuitpython_display_ht16k33.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-04 20:23:35.000000 circuitpython-display_ht16k33-0.4.2/circuitpython_display_ht16k33.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:23:35.000000 circuitpython-display_ht16k33-0.4.2/circuitpython_display_ht16k33.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-04 20:23:35.000000 circuitpython-display_ht16k33-0.4.2/circuitpython_display_ht16k33.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-04 20:23:35.000000 circuitpython-display_ht16k33-0.4.2/circuitpython_display_ht16k33.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:23:35.466637 circuitpython-display_ht16k33-0.4.2/display_ht16k33/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/display_ht16k33/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/display_ht16k33/ht16k33.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/display_ht16k33/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30459 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/display_ht16k33/segments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:23:35.470636 circuitpython-display_ht16k33-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1981287 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/7mwahe.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:23:35.474637 circuitpython-display_ht16k33-0.4.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/font5x8.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    48491 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/docs/segments.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:23:35.474637 circuitpython-display_ht16k33-0.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_advanced_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_frame_buffer_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_segments_14x4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_segments_count_down.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_segments_custom_chars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_segments_marquee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_segments_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-04 20:23:25.000000 circuitpython-display_ht16k33-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-04 20:23:15.000000 circuitpython-display_ht16k33-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 20:23:35.474637 circuitpython-display_ht16k33-0.4.2/setup.cfg
```

### Comparing `circuitpython-display_ht16k33-0.4.1/.github/workflows/build.yml` & `circuitpython-display_ht16k33-0.4.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/.github/workflows/release_gh.yml` & `circuitpython-display_ht16k33-0.4.2/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/.gitignore` & `circuitpython-display_ht16k33-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/.pre-commit-config.yaml` & `circuitpython-display_ht16k33-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/.pylintrc` & `circuitpython-display_ht16k33-0.4.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/LICENSE` & `circuitpython-display_ht16k33-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/PKG-INFO` & `circuitpython-display_ht16k33-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-display_ht16k33
-Version: 0.4.1
+Version: 0.4.2
 Summary: On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 Author-email: JDM <xxxy@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33
 Keywords: sensor,blinka,circuitpython,micropython,display_ht16k33,ht16k33,displayio,matrix,8x8,16x8,display
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-display_ht16k33-0.4.1/README.rst` & `circuitpython-display_ht16k33-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/PKG-INFO` & `circuitpython-display_ht16k33-0.4.2/circuitpython_display_ht16k33.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-display-ht16k33
-Version: 0.4.1
+Version: 0.4.2
 Summary: On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 Author-email: JDM <xxxy@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33
 Keywords: sensor,blinka,circuitpython,micropython,display_ht16k33,ht16k33,displayio,matrix,8x8,16x8,display
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/SOURCES.txt` & `circuitpython-display_ht16k33-0.4.2/circuitpython_display_ht16k33.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 docs/_static/Logo.png
 docs/_static/Logo.png.license
 docs/_static/extra_css.css
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/display_ht16k33_advanced_example.py
+examples/display_ht16k33_frame_buffer_example.py
 examples/display_ht16k33_segments_14x4.py
 examples/display_ht16k33_segments_count_down.py
 examples/display_ht16k33_segments_custom_chars.py
 examples/display_ht16k33_segments_marquee.py
 examples/display_ht16k33_segments_simpletest.py
 examples/display_ht16k33_simpletest.py
 examples/display_ht16k33_text.py
```

### Comparing `circuitpython-display_ht16k33-0.4.1/display_ht16k33/ht16k33.py` & `circuitpython-display_ht16k33-0.4.2/display_ht16k33/ht16k33.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 """
 from vectorio import Circle
 import displayio
 import ulab.numpy as np
 
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 __repo__ = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33.git"
 
 
 # pylint: disable=too-many-arguments, too-many-instance-attributes
 class HT16K33:
     """
     Main class
```

### Comparing `circuitpython-display_ht16k33-0.4.1/display_ht16k33/matrix.py` & `circuitpython-display_ht16k33-0.4.2/display_ht16k33/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 try:
     from typing import Optional, Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 __repo__ = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33.git"
 
 
 class Matrix8x8(HT16K33):
     """A single matrix.
     :param int x: x coordinates in pixels for the matrix to start. This is the top
     left corner of the first digit
```

### Comparing `circuitpython-display_ht16k33-0.4.1/display_ht16k33/segments.py` & `circuitpython-display_ht16k33-0.4.2/display_ht16k33/segments.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import displayio
 
 try:
     from typing import Optional, Dict, Tuple, Union
 except ImportError:
     pass
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 __repo__ = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33.git"
 
 
 # fmt: off
 CHARS = (
     0b00000000, 0b00000000,  #
     0b01000000, 0b00000110,  # !
```

### Comparing `circuitpython-display_ht16k33-0.4.1/docs/7mwahe.gif` & `circuitpython-display_ht16k33-0.4.2/docs/7mwahe.gif`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/docs/_static/Logo.png` & `circuitpython-display_ht16k33-0.4.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/docs/_static/favicon.ico` & `circuitpython-display_ht16k33-0.4.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/docs/conf.py` & `circuitpython-display_ht16k33-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/docs/examples.rst` & `circuitpython-display_ht16k33-0.4.2/docs/examples.rst`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,26 @@
 Marquee 14x4 example
 ------------------------------
 
 Marquee 14x4 example
 
 .. literalinclude:: ../examples/display_ht16k33_segments_marquee.py
     :caption: examples/display_ht16k33_segments_marquee.py
+    :lines: 5-
 
 Advanced Example
 ------------------------------
 
 Advanced Example
 
 .. literalinclude:: ../examples/display_ht16k33_advanced_example.py
     :caption: examples/display_ht16k33_advanced_example.py
+    :lines: 7-
+
+FrameBuffer Example
+------------------------------
+
+FrameBuffer Example
+
+.. literalinclude:: ../examples/display_ht16k33_frame_buffer_example.py
+    :caption: examples/display_ht16k33_frame_buffer_example.py
+    :lines: 5-
```

### Comparing `circuitpython-display_ht16k33-0.4.1/docs/font5x8.bin` & `circuitpython-display_ht16k33-0.4.2/docs/font5x8.bin`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/docs/segments.jpg` & `circuitpython-display_ht16k33-0.4.2/docs/segments.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_advanced_example.py` & `circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_advanced_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_segments_custom_chars.py` & `circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_segments_custom_chars.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_segments_simpletest.py` & `circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_segments_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_simpletest.py` & `circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_text.py` & `circuitpython-display_ht16k33-0.4.2/examples/display_ht16k33_text.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.1/pyproject.toml` & `circuitpython-display_ht16k33-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-display_ht16k33"
 description = "On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices."
-version = "0.4.1"
+version = "0.4.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxxy@mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33"}
 keywords = [
     "sensor",
```

