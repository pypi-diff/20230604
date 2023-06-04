# Comparing `tmp/rlenvironments-0.1.0.tar.gz` & `tmp/rlenvironments-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlenvironments-0.1.0.tar", last modified: Sun Jun  4 21:07:59 2023, max compression
+gzip compressed data, was "rlenvironments-0.1.1.tar", last modified: Sun Jun  4 21:26:30 2023, max compression
```

## Comparing `rlenvironments-0.1.0.tar` & `rlenvironments-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 21:07:59.853211 rlenvironments-0.1.0/
--rw-rw-rw-   0        0        0     1638 2023-06-04 21:07:59.853211 rlenvironments-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      938 2023-06-04 19:57:06.000000 rlenvironments-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 21:07:59.853211 rlenvironments-0.1.0/rlenvironments.egg-info/
--rw-rw-rw-   0        0        0     1638 2023-06-04 21:07:59.000000 rlenvironments-0.1.0/rlenvironments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-06-04 21:07:59.000000 rlenvironments-0.1.0/rlenvironments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 21:07:59.000000 rlenvironments-0.1.0/rlenvironments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-04 21:07:59.000000 rlenvironments-0.1.0/rlenvironments.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 21:07:59.000000 rlenvironments-0.1.0/rlenvironments.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 21:07:59.853211 rlenvironments-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1021 2023-06-04 19:40:38.000000 rlenvironments-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:26:30.686382 rlenvironments-0.1.1/
+-rw-rw-rw-   0        0        0     1638 2023-06-04 21:26:30.686382 rlenvironments-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      938 2023-06-04 19:57:06.000000 rlenvironments-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 21:26:30.670757 rlenvironments-0.1.1/rlenvironments.egg-info/
+-rw-rw-rw-   0        0        0     1638 2023-06-04 21:26:30.000000 rlenvironments-0.1.1/rlenvironments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-06-04 21:26:30.000000 rlenvironments-0.1.1/rlenvironments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 21:26:30.000000 rlenvironments-0.1.1/rlenvironments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-04 21:26:30.000000 rlenvironments-0.1.1/rlenvironments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 21:26:30.000000 rlenvironments-0.1.1/rlenvironments.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 21:26:30.686382 rlenvironments-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1021 2023-06-04 21:26:11.000000 rlenvironments-0.1.1/setup.py
```

### Comparing `rlenvironments-0.1.0/PKG-INFO` & `rlenvironments-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlenvironments
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for target seeking environment
 Home-page: https://github.com/ukoksoy/rlenvironments
 Author: Umut Koksoy
 Author-email: umutkoksoy@gmail.com
 Keywords: reinforcement-learning environment target-seeking
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rlenvironments-0.1.0/README.md` & `rlenvironments-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rlenvironments-0.1.0/rlenvironments.egg-info/PKG-INFO` & `rlenvironments-0.1.1/rlenvironments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlenvironments
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for target seeking environment
 Home-page: https://github.com/ukoksoy/rlenvironments
 Author: Umut Koksoy
 Author-email: umutkoksoy@gmail.com
 Keywords: reinforcement-learning environment target-seeking
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rlenvironments-0.1.0/setup.py` & `rlenvironments-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rlenvironments",
-    version="0.1.0",
+    version="0.1.1",
     author="Umut Koksoy",
     author_email="umutkoksoy@gmail.com",
     description="Python library for target seeking environment",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ukoksoy/rlenvironments",
     packages=setuptools.find_packages(),
```

