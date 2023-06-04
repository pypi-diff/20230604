# Comparing `tmp/juno-ai-0.0.6.tar.gz` & `tmp/juno-ai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juno-ai-0.0.6.tar", last modified: Wed May 31 03:47:19 2023, max compression
+gzip compressed data, was "juno-ai-0.0.7.tar", last modified: Sun Jun  4 15:49:27 2023, max compression
```

## Comparing `juno-ai-0.0.6.tar` & `juno-ai-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-05-31 03:47:19.941022 juno-ai-0.0.6/
--rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-05-31 03:47:19.940720 juno-ai-0.0.6/PKG-INFO
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1938 2023-05-26 07:12:21.000000 juno-ai-0.0.6/README.md
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-05-31 03:47:19.937719 juno-ai-0.0.6/juno/
--rw-r--r--   0 alexirobbins   (501) staff       (20)       58 2023-04-09 05:43:26.000000 juno-ai-0.0.6/juno/__init__.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1002 2023-05-24 08:38:40.000000 juno-ai-0.0.6/juno/agent_injection.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1253 2023-04-16 22:35:57.000000 juno-ai-0.0.6/juno/client_setup.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1916 2023-05-26 07:12:21.000000 juno-ai-0.0.6/juno/event_javascript.py
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-05-31 03:47:19.938329 juno-ai-0.0.6/juno/js/
--rw-r--r--   0 alexirobbins   (501) staff       (20)    15888 2023-05-26 06:26:51.000000 juno-ai-0.0.6/juno/js/juno.min.js
--rw-r--r--   0 alexirobbins   (501) staff       (20)     2723 2023-05-24 08:38:40.000000 juno-ai-0.0.6/juno/juno.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1984 2023-05-11 01:35:57.000000 juno-ai-0.0.6/juno/magic.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)      873 2023-03-31 21:04:15.000000 juno-ai-0.0.6/juno/output_parser.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)    14035 2023-05-26 06:26:51.000000 juno-ai-0.0.6/juno/prompting_javascript.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     4685 2023-04-26 23:26:15.000000 juno-ai-0.0.6/juno/serialize_context.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)      473 2023-05-26 07:12:21.000000 juno-ai-0.0.6/juno/version.py
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-05-31 03:47:19.940336 juno-ai-0.0.6/juno_ai.egg-info/
--rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-05-31 03:47:19.000000 juno-ai-0.0.6/juno_ai.egg-info/PKG-INFO
--rw-r--r--   0 alexirobbins   (501) staff       (20)      399 2023-05-31 03:47:19.000000 juno-ai-0.0.6/juno_ai.egg-info/SOURCES.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)        1 2023-05-31 03:47:19.000000 juno-ai-0.0.6/juno_ai.egg-info/dependency_links.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)       53 2023-05-31 03:47:19.000000 juno-ai-0.0.6/juno_ai.egg-info/requires.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)        5 2023-05-31 03:47:19.000000 juno-ai-0.0.6/juno_ai.egg-info/top_level.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)       38 2023-05-31 03:47:19.941100 juno-ai-0.0.6/setup.cfg
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1322 2023-05-31 03:46:36.000000 juno-ai-0.0.6/setup.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-06-04 15:49:27.249196 juno-ai-0.0.7/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-06-04 15:49:27.248873 juno-ai-0.0.7/PKG-INFO
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1938 2023-05-26 07:12:21.000000 juno-ai-0.0.7/README.md
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-06-04 15:49:27.246071 juno-ai-0.0.7/juno/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       58 2023-04-09 05:43:26.000000 juno-ai-0.0.7/juno/__init__.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1002 2023-05-24 08:38:40.000000 juno-ai-0.0.7/juno/agent_injection.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1253 2023-04-16 22:35:57.000000 juno-ai-0.0.7/juno/client_setup.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1916 2023-05-26 07:12:21.000000 juno-ai-0.0.7/juno/event_javascript.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-06-04 15:49:27.246666 juno-ai-0.0.7/juno/js/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)    15808 2023-06-04 15:46:16.000000 juno-ai-0.0.7/juno/js/juno.min.js
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     2723 2023-05-24 08:38:40.000000 juno-ai-0.0.7/juno/juno.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1984 2023-05-11 01:35:57.000000 juno-ai-0.0.7/juno/magic.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      873 2023-03-31 21:04:15.000000 juno-ai-0.0.7/juno/output_parser.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)    14065 2023-06-04 15:46:04.000000 juno-ai-0.0.7/juno/prompting_javascript.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     4685 2023-04-26 23:26:15.000000 juno-ai-0.0.7/juno/serialize_context.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      473 2023-05-26 07:12:21.000000 juno-ai-0.0.7/juno/version.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-06-04 15:49:27.248507 juno-ai-0.0.7/juno_ai.egg-info/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-06-04 15:49:27.000000 juno-ai-0.0.7/juno_ai.egg-info/PKG-INFO
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      399 2023-06-04 15:49:27.000000 juno-ai-0.0.7/juno_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)        1 2023-06-04 15:49:27.000000 juno-ai-0.0.7/juno_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       53 2023-06-04 15:49:27.000000 juno-ai-0.0.7/juno_ai.egg-info/requires.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)        5 2023-06-04 15:49:27.000000 juno-ai-0.0.7/juno_ai.egg-info/top_level.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       38 2023-06-04 15:49:27.249282 juno-ai-0.0.7/setup.cfg
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1322 2023-06-04 15:46:04.000000 juno-ai-0.0.7/setup.py
```

### Comparing `juno-ai-0.0.6/PKG-INFO` & `juno-ai-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juno-ai
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/alexi/juno
 Author: juno
 Author-email: hellojunoai@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `juno-ai-0.0.6/README.md` & `juno-ai-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.6/juno/agent_injection.py` & `juno-ai-0.0.7/juno/agent_injection.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.6/juno/client_setup.py` & `juno-ai-0.0.7/juno/client_setup.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.6/juno/event_javascript.py` & `juno-ai-0.0.7/juno/event_javascript.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.6/juno/js/juno.min.js` & `juno-ai-0.0.7/juno/js/juno.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -393,15 +393,15 @@
                 removeFixButton: c
             } = e("./handlers.js");
         class d {
             constructor() {
                 this.initialized = !1, this.initialize()
             }
             initialize() {
-                this.initialized || (this.juno_url = "https://getjuno.ai/", this.api_endpoint = "http://127.0.0.1:8000/", r(), this.agent_manager = new o, this.edit_zones = new l, this._listen(), this.initialized = !0)
+                this.initialized || (this.juno_url = "https://getjuno.ai/", this.api_endpoint = "https://api.getjuno.ai/", r(), this.agent_manager = new o, this.edit_zones = new l, this._listen(), this.initialized = !0)
             }
             cleanDebugButtons(e) {
                 var t, n;
                 for ([t, n] of Jupyter.notebook.get_cells().entries()) {
                     var o = i.cellHasErrorOutput(n) && !this.edit_zones.isEditCell(n);
                     o ? a(n, t) : e || o || c(n)
                 }
@@ -425,15 +425,15 @@
                     setTimeout(() => s(this.edit_zones), 150), setTimeout(() => s(this.edit_zones), 400)
                 }), setInterval(() => s(this.edit_zones), 3e3), setInterval(() => this.cleanDebugButtons(!0), 3e3), Jupyter.notebook.events.on("delete.Cell", (e, t) => this.edit_zones.handleDeleteCell(t.cell)), s(this.edit_zones), setTimeout(() => s(this.edit_zones), 600)
             }
             openEditor(t, e = !1) {
                 var n = Jupyter.notebook.get_cells().find(e => e.cell_id == t);
                 this.edit_zones.createZone(n, e)
             }
-        }(e = window).juno ? e.juno.initialized || e.juno.initialize() : (e.juno = new d, e.juno_url = "https://getjuno.ai/", e.juno_api_endpoint = "https://api.getjuno.ai/")
+        }(e = window).juno ? e.juno.initialized || e.juno.initialize() : e.juno = new d
     }, {
         "./agent.js": 1,
         "./handlers.js": 2,
         "./utils.js": 4
     }],
     4: [function(e, t, n) {
         async function i(e, t) {
```

### Comparing `juno-ai-0.0.6/juno/juno.py` & `juno-ai-0.0.7/juno/juno.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.6/juno/magic.py` & `juno-ai-0.0.7/juno/magic.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.6/juno/output_parser.py` & `juno-ai-0.0.7/juno/output_parser.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.6/juno/prompting_javascript.py` & `juno-ai-0.0.7/juno/prompting_javascript.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,25 +123,25 @@
     }}
     
     source.onerror = (e) => {{
       console.log("handling error fetching", e);
       if(e.status == 402) {{
           console.log("opening signup page")
           setTimeout(() => {{
-              window.open(window.juno_url + 'signup', '_blank');
+              window.open(window.juno.juno_url + 'signup', '_blank');
           }}, 10);
           // get selected cell
           let cell = Jupyter.notebook.get_selected_cell();
           // print login prompt below cell
           let outputArea = cell.output_area;
           let junoInfo = document.createElement("div");
           junoInfo.id = "juno-info";
           junoInfo.style = "margin-left: 114px; margin-top: 10px; margin-bottom: 10px; padding: 10px; border: 1px solid #e6e6e6; border-radius: 3px; background-color: #f9f9f9; font-size: 12px; color: #666;";
           // list the commands juno can run with explanations
-          junoInfo.innerHTML = "Please <a href='" + window.juno_url + "signup' target='_blank'>signup</a> or <a href='" + window.juno_url + "login' target='_blank'>login</a> to continue using Juno"
+          junoInfo.innerHTML = "Please <a href='" + window.juno.juno_url + "signup' target='_blank'>signup</a> or <a href='" + window.juno.juno_url + "login' target='_blank'>login</a> to continue using Juno"
           outputArea.element.append(junoInfo);
       }}
     }}
     
     if (doneCallback !== undefined) {{
         doneCallback();
     }}
@@ -190,24 +190,24 @@
             }}
         }},
         onError(e) {{
             console.log("handling error fetching", e);
             if(e.status == 402) {{
                 console.log("opening signup page")
                 setTimeout(() => {{
-                    window.open(window.juno_url + 'signup', '_blank');
+                    window.open(window.juno.juno_url + 'signup', '_blank');
                 }}, 10);
                 // get selected cell
                 let cell = Jupyter.notebook.get_selected_cell();
                 // print login prompt below cell
                 let outputArea = cell.output_area;
                 let junoInfo = document.createElement("div");
                 junoInfo.id = "juno-login-info";
                 junoInfo.style = "margin-left: 114px; margin-top: 10px; margin-bottom: 10px; padding: 10px; border: 1px solid #e6e6e6; border-radius: 3px; background-color: #f9f9f9; font-size: 12px; color: #666;";
-                junoInfo.innerHTML = "Please <a href='" + window.juno_url + "signup' target='_blank'>signup</a> or <a href='" + window.juno_url + "login' target='_blank'>login</a> to continue using Juno"
+                junoInfo.innerHTML = "Please <a href='" + window.juno.juno_url + "signup' target='_blank'>signup</a> or <a href='" + window.juno.juno_url + "login' target='_blank'>login</a> to continue using Juno"
                 // add text input form for user to enter api key and call localStorage.setItem("api_key", api_key) on submit
                 outputArea.element.append(junoInfo);
             }}
         }}
     }});
 }}
```

### Comparing `juno-ai-0.0.6/juno/serialize_context.py` & `juno-ai-0.0.7/juno/serialize_context.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.6/juno_ai.egg-info/PKG-INFO` & `juno-ai-0.0.7/juno_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juno-ai
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/alexi/juno
 Author: juno
 Author-email: hellojunoai@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `juno-ai-0.0.6/setup.py` & `juno-ai-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # exec(open(read('juno/version.py')).read())
 print('packages:', [package for package in find_packages()
                 if package.startswith('juno')])
 setup(
     name='juno-ai', 
     # version=__version__, 
-    version='0.0.6',
+    version='0.0.7',
     packages=[package for package in find_packages()
                 if package.startswith('juno')], 
     package_data={'': ['js/juno.min.js']},
     include_package_data=True,
     long_description='Juno AI Assistant for Jupyter Notebook',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
```

