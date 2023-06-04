# Comparing `tmp/PySupercell-0.0.7.tar.gz` & `tmp/PySupercell-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySupercell-0.0.7.tar", last modified: Sun Jun  4 07:26:53 2023, max compression
+gzip compressed data, was "PySupercell-0.0.8.tar", last modified: Sun Jun  4 08:44:37 2023, max compression
```

## Comparing `PySupercell-0.0.7.tar` & `PySupercell-0.0.8.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.255631 PySupercell-0.0.7/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1058 2023-06-03 15:54:33.000000 PySupercell-0.0.7/LICENSE.txt
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      294 2023-06-03 15:54:33.000000 PySupercell-0.0.7/MANIFEST.in
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      484 2023-06-04 07:26:53.255631 PySupercell-0.0.7/PKG-INFO
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.247631 PySupercell-0.0.7/PySupercell.egg-info/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      484 2023-06-04 07:26:53.000000 PySupercell-0.0.7/PySupercell.egg-info/PKG-INFO
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1228 2023-06-04 07:26:53.000000 PySupercell-0.0.7/PySupercell.egg-info/SOURCES.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-06-04 07:26:53.000000 PySupercell-0.0.7/PySupercell.egg-info/dependency_links.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       33 2023-06-04 07:26:53.000000 PySupercell-0.0.7/PySupercell.egg-info/requires.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       92 2023-06-04 07:26:53.000000 PySupercell-0.0.7/PySupercell.egg-info/top_level.txt
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2282 2023-06-03 15:54:33.000000 PySupercell-0.0.7/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.247631 PySupercell-0.0.7/bin/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    10217 2023-06-03 15:54:33.000000 PySupercell-0.0.7/bin/pysc.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    11607 2023-06-04 07:24:48.000000 PySupercell-0.0.7/bin/v2qe.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.247631 PySupercell-0.0.7/examples/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      266 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.251631 PySupercell-0.0.7/examples/example1/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      364 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example1/POSCAR
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      369 2023-06-04 07:23:49.000000 PySupercell-0.0.7/examples/example1/POSCAR_1
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      376 2023-06-04 07:24:52.000000 PySupercell-0.0.7/examples/example1/POSCAR_Primitive
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      735 2023-06-04 07:23:49.000000 PySupercell-0.0.7/examples/example1/POSCAR_std
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      691 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example1/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.251631 PySupercell-0.0.7/examples/example1/reference/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      704 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example1/reference/POSCAR_redefine
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1312 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example1/reference/POSCAR_slab
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      610 2023-06-04 07:24:52.000000 PySupercell-0.0.7/examples/example1/rx.in
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      761 2023-06-04 07:23:48.000000 PySupercell-0.0.7/examples/example1/test_phonopy.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.251631 PySupercell-0.0.7/examples/example2/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      437 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example2/POSCAR
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12072 2023-06-03 15:57:48.000000 PySupercell-0.0.7/examples/example2/POSCAR_sc
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12078 2023-06-03 15:57:48.000000 PySupercell-0.0.7/examples/example2/POSCAR_tube_4_6
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)       37 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example2/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.251631 PySupercell-0.0.7/examples/example2/reference/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9732 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example2/reference/POSCAR_sc
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9738 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example2/reference/POSCAR_tube
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.251631 PySupercell-0.0.7/examples/example3/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      948 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example3/POSCAR
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    54936 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example3/POSCAR_redefine
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      569 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example3/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9854 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example3/make_screw_diamond.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.255631 PySupercell-0.0.7/examples/example3/reference/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    44136 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example3/reference/POSCAR_redefine
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    54957 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example3/reference/POSCAR_screw
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.255631 PySupercell-0.0.7/examples/example4/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      534 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example4/POSCAR
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      124 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example4/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.255631 PySupercell-0.0.7/examples/example4/reference/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2176 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example4/reference/POSCAR_bending
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2168 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example4/reference/POSCAR_flat
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.255631 PySupercell-0.0.7/pysupercell/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     8665 2023-06-03 15:54:34.000000 PySupercell-0.0.7/pysupercell/QE_ibrav_lib.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      293 2023-06-04 07:26:32.000000 PySupercell-0.0.7/pysupercell/__init__.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4589 2023-06-04 07:02:36.000000 PySupercell-0.0.7/pysupercell/arguments.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    44518 2023-06-04 07:26:03.000000 PySupercell-0.0.7/pysupercell/pysupercell.py
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-06-04 07:26:53.255631 PySupercell-0.0.7/setup.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3621 2023-06-04 07:26:43.000000 PySupercell-0.0.7/setup.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.255631 PySupercell-0.0.7/tests_basic/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)       40 2023-06-03 15:54:34.000000 PySupercell-0.0.7/tests_basic/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)       72 2023-06-03 15:54:34.000000 PySupercell-0.0.7/tests_basic/test_1.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.866731 PySupercell-0.0.8/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1058 2023-06-03 15:54:33.000000 PySupercell-0.0.8/LICENSE.txt
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      204 2023-06-04 08:16:08.000000 PySupercell-0.0.8/MANIFEST.in
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      499 2023-06-04 08:44:37.866731 PySupercell-0.0.8/PKG-INFO
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.854731 PySupercell-0.0.8/PySupercell.egg-info/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      499 2023-06-04 08:44:37.000000 PySupercell-0.0.8/PySupercell.egg-info/PKG-INFO
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1344 2023-06-04 08:44:37.000000 PySupercell-0.0.8/PySupercell.egg-info/SOURCES.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-06-04 08:44:37.000000 PySupercell-0.0.8/PySupercell.egg-info/dependency_links.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       23 2023-06-04 08:44:37.000000 PySupercell-0.0.8/PySupercell.egg-info/requires.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       92 2023-06-04 08:44:37.000000 PySupercell-0.0.8/PySupercell.egg-info/top_level.txt
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2282 2023-06-03 15:54:33.000000 PySupercell-0.0.8/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.854731 PySupercell-0.0.8/bin/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    10217 2023-06-03 15:54:33.000000 PySupercell-0.0.8/bin/pysc
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    11607 2023-06-04 07:24:48.000000 PySupercell-0.0.8/bin/v2qe
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.854731 PySupercell-0.0.8/examples/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.858731 PySupercell-0.0.8/examples/example1/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      364 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example1/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      369 2023-06-04 07:23:49.000000 PySupercell-0.0.8/examples/example1/POSCAR_1
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      376 2023-06-04 08:41:34.000000 PySupercell-0.0.8/examples/example1/POSCAR_Primitive
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      824 2023-06-04 08:15:00.000000 PySupercell-0.0.8/examples/example1/POSCAR_redefine
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1582 2023-06-04 08:15:01.000000 PySupercell-0.0.8/examples/example1/POSCAR_slab_111
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      735 2023-06-04 07:23:49.000000 PySupercell-0.0.8/examples/example1/POSCAR_std
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      676 2023-06-04 08:39:59.000000 PySupercell-0.0.8/examples/example1/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.858731 PySupercell-0.0.8/examples/example1/reference/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      704 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example1/reference/POSCAR_redefine
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1312 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example1/reference/POSCAR_slab
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      610 2023-06-04 08:41:34.000000 PySupercell-0.0.8/examples/example1/rx.in
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      761 2023-06-04 07:23:48.000000 PySupercell-0.0.8/examples/example1/test_phonopy.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.858731 PySupercell-0.0.8/examples/example2/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      437 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example2/POSCAR
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12072 2023-06-04 08:15:04.000000 PySupercell-0.0.8/examples/example2/POSCAR_sc
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12078 2023-06-04 08:15:04.000000 PySupercell-0.0.8/examples/example2/POSCAR_tube_4_6
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)       34 2023-06-04 08:39:59.000000 PySupercell-0.0.8/examples/example2/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.862731 PySupercell-0.0.8/examples/example2/reference/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9732 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example2/reference/POSCAR_sc
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9738 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example2/reference/POSCAR_tube
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.862731 PySupercell-0.0.8/examples/example3/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      948 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example3/POSCAR
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    54936 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example3/POSCAR_redefine
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      596 2023-06-04 08:39:59.000000 PySupercell-0.0.8/examples/example3/README.md
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9854 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example3/make_screw_diamond.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.862731 PySupercell-0.0.8/examples/example3/reference/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    44136 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example3/reference/POSCAR_redefine
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    54957 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example3/reference/POSCAR_screw
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.862731 PySupercell-0.0.8/examples/example4/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      534 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example4/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     2656 2023-06-04 08:15:08.000000 PySupercell-0.0.8/examples/example4/POSCAR_bending
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     2648 2023-06-04 08:15:07.000000 PySupercell-0.0.8/examples/example4/POSCAR_flat
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      118 2023-06-04 08:39:59.000000 PySupercell-0.0.8/examples/example4/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.862731 PySupercell-0.0.8/examples/example4/reference/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2176 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example4/reference/POSCAR_bending
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2168 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example4/reference/POSCAR_flat
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1794 2023-06-04 08:39:31.000000 PySupercell-0.0.8/examples/run_all_examples.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.866731 PySupercell-0.0.8/pysupercell/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     8665 2023-06-03 15:54:34.000000 PySupercell-0.0.8/pysupercell/QE_ibrav_lib.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      293 2023-06-04 08:40:44.000000 PySupercell-0.0.8/pysupercell/__init__.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4589 2023-06-04 07:02:36.000000 PySupercell-0.0.8/pysupercell/arguments.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    44519 2023-06-04 08:43:58.000000 PySupercell-0.0.8/pysupercell/pysupercell.py
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-06-04 08:44:37.866731 PySupercell-0.0.8/setup.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3782 2023-06-04 08:44:33.000000 PySupercell-0.0.8/setup.py
```

### Comparing `PySupercell-0.0.7/LICENSE.txt` & `PySupercell-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/PySupercell.egg-info/SOURCES.txt` & `PySupercell-0.0.8/PySupercell.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,41 +3,44 @@
 README.md
 setup.py
 PySupercell.egg-info/PKG-INFO
 PySupercell.egg-info/SOURCES.txt
 PySupercell.egg-info/dependency_links.txt
 PySupercell.egg-info/requires.txt
 PySupercell.egg-info/top_level.txt
-bin/pysc.py
-bin/v2qe.py
+bin/pysc
+bin/v2qe
 examples/README.md
+examples/run_all_examples.py
 examples/example1/POSCAR
 examples/example1/POSCAR_1
 examples/example1/POSCAR_Primitive
+examples/example1/POSCAR_redefine
+examples/example1/POSCAR_slab_111
 examples/example1/POSCAR_std
 examples/example1/README.md
 examples/example1/rx.in
 examples/example1/test_phonopy.py
 examples/example1/reference/POSCAR_redefine
 examples/example1/reference/POSCAR_slab
 examples/example2/POSCAR
 examples/example2/POSCAR_sc
 examples/example2/POSCAR_tube_4_6
 examples/example2/README.md
 examples/example2/reference/POSCAR_sc
 examples/example2/reference/POSCAR_tube
 examples/example3/POSCAR
 examples/example3/POSCAR_redefine
-examples/example3/README
+examples/example3/README.md
 examples/example3/make_screw_diamond.py
 examples/example3/reference/POSCAR_redefine
 examples/example3/reference/POSCAR_screw
 examples/example4/POSCAR
+examples/example4/POSCAR_bending
+examples/example4/POSCAR_flat
 examples/example4/README.md
 examples/example4/reference/POSCAR_bending
 examples/example4/reference/POSCAR_flat
 pysupercell/QE_ibrav_lib.py
 pysupercell/__init__.py
 pysupercell/arguments.py
-pysupercell/pysupercell.py
-tests_basic/README
-tests_basic/test_1.py
+pysupercell/pysupercell.py
```

### Comparing `PySupercell-0.0.7/README.md` & `PySupercell-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/bin/pysc.py` & `PySupercell-0.0.8/bin/pysc`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/bin/v2qe.py` & `PySupercell-0.0.8/bin/v2qe`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example1/POSCAR_std` & `PySupercell-0.0.8/examples/example1/POSCAR_std`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example1/README.md` & `PySupercell-0.0.8/examples/example1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 This example show how to create a supercell of diamond-Si
 and create a slab based on it
 
 The primitive cell structure is used, stored in POSCAR
 
 * To create a convention cell, use the command
 
-    pysc.py --task=redefine --sc1=-1,1,1 --sc2=1,-1,1 --sc3=1,1,-1
+    pysc --task=redefine --sc1=-1,1,1 --sc2=1,-1,1 --sc3=1,1,-1
 
     You can check the generated POSCAR_redefine file 
 
 * To create a slab structure, run
 
-    pysc.py --task=slab --hkl=111 --thickness=3 --vacuum=20
+    pysc --task=slab --hkl=111 --thickness=3 --vacuum=20
 
 * To query the bond length between two atoms
 
-    pysc.py --task=bond --atom_index=0,1 --poscar=POSCAR_slab
+    pysc --task=bond --atom_index=0,1 --poscar=POSCAR_slab
 
-    pysc.py --task=latt_info --poscar=POSCAR_slab
+    pysc --task=latt_info --poscar=POSCAR_slab
 
 
 * To write structure information for QE pw.x (under testing)
     
-    v2qe.py
+    v2qe
```

### Comparing `PySupercell-0.0.7/examples/example1/reference/POSCAR_redefine` & `PySupercell-0.0.8/examples/example1/reference/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example1/reference/POSCAR_slab` & `PySupercell-0.0.8/examples/example1/reference/POSCAR_slab`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example1/rx.in` & `PySupercell-0.0.8/examples/example1/rx.in`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example1/test_phonopy.py` & `PySupercell-0.0.8/examples/example1/test_phonopy.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example2/POSCAR_sc` & `PySupercell-0.0.8/examples/example2/POSCAR_sc`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example2/POSCAR_tube_4_6` & `PySupercell-0.0.8/examples/example2/POSCAR_tube_4_6`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example2/reference/POSCAR_sc` & `PySupercell-0.0.8/examples/example2/reference/POSCAR_sc`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example2/reference/POSCAR_tube` & `PySupercell-0.0.8/examples/example2/reference/POSCAR_tube`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example3/POSCAR` & `PySupercell-0.0.8/examples/example3/POSCAR`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example3/POSCAR_redefine` & `PySupercell-0.0.8/examples/example3/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example3/make_screw_diamond.py` & `PySupercell-0.0.8/examples/example3/make_screw_diamond.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example3/reference/POSCAR_redefine` & `PySupercell-0.0.8/examples/example3/reference/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example3/reference/POSCAR_screw` & `PySupercell-0.0.8/examples/example3/reference/POSCAR_screw`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example4/POSCAR` & `PySupercell-0.0.8/examples/example4/POSCAR`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example4/reference/POSCAR_bending` & `PySupercell-0.0.8/examples/example4/reference/POSCAR_bending`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/examples/example4/reference/POSCAR_flat` & `PySupercell-0.0.8/examples/example4/reference/POSCAR_flat`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/pysupercell/QE_ibrav_lib.py` & `PySupercell-0.0.8/pysupercell/QE_ibrav_lib.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/pysupercell/arguments.py` & `PySupercell-0.0.8/pysupercell/arguments.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.7/pysupercell/pysupercell.py` & `PySupercell-0.0.8/pysupercell/pysupercell.py`

 * *Files 0% similar despite different names*

```diff
@@ -704,15 +704,15 @@
 
 
     def molar_mass(self):
         def gcd(a,b): return gcd(b, a % b) if b else a
         nfu=self._counts[0]
         for ispec in range(1,len(self._species)):
             nfu=gcd(self._counts[ispec],nfu)
-        print ('no. of formula in unit cell: {0}'.format(nfu))
+        print ('No. of formula units in cell: {0}'.format(nfu))
         try:
             amass=[get_element_info_phonopy(sym)[-1] for sym in self._species]
             molar_mass=sum(self._counts/nfu*amass)
         except:
             exit('cannot calculate molar mass from phonopy')
         return molar_mass
```

### Comparing `PySupercell-0.0.7/setup.py` & `PySupercell-0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/env python
 
 
 #===========================================================================#
 #                                                                           #
 #  File:       setup.py                                                     #
-#  Dependence: the whole tool-kit                                           #
 #  Usage:      install the files as a lib and generate excutables           #      
 #  Author:     Shunhong Zhang <szhang2@ustc.edu.cn>                         #
-#  Date:       Nov 22, 2019                                                 #
+#  Date:       Jun 04, 2023                                                 #
 #                                                                           #
 #===========================================================================#
 
 
-from __future__ import print_function
+import glob
 import os
 import sys
 import platform
 from distutils.core import setup
 #from setuptools import setup
 
 
@@ -30,14 +29,17 @@
             if bin_dir not in current_path:  
                 print ('It has been added to ~/.bashrc')
                 print ('Run "source ~/.bashrc" to activate it')
                 add_binpath = 'echo "{0}"|cat >>~/.bashrc'.format(binpath)
                 os.system(add_binpath)
             else:  
                 print ('The utility directory already in the path\n')
+        else:
+            print ('You are using {} operating system'.format(sys.plotform))
+            print ('Please set the environment variable manually')
 
 
 
 def test_modules(module_list,desc,pkg='asd'):
     import importlib
     import glob
     import shutil
@@ -62,31 +64,40 @@
 'QE_ibrav_lib',
 'arguments',
 'pysupercell',
 '__init__',
 ]
 
 core_modules = ['pysupercell/{}'.format(item) for item in core_modules]
+scripts_pysupercell = ['bin/pysc','bin/v2qe']
 
+long_desc="A Open-source Python library for playing with crystal structures, such as supercell, dislocation, slab, and nanotube"
 
 
 kwargs_setup=dict(
 name='PySupercell',
-version='0.0.7',
+version='0.0.8',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
 url='https://to_be_posted',
 download_url='https://on_request',
 keywords=['Python','Crystal structure','supercell'],
 py_modules=core_modules,
 license="MIT License",
 description='Python library for creating and manipulating crystal structures',
-long_description="A Open-source Python library for playing with crystal structures, such as supercell, dislocation, slab, and nanotube",
+long_description=long_desc,
 platforms=[platform.system()],
-install_requires=['numpy','matplotlib','scipy','termcolor'],
+install_requires=[
+'numpy',
+'matplotlib',
+'scipy'
+],
+provides=["pysc"],
+scripts=scripts_pysupercell,
+
 )
 
 
 if __name__=='__main__':
     print ('{0}\nOperating System: {1}'.format('-'*50,platform.system()))
 
     print ('\n{0}\nINSTALL\n{0}\n'.format('-'*50))
```

