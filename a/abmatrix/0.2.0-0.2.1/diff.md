# Comparing `tmp/abmatrix-0.2.0.tar.gz` & `tmp/abmatrix-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abmatrix-0.2.0.tar", last modified: Sun Jun  4 15:35:52 2023, max compression
+gzip compressed data, was "abmatrix-0.2.1.tar", last modified: Sun Jun  4 15:59:15 2023, max compression
```

## Comparing `abmatrix-0.2.0.tar` & `abmatrix-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:35:52.335849 abmatrix-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-04 15:35:52.335849 abmatrix-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-04 15:35:42.000000 abmatrix-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:35:52.335849 abmatrix-0.2.0/abmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 15:35:42.000000 abmatrix-0.2.0/abmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-04 15:35:42.000000 abmatrix-0.2.0/abmatrix/abmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:35:52.335849 abmatrix-0.2.0/abmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-04 15:35:52.000000 abmatrix-0.2.0/abmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-04 15:35:52.000000 abmatrix-0.2.0/abmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 15:35:52.000000 abmatrix-0.2.0/abmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 15:35:52.000000 abmatrix-0.2.0/abmatrix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 15:35:42.000000 abmatrix-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-04 15:35:52.339849 abmatrix-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:59:15.048549 abmatrix-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-04 15:59:15.048549 abmatrix-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-04 15:59:05.000000 abmatrix-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:59:15.048549 abmatrix-0.2.1/abmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 15:59:05.000000 abmatrix-0.2.1/abmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-04 15:59:05.000000 abmatrix-0.2.1/abmatrix/abmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:59:15.048549 abmatrix-0.2.1/abmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-04 15:59:15.000000 abmatrix-0.2.1/abmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-04 15:59:15.000000 abmatrix-0.2.1/abmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 15:59:15.000000 abmatrix-0.2.1/abmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 15:59:15.000000 abmatrix-0.2.1/abmatrix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 15:59:05.000000 abmatrix-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-04 15:59:15.048549 abmatrix-0.2.1/setup.cfg
```

### Comparing `abmatrix-0.2.0/abmatrix/abmatrix.py` & `abmatrix-0.2.1/abmatrix/abmatrix.py`

 * *Files 23% similar despite different names*

```diff
@@ -36,14 +36,27 @@
                         for pos, sample in enumerate(sample_list):
                             self.sample_index[sample] = pos
                         is_header = False
                     else:
                         entry = line.rstrip("\n").split("\t")
                         if len(entry) < 2:
                             raise Exception("Malformed header")
+                        elif len(entry) > 2:
+                            nread = 0
+                            key = ""
+                            value = ""
+                            for elem in entry:
+                                if len(elem) > 1:
+                                    if nread < 1:
+                                        key = elem
+                                        nread += 1
+                                    else:
+                                        value = elem
+                                        break
+                            self.header[key] = value
                         else:
                             self.header[entry[0]] = entry[1]
                 else:
                     locus_id = line.rstrip("\n").split("\t")[0]
                     self.index[locus_id] = offset
                 offset += len(line)
         else:
```

