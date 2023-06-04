# Comparing `tmp/PySupercell-0.0.6.tar.gz` & `tmp/PySupercell-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySupercell-0.0.6.tar", last modified: Sat Jun  3 15:56:45 2023, max compression
+gzip compressed data, was "PySupercell-0.0.7.tar", last modified: Sun Jun  4 07:26:53 2023, max compression
```

## Comparing `PySupercell-0.0.6.tar` & `PySupercell-0.0.7.tar`

### file list

```diff
@@ -1,60 +1,59 @@
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1058 2023-06-03 15:54:33.000000 PySupercell-0.0.6/LICENSE.txt
--rwxr-xr-x   0 shz       (1000) shz       (1000)      294 2023-06-03 15:54:33.000000 PySupercell-0.0.6/MANIFEST.in
--rw-r--r--   0 shz       (1000) shz       (1000)      484 2023-06-03 15:56:45.226954 PySupercell-0.0.6/PKG-INFO
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/PySupercell.egg-info/
--rw-r--r--   0 shz       (1000) shz       (1000)      484 2023-06-03 15:56:45.000000 PySupercell-0.0.6/PySupercell.egg-info/PKG-INFO
--rw-r--r--   0 shz       (1000) shz       (1000)     1297 2023-06-03 15:56:45.000000 PySupercell-0.0.6/PySupercell.egg-info/SOURCES.txt
--rw-r--r--   0 shz       (1000) shz       (1000)        1 2023-06-03 15:56:45.000000 PySupercell-0.0.6/PySupercell.egg-info/dependency_links.txt
--rw-r--r--   0 shz       (1000) shz       (1000)       33 2023-06-03 15:56:45.000000 PySupercell-0.0.6/PySupercell.egg-info/requires.txt
--rw-r--r--   0 shz       (1000) shz       (1000)       92 2023-06-03 15:56:45.000000 PySupercell-0.0.6/PySupercell.egg-info/top_level.txt
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2282 2023-06-03 15:54:33.000000 PySupercell-0.0.6/README.md
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/bin/
--rwxr-xr-x   0 shz       (1000) shz       (1000)    10217 2023-06-03 15:54:33.000000 PySupercell-0.0.6/bin/pysc.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    10425 2023-06-03 15:54:33.000000 PySupercell-0.0.6/bin/v2qe.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/
--rwxr-xr-x   0 shz       (1000) shz       (1000)      266 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/README.md
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example1/
--rwxr-xr-x   0 shz       (1000) shz       (1000)      364 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/POSCAR
--rwxr-xr-x   0 shz       (1000) shz       (1000)      376 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/POSCAR_Primitive
--rwxr-xr-x   0 shz       (1000) shz       (1000)      378 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/POSCAR_for_symm_analysis
--rwxr-xr-x   0 shz       (1000) shz       (1000)      691 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/README.md
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1739 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/phonopy_symcells.yaml
--rwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/phonopy_symm.yaml
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example1/reference/
--rwxr-xr-x   0 shz       (1000) shz       (1000)      704 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/reference/POSCAR_redefine
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1312 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/reference/POSCAR_slab
--rwxr-xr-x   0 shz       (1000) shz       (1000)      456 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/rx.in
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example2/
--rwxr-xr-x   0 shz       (1000) shz       (1000)       20 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/53s}'.format('version
--rwxr-xr-x   0 shz       (1000) shz       (1000)      437 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/POSCAR
--rwxr-xr-x   0 shz       (1000) shz       (1000)    12072 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/POSCAR_sc
--rwxr-xr-x   0 shz       (1000) shz       (1000)    12078 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/POSCAR_tube_4_6
--rwxr-xr-x   0 shz       (1000) shz       (1000)       37 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/README.md
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example2/reference/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     9732 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/reference/POSCAR_sc
--rwxr-xr-x   0 shz       (1000) shz       (1000)     9738 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/reference/POSCAR_tube
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example3/
--rwxr-xr-x   0 shz       (1000) shz       (1000)      948 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example3/POSCAR
--rwxr-xr-x   0 shz       (1000) shz       (1000)    54936 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example3/POSCAR_redefine
--rwxr-xr-x   0 shz       (1000) shz       (1000)      569 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example3/README
--rwxr-xr-x   0 shz       (1000) shz       (1000)     9854 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example3/make_screw_diamond.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example3/reference/
--rwxr-xr-x   0 shz       (1000) shz       (1000)    44136 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example3/reference/POSCAR_redefine
--rwxr-xr-x   0 shz       (1000) shz       (1000)    54957 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example3/reference/POSCAR_screw
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example4/
--rwxr-xr-x   0 shz       (1000) shz       (1000)      534 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example4/POSCAR
--rwxr-xr-x   0 shz       (1000) shz       (1000)      124 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example4/README.md
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example4/reference/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2176 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example4/reference/POSCAR_bending
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2168 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example4/reference/POSCAR_flat
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/pysupercell/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     8665 2023-06-03 15:54:34.000000 PySupercell-0.0.6/pysupercell/QE_ibrav_lib.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)      293 2023-06-03 15:55:22.000000 PySupercell-0.0.6/pysupercell/__init__.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     4589 2023-06-03 15:54:34.000000 PySupercell-0.0.6/pysupercell/arguments.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    44613 2023-06-03 15:54:34.000000 PySupercell-0.0.6/pysupercell/pysupercell.py
--rw-r--r--   0 shz       (1000) shz       (1000)       38 2023-06-03 15:56:45.226954 PySupercell-0.0.6/setup.cfg
--rwxr-xr-x   0 shz       (1000) shz       (1000)     3621 2023-06-03 15:56:37.000000 PySupercell-0.0.6/setup.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/tests_basic/
--rwxr-xr-x   0 shz       (1000) shz       (1000)       40 2023-06-03 15:54:34.000000 PySupercell-0.0.6/tests_basic/README
--rwxr-xr-x   0 shz       (1000) shz       (1000)       72 2023-06-03 15:54:34.000000 PySupercell-0.0.6/tests_basic/test_1.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.255631 PySupercell-0.0.7/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1058 2023-06-03 15:54:33.000000 PySupercell-0.0.7/LICENSE.txt
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      294 2023-06-03 15:54:33.000000 PySupercell-0.0.7/MANIFEST.in
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      484 2023-06-04 07:26:53.255631 PySupercell-0.0.7/PKG-INFO
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.247631 PySupercell-0.0.7/PySupercell.egg-info/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      484 2023-06-04 07:26:53.000000 PySupercell-0.0.7/PySupercell.egg-info/PKG-INFO
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1228 2023-06-04 07:26:53.000000 PySupercell-0.0.7/PySupercell.egg-info/SOURCES.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-06-04 07:26:53.000000 PySupercell-0.0.7/PySupercell.egg-info/dependency_links.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       33 2023-06-04 07:26:53.000000 PySupercell-0.0.7/PySupercell.egg-info/requires.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       92 2023-06-04 07:26:53.000000 PySupercell-0.0.7/PySupercell.egg-info/top_level.txt
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2282 2023-06-03 15:54:33.000000 PySupercell-0.0.7/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.247631 PySupercell-0.0.7/bin/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    10217 2023-06-03 15:54:33.000000 PySupercell-0.0.7/bin/pysc.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    11607 2023-06-04 07:24:48.000000 PySupercell-0.0.7/bin/v2qe.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.247631 PySupercell-0.0.7/examples/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      266 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.251631 PySupercell-0.0.7/examples/example1/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      364 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example1/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      369 2023-06-04 07:23:49.000000 PySupercell-0.0.7/examples/example1/POSCAR_1
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      376 2023-06-04 07:24:52.000000 PySupercell-0.0.7/examples/example1/POSCAR_Primitive
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      735 2023-06-04 07:23:49.000000 PySupercell-0.0.7/examples/example1/POSCAR_std
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      691 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example1/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.251631 PySupercell-0.0.7/examples/example1/reference/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      704 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example1/reference/POSCAR_redefine
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1312 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example1/reference/POSCAR_slab
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      610 2023-06-04 07:24:52.000000 PySupercell-0.0.7/examples/example1/rx.in
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      761 2023-06-04 07:23:48.000000 PySupercell-0.0.7/examples/example1/test_phonopy.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.251631 PySupercell-0.0.7/examples/example2/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      437 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example2/POSCAR
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12072 2023-06-03 15:57:48.000000 PySupercell-0.0.7/examples/example2/POSCAR_sc
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12078 2023-06-03 15:57:48.000000 PySupercell-0.0.7/examples/example2/POSCAR_tube_4_6
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)       37 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example2/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.251631 PySupercell-0.0.7/examples/example2/reference/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9732 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example2/reference/POSCAR_sc
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9738 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example2/reference/POSCAR_tube
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.251631 PySupercell-0.0.7/examples/example3/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      948 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example3/POSCAR
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    54936 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example3/POSCAR_redefine
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      569 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example3/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9854 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example3/make_screw_diamond.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.255631 PySupercell-0.0.7/examples/example3/reference/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    44136 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example3/reference/POSCAR_redefine
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    54957 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example3/reference/POSCAR_screw
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.255631 PySupercell-0.0.7/examples/example4/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      534 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example4/POSCAR
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      124 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example4/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.255631 PySupercell-0.0.7/examples/example4/reference/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2176 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example4/reference/POSCAR_bending
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2168 2023-06-03 15:54:34.000000 PySupercell-0.0.7/examples/example4/reference/POSCAR_flat
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.255631 PySupercell-0.0.7/pysupercell/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     8665 2023-06-03 15:54:34.000000 PySupercell-0.0.7/pysupercell/QE_ibrav_lib.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      293 2023-06-04 07:26:32.000000 PySupercell-0.0.7/pysupercell/__init__.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4589 2023-06-04 07:02:36.000000 PySupercell-0.0.7/pysupercell/arguments.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    44518 2023-06-04 07:26:03.000000 PySupercell-0.0.7/pysupercell/pysupercell.py
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-06-04 07:26:53.255631 PySupercell-0.0.7/setup.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3621 2023-06-04 07:26:43.000000 PySupercell-0.0.7/setup.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 07:26:53.255631 PySupercell-0.0.7/tests_basic/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)       40 2023-06-03 15:54:34.000000 PySupercell-0.0.7/tests_basic/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)       72 2023-06-03 15:54:34.000000 PySupercell-0.0.7/tests_basic/test_1.py
```

### Comparing `PySupercell-0.0.6/LICENSE.txt` & `PySupercell-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/PySupercell.egg-info/SOURCES.txt` & `PySupercell-0.0.7/PySupercell.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 PySupercell.egg-info/dependency_links.txt
 PySupercell.egg-info/requires.txt
 PySupercell.egg-info/top_level.txt
 bin/pysc.py
 bin/v2qe.py
 examples/README.md
 examples/example1/POSCAR
+examples/example1/POSCAR_1
 examples/example1/POSCAR_Primitive
-examples/example1/POSCAR_for_symm_analysis
+examples/example1/POSCAR_std
 examples/example1/README.md
-examples/example1/phonopy_symcells.yaml
-examples/example1/phonopy_symm.yaml
 examples/example1/rx.in
+examples/example1/test_phonopy.py
 examples/example1/reference/POSCAR_redefine
 examples/example1/reference/POSCAR_slab
-examples/example2/53s}'.format('version
 examples/example2/POSCAR
 examples/example2/POSCAR_sc
 examples/example2/POSCAR_tube_4_6
 examples/example2/README.md
 examples/example2/reference/POSCAR_sc
 examples/example2/reference/POSCAR_tube
 examples/example3/POSCAR
```

### Comparing `PySupercell-0.0.6/README.md` & `PySupercell-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/bin/pysc.py` & `PySupercell-0.0.7/bin/pysc.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/bin/v2qe.py` & `PySupercell-0.0.7/bin/v2qe.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,29 +42,54 @@
     so the magnetic unit cell may differs from the chemical primitive cell.
 3.  Body/Face/Base-centered structures: 
     The choice of the base plane is alternative, 
     please check the generated structure carefully using xcrysden.
 '''
 
 conv_cell_prompt='''
-this is a structure with face/body/base-centered symmetry
+This is a structure with face/body/base-centered symmetry
 The POSCAR you provide is a primitive cell
-use phonopy to generate BPOSCAR which is a conventional cell
+Use phonopy to generate a conventional cell (BPOSCAR)
 and then try again
-good luck!
+Good luck!
 '''
 
+
+def generate_standard_poscar_by_phonopy(poscar,symprec=5e-5):
+    from phonopy.interface.vasp import read_vasp,write_vasp
+    from phonopy.structure.grid_points import get_symmetry_dataset
+    from phonopy.structure import atoms
+    struct = read_vasp(poscar)
+    dataset = get_symmetry_dataset(struct,symprec=symprec)
+    struct_std = struct.copy()
+
+    symbols = [atoms.atom_data[n][1] for n in dataset['std_types']]
+
+    struct_std._set_parameters(
+    cell=dataset['std_lattice'],
+    symbols=symbols,
+    numbers=dataset['std_types'],
+    scaled_positions=dataset['std_positions'])
+
+    write_vasp('POSCAR_standardized',struct_std,direct=True)
+
+
 def standardize_poscar(ibrav,spg,poscar='POSCAR'):
     struct = cryst_struct.load_poscar(poscar)
     sc=np.eye(3)
     if abs(ibrav)==9 and spg.split()[0]=="A": 
         sc=sc[[1,2,0]]
     elif ibrav in [2,3,11,13]:
         latt_param = struct.latt_param()
         if latt_param['alpha']!=90 or latt_param['beta']!=90 or latt_param['gamma']!=90:
+            from phonopy.interface.vasp import read_vasp,write_vasp
+            from phonopy.structure.grid_points import get_symmetry_dataset
+            struct = read_vasp(poscar)
+            dateset = get_symmetry_dataset(struct,symprec=1e-4)
+            
             if os.path.isfile('BPOSCAR'): 
                 struct = cryst_struct.load_poscar('BPOSCAR')
                 print ('use BPOSCAR generated from phonopy')
             else:
                 exit (conv_cell_prompt)
         if ibrav == 13:
             print ('note: the unit cell is reoriented so that')
@@ -166,14 +191,15 @@
     parser.add_argument('--calculation',type=str,default="'vc-relax'",help="calculation task of QE")
     parser.add_argument('--outdir',type=str,default="'./tmp'",help="directory for temporary files")
     parser.add_argument('--prefix', type=str, default="pw", help='prefix for the pw calculation')
     parser.add_argument('--pseudo_dir',type=str,default="'/home/zsh/pseudo/pbe'",help="directory for pseudopotential files")
     parser.add_argument('--upf',    type=str, default=".pbe-mt_fhi.UPF",help="type of pseudopotentail")
     parser.add_argument('--kmesh', type=str, default='auto', help='k point mesh using the Monkhorst Pack scheme')
     parser.add_argument('--kshift', type=str, default="0 0 0", help='k point mesh shift from the Gamma point')
+    parser.add_argument('--filpw',type=str,default='rx.in',help='QE pw.x input file with structures')
     args=   parser.parse_args()
     return parser, args
 
 
 def main():
     print ('\nrunning the script {0}\n'.format(__file__.lstrip('./')))
     try:
@@ -211,33 +237,39 @@
     if ldef=="y": ibrav=input(colored("ibrav = ","red"))
     ibrav=int(ibrav)
 
     connect=get_connect(ibrav,spg,struct.latt_param())
     print ( "connect matrix\n")
     print ((('{:7.4f} '*3+'\n')*3+'\n').format(*tuple(connect.flatten())))
 
-    standardize_poscar(ibrav,spg,poscar=args.poscar)
+    #standardize_poscar(ibrav,spg,poscar=args.poscar)
+    generate_standard_poscar_by_phonopy(poscar=args.poscar,symprec=args.symmprec)
+
     struct_std = cryst_struct.load_poscar('POSCAR_standardized')
     if ldef=='y':struct_std=struct
     celldm=struct_std.find_celldm(ibrav=ibrav)
     print ("Lattice Parameters of standardized POSCAR:")
     struct_std.print_latt_param()
     
     struct_pm = struct_std.build_supercell(connect)
     struct_pm._system='primitive cell'
     struct_pm.write_poscar_head(filename="POSCAR_Primitive")
     struct_pm.write_poscar_atoms(filename="POSCAR_Primitive",mode='a')
 
     print ("\n{0}\nSample input for PWscf(Quantum ESPRESSO),Start\n{0}\n".format('-'*60))
     write_pwi(pw_setup_dic,ibrav,struct_std,struct_pm,filename=None)
-    write_pwi(pw_setup_dic,ibrav,struct_std,struct_pm,filename="rx.in")
+    struct_pm.write_pw_atoms(filename=None)
+ 
+    write_pwi(pw_setup_dic,ibrav,struct_std,struct_pm,filename=args.filpw)
+    with open(args.filpw,'a') as fw:
+        struct_pm.write_pw_atoms(filename=fw)
     print ("\n{0}\nSample input for PWscf(Quantum ESPRESSO),End\n{0}\n".format('-'*60))
     #struct._visualize_struct()
 
-    for file in ['BPOSCAR','PPOSCAR','phonopy_symm.yaml','POSCAR_standardized','POSCAR_for_symm_analysis']:
+    for file in ['POSCAR_standardized','POSCAR_for_symm_analysis']:
         if os.path.isfile(file): os.remove(file)
 
 
 
 desc_str = 'Convert POSCAR into QE pwscf input'
 
 if __name__=='__main__':
```

### Comparing `PySupercell-0.0.6/examples/example1/README.md` & `PySupercell-0.0.7/examples/example1/README.md`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example1/reference/POSCAR_redefine` & `PySupercell-0.0.7/examples/example1/reference/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example1/reference/POSCAR_slab` & `PySupercell-0.0.7/examples/example1/reference/POSCAR_slab`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example2/POSCAR_sc` & `PySupercell-0.0.7/examples/example2/POSCAR_sc`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example2/POSCAR_tube_4_6` & `PySupercell-0.0.7/examples/example2/POSCAR_tube_4_6`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example2/reference/POSCAR_sc` & `PySupercell-0.0.7/examples/example2/reference/POSCAR_sc`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example2/reference/POSCAR_tube` & `PySupercell-0.0.7/examples/example2/reference/POSCAR_tube`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example3/POSCAR` & `PySupercell-0.0.7/examples/example3/POSCAR`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example3/POSCAR_redefine` & `PySupercell-0.0.7/examples/example3/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example3/README` & `PySupercell-0.0.7/examples/example3/README`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example3/make_screw_diamond.py` & `PySupercell-0.0.7/examples/example3/make_screw_diamond.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example3/reference/POSCAR_redefine` & `PySupercell-0.0.7/examples/example3/reference/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example3/reference/POSCAR_screw` & `PySupercell-0.0.7/examples/example3/reference/POSCAR_screw`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example4/POSCAR` & `PySupercell-0.0.7/examples/example4/POSCAR`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example4/reference/POSCAR_bending` & `PySupercell-0.0.7/examples/example4/reference/POSCAR_bending`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/examples/example4/reference/POSCAR_flat` & `PySupercell-0.0.7/examples/example4/reference/POSCAR_flat`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/pysupercell/QE_ibrav_lib.py` & `PySupercell-0.0.7/pysupercell/QE_ibrav_lib.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/pysupercell/arguments.py` & `PySupercell-0.0.7/pysupercell/arguments.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.6/pysupercell/pysupercell.py` & `PySupercell-0.0.7/pysupercell/pysupercell.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,28 +131,24 @@
     counts=np.array([cc[ispec] for ispec in species])
     pos=np.array([np.array(item.split()[1:],float) for item in get_pos])
     cell=make_cell_qe(ibrav,celldm)
     return cell,species,counts,pos
 
 
 
-
+# Note: This function has a strong dependence on phonopy version
+# If it reports some errors, most likely your need ot modify it
+# according to the version of phonopy used in your platform
 def get_symm_from_phonopy(symmprec=1e-4,poscar='POSCAR'):
-    try:    import yaml
-    except: ImportError("You need to install python-yaml")
-    try:
-        from yaml import CLoader as Loader
-        from yaml import CDumper as Dumper
-    except ImportError:
-        from yaml import Loader, Dumper
-    phonopy_cmd = os.popen('which phonopy').read().rstrip('\n')
-    phonopy_cmd+=' --symmetry --tolerance={} -c {}> phonopy_symm.yaml'.format(symmprec,poscar)
-    os.system(phonopy_cmd)
-    data=yaml.load(open('phonopy_symm.yaml'),Loader=Loader)
-    return data
+    from phonopy.interface.vasp import read_vasp
+    try: from phonopy.structure.grid_points import get_symmetry_dataset
+    except: from phonopy.structure.cells import get_symmetry_dataset
+    struct = read_vasp(poscar)
+    dataset = get_symmetry_dataset(struct,symprec=symmprec)
+    return dataset
 
 
 def print_latt_param(latt):
     print ('\n{0}\nLattice Parameters\n{0}\n'.format('-'*40))
     keys=['a','b','c','alpha','beta','gamma']
     units=['Angs']*3+['deg']*3
     fmt='{0:8s}  {1:10.5f}  {2:8s}'
@@ -474,27 +470,26 @@
         spg = None
         spg_no = 0
         try:
             filposcar = 'POSCAR_for_symm_analysis'
             self.write_poscar_head(filposcar)
             self.write_poscar_atoms(filposcar,mode='a')
             symm_data=get_symm_from_phonopy(symmprec=symmprec,poscar=filposcar)
-            spg,spg_no = symm_data['space_group_type'],symm_data['space_group_number']
+            spg_no = symm_data['number']
+            spg = symm_data['hall']
         except:
-            if os.popen('which findsym').read() and os.popen('which pos2find').read():
-                get_sym=os.popen('pos2find {}|grep "Space Group"'.format(np.log(symprec))).readline().split()
-                spg_no = int(get_sym[2])
-                spg=get_sym[4]
+            raise Exception('Fail to extract symmetry information via phonopy.\nPlease check the phonopy version compatibility.')
+
         if spg is not None and spg_no>0:
             if report:
                 print ("space group:    {0}".format(spg))
                 print ("space group No: {0}".format(spg_no))
             return spg,spg_no
         else:
-            raise Exception('we need phonopy or ISOTROPY to help find symmetry currently, please install either of them')
+            raise Exception('we need phonopy to help find symmetry currently, please install it via pip install phonopy')
 
 
     def get_ibrav(self,symmprec=1e-4,report=False):
         spg,spg_no=self.find_symmetry(symmprec=symmprec)
         brav   = brav_dic[spg_no]
         center = center_dic[spg[0]]
         ibrav=ibrav_dic[brav,center]
@@ -591,15 +586,15 @@
             else:
                 print('\n'.join([('{:25.18f}'*3).format(*tuple(pos)) for pos in print_pos]),file=fpos)
 
 
     def write_pw_cell(self,filename=None):
         ibrav,brav,center=self.get_ibrav()
         celldm=self.find_celldm(ibrav)
-        print ("ibrav=",ibrav, file=filename)
+        print ("ibrav={}".format(ibrav), file=filename)
         for i in range(1,7):
             if celldm[i]: print ('celldm({:1d}) = {:20.12f}'.format(i,celldm[i]), file=filename)
         print ("nat = {0:3d}".format(self._natom), file=filename)
         print ("ntyp = {0:2d}".format(len(self._species)), file=filename)
 
 
     def write_pw_atoms(self,ctype='crystal',filename=None):
@@ -739,17 +734,18 @@
         if verbosity:
             print ('Supercell scale = {:10.5f}'.format(sc_scale))
             if sc_scale==0:  warnings.warn('The supercell size is zero!','red')
             elif sc_scale<0: warnings.warn("The supercell basis vectors are not right-handed!")
 
         sc_scale=abs(sc_scale)
         sc_counts=int(round(sc_scale))*self._counts
+        primitive_cell_warning = '\nThe supercell size is smaller than the unit cell.\nAre you constructing primitive cell?'
         for nn in range(2,5):
             if (sc_scale*nn-1.<eps): 
-                warnings.warn('The supercell size is smaller than the unit cell. Are you constructing primitive cell?')
+                warnings.warn(primitive_cell_warning)
                 sc_counts=np.array(list(map(int,self._counts/nn)))
                 sc_symbols=np.concatenate([[item]*cc for item,cc in zip(self._species,sc_counts)])
         sc_cell=np.dot(sc,self._cell)
         sc_pos=np.zeros((0,3),float)
         nimage_atom=np.zeros(self._natom,int)
 
         rb1 = int(round(abs(sc[0,0])+abs(sc[1,0])+abs(sc[2,0])))+nr
```

### Comparing `PySupercell-0.0.6/setup.py` & `PySupercell-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 core_modules = ['pysupercell/{}'.format(item) for item in core_modules]
 
 
 
 kwargs_setup=dict(
 name='PySupercell',
-version='0.0.6',
+version='0.0.7',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
 url='https://to_be_posted',
 download_url='https://on_request',
 keywords=['Python','Crystal structure','supercell'],
 py_modules=core_modules,
 license="MIT License",
```

