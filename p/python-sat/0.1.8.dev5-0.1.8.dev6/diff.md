# Comparing `tmp/python-sat-0.1.8.dev5.tar.gz` & `tmp/python-sat-0.1.8.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sat-0.1.8.dev5.tar", last modified: Sat Jun  3 01:33:44 2023, max compression
+gzip compressed data, was "python-sat-0.1.8.dev6.tar", last modified: Sun Jun  4 07:55:49 2023, max compression
```

## Comparing `python-sat-0.1.8.dev5.tar` & `python-sat-0.1.8.dev6.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.233020 python-sat-0.1.8.dev5/
--rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/LICENSE.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/MANIFEST.in
--rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-06-03 01:33:44.233115 python-sat-0.1.8.dev5/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567    14137 2023-04-21 08:05:23.000000 python-sat-0.1.8.dev5/README.rst
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.203440 python-sat-0.1.8.dev5/allies/
--rw-------   0 aign0002 (892519254) 907548567        0 2023-04-14 00:41:27.000000 python-sat-0.1.8.dev5/allies/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    13572 2023-05-09 14:01:54.000000 python-sat-0.1.8.dev5/allies/approxmc.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.206274 python-sat-0.1.8.dev5/cardenc/
--rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/bitwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev5/cardenc/card.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/clset.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/common.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/itot.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/ladder.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/mto.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/pairwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/ptypes.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/pycard.cc
--rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/seqcounter.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/sortcard.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/utils.hh
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.210505 python-sat-0.1.8.dev5/examples/
--rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/fm.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev5/examples/genhard.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    24012 2023-06-02 13:29:16.000000 python-sat-0.1.8.dev5/examples/hitman.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/lbx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev5/examples/lsu.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/mcsls.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev5/examples/models.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/musx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    23950 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/optux.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    67020 2023-05-25 10:53:45.000000 python-sat-0.1.8.dev5/examples/rc2.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/usage.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.212751 python-sat-0.1.8.dev5/pysat/
--rw-r--r--   0 aign0002 (892519254) 907548567      653 2023-06-03 01:29:39.000000 python-sat-0.1.8.dev5/pysat/__init__.py
--rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/pysat/_fileio.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/pysat/_utils.py
--rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/pysat/card.py
--rw-r--r--   0 aign0002 (892519254) 907548567    95959 2023-05-19 07:25:29.000000 python-sat-0.1.8.dev5/pysat/formula.py
--rw-r--r--   0 aign0002 (892519254) 907548567    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/pysat/pb.py
--rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev5/pysat/process.py
--rw-r--r--   0 aign0002 (892519254) 907548567   174192 2023-06-03 01:28:00.000000 python-sat-0.1.8.dev5/pysat/solvers.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.214048 python-sat-0.1.8.dev5/python_sat.egg-info/
--rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-06-03 01:33:44.000000 python-sat-0.1.8.dev5/python_sat.egg-info/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567     1863 2023-06-03 01:33:44.000000 python-sat-0.1.8.dev5/python_sat.egg-info/SOURCES.txt
--rw-r--r--   0 aign0002 (892519254) 907548567        1 2023-06-03 01:33:44.000000 python-sat-0.1.8.dev5/python_sat.egg-info/dependency_links.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       87 2023-06-03 01:33:44.000000 python-sat-0.1.8.dev5/python_sat.egg-info/requires.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       23 2023-06-03 01:33:44.000000 python-sat-0.1.8.dev5/python_sat.egg-info/top_level.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/requirements.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      107 2023-06-03 01:33:44.233388 python-sat-0.1.8.dev5/setup.cfg
--rw-r--r--   0 aign0002 (892519254) 907548567     6549 2023-04-21 07:47:02.000000 python-sat-0.1.8.dev5/setup.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.222854 python-sat-0.1.8.dev5/solvers/
--rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev5/solvers/cadical103.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev5/solvers/cadical153.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/glucose30.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/glucose41.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/lingeling.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/maplechrono.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/maplecm.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/maplesat.zip
--rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/mergesat3.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/minicard.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/minisat22.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/minisatgh.zip
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.229963 python-sat-0.1.8.dev5/solvers/patches/
--rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev5/solvers/patches/cadical103.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    66092 2023-06-03 01:29:02.000000 python-sat-0.1.8.dev5/solvers/patches/cadical153.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/glucose30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/glucose41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/gluecard30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/gluecard41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/lingeling.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev5/solvers/patches/maplechrono.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev5/solvers/patches/maplecm.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/maplesat.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev5/solvers/patches/mergesat3.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/minicard.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/minisat22.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/minisatgh.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    25391 2023-06-03 01:04:24.000000 python-sat-0.1.8.dev5/solvers/prepare.py
--rw-r--r--   0 aign0002 (892519254) 907548567   222394 2023-06-03 01:27:14.000000 python-sat-0.1.8.dev5/solvers/pysolvers.cc
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.232748 python-sat-0.1.8.dev5/tests/
--rw-r--r--   0 aign0002 (892519254) 907548567      948 2023-03-05 08:16:22.000000 python-sat-0.1.8.dev5/tests/test_accum_stats.py
--rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/tests/test_atmost.py
--rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/tests/test_atmost1.py
--rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/tests/test_atmostk.py
--rw-r--r--   0 aign0002 (892519254) 907548567     2408 2023-03-05 08:17:09.000000 python-sat-0.1.8.dev5/tests/test_cnfplus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/tests/test_equals1.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev5/tests/test_process.py
--rw-r--r--   0 aign0002 (892519254) 907548567      866 2023-03-05 08:17:46.000000 python-sat-0.1.8.dev5/tests/test_unique_model.py
--rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/tests/test_unique_mus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      643 2023-01-14 22:33:39.000000 python-sat-0.1.8.dev5/tests/test_warmstart.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.073139 python-sat-0.1.8.dev6/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/LICENSE.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/MANIFEST.in
+-rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-06-04 07:55:49.073227 python-sat-0.1.8.dev6/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567    14137 2023-04-21 08:05:23.000000 python-sat-0.1.8.dev6/README.rst
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.052925 python-sat-0.1.8.dev6/allies/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-04-14 00:41:27.000000 python-sat-0.1.8.dev6/allies/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    13572 2023-05-09 14:01:54.000000 python-sat-0.1.8.dev6/allies/approxmc.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.055528 python-sat-0.1.8.dev6/cardenc/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/bitwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev6/cardenc/card.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/clset.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/common.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/itot.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/ladder.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/mto.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/pairwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/ptypes.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/pycard.cc
+-rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/seqcounter.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/sortcard.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/cardenc/utils.hh
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.057669 python-sat-0.1.8.dev6/examples/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/examples/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/examples/fm.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev6/examples/genhard.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    25406 2023-06-04 07:07:20.000000 python-sat-0.1.8.dev6/examples/hitman.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/examples/lbx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev6/examples/lsu.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/examples/mcsls.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev6/examples/models.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/examples/musx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    25636 2023-06-04 07:39:47.000000 python-sat-0.1.8.dev6/examples/optux.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    67020 2023-05-25 10:53:45.000000 python-sat-0.1.8.dev6/examples/rc2.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/examples/usage.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.058958 python-sat-0.1.8.dev6/pysat/
+-rw-r--r--   0 aign0002 (892519254) 907548567      653 2023-06-04 07:53:48.000000 python-sat-0.1.8.dev6/pysat/__init__.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/pysat/_fileio.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/pysat/_utils.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/pysat/card.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    95959 2023-05-19 07:25:29.000000 python-sat-0.1.8.dev6/pysat/formula.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/pysat/pb.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev6/pysat/process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   175975 2023-06-04 02:20:27.000000 python-sat-0.1.8.dev6/pysat/solvers.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.059861 python-sat-0.1.8.dev6/python_sat.egg-info/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-06-04 07:55:48.000000 python-sat-0.1.8.dev6/python_sat.egg-info/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567     1863 2023-06-04 07:55:49.000000 python-sat-0.1.8.dev6/python_sat.egg-info/SOURCES.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567        1 2023-06-04 07:55:48.000000 python-sat-0.1.8.dev6/python_sat.egg-info/dependency_links.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       87 2023-06-04 07:55:48.000000 python-sat-0.1.8.dev6/python_sat.egg-info/requires.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       23 2023-06-04 07:55:48.000000 python-sat-0.1.8.dev6/python_sat.egg-info/top_level.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/requirements.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      107 2023-06-04 07:55:49.073491 python-sat-0.1.8.dev6/setup.cfg
+-rw-r--r--   0 aign0002 (892519254) 907548567     6549 2023-04-21 07:47:02.000000 python-sat-0.1.8.dev6/setup.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.064825 python-sat-0.1.8.dev6/solvers/
+-rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev6/solvers/cadical103.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev6/solvers/cadical153.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/glucose30.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/glucose41.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/lingeling.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/maplechrono.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/maplecm.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/maplesat.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/mergesat3.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/minicard.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/minisat22.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/minisatgh.zip
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.069556 python-sat-0.1.8.dev6/solvers/patches/
+-rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev6/solvers/patches/cadical103.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    66092 2023-06-03 01:29:02.000000 python-sat-0.1.8.dev6/solvers/patches/cadical153.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/glucose30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/glucose41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/gluecard30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/gluecard41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/lingeling.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev6/solvers/patches/maplechrono.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev6/solvers/patches/maplecm.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/maplesat.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev6/solvers/patches/mergesat3.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/minicard.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/minisat22.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/solvers/patches/minisatgh.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    25391 2023-06-03 01:04:24.000000 python-sat-0.1.8.dev6/solvers/prepare.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   223063 2023-06-04 02:10:25.000000 python-sat-0.1.8.dev6/solvers/pysolvers.cc
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-04 07:55:49.072728 python-sat-0.1.8.dev6/tests/
+-rw-r--r--   0 aign0002 (892519254) 907548567      948 2023-03-05 08:16:22.000000 python-sat-0.1.8.dev6/tests/test_accum_stats.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/tests/test_atmost.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/tests/test_atmost1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/tests/test_atmostk.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     2408 2023-03-05 08:17:09.000000 python-sat-0.1.8.dev6/tests/test_cnfplus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/tests/test_equals1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev6/tests/test_process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      866 2023-03-05 08:17:46.000000 python-sat-0.1.8.dev6/tests/test_unique_model.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev6/tests/test_unique_mus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      643 2023-01-14 22:33:39.000000 python-sat-0.1.8.dev6/tests/test_warmstart.py
```

### Comparing `python-sat-0.1.8.dev5/LICENSE.txt` & `python-sat-0.1.8.dev6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/PKG-INFO` & `python-sat-0.1.8.dev6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev5
+Version: 0.1.8.dev6
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
```

### Comparing `python-sat-0.1.8.dev5/README.rst` & `python-sat-0.1.8.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/allies/approxmc.py` & `python-sat-0.1.8.dev6/allies/approxmc.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/cardenc/bitwise.hh` & `python-sat-0.1.8.dev6/cardenc/bitwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/cardenc/card.hh` & `python-sat-0.1.8.dev6/cardenc/card.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/cardenc/clset.hh` & `python-sat-0.1.8.dev6/cardenc/clset.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/cardenc/common.hh` & `python-sat-0.1.8.dev6/cardenc/common.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/cardenc/itot.hh` & `python-sat-0.1.8.dev6/cardenc/itot.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/cardenc/ladder.hh` & `python-sat-0.1.8.dev6/cardenc/ladder.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/cardenc/mto.hh` & `python-sat-0.1.8.dev6/cardenc/mto.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/cardenc/pairwise.hh` & `python-sat-0.1.8.dev6/cardenc/pairwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/cardenc/ptypes.hh` & `python-sat-0.1.8.dev6/cardenc/ptypes.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/cardenc/pycard.cc` & `python-sat-0.1.8.dev6/cardenc/pycard.cc`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/cardenc/seqcounter.hh` & `python-sat-0.1.8.dev6/cardenc/seqcounter.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/cardenc/sortcard.hh` & `python-sat-0.1.8.dev6/cardenc/sortcard.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/cardenc/utils.hh` & `python-sat-0.1.8.dev6/cardenc/utils.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/examples/fm.py` & `python-sat-0.1.8.dev6/examples/fm.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/examples/genhard.py` & `python-sat-0.1.8.dev6/examples/genhard.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/examples/hitman.py` & `python-sat-0.1.8.dev6/examples/hitman.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,15 +209,16 @@
         be ``'sorted'`` by default. The MaxSAT-based enumerator can be chosen
         by setting ``htype`` to one of the following values: ``'maxsat'``,
         ``'mxsat'``, or ``'rc2'``. Alternatively, by setting it to ``'mcs'``
         or ``'lbx'``, a user can enforce using the :class:`.LBX` MCS
         enumerator. If ``htype`` is set to ``'mcsls'``, the :class:`.MCSls`
         enumerator is used. Finally, value ``'sat'`` can be given, in which
         case minimal hitting set enumeration will performed by means of a SAT
-        solver (can be either MiniSat-GH or Lingeling) with polarity setting.
+        solver (can be either MiniSat-GH, or Lingeling, or CaDiCaL 153) with
+        polarity setting.
 
         In either case, unless pure SAT-based hitting set enumeration is
         selected, an underlying problem solver can use a SAT oracle specified
         as an input parameter ``solver``. The default SAT solver is Glucose3
         (specified as ``g3``, see :class:`.SolverNames` for details). For
         SAT-based enumeration, MinisatGH is used as an underlying SAT solver.
 
@@ -280,14 +281,18 @@
         # various oracle options
         self.adapt    = mxs_adapt
         self.exhaust  = mxs_exhaust
         self.minz     = mxs_minz
         self.trim     = mxs_trim
         self.usecld   = mcs_usecld
 
+        # enumeration phase, for SAT-based oracles only
+        # (can be equal either to 1 or to -1)
+        self.phase = 1
+
         # hitman type: either a MaxSAT solver or an MCS enumerator
         if htype in ('maxsat', 'mxsat', 'rc2', 'sorted'):
             self.htype = 'rc2'
         elif htype in ('mcs', 'lbx'):
             self.htype = 'lbx'
         elif htype == 'mcsls':
             self.htype = 'mcsls'
@@ -350,17 +355,17 @@
         """
 
         # formula encoding the sets to hit
         formula = WCNFPlus()
 
         # hard clauses
         for to_hit in bootstrap_with:
-            to_hit = list(map(lambda obj: self.idpool.id(obj), to_hit))
+            to_hit = map(lambda obj: self.idpool.id(obj), to_hit)
 
-            formula.append(to_hit)
+            formula.append([self.phase * vid for vid in to_hit])
 
         # additional hard constraints
         for cl in subject_to:
             if not len(cl) == 2 or not type(cl[0]) in (list, tuple, set):
                 # this is a pure clause
                 formula.append(list(map(lambda a: self.idpool.id(a.obj) * (2 * a.sign - 1), cl)))
             else:
@@ -383,42 +388,62 @@
         elif self.htype == 'lbx':
             self.oracle = LBX(formula, solver_name=self.solver,
                     use_cld=self.usecld)
         elif self.htype == 'mcsls':
             self.oracle = MCSls(formula, solver_name=self.solver,
                     use_cld=self.usecld)
         else:  # 'sat'
-            assert self.solver in SolverNames.minisatgh + SolverNames.lingeling, \
+            assert self.solver in SolverNames.minisatgh + \
+                    SolverNames.lingeling + SolverNames.cadical153, \
                     'Hard polarity setting is unsupported by {0}'.format(self.solver)
 
             assert formula.atms == [], 'Native AtMostK constraints aren\'t' \
-            'supported by MinisatGH, Lingeling'
+            'supported by MinisatGH, Lingeling, or CaDiCaL 153'
 
             # setting up a SAT solver, so that it supports the same interface
             self.oracle = Solver(name=self.solver, bootstrap_with=formula.hard,
                                  use_timer=True)
 
             # MinisatGH supports warm start mode
             if self.solver in SolverNames.minisatgh:
                 self.oracle.start_mode(warm=True)
 
             # soft clauses are enforced by means of setting polarities
-            self.oracle.set_phases(literals=[cl[0] for cl in formula.soft])
+            self.oracle.set_phases(literals=[self.phase * cl[0] for cl in formula.soft])
 
             # "adding" the missing compute() and oracle_time() methods
             self.oracle.compute = lambda: [self.oracle.solve(), self.oracle.get_model()][-1]
             self.oracle.oracle_time = self.oracle.time_accum
 
             # adding a dummy VariableMap, as is in RC2 and LBX/MCSls
             VariableMap = collections.namedtuple('VariableMap', ['e2i', 'i2e'])
             self.oracle.vmap = VariableMap(e2i={}, i2e={})
             for vid in self.idpool.id2obj.keys():
                 self.oracle.vmap.e2i[vid] = vid
                 self.oracle.vmap.i2e[vid] = vid
 
+    def switch_phase(self):
+        """
+            If a pure SAT-based hitting set enumeration is used, it is
+            possible to instruct it to switch from enumerating target sets to
+            enumerating dual sets, by polarity switching. This is what this
+            method enables a user to do.
+        """
+
+        if self.htype == 'sat':
+            if self.solver in SolverNames.minisatgh:
+                # resetting the mode forces the solver to backtrack to level 0
+                self.oracle.start_mode(warm=True)
+
+            # switching the phase value
+            self.phase *= -1
+
+            # updating the preferences
+            self.oracle.set_phases(literals=[self.phase * (-v) for v in self.idpool.id2obj])
+
     def add_hard(self, clause, weights=None):
         """
             Add a hard constraint, which can be either a pure clause or an
             AtMostK constraint.
 
             Note that an optional parameter that can be passed to this method
             is ``weights``, which contains a mapping the objects under
@@ -461,15 +486,15 @@
         else:
             # dummy variable id mapping
             for vid in new_obj:
                 self.oracle.vmap.e2i[vid] = vid
                 self.oracle.vmap.i2e[vid] = vid
 
             # setting variable polarities
-            self.oracle.set_phases(literals=[-vid for vid in new_obj])
+            self.oracle.set_phases(literals=[self.phase * (-vid) for vid in new_obj])
 
     def delete(self):
         """
             Explicit destructor of the internal hitting set oracle.
         """
 
         if self.oracle:
@@ -486,16 +511,17 @@
             :rtype: list(obj)
         """
 
         model = self.oracle.compute()
 
         if model is not None:
             if self.htype in ('rc2', 'sat'):
-                # extracting a hitting set
-                self.hset = filter(lambda v: v > 0, model)
+                # extracting a hitting set; the use of map may look
+                # silly but this is to support negative phases too
+                self.hset = map(lambda v: abs(v), filter(lambda v: v * self.phase > 0, model))
             else:
                 self.hset = model
 
             return list(map(lambda vid: self.idpool.id2obj[vid], self.hset))
 
     def hit(self, to_hit, weights=None):
         """
@@ -517,30 +543,31 @@
 
         # translating objects to variables
         to_hit = list(map(lambda obj: self.idpool.id(obj), to_hit))
 
         # a soft clause should be added for each new object
         new_obj = list(filter(lambda vid: vid not in self.oracle.vmap.e2i, to_hit))
 
-        # new hard clause
-        self.oracle.add_clause(to_hit)
+        # new hard clause; phase multiplication is needed
+        # for making phase switching possible (pure SAT only)
+        self.oracle.add_clause([self.phase * vid for vid in to_hit])
 
         # new soft clauses
         if self.htype != 'sat':
             # new soft clauses
             for vid in new_obj:
                 self.oracle.add_clause([-vid], 1 if not weights else weights[self.idpool.obj(vid)])
         else:
             # dummy variable id mapping
             for vid in new_obj:
                 self.oracle.vmap.e2i[vid] = vid
                 self.oracle.vmap.i2e[vid] = vid
 
             # setting variable polarities
-            self.oracle.set_phases(literals=[-vid for vid in new_obj])
+            self.oracle.set_phases(literals=[self.phase * (-vid) for vid in new_obj])
 
     def block(self, to_block, weights=None):
         """
             The method serves for imposing a constraint forbidding the hitting
             set solver to compute a given hitting set. Each set to block is
             encoded as a hard clause in the MaxSAT problem formulation, which
             is then added to the underlying oracle.
@@ -559,29 +586,30 @@
 
         # translating objects to variables
         to_block = list(map(lambda obj: self.idpool.id(obj), to_block))
 
         # a soft clause should be added for each new object
         new_obj = list(filter(lambda vid: vid not in self.oracle.vmap.e2i, to_block))
 
-        # new hard clause
-        self.oracle.add_clause([-vid for vid in to_block])
+        # new hard clause; phase multiplication is needed
+        # for making phase switching possible (pure SAT only)
+        self.oracle.add_clause([self.phase * (-vid) for vid in to_block])
 
         # new soft clauses
         if self.htype != 'sat':
             for vid in new_obj:
                 self.oracle.add_clause([-vid], 1 if not weights else weights[self.idpool.obj(vid)])
         else:
             # dummy variable id mapping
             for vid in new_obj:
                 self.oracle.vmap.e2i[vid] = vid
                 self.oracle.vmap.i2e[vid] = vid
 
             # setting variable polarities
-            self.oracle.set_phases(literals=[-vid for vid in new_obj])
+            self.oracle.set_phases(literals=[self.phase * (-vid) for vid in new_obj])
 
     def enumerate(self):
         """
             The method can be used as a simple iterator computing and blocking
             the hitting sets on the fly. It essentially calls :func:`get`
             followed by :func:`block`. Each hitting set is reported as a list
             of objects in the original problem domain, i.e. it is mapped back
```

### Comparing `python-sat-0.1.8.dev5/examples/lbx.py` & `python-sat-0.1.8.dev6/examples/lbx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/examples/lsu.py` & `python-sat-0.1.8.dev6/examples/lsu.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/examples/mcsls.py` & `python-sat-0.1.8.dev6/examples/mcsls.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/examples/models.py` & `python-sat-0.1.8.dev6/examples/models.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/examples/musx.py` & `python-sat-0.1.8.dev6/examples/musx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/examples/optux.py` & `python-sat-0.1.8.dev6/examples/optux.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,14 +154,22 @@
         Two additional optional parameters ``unsorted`` and ``dcalls`` can be
         used to instruct the tool to enumerate MUSes in the unsorted fashion,
         i.e. optimal MUSes are not guaranteed to go first. For this,
         :class:`OptUx` applies LBX-like MCS enumeration (it uses :class:`.LBX`
         directly). Parameter ``dcalls`` can be applied to instruct the
         underlying MCS enumerator to apply clause D oracle calls.
 
+        Another optional paramater ``puresat`` can be used to instruct OptUx
+        to run a purely SAT-based minimal hitting set enumerator, following
+        the ideas of [7]_. The value of ``puresat`` can be either ``False``,
+        meaning that no pure SAT enumeration is to be done or be equal to
+        ``'mgh'``, ``'cd15'``, or ``'lgl'`` - these are the solvers that
+        support *hard* phase setting, i.e. user preferences will not be
+        overwritten by the *phase saving* heuristic [8]_.
+
         Finally, one more optional input parameter ``cover`` is to be used
         when exhaustive enumeration of MUSes is not necessary and the tool can
         stop as soon as a given formula is covered by the set of currently
         computed MUSes. This can be made to work if the soft clauses of
         ``formula`` are of size 1.
 
         .. [5] Alexey Ignatiev, Antonio Morgado, Joao Marques-Silva. *RC2: an
@@ -169,44 +177,55 @@
             2019. pp. 53-64
 
         .. [6] Gilles Audemard, Jean-Marie Lagniez, Laurent Simon.
             *Improving Glucose for Incremental SAT Solving with
             Assumptions: Application to MUS Extraction*. SAT 2013.
             pp. 309-317
 
+        .. [7] Enrico Giunchiglia, Marco Maratea. *Solving Optimization
+            Problems with DLL*. ECAI 2006. pp. 377-381
+
+        .. [8] Knot Pipatsrisawat, Adnan Darwiche. *A Lightweight Component
+            Caching Scheme for Satisfiability Solvers*. SAT 2007. pp. 294-299
+
+
         :param formula: (weighted) (partial) CNFPlus formula
         :param solver: SAT oracle name
         :param adapt: detect and adapt intrinsic AtMost1 constraints
         :param cover: CNFPlus formula to cover when doing MUS enumeration
         :param dcalls: apply clause D oracle calls (for unsorted enumeration only)
         :param exhaust: do core exhaustion
         :param minz: do heuristic core reduction
+        :param puresat: use pure SAT-based hitting set enumeration
         :param unsorted: apply unsorted MUS enumeration
         :param trim: do core trimming at most this number of times
         :param verbose: verbosity level
 
         :type formula: :class:`.WCNFPlus`
         :type solver: str
         :type adapt: bool
         :type cover: :class:`.CNFPlus`
         :type dcalls: bool
         :type exhaust: bool
         :type minz: bool
+        :type puresat: str
         :type unsorted: bool
         :type trim: int
         :type verbose: int
     """
 
     def __init__(self, formula, solver='g3', adapt=False, cover=None,
-            dcalls=False, exhaust=False, minz=False, unsorted=False,
-            trim=False, verbose=0):
+            dcalls=False, exhaust=False, minz=False, puresat=False,
+                 unsorted=False, trim=False, verbose=0):
         """
             Constructor.
         """
 
+        assert not puresat or unsorted, '\'unsorted\' needs to be True for pure SAT mode'
+
         # verbosity level
         self.verbose = verbose
 
         # constructing a local copy of the formula
         self.formula = WCNFPlus()
         self.formula.hard = formula.hard[:]
         self.formula.wght = formula.wght[:]
@@ -237,18 +256,22 @@
                 len(to_hit) + len(self.units)))
 
         if not unsorted:
             # MaxSAT-based hitting set enumerator
             self.hitman = Hitman(bootstrap_with=to_hit, weights=self.weights,
                     solver=solver, htype='sorted', mxs_adapt=adapt,
                     mxs_exhaust=exhaust, mxs_minz=minz, mxs_trim=trim)
-        else:
+        elif not puresat:
             # MCS-based hitting set enumerator
             self.hitman = Hitman(bootstrap_with=to_hit, weights=self.weights,
                     solver=solver, htype='lbx', mcs_usecld=dcalls)
+        else:
+            # pure SAT-based hitting set enumerator with preferred phases
+            self.hitman = Hitman(bootstrap_with=to_hit, weights=self.weights,
+                    solver=puresat, htype='sat')
 
         # adding the formula to cover to the hitting set enumerator
         self.cover = cover is not None
         if cover:
             # mapping literals to Hitman's atoms
             m = lambda l: Atom(l, sign=True) if -l not in self.weights else Atom(-l, sign=False)
 
@@ -516,29 +539,31 @@
 #==============================================================================
 def parse_options():
     """
         Parses command-line options.
     """
 
     try:
-        opts, args = getopt.getopt(sys.argv[1:], 'ac:de:hms:t:uvx',
+        opts, args = getopt.getopt(sys.argv[1:], 'ac:de:hmp:s:t:uvx',
                 ['adapt', 'cover=', 'dcalls', 'enum=', 'exhaust', 'help',
-                    'minimize', 'solver=', 'unsorted', 'trim=', 'verbose'])
+                    'minimize', 'solver=', 'puresat=', 'unsorted', 'trim=',
+                    'verbose'])
     except getopt.GetoptError as err:
         sys.stderr.write(str(err).capitalize() + '\n')
         usage()
         sys.exit(1)
 
     adapt = False
     cover = None
     dcalls = False
     exhaust = False
     minz = False
     to_enum = 1
     solver = 'm22'
+    puresat = False
     unsorted = False
     trim = 0
     verbose = 1
 
     for opt, arg in opts:
         if opt in ('-a', '--adapt'):
             adapt = True
@@ -553,62 +578,67 @@
             if to_enum != 'all':
                 to_enum = int(to_enum)
         elif opt in ('-h', '--help'):
             usage()
             sys.exit(0)
         elif opt in ('-m', '--minimize'):
             minz = True
+        elif opt in ('-p', '--puresat'):
+            puresat = str(arg)
         elif opt in ('-s', '--solver'):
             solver = str(arg)
         elif opt in ('-u', '--unsorted'):
             unsorted = True
         elif opt in ('-t', '--trim'):
             trim = int(arg)
         elif opt in ('-v', '--verbose'):
             verbose += 1
         elif opt in ('-x', '--exhaust'):
             exhaust = True
         else:
             assert False, 'Unhandled option: {0} {1}'.format(opt, arg)
 
     return adapt, cover, dcalls, exhaust, minz, trim, to_enum, solver, \
-            unsorted, verbose, args
+            puresat, unsorted, verbose, args
 
 
 #
 #==============================================================================
 def usage():
     """
         Prints help message.
     """
 
     print('Usage:', os.path.basename(sys.argv[0]), '[options] file')
     print('Options:')
-    print('        -a, --adapt             Try to adapt (simplify) input formula')
-    print('        -c, --cover=<string>    Stop MUS enumeration as soon as this formula is covered')
-    print('                                Available values: any valid file path, none (default = none)')
-    print('        -d, --dcalls            Apply clause D calls (in unsorted enumeration only)')
-    print('        -e, --enum=<string>     Enumerate top-k solutions')
-    print('                                Available values: [1 .. INT_MAX], all (default: 1)')
-    print('        -h, --help              Show this message')
-    print('        -m, --minimize          Use a heuristic unsatisfiable core minimizer')
-    print('        -s, --solver            SAT solver to use')
-    print('                                Available values: g3, g4, lgl, mcb, mcm, mpl, m22, mc, mgh (default = m22)')
-    print('        -t, --trim=<int>        How many times to trim unsatisfiable cores')
-    print('                                Available values: [0 .. INT_MAX] (default = 0)')
-    print('        -u, --unsorted          Enumerate MUSes in an unsorted way')
-    print('        -v, --verbose           Be verbose')
-    print('        -x, --exhaust           Exhaust new unsatisfiable cores')
+    print('        -a, --adapt               Try to adapt (simplify) input formula')
+    print('        -c, --cover=<string>      Stop MUS enumeration as soon as this formula is covered')
+    print('                                  Available values: any valid file path, none (default = none)')
+    print('        -d, --dcalls              Apply clause D calls (in unsorted enumeration only)')
+    print('        -e, --enum=<string>       Enumerate top-k solutions')
+    print('                                  Available values: [1 .. INT_MAX], all (default: 1)')
+    print('        -h, --help                Show this message')
+    print('        -m, --minimize            Use a heuristic unsatisfiable core minimizer')
+    print('        -p, --puresat=<string>    Use a pure SAT-based hitting set enumerator')
+    print('                                  Available values: cd15, lgl, mgh (default = mgh)')
+    print('                                  Requires: unsorted mode, i.e. \'-u\'')
+    print('        -s, --solver              SAT solver to use')
+    print('                                  Available values: g3, g4, lgl, mcb, mcm, mpl, m22, mc, mgh (default = m22)')
+    print('        -t, --trim=<int>          How many times to trim unsatisfiable cores')
+    print('                                  Available values: [0 .. INT_MAX] (default = 0)')
+    print('        -u, --unsorted            Enumerate MUSes in an unsorted way')
+    print('        -v, --verbose             Be verbose')
+    print('        -x, --exhaust             Exhaust new unsatisfiable cores')
 
 
 #
 #==============================================================================
 if __name__ == '__main__':
-    adapt, cover, dcalls, exhaust, minz, trim, to_enum, solver, unsorted, \
-            verbose, files = parse_options()
+    adapt, cover, dcalls, exhaust, minz, trim, to_enum, solver, puresat, \
+            unsorted, verbose, files = parse_options()
 
     if files:
         # reading standard CNF, WCNF, or (W)CNF+
         if re.search(r'cnf[p|+]?(\.(gz|bz2|lzma|xz))?$', files[0]):
             if re.search(r'\.wcnf[p|+]?(\.(gz|bz2|lzma|xz))?$', files[0]):
                 formula = WCNFPlus(from_file=files[0])
             else:  # expecting '*.cnf[,p,+].*'
@@ -616,16 +646,16 @@
 
         if cover:  # expecting  '*.cnf[,p,+].*' only!
             assert re.search(r'cnf[p|+]?(\.(gz|bz2|lzma|xz))?$', cover), 'wrong file for formula to cover'
             cover = CNFPlus(from_file=cover)
 
         # creating an object of OptUx
         with OptUx(formula, solver=solver, adapt=adapt, cover=cover,
-                dcalls=dcalls, exhaust=exhaust, minz=minz, unsorted=unsorted,
-                trim=trim, verbose=verbose) as optux:
+                dcalls=dcalls, exhaust=exhaust, minz=minz, puresat=puresat,
+                unsorted=unsorted, trim=trim, verbose=verbose) as optux:
 
             # iterating over the necessary number of optimal MUSes
             for i, mus in enumerate(optux.enumerate()):
                 # reporting the current solution
                 if verbose:
                     print('c mus:', ' '.join([str(cl_id) for cl_id in mus]), '0')
```

### Comparing `python-sat-0.1.8.dev5/examples/rc2.py` & `python-sat-0.1.8.dev6/examples/rc2.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/examples/usage.py` & `python-sat-0.1.8.dev6/examples/usage.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/pysat/__init__.py` & `python-sat-0.1.8.dev6/pysat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ##  Created on: Mar 4, 2017
 ##      Author: Alexey S. Ignatiev
 ##      E-mail: aignatiev@ciencias.ulisboa.pt
 ##
 
 # current version
 #==============================================================================
-VERSION = (0, 1, 8, "dev", 5)
+VERSION = (0, 1, 8, "dev", 6)
 
 
 # PEP440 Format
 #==============================================================================
 __version__ = "%d.%d.%d.%s%d" % VERSION if len(VERSION) == 5 else \
               "%d.%d.%d" % VERSION
```

### Comparing `python-sat-0.1.8.dev5/pysat/_fileio.py` & `python-sat-0.1.8.dev6/pysat/_fileio.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/pysat/_utils.py` & `python-sat-0.1.8.dev6/pysat/_utils.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/pysat/card.py` & `python-sat-0.1.8.dev6/pysat/card.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/pysat/formula.py` & `python-sat-0.1.8.dev6/pysat/formula.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/pysat/pb.py` & `python-sat-0.1.8.dev6/pysat/pb.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/pysat/process.py` & `python-sat-0.1.8.dev6/pysat/process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/pysat/solvers.py` & `python-sat-0.1.8.dev6/pysat/solvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,14 +447,35 @@
                 >>> model_count('mpl', cnf, vlimit=16, warm_start=True)
                 58651 models in 0.3951s
         """
 
         if self.solver:
             self.solver.start_mode(warm)
 
+    def configure(self, parameters):
+        """
+            Configure :class:`Cadical153` by setting some of the predefined
+            parameters to selected values. Note that this method can be
+            invoked only for :class:`Cadical153` -- no other solvers support
+            this for now.
+
+            Also note that this call must follow the creation of the new
+            solver object; otherwise, an exception may be thrown.
+
+            The list of available options of :class:`Cadical153` and the
+            corresponding values they can be assigned to is provided `here
+            <https://github.com/arminbiere/cadical/blob/master/src/options.hpp>`__.
+
+            :param parameters: parameter names mapped to integer values
+            :type parameters: dict
+        """
+
+        if self.solver and type(self.solver) == Cadical153:
+            self.solver.configure(parameters)
+
     def accum_stats(self):
         """
             Get accumulated low-level stats from the solver. Currently, the
             statistics includes the number of restarts, conflicts, decisions,
             and propagations.
 
             :rtype: dict.
@@ -1622,14 +1643,32 @@
                 for clause in bootstrap_with:
                     self.add_clause(clause)
 
             self.use_timer = use_timer
             self.call_time = 0.0  # time spent for the last call to oracle
             self.accu_time = 0.0  # time accumulated for all calls to oracle
 
+    def configure(self, parameters):
+        """
+            Configure Cadical153 by setting some of the predefined parameters.
+            This call must follow the creation of the new solver object;
+            otherwise, an exception will be thrown.
+
+            The list of available options and the corresponding
+            values they can be assigned to is provided `here
+            <https://github.com/arminbiere/cadical/blob/master/src/options.hpp>`__.
+
+            :param parameters: parameter names mapped to integer values
+            :type parameters: dict
+        """
+
+        if self.cadical:
+            for name, value in parameters.items():
+                pysolvers.cadical153_set(self.cadical, name, value)
+
     def delete(self):
         """
             Destructor.
         """
 
         if self.cadical:
             pysolvers.cadical153_del(self.cadical, self.prfile)
@@ -1757,15 +1796,20 @@
         raise NotImplementedError('Simple literal propagation is not yet implemented for CaDiCaL.')
 
     def set_phases(self, literals=[]):
         """
             Sets polarities of a given list of variables.
         """
 
-        raise NotImplementedError('Setting preferred phases is not yet implemented for CaDiCaL.')
+        if self.cadical:
+            # making sure 'lucky' phases don't interfere with our preferences
+            self.configure({'lucky': 0})
+
+            # setting preferred phases
+            pysolvers.cadical153_setphases(self.cadical, literals)
 
     def get_status(self):
         """
             Returns solver's status.
         """
 
         if self.cadical:
```

### Comparing `python-sat-0.1.8.dev5/python_sat.egg-info/PKG-INFO` & `python-sat-0.1.8.dev6/python_sat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev5
+Version: 0.1.8.dev6
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
```

### Comparing `python-sat-0.1.8.dev5/python_sat.egg-info/SOURCES.txt` & `python-sat-0.1.8.dev6/python_sat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/setup.py` & `python-sat-0.1.8.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/cadical103.tar.gz` & `python-sat-0.1.8.dev6/solvers/cadical103.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/cadical153.tar.gz` & `python-sat-0.1.8.dev6/solvers/cadical153.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/glucose30.tar.gz` & `python-sat-0.1.8.dev6/solvers/glucose30.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/glucose41.tar.gz` & `python-sat-0.1.8.dev6/solvers/glucose41.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/lingeling.tar.gz` & `python-sat-0.1.8.dev6/solvers/lingeling.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/maplechrono.zip` & `python-sat-0.1.8.dev6/solvers/maplechrono.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/maplecm.zip` & `python-sat-0.1.8.dev6/solvers/maplecm.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/maplesat.zip` & `python-sat-0.1.8.dev6/solvers/maplesat.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/mergesat3.tar.gz` & `python-sat-0.1.8.dev6/solvers/mergesat3.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/minicard.tar.gz` & `python-sat-0.1.8.dev6/solvers/minicard.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/minisat22.tar.gz` & `python-sat-0.1.8.dev6/solvers/minisat22.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/minisatgh.zip` & `python-sat-0.1.8.dev6/solvers/minisatgh.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/cadical103.patch` & `python-sat-0.1.8.dev6/solvers/patches/cadical103.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/cadical153.patch` & `python-sat-0.1.8.dev6/solvers/patches/cadical153.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/glucose30.patch` & `python-sat-0.1.8.dev6/solvers/patches/glucose30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/glucose41.patch` & `python-sat-0.1.8.dev6/solvers/patches/glucose41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/gluecard30.patch` & `python-sat-0.1.8.dev6/solvers/patches/gluecard30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/gluecard41.patch` & `python-sat-0.1.8.dev6/solvers/patches/gluecard41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/lingeling.patch` & `python-sat-0.1.8.dev6/solvers/patches/lingeling.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/maplechrono.patch` & `python-sat-0.1.8.dev6/solvers/patches/maplechrono.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/maplecm.patch` & `python-sat-0.1.8.dev6/solvers/patches/maplecm.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/maplesat.patch` & `python-sat-0.1.8.dev6/solvers/patches/maplesat.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/mergesat3.patch` & `python-sat-0.1.8.dev6/solvers/patches/mergesat3.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/minicard.patch` & `python-sat-0.1.8.dev6/solvers/patches/minicard.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/minisat22.patch` & `python-sat-0.1.8.dev6/solvers/patches/minisat22.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/patches/minisatgh.patch` & `python-sat-0.1.8.dev6/solvers/patches/minisatgh.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/prepare.py` & `python-sat-0.1.8.dev6/solvers/prepare.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/solvers/pysolvers.cc` & `python-sat-0.1.8.dev6/solvers/pysolvers.cc`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,16 @@
 using namespace std;
 
 // docstrings
 //=============================================================================
 static char    module_docstring[] = "This module provides a wrapper interface "
                                     "for several SAT solvers.";
 static char       new_docstring[] = "Create a new solver object.";
+static char       set_docstring[] = "Set a value of a solver's parameter "
+                                    "(for CaDiCaL 153 only).";
 static char     addcl_docstring[] = "Add a clause to formula.";
 static char     addam_docstring[] = "Add an atmost constraint to formula "
                                     "(for Minicard only).";
 static char     solve_docstring[] = "Solve a given CNF instance.";
 static char       lim_docstring[] = "Solve a given CNF instance within a budget.";
 static char   process_docstring[] = "(Pre)process a given CNF formula using "
                                     "the CaDiCaL 1.5.3 preprocessor";
@@ -127,20 +129,21 @@
 	static PyObject *py_cadical103_nof_vars  (PyObject *, PyObject *);
 	static PyObject *py_cadical103_nof_cls   (PyObject *, PyObject *);
 	static PyObject *py_cadical103_del       (PyObject *, PyObject *);
 	static PyObject *py_cadical103_acc_stats (PyObject *, PyObject *);
 #endif
 #ifdef WITH_CADICAL153
 	static PyObject *py_cadical153_new       (PyObject *, PyObject *);
+	static PyObject *py_cadical153_set       (PyObject *, PyObject *);
 	static PyObject *py_cadical153_add_cl    (PyObject *, PyObject *);
 	static PyObject *py_cadical153_process   (PyObject *, PyObject *);
 	static PyObject *py_cadical153_restore   (PyObject *, PyObject *);
 	static PyObject *py_cadical153_solve     (PyObject *, PyObject *);
 	static PyObject *py_cadical153_solve_lim (PyObject *, PyObject *);
-	/* static PyObject *py_cadical153_setphases (PyObject *, PyObject *); */
+	static PyObject *py_cadical153_setphases (PyObject *, PyObject *);
 	static PyObject *py_cadical153_cbudget   (PyObject *, PyObject *);
 	static PyObject *py_cadical153_dbudget   (PyObject *, PyObject *);
 	static PyObject *py_cadical153_tracepr   (PyObject *, PyObject *);
 	static PyObject *py_cadical153_core      (PyObject *, PyObject *);
 	static PyObject *py_cadical153_model     (PyObject *, PyObject *);
 	static PyObject *py_cadical153_nof_vars  (PyObject *, PyObject *);
 	static PyObject *py_cadical153_nof_cls   (PyObject *, PyObject *);
@@ -399,18 +402,19 @@
 	{ "cadical103_nof_vars",  py_cadical103_nof_vars,  METH_VARARGS,    nvars_docstring },
 	{ "cadical103_nof_cls",   py_cadical103_nof_cls,   METH_VARARGS,     ncls_docstring },
 	{ "cadical103_del",       py_cadical103_del,       METH_VARARGS,      del_docstring },
 	{ "cadical103_acc_stats", py_cadical103_acc_stats, METH_VARARGS, acc_stat_docstring },
 #endif
 #ifdef WITH_CADICAL153
 	{ "cadical153_new",       py_cadical153_new,       METH_VARARGS,      new_docstring },
+	{ "cadical153_set",       py_cadical153_set,       METH_VARARGS,      set_docstring },
 	{ "cadical153_add_cl",    py_cadical153_add_cl,    METH_VARARGS,    addcl_docstring },
 	{ "cadical153_solve",     py_cadical153_solve,     METH_VARARGS,    solve_docstring },
 	{ "cadical153_solve_lim", py_cadical153_solve_lim, METH_VARARGS,      lim_docstring },
-	/* { "cadical153_setphases", py_cadical153_setphases, METH_VARARGS,   phases_docstring }, */
+	{ "cadical153_setphases", py_cadical153_setphases, METH_VARARGS,   phases_docstring },
 	{ "cadical153_cbudget",   py_cadical153_cbudget,   METH_VARARGS,  cbudget_docstring },
 	{ "cadical153_dbudget",   py_cadical153_dbudget,   METH_VARARGS,  dbudget_docstring },
 	{ "cadical153_process",   py_cadical153_process,   METH_VARARGS,  process_docstring },
 	{ "cadical153_restore",   py_cadical153_restore,   METH_VARARGS,  restore_docstring },
 	{ "cadical153_tracepr",   py_cadical153_tracepr,   METH_VARARGS,  tracepr_docstring },
 	{ "cadical153_core",      py_cadical153_core,      METH_VARARGS,     core_docstring },
 	{ "cadical153_model",     py_cadical153_model,     METH_VARARGS,    model_docstring },
@@ -1272,14 +1276,37 @@
 	}
 
 	return void_to_pyobj((void *)s);
 }
 
 //
 //=============================================================================
+static PyObject *py_cadical153_set(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	const char *name;
+	int64_t value;
+
+	if (!PyArg_ParseTuple(args, "Osl", &s_obj, &name, &value))
+		return NULL;
+
+	// get pointer to solver
+	CaDiCaL153::Solver *s = (CaDiCaL153::Solver *)pyobj_to_void(s_obj);
+
+	// set the parameter
+	CaDiCaL153::State temp = s->state();
+	s->set_state(CaDiCaL153::State::CONFIGURING); // temporarily set state to configuring to enable option setting
+	s->set(name, value);
+	s->set_state(temp); // restore the original state
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
 static PyObject *py_cadical153_add_cl(PyObject *self, PyObject *args)
 {
 	PyObject *s_obj;
 	PyObject *c_obj;
 
 	if (!PyArg_ParseTuple(args, "OO", &s_obj, &c_obj))
 		return NULL;
@@ -1591,59 +1618,59 @@
 	if (main_thread)
 		PyOS_setsig(SIGINT, sig_save);
 
 	PyObject *ret = pyint_from_cint(res);
 	return ret;
 }
 
-// calling phase() does not seem to work for now!
+//
 //=============================================================================
-/* static PyObject *py_cadical153_setphases(PyObject *self, PyObject *args) */
-/* { */
-/* 	PyObject *s_obj; */
-/* 	PyObject *p_obj;  // polarities given as a list of integer literals */
-
-/* 	if (!PyArg_ParseTuple(args, "OO", &s_obj, &p_obj)) */
-/* 		return NULL; */
-
-/* 	// get pointer to solver */
-/* 	CaDiCaL153::Solver *s = (CaDiCaL153::Solver *)pyobj_to_void(s_obj); */
-
-/* 	// assumptions iterator */
-/* 	PyObject *i_obj = PyObject_GetIter(p_obj); */
-/* 	if (i_obj == NULL) { */
-/* 		PyErr_SetString(PyExc_RuntimeError, */
-/* 				"Object does not seem to be an iterable."); */
-/* 		return NULL; */
-/* 	} */
-
-/* 	PyObject *l_obj; */
-/* 	while ((l_obj = PyIter_Next(i_obj)) != NULL) { */
-/* 		if (!pyint_check(l_obj)) { */
-/* 			Py_DECREF(l_obj); */
-/* 			Py_DECREF(i_obj); */
-/* 			PyErr_SetString(PyExc_TypeError, "integer expected"); */
-/* 			return NULL; */
-/* 		} */
-
-/* 		int l = pyint_to_cint(l_obj); */
-/* 		Py_DECREF(l_obj); */
-
-/* 		if (l == 0) { */
-/* 			Py_DECREF(i_obj); */
-/* 			PyErr_SetString(PyExc_ValueError, "non-zero integer expected"); */
-/* 			return NULL; */
-/* 		} */
-
-/* 		s->phase(l); */
-/* 	} */
-
-/* 	Py_DECREF(i_obj); */
-/* 	Py_RETURN_NONE; */
-/* } */
+static PyObject *py_cadical153_setphases(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	PyObject *p_obj;  // polarities given as a list of integer literals
+
+	if (!PyArg_ParseTuple(args, "OO", &s_obj, &p_obj))
+		return NULL;
+
+	// get pointer to solver
+	CaDiCaL153::Solver *s = (CaDiCaL153::Solver *)pyobj_to_void(s_obj);
+
+	// assumptions iterator
+	PyObject *i_obj = PyObject_GetIter(p_obj);
+	if (i_obj == NULL) {
+		PyErr_SetString(PyExc_RuntimeError,
+				"Object does not seem to be an iterable.");
+		return NULL;
+	}
+
+	PyObject *l_obj;
+	while ((l_obj = PyIter_Next(i_obj)) != NULL) {
+		if (!pyint_check(l_obj)) {
+			Py_DECREF(l_obj);
+			Py_DECREF(i_obj);
+			PyErr_SetString(PyExc_TypeError, "integer expected");
+			return NULL;
+		}
+
+		int l = pyint_to_cint(l_obj);
+		Py_DECREF(l_obj);
+
+		if (l == 0) {
+			Py_DECREF(i_obj);
+			PyErr_SetString(PyExc_ValueError, "non-zero integer expected");
+			return NULL;
+		}
+
+		s->phase(l);
+	}
+
+	Py_DECREF(i_obj);
+	Py_RETURN_NONE;
+}
 
 //
 //=============================================================================
 static PyObject *py_cadical153_cbudget(PyObject *self, PyObject *args)
 {
 	PyObject *s_obj;
 	int64_t budget;
```

### Comparing `python-sat-0.1.8.dev5/tests/test_accum_stats.py` & `python-sat-0.1.8.dev6/tests/test_accum_stats.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/tests/test_atmost1.py` & `python-sat-0.1.8.dev6/tests/test_atmost1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/tests/test_atmostk.py` & `python-sat-0.1.8.dev6/tests/test_atmostk.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/tests/test_cnfplus.py` & `python-sat-0.1.8.dev6/tests/test_cnfplus.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/tests/test_equals1.py` & `python-sat-0.1.8.dev6/tests/test_equals1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/tests/test_process.py` & `python-sat-0.1.8.dev6/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/tests/test_unique_model.py` & `python-sat-0.1.8.dev6/tests/test_unique_model.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/tests/test_unique_mus.py` & `python-sat-0.1.8.dev6/tests/test_unique_mus.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev5/tests/test_warmstart.py` & `python-sat-0.1.8.dev6/tests/test_warmstart.py`

 * *Files identical despite different names*

