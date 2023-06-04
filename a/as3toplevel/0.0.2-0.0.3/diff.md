# Comparing `tmp/as3toplevel-0.0.2.tar.gz` & `tmp/as3toplevel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "as3toplevel-0.0.2.tar", last modified: Wed May 31 20:32:03 2023, max compression
+gzip compressed data, was "as3toplevel-0.0.3.tar", last modified: Sun Jun  4 14:20:13 2023, max compression
```

## Comparing `as3toplevel-0.0.2.tar` & `as3toplevel-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ajdel     (1000) ajdel     (1000)        0 2023-05-31 20:32:03.038374 as3toplevel-0.0.2/
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     1069 2023-05-26 23:44:21.000000 as3toplevel-0.0.2/LICENSE
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       42 2023-05-27 00:52:01.000000 as3toplevel-0.0.2/MANIFEST.in
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     6251 2023-05-31 20:32:03.038374 as3toplevel-0.0.2/PKG-INFO
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     5707 2023-05-31 20:25:51.000000 as3toplevel-0.0.2/README.md
-drwxrwxr-x   0 ajdel     (1000) ajdel     (1000)        0 2023-05-31 20:32:03.038374 as3toplevel-0.0.2/as3toplevel.egg-info/
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     6251 2023-05-31 20:32:03.000000 as3toplevel-0.0.2/as3toplevel.egg-info/PKG-INFO
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)      252 2023-05-31 20:32:03.000000 as3toplevel-0.0.2/as3toplevel.egg-info/SOURCES.txt
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)        1 2023-05-31 20:32:03.000000 as3toplevel-0.0.2/as3toplevel.egg-info/dependency_links.txt
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)        6 2023-05-31 20:32:03.000000 as3toplevel-0.0.2/as3toplevel.egg-info/requires.txt
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       12 2023-05-31 20:32:03.000000 as3toplevel-0.0.2/as3toplevel.egg-info/top_level.txt
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)    41067 2023-05-31 20:25:22.000000 as3toplevel-0.0.2/as3toplevel.py
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       99 2023-05-27 00:14:36.000000 as3toplevel-0.0.2/pyproject.toml
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       73 2023-05-31 20:32:03.042374 as3toplevel-0.0.2/setup.cfg
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)      868 2023-05-30 22:11:06.000000 as3toplevel-0.0.2/setup.py
+drwxrwxr-x   0 ajdel     (1000) ajdel     (1000)        0 2023-06-04 14:20:13.558708 as3toplevel-0.0.3/
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     1069 2023-05-26 23:44:21.000000 as3toplevel-0.0.3/LICENSE
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       42 2023-05-27 00:52:01.000000 as3toplevel-0.0.3/MANIFEST.in
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     6672 2023-06-04 14:20:13.558708 as3toplevel-0.0.3/PKG-INFO
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     6128 2023-06-04 14:11:36.000000 as3toplevel-0.0.3/README.md
+drwxrwxr-x   0 ajdel     (1000) ajdel     (1000)        0 2023-06-04 14:20:13.558708 as3toplevel-0.0.3/as3toplevel.egg-info/
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     6672 2023-06-04 14:20:13.000000 as3toplevel-0.0.3/as3toplevel.egg-info/PKG-INFO
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)      252 2023-06-04 14:20:13.000000 as3toplevel-0.0.3/as3toplevel.egg-info/SOURCES.txt
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)        1 2023-06-04 14:20:13.000000 as3toplevel-0.0.3/as3toplevel.egg-info/dependency_links.txt
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)        6 2023-06-04 14:20:13.000000 as3toplevel-0.0.3/as3toplevel.egg-info/requires.txt
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       12 2023-06-04 14:20:13.000000 as3toplevel-0.0.3/as3toplevel.egg-info/top_level.txt
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)    46028 2023-06-04 14:09:38.000000 as3toplevel-0.0.3/as3toplevel.py
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       99 2023-05-27 00:14:36.000000 as3toplevel-0.0.3/pyproject.toml
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       73 2023-06-04 14:20:13.558708 as3toplevel-0.0.3/setup.cfg
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)      868 2023-06-03 20:31:04.000000 as3toplevel-0.0.3/setup.py
```

### Comparing `as3toplevel-0.0.2/LICENSE` & `as3toplevel-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `as3toplevel-0.0.2/PKG-INFO` & `as3toplevel-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,16 @@
-Metadata-Version: 2.1
-Name: as3toplevel
-Version: 0.0.2
-Summary: Python implementation of the ActionScript3 toplevel
-Home-page: https://github.com/ajdelguidice/python-as3toplevel
-Author: ajdelguidice
-Author-email: ajdelguidice@gmail.com
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # python-as3toplevel
 A python implementation of some of the ActionScript3 toplevel functions and classes. They are as close as I could get them with my knowledge and the very limited documentation that adobe provides.
 <br><br>The types (Array, Boolean, Number, and String) are actual types so you can use them as such. They include almost everything that they did in ActionScript3. The length method in each type can only be used to get the length, I didn't implement the length assignment for Arrays.
 <br><br>Most of the inherited properties would be too hard to implement so I didn't bother with them.
 <br><br>I implemented the type conversion functions inside the types themselves (ex: instead of String(expression) use String.String(expression)).
 <br><br>For functions that needed a placeholder value for input(s) that aren't easily definable, could be multiple types, or relied on other factors to be set I use an empty dictionary as a placeholder. The values that these empty dictionaries represent aren't actually dictionaries, I just used something that would never be used in these functions so that I could detect it.
 <br><br>I have no way as of current to test the accuracy of these functions as I can't find a compiler for actionscript that I could get to work so if anything doesn't work or there is undocumented functionality please let me know on the github page.
 <br><br>
 # Currently Implemented
-<br>isFinite
-<br>isNaN
 <br>ArgumentError(Error Class)
 <br>Array(Function) - Moved to Array.Array()
 <br>Array(Data Type)
 <br>&emsp;Array(Constructor) - Create from values moved to class init function, create to size moved to toSize(Function).
 <br>&emsp;length(Property) - Moved to length(Function). Length assignment functionality not implemented yet
 <br>&emsp;concat(Function)
 <br>&emsp;every(Function)
@@ -52,18 +34,21 @@
 <br>&emsp;unshift(Function)
 <br>Boolean(Function) - Moved to Boolean.Boolean()
 <br>Boolean(Data Type) - Data representation changed from "true" and "false" to "True" and "False"
 <br>&emsp;Boolean(Constructor) - Moved to class init function
 <br>&emsp;toString(Function)
 <br>&emsp;valueOf(Function)
 <br>DefinitionError(Error Class)
-<br>escape(Function)
 <br>Error(Error Class)
 <br>EvalError(Error Class)
 <br>int(Data Type) - Moved to Int
+<br>&emsp;toExponential(Function)
+<br>&emsp;toFixed(Function)
+<br>isFinite(Function)
+<br>isNaN(Function)
 <br>valueOf(Function)
 <br><br>Math(Class) - All functions in this class had corresponding functions in python
 <br>&emsp;E(Constant)
 <br>&emsp;LN10(Constant)
 <br>&emsp;LN2(Constant)
 <br>&emsp;LOG10E(Constant)
 <br>&emsp;LOG2E(Constant)
@@ -87,15 +72,14 @@
 <br>&emsp;round(Function)
 <br>&emsp;sin(Function)
 <br>&emsp;sqrt(Function)
 <br>&emsp;tan(Function)
 <br>Number(Function) - Moved to Number.Number()
 <br>Number(Data Type)
 <br>&emsp;Number(Constructor) - Moved to class init function
-<br>&emsp;toFixed(Function)
 <br>&emsp;valueOf(Function)
 <br>RangeError(Error Class)
 <br>ReferenceError(Error Class)
 <br>SecurityError(Error Class)
 <br>String(Function) - Moved to String.String()
 <br>String(Data Type)
 <br>&emsp;String(Constructor) - Moved to class init function
@@ -109,57 +93,63 @@
 <br>&emsp;toLocaleLowerCase(Function)
 <br>&emsp;toLocaleUpperCase(Function)
 <br>&emsp;toLowerCase(Function)
 <br>&emsp;toUpperCase(Function)
 <br>&emsp;valueOf(Function)
 <br>SyntaxError(Error Class)
 <br>TypeError(Error Class)
-<br>unescape(Function)
 <br>URIError(Error Class)
 <br>VerifyError(Error Class)
 <br><br>
 # Partially Implemented
+<br>Date(Data Type)
+<br>escape(Function)
 <br>Number(Data Type)
 <br>&emsp;toString(Function)
 <br>int(Data Type)
-<br>&emsp;toString(Function)
-<br>trace(Function)
+<br>&emsp;toString(Function) - Don't know what is supposed to happen when radix is outside of the given range (not documented)
+<br>Number(Data Type)
+<br>&emsp;toExponential(Function)
+<br>String(Data Type)
+<br>&emsp;substr(Function) - Don't know what happens when startIndex is outside of string (not documented)
+<br>trace(Function) - Don't know how to accept which file to write to (not documented)
+<br>unescape(Function)
 <br><br>
 # Future Plans
 <br>Array(Data Type)
 <br>&emsp;sort(Function)
 <br>&emsp;sortOn(Function)
+<br>Date(Function)
+<br>Date(Data Type)
 <br>decodeURI(Function)
 <br>decodeURIComponent(Function)
 <br>encodeURI(Function)
 <br>encodeURIComponent(Function)
 <br>int(Function)
 <br>int(Data Type)
-<br>&emsp;toExponential(Function)
-<br>&emsp;toFixed(Function)
 <br>&emsp;toPrecision(Function)
 <br>RegExp(Data Type)
 <br>Number(Data Type)
 <br>&emsp;toExponential(Function)
+<br>&emsp;toFixed(Function)
 <br>&emsp;toPrecision(Function)
 <br>&emsp;toString(Function)
 <br>parseFloat(Function)
 <br>parseInt(Function)
 <br>String(Data Type)
 <br>&emsp;localeCompare(Function)
 <br>&emsp;match(Function)
 <br>&emsp;replace(Function)
 <br>&emsp;search(Function)
 <br>&emsp;slice(Function)
 <br>&emsp;split(Function)
-<br>&emsp;substr(Function)
 <br>uint(Function)
 <br>uint(Data Type)
 <br>Vector(Function)
 <br>Vector(Data Type)
 <br><br>
 # Functions I added
-<br>listtoarray - converts a given list to an Array.
+<br>listtoarray - converts a given list to an Array. Returns the Array.
 <br>Array.toSize - Creates an Array to specified size. If nothing is specified, assumes 0 elements
 <br>Number dunder methods int, float, add, sub, mul, truediv
 <br>escapeFullConvert - converts all characters to URL-encoded format
```

### Comparing `as3toplevel-0.0.2/README.md` & `as3toplevel-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,32 @@
+Metadata-Version: 2.1
+Name: as3toplevel
+Version: 0.0.3
+Summary: Python implementation of the ActionScript3 toplevel
+Home-page: https://github.com/ajdelguidice/python-as3toplevel
+Author: ajdelguidice
+Author-email: ajdelguidice@gmail.com
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Utilities
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # python-as3toplevel
 A python implementation of some of the ActionScript3 toplevel functions and classes. They are as close as I could get them with my knowledge and the very limited documentation that adobe provides.
 <br><br>The types (Array, Boolean, Number, and String) are actual types so you can use them as such. They include almost everything that they did in ActionScript3. The length method in each type can only be used to get the length, I didn't implement the length assignment for Arrays.
 <br><br>Most of the inherited properties would be too hard to implement so I didn't bother with them.
 <br><br>I implemented the type conversion functions inside the types themselves (ex: instead of String(expression) use String.String(expression)).
 <br><br>For functions that needed a placeholder value for input(s) that aren't easily definable, could be multiple types, or relied on other factors to be set I use an empty dictionary as a placeholder. The values that these empty dictionaries represent aren't actually dictionaries, I just used something that would never be used in these functions so that I could detect it.
 <br><br>I have no way as of current to test the accuracy of these functions as I can't find a compiler for actionscript that I could get to work so if anything doesn't work or there is undocumented functionality please let me know on the github page.
 <br><br>
 # Currently Implemented
-<br>isFinite
-<br>isNaN
 <br>ArgumentError(Error Class)
 <br>Array(Function) - Moved to Array.Array()
 <br>Array(Data Type)
 <br>&emsp;Array(Constructor) - Create from values moved to class init function, create to size moved to toSize(Function).
 <br>&emsp;length(Property) - Moved to length(Function). Length assignment functionality not implemented yet
 <br>&emsp;concat(Function)
 <br>&emsp;every(Function)
@@ -36,18 +50,21 @@
 <br>&emsp;unshift(Function)
 <br>Boolean(Function) - Moved to Boolean.Boolean()
 <br>Boolean(Data Type) - Data representation changed from "true" and "false" to "True" and "False"
 <br>&emsp;Boolean(Constructor) - Moved to class init function
 <br>&emsp;toString(Function)
 <br>&emsp;valueOf(Function)
 <br>DefinitionError(Error Class)
-<br>escape(Function)
 <br>Error(Error Class)
 <br>EvalError(Error Class)
 <br>int(Data Type) - Moved to Int
+<br>&emsp;toExponential(Function)
+<br>&emsp;toFixed(Function)
+<br>isFinite(Function)
+<br>isNaN(Function)
 <br>valueOf(Function)
 <br><br>Math(Class) - All functions in this class had corresponding functions in python
 <br>&emsp;E(Constant)
 <br>&emsp;LN10(Constant)
 <br>&emsp;LN2(Constant)
 <br>&emsp;LOG10E(Constant)
 <br>&emsp;LOG2E(Constant)
@@ -71,15 +88,14 @@
 <br>&emsp;round(Function)
 <br>&emsp;sin(Function)
 <br>&emsp;sqrt(Function)
 <br>&emsp;tan(Function)
 <br>Number(Function) - Moved to Number.Number()
 <br>Number(Data Type)
 <br>&emsp;Number(Constructor) - Moved to class init function
-<br>&emsp;toFixed(Function)
 <br>&emsp;valueOf(Function)
 <br>RangeError(Error Class)
 <br>ReferenceError(Error Class)
 <br>SecurityError(Error Class)
 <br>String(Function) - Moved to String.String()
 <br>String(Data Type)
 <br>&emsp;String(Constructor) - Moved to class init function
@@ -93,57 +109,63 @@
 <br>&emsp;toLocaleLowerCase(Function)
 <br>&emsp;toLocaleUpperCase(Function)
 <br>&emsp;toLowerCase(Function)
 <br>&emsp;toUpperCase(Function)
 <br>&emsp;valueOf(Function)
 <br>SyntaxError(Error Class)
 <br>TypeError(Error Class)
-<br>unescape(Function)
 <br>URIError(Error Class)
 <br>VerifyError(Error Class)
 <br><br>
 # Partially Implemented
+<br>Date(Data Type)
+<br>escape(Function)
 <br>Number(Data Type)
 <br>&emsp;toString(Function)
 <br>int(Data Type)
-<br>&emsp;toString(Function)
-<br>trace(Function)
+<br>&emsp;toString(Function) - Don't know what is supposed to happen when radix is outside of the given range (not documented)
+<br>Number(Data Type)
+<br>&emsp;toExponential(Function)
+<br>String(Data Type)
+<br>&emsp;substr(Function) - Don't know what happens when startIndex is outside of string (not documented)
+<br>trace(Function) - Don't know how to accept which file to write to (not documented)
+<br>unescape(Function)
 <br><br>
 # Future Plans
 <br>Array(Data Type)
 <br>&emsp;sort(Function)
 <br>&emsp;sortOn(Function)
+<br>Date(Function)
+<br>Date(Data Type)
 <br>decodeURI(Function)
 <br>decodeURIComponent(Function)
 <br>encodeURI(Function)
 <br>encodeURIComponent(Function)
 <br>int(Function)
 <br>int(Data Type)
-<br>&emsp;toExponential(Function)
-<br>&emsp;toFixed(Function)
 <br>&emsp;toPrecision(Function)
 <br>RegExp(Data Type)
 <br>Number(Data Type)
 <br>&emsp;toExponential(Function)
+<br>&emsp;toFixed(Function)
 <br>&emsp;toPrecision(Function)
 <br>&emsp;toString(Function)
 <br>parseFloat(Function)
 <br>parseInt(Function)
 <br>String(Data Type)
 <br>&emsp;localeCompare(Function)
 <br>&emsp;match(Function)
 <br>&emsp;replace(Function)
 <br>&emsp;search(Function)
 <br>&emsp;slice(Function)
 <br>&emsp;split(Function)
-<br>&emsp;substr(Function)
 <br>uint(Function)
 <br>uint(Data Type)
 <br>Vector(Function)
 <br>Vector(Data Type)
 <br><br>
 # Functions I added
-<br>listtoarray - converts a given list to an Array.
+<br>listtoarray - converts a given list to an Array. Returns the Array.
 <br>Array.toSize - Creates an Array to specified size. If nothing is specified, assumes 0 elements
 <br>Number dunder methods int, float, add, sub, mul, truediv
 <br>escapeFullConvert - converts all characters to URL-encoded format
```

### Comparing `as3toplevel-0.0.2/as3toplevel.egg-info/PKG-INFO` & `as3toplevel-0.0.3/as3toplevel.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: as3toplevel
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python implementation of the ActionScript3 toplevel
 Home-page: https://github.com/ajdelguidice/python-as3toplevel
 Author: ajdelguidice
 Author-email: ajdelguidice@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,16 +19,14 @@
 <br><br>The types (Array, Boolean, Number, and String) are actual types so you can use them as such. They include almost everything that they did in ActionScript3. The length method in each type can only be used to get the length, I didn't implement the length assignment for Arrays.
 <br><br>Most of the inherited properties would be too hard to implement so I didn't bother with them.
 <br><br>I implemented the type conversion functions inside the types themselves (ex: instead of String(expression) use String.String(expression)).
 <br><br>For functions that needed a placeholder value for input(s) that aren't easily definable, could be multiple types, or relied on other factors to be set I use an empty dictionary as a placeholder. The values that these empty dictionaries represent aren't actually dictionaries, I just used something that would never be used in these functions so that I could detect it.
 <br><br>I have no way as of current to test the accuracy of these functions as I can't find a compiler for actionscript that I could get to work so if anything doesn't work or there is undocumented functionality please let me know on the github page.
 <br><br>
 # Currently Implemented
-<br>isFinite
-<br>isNaN
 <br>ArgumentError(Error Class)
 <br>Array(Function) - Moved to Array.Array()
 <br>Array(Data Type)
 <br>&emsp;Array(Constructor) - Create from values moved to class init function, create to size moved to toSize(Function).
 <br>&emsp;length(Property) - Moved to length(Function). Length assignment functionality not implemented yet
 <br>&emsp;concat(Function)
 <br>&emsp;every(Function)
@@ -52,18 +50,21 @@
 <br>&emsp;unshift(Function)
 <br>Boolean(Function) - Moved to Boolean.Boolean()
 <br>Boolean(Data Type) - Data representation changed from "true" and "false" to "True" and "False"
 <br>&emsp;Boolean(Constructor) - Moved to class init function
 <br>&emsp;toString(Function)
 <br>&emsp;valueOf(Function)
 <br>DefinitionError(Error Class)
-<br>escape(Function)
 <br>Error(Error Class)
 <br>EvalError(Error Class)
 <br>int(Data Type) - Moved to Int
+<br>&emsp;toExponential(Function)
+<br>&emsp;toFixed(Function)
+<br>isFinite(Function)
+<br>isNaN(Function)
 <br>valueOf(Function)
 <br><br>Math(Class) - All functions in this class had corresponding functions in python
 <br>&emsp;E(Constant)
 <br>&emsp;LN10(Constant)
 <br>&emsp;LN2(Constant)
 <br>&emsp;LOG10E(Constant)
 <br>&emsp;LOG2E(Constant)
@@ -87,15 +88,14 @@
 <br>&emsp;round(Function)
 <br>&emsp;sin(Function)
 <br>&emsp;sqrt(Function)
 <br>&emsp;tan(Function)
 <br>Number(Function) - Moved to Number.Number()
 <br>Number(Data Type)
 <br>&emsp;Number(Constructor) - Moved to class init function
-<br>&emsp;toFixed(Function)
 <br>&emsp;valueOf(Function)
 <br>RangeError(Error Class)
 <br>ReferenceError(Error Class)
 <br>SecurityError(Error Class)
 <br>String(Function) - Moved to String.String()
 <br>String(Data Type)
 <br>&emsp;String(Constructor) - Moved to class init function
@@ -109,57 +109,63 @@
 <br>&emsp;toLocaleLowerCase(Function)
 <br>&emsp;toLocaleUpperCase(Function)
 <br>&emsp;toLowerCase(Function)
 <br>&emsp;toUpperCase(Function)
 <br>&emsp;valueOf(Function)
 <br>SyntaxError(Error Class)
 <br>TypeError(Error Class)
-<br>unescape(Function)
 <br>URIError(Error Class)
 <br>VerifyError(Error Class)
 <br><br>
 # Partially Implemented
+<br>Date(Data Type)
+<br>escape(Function)
 <br>Number(Data Type)
 <br>&emsp;toString(Function)
 <br>int(Data Type)
-<br>&emsp;toString(Function)
-<br>trace(Function)
+<br>&emsp;toString(Function) - Don't know what is supposed to happen when radix is outside of the given range (not documented)
+<br>Number(Data Type)
+<br>&emsp;toExponential(Function)
+<br>String(Data Type)
+<br>&emsp;substr(Function) - Don't know what happens when startIndex is outside of string (not documented)
+<br>trace(Function) - Don't know how to accept which file to write to (not documented)
+<br>unescape(Function)
 <br><br>
 # Future Plans
 <br>Array(Data Type)
 <br>&emsp;sort(Function)
 <br>&emsp;sortOn(Function)
+<br>Date(Function)
+<br>Date(Data Type)
 <br>decodeURI(Function)
 <br>decodeURIComponent(Function)
 <br>encodeURI(Function)
 <br>encodeURIComponent(Function)
 <br>int(Function)
 <br>int(Data Type)
-<br>&emsp;toExponential(Function)
-<br>&emsp;toFixed(Function)
 <br>&emsp;toPrecision(Function)
 <br>RegExp(Data Type)
 <br>Number(Data Type)
 <br>&emsp;toExponential(Function)
+<br>&emsp;toFixed(Function)
 <br>&emsp;toPrecision(Function)
 <br>&emsp;toString(Function)
 <br>parseFloat(Function)
 <br>parseInt(Function)
 <br>String(Data Type)
 <br>&emsp;localeCompare(Function)
 <br>&emsp;match(Function)
 <br>&emsp;replace(Function)
 <br>&emsp;search(Function)
 <br>&emsp;slice(Function)
 <br>&emsp;split(Function)
-<br>&emsp;substr(Function)
 <br>uint(Function)
 <br>uint(Data Type)
 <br>Vector(Function)
 <br>Vector(Data Type)
 <br><br>
 # Functions I added
-<br>listtoarray - converts a given list to an Array.
+<br>listtoarray - converts a given list to an Array. Returns the Array.
 <br>Array.toSize - Creates an Array to specified size. If nothing is specified, assumes 0 elements
 <br>Number dunder methods int, float, add, sub, mul, truediv
 <br>escapeFullConvert - converts all characters to URL-encoded format
```

### Comparing `as3toplevel-0.0.2/as3toplevel.py` & `as3toplevel-0.0.3/as3toplevel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import math as m
 import random as r
 from numpy import nan
 from numpy import inf
 from numpy import NINF
 from numpy import base_repr
 from textwrap import wrap
+from time import time, strftime
+from datetime import datetime
 
 def listtoarray(l:list):
    """
    A function to convert a python list to an Array.
    """
    tempArray = Array()
    for i in range(0,len(l)):
@@ -37,20 +39,24 @@
 
 class NInfinity:
    def __init__(self):
       self.string = "-Infinity"
       self.value = NINF
    def __str__(self):
       return self.string
+   def __repr__(self):
+      return self.value
 class Infinity:
    def __init__(self):
       self.string = "Infinity"
       self.value = inf
    def __str__(self):
       return self.string
+   def __repr__(self):
+      return self.value
 class NaN:
    def __init__(self):
       self.string = "NaN"
       self.value = nan
    def __str__(self):
       return self.string
    def __repr__(self):
@@ -451,14 +457,147 @@
    def toString(self):
       return str(self.bool)
    def valueOf(self):
       if self.bool == True:
          return True
       else:
          return False
+class Date:
+   def __init__(self, time=time()):
+      self.time = time
+      #self.date
+      #self.dateUTC
+      #self.day
+      #self.dayUTC
+      #self.fullYear
+      #self.fullYearUTC
+      #self.hours
+      #self.hoursUTC
+      #self.milliseconds
+      #self.millisecondsUTC
+      #self.minutes
+      #self.minutesUTC
+      #self.month
+      #self.monthUTC
+      #self.seconds
+      #self.secondsUTC
+      self._tz = str(strftime('%Z%z'))
+      self.timezoneOffset = self._getcurrenttzoffset()
+   def __str__(self):
+      #returns dayoftheweek month dayofmonth time timezone year
+      pass
+   def __repr__(self):
+      return self.time
+   def _getcurrenttzoffset(self):
+      #Returns difference in minutes between local and UTC
+      i1 = self._tz.find("-")
+      if i1 == -1:
+         i1 = self._tz.find("+")
+         if i1 == -1:
+            return 0
+         else:
+            signmult = 1
+            l1 = self._tz.split("+")
+      else:
+         signmult = -1
+         l1 = self._tz.split("-")
+      l2 = wrap(l1[1],1)
+      hours = int(l2.pop(0) + l2.pop(0))
+      minutes = int(l2.pop(0) + l2.pop(0))
+      return (hours * 60 + minutes) * signmult
+   def Date():
+      pass
+   def getDate():
+      pass
+   def getDay():
+      pass
+   def getFullYear():
+      pass
+   def getHours():
+      pass
+   def getMilliseconds():
+      pass
+   def getMinutes():
+      pass
+   def getMonth():
+      pass
+   def getSeconds():
+      pass
+   def getTime():
+      pass
+   def getTimezoneOffset():
+      pass
+   def getUTCDate():
+      pass
+   def getUTCDay():
+      pass
+   def getUTCFullYear():
+      pass
+   def getUTCHours():
+      pass
+   def getUTCMilliseconds():
+      pass
+   def getUTCMinutes():
+      pass
+   def GetUTCMonth():
+      pass
+   def getUTCSeconds():
+      pass
+   def parse():
+      pass
+   def setDate():
+      pass
+   def setFullYear():
+      pass
+   def setHours():
+      pass
+   def setMilliseconds():
+      pass
+   def setMinutes():
+      pass
+   def setMonth():
+      pass
+   def setSeconds():
+      pass
+   def setTime():
+      pass
+   def setUTCDate():
+      pass
+   def setUTCFullYear():
+      pass
+   def setUTCHours():
+      pass
+   def setUTCMilliseconds():
+      pass
+   def setUTCMinutes():
+      pass
+   def setUTCMonth():
+      pass
+   def setUTCSeconds():
+      pass
+   def toDateString():
+      pass
+   def toJSON():
+      pass
+   def toLocaleDateString():
+      pass
+   def toLocaleString():
+      pass
+   def toLocaleTimeString():
+      pass
+   def toString():
+      pass
+   def toTimeString():
+      pass
+   def toUTCString():
+      pass
+   def UTC():
+      pass
+   def valueOf(self):
+      return self.time
 class DefinitionError(Exception):
    def __init__(self, message=""):
       self.error = message
 def decodeURI():
    pass
 def decodeURIComponent():
    pass
@@ -502,16 +641,31 @@
       return f'{self.value}'
    def __getitem__(self):
       return self.value
    def __setitem__(self, value):
       self.value = self.int(value)
    def __add__(self, value):
       return Int(self.value + self.int(value))
-   def __truediv__(self):
-      pass
+   def __sub__(self, value):
+      return Int(self.value - self.int(value))
+   def __mul__(self, value):
+      return Int(self.value * self.int(value))
+   def __truediv__(self, value):
+      if value == 0:
+         if self.value == 0:
+            return Number(Number.NaN)
+         elif self.value > 0:
+            return Number(Number.POSITIVE_INFINITY)
+         elif self.value < 0:
+            return Number(Number.NEGATIVE_INFINITY)
+      else:
+         try:
+            return Int(self.value / self.int(value))
+         except:
+            raise TypeError("Can not divide Int by " + f'{type(value)}')
    def __float__(self):
       return float(self.value)
    def __int__(self):
       return self.value
    def int(self, value):
       if type(value) == int or type(value) == Int:
          return value
@@ -520,18 +674,49 @@
       elif type(value) == str or type(value) == String:
          try:
             return int(value)
          except:
             raise TypeError("Can not convert " + str(value) + " to integer")
       else:
          raise TypeError("Can not convert " + str(value) + " to integer")
-   def toExponential(self):
-      pass
-   def toFixed():
-      pass
+   def toExponential(self, fractionDigits):
+      if fractionDigits < 0 or fractionDigits > 20:
+         raise Exception("RangeError: fractionDigits is outside of acceptable range")
+      else:
+         tempString1 = str(self.value)
+         templist = wrap(tempString1,1)
+         if templist[0] == "-":
+            templist.pop(0)
+            exponent = len(templist) - 1
+            tempString2 = "-" + templist.pop(0) + "."
+         else:
+            exponent = len(templist) - 1
+            tempString2 = templist.pop(0) + "."
+         if exponent == 0:
+            return self.value
+         else:
+            i = 0
+            while i < fractionDigits:
+               tempString2 += templist.pop(0)
+               i += 1
+            return tempString2 + "e+" + str(exponent)
+   def toFixed(self,fractionDigits):
+      if fractionDigits < 0 or fractionDigits > 20:
+         raise Exception("RangeError: fractionDigits is outside of acceptable range")
+      else:
+         tempString = str(self.value)
+         if fractionDigits == 0:
+            return tempString
+         else:
+            tempString += "."
+            i = 0
+            while i < fractionDigits:
+               tempString += "0"
+               i += 1
+            return tempString
    def toPrecision():
       pass
    def toString(self, radix=10):
       #!
       if radix > 36 or radix < 2:
          pass
       else:
@@ -592,20 +777,22 @@
    def sqrt(val):
       return m.sqrt(val)
    def tan(angleRadians):
       return m.tan(angleRadians)
 class Number:
    MAX_VALUE = 1.79e308
    MIN_VALUE = 5e-324
-   NaN = nan
-   NEGATIVE_INFINITY = inf
-   POSITIVE_INFINITY = NINF
+   NaN = NaN()
+   NEGATIVE_INFINITY = NInfinity()
+   POSITIVE_INFINITY = Infinity()
    def __init__(self, num):
       self.number = self.Number(num)
    def __str__(self):
+      if self.number == self.NaN or self.number == self.POSITIVE_INFINITY or self.number == self.NEGATIVE_INFINITY:
+         return str(self.number)
       tempString = str(self.number)
       templist = tempString.split(".")
       if templist[1] == "0":
          return f'{int(templist[0])}'
       else:
          return f'{self.number}'
    def __getitem__(self):
@@ -641,58 +828,43 @@
          except:
             raise TypeError("Can not divide Number by " + f'{type(value)}')
    def __float__(self):
       return float(self.number)
    def __int__(self):
       return int(self.number)
    def Number(self, expression):
-      if type(expression) == int or type(expression) == float or type(expression) == Number:
+      if expression == self.NEGATIVE_INFINITY:
+         return self.NEGATIVE_INFINITY
+      elif expression == self.POSITIVE_INFINITY:
+         return self.POSITIVE_INFINITY
+      elif type(expression) == int or type(expression) == float or type(expression) == Number:
          return expression
       elif expression == "undefined":
          return self.NaN
       elif expression == "null":
          return 0.0
       elif expression == self.NaN:
          return self.NaN
-      elif type(expresssion) == bool or type(expression) == Boolean:
+      elif type(expression) == bool or type(expression) == Boolean:
          if expression == True:
             return 1.0
          else:
             return 0.0
-      elif type(expresssion) == str or type(expression) == String:
+      elif type(expression) == str or type(expression) == String:
          if expression == "":
             return 0.0
          else:
             try:
                return float(expression)
             except:
                return self.NaN
-   def toExponential(self, fractionDigits):
-      if fractionDigits < 0 or fractionDigits > 20:
-         raise Exception("RangeError: fractionDigits is outside of acceptable range")
-      else:
-         pass
-   def toFixed(self, fractionDigits):
-      if fractionDigits < 0 or fractionDigits > 20:
-         raise Exception("RangeError: fractionDigits is outside of acceptable range")
-      else:
-         tempString1 = str(self.number)
-         templist = tempString1.split(".")
-         if fractionDigits == 0:
-            return templist[0]
-         else:
-            tempString2 = templist[0]
-            tempString2 += "."
-            tempString3 = templist[1]
-            for i in range(0,fractionDigits):
-               try:
-                  tempString2 += tempString3[i]
-               except IndexError:
-                  tempString2 += "0"
-            return tempString2
+   def toExponential(self):
+      pass
+   def toFixed(self):
+      pass
    def toPrecision():
       pass
    def toString(self, radix=10):
       #!
       return str(self.number)
    def valueOf(self):
       return self.number
@@ -728,15 +900,15 @@
    def __add__(self, value):
       return String(self.string + self.String(value))
    def __int__(self):
       return int(self.string)
    def __float__(self):
       return float(self.string)
    def length(self):
-      len(self.string)
+      return len(self.string)
    def String(self, expression):
       if type(expression) == str:
          return expression
       elif type(expression) == String:
          return expression.string
       elif type(expression) == bool:
          if expression == True:
@@ -782,16 +954,40 @@
       pass
    def search():
       pass
    def slice():
       pass
    def split():
       pass
-   def substr():
-      pass
+   def substr(self, startIndex=0, Len={}):
+      tempInt = len(self.string)
+      tempString1 = wrap(self.string,1)
+      if startIndex > tempInt - 1:
+         raise RangeError("startIndex is outside of the string")
+      if startIndex < 0 and abs(startIndex) > tempInt:
+         raise RangeError("startIndex is outside of the string")
+      if Len == {}:
+         length = tempInt
+      else:
+         length = Len
+      if startIndex < 0:
+         tempIndex = tempInt - abs(startIndex)
+      else:
+         tempIndex = startIndex
+      i = tempIndex
+      tempString2 = ""
+      if tempIndex + length >= tempInt:
+         while i < tempInt:
+            tempString2 += tempString1[i]
+            i += 1
+      else:
+         while i < tempIndex + length:
+            tempString2 += tempString1[i]
+            i += 1
+      return tempString2
    def substring(self, startIndex=0, endIndex={}):
       tempInt = len(self.string)
       si = startIndex
       ei = endIndex
       tempString = String()
       if si < 0:
          si = 0
@@ -816,14 +1012,25 @@
    def toUpperCase(self):
       return self.string.upper()
    def valueOf(self):
       return self.string
 class SyntaxError(Exception):
    def __init__(self, message=""):
       self.error = message
+def trace(*args):
+   output = ""
+   for i in range(0, len(args)):
+      if len(args) == 1:
+         output = str(args[0])
+      else:
+         if i == len(args) - 1:
+            output += str(args[i])
+         else:
+            output += str(args[i]) + " "
+   print(output)
 class TypeError(Exception):
    def __init__(self, message=""):
       self.error = message
 class uint:
    pass
 def unescape(Str):
    """
@@ -849,18 +1056,9 @@
       self.error = message
 class Vector:
    pass
 class VerifyError(Exception):
    def __init__(self, message=""):
       self.error = message
 
-def trace(*args):
-   output = ""
-   for i in range(0, len(args)):
-      if len(args) == 1:
-         output = str(args[0])
-      else:
-         if i == len(args) - 1:
-            output += str(args[i])
-         else:
-            output += str(args[i]) + ", "
-   print(output)
+s1 = String("1234567890")
+print(s1.substr(-11,1))
```

### Comparing `as3toplevel-0.0.2/setup.py` & `as3toplevel-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as ld:
       long_desc = ld.read()
 
 setup(name="as3toplevel",
-      version="0.0.2",
+      version="0.0.3",
       author="ajdelguidice",
       author_email="ajdelguidice@gmail.com",
       url="https://github.com/ajdelguidice/python-as3toplevel",
       py_modules=["as3toplevel"],
       description="Python implementation of the ActionScript3 toplevel",
       long_description=long_desc,
       long_description_content_type="text/markdown",
```

