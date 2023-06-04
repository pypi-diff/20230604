# Comparing `tmp/webint_editor-0.0.164.tar.gz` & `tmp/webint_editor-0.0.165.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_editor-0.0.164.tar", max compression
+gzip compressed data, was "webint_editor-0.0.165.tar", max compression
```

## Comparing `webint_editor-0.0.164.tar` & `webint_editor-0.0.165.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      892 2023-06-03 07:32:40.607071 webint_editor-0.0.164/pyproject.toml
--rw-r--r--   0        0        0     4929 2023-06-03 02:55:47.150152 webint_editor-0.0.164/webint_editor/__init__.py
--rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.164/webint_editor/templates/__init__.py
--rw-r--r--   0        0        0    17470 2023-06-03 07:32:37.555040 webint_editor-0.0.164/webint_editor/templates/draft.html
--rw-r--r--   0        0        0       44 2023-03-08 03:45:25.484536 webint_editor-0.0.164/webint_editor/templates/editor.html
--rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.164/webint_editor/templates/template.html
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.164/setup.py
--rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.164/PKG-INFO
+-rw-r--r--   0        0        0      892 2023-06-03 07:34:05.720006 webint_editor-0.0.165/pyproject.toml
+-rw-r--r--   0        0        0     4929 2023-06-03 02:55:47.150152 webint_editor-0.0.165/webint_editor/__init__.py
+-rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.165/webint_editor/templates/__init__.py
+-rw-r--r--   0        0        0    17468 2023-06-03 07:34:02.335967 webint_editor-0.0.165/webint_editor/templates/draft.html
+-rw-r--r--   0        0        0       44 2023-03-08 03:45:25.484536 webint_editor-0.0.165/webint_editor/templates/editor.html
+-rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.165/webint_editor/templates/template.html
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.165/setup.py
+-rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.165/PKG-INFO
```

### Comparing `webint_editor-0.0.164/pyproject.toml` & `webint_editor-0.0.165/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-editor"
-version = "0.0.164"
+version = "0.0.165"
 description = "Edit posts on your website"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "AGPL-3.0-or-later"
 keywords = ["Micropub"]
 packages = [{include="webint_editor"}]
 
 [tool.poetry.plugins.webapps]
```

### Comparing `webint_editor-0.0.164/webint_editor/__init__.py` & `webint_editor-0.0.165/webint_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `webint_editor-0.0.164/webint_editor/templates/draft.html` & `webint_editor-0.0.165/webint_editor/templates/draft.html`

 * *Files 0% similar despite different names*

```diff
@@ -328,23 +328,23 @@
   }
 
   var frequency = 1;  // seconds
   var count = 0;
   var clean = true;
   const tick = () => {
     setTimeout(() => {
-      if (count++ > frequency * 10) // && !clean)
+      if (count++ > frequency * 5) // && !clean)
         updatePreview();
       tick();
     }, 1000);
   }
   tick();
   const updatePreview = () => {
     clean = false;
-    if (count > frequency * 10) {
+    if (count > frequency * 5) {
       previewMarkdown(getContent());
       clean = true;
       count = 0;
     }
   }
   updatePreview()
```

### Comparing `webint_editor-0.0.164/setup.py` & `webint_editor-0.0.165/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['webint>=0.0']
 
 entry_points = \
 {'webapps': ['editor = webint_editor:app']}
 
 setup_kwargs = {
     'name': 'webint-editor',
-    'version': '0.0.164',
+    'version': '0.0.165',
     'description': 'Edit posts on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

