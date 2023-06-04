# Comparing `tmp/xspf_fixup-0.9.tar.gz` & `tmp/xspf_fixup-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspf_fixup-0.9.tar", last modified: Wed May 24 22:01:26 2023, max compression
+gzip compressed data, was "xspf_fixup-0.9.1.tar", last modified: Sun Jun  4 00:44:31 2023, max compression
```

## Comparing `xspf_fixup-0.9.tar` & `xspf_fixup-0.9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:01:26.808773 xspf_fixup-0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 22:01:16.000000 xspf_fixup-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-24 22:01:26.808773 xspf_fixup-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-24 22:01:16.000000 xspf_fixup-0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 22:01:26.808773 xspf_fixup-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-24 22:01:16.000000 xspf_fixup-0.9/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-05-24 22:01:16.000000 xspf_fixup-0.9/xspf_fixup
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:01:26.808773 xspf_fixup-0.9/xspf_fixup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-24 22:01:26.000000 xspf_fixup-0.9/xspf_fixup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-24 22:01:26.000000 xspf_fixup-0.9/xspf_fixup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:01:26.000000 xspf_fixup-0.9/xspf_fixup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-24 22:01:26.000000 xspf_fixup-0.9/xspf_fixup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:01:26.000000 xspf_fixup-0.9/xspf_fixup.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     7342 2023-05-24 22:01:16.000000 xspf_fixup-0.9/xspf_fixup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:44:31.494854 xspf_fixup-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-04 00:44:15.000000 xspf_fixup-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-04 00:44:31.494854 xspf_fixup-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-04 00:44:15.000000 xspf_fixup-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 00:44:31.494854 xspf_fixup-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-04 00:44:15.000000 xspf_fixup-0.9.1/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-06-04 00:44:15.000000 xspf_fixup-0.9.1/xspf_fixup
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:44:31.494854 xspf_fixup-0.9.1/xspf_fixup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-04 00:44:31.000000 xspf_fixup-0.9.1/xspf_fixup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-04 00:44:31.000000 xspf_fixup-0.9.1/xspf_fixup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 00:44:31.000000 xspf_fixup-0.9.1/xspf_fixup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-04 00:44:31.000000 xspf_fixup-0.9.1/xspf_fixup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 00:44:31.000000 xspf_fixup-0.9.1/xspf_fixup.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7536 2023-06-04 00:44:15.000000 xspf_fixup-0.9.1/xspf_fixup.py
```

### Comparing `xspf_fixup-0.9/LICENSE` & `xspf_fixup-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xspf_fixup-0.9/PKG-INFO` & `xspf_fixup-0.9.1/xspf_fixup.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xspf_fixup
-Version: 0.9
+Name: xspf-fixup
+Version: 0.9.1
 Summary: A simple command line program to fix playlist (.xspf files) with broken links.
 Author: Juan S. Bokser
 Author-email: juan.bokser@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `xspf_fixup-0.9/README.md` & `xspf_fixup-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `xspf_fixup-0.9/setup.py` & `xspf_fixup-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `xspf_fixup-0.9/xspf_fixup.egg-info/PKG-INFO` & `xspf_fixup-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xspf-fixup
-Version: 0.9
+Name: xspf_fixup
+Version: 0.9.1
 Summary: A simple command line program to fix playlist (.xspf files) with broken links.
 Author: Juan S. Bokser
 Author-email: juan.bokser@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `xspf_fixup-0.9/xspf_fixup.py` & `xspf_fixup-0.9.1/xspf_fixup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 from os import chdir
 from tabulate import tabulate
 from datetime import timedelta
 from contextlib import contextmanager
 
 
-version='0.9'
+version='0.9.1'
 
 
 
 @contextmanager
 def working_directory(path):
     """Changes working directory and returns to previous on exit."""
     prev_cwd = Path.cwd()
@@ -204,15 +204,19 @@
         out.append(f"Total duration: ... {cls.timedelta_to_string(total_duration)}")
         out.append("")
 
         return '\n'.join(out)
 
 
     def __str__(self):
-        return self.soup.prettify()
+        out = self.soup.prettify()
+        # FIXME! I need to find a better prettify() 
+        out = out.replace("<location>\n    ", "<location>")
+        out = out.replace("\n   </location>", "</location>")
+        return out
 
 
     def dump_to_file(self, filename=None):
         if filename is None:
             filename = self.filename
         with open(filename, "w") as file:
             print(self, file=file)
```

