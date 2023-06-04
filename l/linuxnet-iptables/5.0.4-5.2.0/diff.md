# Comparing `tmp/linuxnet-iptables-5.0.4.tar.gz` & `tmp/linuxnet-iptables-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/panos/dvl/gitlab/iptables/linuxnet-iptables/dist/tmpwbcicdk4/linuxnet-iptables-5.0.4.tar", last modified: Sun Mar  5 20:37:11 2023, max compression
+gzip compressed data, was "linuxnet-iptables-5.2.0.tar", last modified: Sun Jun  4 01:22:27 2023, max compression
```

## Comparing `linuxnet-iptables-5.0.4.tar` & `linuxnet-iptables-5.2.0.tar`

### file list

```diff
@@ -1,97 +1,101 @@
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/docs/
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/docs/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/matches/commentmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)      990 2023-02-05 23:48:23.000000 linuxnet-iptables-5.0.4/docs/matches/connmarkmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1583 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/matches/conntrackmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/matches/icmpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-5.0.4/docs/matches/limitmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1439 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/matches/markmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1965 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/matches/ownermatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-5.0.4/docs/matches/packetmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/matches/packettypematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/matches/statematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1492 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/matches/tcpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/matches/tcpmssmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1521 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/matches/ttlmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/matches/udpmatch.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/docs/targets/
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/targets/chaintarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/targets/connmarktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/targets/dnattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/targets/logtarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/targets/marktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/targets/masqueradetarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/targets/rejecttarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/targets/snattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/targets/ttltarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-5.0.4/docs/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-5.0.4/docs/chain.rst
--rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-5.0.4/docs/conf.py
--rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/exception.rst
--rw-r--r--   0 panos     (1001) users      (100)     8374 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/extensibility.rst
--rw-r--r--   0 panos     (1001) users      (100)     3319 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/index.rst
--rw-r--r--   0 panos     (1001) users      (100)     3187 2023-03-01 20:08:53.000000 linuxnet-iptables-5.0.4/docs/iptables_api.rst
--rw-r--r--   0 panos     (1001) users      (100)     3176 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/match-example.py
--rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-5.0.4/docs/match.rst
--rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-5.0.4/docs/rule.rst
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-5.0.4/docs/table.rst
--rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/docs/target-example.py
--rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-5.0.4/docs/target.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/linuxnet/
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1295 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     2889 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/commentmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2271 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/connmarkmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     5226 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/conntrackmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     9769 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/icmpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4667 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/limitmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3852 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/markmatch.py
--rw-r--r--   0 panos     (1001) users      (100)    14678 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/match.py
--rw-r--r--   0 panos     (1001) users      (100)     7798 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/ownermatch.py
--rw-r--r--   0 panos     (1001) users      (100)     7343 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/packetmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2844 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/packettypematch.py
--rw-r--r--   0 panos     (1001) users      (100)     3155 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/statematch.py
--rw-r--r--   0 panos     (1001) users      (100)    10665 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/tcpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3833 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/tcpmssmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4322 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/ttlmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2724 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/udpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     5060 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/matches/util.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/targets/
--rw-r--r--   0 panos     (1001) users      (100)     1087 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/targets/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     7386 2023-03-05 20:30:06.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/targets/connmarktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6518 2023-02-08 00:19:00.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/targets/logtarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6551 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/targets/marktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     4133 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/targets/masqueradetarget.py
--rw-r--r--   0 panos     (1001) users      (100)     8146 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/targets/nattarget.py
--rw-r--r--   0 panos     (1001) users      (100)     2124 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/targets/rejecttarget.py
--rw-r--r--   0 panos     (1001) users      (100)    10896 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/targets/target.py
--rw-r--r--   0 panos     (1001) users      (100)     4873 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/targets/ttltarget.py
--rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    24908 2023-03-01 20:08:53.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/chain.py
--rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/deps.py
--rw-r--r--   0 panos     (1001) users      (100)     1825 2023-02-05 23:48:20.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/exceptions.py
--rw-r--r--   0 panos     (1001) users      (100)     1340 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/extension.py
--rw-r--r--   0 panos     (1001) users      (100)      918 2023-03-05 20:30:07.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/metadata.py
--rw-r--r--   0 panos     (1001) users      (100)     7810 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/parsing.py
--rw-r--r--   0 panos     (1001) users      (100)    16442 2023-03-01 20:08:53.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/rule.py
--rw-r--r--   0 panos     (1001) users      (100)    28867 2023-03-01 20:08:53.000000 linuxnet-iptables-5.0.4/linuxnet/iptables/table.py
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.0.4/linuxnet/__init__.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/linuxnet_iptables.egg-info/
--rw-r--r--   0 panos     (1001) users      (100)     4152 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/linuxnet_iptables.egg-info/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     2481 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/linuxnet_iptables.egg-info/SOURCES.txt
--rw-r--r--   0 panos     (1001) users      (100)        1 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/linuxnet_iptables.egg-info/dependency_links.txt
--rw-r--r--   0 panos     (1001) users      (100)        9 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/linuxnet_iptables.egg-info/top_level.txt
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/tests/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.0.4/tests/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    57076 2023-03-01 20:08:53.000000 linuxnet-iptables-5.0.4/tests/iptables_test.py
--rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-5.0.4/.pylintrc
--rw-r--r--   0 panos     (1001) users      (100)     2522 2023-03-05 20:31:52.000000 linuxnet-iptables-5.0.4/CHANGELOG.md
--rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-5.0.4/LICENSE
--rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/MANIFEST.in
--rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-5.0.4/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     3237 2023-02-06 17:07:04.000000 linuxnet-iptables-5.0.4/README.md
--rw-r--r--   0 panos     (1001) users      (100)     6659 2023-02-20 17:08:37.000000 linuxnet-iptables-5.0.4/setup.py
--rw-r--r--   0 panos     (1001) users      (100)     4152 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)       38 2023-03-05 20:37:11.000000 linuxnet-iptables-5.0.4/setup.cfg
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.703190 linuxnet-iptables-5.2.0/
+-rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-5.2.0/.pylintrc
+-rw-r--r--   0 panos     (1001) users      (100)     2692 2023-06-04 01:14:51.000000 linuxnet-iptables-5.2.0/CHANGELOG.md
+-rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-5.2.0/LICENSE
+-rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/MANIFEST.in
+-rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-5.2.0/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     4132 2023-06-04 01:22:27.703190 linuxnet-iptables-5.2.0/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     3237 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/README.md
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.690189 linuxnet-iptables-5.2.0/docs/
+-rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-5.2.0/docs/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-5.2.0/docs/chain.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-5.2.0/docs/conf.py
+-rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/exception.rst
+-rw-r--r--   0 panos     (1001) users      (100)     8374 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/extensibility.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3319 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/index.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3187 2023-03-01 20:08:53.000000 linuxnet-iptables-5.2.0/docs/iptables_api.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3176 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/match-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-5.2.0/docs/match.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.694189 linuxnet-iptables-5.2.0/docs/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/commentmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)      990 2023-02-05 23:48:23.000000 linuxnet-iptables-5.2.0/docs/matches/connmarkmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1583 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/conntrackmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/icmpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-5.2.0/docs/matches/limitmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1439 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/markmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1965 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/ownermatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-5.2.0/docs/matches/packetmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/packettypematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/statematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1492 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/tcpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/tcpmssmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1521 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/ttlmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/udpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-5.2.0/docs/rule.rst
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-5.2.0/docs/table.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/target-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-5.2.0/docs/target.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.697189 linuxnet-iptables-5.2.0/docs/targets/
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/chaintarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/connmarktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/dnattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/logtarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/marktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/masqueradetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      902 2023-06-04 01:12:58.000000 linuxnet-iptables-5.2.0/docs/targets/notracktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/rejecttarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/snattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      896 2023-06-04 01:12:58.000000 linuxnet-iptables-5.2.0/docs/targets/tracetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/ttltarget.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.697189 linuxnet-iptables-5.2.0/linuxnet/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.2.0/linuxnet/__init__.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.698190 linuxnet-iptables-5.2.0/linuxnet/iptables/
+-rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    24908 2023-03-01 20:08:53.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/chain.py
+-rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/deps.py
+-rw-r--r--   0 panos     (1001) users      (100)     1825 2023-02-05 23:48:20.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/exceptions.py
+-rw-r--r--   0 panos     (1001) users      (100)     1340 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/extension.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.700190 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1295 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     2889 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/commentmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2271 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/connmarkmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     5226 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/conntrackmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     9769 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/icmpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4667 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/limitmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3852 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/markmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)    14678 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/match.py
+-rw-r--r--   0 panos     (1001) users      (100)     7798 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/ownermatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     7343 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/packetmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2844 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/packettypematch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3155 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/statematch.py
+-rw-r--r--   0 panos     (1001) users      (100)    10665 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/tcpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3833 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/tcpmssmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4322 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/ttlmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2724 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/udpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     5060 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/util.py
+-rw-r--r--   0 panos     (1001) users      (100)      918 2023-06-04 01:12:57.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/metadata.py
+-rw-r--r--   0 panos     (1001) users      (100)     7810 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/parsing.py
+-rw-r--r--   0 panos     (1001) users      (100)    16442 2023-03-01 20:08:53.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/rule.py
+-rw-r--r--   0 panos     (1001) users      (100)    29087 2023-06-04 01:12:57.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/table.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.702190 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/
+-rw-r--r--   0 panos     (1001) users      (100)     1165 2023-06-04 01:12:57.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     7386 2023-03-05 20:39:10.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/connmarktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6518 2023-02-08 00:19:00.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/logtarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6551 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/marktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4133 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/masqueradetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     8146 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/nattarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     1414 2023-06-04 01:12:58.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/notracktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     2124 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/rejecttarget.py
+-rw-r--r--   0 panos     (1001) users      (100)    10896 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/target.py
+-rw-r--r--   0 panos     (1001) users      (100)     1396 2023-06-04 01:12:58.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/tracetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4873 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/ttltarget.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.703190 linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/
+-rw-r--r--   0 panos     (1001) users      (100)     4132 2023-06-04 01:22:27.000000 linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     2625 2023-06-04 01:22:27.000000 linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/SOURCES.txt
+-rw-r--r--   0 panos     (1001) users      (100)        1 2023-06-04 01:22:27.000000 linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/dependency_links.txt
+-rw-r--r--   0 panos     (1001) users      (100)        9 2023-06-04 01:22:27.000000 linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/top_level.txt
+-rw-r--r--   0 panos     (1001) users      (100)       38 2023-06-04 01:22:27.703190 linuxnet-iptables-5.2.0/setup.cfg
+-rw-r--r--   0 panos     (1001) users      (100)     6659 2023-02-20 17:08:37.000000 linuxnet-iptables-5.2.0/setup.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.703190 linuxnet-iptables-5.2.0/tests/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.2.0/tests/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    58452 2023-06-04 01:12:57.000000 linuxnet-iptables-5.2.0/tests/iptables_test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `linuxnet-iptables-5.0.4/docs/matches/commentmatch.rst` & `linuxnet-iptables-5.2.0/docs/matches/commentmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/matches/connmarkmatch.rst` & `linuxnet-iptables-5.2.0/docs/matches/connmarkmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/matches/conntrackmatch.rst` & `linuxnet-iptables-5.2.0/docs/matches/conntrackmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/matches/icmpmatch.rst` & `linuxnet-iptables-5.2.0/docs/matches/icmpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/matches/limitmatch.rst` & `linuxnet-iptables-5.2.0/docs/matches/limitmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/matches/markmatch.rst` & `linuxnet-iptables-5.2.0/docs/matches/markmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/matches/ownermatch.rst` & `linuxnet-iptables-5.2.0/docs/matches/ownermatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/matches/packetmatch.rst` & `linuxnet-iptables-5.2.0/docs/matches/packetmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/matches/packettypematch.rst` & `linuxnet-iptables-5.2.0/docs/matches/packettypematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/matches/statematch.rst` & `linuxnet-iptables-5.2.0/docs/matches/statematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/matches/tcpmatch.rst` & `linuxnet-iptables-5.2.0/docs/matches/tcpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/matches/tcpmssmatch.rst` & `linuxnet-iptables-5.2.0/docs/matches/tcpmssmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/matches/ttlmatch.rst` & `linuxnet-iptables-5.2.0/docs/matches/ttlmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/matches/udpmatch.rst` & `linuxnet-iptables-5.2.0/docs/matches/udpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/targets/chaintarget.rst` & `linuxnet-iptables-5.2.0/docs/targets/chaintarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/targets/connmarktarget.rst` & `linuxnet-iptables-5.2.0/docs/targets/connmarktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/targets/dnattarget.rst` & `linuxnet-iptables-5.2.0/docs/targets/dnattarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/targets/logtarget.rst` & `linuxnet-iptables-5.2.0/docs/targets/logtarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/targets/marktarget.rst` & `linuxnet-iptables-5.2.0/docs/targets/marktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/targets/masqueradetarget.rst` & `linuxnet-iptables-5.2.0/docs/targets/masqueradetarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/targets/rejecttarget.rst` & `linuxnet-iptables-5.2.0/docs/targets/rejecttarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/targets/snattarget.rst` & `linuxnet-iptables-5.2.0/docs/targets/snattarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/targets/ttltarget.rst` & `linuxnet-iptables-5.2.0/docs/targets/ttltarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/Makefile` & `linuxnet-iptables-5.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/chain.rst` & `linuxnet-iptables-5.2.0/docs/chain.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/conf.py` & `linuxnet-iptables-5.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/exception.rst` & `linuxnet-iptables-5.2.0/docs/exception.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/extensibility.rst` & `linuxnet-iptables-5.2.0/docs/extensibility.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/index.rst` & `linuxnet-iptables-5.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/iptables_api.rst` & `linuxnet-iptables-5.2.0/docs/iptables_api.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/match-example.py` & `linuxnet-iptables-5.2.0/docs/match-example.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/match.rst` & `linuxnet-iptables-5.2.0/docs/match.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/rule.rst` & `linuxnet-iptables-5.2.0/docs/rule.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/table.rst` & `linuxnet-iptables-5.2.0/docs/table.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/target-example.py` & `linuxnet-iptables-5.2.0/docs/target-example.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/docs/target.rst` & `linuxnet-iptables-5.2.0/docs/target.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/__init__.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/commentmatch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/commentmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/connmarkmatch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/connmarkmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/conntrackmatch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/conntrackmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/icmpmatch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/icmpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/limitmatch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/limitmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/markmatch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/markmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/match.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/match.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/ownermatch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/ownermatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/packetmatch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/packetmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/packettypematch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/packettypematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/statematch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/statematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/tcpmatch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/tcpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/tcpmssmatch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/tcpmssmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/ttlmatch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/ttlmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/udpmatch.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/udpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/matches/util.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/util.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/targets/__init__.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,9 +21,11 @@
 
 from .target import Target, Targets, TargetNone, ChainTarget, UnparsedTarget
 from .connmarktarget import ConnmarkTarget
 from .logtarget import LogTarget
 from .nattarget import SnatTarget, DnatTarget
 from .marktarget import MarkTarget
 from .masqueradetarget import MasqueradeTarget
+from .notracktarget import NoTrackTarget
 from .rejecttarget import RejectTarget
+from .tracetarget import TraceTarget
 from .ttltarget import TtlTarget
```

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/targets/connmarktarget.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/connmarktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/targets/logtarget.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/logtarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/targets/marktarget.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/marktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/targets/masqueradetarget.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/masqueradetarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/targets/nattarget.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/nattarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/targets/rejecttarget.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/rejecttarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/targets/target.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/target.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/targets/ttltarget.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/ttltarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/__init__.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/chain.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/chain.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/deps.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/deps.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/exceptions.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/exceptions.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/extension.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/extension.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/metadata.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 """
 Metadata information intended to be used by setup.py and the
 Sphinx conf.py
 """
 
 # pylint: disable=invalid-name
 
-_version_ = "5.0.4"
+_version_ = "5.2.0"
 _author_ = "Panagiotis (Panos) Tsirigotis"
 _package_ = "linuxnet.iptables"
```

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/parsing.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/parsing.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/rule.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/rule.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/linuxnet/iptables/table.py` & `linuxnet-iptables-5.2.0/linuxnet/iptables/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,21 +74,25 @@
                         'nat' : ('PREROUTING', 'POSTROUTING', 'OUTPUT'),
                         'raw' : ('PREROUTING', 'OUTPUT'),
                         'security' : ('INPUT', 'OUTPUT', 'FORWARD'),
                     }
 
     __CHAIN_NAME_LIMIT = 28
 
-    def __init__(self, table_name: str, chain_prefix: str =None, runner=None):
+    def __init__(self, table_name: str, chain_prefix: Optional[str] =None,
+                        runner=None):
         """
         :param table_name: one of ``filter``, ``mangle``, ``nat``, ``raw``,
             or ``security``
-        :param chain_prefix: if specified, only chains with names starting
-            with this prefix will be included (however, the builtin chains
-            are **always** included)
+        :param chain_prefix: if specified, user chains are split into two
+            groups: those with names starting with the prefix and those
+            that don't) with methods like :meth:`get_user_chains`
+            returning only these user chains;
+            the chain name that excludes the prefix is referred to as
+            the **logical** chain name
         :param runner: optional Callable object used to invoke the
             **iptables(8)** command. The object should have the same signature
             as :func:`subprocess.run` and provide the same functionality.
             It also needs to consume the ``execute_always`` boolean parameter;
             this parameter is used to indicate that the **iptables(8)** command
             should be invoked even if the ``runner`` is in dryrun mode (this
             is used for read-only commands like ``iptables -L``).
@@ -141,15 +145,15 @@
 
     def get_prefix(self) -> Optional[str]:
         """Returns the chain prefix
         """
         return self.__prefix
 
     def set_prefix(self, prefix: Optional[str]) -> None:
-        """Partition (or repartition) the chains according to the
+        """Partition (or repartition) the user chains according to the
         specified prefix.
 
         :param prefix: the new prefix
         """
         chain_map = self.__chain_map.copy()
         chain_map.update(self.__other_chain_map)
         self.__chain_map.clear()
@@ -487,15 +491,15 @@
             chain._clear_pft()          # pylint: disable=protected-access
 
     def init_from_output(self, iptables_output: str,
                         add_builtins=True, log_parsing_failures=True) -> bool:
         """Initialize the attributes of this :class:`IptablesPacketFilterTable`
         from the output of **iptables(8)**
 
-        :param iptables_output: the output of ``iptables -L -xnv` as
+        :param iptables_output: the output of ``iptables -L -xnv`` as
             included in ``subprocess.CompletedProcess.stdout``
         :param add_builtins: if this parameter is ``True`` then for any
             builtin chain that is not in the ``iptables_output`` (or
             if there is an error parsing its contents), an (empty) chain
             will be added to the :class:`IptablesPacketFilterTable`
         :param log_parsing_failures: if this parameter is ``True`` then
             parsing failures will be logged; such failures are typically
```

### Comparing `linuxnet-iptables-5.0.4/linuxnet_iptables.egg-info/PKG-INFO` & `linuxnet-iptables-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 5.0.4
+Version: 5.2.0
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Networking :: Firewalls
@@ -138,9 +137,7 @@
 
 Available `Makefile` targets can be listed by invoking `make` with no arguments.
 
 `make install` will install the package.
 
 `make test` runs the unit tests.
 
-
-
```

### Comparing `linuxnet-iptables-5.0.4/linuxnet_iptables.egg-info/SOURCES.txt` & `linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -34,16 +34,18 @@
 docs/matches/udpmatch.rst
 docs/targets/chaintarget.rst
 docs/targets/connmarktarget.rst
 docs/targets/dnattarget.rst
 docs/targets/logtarget.rst
 docs/targets/marktarget.rst
 docs/targets/masqueradetarget.rst
+docs/targets/notracktarget.rst
 docs/targets/rejecttarget.rst
 docs/targets/snattarget.rst
+docs/targets/tracetarget.rst
 docs/targets/ttltarget.rst
 linuxnet/__init__.py
 linuxnet/iptables/__init__.py
 linuxnet/iptables/chain.py
 linuxnet/iptables/deps.py
 linuxnet/iptables/exceptions.py
 linuxnet/iptables/extension.py
@@ -70,16 +72,18 @@
 linuxnet/iptables/matches/util.py
 linuxnet/iptables/targets/__init__.py
 linuxnet/iptables/targets/connmarktarget.py
 linuxnet/iptables/targets/logtarget.py
 linuxnet/iptables/targets/marktarget.py
 linuxnet/iptables/targets/masqueradetarget.py
 linuxnet/iptables/targets/nattarget.py
+linuxnet/iptables/targets/notracktarget.py
 linuxnet/iptables/targets/rejecttarget.py
 linuxnet/iptables/targets/target.py
+linuxnet/iptables/targets/tracetarget.py
 linuxnet/iptables/targets/ttltarget.py
 linuxnet_iptables.egg-info/PKG-INFO
 linuxnet_iptables.egg-info/SOURCES.txt
 linuxnet_iptables.egg-info/dependency_links.txt
 linuxnet_iptables.egg-info/top_level.txt
 tests/__init__.py
 tests/iptables_test.py
```

### Comparing `linuxnet-iptables-5.0.4/tests/iptables_test.py` & `linuxnet-iptables-5.2.0/tests/iptables_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,17 @@
                 IptablesError,
                 ChainRule,
                 # Targets
                 ChainTarget, Targets,
                 MarkTarget, ConnmarkTarget,
                 RejectTarget,
                 MasqueradeTarget,
+                NoTrackTarget,
                 TtlTarget,
+                TraceTarget,
                 # Matches
                 CommentMatch,
                 TcpmssMatch, TcpMatch,
                 UdpMatch, IcmpMatch,
                 PacketTypeMatch,
                 ConnmarkMatch,
                 LimitMatch,
@@ -70,17 +72,14 @@
     """
     def __init__(self, exitcode, output):
         self.__output = output
         self.__exitcode = exitcode
         # A run is a list of ExecutedCommand instances
         self.__run = []
 
-    def get_cmd(self):
-        return self.__cmd
-
     def get_run(self):
         return self.__run
 
     def clear_run(self):
         self.__run.clear()
 
     def __call__(self, cmd, *args, **kwargs):
@@ -776,14 +775,44 @@
                             target.get_ports() == (2000, None) and
                                 target.uses_random_port_mapping())
         rule = postrouting_chain.get_rules()[4]
         target = rule.get_target()
         self.assertTrue(isinstance(target, MasqueradeTarget) and
                                 target.get_ports() == (20000, 30000))
 
+    def test_parsing_notrack_target(self):
+        """Parse output with NOTRACK target
+        """
+        output = (self.EMPTY_PREROUTING + '\n' + """\
+Chain OUTPUT (policy ACCEPT 12 packets, 1845 bytes)
+ pkts bytes target     prot opt in     out     source               destination
+    0     0 NOTRACK    tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           tcp dpt:55555
+""")
+        pft = IptablesPacketFilterTable('raw')
+        self.assertTrue(pft.init_from_output(output))
+        output_chain = pft.get_builtin_chain('OUTPUT')
+        rule = output_chain.get_rules()[0]
+        target = rule.get_target()
+        self.assertTrue(isinstance(target, NoTrackTarget))
+
+    def test_parsing_trace_target(self):
+        """Parse output with TRACE target
+        """
+        output = (self.EMPTY_PREROUTING + '\n' + """\
+Chain OUTPUT (policy ACCEPT 12 packets, 1845 bytes)
+ pkts bytes target     prot opt in     out     source               destination
+    0     0 TRACE      tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           tcp dpt:55555
+""")
+        pft = IptablesPacketFilterTable('raw')
+        self.assertTrue(pft.init_from_output(output))
+        output_chain = pft.get_builtin_chain('OUTPUT')
+        rule = output_chain.get_rules()[0]
+        target = rule.get_target()
+        self.assertTrue(isinstance(target, TraceTarget))
+
     def test_parsing_unknown_target(self):
         """Parse output with unknown target
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
 196245663 314408786102 prod_INPUT  all  --  *      *       0.0.0.0/0            0.0.0.0/0
```

### Comparing `linuxnet-iptables-5.0.4/.pylintrc` & `linuxnet-iptables-5.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/CHANGELOG.md` & `linuxnet-iptables-5.2.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Change Log
 ==========
 
+5.2.0 (2023-06-03)
+------------------
+
+- added NoTrackTarget class to support the iptables NOTRACK target
+- added TraceTarget class to support the iptables TRACE target
+
 5.0.4 (2023-03-05)
 ------------------
 
 - bugfixes in ConnmarkTarget class
 
 5.0.2 (2023-03-01)
 ------------------
```

### Comparing `linuxnet-iptables-5.0.4/LICENSE` & `linuxnet-iptables-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/Makefile` & `linuxnet-iptables-5.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/README.md` & `linuxnet-iptables-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/setup.py` & `linuxnet-iptables-5.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.0.4/PKG-INFO` & `linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 5.0.4
+Version: 5.2.0
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Networking :: Firewalls
@@ -138,9 +137,7 @@
 
 Available `Makefile` targets can be listed by invoking `make` with no arguments.
 
 `make install` will install the package.
 
 `make test` runs the unit tests.
 
-
-
```

