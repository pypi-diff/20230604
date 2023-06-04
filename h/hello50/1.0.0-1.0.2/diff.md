# Comparing `tmp/hello50-1.0.0.tar.gz` & `tmp/hello50-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello50-1.0.0.tar", last modified: Sun Jun  4 21:31:40 2023, max compression
+gzip compressed data, was "hello50-1.0.2.tar", last modified: Sun Jun  4 21:42:56 2023, max compression
```

## Comparing `hello50-1.0.0.tar` & `hello50-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 21:31:40.935220 hello50-1.0.0/
--rw-rw-rw-   0        0        0      511 2023-06-04 21:31:40.935220 hello50-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-06-04 21:31:36.000000 hello50-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 21:31:40.913213 hello50-1.0.0/hello/
--rw-rw-rw-   0        0        0       24 2023-06-04 21:28:51.000000 hello50-1.0.0/hello/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-04 21:28:42.000000 hello50-1.0.0/hello/hello.py
-drwxrwxrwx   0        0        0        0 2023-06-04 21:31:40.933217 hello50-1.0.0/hello50.egg-info/
--rw-rw-rw-   0        0        0      511 2023-06-04 21:31:40.000000 hello50-1.0.0/hello50.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-06-04 21:31:40.000000 hello50-1.0.0/hello50.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 21:31:40.000000 hello50-1.0.0/hello50.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-04 21:31:40.000000 hello50-1.0.0/hello50.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-04 21:31:40.000000 hello50-1.0.0/hello50.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 21:31:40.935220 hello50-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-06-04 21:27:56.000000 hello50-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:42:56.400070 hello50-1.0.2/
+-rw-rw-rw-   0        0        0      514 2023-06-04 21:42:56.396071 hello50-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-06-04 21:31:36.000000 hello50-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 21:42:56.255256 hello50-1.0.2/hello/
+-rw-rw-rw-   0        0        0       43 2023-06-04 21:37:05.000000 hello50-1.0.2/hello/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-04 21:28:42.000000 hello50-1.0.2/hello/index.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:42:56.390034 hello50-1.0.2/hello50.egg-info/
+-rw-rw-rw-   0        0        0      514 2023-06-04 21:42:55.000000 hello50-1.0.2/hello50.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-06-04 21:42:56.000000 hello50-1.0.2/hello50.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 21:42:55.000000 hello50-1.0.2/hello50.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-04 21:42:55.000000 hello50-1.0.2/hello50.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-04 21:42:55.000000 hello50-1.0.2/hello50.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 21:42:56.400070 hello50-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1006 2023-06-04 21:41:48.000000 hello50-1.0.2/setup.py
```

### Comparing `hello50-1.0.0/setup.py` & `hello50-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.2'
 DESCRIPTION = 'Hello world shit!!!!'
-LONG_DESCRIPTION = 'Hello world ~~~~~'
+LONG_DESCRIPTION = 'Hello world 000~~~~~'
 
 # Setting up
 setup(
     name="hello50",
     version=VERSION,
     author="Malik",
     author_email="myemail46926213@gmail.com",
```

