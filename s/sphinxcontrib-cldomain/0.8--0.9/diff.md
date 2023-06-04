# Comparing `tmp/sphinxcontrib-cldomain-0.8-.tar.gz` & `tmp/sphinxcontrib-cldomain-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinxcontrib-cldomain-0.8-.tar", last modified: Mon Feb 10 07:23:08 2014, max compression
+gzip compressed data, was "dist/sphinxcontrib-cldomain-0.9.tar", last modified: Mon Feb 10 07:55:46 2014, max compression
```

## Comparing `sphinxcontrib-cldomain-0.8-.tar` & `sphinxcontrib-cldomain-0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 russell   (2001) russell   (2001)        0 2014-02-10 07:23:08.000000 sphinxcontrib-cldomain-0.8-/
--rw-r--r--   0 russell   (2001) russell   (2001)       97 2014-02-10 07:23:08.000000 sphinxcontrib-cldomain-0.8-/setup.cfg
-drwxr-xr-x   0 russell   (2001) russell   (2001)        0 2014-02-10 07:23:08.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib/
--rw-r--r--   0 russell   (2001) russell   (2001)     1931 2013-04-16 08:39:19.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib/test.lisp
--rw-r--r--   0 russell   (2001) russell   (2001)     1137 2013-04-16 08:40:31.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib/package.lisp
--rw-r--r--   0 russell   (2001) russell   (2001)     1448 2014-02-10 06:56:49.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib/sphinxcontrib.cldomain.asd
--rw-r--r--   0 russell   (2001) russell   (2001)    33840 2014-02-10 07:21:19.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib/cldomain.py
--rw-r--r--   0 russell   (2001) russell   (2001)        6 2014-02-10 07:04:34.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib/version.lisp-expr
--rw-r--r--   0 russell   (2001) russell   (2001)     1113 2013-04-16 08:39:19.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib/sphinxcontrib.cldomain-test.asd
--rw-r--r--   0 russell   (2001) russell   (2001)    56932 2013-04-16 14:41:41.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib/hyperspec.py
--rw-r--r--   0 russell   (2001) russell   (2001)     1017 2013-04-16 08:39:19.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib/__init__.py
--rwxr-xr-x   0 russell   (2001) russell   (2001)    13632 2014-02-10 06:56:49.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib/cldomain.lisp
--rw-r--r--   0 russell   (2001) russell   (2001)     1411 2014-02-10 07:07:42.000000 sphinxcontrib-cldomain-0.8-/CHANGELOG.rst
--rw-r--r--   0 russell   (2001) russell   (2001)      894 2013-04-16 08:39:19.000000 sphinxcontrib-cldomain-0.8-/README.rst
--rw-r--r--   0 russell   (2001) russell   (2001)    35147 2012-04-21 12:03:16.000000 sphinxcontrib-cldomain-0.8-/LICENSE
--rw-r--r--   0 russell   (2001) russell   (2001)     2232 2013-04-16 12:46:17.000000 sphinxcontrib-cldomain-0.8-/setup.py
-drwxr-xr-x   0 russell   (2001) russell   (2001)        0 2014-02-10 07:23:08.000000 sphinxcontrib-cldomain-0.8-/doc/
--rw-r--r--   0 russell   (2001) russell   (2001)     2143 2013-06-12 08:23:56.000000 sphinxcontrib-cldomain-0.8-/doc/doc.lisp
--rw-r--r--   0 russell   (2001) russell   (2001)     1035 2012-11-23 23:53:16.000000 sphinxcontrib-cldomain-0.8-/doc/sphinxcontrib.cldomain.doc.asd
--rw-r--r--   0 russell   (2001) russell   (2001)     3648 2014-02-10 07:23:08.000000 sphinxcontrib-cldomain-0.8-/PKG-INFO
--rw-r--r--   0 russell   (2001) russell   (2001)      145 2013-06-12 08:11:11.000000 sphinxcontrib-cldomain-0.8-/MANIFEST.in
-drwxr-xr-x   0 russell   (2001) russell   (2001)        0 2014-02-10 07:23:08.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib_cldomain.egg-info/
--rw-r--r--   0 russell   (2001) russell   (2001)      717 2014-02-10 07:23:08.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib_cldomain.egg-info/SOURCES.txt
--rw-r--r--   0 russell   (2001) russell   (2001)        1 2014-02-10 07:23:07.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib_cldomain.egg-info/dependency_links.txt
--rw-r--r--   0 russell   (2001) russell   (2001)     3648 2014-02-10 07:23:07.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib_cldomain.egg-info/PKG-INFO
--rw-r--r--   0 russell   (2001) russell   (2001)       11 2014-02-10 07:23:07.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib_cldomain.egg-info/requires.txt
--rw-r--r--   0 russell   (2001) russell   (2001)       14 2014-02-10 07:23:07.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib_cldomain.egg-info/top_level.txt
--rw-r--r--   0 russell   (2001) russell   (2001)        1 2012-04-21 10:41:18.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib_cldomain.egg-info/not-zip-safe
--rw-r--r--   0 russell   (2001) russell   (2001)       14 2014-02-10 07:23:07.000000 sphinxcontrib-cldomain-0.8-/sphinxcontrib_cldomain.egg-info/namespace_packages.txt
+drwxr-xr-x   0 russell   (2001) russell   (2001)        0 2014-02-10 07:55:46.000000 sphinxcontrib-cldomain-0.9/
+-rw-r--r--   0 russell   (2001) russell   (2001)       97 2014-02-10 07:55:46.000000 sphinxcontrib-cldomain-0.9/setup.cfg
+drwxr-xr-x   0 russell   (2001) russell   (2001)        0 2014-02-10 07:55:46.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib/
+-rw-r--r--   0 russell   (2001) russell   (2001)     1931 2013-04-16 08:39:19.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib/test.lisp
+-rw-r--r--   0 russell   (2001) russell   (2001)     1137 2013-04-16 08:40:31.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib/package.lisp
+-rw-r--r--   0 russell   (2001) russell   (2001)     1448 2014-02-10 06:56:49.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib/sphinxcontrib.cldomain.asd
+-rw-r--r--   0 russell   (2001) russell   (2001)    33840 2014-02-10 07:55:05.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib/cldomain.py
+-rw-r--r--   0 russell   (2001) russell   (2001)        5 2014-02-10 07:55:33.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib/version.lisp-expr
+-rw-r--r--   0 russell   (2001) russell   (2001)     1113 2013-04-16 08:39:19.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib/sphinxcontrib.cldomain-test.asd
+-rw-r--r--   0 russell   (2001) russell   (2001)    56932 2013-04-16 14:41:41.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib/hyperspec.py
+-rw-r--r--   0 russell   (2001) russell   (2001)     1017 2013-04-16 08:39:19.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib/__init__.py
+-rwxr-xr-x   0 russell   (2001) russell   (2001)    13632 2014-02-10 06:56:49.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib/cldomain.lisp
+-rw-r--r--   0 russell   (2001) russell   (2001)     1505 2014-02-10 07:55:05.000000 sphinxcontrib-cldomain-0.9/CHANGELOG.rst
+-rw-r--r--   0 russell   (2001) russell   (2001)      894 2013-04-16 08:39:19.000000 sphinxcontrib-cldomain-0.9/README.rst
+-rw-r--r--   0 russell   (2001) russell   (2001)    35147 2012-04-21 12:03:16.000000 sphinxcontrib-cldomain-0.9/LICENSE
+-rw-r--r--   0 russell   (2001) russell   (2001)     2240 2014-02-10 07:34:13.000000 sphinxcontrib-cldomain-0.9/setup.py
+drwxr-xr-x   0 russell   (2001) russell   (2001)        0 2014-02-10 07:55:46.000000 sphinxcontrib-cldomain-0.9/doc/
+-rw-r--r--   0 russell   (2001) russell   (2001)     2143 2013-06-12 08:23:56.000000 sphinxcontrib-cldomain-0.9/doc/doc.lisp
+-rw-r--r--   0 russell   (2001) russell   (2001)     1035 2012-11-23 23:53:16.000000 sphinxcontrib-cldomain-0.9/doc/sphinxcontrib.cldomain.doc.asd
+-rw-r--r--   0 russell   (2001) russell   (2001)     3773 2014-02-10 07:55:46.000000 sphinxcontrib-cldomain-0.9/PKG-INFO
+-rw-r--r--   0 russell   (2001) russell   (2001)      145 2013-06-12 08:11:11.000000 sphinxcontrib-cldomain-0.9/MANIFEST.in
+drwxr-xr-x   0 russell   (2001) russell   (2001)        0 2014-02-10 07:55:46.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib_cldomain.egg-info/
+-rw-r--r--   0 russell   (2001) russell   (2001)      717 2014-02-10 07:55:46.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib_cldomain.egg-info/SOURCES.txt
+-rw-r--r--   0 russell   (2001) russell   (2001)        1 2014-02-10 07:55:46.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib_cldomain.egg-info/dependency_links.txt
+-rw-r--r--   0 russell   (2001) russell   (2001)     3773 2014-02-10 07:55:46.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib_cldomain.egg-info/PKG-INFO
+-rw-r--r--   0 russell   (2001) russell   (2001)       11 2014-02-10 07:55:46.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib_cldomain.egg-info/requires.txt
+-rw-r--r--   0 russell   (2001) russell   (2001)       14 2014-02-10 07:55:46.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib_cldomain.egg-info/top_level.txt
+-rw-r--r--   0 russell   (2001) russell   (2001)        1 2012-04-21 10:41:18.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib_cldomain.egg-info/not-zip-safe
+-rw-r--r--   0 russell   (2001) russell   (2001)       14 2014-02-10 07:55:46.000000 sphinxcontrib-cldomain-0.9/sphinxcontrib_cldomain.egg-info/namespace_packages.txt
```

### Comparing `sphinxcontrib-cldomain-0.8-/sphinxcontrib/test.lisp` & `sphinxcontrib-cldomain-0.9/sphinxcontrib/test.lisp`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-cldomain-0.8-/sphinxcontrib/package.lisp` & `sphinxcontrib-cldomain-0.9/sphinxcontrib/package.lisp`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-cldomain-0.8-/sphinxcontrib/sphinxcontrib.cldomain.asd` & `sphinxcontrib-cldomain-0.9/sphinxcontrib/sphinxcontrib.cldomain.asd`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-cldomain-0.8-/sphinxcontrib/cldomain.py` & `sphinxcontrib-cldomain-0.9/sphinxcontrib/cldomain.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-cldomain-0.8-/sphinxcontrib/sphinxcontrib.cldomain-test.asd` & `sphinxcontrib-cldomain-0.9/sphinxcontrib/sphinxcontrib.cldomain-test.asd`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-cldomain-0.8-/sphinxcontrib/hyperspec.py` & `sphinxcontrib-cldomain-0.9/sphinxcontrib/hyperspec.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-cldomain-0.8-/sphinxcontrib/__init__.py` & `sphinxcontrib-cldomain-0.9/sphinxcontrib/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-cldomain-0.8-/sphinxcontrib/cldomain.lisp` & `sphinxcontrib-cldomain-0.9/sphinxcontrib/cldomain.lisp`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-cldomain-0.8-/CHANGELOG.rst` & `sphinxcontrib-cldomain-0.9/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+Release 0.9 10-02-2014
+----------------------
+* fixed problem with version number generation
+
 Release 0.8 10-02-2014
 ----------------------
 * fixed bug with lisps argument
 * removed dependency on swank
 * remove specializers symbols package if it's the current package
 
 Release 0.7 12-06-2013
```

### Comparing `sphinxcontrib-cldomain-0.8-/README.rst` & `sphinxcontrib-cldomain-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-cldomain-0.8-/LICENSE` & `sphinxcontrib-cldomain-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-cldomain-0.8-/setup.py` & `sphinxcontrib-cldomain-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 desc_file = path.join(path.dirname(__file__), "README.rst")
 changelog_file = path.join(path.dirname(__file__), "CHANGELOG.rst")
 description = open(desc_file).read() + changelog_header + open(changelog_file).read()
 
 __version__ = open(path.join(path.dirname(__file__),
                              "sphinxcontrib",
-                             "version.lisp-expr")).read().strip('"')
+                             "version.lisp-expr")).read().strip().strip('"')
 
 requires = ['Sphinx>=0.6']
 
 setup(
     name='sphinxcontrib-cldomain',
     version=__version__,
     url='http://cldomain.russellsim.org/',
```

### Comparing `sphinxcontrib-cldomain-0.8-/doc/doc.lisp` & `sphinxcontrib-cldomain-0.9/doc/doc.lisp`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-cldomain-0.8-/doc/sphinxcontrib.cldomain.doc.asd` & `sphinxcontrib-cldomain-0.9/doc/sphinxcontrib.cldomain.doc.asd`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-cldomain-0.8-/PKG-INFO` & `sphinxcontrib-cldomain-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sphinxcontrib-cldomain
-Version: 0.8-
+Version: 0.9
 Summary: Sphinx domain for Common Lisp
 Home-page: http://cldomain.russellsim.org/
 Author: Russell Sim
 Author-email: russell.sim@gmail.com
 License: GPL
 Download-URL: http://pypi.python.org/pypi/sphinxcontrib-cldomain
 Description: CLDomain
@@ -32,14 +32,18 @@
         .. _Bug Tracker: https://github.com/russell/sphinxcontrib-cldomain
         .. _GPLv3: https://www.gnu.org/licenses/gpl-3.0-standalone.html
         
         
         Changelog
         =========
         
+        Release 0.9 10-02-2014
+        ----------------------
+        * fixed problem with version number generation
+        
         Release 0.8 10-02-2014
         ----------------------
         * fixed bug with lisps argument
         * removed dependency on swank
         * remove specializers symbols package if it's the current package
         
         Release 0.7 12-06-2013
```

### Comparing `sphinxcontrib-cldomain-0.8-/sphinxcontrib_cldomain.egg-info/SOURCES.txt` & `sphinxcontrib-cldomain-0.9/sphinxcontrib_cldomain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-cldomain-0.8-/sphinxcontrib_cldomain.egg-info/PKG-INFO` & `sphinxcontrib-cldomain-0.9/sphinxcontrib_cldomain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sphinxcontrib-cldomain
-Version: 0.8-
+Version: 0.9
 Summary: Sphinx domain for Common Lisp
 Home-page: http://cldomain.russellsim.org/
 Author: Russell Sim
 Author-email: russell.sim@gmail.com
 License: GPL
 Download-URL: http://pypi.python.org/pypi/sphinxcontrib-cldomain
 Description: CLDomain
@@ -32,14 +32,18 @@
         .. _Bug Tracker: https://github.com/russell/sphinxcontrib-cldomain
         .. _GPLv3: https://www.gnu.org/licenses/gpl-3.0-standalone.html
         
         
         Changelog
         =========
         
+        Release 0.9 10-02-2014
+        ----------------------
+        * fixed problem with version number generation
+        
         Release 0.8 10-02-2014
         ----------------------
         * fixed bug with lisps argument
         * removed dependency on swank
         * remove specializers symbols package if it's the current package
         
         Release 0.7 12-06-2013
```

