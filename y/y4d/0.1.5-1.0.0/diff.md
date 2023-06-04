# Comparing `tmp/y4d-0.1.5.tar.gz` & `tmp/y4d-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y4d-0.1.5.tar", max compression
+gzip compressed data, was "y4d-1.0.0.tar", max compression
```

## Comparing `y4d-0.1.5.tar` & `y4d-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      580 2023-06-04 09:29:22.882327 y4d-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      217 2023-05-31 19:18:03.375800 y4d-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-27 19:23:01.005617 y4d-0.1.5/y4d/__init__.py
--rw-r--r--   0        0        0     1560 2023-06-04 09:29:35.108938 y4d-0.1.5/y4d/checkAPI.py
--rw-r--r--   0        0        0    14921 2023-06-04 09:29:56.900945 y4d-0.1.5/y4d/codeParser.py
--rw-r--r--   0        0        0     8160 2023-06-04 09:30:32.127907 y4d-0.1.5/y4d/commentController.py
--rw-r--r--   0        0        0     7354 2023-06-04 09:30:48.366646 y4d-0.1.5/y4d/isolator.py
--rw-r--r--   0        0        0    37610 2023-06-04 09:31:13.769899 y4d-0.1.5/y4d/restrictor.py
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 y4d-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      580 2023-06-04 20:49:26.041105 y4d-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      217 2023-05-31 19:18:03.375800 y4d-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 19:23:01.005617 y4d-1.0.0/y4d/__init__.py
+-rw-r--r--   0        0        0     1560 2023-06-04 09:29:35.108938 y4d-1.0.0/y4d/checkAPI.py
+-rw-r--r--   0        0        0    14921 2023-06-04 09:29:56.900945 y4d-1.0.0/y4d/codeParser.py
+-rw-r--r--   0        0        0     8160 2023-06-04 09:30:32.127907 y4d-1.0.0/y4d/commentController.py
+-rw-r--r--   0        0        0     7354 2023-06-04 09:30:48.366646 y4d-1.0.0/y4d/isolator.py
+-rw-r--r--   0        0        0    38388 2023-06-04 20:49:49.930586 y4d-1.0.0/y4d/restrictor.py
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 y4d-1.0.0/PKG-INFO
```

### Comparing `y4d-0.1.5/pyproject.toml` & `y4d-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "y4d"
-version = "0.1.5"
+version = "1.0.0"
 description = ""
 authors = ["BahouA <antonbahou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 checkAPI = "y4d.checkAPI:app"
 restrict = "y4d.restrictor:app"
```

### Comparing `y4d-0.1.5/y4d/checkAPI.py` & `y4d-1.0.0/y4d/checkAPI.py`

 * *Files identical despite different names*

### Comparing `y4d-0.1.5/y4d/codeParser.py` & `y4d-1.0.0/y4d/codeParser.py`

 * *Files identical despite different names*

### Comparing `y4d-0.1.5/y4d/commentController.py` & `y4d-1.0.0/y4d/commentController.py`

 * *Files identical despite different names*

### Comparing `y4d-0.1.5/y4d/isolator.py` & `y4d-1.0.0/y4d/isolator.py`

 * *Files identical despite different names*

### Comparing `y4d-0.1.5/y4d/restrictor.py` & `y4d-1.0.0/y4d/restrictor.py`

 * *Files 5% similar despite different names*

```diff
@@ -563,43 +563,56 @@
         file = open("restrictorGen.cpp", "w")
         file.write(scopeG)
         file.close()
         data = codeParser.prepareData("restrictorGen.cpp")
 
     unsigned = ""
     longlong = ""
+    point = ""
     #Variables used in the following if statement to find if function is private
     if prototype.strip()[0:8] == "unsigned":
         unsigned = "unsigned "
     if len(prototype.split("long long")) > 1:
         longlong = "long "
     if len(prototype.split("virtual")) == 1 and len(prototype.split("static")) == 1:
+        if len(prototype.split("(")[0].split("**")) > 1:
+            point = " **"
+        elif len(prototype.split("(")[0].split("*")) > 1:
+            point = " *"
+        else:
+            point = ""
         if unsigned == "":
             if longlong == "":
-                proto = unsigned + longlong + prototype.split(' ')[0] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+                proto = unsigned + longlong + prototype.split(' ')[0] + point + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
             else:
-                proto = unsigned + longlong + prototype.split(' ')[1] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+                proto = unsigned + longlong + prototype.split(' ')[1] + point + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
         else:
             if longlong == "":
-                proto = unsigned + longlong + prototype.split(' ')[1] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+                proto = unsigned + longlong + prototype.split(' ')[1] + point + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
             else:
-                proto = unsigned + longlong + prototype.split(' ')[2] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+                proto = unsigned + longlong + prototype.split(' ')[2] + point + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
         if len(proto.split("(")) > 2:
             proto = "void ()"
     else:
+        if len(prototype.split("(")[0].split("**")) > 1:
+            point = " **"
+        elif len(prototype.split("(")[0].split("*")) > 1:
+            point = " *"
+        else:
+            point = ""
         if unsigned == "":
             if longlong == "":
-                proto = unsigned + longlong + prototype.split(' ')[1] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+                proto = unsigned + longlong + prototype.split(' ')[1] + point + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
             else:
-                proto = unsigned + longlong + prototype.split(' ')[2] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+                proto = unsigned + longlong + prototype.split(' ')[2] + point + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
         else:
             if longlong == "":
-                proto = unsigned + longlong + prototype.split(' ')[2] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+                proto = unsigned + longlong + prototype.split(' ')[2] + point+ ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
             else:
-                proto = unsigned + longlong + prototype.split(' ')[3] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+                proto = unsigned + longlong + prototype.split(' ')[3] + point + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
 
     unsigned = ""
     longlong = ""
     spelling = prototype.split('(')[0].split(' ')[-1].split('::')[-1]
     
     for decl in data['nodes']:
         if (decl['kind'] == "CXX_METHOD" or decl['kind'] == "CONSTRUCTOR" or decl['kind'] == "DESTRUCTOR") and decl['spelling'] == spelling and decl['prototype'].replace(" ","") == proto.replace(" ","") and decl['access_type'] == type.lower():
@@ -619,15 +632,15 @@
     """
     Compares two files together, the source and compare file, it will check if the function prototypes and class names match then return true or false accordingly.
     """
     #Used to control the style of output
     if output not in ["n", "N", "V", "v"]:
         print("Invalid -o input")
         return False
-
+    
     data = codeParser.prepareData(compare)
 
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
@@ -638,14 +651,15 @@
     allFunctions = []
     allClasses = []
     virtual = ""
     const = ""
     unsigned = ""
     pure = ""
     static = ""
+    point = " "
     for decl in data['nodes']:
         if decl['prototype'].split(' ')[0] == "unsigned":
             unsigned = " " + decl['prototype'].split(' ')[1]
         else:
             unsigned = ""
         if decl['kind'] == "CXX_METHOD":
             if decl['is_pure'] == True:
@@ -660,22 +674,28 @@
                 virtual = "virtual "
             else:
                 virtual = ""
             if decl['is_const_method'] == True:
                 const = " const"
             else:
                 const = ""
+            if len(decl['prototype'].split("(")[0].split('**')) > 1:
+                point = " ** "
+            elif len(decl['prototype'].split("(")[0].split('*')) > 1:
+                point = " * "
+            else:
+                point = " "
             if decl['access_type'] == "":
-                allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " " + decl['displayname'] + const + pure)
+                allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + point + decl['displayname'] + const + pure)
             elif decl['access_type'] == 'private':
-                allPrivFunctions.append(virtual + static + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const + pure)
+                allPrivFunctions.append(virtual + static + decl['prototype'].split(' ')[0] + unsigned + point + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const + pure)
             elif decl['access_type'] == 'public':
-                allPublicFunctions.append(virtual + static + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const + pure)
+                allPublicFunctions.append(virtual + static + decl['prototype'].split(' ')[0] + unsigned + point + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const + pure)
             elif decl['access_type'] == 'protected':
-                allProtectedFunctions.append(virtual + static + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const + pure)
+                allProtectedFunctions.append(virtual + static + decl['prototype'].split(' ')[0] + unsigned + point + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const + pure)
         elif decl['kind'] == "FUNCTION_DECL":
             if len(decl['prototype'].split('(')[0].split('**')) == 1 and len(decl['prototype'].split('(')[0].split('*')) == 1:
                 allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " " + decl['displayname'] + const + pure)
             elif len(decl['prototype'].split('**')) > 1:
                 allFunctions.append(decl['prototype'].split('**')[0] + unsigned + "** " + decl['displayname'] + const + pure)
             else:
                 allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " * " + decl['displayname' + const] + pure)
```

### Comparing `y4d-0.1.5/PKG-INFO` & `y4d-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y4d
-Version: 0.1.5
+Version: 1.0.0
 Summary: 
 Author: BahouA
 Author-email: antonbahou@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

