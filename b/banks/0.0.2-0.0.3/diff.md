# Comparing `tmp/banks-0.0.2.tar.gz` & `tmp/banks-0.0.3.tar.gz`

## Comparing `banks-0.0.2.tar` & `banks-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 banks-0.0.2/MANIFEST.in
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 banks-0.0.2/src/banks/__about__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 banks-0.0.2/src/banks/__init__.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 banks-0.0.2/src/banks/env.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 banks-0.0.2/src/banks/prompt.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 banks-0.0.2/src/banks/extensions/__init__.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 banks-0.0.2/src/banks/extensions/generate.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 banks-0.0.2/src/banks/filters/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 banks-0.0.2/src/banks/filters/lemmatize.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 banks-0.0.2/src/banks/templates/blog.jinja
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 banks-0.0.2/src/banks/templates/generate_tweet.jinja
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 banks-0.0.2/src/banks/templates/summarize.jinja
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 banks-0.0.2/src/banks/templates/summarize_lemma.jinja
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 banks-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 banks-0.0.2/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 banks-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 banks-0.0.2/README.md
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 banks-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 banks-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 banks-0.0.3/MANIFEST.in
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/__about__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/__init__.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/env.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/prompt.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/extensions/__init__.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/extensions/generate.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/filters/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/filters/lemmatize.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/templates/blog.jinja
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/templates/generate_tweet.jinja
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/templates/summarize.jinja
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/templates/summarize_lemma.jinja
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 banks-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 banks-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 banks-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 banks-0.0.3/README.md
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 banks-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 banks-0.0.3/PKG-INFO
```

### Comparing `banks-0.0.2/src/banks/env.py` & `banks-0.0.3/src/banks/env.py`

 * *Files identical despite different names*

### Comparing `banks-0.0.2/src/banks/prompt.py` & `banks-0.0.3/src/banks/prompt.py`

 * *Files identical despite different names*

### Comparing `banks-0.0.2/src/banks/extensions/generate.py` & `banks-0.0.3/src/banks/extensions/generate.py`

 * *Files identical despite different names*

### Comparing `banks-0.0.2/.gitignore` & `banks-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `banks-0.0.2/LICENSE.txt` & `banks-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `banks-0.0.2/README.md` & `banks-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `banks-0.0.2/pyproject.toml` & `banks-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,17 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "jinja2"
+  "jinja2",
+  "openai",
+  "simplemma",
 ]
 
 [project.urls]
 Documentation = "https://github.com/unknown/banks#readme"
 Issues = "https://github.com/unknown/banks/issues"
 Source = "https://github.com/unknown/banks"
```

### Comparing `banks-0.0.2/PKG-INFO` & `banks-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banks
-Version: 0.0.2
+Version: 0.0.3
 Summary: A prompt programming language
 Project-URL: Documentation, https://github.com/unknown/banks#readme
 Project-URL: Issues, https://github.com/unknown/banks/issues
 Project-URL: Source, https://github.com/unknown/banks
 Author-email: Massimiliano Pippi <mpippi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: jinja2
+Requires-Dist: openai
+Requires-Dist: simplemma
 Description-Content-Type: text/markdown
 
 # banks
 
 [![PyPI - Version](https://img.shields.io/pypi/v/banks.svg)](https://pypi.org/project/banks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/banks.svg)](https://pypi.org/project/banks)
```

