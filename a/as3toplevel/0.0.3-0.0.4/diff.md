# Comparing `tmp/as3toplevel-0.0.3.tar.gz` & `tmp/as3toplevel-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "as3toplevel-0.0.3.tar", last modified: Sun Jun  4 14:20:13 2023, max compression
+gzip compressed data, was "as3toplevel-0.0.4.tar", last modified: Sun Jun  4 14:43:06 2023, max compression
```

## Comparing `as3toplevel-0.0.3.tar` & `as3toplevel-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ajdel     (1000) ajdel     (1000)        0 2023-06-04 14:20:13.558708 as3toplevel-0.0.3/
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     1069 2023-05-26 23:44:21.000000 as3toplevel-0.0.3/LICENSE
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       42 2023-05-27 00:52:01.000000 as3toplevel-0.0.3/MANIFEST.in
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     6672 2023-06-04 14:20:13.558708 as3toplevel-0.0.3/PKG-INFO
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     6128 2023-06-04 14:11:36.000000 as3toplevel-0.0.3/README.md
-drwxrwxr-x   0 ajdel     (1000) ajdel     (1000)        0 2023-06-04 14:20:13.558708 as3toplevel-0.0.3/as3toplevel.egg-info/
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     6672 2023-06-04 14:20:13.000000 as3toplevel-0.0.3/as3toplevel.egg-info/PKG-INFO
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)      252 2023-06-04 14:20:13.000000 as3toplevel-0.0.3/as3toplevel.egg-info/SOURCES.txt
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)        1 2023-06-04 14:20:13.000000 as3toplevel-0.0.3/as3toplevel.egg-info/dependency_links.txt
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)        6 2023-06-04 14:20:13.000000 as3toplevel-0.0.3/as3toplevel.egg-info/requires.txt
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       12 2023-06-04 14:20:13.000000 as3toplevel-0.0.3/as3toplevel.egg-info/top_level.txt
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)    46028 2023-06-04 14:09:38.000000 as3toplevel-0.0.3/as3toplevel.py
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       99 2023-05-27 00:14:36.000000 as3toplevel-0.0.3/pyproject.toml
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       73 2023-06-04 14:20:13.558708 as3toplevel-0.0.3/setup.cfg
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)      868 2023-06-03 20:31:04.000000 as3toplevel-0.0.3/setup.py
+drwxrwxr-x   0 ajdel     (1000) ajdel     (1000)        0 2023-06-04 14:43:06.911864 as3toplevel-0.0.4/
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     1069 2023-05-26 23:44:21.000000 as3toplevel-0.0.4/LICENSE
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       42 2023-05-27 00:52:01.000000 as3toplevel-0.0.4/MANIFEST.in
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     6752 2023-06-04 14:43:06.911864 as3toplevel-0.0.4/PKG-INFO
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     6208 2023-06-04 14:41:21.000000 as3toplevel-0.0.4/README.md
+drwxrwxr-x   0 ajdel     (1000) ajdel     (1000)        0 2023-06-04 14:43:06.907864 as3toplevel-0.0.4/as3toplevel.egg-info/
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     6752 2023-06-04 14:43:06.000000 as3toplevel-0.0.4/as3toplevel.egg-info/PKG-INFO
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)      252 2023-06-04 14:43:06.000000 as3toplevel-0.0.4/as3toplevel.egg-info/SOURCES.txt
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)        1 2023-06-04 14:43:06.000000 as3toplevel-0.0.4/as3toplevel.egg-info/dependency_links.txt
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)        6 2023-06-04 14:43:06.000000 as3toplevel-0.0.4/as3toplevel.egg-info/requires.txt
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       12 2023-06-04 14:43:06.000000 as3toplevel-0.0.4/as3toplevel.egg-info/top_level.txt
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)    45978 2023-06-04 14:38:25.000000 as3toplevel-0.0.4/as3toplevel.py
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       99 2023-05-27 00:14:36.000000 as3toplevel-0.0.4/pyproject.toml
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       74 2023-06-04 14:43:06.911864 as3toplevel-0.0.4/setup.cfg
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)      868 2023-06-04 14:39:47.000000 as3toplevel-0.0.4/setup.py
```

### Comparing `as3toplevel-0.0.3/LICENSE` & `as3toplevel-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `as3toplevel-0.0.3/PKG-INFO` & `as3toplevel-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: as3toplevel
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python implementation of the ActionScript3 toplevel
 Home-page: https://github.com/ajdelguidice/python-as3toplevel
 Author: ajdelguidice
 Author-email: ajdelguidice@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-as3toplevel
-A python implementation of some of the ActionScript3 toplevel functions and classes. They are as close as I could get them with my knowledge and the very limited documentation that adobe provides.
-<br><br>The types (Array, Boolean, Number, and String) are actual types so you can use them as such. They include almost everything that they did in ActionScript3. The length method in each type can only be used to get the length, I didn't implement the length assignment for Arrays.
+Do not use version 0.0.3. I forgot to remove the stuff I used for debugging
+<br><br>A python implementation of some of the ActionScript3 toplevel functions and classes. They are as close as I could get them with my knowledge and the very limited documentation that adobe provides.
+<br><br>The types (Array, Boolean, Int, Number, and String) are actual types so you can use them as such. They include almost everything that they did in ActionScript3. The length method in each type can only be used to get the length, I didn't implement the length assignment for Arrays.
 <br><br>Most of the inherited properties would be too hard to implement so I didn't bother with them.
 <br><br>I implemented the type conversion functions inside the types themselves (ex: instead of String(expression) use String.String(expression)).
-<br><br>For functions that needed a placeholder value for input(s) that aren't easily definable, could be multiple types, or relied on other factors to be set I use an empty dictionary as a placeholder. The values that these empty dictionaries represent aren't actually dictionaries, I just used something that would never be used in these functions so that I could detect it.
+<br><br>For functions that needed a placeholder value for input(s) that aren't easily definable, like multiple possible types or they relied on other factors to be set, I use an empty dictionary as a placeholder. The values that these empty dictionaries represent aren't actually dictionaries, I just used something that would never be used in these functions so that I could detect it.
 <br><br>I have no way as of current to test the accuracy of these functions as I can't find a compiler for actionscript that I could get to work so if anything doesn't work or there is undocumented functionality please let me know on the github page.
 <br><br>
 # Currently Implemented
 <br>ArgumentError(Error Class)
 <br>Array(Function) - Moved to Array.Array()
 <br>Array(Data Type)
 <br>&emsp;Array(Constructor) - Create from values moved to class init function, create to size moved to toSize(Function).
@@ -162,10 +163,10 @@
 <br>uint(Data Type)
 <br>Vector(Function)
 <br>Vector(Data Type)
 <br><br>
 # Functions I added
 <br>listtoarray - converts a given list to an Array. Returns the Array.
 <br>Array.toSize - Creates an Array to specified size. If nothing is specified, assumes 0 elements
-<br>Number dunder methods int, float, add, sub, mul, truediv
+<br>Dunder methods to relavent data types
 <br>escapeFullConvert - converts all characters to URL-encoded format
```

### Comparing `as3toplevel-0.0.3/README.md` & `as3toplevel-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # python-as3toplevel
-A python implementation of some of the ActionScript3 toplevel functions and classes. They are as close as I could get them with my knowledge and the very limited documentation that adobe provides.
-<br><br>The types (Array, Boolean, Number, and String) are actual types so you can use them as such. They include almost everything that they did in ActionScript3. The length method in each type can only be used to get the length, I didn't implement the length assignment for Arrays.
+Do not use version 0.0.3. I forgot to remove the stuff I used for debugging
+<br><br>A python implementation of some of the ActionScript3 toplevel functions and classes. They are as close as I could get them with my knowledge and the very limited documentation that adobe provides.
+<br><br>The types (Array, Boolean, Int, Number, and String) are actual types so you can use them as such. They include almost everything that they did in ActionScript3. The length method in each type can only be used to get the length, I didn't implement the length assignment for Arrays.
 <br><br>Most of the inherited properties would be too hard to implement so I didn't bother with them.
 <br><br>I implemented the type conversion functions inside the types themselves (ex: instead of String(expression) use String.String(expression)).
-<br><br>For functions that needed a placeholder value for input(s) that aren't easily definable, could be multiple types, or relied on other factors to be set I use an empty dictionary as a placeholder. The values that these empty dictionaries represent aren't actually dictionaries, I just used something that would never be used in these functions so that I could detect it.
+<br><br>For functions that needed a placeholder value for input(s) that aren't easily definable, like multiple possible types or they relied on other factors to be set, I use an empty dictionary as a placeholder. The values that these empty dictionaries represent aren't actually dictionaries, I just used something that would never be used in these functions so that I could detect it.
 <br><br>I have no way as of current to test the accuracy of these functions as I can't find a compiler for actionscript that I could get to work so if anything doesn't work or there is undocumented functionality please let me know on the github page.
 <br><br>
 # Currently Implemented
 <br>ArgumentError(Error Class)
 <br>Array(Function) - Moved to Array.Array()
 <br>Array(Data Type)
 <br>&emsp;Array(Constructor) - Create from values moved to class init function, create to size moved to toSize(Function).
@@ -146,10 +147,10 @@
 <br>uint(Data Type)
 <br>Vector(Function)
 <br>Vector(Data Type)
 <br><br>
 # Functions I added
 <br>listtoarray - converts a given list to an Array. Returns the Array.
 <br>Array.toSize - Creates an Array to specified size. If nothing is specified, assumes 0 elements
-<br>Number dunder methods int, float, add, sub, mul, truediv
+<br>Dunder methods to relavent data types
 <br>escapeFullConvert - converts all characters to URL-encoded format
```

### Comparing `as3toplevel-0.0.3/as3toplevel.egg-info/PKG-INFO` & `as3toplevel-0.0.4/as3toplevel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: as3toplevel
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python implementation of the ActionScript3 toplevel
 Home-page: https://github.com/ajdelguidice/python-as3toplevel
 Author: ajdelguidice
 Author-email: ajdelguidice@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-as3toplevel
-A python implementation of some of the ActionScript3 toplevel functions and classes. They are as close as I could get them with my knowledge and the very limited documentation that adobe provides.
-<br><br>The types (Array, Boolean, Number, and String) are actual types so you can use them as such. They include almost everything that they did in ActionScript3. The length method in each type can only be used to get the length, I didn't implement the length assignment for Arrays.
+Do not use version 0.0.3. I forgot to remove the stuff I used for debugging
+<br><br>A python implementation of some of the ActionScript3 toplevel functions and classes. They are as close as I could get them with my knowledge and the very limited documentation that adobe provides.
+<br><br>The types (Array, Boolean, Int, Number, and String) are actual types so you can use them as such. They include almost everything that they did in ActionScript3. The length method in each type can only be used to get the length, I didn't implement the length assignment for Arrays.
 <br><br>Most of the inherited properties would be too hard to implement so I didn't bother with them.
 <br><br>I implemented the type conversion functions inside the types themselves (ex: instead of String(expression) use String.String(expression)).
-<br><br>For functions that needed a placeholder value for input(s) that aren't easily definable, could be multiple types, or relied on other factors to be set I use an empty dictionary as a placeholder. The values that these empty dictionaries represent aren't actually dictionaries, I just used something that would never be used in these functions so that I could detect it.
+<br><br>For functions that needed a placeholder value for input(s) that aren't easily definable, like multiple possible types or they relied on other factors to be set, I use an empty dictionary as a placeholder. The values that these empty dictionaries represent aren't actually dictionaries, I just used something that would never be used in these functions so that I could detect it.
 <br><br>I have no way as of current to test the accuracy of these functions as I can't find a compiler for actionscript that I could get to work so if anything doesn't work or there is undocumented functionality please let me know on the github page.
 <br><br>
 # Currently Implemented
 <br>ArgumentError(Error Class)
 <br>Array(Function) - Moved to Array.Array()
 <br>Array(Data Type)
 <br>&emsp;Array(Constructor) - Create from values moved to class init function, create to size moved to toSize(Function).
@@ -162,10 +163,10 @@
 <br>uint(Data Type)
 <br>Vector(Function)
 <br>Vector(Data Type)
 <br><br>
 # Functions I added
 <br>listtoarray - converts a given list to an Array. Returns the Array.
 <br>Array.toSize - Creates an Array to specified size. If nothing is specified, assumes 0 elements
-<br>Number dunder methods int, float, add, sub, mul, truediv
+<br>Dunder methods to relavent data types
 <br>escapeFullConvert - converts all characters to URL-encoded format
```

### Comparing `as3toplevel-0.0.3/as3toplevel.py` & `as3toplevel-0.0.4/as3toplevel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1055,10 +1055,7 @@
    def __init__(self, message=""):
       self.error = message
 class Vector:
    pass
 class VerifyError(Exception):
    def __init__(self, message=""):
       self.error = message
-
-s1 = String("1234567890")
-print(s1.substr(-11,1))
```

### Comparing `as3toplevel-0.0.3/setup.py` & `as3toplevel-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as ld:
       long_desc = ld.read()
 
 setup(name="as3toplevel",
-      version="0.0.3",
+      version="0.0.4",
       author="ajdelguidice",
       author_email="ajdelguidice@gmail.com",
       url="https://github.com/ajdelguidice/python-as3toplevel",
       py_modules=["as3toplevel"],
       description="Python implementation of the ActionScript3 toplevel",
       long_description=long_desc,
       long_description_content_type="text/markdown",
```

