# Comparing `tmp/git2pdf-0.1.3.tar.gz` & `tmp/git2pdf-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2pdf-0.1.3.tar", last modified: Sun Jun  4 20:47:18 2023, max compression
+gzip compressed data, was "git2pdf-0.1.4.tar", last modified: Sun Jun  4 21:08:26 2023, max compression
```

## Comparing `git2pdf-0.1.3.tar` & `git2pdf-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 20:47:18.187999 git2pdf-0.1.3/
--rw-r--r--   0 erguncan   (501) staff       (20)     1079 2023-06-04 20:31:55.000000 git2pdf-0.1.3/LICENSE.txt
--rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 20:47:18.188070 git2pdf-0.1.3/PKG-INFO
--rw-r--r--   0 erguncan   (501) staff       (20)      389 2023-06-04 20:32:44.000000 git2pdf-0.1.3/README.rst
-drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 20:47:18.187880 git2pdf-0.1.3/git2pdf.egg-info/
--rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 20:47:18.000000 git2pdf-0.1.3/git2pdf.egg-info/PKG-INFO
--rw-r--r--   0 erguncan   (501) staff       (20)      267 2023-06-04 20:47:18.000000 git2pdf-0.1.3/git2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:47:18.000000 git2pdf-0.1.3/git2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 erguncan   (501) staff       (20)       39 2023-06-04 20:47:18.000000 git2pdf-0.1.3/git2pdf.egg-info/entry_points.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:34:17.000000 git2pdf-0.1.3/git2pdf.egg-info/not-zip-safe
--rw-r--r--   0 erguncan   (501) staff       (20)       14 2023-06-04 20:47:18.000000 git2pdf-0.1.3/git2pdf.egg-info/requires.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        5 2023-06-04 20:47:18.000000 git2pdf-0.1.3/git2pdf.egg-info/top_level.txt
--rw-r--r--   0 erguncan   (501) staff       (20)     4482 2023-06-04 20:46:27.000000 git2pdf-0.1.3/main.py
--rw-r--r--   0 erguncan   (501) staff       (20)      665 2023-06-04 20:47:18.188401 git2pdf-0.1.3/setup.cfg
--rw-r--r--   0 erguncan   (501) staff       (20)      344 2023-06-04 20:47:07.000000 git2pdf-0.1.3/setup.py
+drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 21:08:26.974129 git2pdf-0.1.4/
+-rw-r--r--   0 erguncan   (501) staff       (20)     1079 2023-06-04 20:31:55.000000 git2pdf-0.1.4/LICENSE.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 21:08:26.974233 git2pdf-0.1.4/PKG-INFO
+-rw-r--r--   0 erguncan   (501) staff       (20)      389 2023-06-04 20:32:44.000000 git2pdf-0.1.4/README.rst
+drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 21:08:26.972679 git2pdf-0.1.4/git2pdf/
+-rw-r--r--   0 erguncan   (501) staff       (20)   757076 2023-06-04 01:56:54.000000 git2pdf-0.1.4/git2pdf/DejaVuSans.ttf
+-rw-r--r--   0 erguncan   (501) staff       (20)     4491 2023-06-04 21:08:09.000000 git2pdf-0.1.4/git2pdf/main.py
+drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-04 21:08:26.973998 git2pdf-0.1.4/git2pdf.egg-info/
+-rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-04 21:08:26.000000 git2pdf-0.1.4/git2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 erguncan   (501) staff       (20)      298 2023-06-04 21:08:26.000000 git2pdf-0.1.4/git2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 21:08:26.000000 git2pdf-0.1.4/git2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)       47 2023-06-04 21:08:26.000000 git2pdf-0.1.4/git2pdf.egg-info/entry_points.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:34:17.000000 git2pdf-0.1.4/git2pdf.egg-info/not-zip-safe
+-rw-r--r--   0 erguncan   (501) staff       (20)       14 2023-06-04 21:08:26.000000 git2pdf-0.1.4/git2pdf.egg-info/requires.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        8 2023-06-04 21:08:26.000000 git2pdf-0.1.4/git2pdf.egg-info/top_level.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)      712 2023-06-04 21:08:26.974622 git2pdf-0.1.4/setup.cfg
+-rw-r--r--   0 erguncan   (501) staff       (20)      321 2023-06-04 21:02:04.000000 git2pdf-0.1.4/setup.py
```

### Comparing `git2pdf-0.1.3/LICENSE.txt` & `git2pdf-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `git2pdf-0.1.3/PKG-INFO` & `git2pdf-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2pdf
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generate a PDF with the contents of files in a GitHub repository
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git2pdf-0.1.3/git2pdf.egg-info/PKG-INFO` & `git2pdf-0.1.4/git2pdf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2pdf
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generate a PDF with the contents of files in a GitHub repository
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git2pdf-0.1.3/main.py` & `git2pdf-0.1.4/git2pdf/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import requests
 import pkg_resources
 import os
 import base64
-from fpdf import FPDF, XPos, YPos
+from fpdf import FPDF
+from fpdf.enums import XPos, YPos
+
 
 def main():
     # Get repository URL from the user
     repo_url = input("Enter the GitHub repository URL: ")
     # Constants for text
     LINE_WIDTH = 200
     CHARS_PER_LINE = 95
     # Extract the owner and repo names from the URL
     owner, repo = repo_url.split("github.com/")[-1].split('/')
 
     # Specify the directory where you want to save the PDF
-    output_directory = os.path.join(os.path.dirname(os.path.realpath(__file__)), "pdf_output")
+    output_directory = os.path.join(os.path.expanduser("~"), "git2pdf_output")
 
     # Ensure the directory exists (if not, create it)
     os.makedirs(output_directory, exist_ok=True)
 
     try:
         # Fetch the file tree
         tree_url = f"https://api.github.com/repos/{owner}/{repo}/git/trees/main?recursive=1"
@@ -101,9 +103,10 @@
         pdf.output(pdf_path)
 
         print(f"\nPDF created successfully at {pdf_path}!")
 
     except Exception as e:
         print(f"An error occurred: {e}")
 
+
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `git2pdf-0.1.3/setup.cfg` & `git2pdf-0.1.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = git2pdf
-version = 0.1.3
+version = 0.1.4
 description = Generate a PDF with the contents of files in a GitHub repository
 long_description = file: README.rst
 license = MIT
 classifiers = 
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
@@ -12,20 +12,23 @@
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 
 [options]
 zip_safe = False
 include_package_data = True
-py_modules = main
+packages = find:
 install_requires = 
 	requests
 	fpdf
 
+[options.package_data]
+git2pdf = *.ttf
+
 [options.entry_points]
 console_scripts = 
-	git2pdf = main:main
+	git2pdf = git2pdf.main:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

