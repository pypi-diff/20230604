# Comparing `tmp/abmatrix-0.2.1.tar.gz` & `tmp/abmatrix-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abmatrix-0.2.1.tar", last modified: Sun Jun  4 15:59:15 2023, max compression
+gzip compressed data, was "abmatrix-0.3.0.tar", last modified: Sun Jun  4 19:02:00 2023, max compression
```

## Comparing `abmatrix-0.2.1.tar` & `abmatrix-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:59:15.048549 abmatrix-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-04 15:59:15.048549 abmatrix-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-04 15:59:05.000000 abmatrix-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:59:15.048549 abmatrix-0.2.1/abmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 15:59:05.000000 abmatrix-0.2.1/abmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-04 15:59:05.000000 abmatrix-0.2.1/abmatrix/abmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:59:15.048549 abmatrix-0.2.1/abmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-04 15:59:15.000000 abmatrix-0.2.1/abmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-04 15:59:15.000000 abmatrix-0.2.1/abmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 15:59:15.000000 abmatrix-0.2.1/abmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 15:59:15.000000 abmatrix-0.2.1/abmatrix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 15:59:05.000000 abmatrix-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-04 15:59:15.048549 abmatrix-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:02:00.836068 abmatrix-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-04 19:02:00.836068 abmatrix-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-04 19:01:51.000000 abmatrix-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:02:00.832068 abmatrix-0.3.0/abmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 19:01:51.000000 abmatrix-0.3.0/abmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-04 19:01:51.000000 abmatrix-0.3.0/abmatrix/abmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:02:00.832068 abmatrix-0.3.0/abmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-04 19:02:00.000000 abmatrix-0.3.0/abmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-04 19:02:00.000000 abmatrix-0.3.0/abmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 19:02:00.000000 abmatrix-0.3.0/abmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 19:02:00.000000 abmatrix-0.3.0/abmatrix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 19:01:51.000000 abmatrix-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-04 19:02:00.836068 abmatrix-0.3.0/setup.cfg
```

### Comparing `abmatrix-0.2.1/abmatrix/abmatrix.py` & `abmatrix-0.3.0/abmatrix/abmatrix.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     def __init__(self):
         self.filename = ""
         self.iszip = False
         self.header = {}
         self.index = {}
         self.sample_index = {}
 
-    def open(self, filename):
+    def read(self, filename):
         if os.path.isfile(filename):
             self.filename = filename
             if zipfile.is_zipfile(filename):
                 self.iszip = True
                 zipstream = zipfile.ZipFile(filename, "r")
                 self.fstream = zipstream.open("-", "r")
             else:
@@ -58,15 +58,31 @@
                 else:
                     locus_id = line.rstrip("\n").split("\t")[0]
                     self.index[locus_id] = offset
                 offset += len(line)
         else:
             raise FileNotFoundError
 
-    def reduce(self, locus_list, **kwargs):
+    def write(self, filename, locus_list):
+        with open(filename, "w") as f:
+            f.write("[Header]\n")
+            for key, value in self.header.items():
+                f.write("{}\t{}\n".format(key, value))
+            f.write("[Data]\n")
+            sorted_samples = sorted(self.sample_index.items(), key=lambda x:x[1])
+            for id in sorted_samples:
+                f.write("\t{}".format(id[0]))
+            f.write("\n")
+            for locus in locus_list:
+                f.write(locus["id"])
+                for id in sorted_samples:
+                    f.write("\t{}".format(locus[id[0]]))
+                f.write("\n")
+
+    def subset(self, locus_list, **kwargs):
         output_list = []
         if "samples" in kwargs:
             sample_list = kwargs["samples"]
         else:
             sample_list = list(self.sample_index.keys())
         if type(locus_list) != list:
             raise Exception("reduce needs list of locus identifiers")
```

