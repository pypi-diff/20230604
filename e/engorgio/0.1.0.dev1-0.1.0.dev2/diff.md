# Comparing `tmp/engorgio-0.1.0.dev1.tar.gz` & `tmp/engorgio-0.1.0.dev2.tar.gz`

## Comparing `engorgio-0.1.0.dev1.tar` & `engorgio-0.1.0.dev2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/.pydantic-typer-copier-answers.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/CHANGELOG.md
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/.github/workflows/release.yml
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/engorgio/__about__.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/engorgio/__init__.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/engorgio/decorator.py
--rw-r--r--   0        0        0     6107 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/engorgio/expand.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/examples/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/examples/person.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/examples/person_cli.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/tests/__init__.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/tests/models.py
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/tests/test_person.py
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/LICENSE.txt
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/README.md
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/.pydantic-typer-copier-answers.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/CHANGELOG.md
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/engorgio/__about__.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/engorgio/__init__.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/engorgio/decorator.py
+-rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/engorgio/expand.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/examples/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/examples/person.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/examples/person_cli.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/tests/__init__.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/tests/models.py
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/tests/test_person.py
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/LICENSE.txt
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/README.md
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/PKG-INFO
```

### Comparing `engorgio-0.1.0.dev1/engorgio/decorator.py` & `engorgio-0.1.0.dev2/engorgio/decorator.py`

 * *Files identical despite different names*

### Comparing `engorgio-0.1.0.dev1/engorgio/expand.py` & `engorgio-0.1.0.dev2/engorgio/expand.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,15 @@
     for name, value in kwargs.items():
         if name in sig.parameters:
             updated_kwargs[name] = value
 
     for name, param in sig.parameters.items():
         # func wants this directly
         # this should check isinstance, but it's not working
+        #
         if name in kwargs and repr(param.annotation) == repr(kwargs[name]):
             updated_kwargs[name] = kwargs[name]
 
         # an instance was not passed in, create one with kwargs passed in
         elif hasattr(param.annotation, "__fields__"):
             updated_kwargs[name] = expand_param(param, kwargs)
         # its something else so pass it
```

### Comparing `engorgio-0.1.0.dev1/examples/person_cli.py` & `engorgio-0.1.0.dev2/examples/person_cli.py`

 * *Files identical despite different names*

### Comparing `engorgio-0.1.0.dev1/tests/models.py` & `engorgio-0.1.0.dev2/tests/models.py`

 * *Files identical despite different names*

### Comparing `engorgio-0.1.0.dev1/tests/test_person.py` & `engorgio-0.1.0.dev2/tests/test_person.py`

 * *Files identical despite different names*

### Comparing `engorgio-0.1.0.dev1/.gitignore` & `engorgio-0.1.0.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `engorgio-0.1.0.dev1/LICENSE.txt` & `engorgio-0.1.0.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `engorgio-0.1.0.dev1/README.md` & `engorgio-0.1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `engorgio-0.1.0.dev1/pyproject.toml` & `engorgio-0.1.0.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `engorgio-0.1.0.dev1/PKG-INFO` & `engorgio-0.1.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: engorgio
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: Expand pydantic function arguments by casting the engorgio decorator
 Project-URL: Documentation, https://github.com/waylonwalker/engorgio#readme
 Project-URL: Issues, https://github.com/waylonwalker/engorgio/issues
 Project-URL: Source, https://github.com/waylonwalker/engorgio
 Project-URL: Changelog, https://github.com/WaylonWalker/engorgio/blob/main/CHANGELOG.md
 Author-email: "Waylon S. Walker" <waylon@waylonwalker.com>
 License-Expression: MIT
```

