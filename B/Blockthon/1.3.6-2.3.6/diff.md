# Comparing `tmp/Blockthon-1.3.6.tar.gz` & `tmp/Blockthon-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Blockthon-1.3.6.tar", last modified: Mon May 29 03:15:43 2023, max compression
+gzip compressed data, was "Blockthon-2.3.6.tar", last modified: Sun Jun  4 02:17:40 2023, max compression
```

## Comparing `Blockthon-1.3.6.tar` & `Blockthon-2.3.6.tar`

### file list

```diff
@@ -1,12 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 03:15:43.691475 Blockthon-1.3.6/
-drwxrwxrwx   0        0        0        0 2023-05-29 03:15:43.690544 Blockthon-1.3.6/Blockthon.egg-info/
--rw-rw-rw-   0        0        0    11623 2023-05-29 03:15:43.000000 Blockthon-1.3.6/Blockthon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-05-29 03:15:43.000000 Blockthon-1.3.6/Blockthon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 03:15:43.000000 Blockthon-1.3.6/Blockthon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      166 2023-05-29 03:15:43.000000 Blockthon-1.3.6/Blockthon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 03:15:43.000000 Blockthon-1.3.6/Blockthon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-05-29 01:42:28.000000 Blockthon-1.3.6/LICENSE
--rw-rw-rw-   0        0        0    11623 2023-05-29 03:15:43.690544 Blockthon-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0    10764 2023-05-29 01:42:28.000000 Blockthon-1.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 03:15:43.691475 Blockthon-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1434 2023-05-29 03:14:02.000000 Blockthon-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:17:40.261268 Blockthon-2.3.6/
+drwxrwxrwx   0        0        0        0 2023-06-04 02:17:40.245613 Blockthon-2.3.6/Blockthon/
+-rw-rw-rw-   0        0        0     2160 2023-06-02 20:46:04.000000 Blockthon-2.3.6/Blockthon/Base58.py
+-rw-rw-rw-   0        0        0     3088 2023-06-03 19:21:06.000000 Blockthon-2.3.6/Blockthon/Bitcoin.py
+-rw-rw-rw-   0        0        0     1159 2023-06-03 18:38:02.000000 Blockthon-2.3.6/Blockthon/BitcoinGold.py
+-rw-rw-rw-   0        0        0     1041 2023-06-03 18:38:02.000000 Blockthon-2.3.6/Blockthon/Dash.py
+-rw-rw-rw-   0        0        0     1032 2023-06-03 18:38:02.000000 Blockthon-2.3.6/Blockthon/DigiByte.py
+-rw-rw-rw-   0        0        0      497 2023-06-03 12:50:01.000000 Blockthon-2.3.6/Blockthon/Dogecoin.py
+-rw-rw-rw-   0        0        0      492 2023-06-02 23:40:53.000000 Blockthon-2.3.6/Blockthon/Ethereum.py
+-rw-rw-rw-   0        0        0     1407 2023-06-03 13:19:05.000000 Blockthon-2.3.6/Blockthon/Litecoin.py
+-rw-rw-rw-   0        0        0      859 2023-06-04 00:55:43.000000 Blockthon-2.3.6/Blockthon/Qtum.py
+-rw-rw-rw-   0        0        0      847 2023-06-04 00:59:12.000000 Blockthon-2.3.6/Blockthon/Ravencoin.py
+-rw-rw-rw-   0        0        0      495 2023-06-02 23:40:53.000000 Blockthon-2.3.6/Blockthon/Tron.py
+-rw-rw-rw-   0        0        0    24350 2023-06-04 00:55:43.000000 Blockthon-2.3.6/Blockthon/Utils.py
+-rw-rw-rw-   0        0        0     1484 2023-06-04 01:02:25.000000 Blockthon-2.3.6/Blockthon/Wallet.py
+-rw-rw-rw-   0        0        0      588 2023-06-04 01:02:25.000000 Blockthon-2.3.6/Blockthon/__init__.py
+-rw-rw-rw-   0        0        0      822 2023-06-04 00:29:18.000000 Blockthon-2.3.6/Blockthon/zCash.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:17:40.261268 Blockthon-2.3.6/Blockthon.egg-info/
+-rw-rw-rw-   0        0        0     3514 2023-06-04 02:17:40.000000 Blockthon-2.3.6/Blockthon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2023-06-04 02:17:40.000000 Blockthon-2.3.6/Blockthon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 02:17:40.000000 Blockthon-2.3.6/Blockthon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      166 2023-06-04 02:17:40.000000 Blockthon-2.3.6/Blockthon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 02:17:40.000000 Blockthon-2.3.6/Blockthon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3514 2023-06-04 02:17:40.261268 Blockthon-2.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2674 2023-06-04 01:48:32.000000 Blockthon-2.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-04 02:17:40.261268 Blockthon-2.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1477 2023-06-04 02:00:50.000000 Blockthon-2.3.6/setup.py
```

