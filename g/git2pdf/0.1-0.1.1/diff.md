# Comparing `tmp/git2pdf-0.1.tar.gz` & `tmp/git2pdf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2pdf-0.1.tar", last modified: Sun Jun  4 20:34:17 2023, max compression
+gzip compressed data, was "git2pdf-0.1.1.tar", last modified: Sun Jun  4 20:38:06 2023, max compression
```

## Comparing `git2pdf-0.1.tar` & `git2pdf-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 20:34:17.672448 git2pdf-0.1/
--rw-r--r--   0 erguncan   (501) staff       (20)     1079 2023-06-04 20:31:55.000000 git2pdf-0.1/LICENSE.txt
--rw-r--r--   0 erguncan   (501) staff       (20)      934 2023-06-04 20:34:17.672551 git2pdf-0.1/PKG-INFO
--rw-r--r--   0 erguncan   (501) staff       (20)      389 2023-06-04 20:32:44.000000 git2pdf-0.1/README.rst
-drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 20:34:17.672290 git2pdf-0.1/git2pdf.egg-info/
--rw-r--r--   0 erguncan   (501) staff       (20)      934 2023-06-04 20:34:17.000000 git2pdf-0.1/git2pdf.egg-info/PKG-INFO
--rw-r--r--   0 erguncan   (501) staff       (20)      259 2023-06-04 20:34:17.000000 git2pdf-0.1/git2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:34:17.000000 git2pdf-0.1/git2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 erguncan   (501) staff       (20)       42 2023-06-04 20:34:17.000000 git2pdf-0.1/git2pdf.egg-info/entry_points.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:34:17.000000 git2pdf-0.1/git2pdf.egg-info/not-zip-safe
--rw-r--r--   0 erguncan   (501) staff       (20)       38 2023-06-04 20:34:17.000000 git2pdf-0.1/git2pdf.egg-info/requires.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:34:17.000000 git2pdf-0.1/git2pdf.egg-info/top_level.txt
--rw-r--r--   0 erguncan   (501) staff       (20)      694 2023-06-04 20:34:17.672988 git2pdf-0.1/setup.cfg
--rw-r--r--   0 erguncan   (501) staff       (20)      423 2023-06-04 20:29:09.000000 git2pdf-0.1/setup.py
+drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 20:38:06.574382 git2pdf-0.1.1/
+-rw-r--r--   0 erguncan   (501) staff       (20)     1079 2023-06-04 20:31:55.000000 git2pdf-0.1.1/LICENSE.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 20:38:06.574478 git2pdf-0.1.1/PKG-INFO
+-rw-r--r--   0 erguncan   (501) staff       (20)      389 2023-06-04 20:32:44.000000 git2pdf-0.1.1/README.rst
+drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 20:38:06.574214 git2pdf-0.1.1/git2pdf.egg-info/
+-rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 20:38:06.000000 git2pdf-0.1.1/git2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 erguncan   (501) staff       (20)      259 2023-06-04 20:38:06.000000 git2pdf-0.1.1/git2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:38:06.000000 git2pdf-0.1.1/git2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)       42 2023-06-04 20:38:06.000000 git2pdf-0.1.1/git2pdf.egg-info/entry_points.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:34:17.000000 git2pdf-0.1.1/git2pdf.egg-info/not-zip-safe
+-rw-r--r--   0 erguncan   (501) staff       (20)       14 2023-06-04 20:38:06.000000 git2pdf-0.1.1/git2pdf.egg-info/requires.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:38:06.000000 git2pdf-0.1.1/git2pdf.egg-info/top_level.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)      667 2023-06-04 20:38:06.574917 git2pdf-0.1.1/setup.cfg
+-rw-r--r--   0 erguncan   (501) staff       (20)      368 2023-06-04 20:37:17.000000 git2pdf-0.1.1/setup.py
```

### Comparing `git2pdf-0.1/LICENSE.txt` & `git2pdf-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `git2pdf-0.1/PKG-INFO` & `git2pdf-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2pdf
-Version: 0.1
+Version: 0.1.1
 Summary: Generate a PDF with the contents of files in a GitHub repository
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git2pdf-0.1/git2pdf.egg-info/PKG-INFO` & `git2pdf-0.1.1/git2pdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2pdf
-Version: 0.1
+Version: 0.1.1
 Summary: Generate a PDF with the contents of files in a GitHub repository
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git2pdf-0.1/setup.cfg` & `git2pdf-0.1.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = git2pdf
-version = 0.1.0
+version = 0.1.1
 description = Generate a PDF with the contents of files in a GitHub repository
 long_description = file: README.rst
 license = MIT
 classifiers = 
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
@@ -16,17 +16,14 @@
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	requests
 	fpdf
-	os
-	base64
-	pkg_resources
 
 [options.entry_points]
 console_scripts = 
 	git2pdf = git2pdf:main
 
 [egg_info]
 tag_build =
```

