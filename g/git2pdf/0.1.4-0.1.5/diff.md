# Comparing `tmp/git2pdf-0.1.4.tar.gz` & `tmp/git2pdf-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2pdf-0.1.4.tar", last modified: Sun Jun  4 21:08:26 2023, max compression
+gzip compressed data, was "git2pdf-0.1.5.tar", last modified: Sun Jun  4 21:32:28 2023, max compression
```

## Comparing `git2pdf-0.1.4.tar` & `git2pdf-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 21:08:26.974129 git2pdf-0.1.4/
--rw-r--r--   0 erguncan   (501) staff       (20)     1079 2023-06-04 20:31:55.000000 git2pdf-0.1.4/LICENSE.txt
--rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 21:08:26.974233 git2pdf-0.1.4/PKG-INFO
--rw-r--r--   0 erguncan   (501) staff       (20)      389 2023-06-04 20:32:44.000000 git2pdf-0.1.4/README.rst
-drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 21:08:26.972679 git2pdf-0.1.4/git2pdf/
--rw-r--r--   0 erguncan   (501) staff       (20)   757076 2023-06-04 01:56:54.000000 git2pdf-0.1.4/git2pdf/DejaVuSans.ttf
--rw-r--r--   0 erguncan   (501) staff       (20)     4491 2023-06-04 21:08:09.000000 git2pdf-0.1.4/git2pdf/main.py
-drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 21:08:26.973998 git2pdf-0.1.4/git2pdf.egg-info/
--rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 21:08:26.000000 git2pdf-0.1.4/git2pdf.egg-info/PKG-INFO
--rw-r--r--   0 erguncan   (501) staff       (20)      298 2023-06-04 21:08:26.000000 git2pdf-0.1.4/git2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 21:08:26.000000 git2pdf-0.1.4/git2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 erguncan   (501) staff       (20)       47 2023-06-04 21:08:26.000000 git2pdf-0.1.4/git2pdf.egg-info/entry_points.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:34:17.000000 git2pdf-0.1.4/git2pdf.egg-info/not-zip-safe
--rw-r--r--   0 erguncan   (501) staff       (20)       14 2023-06-04 21:08:26.000000 git2pdf-0.1.4/git2pdf.egg-info/requires.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        8 2023-06-04 21:08:26.000000 git2pdf-0.1.4/git2pdf.egg-info/top_level.txt
--rw-r--r--   0 erguncan   (501) staff       (20)      712 2023-06-04 21:08:26.974622 git2pdf-0.1.4/setup.cfg
--rw-r--r--   0 erguncan   (501) staff       (20)      321 2023-06-04 21:02:04.000000 git2pdf-0.1.4/setup.py
+drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 21:32:28.585536 git2pdf-0.1.5/
+-rw-r--r--   0 erguncan   (501) staff       (20)     1079 2023-06-04 20:31:55.000000 git2pdf-0.1.5/LICENSE.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 21:32:28.585609 git2pdf-0.1.5/PKG-INFO
+-rw-r--r--   0 erguncan   (501) staff       (20)      389 2023-06-04 20:32:44.000000 git2pdf-0.1.5/README.rst
+drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 21:32:28.584099 git2pdf-0.1.5/git2pdf/
+-rw-r--r--   0 erguncan   (501) staff       (20)   757076 2023-06-04 01:56:54.000000 git2pdf-0.1.5/git2pdf/DejaVuSans.ttf
+-rw-r--r--   0 erguncan   (501) staff       (20)     4491 2023-06-04 21:31:25.000000 git2pdf-0.1.5/git2pdf/main.py
+drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 21:32:28.585409 git2pdf-0.1.5/git2pdf.egg-info/
+-rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 21:32:28.000000 git2pdf-0.1.5/git2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 erguncan   (501) staff       (20)      298 2023-06-04 21:32:28.000000 git2pdf-0.1.5/git2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 21:32:28.000000 git2pdf-0.1.5/git2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)       47 2023-06-04 21:32:28.000000 git2pdf-0.1.5/git2pdf.egg-info/entry_points.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:34:17.000000 git2pdf-0.1.5/git2pdf.egg-info/not-zip-safe
+-rw-r--r--   0 erguncan   (501) staff       (20)       15 2023-06-04 21:32:28.000000 git2pdf-0.1.5/git2pdf.egg-info/requires.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        8 2023-06-04 21:32:28.000000 git2pdf-0.1.5/git2pdf.egg-info/top_level.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)      713 2023-06-04 21:32:28.585966 git2pdf-0.1.5/setup.cfg
+-rw-r--r--   0 erguncan   (501) staff       (20)      322 2023-06-04 21:32:22.000000 git2pdf-0.1.5/setup.py
```

### Comparing `git2pdf-0.1.4/LICENSE.txt` & `git2pdf-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `git2pdf-0.1.4/PKG-INFO` & `git2pdf-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2pdf
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generate a PDF with the contents of files in a GitHub repository
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git2pdf-0.1.4/git2pdf/DejaVuSans.ttf` & `git2pdf-0.1.5/git2pdf/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `git2pdf-0.1.4/git2pdf/main.py` & `git2pdf-0.1.5/git2pdf/main.py`

 * *Files identical despite different names*

### Comparing `git2pdf-0.1.4/git2pdf.egg-info/PKG-INFO` & `git2pdf-0.1.5/git2pdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2pdf
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generate a PDF with the contents of files in a GitHub repository
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git2pdf-0.1.4/setup.cfg` & `git2pdf-0.1.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = git2pdf
-version = 0.1.4
+version = 0.1.5
 description = Generate a PDF with the contents of files in a GitHub repository
 long_description = file: README.rst
 license = MIT
 classifiers = 
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	requests
-	fpdf
+	fpdf2
 
 [options.package_data]
 git2pdf = *.ttf
 
 [options.entry_points]
 console_scripts = 
 	git2pdf = git2pdf.main:main
```

