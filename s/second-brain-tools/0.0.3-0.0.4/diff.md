# Comparing `tmp/second_brain_tools-0.0.3.tar.gz` & `tmp/second_brain_tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "second_brain_tools-0.0.3.tar", last modified: Mon Dec 26 09:51:28 2022, max compression
+gzip compressed data, was "second_brain_tools-0.0.4.tar", last modified: Sun Jun  4 16:47:58 2023, max compression
```

## Comparing `second_brain_tools-0.0.3.tar` & `second_brain_tools-0.0.4.tar`

### file list

```diff
@@ -1,58 +1,67 @@
-drwxr-xr-x   0 rohan     (1000) rohan     (1000)        0 2022-12-26 09:51:28.466974 second_brain_tools-0.0.3/
--rw-r--r--   0 rohan     (1000) rohan     (1000)      530 2022-12-26 09:08:02.000000 second_brain_tools-0.0.3/.bumpversion.cfg
--rw-r--r--   0 rohan     (1000) rohan     (1000)     3032 2022-12-26 09:08:02.000000 second_brain_tools-0.0.3/.cookiecutterrc
--rw-r--r--   0 rohan     (1000) rohan     (1000)      186 2022-11-19 17:02:54.000000 second_brain_tools-0.0.3/.coveragerc
--rw-r--r--   0 rohan     (1000) rohan     (1000)      353 2022-11-18 04:16:07.000000 second_brain_tools-0.0.3/.editorconfig
--rw-r--r--   0 rohan     (1000) rohan     (1000)      636 2022-11-18 04:16:07.000000 second_brain_tools-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 rohan     (1000) rohan     (1000)       48 2022-12-17 17:35:08.000000 second_brain_tools-0.0.3/AUTHORS.rst
--rw-r--r--   0 rohan     (1000) rohan     (1000)       86 2022-12-17 17:35:13.000000 second_brain_tools-0.0.3/CHANGELOG.rst
--rw-r--r--   0 rohan     (1000) rohan     (1000)     5218 2022-12-17 17:35:16.000000 second_brain_tools-0.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 rohan     (1000) rohan     (1000)     2471 2022-12-17 17:35:20.000000 second_brain_tools-0.0.3/CONTRIBUTING.rst
--rw-r--r--   0 rohan     (1000) rohan     (1000)      588 2022-12-17 17:35:28.000000 second_brain_tools-0.0.3/LICENSE
--rw-r--r--   0 rohan     (1000) rohan     (1000)      502 2022-12-17 17:35:33.000000 second_brain_tools-0.0.3/MANIFEST.in
--rw-r--r--   0 rohan     (1000) rohan     (1000)     2349 2022-12-26 09:51:28.466974 second_brain_tools-0.0.3/PKG-INFO
--rw-r--r--   0 rohan     (1000) rohan     (1000)     3240 2022-12-26 09:33:31.000000 second_brain_tools-0.0.3/README.rst
--rw-r--r--   0 rohan     (1000) rohan     (1000)      619 2022-12-17 17:35:48.000000 second_brain_tools-0.0.3/SECURITY.md
-drwxr-xr-x   0 rohan     (1000) rohan     (1000)        0 2022-12-26 09:51:28.420308 second_brain_tools-0.0.3/ci/
--rwxr-xr-x   0 rohan     (1000) rohan     (1000)     2930 2022-11-18 04:16:07.000000 second_brain_tools-0.0.3/ci/bootstrap.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)       85 2022-12-12 15:21:30.000000 second_brain_tools-0.0.3/ci/requirements.txt
-drwxr-xr-x   0 rohan     (1000) rohan     (1000)        0 2022-12-26 09:51:28.390309 second_brain_tools-0.0.3/ci/templates/
-drwxr-xr-x   0 rohan     (1000) rohan     (1000)        0 2022-12-26 09:51:28.390309 second_brain_tools-0.0.3/ci/templates/.github/
-drwxr-xr-x   0 rohan     (1000) rohan     (1000)        0 2022-12-26 09:51:28.426975 second_brain_tools-0.0.3/ci/templates/.github/workflows/
--rw-r--r--   0 rohan     (1000) rohan     (1000)     1855 2022-11-18 04:16:07.000000 second_brain_tools-0.0.3/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 rohan     (1000) rohan     (1000)        0 2022-12-26 09:51:28.426975 second_brain_tools-0.0.3/docs/
--rw-r--r--   0 rohan     (1000) rohan     (1000)      491 2022-12-25 10:02:55.000000 second_brain_tools-0.0.3/docs/index.md
--rw-r--r--   0 rohan     (1000) rohan     (1000)      160 2022-12-17 17:35:39.000000 second_brain_tools-0.0.3/pyproject.toml
--rw-r--r--   0 rohan     (1000) rohan     (1000)      783 2022-12-17 17:35:42.000000 second_brain_tools-0.0.3/pytest.ini
--rw-r--r--   0 rohan     (1000) rohan     (1000)      324 2022-12-26 09:51:28.470307 second_brain_tools-0.0.3/setup.cfg
--rwxr-xr-x   0 rohan     (1000) rohan     (1000)     3232 2022-12-26 09:17:22.000000 second_brain_tools-0.0.3/setup.py
-drwxr-xr-x   0 rohan     (1000) rohan     (1000)        0 2022-12-26 09:51:28.393642 second_brain_tools-0.0.3/src/
-drwxr-xr-x   0 rohan     (1000) rohan     (1000)        0 2022-12-26 09:51:28.453641 second_brain_tools-0.0.3/src/second_brain_tools/
--rw-r--r--   0 rohan     (1000) rohan     (1000)    38019 2022-12-26 09:23:01.000000 second_brain_tools-0.0.3/src/second_brain_tools/.sbt_config
--rw-r--r--   0 rohan     (1000) rohan     (1000)      117 2022-12-26 09:17:21.000000 second_brain_tools-0.0.3/src/second_brain_tools/__init__.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)      407 2022-12-17 17:35:59.000000 second_brain_tools-0.0.3/src/second_brain_tools/__main__.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)     6234 2022-12-26 09:08:02.000000 second_brain_tools-0.0.3/src/second_brain_tools/append.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)    38361 2022-12-25 17:22:43.000000 second_brain_tools-0.0.3/src/second_brain_tools/capture.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)     9480 2022-12-25 17:19:46.000000 second_brain_tools-0.0.3/src/second_brain_tools/cli.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)    46579 2022-12-26 09:08:02.000000 second_brain_tools-0.0.3/src/second_brain_tools/config.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)   350029 2022-12-26 09:08:02.000000 second_brain_tools-0.0.3/src/second_brain_tools/daily_note.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)    68442 2022-12-26 09:08:02.000000 second_brain_tools-0.0.3/src/second_brain_tools/defaults.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)    27669 2022-12-26 09:08:02.000000 second_brain_tools-0.0.3/src/second_brain_tools/directories.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)     2334 2022-12-26 09:08:02.000000 second_brain_tools-0.0.3/src/second_brain_tools/misc.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)     1400 2022-12-24 09:23:29.000000 second_brain_tools-0.0.3/src/second_brain_tools/notes.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)      779 2022-12-24 09:23:34.000000 second_brain_tools-0.0.3/src/second_brain_tools/quick_capture.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)   165846 2022-12-26 09:08:02.000000 second_brain_tools-0.0.3/src/second_brain_tools/routines.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)    64528 2022-12-25 17:36:52.000000 second_brain_tools-0.0.3/src/second_brain_tools/setup.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)      287 2022-12-24 09:24:02.000000 second_brain_tools-0.0.3/src/second_brain_tools/time.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)      557 2022-12-24 09:24:12.000000 second_brain_tools-0.0.3/src/second_brain_tools/url.py
-drwxr-xr-x   0 rohan     (1000) rohan     (1000)        0 2022-12-26 09:51:28.463641 second_brain_tools-0.0.3/src/second_brain_tools.egg-info/
--rw-r--r--   0 rohan     (1000) rohan     (1000)     2349 2022-12-26 09:51:28.000000 second_brain_tools-0.0.3/src/second_brain_tools.egg-info/PKG-INFO
--rw-r--r--   0 rohan     (1000) rohan     (1000)     1272 2022-12-26 09:51:28.000000 second_brain_tools-0.0.3/src/second_brain_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rohan     (1000) rohan     (1000)        1 2022-12-26 09:51:28.000000 second_brain_tools-0.0.3/src/second_brain_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rohan     (1000) rohan     (1000)      101 2022-12-26 09:51:28.000000 second_brain_tools-0.0.3/src/second_brain_tools.egg-info/entry_points.txt
--rw-r--r--   0 rohan     (1000) rohan     (1000)        1 2022-11-20 16:56:05.000000 second_brain_tools-0.0.3/src/second_brain_tools.egg-info/not-zip-safe
--rw-r--r--   0 rohan     (1000) rohan     (1000)       41 2022-12-26 09:51:28.000000 second_brain_tools-0.0.3/src/second_brain_tools.egg-info/requires.txt
--rw-r--r--   0 rohan     (1000) rohan     (1000)       19 2022-12-26 09:51:28.000000 second_brain_tools-0.0.3/src/second_brain_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rohan     (1000) rohan     (1000)        0 2022-12-26 09:51:28.466974 second_brain_tools-0.0.3/tests/
--rw-r--r--   0 rohan     (1000) rohan     (1000)    31981 2022-12-15 10:16:14.000000 second_brain_tools-0.0.3/tests/test_second_brain_tools.py
--rw-r--r--   0 rohan     (1000) rohan     (1000)     1624 2022-12-17 17:35:59.000000 second_brain_tools-0.0.3/tox.ini
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-04 16:47:58.739126 second_brain_tools-0.0.4/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      508 2023-06-04 16:28:59.000000 second_brain_tools-0.0.4/.bumpversion.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3032 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/.cookiecutterrc
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      186 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/.coveragerc
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      353 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/.editorconfig
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      636 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/.pre-commit-config.yaml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       48 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/AUTHORS.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      508 2023-06-04 16:47:50.000000 second_brain_tools-0.0.4/CHANGELOG.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5218 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2471 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/CONTRIBUTING.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      588 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      501 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4649 2023-06-04 16:47:58.739126 second_brain_tools-0.0.4/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4128 2023-06-04 16:30:05.000000 second_brain_tools-0.0.4/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2825 2023-06-04 16:34:58.000000 second_brain_tools-0.0.4/README.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      619 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/SECURITY.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-04 16:47:58.699126 second_brain_tools-0.0.4/ci/
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)     2930 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/ci/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       85 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/ci/requirements.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-04 16:47:58.683126 second_brain_tools-0.0.4/ci/templates/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-04 16:47:58.683126 second_brain_tools-0.0.4/ci/templates/.github/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-04 16:47:58.699126 second_brain_tools-0.0.4/ci/templates/.github/workflows/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1855 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/ci/templates/.github/workflows/github-actions.yml
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-04 16:47:58.707126 second_brain_tools-0.0.4/docs/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1048 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/docs/Bullet-Journal.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1189 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/docs/Capture.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/docs/Config-File.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1791 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/docs/Config.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/docs/Daily-Note.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/docs/Notes.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/docs/Quick-Capture.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/docs/Random-Note.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1514 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/docs/index.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      160 2023-06-04 16:27:54.000000 second_brain_tools-0.0.4/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      783 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/pytest.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      324 2023-06-04 16:47:58.743126 second_brain_tools-0.0.4/setup.cfg
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)     3188 2023-06-04 16:39:10.000000 second_brain_tools-0.0.4/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-04 16:47:58.683126 second_brain_tools-0.0.4/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-04 16:47:58.731126 second_brain_tools-0.0.4/src/second_brain_tools/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    38019 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/.sbt_config
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      117 2023-06-04 16:30:05.000000 second_brain_tools-0.0.4/src/second_brain_tools/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      407 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/__main__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6234 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/append.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    38361 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/capture.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9480 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/cli.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    46579 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   350029 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/daily_note.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68442 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/defaults.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27669 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/directories.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2334 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/misc.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1400 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/notes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      779 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/quick_capture.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   165846 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/routines.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    64533 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/setup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      287 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/time.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      557 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/src/second_brain_tools/url.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-04 16:47:58.739126 second_brain_tools-0.0.4/src/second_brain_tools.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4649 2023-06-04 16:47:58.000000 second_brain_tools-0.0.4/src/second_brain_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1431 2023-06-04 16:47:58.000000 second_brain_tools-0.0.4/src/second_brain_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-04 16:47:58.000000 second_brain_tools-0.0.4/src/second_brain_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      101 2023-06-04 16:47:58.000000 second_brain_tools-0.0.4/src/second_brain_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-04 16:24:03.000000 second_brain_tools-0.0.4/src/second_brain_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       41 2023-06-04 16:47:58.000000 second_brain_tools-0.0.4/src/second_brain_tools.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       19 2023-06-04 16:47:58.000000 second_brain_tools-0.0.4/src/second_brain_tools.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-04 16:47:58.739126 second_brain_tools-0.0.4/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    31981 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/tests/test_second_brain_tools.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1624 2023-06-04 16:23:40.000000 second_brain_tools-0.0.4/tox.ini
```

### Comparing `second_brain_tools-0.0.3/.cookiecutterrc` & `second_brain_tools-0.0.4/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/.pre-commit-config.yaml` & `second_brain_tools-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/CODE_OF_CONDUCT.md` & `second_brain_tools-0.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/CONTRIBUTING.rst` & `second_brain_tools-0.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/LICENSE` & `second_brain_tools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/SECURITY.md` & `second_brain_tools-0.0.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/ci/bootstrap.py` & `second_brain_tools-0.0.4/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/ci/templates/.github/workflows/github-actions.yml` & `second_brain_tools-0.0.4/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/pytest.ini` & `second_brain_tools-0.0.4/pytest.ini`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/setup.py` & `second_brain_tools-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 def read(*names, **kwargs):
     with io.open(join(dirname(__file__), *names), encoding=kwargs.get('encoding', 'utf8')) as fh:
         return fh.read()
 
 
 setup(
     name='second_brain_tools',
-    version='0.0.3',
+    version='0.0.4',
     license='Apache-2.0',
     description="""This project is a toolset for Second Brain,
     This would help us to quickly and more efficiently create notes using Second Brain Vault.
     """,
     long_description='{}\n{}'.format(
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst')),
     ),
     author='Rohan Batra',
-    author_email='me@rohanbatra.in',
+    author_email='contact@rohanbatra.in',
     url='https://github.com/rohanbatrain/Second-Brain-Tools',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
@@ -44,15 +44,14 @@
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: Unix',
         'Operating System :: POSIX',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         # uncomment if you test on these interpreters:
```

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/.sbt_config` & `second_brain_tools-0.0.4/src/second_brain_tools/.sbt_config`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/append.py` & `second_brain_tools-0.0.4/src/second_brain_tools/append.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/capture.py` & `second_brain_tools-0.0.4/src/second_brain_tools/capture.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/cli.py` & `second_brain_tools-0.0.4/src/second_brain_tools/cli.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/config.py` & `second_brain_tools-0.0.4/src/second_brain_tools/config.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/daily_note.py` & `second_brain_tools-0.0.4/src/second_brain_tools/daily_note.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/defaults.py` & `second_brain_tools-0.0.4/src/second_brain_tools/defaults.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/directories.py` & `second_brain_tools-0.0.4/src/second_brain_tools/directories.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/misc.py` & `second_brain_tools-0.0.4/src/second_brain_tools/misc.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/notes.py` & `second_brain_tools-0.0.4/src/second_brain_tools/notes.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/quick_capture.py` & `second_brain_tools-0.0.4/src/second_brain_tools/quick_capture.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/routines.py` & `second_brain_tools-0.0.4/src/second_brain_tools/routines.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/setup.py` & `second_brain_tools-0.0.4/src/second_brain_tools/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from git.repo.base import Repo
 from rich import print
 # Importing production modules finished
 
 
 # Default variable assignation started.
-DEFAULT_GIT_URL = "https://github.com/rohanbatrain/Second-Brain"
+DEFAULT_GIT_URL = "https://github.com/rohanbatrain/Second-Brain-2022"
 NO_VAULT = f"""A Second Brain Vault is required in order to run this script
 \n You can get a copy from : {DEFAULT_GIT_URL}"""
 # Default variable assignation completed
 
 
 # Default Warnings assignation started
 Warning_WAP = "Wrong argument passed"
```

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools/url.py` & `second_brain_tools-0.0.4/src/second_brain_tools/url.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/src/second_brain_tools.egg-info/SOURCES.txt` & `second_brain_tools-0.0.4/src/second_brain_tools.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,33 @@
 .pre-commit-config.yaml
 AUTHORS.rst
 CHANGELOG.rst
 CODE_OF_CONDUCT.md
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
+README.md
 README.rst
 SECURITY.md
 pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
 tox.ini
 ci/bootstrap.py
 ci/requirements.txt
 ci/templates/.github/workflows/github-actions.yml
+docs/Bullet-Journal.md
+docs/Capture.md
+docs/Config-File.md
+docs/Config.md
+docs/Daily-Note.md
+docs/Notes.md
+docs/Quick-Capture.md
+docs/Random-Note.md
 docs/index.md
 src/second_brain_tools/.sbt_config
 src/second_brain_tools/__init__.py
 src/second_brain_tools/__main__.py
 src/second_brain_tools/append.py
 src/second_brain_tools/capture.py
 src/second_brain_tools/cli.py
```

### Comparing `second_brain_tools-0.0.3/tests/test_second_brain_tools.py` & `second_brain_tools-0.0.4/tests/test_second_brain_tools.py`

 * *Files identical despite different names*

### Comparing `second_brain_tools-0.0.3/tox.ini` & `second_brain_tools-0.0.4/tox.ini`

 * *Files identical despite different names*

