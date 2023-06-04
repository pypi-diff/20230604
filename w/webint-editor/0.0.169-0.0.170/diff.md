# Comparing `tmp/webint_editor-0.0.169.tar.gz` & `tmp/webint_editor-0.0.170.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_editor-0.0.169.tar", max compression
+gzip compressed data, was "webint_editor-0.0.170.tar", max compression
```

## Comparing `webint_editor-0.0.169.tar` & `webint_editor-0.0.170.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      892 2023-06-04 02:50:28.678207 webint_editor-0.0.169/pyproject.toml
--rw-r--r--   0        0        0     5180 2023-06-04 01:57:48.120671 webint_editor-0.0.169/webint_editor/__init__.py
--rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.169/webint_editor/templates/__init__.py
--rw-r--r--   0        0        0    17489 2023-06-04 02:50:26.314178 webint_editor-0.0.169/webint_editor/templates/draft.html
--rw-r--r--   0        0        0       44 2023-03-08 03:45:25.484536 webint_editor-0.0.169/webint_editor/templates/editor.html
--rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.169/webint_editor/templates/template.html
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.169/setup.py
--rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.169/PKG-INFO
+-rw-r--r--   0        0        0      892 2023-06-04 02:55:53.666426 webint_editor-0.0.170/pyproject.toml
+-rw-r--r--   0        0        0     5180 2023-06-04 01:57:48.120671 webint_editor-0.0.170/webint_editor/__init__.py
+-rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.170/webint_editor/templates/__init__.py
+-rw-r--r--   0        0        0    17501 2023-06-04 02:55:51.470396 webint_editor-0.0.170/webint_editor/templates/draft.html
+-rw-r--r--   0        0        0       44 2023-03-08 03:45:25.484536 webint_editor-0.0.170/webint_editor/templates/editor.html
+-rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.170/webint_editor/templates/template.html
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.170/setup.py
+-rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.170/PKG-INFO
```

### Comparing `webint_editor-0.0.169/pyproject.toml` & `webint_editor-0.0.170/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-editor"
-version = "0.0.169"
+version = "0.0.170"
 description = "Edit posts on your website"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "AGPL-3.0-or-later"
 keywords = ["Micropub"]
 packages = [{include="webint_editor"}]
 
 [tool.poetry.plugins.webapps]
```

### Comparing `webint_editor-0.0.169/webint_editor/__init__.py` & `webint_editor-0.0.170/webint_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `webint_editor-0.0.169/webint_editor/templates/draft.html` & `webint_editor-0.0.170/webint_editor/templates/draft.html`

 * *Files 1% similar despite different names*

```diff
@@ -290,18 +290,18 @@
 <script type=module>
 // XXX import { load, diamondMonaco, MicropubClient } from '/static/web.js'
 import { load, MicropubClient } from '/static/web.js'
 
 const pub = new MicropubClient('/posts')
 
 load(() => {
-  document.querySelector('#card_properties').style.display = 'none'
-  document.querySelector('#event_properties').style.display = 'none'
-  document.querySelector('#resume_properties').style.display = 'none'
-  document.querySelector('#review_properties').style.display = 'none'
+  // document.querySelector('#card_properties').style.display = 'none'
+  // document.querySelector('#event_properties').style.display = 'none'
+  // document.querySelector('#resume_properties').style.display = 'none'
+  // document.querySelector('#review_properties').style.display = 'none'
   const enlivenOptionalProperty = (type, property) => {
     const textbox = document.querySelector(`#$${type}_properties #$${property} .bounding`)
     textbox.style.display = 'none'
     const checkbox = document.createElement('input')
     checkbox.type = 'checkbox'
     checkbox.addEventListener('click', ev => {
       textbox.style.display = ev.target.checked ? 'block' : 'none'
```

### Comparing `webint_editor-0.0.169/setup.py` & `webint_editor-0.0.170/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['webint>=0.0']
 
 entry_points = \
 {'webapps': ['editor = webint_editor:app']}
 
 setup_kwargs = {
     'name': 'webint-editor',
-    'version': '0.0.169',
+    'version': '0.0.170',
     'description': 'Edit posts on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

