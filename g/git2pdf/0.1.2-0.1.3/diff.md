# Comparing `tmp/git2pdf-0.1.2.tar.gz` & `tmp/git2pdf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2pdf-0.1.2.tar", last modified: Sun Jun  4 20:41:37 2023, max compression
+gzip compressed data, was "git2pdf-0.1.3.tar", last modified: Sun Jun  4 20:47:18 2023, max compression
```

## Comparing `git2pdf-0.1.2.tar` & `git2pdf-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 20:41:37.219284 git2pdf-0.1.2/
--rw-r--r--   0 erguncan   (501) staff       (20)     1079 2023-06-04 20:31:55.000000 git2pdf-0.1.2/LICENSE.txt
--rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 20:41:37.219428 git2pdf-0.1.2/PKG-INFO
--rw-r--r--   0 erguncan   (501) staff       (20)      389 2023-06-04 20:32:44.000000 git2pdf-0.1.2/README.rst
-drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 20:41:37.219120 git2pdf-0.1.2/git2pdf.egg-info/
--rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 20:41:37.000000 git2pdf-0.1.2/git2pdf.egg-info/PKG-INFO
--rw-r--r--   0 erguncan   (501) staff       (20)      259 2023-06-04 20:41:37.000000 git2pdf-0.1.2/git2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:41:37.000000 git2pdf-0.1.2/git2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 erguncan   (501) staff       (20)       42 2023-06-04 20:41:37.000000 git2pdf-0.1.2/git2pdf.egg-info/entry_points.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:34:17.000000 git2pdf-0.1.2/git2pdf.egg-info/not-zip-safe
--rw-r--r--   0 erguncan   (501) staff       (20)       14 2023-06-04 20:41:37.000000 git2pdf-0.1.2/git2pdf.egg-info/requires.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:41:37.000000 git2pdf-0.1.2/git2pdf.egg-info/top_level.txt
--rw-r--r--   0 erguncan   (501) staff       (20)      672 2023-06-04 20:41:37.220002 git2pdf-0.1.2/setup.cfg
--rw-r--r--   0 erguncan   (501) staff       (20)      368 2023-06-04 20:41:29.000000 git2pdf-0.1.2/setup.py
+drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 20:47:18.187999 git2pdf-0.1.3/
+-rw-r--r--   0 erguncan   (501) staff       (20)     1079 2023-06-04 20:31:55.000000 git2pdf-0.1.3/LICENSE.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 20:47:18.188070 git2pdf-0.1.3/PKG-INFO
+-rw-r--r--   0 erguncan   (501) staff       (20)      389 2023-06-04 20:32:44.000000 git2pdf-0.1.3/README.rst
+drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 20:47:18.187880 git2pdf-0.1.3/git2pdf.egg-info/
+-rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 20:47:18.000000 git2pdf-0.1.3/git2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 erguncan   (501) staff       (20)      267 2023-06-04 20:47:18.000000 git2pdf-0.1.3/git2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:47:18.000000 git2pdf-0.1.3/git2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)       39 2023-06-04 20:47:18.000000 git2pdf-0.1.3/git2pdf.egg-info/entry_points.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:34:17.000000 git2pdf-0.1.3/git2pdf.egg-info/not-zip-safe
+-rw-r--r--   0 erguncan   (501) staff       (20)       14 2023-06-04 20:47:18.000000 git2pdf-0.1.3/git2pdf.egg-info/requires.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        5 2023-06-04 20:47:18.000000 git2pdf-0.1.3/git2pdf.egg-info/top_level.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)     4482 2023-06-04 20:46:27.000000 git2pdf-0.1.3/main.py
+-rw-r--r--   0 erguncan   (501) staff       (20)      665 2023-06-04 20:47:18.188401 git2pdf-0.1.3/setup.cfg
+-rw-r--r--   0 erguncan   (501) staff       (20)      344 2023-06-04 20:47:07.000000 git2pdf-0.1.3/setup.py
```

### Comparing `git2pdf-0.1.2/LICENSE.txt` & `git2pdf-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `git2pdf-0.1.2/PKG-INFO` & `git2pdf-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2pdf
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate a PDF with the contents of files in a GitHub repository
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git2pdf-0.1.2/git2pdf.egg-info/PKG-INFO` & `git2pdf-0.1.3/git2pdf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2pdf
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate a PDF with the contents of files in a GitHub repository
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git2pdf-0.1.2/setup.cfg` & `git2pdf-0.1.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = git2pdf
-version = 0.1.2
+version = 0.1.3
 description = Generate a PDF with the contents of files in a GitHub repository
 long_description = file: README.rst
 license = MIT
 classifiers = 
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
@@ -12,20 +12,20 @@
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 
 [options]
 zip_safe = False
 include_package_data = True
-packages = find:
+py_modules = main
 install_requires = 
 	requests
 	fpdf
 
 [options.entry_points]
 console_scripts = 
-	git2pdf = git2pdf.main:main
+	git2pdf = main:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

