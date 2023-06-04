# Comparing `tmp/webint_editor-0.0.167.tar.gz` & `tmp/webint_editor-0.0.168.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_editor-0.0.167.tar", max compression
+gzip compressed data, was "webint_editor-0.0.168.tar", max compression
```

## Comparing `webint_editor-0.0.167.tar` & `webint_editor-0.0.168.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      892 2023-06-04 02:09:08.990552 webint_editor-0.0.167/pyproject.toml
--rw-r--r--   0        0        0     5180 2023-06-04 01:57:48.120671 webint_editor-0.0.167/webint_editor/__init__.py
--rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.167/webint_editor/templates/__init__.py
--rw-r--r--   0        0        0    17370 2023-06-04 02:09:07.138525 webint_editor-0.0.167/webint_editor/templates/draft.html
--rw-r--r--   0        0        0       44 2023-03-08 03:45:25.484536 webint_editor-0.0.167/webint_editor/templates/editor.html
--rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.167/webint_editor/templates/template.html
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.167/setup.py
--rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.167/PKG-INFO
+-rw-r--r--   0        0        0      892 2023-06-04 02:10:00.327299 webint_editor-0.0.168/pyproject.toml
+-rw-r--r--   0        0        0     5180 2023-06-04 01:57:48.120671 webint_editor-0.0.168/webint_editor/__init__.py
+-rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.168/webint_editor/templates/__init__.py
+-rw-r--r--   0        0        0    17369 2023-06-04 02:09:58.051266 webint_editor-0.0.168/webint_editor/templates/draft.html
+-rw-r--r--   0        0        0       44 2023-03-08 03:45:25.484536 webint_editor-0.0.168/webint_editor/templates/editor.html
+-rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.168/webint_editor/templates/template.html
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.168/setup.py
+-rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.168/PKG-INFO
```

### Comparing `webint_editor-0.0.167/pyproject.toml` & `webint_editor-0.0.168/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-editor"
-version = "0.0.167"
+version = "0.0.168"
 description = "Edit posts on your website"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "AGPL-3.0-or-later"
 keywords = ["Micropub"]
 packages = [{include="webint_editor"}]
 
 [tool.poetry.plugins.webapps]
```

### Comparing `webint_editor-0.0.167/webint_editor/__init__.py` & `webint_editor-0.0.168/webint_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `webint_editor-0.0.167/webint_editor/templates/draft.html` & `webint_editor-0.0.168/webint_editor/templates/draft.html`

 * *Files 1% similar despite different names*

```diff
@@ -223,17 +223,17 @@
 </form>
 
 $if post:
     <pre>$pformat(post)</pre>
 
 <style>
 form#editor {
-  column-gap: 2em;
+  column-gap: 2%;
   display: grid;
-  grid-template-columns: 50% 50%; }
+  grid-template-columns: 49% 49%; }
 form#editor input[type=text], textarea {
   background-color: #ddd;
   border: 0;
   padding: 0;
   width: 100%; }
 form#editor textarea {
   height: 20em;
```

### Comparing `webint_editor-0.0.167/setup.py` & `webint_editor-0.0.168/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['webint>=0.0']
 
 entry_points = \
 {'webapps': ['editor = webint_editor:app']}
 
 setup_kwargs = {
     'name': 'webint-editor',
-    'version': '0.0.167',
+    'version': '0.0.168',
     'description': 'Edit posts on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

