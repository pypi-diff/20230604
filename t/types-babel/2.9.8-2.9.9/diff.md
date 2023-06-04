# Comparing `tmp/types-babel-2.9.8.tar.gz` & `tmp/types-babel-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-babel-2.9.8.tar", last modified: Wed Feb 16 01:04:55 2022, max compression
+gzip compressed data, was "types-babel-2.9.9.tar", last modified: Sat Mar 19 15:18:21 2022, max compression
```

## Comparing `types-babel-2.9.8.tar` & `types-babel-2.9.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 01:04:55.381186 types-babel-2.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-02-16 01:04:53.000000 types-babel-2.9.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-02-16 01:04:53.000000 types-babel-2.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-02-16 01:04:55.381186 types-babel-2.9.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 01:04:55.377186 types-babel-2.9.8/babel-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-02-16 01:04:53.000000 types-babel-2.9.8/babel-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/_compat.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/core.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/dates.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/languages.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/lists.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/localedata.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 01:04:55.381186 types-babel-2.9.8/babel-stubs/localtime/
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/localtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/localtime/_unix.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/localtime/_win32.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 01:04:55.381186 types-babel-2.9.8/babel-stubs/messages/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/messages/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/messages/catalog.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/messages/checkers.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/messages/extract.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2808 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/messages/frontend.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/messages/jslexer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/messages/mofile.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/messages/plurals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/messages/pofile.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/plural.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3681 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/support.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/units.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-02-16 01:04:43.000000 types-babel-2.9.8/babel-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-16 01:04:55.381186 types-babel-2.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-02-16 01:04:53.000000 types-babel-2.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 01:04:55.381186 types-babel-2.9.8/types_babel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-02-16 01:04:55.000000 types-babel-2.9.8/types_babel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-02-16 01:04:55.000000 types-babel-2.9.8/types_babel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-16 01:04:55.000000 types-babel-2.9.8/types_babel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-16 01:04:55.000000 types-babel-2.9.8/types_babel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-16 01:04:55.000000 types-babel-2.9.8/types_babel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-19 15:18:21.708283 types-babel-2.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-03-19 15:18:21.000000 types-babel-2.9.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-03-19 15:18:21.000000 types-babel-2.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-03-19 15:18:21.708283 types-babel-2.9.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-19 15:18:21.708283 types-babel-2.9.9/babel-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-03-19 15:18:21.000000 types-babel-2.9.9/babel-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/_compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/dates.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/languages.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/lists.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/localedata.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-19 15:18:21.708283 types-babel-2.9.9/babel-stubs/localtime/
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/localtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/localtime/_unix.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/localtime/_win32.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-19 15:18:21.708283 types-babel-2.9.9/babel-stubs/messages/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/messages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/messages/catalog.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/messages/checkers.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/messages/extract.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2808 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/messages/frontend.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/messages/jslexer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/messages/mofile.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/messages/plurals.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/messages/pofile.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/plural.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3621 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/support.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/units.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      921 2022-03-19 15:18:00.000000 types-babel-2.9.9/babel-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-19 15:18:21.708283 types-babel-2.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-03-19 15:18:21.000000 types-babel-2.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-19 15:18:21.708283 types-babel-2.9.9/types_babel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-03-19 15:18:21.000000 types-babel-2.9.9/types_babel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-03-19 15:18:21.000000 types-babel-2.9.9/types_babel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-19 15:18:21.000000 types-babel-2.9.9/types_babel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-03-19 15:18:21.000000 types-babel-2.9.9/types_babel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-19 15:18:21.000000 types-babel-2.9.9/types_babel.egg-info/top_level.txt
```

### Comparing `types-babel-2.9.8/CHANGELOG.md` & `types-babel-2.9.9/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.9.9 (2022-03-19)
+
+Add mypy error codes to `type: ignore`s, remove unused ignores (#7504)
+
+Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
+
 ## 2.9.8 (2022-02-16)
 
 Remove unused allowlist entries in `babel` and `requests` (#7233)
 
 ## 2.9.7 (2022-02-07)
 
 Improve a bunch of `__(deep)copy__` methods (#7148)
```

### Comparing `types-babel-2.9.8/PKG-INFO` & `types-babel-2.9.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-babel
-Version: 2.9.8
+Version: 2.9.9
 Summary: Typing stubs for babel
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/babel.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -18,10 +18,10 @@
 This is a PEP 561 type stub package for the `babel` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `babel`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/babel. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `1341a345258735c695892a1470ace41ca29eb6c9`.
+This package was generated from typeshed commit `1acc8f3bd645aea6b18cf15d5fca271b9c3cd785`.
```

### Comparing `types-babel-2.9.8/babel-stubs/core.pyi` & `types-babel-2.9.9/babel-stubs/core.pyi`

 * *Files identical despite different names*

### Comparing `types-babel-2.9.8/babel-stubs/dates.pyi` & `types-babel-2.9.9/babel-stubs/dates.pyi`

 * *Files identical despite different names*

### Comparing `types-babel-2.9.8/babel-stubs/localedata.pyi` & `types-babel-2.9.9/babel-stubs/localedata.pyi`

 * *Files identical despite different names*

### Comparing `types-babel-2.9.8/babel-stubs/messages/catalog.pyi` & `types-babel-2.9.9/babel-stubs/messages/catalog.pyi`

 * *Files identical despite different names*

### Comparing `types-babel-2.9.8/babel-stubs/messages/extract.pyi` & `types-babel-2.9.9/babel-stubs/messages/extract.pyi`

 * *Files identical despite different names*

### Comparing `types-babel-2.9.8/babel-stubs/messages/frontend.pyi` & `types-babel-2.9.9/babel-stubs/messages/frontend.pyi`

 * *Files identical despite different names*

### Comparing `types-babel-2.9.8/babel-stubs/messages/pofile.pyi` & `types-babel-2.9.9/babel-stubs/messages/pofile.pyi`

 * *Files identical despite different names*

### Comparing `types-babel-2.9.8/babel-stubs/numbers.pyi` & `types-babel-2.9.9/babel-stubs/numbers.pyi`

 * *Files identical despite different names*

### Comparing `types-babel-2.9.8/babel-stubs/plural.pyi` & `types-babel-2.9.9/babel-stubs/plural.pyi`

 * *Files identical despite different names*

### Comparing `types-babel-2.9.8/babel-stubs/support.pyi` & `types-babel-2.9.9/babel-stubs/support.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     def dnpgettext(self, domain, context, singular, plural, num): ...
     def udnpgettext(self, domain, context, singular, plural, num): ...
     dunpgettext: Any
     def ldnpgettext(self, domain, context, singular, plural, num): ...
     ugettext: Any
     ungettext: Any
 
-class Translations(NullTranslations, gettext.GNUTranslations):  # type: ignore # argument disparities between base classes
+class Translations(NullTranslations, gettext.GNUTranslations):
     DEFAULT_DOMAIN: str
     domain: Any
     def __init__(self, fp: Any | None = ..., domain: Any | None = ...) -> None: ...
     ugettext: Any
     ungettext: Any
     @classmethod
     def load(cls, dirname: Any | None = ..., locales: Any | None = ..., domain: Any | None = ...): ...
```

### Comparing `types-babel-2.9.8/babel-stubs/units.pyi` & `types-babel-2.9.9/babel-stubs/units.pyi`

 * *Files identical despite different names*

### Comparing `types-babel-2.9.8/babel-stubs/util.pyi` & `types-babel-2.9.9/babel-stubs/util.pyi`

 * *Files identical despite different names*

### Comparing `types-babel-2.9.8/setup.py` & `types-babel-2.9.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `babel` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `babel`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/babel. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `1341a345258735c695892a1470ace41ca29eb6c9`.
+This package was generated from typeshed commit `1acc8f3bd645aea6b18cf15d5fca271b9c3cd785`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.9.8",
+      version="2.9.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/babel.md",
```

### Comparing `types-babel-2.9.8/types_babel.egg-info/PKG-INFO` & `types-babel-2.9.9/types_babel.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-babel
-Version: 2.9.8
+Version: 2.9.9
 Summary: Typing stubs for babel
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/babel.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -18,10 +18,10 @@
 This is a PEP 561 type stub package for the `babel` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `babel`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/babel. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `1341a345258735c695892a1470ace41ca29eb6c9`.
+This package was generated from typeshed commit `1acc8f3bd645aea6b18cf15d5fca271b9c3cd785`.
```

### Comparing `types-babel-2.9.8/types_babel.egg-info/SOURCES.txt` & `types-babel-2.9.9/types_babel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

