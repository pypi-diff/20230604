# Comparing `tmp/briefcase_media-0.3.0.tar.gz` & `tmp/briefcase_media-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "briefcase_media-0.3.0.tar", max compression
+gzip compressed data, was "briefcase_media-0.4.0.tar", max compression
```

## Comparing `briefcase_media-0.3.0.tar` & `briefcase_media-0.4.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       20 2023-06-04 18:45:44.934542 briefcase_media-0.3.0/README.md
--rw-r--r--   0        0        0       81 2023-06-04 19:30:06.514938 briefcase_media-0.3.0/briefcase_media/media.py
--rw-r--r--   0        0        0      376 2023-06-04 19:30:06.514938 briefcase_media-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 briefcase_media-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-06-04 18:45:44.934542 briefcase_media-0.4.0/README.md
+-rw-r--r--   0        0        0       97 2023-06-04 19:43:00.586770 briefcase_media-0.4.0/briefcase_media/media.py
+-rw-r--r--   0        0        0      376 2023-06-04 19:43:18.602672 briefcase_media-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 briefcase_media-0.4.0/PKG-INFO
```

### Comparing `briefcase_media-0.3.0/PKG-INFO` & `briefcase_media-0.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: briefcase-media
-Version: 0.3.0
+Version: 0.4.0
 Summary: This tool shows the current workingdirectory
 Author: tct123
 Author-email: 42028373+tct123@users.noreply.github.com
 Requires-Python: >=3.5,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

