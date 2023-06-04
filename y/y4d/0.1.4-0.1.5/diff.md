# Comparing `tmp/y4d-0.1.4.tar.gz` & `tmp/y4d-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y4d-0.1.4.tar", max compression
+gzip compressed data, was "y4d-0.1.5.tar", max compression
```

## Comparing `y4d-0.1.4.tar` & `y4d-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      580 2023-06-02 19:50:47.924343 y4d-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      217 2023-05-31 19:18:03.375800 y4d-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-27 19:23:01.005617 y4d-0.1.4/y4d/__init__.py
--rw-r--r--   0        0        0     1560 2023-06-02 19:25:50.118169 y4d-0.1.4/y4d/checkAPI.py
--rw-r--r--   0        0        0    14732 2023-06-02 19:51:03.806133 y4d-0.1.4/y4d/codeParser.py
--rw-r--r--   0        0        0     8160 2023-06-02 19:26:45.386030 y4d-0.1.4/y4d/commentController.py
--rw-r--r--   0        0        0     7354 2023-06-02 19:51:25.780979 y4d-0.1.4/y4d/isolator.py
--rw-r--r--   0        0        0    35173 2023-06-02 19:27:27.852256 y4d-0.1.4/y4d/restrictor.py
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 y4d-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      580 2023-06-04 09:29:22.882327 y4d-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      217 2023-05-31 19:18:03.375800 y4d-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 19:23:01.005617 y4d-0.1.5/y4d/__init__.py
+-rw-r--r--   0        0        0     1560 2023-06-04 09:29:35.108938 y4d-0.1.5/y4d/checkAPI.py
+-rw-r--r--   0        0        0    14921 2023-06-04 09:29:56.900945 y4d-0.1.5/y4d/codeParser.py
+-rw-r--r--   0        0        0     8160 2023-06-04 09:30:32.127907 y4d-0.1.5/y4d/commentController.py
+-rw-r--r--   0        0        0     7354 2023-06-04 09:30:48.366646 y4d-0.1.5/y4d/isolator.py
+-rw-r--r--   0        0        0    37610 2023-06-04 09:31:13.769899 y4d-0.1.5/y4d/restrictor.py
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 y4d-0.1.5/PKG-INFO
```

### Comparing `y4d-0.1.4/pyproject.toml` & `y4d-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "y4d"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["BahouA <antonbahou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 checkAPI = "y4d.checkAPI:app"
 restrict = "y4d.restrictor:app"
```

### Comparing `y4d-0.1.4/y4d/checkAPI.py` & `y4d-0.1.5/y4d/checkAPI.py`

 * *Files identical despite different names*

### Comparing `y4d-0.1.4/y4d/codeParser.py` & `y4d-0.1.5/y4d/codeParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 from pathlib import Path
 
 def findLocationFunction(data, prototype: str, source):
     #Check for static, virtual, pure virtual, and constructors
     is_static = False
     is_pure = False
     is_virtual = False
-
     #Check static functions
     if len(prototype.split("static")) > 1:
         is_static= True
+        prototype = prototype.split("static")[1]
 
     #Check virtual and pure virtual functions
     if len(prototype.split("virtual")) > 1:
         is_virtual= True
         if len( prototype.split("=0")) > 1:
             prototype = prototype.split("=0")[0]
             is_pure= True
         elif len( prototype.split("= 0")) > 1:
             prototype = prototype.split("= 0")[0]
             is_pure= True
+        prototype= prototype.split("virtual")[1]
             
     #Label function by its type 
     if len(prototype.split("template"))> 1 :
         if len(prototype.split("::")) > 1 :
             type = "template_member_function"
         else:
             type = "template_function"
@@ -34,14 +35,16 @@
         type = "member_function"
     else:
         type="function"
     #Extract information from function prototype
     if type == "member_function" or type == "template_member_function":
         parent_class = prototype.split("::")[0].strip().split(" ")[-1]
         returntype = prototype.split(parent_class)[0]
+        if type == "template_member_function":
+            returntype = returntype.split(">")[1]
         prototype=prototype.replace(" ", "")
         name = prototype.split("::")[1].split("(")[0]
         if len(name.split("~")) > 1 and name.split("~")[1] == parent_class:
             type = "decstructor"
         if name == parent_class:
             type = "constructor"   
     else:
@@ -49,15 +52,14 @@
             prototype = prototype.split(">")[1].strip()
         name = prototype.split('(')[0].split(" ")[-1].strip()
         returntype = prototype.split(name)[0].strip()
         
     if type == "constructor" or type == "decstructor":
         returntype = "void"
         params = "(" + prototype.split("::")[1].split("(")[1]
-
     else:
         params = prototype.split(name)[1]
         
     qualtype = returntype + params
     qualtype = qualtype.replace(" ", "")
 
     #Retrieve position of function
@@ -283,15 +285,14 @@
             "access_type" : access_type.lower(),
             "parent_class" : parent_class
         }
         output["nodes"].append(node_dict)
     
     jsonFormat = json.dumps(output, indent=4)
     data = json.loads(jsonFormat)
-    
     return data
 
 
 #Return postions of anything the user is searching for.
 def positions ( source: str, type: str, prototype: str, option = 0):
     source_path = Path(source)
     if source_path.exists() == False:
```

### Comparing `y4d-0.1.4/y4d/commentController.py` & `y4d-0.1.5/y4d/commentController.py`

 * *Files identical despite different names*

### Comparing `y4d-0.1.4/y4d/isolator.py` & `y4d-0.1.5/y4d/isolator.py`

 * *Files identical despite different names*

### Comparing `y4d-0.1.4/y4d/restrictor.py` & `y4d-0.1.5/y4d/restrictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -471,44 +471,48 @@
 
 
 #Function to restrict a single function, no need for the YAML file, further explanation available exactly below function definition.
 @app.command("f")
 def funcRestrict(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
                  restriction: str = typer.Argument(..., help="The restriction type used for 3 ways of checking:\n\nat_least: The function being checked must exist (It can be with other functions).\n\nexactly: The function being checked must only exist (It can not be with other functions).\n\nforbidden: The function being checked must not exist."),
                  prototype: str = typer.Argument(..., help="The function the user wants to check (Must input like this: \"int functionName(int, int)\"."),
-                 scope: str = typer.Argument(..., help="The scope the user wants to check inside (Function or Class, input their prototypes)."),
+                 scope: str = typer.Argument(..., help="The scope the user wants to check inside (Function or Class, input their prototypes, if class then no need to add class name to prototype)."),
                  hide:bool = typer.Argument(False, hidden=True, help="A hidden variable for developers use, used to return boolean")):
     """
     Checks if a certain function inputted by the user follows as certain restriction type of (at_least/exactly/forbidden) in a .cpp or .h file also inputted by the user.
     """
-
+    
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
     #Check if global scope or not, if not then use scopeGetter to get everything in the scope defined by the user
     if scope.lower() == "global" or scope == "":
         data = codeParser.prepareData(source)
         with open(source, 'r') as f:
             scopeG = f.read()
     else:
+        if len(scope.split("class ")) > 1:
+            fname = prototype.split("(")[0].split(" ")[-1].strip()
+            prototype = prototype.split(fname)[0] + scope.split("class ")[-1].strip() + "::" + fname + "(" + prototype.split("(")[-1]
         scopeG = scopeGetter(source, scope)
         if scopeG == ["error"]:
             return False
         file = open("restrictorGen.cpp", "w")
         file.write(scopeG)
         file.close()
         data = codeParser.prepareData("restrictorGen.cpp")
 
     empty = []
     #Check if function exists and print true or false according to restriction
     if codeParser.findLocationFunction(data, prototype, source) != empty:
         if restriction.lower() == "exactly":
-            if len(re.findall(r"\b[a-zA-Z_][a-zA-Z0-9_]*\s+[a-zA-Z_][a-zA-Z0-9_]*\s*\([^)]*\)\s*\{[^{}]*\}", scopeG, flags=re.MULTILINE)) > 1:
+            # if len(re.findall(r"\b[a-zA-Z_][a-zA-Z0-9_]*\s+[a-zA-Z_][a-zA-Z0-9_]*\s*\([^)]*\)\s*\{[^{}]*\}", scopeG, flags=re.MULTILINE)) > 1:
+            if len(re.findall(r"\b(?:\w+\s+)+\*?\s*\w+\s*\([^)]*\)\s*(?:const\s*)?(?:=\s*0)?(?=\s*\{)", scopeG, flags=re.MULTILINE)) > 1:
                 if not hide:
                     print("False")
                 return False
             else:
                 if not hide:
                     print("True")
                 return True
@@ -533,20 +537,21 @@
 
 
 #Function to restrict a single (private/public/protected) function, no need for the YAML file, further explanation available exactly below function definition.
 @app.command("a")
 def accessRestrict(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
                  restriction: str = typer.Argument(..., help="The restriction type used for 3 ways of checking:\n\nat_least: The function being checked must exist (It can be with other functions).\n\nexactly: The function being checked must only exist (It can not be with other functions).\n\nforbidden: The function being checked must not exist."),
                  prototype: str = typer.Argument(..., help="The function the user wants to check (Must input like this: \"int functionName(int, int)\" or \"int functionName(int x,int y)\")."),
-                 scope: str = typer.Argument(..., help="The scope the user wants to check inside (Function or Class, input their prototypes)."),
+                 scope: str = typer.Argument(..., help="The scope the user wants to check inside (Function or Class, input their prototypes, if class then no need to add class name to prototype)."),
                  type: str = typer.Argument(..., help="The access type the user wants to check for (private/public/protected)."),
                  hide:bool = typer.Argument(False, hidden=True, help="A hidden variable for developers use, used to return boolean")):
     """
     Checks if a certain (private/public/protected) function inputted by the user follows as certain restriction type of (at_least/exactly/forbidden) in a .cpp or .h file also inputted by the user.
     """
+    
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
     #Check if global scope or not, if not then use scopeGetter to get everything in the scope defined by the user as well as preparing data for access_type search
     if scope.lower() == "global" or scope == "":
@@ -556,23 +561,52 @@
         if scopeG == ["error"]:
             return False
         file = open("restrictorGen.cpp", "w")
         file.write(scopeG)
         file.close()
         data = codeParser.prepareData("restrictorGen.cpp")
 
+    unsigned = ""
+    longlong = ""
     #Variables used in the following if statement to find if function is private
+    if prototype.strip()[0:8] == "unsigned":
+        unsigned = "unsigned "
+    if len(prototype.split("long long")) > 1:
+        longlong = "long "
     if len(prototype.split("virtual")) == 1 and len(prototype.split("static")) == 1:
-        proto = prototype.split(' ')[0] + ' (' + prototype.split('(')[1].strip()
+        if unsigned == "":
+            if longlong == "":
+                proto = unsigned + longlong + prototype.split(' ')[0] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+            else:
+                proto = unsigned + longlong + prototype.split(' ')[1] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+        else:
+            if longlong == "":
+                proto = unsigned + longlong + prototype.split(' ')[1] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+            else:
+                proto = unsigned + longlong + prototype.split(' ')[2] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+        if len(proto.split("(")) > 2:
+            proto = "void ()"
     else:
-        proto = prototype.split(' ')[1] + ' (' + prototype.split('(')[1].strip()
+        if unsigned == "":
+            if longlong == "":
+                proto = unsigned + longlong + prototype.split(' ')[1] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+            else:
+                proto = unsigned + longlong + prototype.split(' ')[2] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+        else:
+            if longlong == "":
+                proto = unsigned + longlong + prototype.split(' ')[2] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+            else:
+                proto = unsigned + longlong + prototype.split(' ')[3] + ' (' + prototype.split('(')[1].strip().split("=0")[0].strip()
+
+    unsigned = ""
+    longlong = ""
     spelling = prototype.split('(')[0].split(' ')[-1].split('::')[-1]
     
     for decl in data['nodes']:
-        if decl['kind'] == "CXX_METHOD" and decl['spelling'] == spelling and decl['prototype'].replace(" ","") == proto.replace(" ","") and decl['access_type'] == type.lower():
+        if (decl['kind'] == "CXX_METHOD" or decl['kind'] == "CONSTRUCTOR" or decl['kind'] == "DESTRUCTOR") and decl['spelling'] == spelling and decl['prototype'].replace(" ","") == proto.replace(" ","") and decl['access_type'] == type.lower():
             return funcRestrict(source, restriction, prototype, scope, hide)
     if not hide:
         print("False")
     return False
 
 
 
@@ -602,43 +636,53 @@
     allPublicFunctions =[]
     allProtectedFunctions = []
     allFunctions = []
     allClasses = []
     virtual = ""
     const = ""
     unsigned = ""
+    pure = ""
+    static = ""
     for decl in data['nodes']:
         if decl['prototype'].split(' ')[0] == "unsigned":
             unsigned = " " + decl['prototype'].split(' ')[1]
         else:
             unsigned = ""
         if decl['kind'] == "CXX_METHOD":
+            if decl['is_pure'] == True:
+                pure = "=0"
+            else:
+                pure = ""
+            if decl['is_static_method'] == True:
+                static = "static "
+            else:
+                static = ""
             if decl['is_virtual_method'] == True:
                 virtual = "virtual "
             else:
                 virtual = ""
             if decl['is_const_method'] == True:
                 const = " const"
             else:
                 const = ""
             if decl['access_type'] == "":
-                allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " " + decl['displayname'] + const)
+                allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " " + decl['displayname'] + const + pure)
             elif decl['access_type'] == 'private':
-                allPrivFunctions.append(virtual + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const)
+                allPrivFunctions.append(virtual + static + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const + pure)
             elif decl['access_type'] == 'public':
-                allPublicFunctions.append(virtual + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const)
+                allPublicFunctions.append(virtual + static + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const + pure)
             elif decl['access_type'] == 'protected':
-                allProtectedFunctions.append(virtual + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const )
+                allProtectedFunctions.append(virtual + static + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const + pure)
         elif decl['kind'] == "FUNCTION_DECL":
             if len(decl['prototype'].split('(')[0].split('**')) == 1 and len(decl['prototype'].split('(')[0].split('*')) == 1:
-                allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " " + decl['displayname'] + const)
+                allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " " + decl['displayname'] + const + pure)
             elif len(decl['prototype'].split('**')) > 1:
-                allFunctions.append(decl['prototype'].split('**')[0] + unsigned + "** " + decl['displayname'] + const)
+                allFunctions.append(decl['prototype'].split('**')[0] + unsigned + "** " + decl['displayname'] + const + pure)
             else:
-                allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " * " + decl['displayname' + const])
+                allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " * " + decl['displayname' + const] + pure)
         if decl['kind'] == "CLASS_DECL":
             allClasses.append("class " + decl['prototype'])
     
     #Write the YAML file
     file_yaml = {'classes': {'restriction': f'{restriction}', 'scope': 'global', 'names': list(set(allClasses))}, 'functions': {'restriction': f'{restriction}', 'scope': 'global', 'names': list(set(allFunctions))}, 'public_functions': {'restriction': f'{restriction}', 'scope': 'global', 'names': list(set(allPublicFunctions))}, 'private_functions': {'restriction': f'{restriction}', 'scope': 'global', 'names': list(set(allPrivFunctions))}, 'protected_functions': {'restriction': f'{restriction}', 'scope': 'global', 'names': list(set(allProtectedFunctions))}}
     with open("checkAPI.yaml", 'w') as file:
         yaml.dump(file_yaml, file)
```

### Comparing `y4d-0.1.4/PKG-INFO` & `y4d-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y4d
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: BahouA
 Author-email: antonbahou@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

