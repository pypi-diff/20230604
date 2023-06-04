# Comparing `tmp/nodered.py-0.2.2.tar.gz` & `tmp/nodered.py-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.2.2.tar", last modified: Fri Jun  2 06:36:41 2023, max compression
+gzip compressed data, was "nodered.py-0.2.3.tar", last modified: Sun Jun  4 00:46:33 2023, max compression
```

## Comparing `nodered.py-0.2.2.tar` & `nodered.py-0.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-02 06:36:41.180000 nodered.py-0.2.2/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.2/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-06-02 06:36:41.310000 nodered.py-0.2.2/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2026 2023-05-10 10:48:39.000000 nodered.py-0.2.2/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-02 06:36:41.180000 nodered.py-0.2.2/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-06-02 06:36:41.000000 nodered.py-0.2.2/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-06-02 06:36:41.000000 nodered.py-0.2.2/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-06-02 06:36:41.000000 nodered.py-0.2.2/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       14 2023-06-02 06:36:41.000000 nodered.py-0.2.2/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-06-02 06:36:41.000000 nodered.py-0.2.2/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.2/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-02 06:36:41.180000 nodered.py-0.2.2/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      403 2023-06-02 04:28:48.000000 nodered.py-0.2.2/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    12724 2023-06-02 06:29:12.000000 nodered.py-0.2.2/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4006 2023-05-02 10:42:51.000000 nodered.py-0.2.2/noderedpy/_property.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-02 06:36:41.180000 nodered.py-0.2.2/noderedpy/assets/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.2/noderedpy/assets/python-logo.png
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.2/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-02 06:36:41.190000 nodered.py-0.2.2/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.2/noderedpy/node-red-starter/editorTheme.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3396 2023-06-02 06:24:22.000000 nodered.py-0.2.2/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-06-02 04:29:58.000000 nodered.py-0.2.2/noderedpy/node-red-starter/package.json
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-02 06:36:41.230000 nodered.py-0.2.2/noderedpy/templates/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7985 2023-05-10 10:44:33.000000 nodered.py-0.2.2/noderedpy/templates/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.2/noderedpy/templates/template.html
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3766 2023-05-07 11:55:40.000000 nodered.py-0.2.2/noderedpy/templates/template.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.2/noderedpy/templates/template.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-06-02 06:36:41.310000 nodered.py-0.2.2/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.2/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-04 00:46:33.410000 nodered.py-0.2.3/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.3/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-06-04 00:46:33.500000 nodered.py-0.2.3/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2026 2023-05-10 10:48:39.000000 nodered.py-0.2.3/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-04 00:46:33.410000 nodered.py-0.2.3/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-06-04 00:46:33.000000 nodered.py-0.2.3/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-06-04 00:46:33.000000 nodered.py-0.2.3/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-06-04 00:46:33.000000 nodered.py-0.2.3/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       14 2023-06-04 00:46:33.000000 nodered.py-0.2.3/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-06-04 00:46:33.000000 nodered.py-0.2.3/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.3/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-04 00:46:33.410000 nodered.py-0.2.3/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      403 2023-06-04 00:16:07.000000 nodered.py-0.2.3/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    13016 2023-06-04 00:19:59.000000 nodered.py-0.2.3/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4006 2023-05-02 10:42:51.000000 nodered.py-0.2.3/noderedpy/_property.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-04 00:46:33.410000 nodered.py-0.2.3/noderedpy/assets/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.3/noderedpy/assets/python-logo.png
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.3/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-04 00:46:33.420000 nodered.py-0.2.3/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.3/noderedpy/node-red-starter/editorTheme.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1589 2023-06-04 00:34:19.000000 nodered.py-0.2.3/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-06-02 04:29:58.000000 nodered.py-0.2.3/noderedpy/node-red-starter/package.json
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-06-04 00:46:33.420000 nodered.py-0.2.3/noderedpy/templates/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7985 2023-05-10 10:44:33.000000 nodered.py-0.2.3/noderedpy/templates/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.3/noderedpy/templates/template.html
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3766 2023-05-07 11:55:40.000000 nodered.py-0.2.3/noderedpy/templates/template.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.3/noderedpy/templates/template.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-06-04 00:46:33.500000 nodered.py-0.2.3/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.3/setup.py
```

### Comparing `nodered.py-0.2.2/LICENSE` & `nodered.py-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.2/PKG-INFO` & `nodered.py-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.2
+Version: 0.2.3
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.2 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.3 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
```

### Comparing `nodered.py-0.2.2/README.md` & `nodered.py-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.2/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.2.3/nodered.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.2
+Version: 0.2.3
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.2 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.3 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
```

### Comparing `nodered.py-0.2.2/nodered.py.egg-info/SOURCES.txt` & `nodered.py-0.2.3/nodered.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.2/noderedpy/_nodered.py` & `nodered.py-0.2.3/noderedpy/_nodered.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,28 +20,31 @@
 
         Parameters
         ----------
         user_dir: str, required
             userDir of Node-RED settings
         node_red_dir: str, default None
             directory for Node-RED starter
-        admin_root: str, default "node-red-py"
+        admin_root: str, default "/node-red-py"
             httpAdminRoot of Node-RED settings
         port: int, default 1880
             port of Node-RED server
         show_default_category: bool, default True
             show default categories of Node-RED or not
         editor_theme: dict, default {}
             editorTheme of Node-RED server (for detail information, see https://github.com/node-red/node-red/wiki/Design:-Editor-Themes)
         auths: List[dict], default []
             auth list for Node-RED
         """
         self.user_dir, self.admin_root, self.port, self.show_default_category, self.editor_theme =\
             user_dir, admin_root, port, show_default_category, self.__default_editor_theme(editor_theme)
         
+        if not self.admin_root.startswith("/"):
+            self.admin_root = f"/{self.admin_root}"
+
         self.node_auths = self.__default_node_auth(auths)
         
         # set node_red_dir
         if node_red_dir is None:
             self.node_red_dir = os.path.join(__path__[0], "node-red-starter")
         else:
             self.node_red_dir = node_red_dir = os.path.realpath(node_red_dir)
@@ -156,15 +159,15 @@
                         pass
 
                 node = list(filter(lambda n: n.name == input_data["name"], RED.registered_nodes))[0]
 
                 with open(output_file, "w", encoding = "utf-8") as ofw:
                     json.dump(node.run(input_data["props"], input_data["msg"]), ofw, indent = 4)
 
-    def start(self, debug:bool = True, callback:MethodType = None):
+    def start(self, callback:MethodType = None, debug:bool = True, start_browser:bool = True):
         """
         Start Node-RED server
 
         Parameters
         ----------
         debug: bool, default True
             show outputs on console or not
@@ -215,14 +218,18 @@
         subprocess.Popen([
             "node",
             "index.js"
         ], shell = False, stdout = sys.stdout if debug else subprocess.DEVNULL, cwd = self.node_red_dir)
 
         while True:
             if os.path.exists(self.__started_file):
+                if start_browser:
+                    import webbrowser
+                    webbrowser.open_new(f"http://127.0.0.1:{self.port}{self.admin_root}")
+
                 if callback:
                     callback()
 
                 break
 
         try:
             self.__check_input_from_node()
```

### Comparing `nodered.py-0.2.2/noderedpy/_property.py` & `nodered.py-0.2.3/noderedpy/_property.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.2/noderedpy/assets/python-logo.png` & `nodered.py-0.2.3/noderedpy/assets/python-logo.png`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.2/noderedpy/decorator.py` & `nodered.py-0.2.3/noderedpy/decorator.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.2/noderedpy/templates/__init__.py` & `nodered.py-0.2.3/noderedpy/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.2/noderedpy/templates/template.html` & `nodered.py-0.2.3/noderedpy/templates/template.html`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.2/noderedpy/templates/template.js` & `nodered.py-0.2.3/noderedpy/templates/template.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.2/setup.py` & `nodered.py-0.2.3/setup.py`

 * *Files identical despite different names*

