# Comparing `tmp/BatchParse-0.0.5.tar.gz` & `tmp/BatchParse-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BatchParse-0.0.5.tar", last modified: Sat Jun  3 02:43:10 2023, max compression
+gzip compressed data, was "BatchParse-0.0.6.tar", last modified: Sun Jun  4 02:30:16 2023, max compression
```

## Comparing `BatchParse-0.0.5.tar` & `BatchParse-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:43:10.360257 BatchParse-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:43:10.356257 BatchParse-0.0.5/BatchParse/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-03 02:42:55.000000 BatchParse-0.0.5/BatchParse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-03 02:42:55.000000 BatchParse-0.0.5/BatchParse/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:43:10.356257 BatchParse-0.0.5/BatchParse/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:42:55.000000 BatchParse-0.0.5/BatchParse/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-03 02:42:55.000000 BatchParse-0.0.5/BatchParse/util/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-03 02:42:55.000000 BatchParse-0.0.5/BatchParse/util/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-03 02:42:55.000000 BatchParse-0.0.5/BatchParse/util/splitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:43:10.356257 BatchParse-0.0.5/BatchParse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-03 02:43:10.000000 BatchParse-0.0.5/BatchParse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-03 02:43:10.000000 BatchParse-0.0.5/BatchParse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 02:43:10.000000 BatchParse-0.0.5/BatchParse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 02:43:10.000000 BatchParse-0.0.5/BatchParse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 02:43:10.000000 BatchParse-0.0.5/BatchParse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-03 02:42:55.000000 BatchParse-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-03 02:43:10.360257 BatchParse-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 02:42:55.000000 BatchParse-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 02:43:10.360257 BatchParse-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-03 02:42:55.000000 BatchParse-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:43:10.356257 BatchParse-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-03 02:42:55.000000 BatchParse-0.0.5/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:30:16.339444 BatchParse-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:30:16.339444 BatchParse-0.0.6/BatchParse/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-04 02:30:06.000000 BatchParse-0.0.6/BatchParse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-04 02:30:06.000000 BatchParse-0.0.6/BatchParse/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:30:16.339444 BatchParse-0.0.6/BatchParse/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 02:30:06.000000 BatchParse-0.0.6/BatchParse/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-04 02:30:06.000000 BatchParse-0.0.6/BatchParse/util/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-04 02:30:06.000000 BatchParse-0.0.6/BatchParse/util/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-04 02:30:06.000000 BatchParse-0.0.6/BatchParse/util/splitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:30:16.339444 BatchParse-0.0.6/BatchParse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-04 02:30:16.000000 BatchParse-0.0.6/BatchParse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-04 02:30:16.000000 BatchParse-0.0.6/BatchParse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 02:30:16.000000 BatchParse-0.0.6/BatchParse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 02:30:16.000000 BatchParse-0.0.6/BatchParse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 02:30:16.000000 BatchParse-0.0.6/BatchParse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-04 02:30:06.000000 BatchParse-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-04 02:30:16.339444 BatchParse-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 02:30:06.000000 BatchParse-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 02:30:16.339444 BatchParse-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-04 02:30:06.000000 BatchParse-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:30:16.339444 BatchParse-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-04 02:30:06.000000 BatchParse-0.0.6/test/test.py
```

### Comparing `BatchParse-0.0.5/BatchParse/main.py` & `BatchParse-0.0.6/BatchParse/main.py`

 * *Files identical despite different names*

### Comparing `BatchParse-0.0.5/BatchParse/util/info.py` & `BatchParse-0.0.6/BatchParse/util/info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import re
+
+
 def get_method(line: str) -> str:
     """Get's the Method from a line of Batch Code
 
     Args:
         line (str): Line of Batch Code
 
     Returns:
@@ -41,14 +44,17 @@
         "length": __get_length(code),
         "valid_command_length": valid_length(__get_length(code)),
         "echo_to_file": echo_to_file(code),
         "get_from_file": get_from_file(code),
         "raw": code,
     }
 
+    if info["method"] == "for":
+        info["for_args"] = get_info_for(code)
+
     return info
 
 
 def __get_length(code: str) -> int:
     """Get's the length of the code
 
     Args:
@@ -84,7 +90,23 @@
 
 def get_from_file(code: str) -> bool:
     possible_methods = ["<"]
     unallowed_methods = ["^<"]
     return any([method in code for method in possible_methods]) and not any(
         [method in code for method in unallowed_methods]
     )
+
+
+def get_info_for(code: str) -> list:
+    args_total = {}
+    insides_regex = re.compile(r"\(.*\)")
+    first_arg = code.split(" ")[1]
+    if first_arg.startswith("/"):
+        args_total["flags"] = first_arg
+        args_total["variable"] = code.split(" ")[2]
+        args_total["insides"] = insides_regex.findall(code)[0]
+        args_total["afterwards"] = code.split("do")[1].strip().replace("\n", "")
+    else:
+        args_total["variable"] = first_arg
+        args_total["insides"] = insides_regex.findall(code)[0]
+        args_total["afterwards"] = code.split("do")[1].strip().replace("\n", "")
+    return args_total
```

### Comparing `BatchParse-0.0.5/BatchParse/util/splitting.py` & `BatchParse-0.0.6/BatchParse/util/splitting.py`

 * *Files identical despite different names*

### Comparing `BatchParse-0.0.5/LICENSE` & `BatchParse-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `BatchParse-0.0.5/setup.py` & `BatchParse-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 DESCRIPTION = "A Batch Parser"
 LONG_DESCRIPTION = "Easy Way to Parse Batch Code in Python"
 
 setup(
     name="BatchParse",
     version=VERSION,
     description=DESCRIPTION,
```

