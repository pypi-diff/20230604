# Comparing `tmp/django_jsheet-0.2.0.tar.gz` & `tmp/django_jsheet-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_jsheet-0.2.0.tar", last modified: Thu Apr  6 09:32:16 2023, max compression
+gzip compressed data, was "django_jsheet-0.2.1.tar", last modified: Sun Jun  4 14:14:41 2023, max compression
```

## Comparing `django_jsheet-0.2.0.tar` & `django_jsheet-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-04-06 09:32:16.900966 django_jsheet-0.2.0/
--rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-04-02 11:32:45.000000 django_jsheet-0.2.0/LICENSE
--rw-r--r--   0 shadmod    (501) admin       (80)     1153 2023-04-06 09:32:16.900466 django_jsheet-0.2.0/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      176 2023-04-05 21:03:08.000000 django_jsheet-0.2.0/README.md
--rw-r--r--   0 shadmod    (501) admin       (80)     1085 2023-04-05 22:48:00.000000 django_jsheet-0.2.0/pyproject.toml
--rw-r--r--   0 shadmod    (501) admin       (80)       38 2023-04-06 09:32:16.901102 django_jsheet-0.2.0/setup.cfg
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-04-06 09:32:16.891602 django_jsheet-0.2.0/src/
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-04-06 09:32:16.894656 django_jsheet-0.2.0/src/django_jsheet/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-04-02 09:53:41.000000 django_jsheet-0.2.0/src/django_jsheet/__init__.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-04-06 09:32:16.898113 django_jsheet-0.2.0/src/django_jsheet/core/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-04-02 09:53:41.000000 django_jsheet-0.2.0/src/django_jsheet/core/__init__.py
--rw-r--r--   0 shadmod    (501) admin       (80)    10692 2023-04-05 22:40:28.000000 django_jsheet-0.2.0/src/django_jsheet/core/django_sheet.py
--rw-r--r--   0 shadmod    (501) admin       (80)       88 2023-04-05 21:00:16.000000 django_jsheet-0.2.0/src/django_jsheet/core/forms.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-04-06 09:32:16.899410 django_jsheet-0.2.0/src/django_jsheet/templatetags/
--rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-03-06 19:49:48.000000 django_jsheet-0.2.0/src/django_jsheet/templatetags/__init__.py
--rw-r--r--   0 shadmod    (501) admin       (80)     5753 2023-04-05 22:38:08.000000 django_jsheet-0.2.0/src/django_jsheet/templatetags/jsheet.py
-drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-04-06 09:32:16.896364 django_jsheet-0.2.0/src/django_jsheet.egg-info/
--rw-r--r--   0 shadmod    (501) admin       (80)     1153 2023-04-06 09:32:16.000000 django_jsheet-0.2.0/src/django_jsheet.egg-info/PKG-INFO
--rw-r--r--   0 shadmod    (501) admin       (80)      416 2023-04-06 09:32:16.000000 django_jsheet-0.2.0/src/django_jsheet.egg-info/SOURCES.txt
--rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-04-06 09:32:16.000000 django_jsheet-0.2.0/src/django_jsheet.egg-info/dependency_links.txt
--rw-r--r--   0 shadmod    (501) admin       (80)       14 2023-04-06 09:32:16.000000 django_jsheet-0.2.0/src/django_jsheet.egg-info/top_level.txt
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:14:41.245387 django_jsheet-0.2.1/
+-rw-r--r--   0 shadmod    (501) admin       (80)     1064 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/LICENSE
+-rw-r--r--   0 shadmod    (501) admin       (80)     1408 2023-06-04 14:14:41.245041 django_jsheet-0.2.1/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      334 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/README.md
+-rw-r--r--   0 shadmod    (501) admin       (80)     1116 2023-06-04 14:07:25.000000 django_jsheet-0.2.1/pyproject.toml
+-rw-r--r--   0 shadmod    (501) admin       (80)       38 2023-06-04 14:14:41.245564 django_jsheet-0.2.1/setup.cfg
+-rw-r--r--   0 shadmod    (501) admin       (80)      871 2023-06-04 14:08:17.000000 django_jsheet-0.2.1/setup.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:14:41.237861 django_jsheet-0.2.1/src/
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:14:41.240732 django_jsheet-0.2.1/src/core/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/src/core/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)    10692 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/src/core/django_sheet.py
+-rw-r--r--   0 shadmod    (501) admin       (80)    10675 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/src/core/views.py
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:14:41.243516 django_jsheet-0.2.1/src/django_jsheet.egg-info/
+-rw-r--r--   0 shadmod    (501) admin       (80)     1408 2023-06-04 14:14:41.000000 django_jsheet-0.2.1/src/django_jsheet.egg-info/PKG-INFO
+-rw-r--r--   0 shadmod    (501) admin       (80)      325 2023-06-04 14:14:41.000000 django_jsheet-0.2.1/src/django_jsheet.egg-info/SOURCES.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)        1 2023-06-04 14:14:41.000000 django_jsheet-0.2.1/src/django_jsheet.egg-info/dependency_links.txt
+-rw-r--r--   0 shadmod    (501) admin       (80)       18 2023-06-04 14:14:41.000000 django_jsheet-0.2.1/src/django_jsheet.egg-info/top_level.txt
+drwxr-xr-x   0 shadmod    (501) admin       (80)        0 2023-06-04 14:14:41.244191 django_jsheet-0.2.1/src/templatetags/
+-rw-r--r--   0 shadmod    (501) admin       (80)        0 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/src/templatetags/__init__.py
+-rw-r--r--   0 shadmod    (501) admin       (80)     4553 2023-06-04 13:25:07.000000 django_jsheet-0.2.1/src/templatetags/jsheet.py
```

### Comparing `django_jsheet-0.2.0/LICENSE` & `django_jsheet-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_jsheet-0.2.0/PKG-INFO` & `django_jsheet-0.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: django_jsheet
-Version: 0.2.0
-Summary: A small example package
-Author-email: ShadMod <support@shadmod.it>
-Maintainer-email: Brett Cannon <brett@python.org>
+Version: 0.2.1
+Summary: A little tool to render a simple excel sheet in webpage
+Home-page: https://github.com/shadMod/django-jsheet
+Author: shadMod
+Author-email: shadMod <support@shadmod.it>
+Maintainer-email: ShadMod <support@shadmod.it>
 License: MIT License
 Project-URL: Homepage, https://github.com/shadMod/django-jsheet
 Project-URL: Bug Tracker, https://github.com/shadMod/django-jsheet/issues
 Keywords: Django JSheet,Django-JSheet,Django_JSheet
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,10 +24,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django JSheet
 
 Django JSheet is a little tool to render a simple excel sheet in webpage
 
+A sheet is generated with all the data and its history.
+
+No model is required, but you can eventually add it to allows synchronization of data with the db
+
 There are many around, but mine is cooler because it's made by me .-.
 
-Good luck! \o/
+Good luck! \o/``
```

### Comparing `django_jsheet-0.2.0/pyproject.toml` & `django_jsheet-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
+
 [project]
 name = "django_jsheet"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
-    { name = "ShadMod", email = "support@shadmod.it" },
+    { name = "shadMod", email = "support@shadmod.it" },
 ]
 maintainers = [
-    { name = "Brett Cannon", email = "brett@python.org" }
+    { name = "ShadMod", email = "support@shadmod.it" },
 ]
-description = "A small example package"
+description = "A little tool to render a simple excel sheet in webpage"
 readme = "README.md"
 keywords = [
     "Django JSheet",
     "Django-JSheet",
     "Django_JSheet",
 ]
 license = { text = "MIT License" }
```

### Comparing `django_jsheet-0.2.0/src/django_jsheet/core/django_sheet.py` & `django_jsheet-0.2.1/src/core/django_sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
                 <script type="text/javascript">
                     var clm_len = document.getElementById('id_jsheet').rows[0].cells.length;
             """
             # get number row and init row_v and append value clean
             js_script += """
                     row_%s.addEventListener("input", function (e) {
                         var row_v = [];
-                        for (var i = 0; i < 6; i++) {
+                        for (var i = 0; i < 5; i++) {
                             row_v.push(this.getElementsByTagName('input')[i].value)
                         } 
             """ % i
             # insert model and choice value
             js_script += """ 
                         row_v.splice(1, 0, document.getElementById('User{0}').value.toString())
                         row_v.splice(5, 0, document.getElementById('InvoiceReceiptTypology{0}').value)
```

### Comparing `django_jsheet-0.2.0/src/django_jsheet/templatetags/jsheet.py` & `django_jsheet-0.2.1/src/templatetags/jsheet.py`

 * *Files 24% similar despite different names*

```diff
@@ -130,38 +130,7 @@
     
     {js_script}
     {jsfooter}
     """.format(
         style=CSS_STYLE, thead=thead, tbody=tbody, js_script=js_script, jsfooter=jsfooter,
     )
     return mark_safe(table)
-
-
-def js_script_row(n_row, start: int = 0):
-    js_script = ""
-    for i in range(start, n_row):
-        # init scripts
-        js_script += """
-            <script type="text/javascript">
-                var clm_len = document.getElementById('id_jsheet').rows[0].cells.length;
-        """
-        # get number row and init row_v and append value clean
-        js_script += """
-                row_%s.addEventListener("input", function (e) {
-                    var row_v = [];
-                    for (var i = 0; i < 6; i++) {
-                        row_v.push(this.getElementsByTagName('input')[i].value)
-                    } 
-        """ % i
-        # insert model value
-        js_script += """ 
-                    row_v.splice(1, 0, document.getElementById('User{0}').value.toString())
-                    row_v.splice(5, 0, document.getElementById('InvoiceReceiptTypology{0}').value)
-                    row_v.splice(6, 0, document.getElementById('PaymentMethod{0}').value)
-        """.format(i)
-        # run update_rows to send request POST
-        js_script += """
-                    update_rows(row_v, %s);
-                });
-            </script>
-        """ % i
-    return js_script
```

### Comparing `django_jsheet-0.2.0/src/django_jsheet.egg-info/PKG-INFO` & `django_jsheet-0.2.1/src/django_jsheet.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: django-jsheet
-Version: 0.2.0
-Summary: A small example package
-Author-email: ShadMod <support@shadmod.it>
-Maintainer-email: Brett Cannon <brett@python.org>
+Version: 0.2.1
+Summary: A little tool to render a simple excel sheet in webpage
+Home-page: https://github.com/shadMod/django-jsheet
+Author: shadMod
+Author-email: shadMod <support@shadmod.it>
+Maintainer-email: ShadMod <support@shadmod.it>
 License: MIT License
 Project-URL: Homepage, https://github.com/shadMod/django-jsheet
 Project-URL: Bug Tracker, https://github.com/shadMod/django-jsheet/issues
 Keywords: Django JSheet,Django-JSheet,Django_JSheet
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,10 +24,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django JSheet
 
 Django JSheet is a little tool to render a simple excel sheet in webpage
 
+A sheet is generated with all the data and its history.
+
+No model is required, but you can eventually add it to allows synchronization of data with the db
+
 There are many around, but mine is cooler because it's made by me .-.
 
-Good luck! \o/
+Good luck! \o/``
```

