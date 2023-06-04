# Comparing `tmp/cs.pfx-20230331.tar.gz` & `tmp/cs.pfx-20230604.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.pfx-20230331.tar", last modified: Fri Mar 31 10:10:05 2023, max compression
+gzip compressed data, was "cs.pfx-20230604.tar", last modified: Sun Jun  4 00:13:54 2023, max compression
```

## Comparing `cs.pfx-20230331.tar` & `cs.pfx-20230604.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-03-31 10:10:05.565458 cs.pfx-20230331/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-03-31 10:09:27.000000 cs.pfx-20230331/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     9765 2023-03-31 10:10:05.565629 cs.pfx-20230331/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    10959 2023-03-31 10:09:34.000000 cs.pfx-20230331/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-03-31 10:10:05.560725 cs.pfx-20230331/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-03-31 10:10:05.561092 cs.pfx-20230331/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-03-31 10:10:05.563372 cs.pfx-20230331/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    21282 2023-03-31 10:09:14.000000 cs.pfx-20230331/lib/python/cs/pfx.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-03-31 10:10:05.565173 cs.pfx-20230331/lib/python/cs.pfx.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     9765 2023-03-31 10:10:05.000000 cs.pfx-20230331/lib/python/cs.pfx.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      280 2023-03-31 10:10:05.000000 cs.pfx-20230331/lib/python/cs.pfx.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-03-31 10:10:05.000000 cs.pfx-20230331/lib/python/cs.pfx.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       71 2023-03-31 10:10:05.000000 cs.pfx-20230331/lib/python/cs.pfx.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-03-31 10:10:05.000000 cs.pfx-20230331/lib/python/cs.pfx.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    10026 2023-03-31 10:09:55.000000 cs.pfx-20230331/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)      909 2023-03-31 10:10:05.566323 cs.pfx-20230331/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-03-31 10:09:34.000000 cs.pfx-20230331/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-04 00:13:54.044437 cs.pfx-20230604/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-04 00:13:16.000000 cs.pfx-20230604/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     9893 2023-06-04 00:13:54.044596 cs.pfx-20230604/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    11087 2023-06-04 00:13:24.000000 cs.pfx-20230604/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-04 00:13:54.040011 cs.pfx-20230604/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-04 00:13:54.040365 cs.pfx-20230604/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-04 00:13:54.042394 cs.pfx-20230604/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    21308 2023-06-04 00:13:07.000000 cs.pfx-20230604/lib/python/cs/pfx.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-04 00:13:54.044124 cs.pfx-20230604/lib/python/cs.pfx.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     9893 2023-06-04 00:13:54.000000 cs.pfx-20230604/lib/python/cs.pfx.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      280 2023-06-04 00:13:54.000000 cs.pfx-20230604/lib/python/cs.pfx.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-04 00:13:54.000000 cs.pfx-20230604/lib/python/cs.pfx.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       71 2023-06-04 00:13:54.000000 cs.pfx-20230604/lib/python/cs.pfx.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-04 00:13:54.000000 cs.pfx-20230604/lib/python/cs.pfx.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    10154 2023-06-04 00:13:46.000000 cs.pfx-20230604/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)      909 2023-06-04 00:13:54.045230 cs.pfx-20230604/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-04 00:13:24.000000 cs.pfx-20230604/setup.py
```

### Comparing `cs.pfx-20230331/PKG-INFO` & `cs.pfx-20230604/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.pfx
-Version: 20230331
+Version: 20230604
 Summary: Easy context prefixes for messages.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -16,16 +16,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Dynamic message prefixes providing execution context.
 
-*Latest release 20230331*:
-PfxThread: use HasThreadState.Thread, make target mandatory.
+*Latest release 20230604*:
+@pfx_method: handle methods with no __name__ (generally a misuse of the decorator).
 
 The primary facility here is `Pfx`,
 a context manager which maintains a per thread stack of context prefixes.
 There are also decorators for functions.
 This stack is used to prefix logging messages and exception text with context.
 
 Usage is like this:
@@ -204,14 +204,17 @@
 
     XX("NOTE!", "some message")
 
 # Release Log
 
 
 
+*Release 20230604*:
+@pfx_method: handle methods with no __name__ (generally a misuse of the decorator).
+
 *Release 20230331*:
 PfxThread: use HasThreadState.Thread, make target mandatory.
 
 *Release 20221118*:
 pkg_tags: cs.py.func: update PyPI release: set pypi.release='20221118' [IGNORE]
 
 *Release 20220918*:
```

### Comparing `cs.pfx-20230331/README.md` & `cs.pfx-20230604/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Dynamic message prefixes providing execution context.
 
-*Latest release 20230331*:
-PfxThread: use HasThreadState.Thread, make target mandatory.
+*Latest release 20230604*:
+@pfx_method: handle methods with no __name__ (generally a misuse of the decorator).
 
 The primary facility here is `Pfx`,
 a context manager which maintains a per thread stack of context prefixes.
 There are also decorators for functions.
 This stack is used to prefix logging messages and exception text with context.
 
 Usage is like this:
@@ -251,14 +251,17 @@
 
     XX("NOTE!", "some message")
 
 # Release Log
 
 
 
+*Release 20230604*:
+@pfx_method: handle methods with no __name__ (generally a misuse of the decorator).
+
 *Release 20230331*:
 PfxThread: use HasThreadState.Thread, make target mandatory.
 
 *Release 20221118*:
 pkg_tags: cs.py.func: update PyPI release: set pypi.release='20221118' [IGNORE]
 
 *Release 20220918*:
```

### Comparing `cs.pfx-20230331/lib/python/cs/pfx.py` & `cs.pfx-20230604/lib/python/cs/pfx.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 from cs.deco import decorator, contextdecorator, fmtdoc, logging_wrapper
 from cs.py.func import funcname, func_a_kw_fmt
 from cs.py3 import StringTypes, ustr, unicode
 
 from cs.x import X
 
-__version__ = '20230331'
+__version__ = '20230604'
 
 DISTINFO = {
     'description':
     "Easy context prefixes for messages.",
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
@@ -689,15 +689,15 @@
                   ....
               # include the "b", "c" and "x" arguments
               @pfx_method(with_args=[1,2,'x'])
               def foo3(self, a, b, c, *, x=1, y):
                   ....
   '''
 
-  fname = method.__name__
+  fname = getattr(method, '__name__', repr(method))
 
   def pfx_method_wrapper(self, *a, **kw):
     ''' Prefix messages with "type_name.method_name" or "str(self).method_name".
     '''
     classref = self if use_str else type(self).__name__
     pfxfmt, pfxargs = func_a_kw_fmt(method, *a, **kw)
     with Pfx("%s." + pfxfmt, classref, *pfxargs):
```

### Comparing `cs.pfx-20230331/lib/python/cs.pfx.egg-info/PKG-INFO` & `cs.pfx-20230604/lib/python/cs.pfx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.pfx
-Version: 20230331
+Version: 20230604
 Summary: Easy context prefixes for messages.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -16,16 +16,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Dynamic message prefixes providing execution context.
 
-*Latest release 20230331*:
-PfxThread: use HasThreadState.Thread, make target mandatory.
+*Latest release 20230604*:
+@pfx_method: handle methods with no __name__ (generally a misuse of the decorator).
 
 The primary facility here is `Pfx`,
 a context manager which maintains a per thread stack of context prefixes.
 There are also decorators for functions.
 This stack is used to prefix logging messages and exception text with context.
 
 Usage is like this:
@@ -204,14 +204,17 @@
 
     XX("NOTE!", "some message")
 
 # Release Log
 
 
 
+*Release 20230604*:
+@pfx_method: handle methods with no __name__ (generally a misuse of the decorator).
+
 *Release 20230331*:
 PfxThread: use HasThreadState.Thread, make target mandatory.
 
 *Release 20221118*:
 pkg_tags: cs.py.func: update PyPI release: set pypi.release='20221118' [IGNORE]
 
 *Release 20220918*:
```

### Comparing `cs.pfx-20230331/pyproject.toml` & `cs.pfx-20230604/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230331"
+version = "20230604"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Dynamic message prefixes providing execution context.
 
-*Latest release 20230331*:
-PfxThread: use HasThreadState.Thread, make target mandatory.
+*Latest release 20230604*:
+@pfx_method: handle methods with no __name__ (generally a misuse of the decorator).
 
 The primary facility here is `Pfx`,
 a context manager which maintains a per thread stack of context prefixes.
 There are also decorators for functions.
 This stack is used to prefix logging messages and exception text with context.
 
 Usage is like this:
@@ -220,14 +220,17 @@
 
     XX(\"NOTE!\", \"some message\")
 
 # Release Log
 
 
 
+*Release 20230604*:
+@pfx_method: handle methods with no __name__ (generally a misuse of the decorator).
+
 *Release 20230331*:
 PfxThread: use HasThreadState.Thread, make target mandatory.
 
 *Release 20221118*:
 pkg_tags: cs.py.func: update PyPI release: set pypi.release='20221118' [IGNORE]
 
 *Release 20220918*:
```

### Comparing `cs.pfx-20230331/setup.cfg` & `cs.pfx-20230604/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.pfx
-version = 20230331
+version = 20230604
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Easy context prefixes for messages.
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers =
```

