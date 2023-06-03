# Comparing `tmp/puup-0.1.0.tar.gz` & `tmp/puup-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puup-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "puup-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `puup-0.1.0.tar` & `puup-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1080 2023-05-29 19:05:25.685534 puup-0.1.0/LICENSE
--rw-r--r--   0        0        0      227 2023-06-02 22:30:24.205224 puup-0.1.0/README.md
--rw-r--r--   0        0        0      403 2023-06-02 22:31:57.721312 puup-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      184 2023-06-02 22:34:53.426894 puup-0.1.0/src/puup/__init__.py
--rw-r--r--   0        0        0     1275 2023-06-02 21:41:12.346848 puup-0.1.0/src/puup/cli.py
--rw-r--r--   0        0        0      187 2023-05-31 19:12:04.837811 puup-0.1.0/src/puup/data/Makefile
--rw-r--r--   0        0        0        0 2023-06-02 08:25:43.687585 puup-0.1.0/src/puup/data/__init__.py
--rw-r--r--   0        0        0   257173 2023-06-02 08:31:24.997921 puup-0.1.0/src/puup/data/a.py
--rw-r--r--   0        0        0   601317 2023-06-02 08:31:29.901217 puup-0.1.0/src/puup/data/n.py
--rw-r--r--   0        0        0     5368 2023-06-02 08:30:42.648243 puup-0.1.0/src/puup/data/p.py
--rw-r--r--   0        0        0    57120 2023-06-02 08:31:32.217866 puup-0.1.0/src/puup/data/r.py
--rw-r--r--   0        0        0   173243 2023-06-02 08:31:35.161176 puup-0.1.0/src/puup/data/s.py
--rw-r--r--   0        0        0   108989 2023-06-02 08:31:37.804489 puup-0.1.0/src/puup/data/v.py
--rw-r--r--   0        0        0      845 2023-06-02 22:37:23.582636 puup-0.1.0/src/puup/data/wn.py
--rw-r--r--   0        0        0      987 2023-06-02 22:37:13.339366 puup-0.1.0/src/puup/data/wp.py
--rw-r--r--   0        0        0      425 2023-06-01 22:14:38.850310 puup-0.1.0/src/puup/dump.py
--rw-r--r--   0        0        0      461 2023-06-02 22:38:39.008838 puup-0.1.0/src/puup/entropy.py
--rw-r--r--   0        0        0      291 2023-06-01 22:49:26.144230 puup-0.1.0/src/puup/lazy.py
--rw-r--r--   0        0        0      362 2023-06-02 19:59:50.317512 puup-0.1.0/src/puup/render.py
--rw-r--r--   0        0        0      780 2023-06-02 19:46:21.419645 puup-0.1.0/src/puup/template.py
--rw-r--r--   0        0        0      433 2023-06-02 22:39:37.928475 puup-0.1.0/src/puup/words.py
--rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 puup-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-29 19:05:25.685534 puup-0.1.1/LICENSE
+-rw-r--r--   0        0        0      716 2023-06-03 22:16:42.735457 puup-0.1.1/README.md
+-rw-r--r--   0        0        0      403 2023-06-02 22:31:57.721312 puup-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-06-03 22:26:49.533052 puup-0.1.1/src/puup/__init__.py
+-rw-r--r--   0        0        0     1276 2023-06-03 15:30:07.918602 puup-0.1.1/src/puup/cli.py
+-rw-r--r--   0        0        0      189 2023-06-03 22:13:16.094081 puup-0.1.1/src/puup/data/Makefile
+-rw-r--r--   0        0        0        0 2023-06-02 08:25:43.687585 puup-0.1.1/src/puup/data/__init__.py
+-rw-r--r--   0        0        0   257173 2023-06-02 08:31:24.997921 puup-0.1.1/src/puup/data/a.py
+-rw-r--r--   0        0        0   601317 2023-06-02 08:31:29.901217 puup-0.1.1/src/puup/data/n.py
+-rw-r--r--   0        0        0     5368 2023-06-02 08:30:42.648243 puup-0.1.1/src/puup/data/p.py
+-rw-r--r--   0        0        0    57120 2023-06-02 08:31:32.217866 puup-0.1.1/src/puup/data/r.py
+-rw-r--r--   0        0        0   173243 2023-06-02 08:31:35.161176 puup-0.1.1/src/puup/data/s.py
+-rw-r--r--   0        0        0   108989 2023-06-02 08:31:37.804489 puup-0.1.1/src/puup/data/v.py
+-rw-r--r--   0        0        0      845 2023-06-02 22:37:23.582636 puup-0.1.1/src/puup/data/wn.py
+-rw-r--r--   0        0        0      987 2023-06-02 22:37:13.339366 puup-0.1.1/src/puup/data/wp.py
+-rw-r--r--   0        0        0      482 2023-06-03 22:22:03.095753 puup-0.1.1/src/puup/dump.py
+-rw-r--r--   0        0        0      460 2023-06-03 22:19:53.500315 puup-0.1.1/src/puup/entropy.py
+-rw-r--r--   0        0        0      291 2023-06-01 22:49:26.144230 puup-0.1.1/src/puup/lazy.py
+-rw-r--r--   0        0        0      362 2023-06-02 19:59:50.317512 puup-0.1.1/src/puup/render.py
+-rw-r--r--   0        0        0      780 2023-06-02 19:46:21.419645 puup-0.1.1/src/puup/template.py
+-rw-r--r--   0        0        0      433 2023-06-02 22:39:37.928475 puup-0.1.1/src/puup/words.py
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 puup-0.1.1/PKG-INFO
```

### Comparing `puup-0.1.0/LICENSE` & `puup-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `puup-0.1.0/src/puup/cli.py` & `puup-0.1.1/src/puup/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
+import sys
+
 import click
 import confuse
-import sys
 
 from puup.render import render
 from puup.dump import dump
 import puup.entropy
 
 
 @click.command()
```

### Comparing `puup-0.1.0/src/puup/data/a.py` & `puup-0.1.1/src/puup/data/a.py`

 * *Files identical despite different names*

### Comparing `puup-0.1.0/src/puup/data/n.py` & `puup-0.1.1/src/puup/data/n.py`

 * *Files identical despite different names*

### Comparing `puup-0.1.0/src/puup/data/p.py` & `puup-0.1.1/src/puup/data/p.py`

 * *Files identical despite different names*

### Comparing `puup-0.1.0/src/puup/data/r.py` & `puup-0.1.1/src/puup/data/r.py`

 * *Files identical despite different names*

### Comparing `puup-0.1.0/src/puup/data/s.py` & `puup-0.1.1/src/puup/data/s.py`

 * *Files identical despite different names*

### Comparing `puup-0.1.0/src/puup/data/v.py` & `puup-0.1.1/src/puup/data/v.py`

 * *Files identical despite different names*

### Comparing `puup-0.1.0/src/puup/data/wn.py` & `puup-0.1.1/src/puup/data/wn.py`

 * *Files identical despite different names*

### Comparing `puup-0.1.0/src/puup/data/wp.py` & `puup-0.1.1/src/puup/data/wp.py`

 * *Files identical despite different names*

### Comparing `puup-0.1.0/src/puup/template.py` & `puup-0.1.1/src/puup/template.py`

 * *Files identical despite different names*

