# Comparing `tmp/webint_editor-0.0.168.tar.gz` & `tmp/webint_editor-0.0.169.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_editor-0.0.168.tar", max compression
+gzip compressed data, was "webint_editor-0.0.169.tar", max compression
```

## Comparing `webint_editor-0.0.168.tar` & `webint_editor-0.0.169.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      892 2023-06-04 02:10:00.327299 webint_editor-0.0.168/pyproject.toml
--rw-r--r--   0        0        0     5180 2023-06-04 01:57:48.120671 webint_editor-0.0.168/webint_editor/__init__.py
--rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.168/webint_editor/templates/__init__.py
--rw-r--r--   0        0        0    17369 2023-06-04 02:09:58.051266 webint_editor-0.0.168/webint_editor/templates/draft.html
--rw-r--r--   0        0        0       44 2023-03-08 03:45:25.484536 webint_editor-0.0.168/webint_editor/templates/editor.html
--rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.168/webint_editor/templates/template.html
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.168/setup.py
--rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.168/PKG-INFO
+-rw-r--r--   0        0        0      892 2023-06-04 02:50:28.678207 webint_editor-0.0.169/pyproject.toml
+-rw-r--r--   0        0        0     5180 2023-06-04 01:57:48.120671 webint_editor-0.0.169/webint_editor/__init__.py
+-rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.169/webint_editor/templates/__init__.py
+-rw-r--r--   0        0        0    17489 2023-06-04 02:50:26.314178 webint_editor-0.0.169/webint_editor/templates/draft.html
+-rw-r--r--   0        0        0       44 2023-03-08 03:45:25.484536 webint_editor-0.0.169/webint_editor/templates/editor.html
+-rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.169/webint_editor/templates/template.html
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.169/setup.py
+-rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.169/PKG-INFO
```

### Comparing `webint_editor-0.0.168/pyproject.toml` & `webint_editor-0.0.169/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-editor"
-version = "0.0.168"
+version = "0.0.169"
 description = "Edit posts on your website"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "AGPL-3.0-or-later"
 keywords = ["Micropub"]
 packages = [{include="webint_editor"}]
 
 [tool.poetry.plugins.webapps]
```

### Comparing `webint_editor-0.0.168/webint_editor/__init__.py` & `webint_editor-0.0.169/webint_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `webint_editor-0.0.168/webint_editor/templates/draft.html` & `webint_editor-0.0.169/webint_editor/templates/draft.html`

 * *Files 2% similar despite different names*

```diff
@@ -91,21 +91,23 @@
             $if (not type and _type == "entry") or _type == type:
                 checked
             $else:
                 disabled
             > $_type</label>
         </fieldset>
     </div>
-    <div id=card_properties>
-        <div id=name>
-            <label><small>Name</small><br>
-            <label class=bounding><input type=text name=name
-            value="$get_property('name')"></label></label>
-        </div>
-    </div>
+
+    $# <div id=card_properties>
+    $#     <div id=name>
+    $#         <label><small>Name</small><br>
+    $#         <label class=bounding><input type=text name=name
+    $#         value="$get_property('name')"></label></label>
+    $#     </div>
+    $# </div>
+
     <div id=entry_properties>
         <div id=in_reply_to>
             <label><small>In reply to</small><br>
             <label class=bounding><input type=text name=in_reply_to
             value="$get_property('in-reply-to')"></label></label>
         </div>
         <div id=rsvp>
@@ -159,45 +161,48 @@
             <iframe src="$tx.origin/pads/p/$pad_id"
                 frameborder=0 style=height:30em;width:100%></iframe>
             </label></label>
             $# XXX <div id=connection></div>
             $# XXX <div id=version></div>
         </div>
     </div>
-    <div id=event_properties>
-        <div id=name>
-            <label><small>Name</small><br>
-            <label class=bounding><input type=text name=name
-            value="$get_property('name')"></label></label>
-        </div>
-    </div>
-    <div id=resume_properties>
-        <div id=name>
-            <label><small>Name</small><br>
-            <label class=bounding><input type=text name=name
-            value="$get_property('name')"></label></label>
-        </div>
-    </div>
-    <div id=review_properties>
-        <div id=name>
-            <label><small>Name</small><br>
-            <label class=bounding><input type=text name=name
-            value="$get_property('name')"></label></label>
-        </div>
-    </div>
+
+    $# <div id=event_properties>
+    $#     <div id=name>
+    $#         <label><small>Name</small><br>
+    $#         <label class=bounding><input type=text name=name
+    $#         value="$get_property('name')"></label></label>
+    $#     </div>
+    $# </div>
+    $# <div id=resume_properties>
+    $#     <div id=name>
+    $#         <label><small>Name</small><br>
+    $#         <label class=bounding><input type=text name=name
+    $#         value="$get_property('name')"></label></label>
+    $#     </div>
+    $# </div>
+    $# <div id=review_properties>
+    $#     <div id=name>
+    $#         <label><small>Name</small><br>
+    $#         <label class=bounding><input type=text name=name
+    $#         value="$get_property('name')"></label></label>
+    $#     </div>
+    $# </div>
+
     $# <fieldset id=categories>
     $#   <legend>Categories</legend>
     $#   <!-- XXX todo populate with call to mp?q=config as with channels -->
     $#   <input type=text><button>Add</button>
     $#   <ul>
     $#   $# $for category in c
     $#   $#     <li><input type=checkbox id=coding name=category value=coding>
     $#   $#     <label for=coding>Coding</label></li>
     $#   </ul>
     $# </fieldset>
+
     $if published := get_property("published"):
         <div id=published>
         <label for=published><small>Published</small></label><br>
         <input style="border:1px solid #333" type=datetime-local name=published_datetime
         value="$published.to_date_string()T$published.to_time_string()">
         <input style="font-family:monospace;font-size:.9em;border:1px solid #333;width:10em" type=text name=published_microseconds
         value="$published.microsecond">
@@ -219,14 +224,15 @@
         <button name=action value=update>Update</button>
         $# $else:
         $#     <button name=action value=create>Create</button>
     </div>
 </form>
 
 $if post:
+    <h4>Unused properties</h4>
     <pre>$pformat(post)</pre>
 
 <style>
 form#editor {
   column-gap: 2%;
   display: grid;
   grid-template-columns: 49% 49%; }
```

### Comparing `webint_editor-0.0.168/setup.py` & `webint_editor-0.0.169/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['webint>=0.0']
 
 entry_points = \
 {'webapps': ['editor = webint_editor:app']}
 
 setup_kwargs = {
     'name': 'webint-editor',
-    'version': '0.0.168',
+    'version': '0.0.169',
     'description': 'Edit posts on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

