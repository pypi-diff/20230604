# Comparing `tmp/astro_ghost-2.0.0.tar.gz` & `tmp/astro_ghost-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-2.0.0.tar", last modified: Mon May 22 16:29:32 2023, max compression
+gzip compressed data, was "astro_ghost-2.0.1.tar", last modified: Sun Jun  4 03:58:04 2023, max compression
```

## Comparing `astro_ghost-2.0.0.tar` & `astro_ghost-2.0.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.045274 astro_ghost-2.0.0/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:31.984802 astro_ghost-2.0.0/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:31.989967 astro_ghost-2.0.0/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      626 2023-05-09 16:17:11.000000 astro_ghost-2.0.0/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-22 16:29:32.045579 astro_ghost-2.0.0/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3488 2023-05-10 20:43:06.000000 astro_ghost-2.0.0/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.027095 astro_ghost-2.0.0/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    20843 2023-05-22 16:28:30.000000 astro_ghost-2.0.0/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.0/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    38679 2023-05-22 16:28:56.000000 astro_ghost-2.0.0/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.0/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.0/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.0/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.0/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-05-22 16:29:06.000000 astro_ghost-2.0.0/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.0/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    40036 2023-05-22 16:28:35.000000 astro_ghost-2.0.0/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32867 2023-05-22 05:22:39.000000 astro_ghost-2.0.0/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.0/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-2.0.0/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-05-22 16:28:44.000000 astro_ghost-2.0.0/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     7779 2023-05-22 06:06:54.000000 astro_ghost-2.0.0/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4611 2023-05-11 04:35:06.000000 astro_ghost-2.0.0/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.0/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.029362 astro_ghost-2.0.0/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4089 2023-05-22 16:29:31.000000 astro_ghost-2.0.0/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-05-22 16:29:31.000000 astro_ghost-2.0.0/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-22 16:29:31.000000 astro_ghost-2.0.0/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-22 16:29:31.000000 astro_ghost-2.0.0/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-05-22 16:29:31.000000 astro_ghost-2.0.0/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-05-22 16:29:31.000000 astro_ghost-2.0.0/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.032057 astro_ghost-2.0.0/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.0/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.0/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.038457 astro_ghost-2.0.0/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.0/docs/source/associationmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.0/docs/source/basicusage.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.0/docs/source/catalogmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.0/docs/source/detailedtutorials.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.0/docs/source/installation.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.0/docs/source/preprocessingmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.0/docs/source/supplementalmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.0/docs/source/wrappermodules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.040850 astro_ghost-2.0.0/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.0/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-05-22 16:29:32.046539 astro_ghost-2.0.0/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-05-22 16:29:19.000000 astro_ghost-2.0.0/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-22 16:29:32.044257 astro_ghost-2.0.0/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.0/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.0/tests/debug.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.0/tests/pytest.ini
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4213 2023-05-22 05:37:16.000000 astro_ghost-2.0.0/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1343 2023-05-22 03:39:53.000000 astro_ghost-2.0.0/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.988061 astro_ghost-2.0.1/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.920248 astro_ghost-2.0.1/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.926281 astro_ghost-2.0.1/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      587 2023-05-24 04:50:38.000000 astro_ghost-2.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-04 03:58:04.988323 astro_ghost-2.0.1/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.0.1/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.965719 astro_ghost-2.0.1/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    21836 2023-06-04 03:47:53.000000 astro_ghost-2.0.1/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.1/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    38679 2023-05-22 16:28:56.000000 astro_ghost-2.0.1/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.1/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.1/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.1/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.1/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-06-04 03:56:11.000000 astro_ghost-2.0.1/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.1/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    39826 2023-05-23 03:25:58.000000 astro_ghost-2.0.1/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.0.1/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.1/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-2.0.1/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-05-22 16:28:44.000000 astro_ghost-2.0.1/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     7737 2023-05-24 04:44:13.000000 astro_ghost-2.0.1/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.0.1/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.1/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.969469 astro_ghost-2.0.1/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-04 03:58:04.000000 astro_ghost-2.0.1/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-06-04 03:58:04.000000 astro_ghost-2.0.1/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-04 03:58:04.000000 astro_ghost-2.0.1/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-04 03:58:04.000000 astro_ghost-2.0.1/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-06-04 03:58:04.000000 astro_ghost-2.0.1/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-06-04 03:58:04.000000 astro_ghost-2.0.1/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.972875 astro_ghost-2.0.1/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.1/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.1/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.981314 astro_ghost-2.0.1/docs/source/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.1/docs/source/associationmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.1/docs/source/basicusage.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.1/docs/source/catalogmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.1/docs/source/detailedtutorials.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.1/docs/source/installation.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.1/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.1/docs/source/supplementalmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.1/docs/source/wrappermodules.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.984071 astro_ghost-2.0.1/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-06-04 03:58:04.989543 astro_ghost-2.0.1/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-06-04 03:56:21.000000 astro_ghost-2.0.1/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.987136 astro_ghost-2.0.1/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.1/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.1/tests/debug.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.1/tests/pytest.ini
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4213 2023-05-22 05:37:16.000000 astro_ghost-2.0.1/tests/test_tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1391 2023-05-24 04:36:02.000000 astro_ghost-2.0.1/tox.ini
```

### Comparing `astro_ghost-2.0.0/.github/workflows/tests.yml` & `astro_ghost-2.0.1/.github/workflows/tests.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-name: Run template tests
+name: unit tests
 
 on: [push]
 
 jobs:
   build:
-    runs-on: [ubuntu-latest, macos-latest, windows-latest]
+    runs-on: [macos-latest]
 
     steps:
     - uses: actions/checkout@v1
 
     - name: Set up Python 3.7
       uses: actions/setup-python@v1
       with:
```

### Comparing `astro_ghost-2.0.0/.gitignore` & `astro_ghost-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/PKG-INFO` & `astro_ghost-2.0.1/astro_ghost.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: astro_ghost
-Version: 2.0.0
+Name: astro-ghost
+Version: 2.0.1
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,14 +25,18 @@
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
 
 .. image:: https://img.shields.io/pypi/dm/astro-ghost
    :target: https://pypi.org/project/astro-ghost/
    :alt: PyPI
 
+.. image:: https://github.com/uiucsn/astro_ghost/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/uiucsn/astro_ghost/actions/workflows/tests.yml
+   :alt: Unit Tests
+
 .. image:: https://img.shields.io/readthedocs/uiucsnastro-ghost
    :target: https://uiucsnastro-ghost.readthedocs.io/en/latest/
    :alt: Read the Docs
 
 "At the last dim horizon, we search among ghostly errors of observations for
 landmarks that are scarcely more substantial. The search will continue. The
 urge is older than history. It is not satisfied and it will not be oppressed."
```

### Comparing `astro_ghost-2.0.0/README.rst` & `astro_ghost-2.0.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,18 @@
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
 
 .. image:: https://img.shields.io/pypi/dm/astro-ghost
    :target: https://pypi.org/project/astro-ghost/
    :alt: PyPI
 
+.. image:: https://github.com/uiucsn/astro_ghost/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/uiucsn/astro_ghost/actions/workflows/tests.yml
+   :alt: Unit Tests
+
 .. image:: https://img.shields.io/readthedocs/uiucsnastro-ghost
    :target: https://uiucsnastro-ghost.readthedocs.io/en/latest/
    :alt: Read the Docs
 
 "At the last dim horizon, we search among ghostly errors of observations for
 landmarks that are scarcely more substantial. The search will continue. The
 urge is older than history. It is not satisfied and it will not be oppressed."
```

### Comparing `astro_ghost-2.0.0/astro_ghost/DLR.py` & `astro_ghost-2.0.1/astro_ghost/DLR.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,49 +23,50 @@
 
     :param host_df: The dataframe containing the candidate host galaxy (should just be one galaxy).
     :type host_df: Pandas DataFrame
     :return: The PS1 band with the highest S/N.
     :rtype: str
     """
 
+    host_df.reset_index(inplace=True, drop=True)
     bands = 'grizy'
     SNR = []
     try:
         for band in bands:
-             SNR.append(float(1/host_df["%sKronMagErr"%band]))
+             SNR.append(float(1/host_df.iloc[0, "%sKronMagErr"%band]))
         i = np.nanargmax(np.array(SNR))
     except:
         #if we have issues getting the band with the highest SNR, just use r-band
         i = 1
     return bands[i]
 
 def calc_DLR_glade(ra_SN, dec_SN, ra_host, dec_host, r_a, a_over_b, phi):
-    """TODO: Short summary.
+    """Calculates the DLR between transients and GLADE host galaxy candidates.
 
-    Parameters
-    ----------
-    ra_SN : type
-        Description of parameter `ra_SN`.
-    dec_SN : type
-        Description of parameter `dec_SN`.
-    ra_host : type
-        Description of parameter `ra_host`.
-    dec_host : type
-        Description of parameter `dec_host`.
-    r_a : type
-        Description of parameter `r_a`.
-    a_over_b : type
-        Description of parameter `a_over_b`.
-    phi : type
-        Description of parameter `phi`.
-
-    Returns
-    -------
-    type
-        Description of returned object.
+    (very similar to calc_DLR but the parameters are calculated slightly
+    differently)
+
+    :param ra_SN: The right ascension of the SN, in degrees.
+    :type ra_SN: float
+    :param dec_SN: The declination of the SN, in degrees.
+    :type dec_SN: float
+    :param ra_host: The right ascension of the host, in degrees.
+    :type ra_host: float
+    :param dec_host: The declination of the host, in degrees.
+    :type dec_host: float
+    :param r_a: The semi-major axis of the host in arcseconds.
+    :type r_a: float
+    :param a_over_b: The candidate host axis ratio.
+    :type a_over_b: float
+    :param phi: The galaxy position angle (in radians).
+    :type phi: float
+    :return: The angular separation between galaxy and transient, in arcseconds.
+    :rtype: float
+    :return: The normalized distance (angular separation divided by the DLR).
+    :rtype: float
 
     """
     xr = (ra_SN- float(ra_host))*3600
     yr = (dec_SN - float(dec_host))*3600
 
     SNcoord = SkyCoord(ra_SN*u.deg, dec_SN*u.deg, frame='icrs')
     hostCoord = SkyCoord(ra_host*u.deg, dec_host*u.deg, frame='icrs')
@@ -109,35 +110,37 @@
     :type best_band: str
     :return: The angular separation between galaxy and transient, in arcseconds.
     :rtype: float
     :return: The normalized distance (angular separation divided by the DLR).
     :rtype: float
     """
 
+    source.reset_index(inplace=True, drop=True)
+
     xr = (ra_SN.deg - float(ra_host))*3600
     yr = (dec_SN.deg - float(dec_host))*3600
 
     SNcoord = SkyCoord(ra_SN, dec_SN, frame='icrs')
     hostCoord = SkyCoord(ra_host*u.deg, dec_host*u.deg, frame='icrs')
     sep = SNcoord.separation(hostCoord)
     dist = sep.arcsecond
     badR = 10000000000.0
 
-    XX = best_band + 'momentXX'
-    YY = best_band + 'momentYY'
-    XY = best_band + 'momentXY'
+    XX = float(source.loc[0, best_band + 'momentXX'])
+    YY = float(source.loc[0, best_band + 'momentYY'])
+    XY = float(source.loc[0, best_band + 'momentXY'])
 
     # if we don't have spatial information, get rid of it
     # this gets rid of lots of artifacts without radius information
-    if (float(source[XX]) != float(source[XX])) | (float(source[XY]) != float(source[XY])) | \
-        (float(source[YY]) != float(source[YY])):
+    if (XX != XX) | (XY != XY) | \
+        (YY != YY):
         return dist, badR
 
-    U = float(source[XY])
-    Q = float(source[XX]) - float(source[YY])
+    U = XY
+    Q = XX - YY
     if Q == 0:
         return dist, badR
 
     phi = 0.5*np.arctan(U/Q)
     kappa = Q**2 + U**2
     a_over_b = (1 + kappa + 2*np.sqrt(kappa))/(1 - kappa)
 
@@ -280,16 +283,16 @@
                         GDflag = 1
 
                         if ":" in str(transient_df["RA"].values):
                             ra_SN = Angle(transient_df["RA"].values, unit=u.hourangle)
                         else:
                             ra_SN = Angle(transient_df["RA"].values, unit=u.deg)
                         dec_SN = Angle(transient_df["DEC"].values, unit=u.degree)
-                        ra_host = host_df['raMean']
-                        dec_host = host_df['decMean']
+                        ra_host = host_df['raMean'].values[0]
+                        dec_host = host_df['decMean'].values[0]
                         if len(np.array(ra_SN)) > 1:
                             ra_SN = ra_SN[0]
                             dec_SN = dec_SN[0]
                         if (dec_SN.deg > -30):
                             band = choose_band_SNR(host_df)
                             r_a = r_b = float(host_df[band + 'KronRad'].values[0])
                             dist, R = calc_DLR(ra_SN, dec_SN, ra_host, dec_host, r_a, r_b, host_df, band)
@@ -358,45 +361,44 @@
                     dict_mod[name] = chosenHost
                     hosts.loc[hosts['objID'] == chosenHost, 'dist/DLR'] = R_dict[chosenHost]
                     hosts.loc[hosts['objID'] == chosenHost, 'dist'] = dist_dict[chosenHost]
                     if (GDflag):
                         GDflag = 0
                         print("Issue with DLR. Try Gradient Descent!", file=f)
                         GA_SN.append(name)
-                    print(float(hosts[hosts['objID'] == chosenHost]['raMean']), float(hosts[hosts['objID'] == chosenHost]['decMean']), file=f)
+                    print(float(hosts[hosts['objID'] == chosenHost]['raMean'].values[0]), float(hosts[hosts['objID'] == chosenHost]['decMean'].values[0]), file=f)
                 f.flush()
     f.close()
     if todo == "s":
         with open('../dictionaries/DLR_rankOrdered_hosts.p', 'wb') as fp:
             pickle.dump(dict_mod, fp, protocol=pickle.HIGHEST_PROTOCOL)
         hosts.to_csv("../tables/DLR_rankOrdered_hosts.csv")
         return
     elif todo =="r":
         return hosts, dict_mod, noHosts, GA_SN
 
 #new method - beta!
 def chooseByGladeDLR(path, fn, snDF, todo='r'):
-    """TODO: Short summary.
+    """The wrapper function for selecting hosts by the DLR method (Gupta et al., 2013).
 
-    Parameters
-    ----------
-    path : type
-        Description of parameter `path`.
-    fn : type
-        Description of parameter `fn`.
-    snDF : type
-        Description of parameter `snDF`.
-    todo : type
-        Description of parameter `todo`.
-
-    Returns
-    -------
-    type
-        Description of returned object.
+    Here, candidate hosts are taken from the GLADE (Dalya et al., 2021; arXiv:2110.06184) catalog.
 
+    :param path: Filepath where to write out the results of the DLR algorithm.
+    :type path: str
+    :param fn: Filename to write the results of the associations (useful for debugging).
+    :type fn: str
+    :param transients: DataFrame containing TNS information for all transients.
+    :type transients: Pandas DataFrame
+    :param todo: If todo == \\'s\\', save the dictionary and the list of remaining sources.
+        If todo == \\'r\\', return them.
+    :type todo: str
+    :return: The dataframe of properties for GLADE host galaxies found by DLR.
+    :rtype: Pandas DataFrame
+    :return: List of transients for which no reliable GLADE host galaxy was found.
+    :rtype: array-like
     """
     if todo=="s":
         if not os.path.exists(path+'/dictionaries'):
              os.makedirs(path+'/dictionaries')
         if not os.path.exists(path+'/tables'):
              os.makedirs(path+'/tables')
```

### Comparing `astro_ghost-2.0.0/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-2.0.1/astro_ghost/NEDQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-2.0.1/astro_ghost/PS1QueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-2.0.1/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-2.0.1/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-2.0.1/astro_ghost/TNSQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/astro_ghost/conftest.py` & `astro_ghost-2.0.1/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-2.0.1/astro_ghost/ghostHelperFunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,27 +28,22 @@
 from joblib import dump, load
 import pandas as pd
 
 #we do a lot of copies, sub-selects and rewrites - no need to warn about everything!
 pd.options.mode.chained_assignment = None  # default='warn'
 
 def cleanup(path):
-    """TODO: Short summary.
+    """Cleans up the working directory.
 
-    Parameters
-    ----------
-    path : type
-        Description of parameter `path`.
-
-    Returns
-    -------
-    type
-        Description of returned object.
+    This is done after host-galaxy association is completed.
 
+    :param path: filepath where association files are saved
+    :type path: str
     """
+
     tablePath = path+"/tables/"
     printoutPath = path+'/printouts/'
 
     paths = [tablePath, printoutPath]
 
     for tempPath in paths:
         if not os.path.exists(tempPath):
@@ -174,18 +169,15 @@
             'Hubble Residual', 'TransientName']
         df = pd.DataFrame(columns = colnames)
         df.to_csv(installpath + "/database/GHOST.csv",index=False)
         if verbose:
             print("Successfully created dummy database.\n")
 
 def fracWithHosts(transient_dict):
-    """Calculates the fraction of supernovae
-       in our dictionary that have at least
-       one candidate host associated with
-       them.
+    """Calculates transient fraction with at least one candidate host.
 
     :param transient_dict: The dictionary of supernovae and their host galaxy candidate objIDs from PS1.
     :type transient_dict: dictionary
     :return: The fraction of supernovae with at least one candidate host galaxy.
     :rtype: dictionary
     """
 
@@ -197,30 +189,30 @@
                 count += 1
         else:
             if host == host:
                 count+=1
     return count/len(transient_dict.keys())
 
 def remove_prefix(text, prefix):
-    """Removes the prefix from a string. Very useful for removing the 'SN' from
-       supernova names!
+    """Removes the prefix from a string.
+
+    Very useful for removing the 'SN' from supernova names!
 
     :param text: The full text.
     :type text: str
     :param prefix: The prefix to remove from the text.
     :type prefix: str
     :return: The input text, with prefix removed.
     :rtype: str
     """
 
     return text[text.startswith(prefix) and len(prefix):]
 
 def getDBHostFromTransientCoords(transientCoords, GHOSTpath=''):
-    """Gets the host associated with a supernova in
-       the GHOST database by the supernova's position, if it exists.
+    """Gets the host of a GHOST transient by position.
 
     :param transientCoords: A list of astropy SkyCoord coordinates of transients.
     :type transientCoords: array-like
     :param GHOSTpath: The path to the saved GHOST database.
     :type GHOSTpath: str
 
     :return: The PS1 objects associated with the queried transients in GHOST.
@@ -250,16 +242,15 @@
         else:
             notFound.append(transientCoord)
     if len(hostList) > 0:
         host_DF = pd.concat(hostList, ignore_index=True)
     return host_DF, notFound
 
 def getDBHostFromTransientName(transientNames, GHOSTpath=''):
-    """Gets the host associated with a supernova in
-       the GHOST database by the supernova's name, if it exists.
+    """Gets the host of a GHOST transient by transient name.
 
     :param transientNames: A list of transient names.
     :type transientNames: array-like
     :param GHOSTpath: The path to the saved GHOST database.
     :type GHOSTpath: str
     :return: The PS1 objects associated with the queried transients in GHOST.
     :rtype: Pandas DataFrame
@@ -706,15 +697,15 @@
     os.makedirs(savepath + dir_name)
     path = savepath+dir_name+'/'
 
     #create temp dataframe with RA and DEC corresponding to the transient
     snDF = pd.DataFrame({'Name':transientName_arr, 'RA':snRA_arr, 'DEC':snDEC_arr, 'HostName':['']*len(snDEC_arr), 'Obj. Type':snClass_arr})
     snDF.to_csv(path+fn_transients, index=False)
 
-    #new method (beta) - before we do anything else, find and associate low-z hosts with GLADE
+    #new low-z method (beta) - before we do anything else, find and associate with GLADE
     fn_glade = "gladeDLR.txt"
     foundGladeHosts, noGladeHosts = chooseByGladeDLR(path, fn_glade, snDF, todo="r")
 
     #open transients df and drop the transients already found in GLADE. We'll add these back in at the end
     snDF = snDF[snDF['Name'].isin(noGladeHosts)]
     fn_transients_preGLADE = fn_transients
     fn_transients = 'transients_%s_postGlade.csv' % dateStr
```

### Comparing `astro_ghost-2.0.0/astro_ghost/gradientAscent.py` & `astro_ghost-2.0.1/astro_ghost/gradientAscent.py`

 * *Files 1% similar despite different names*

```diff
@@ -750,15 +750,15 @@
                         if len(tempA) > 0:
                             a = tempA
                         a = a.iloc[[0]]
                         print("S: Picking the closest non-stellar source within 5 arcsec", file=f)
                     print("Nice! Host association chosen.", file=f)
                     print("NED type: %s" % a['NED_type'].values[0], file=f)
                     print(a['objID'].values[0], file=f)
-                    print("Chosen Host RA and DEC: %f %f"% (a['raMean'], a['decMean']), file=f)
+                    print("Chosen Host RA and DEC: %f %f"% (a['raMean'].values[0], a['decMean'].values[0]), file=f)
                     SN_dict_postDLR[transient_name] = a['objID'].values[0]
                     print("Dict value: %i"%SN_dict_postDLR[transient_name],file=f)
                     N = len(hostDF)
                     hostDF = pd.concat([hostDF, a], ignore_index=True)
                     N2 = len(hostDF)
                     if N2 != (N+1):
                         print("ERROR! Value not concatenated!!", file=f)
```

### Comparing `astro_ghost-2.0.0/astro_ghost/hostMatching.py` & `astro_ghost-2.0.1/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/astro_ghost/photoz_helper.py` & `astro_ghost-2.0.1/astro_ghost/photoz_helper.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/astro_ghost/sourceCleaning.py` & `astro_ghost-2.0.1/astro_ghost/sourceCleaning.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/astro_ghost/starSeparation.py` & `astro_ghost-2.0.1/astro_ghost/starSeparation.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,17 +85,17 @@
 
     # plot the distribution of classified stars and galaxies.
     if plot:
         c_gals = '#087e8b'
         c_stars = '#ffbf00'
 
         plt.figure(num=None, figsize=(8, 6), dpi=80, facecolor='w', edgecolor='k')
-        sns.kdeplot(test_gals['iApMag'], test_gals['iApMag_iKronMag'], n_levels=20, shade_lowest=False, shade=False,label='Galaxies', color=c_gals, alpha=0.5,legend=True);
+        sns.kdeplot(test_gals['iApMag'], test_gals['iApMag_iKronMag'], n_levels=20, fill=False,label='Galaxies', color=c_gals, alpha=0.5,legend=True);
         if len(test_stars) > 1:
-            sns.kdeplot(test_stars['iApMag'], test_stars['iApMag_iKronMag'], n_levels=20, shade_lowest=False, shade=False,label='Stars', color=c_stars, alpha=0.5);
+            sns.kdeplot(test_stars['iApMag'], test_stars['iApMag_iKronMag'], n_levels=20, fill=False,label='Stars', color=c_stars, alpha=0.5);
         plt.legend()
         plt.xlim(xmin=13,xmax=23)
         plt.ylim(ymin=-1,ymax=5)
         plt.xlabel("Ap Magnitude, $i$",fontsize=16)
         plt.ylabel("Ap - Kron Magnitude, $i$",fontsize=16)
 
         plt.savefig("TNS_STRM_Stars_vs_Gals_Contours.pdf")
```

### Comparing `astro_ghost-2.0.0/astro_ghost/stellarLocus.py` & `astro_ghost-2.0.1/astro_ghost/stellarLocus.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,10 +105,10 @@
         else:
             c = 'violet'
         g = sns.JointGrid(x="i-z", y="g-r", data=df, height=9, ratio=5, xlim=(-0.4, 0.8), ylim=(-0.2, 2.0), space=0)
         g = g.plot_joint(sns.kdeplot, color=c,gridsize=200)
         g.ax_joint.plot(iz_new, gr_new, '--', c='#8c837c', lw=2)
         plt.xlabel(r"$i-z$",fontsize=18)
         plt.ylabel(r"$g-r$",fontsize=18)
-        g = g.plot_marginals(sns.kdeplot, color=c, shade=True)
+        g = g.plot_marginals(sns.kdeplot, color=c, fill=True)
         if save:
             g.savefig("PS1_%s_StellarLocus_%s.pdf"%(type, timestamp))
```

### Comparing `astro_ghost-2.0.0/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-2.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: astro-ghost
-Version: 2.0.0
+Name: astro_ghost
+Version: 2.0.1
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,14 +25,18 @@
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
 
 .. image:: https://img.shields.io/pypi/dm/astro-ghost
    :target: https://pypi.org/project/astro-ghost/
    :alt: PyPI
 
+.. image:: https://github.com/uiucsn/astro_ghost/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/uiucsn/astro_ghost/actions/workflows/tests.yml
+   :alt: Unit Tests
+
 .. image:: https://img.shields.io/readthedocs/uiucsnastro-ghost
    :target: https://uiucsnastro-ghost.readthedocs.io/en/latest/
    :alt: Read the Docs
 
 "At the last dim horizon, we search among ghostly errors of observations for
 landmarks that are scarcely more substantial. The search will continue. The
 urge is older than history. It is not satisfied and it will not be oppressed."
```

### Comparing `astro_ghost-2.0.0/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-2.0.1/astro_ghost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/docs/Makefile` & `astro_ghost-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/docs/conf.py` & `astro_ghost-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/docs/index.rst` & `astro_ghost-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/docs/make.bat` & `astro_ghost-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/docs/source/associationmodules.rst` & `astro_ghost-2.0.1/docs/source/associationmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/docs/source/basicusage.rst` & `astro_ghost-2.0.1/docs/source/basicusage.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/docs/source/catalogmodules.rst` & `astro_ghost-2.0.1/docs/source/catalogmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/docs/source/installation.rst` & `astro_ghost-2.0.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/docs/source/preprocessingmodules.rst` & `astro_ghost-2.0.1/docs/source/preprocessingmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/licenses/LICENSE.rst` & `astro_ghost-2.0.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/setup.cfg` & `astro_ghost-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/setup.py` & `astro_ghost-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "2.0.0"
+version = "2.0.1"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
```

### Comparing `astro_ghost-2.0.0/tests/debug.py` & `astro_ghost-2.0.1/tests/debug.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/tests/test_tutorial.py` & `astro_ghost-2.0.1/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.0/tox.ini` & `astro_ghost-2.0.1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 extras =
     test
     docs
     alldeps: all
 
 commands =
     pip freeze
-    pytest --pyargs astro_ghost {toxinidir}/docs --cov astro_ghost --cov-config={toxinidir}/setup.cfg {posargs}
+    pytest --cov=astro_ghost {toxinidir}/tests
+    #pytest --pyargs astro_ghost {toxinidir}/docs --cov astro_ghost --cov-config={toxinidir}/setup.cfg {posargs}
 
 [testenv:build_docs]
 changedir = docs
 description = invoke sphinx-build to build the HTML docs
 extras = docs
 commands =
     pip freeze
```

