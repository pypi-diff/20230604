# Comparing `tmp/bantam-2.0.9.tar.gz` & `tmp/bantam-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.0.9.tar", last modified: Sun Nov 13 06:16:56 2022, max compression
+gzip compressed data, was "bantam-2.1.0.tar", last modified: Sun Jun  4 04:51:05 2023, max compression
```

## Comparing `bantam-2.0.9.tar` & `bantam-2.1.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2022-11-13 06:16:56.031843 bantam-2.0.9/
--rw-rw-r--   0 john      (1000) john      (1000)     1267 2022-11-12 20:32:51.000000 bantam-2.0.9/LICENSE.txt
--rw-rw-r--   0 john      (1000) john      (1000)      825 2022-11-13 06:16:56.031843 bantam-2.0.9/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)      370 2022-11-12 23:33:17.000000 bantam-2.0.9/README
--rw-rw-r--   0 john      (1000) john      (1000)      370 2022-11-12 23:17:54.000000 bantam-2.0.9/README.md
--rw-rw-r--   0 john      (1000) john      (1000)       28 2022-11-12 22:33:06.000000 bantam-2.0.9/requirements.txt
--rw-rw-r--   0 john      (1000) john      (1000)       70 2022-11-13 06:16:56.031843 bantam-2.0.9/setup.cfg
--rwxrwxr-x   0 john      (1000) john      (1000)     1425 2022-11-13 06:15:22.000000 bantam-2.0.9/setup.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2022-11-13 06:16:56.027843 bantam-2.0.9/src/
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2022-11-13 06:16:56.031843 bantam-2.0.9/src/bantam/
--rw-rw-r--   0 john      (1000) john      (1000)     4007 2022-11-12 23:25:30.000000 bantam-2.0.9/src/bantam/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    10429 2022-11-12 22:33:06.000000 bantam-2.0.9/src/bantam/api.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2022-11-13 06:16:56.031843 bantam-2.0.9/src/bantam/autogen/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-11-12 22:33:06.000000 bantam-2.0.9/src/bantam/autogen/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3017 2022-11-13 00:02:43.000000 bantam-2.0.9/src/bantam/autogen/main.py
--rw-rw-r--   0 john      (1000) john      (1000)    21468 2022-11-13 05:52:04.000000 bantam-2.0.9/src/bantam/client.py
--rw-rw-r--   0 john      (1000) john      (1000)     5471 2022-11-13 01:42:45.000000 bantam-2.0.9/src/bantam/conversions.py
--rw-rw-r--   0 john      (1000) john      (1000)     4112 2022-11-12 22:33:06.000000 bantam-2.0.9/src/bantam/decorators.py
--rw-rw-r--   0 john      (1000) john      (1000)    40491 2022-11-13 06:14:43.000000 bantam-2.0.9/src/bantam/http.py
--rw-rw-r--   0 john      (1000) john      (1000)    21911 2022-11-13 00:30:35.000000 bantam-2.0.9/src/bantam/js.py
--rw-rw-r--   0 john      (1000) john      (1000)    19836 2022-11-13 05:43:47.000000 bantam-2.0.9/src/bantam/js_async.py
--rw-rw-r--   0 john      (1000) john      (1000)    13103 2022-11-12 22:33:06.000000 bantam-2.0.9/src/bantam/pythonclient.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2022-11-13 06:16:56.031843 bantam-2.0.9/src/bantam.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)      825 2022-11-13 06:16:55.000000 bantam-2.0.9/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)      634 2022-11-13 06:16:55.000000 bantam-2.0.9/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2022-11-13 06:16:55.000000 bantam-2.0.9/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       62 2022-11-13 06:16:55.000000 bantam-2.0.9/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)       28 2022-11-13 06:16:55.000000 bantam-2.0.9/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)        7 2022-11-13 06:16:55.000000 bantam-2.0.9/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2022-11-13 06:16:56.031843 bantam-2.0.9/test/
--rw-rw-r--   0 john      (1000) john      (1000)     4489 2022-11-13 00:35:58.000000 bantam-2.0.9/test/test_client.py
--rw-rw-r--   0 john      (1000) john      (1000)     2849 2022-11-12 22:33:06.000000 bantam-2.0.9/test/test_conversions.py
--rw-rw-r--   0 john      (1000) john      (1000)     7244 2022-11-12 22:33:06.000000 bantam-2.0.9/test/test_decorators.py
--rw-rw-r--   0 john      (1000) john      (1000)     7549 2022-11-12 22:33:06.000000 bantam-2.0.9/test/test_js.py
--rw-rw-r--   0 john      (1000) john      (1000)     2869 2022-11-13 01:30:28.000000 bantam-2.0.9/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 04:51:05.775427 bantam-2.1.0/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-04 04:51:05.775427 bantam-2.1.0/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.1.0/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-03 15:15:17.000000 bantam-2.1.0/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-04 04:51:05.775427 bantam-2.1.0/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-04 04:15:36.000000 bantam-2.1.0/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 04:51:05.771427 bantam-2.1.0/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 04:51:05.775427 bantam-2.1.0/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4011 2023-06-04 04:49:42.000000 bantam-2.1.0/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    10329 2023-06-04 03:58:24.000000 bantam-2.1.0/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 04:51:05.775427 bantam-2.1.0/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.1.0/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.1.0/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    18033 2023-06-04 04:42:49.000000 bantam-2.1.0/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.1.0/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4594 2023-06-03 20:59:30.000000 bantam-2.1.0/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    41752 2023-06-04 03:57:52.000000 bantam-2.1.0/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    21983 2023-06-04 03:28:23.000000 bantam-2.1.0/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.1.0/src/bantam/js_async.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.1.0/src/bantam/pythonclient.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 04:51:05.775427 bantam-2.1.0/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-04 04:51:05.000000 bantam-2.1.0/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      641 2023-06-04 04:51:05.000000 bantam-2.1.0/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-04 04:51:05.000000 bantam-2.1.0/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-04 04:51:05.000000 bantam-2.1.0/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-04 04:51:05.000000 bantam-2.1.0/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-04 04:51:05.000000 bantam-2.1.0/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 04:51:05.775427 bantam-2.1.0/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4472 2023-06-04 02:18:21.000000 bantam-2.1.0/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4517 2023-06-04 02:21:15.000000 bantam-2.1.0/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.1.0/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.1.0/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     7531 2023-06-03 15:33:20.000000 bantam-2.1.0/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2845 2023-06-04 03:14:39.000000 bantam-2.1.0/test/test_js_async.py
```

### Comparing `bantam-2.0.9/PKG-INFO` & `bantam-2.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.0.9
+Version: 2.1.0
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
+Download-URL: https://github.com/bantam/dist/2.1.0
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
-Download-URL: https://github.com/bantam/dist/2.0.9
 Keywords: auto web api python
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
-License-File: LICENSE.txt
 
 
 Bantam is a Python package for building http-based micro-services.
 It abstracts away any knowledge of routes, mappings and translations
 between javascript and Python.  It even provides a means of
 auto-generating the javascript client interface to you app
 on the fly and serve it to web-based/javascript-based clients.
 
 See https://nak.github.io/bantam_docs/ for details.
 
     
-
```

### Comparing `bantam-2.0.9/setup.py` & `bantam-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.0.9"
+VERSION = "2.1.0"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.0.9/src/bantam/__init__.py` & `bantam-2.1.0/src/bantam/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 Let's look at setting up a simple WebApplication on your localhost:
 
 >>> import asyncio
 ... from bantam.http import web_api, RestMethod, WebApplication
 ...
 ... class Greetings:
 ...
+...     @classmethod
 ...     @web_api(content_type='text/html', method=RestMethod.GET)
-...     @staticmethod
-...     async def welcome(name: str) -> str:
+...     async def welcome(cls, name: str) -> str:
 ...         \"\"\"
 ...         Welcome someone
 ...
 ...         :@param name: name of person to greet
 ...         :return: a salutation of welcome
 ...         \"\"\"
 ...         return f"<html><body><p>Welcome, {name}!</p></body></html>"
 ...
-...     @web_api(content_type='text/html', method=RestMethod.GET)
 ...     @classmethod
+...     @web_api(content_type='text/html', method=RestMethod.GET)
 ...     async def goodbye(cls, type_of_day: str) -> str:
 ...         \"\"\"
 ...         Tell someone goodbye by telling them to have a day (of the given type)
 ...
 ...         :@param type_of_day:  an adjective describe what type of day to have
 ...         :return: a saltation of welcome
 ...         \"\"\"
```

### Comparing `bantam-2.0.9/src/bantam/api.py` & `bantam-2.1.0/src/bantam/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 class API:
 
     def __init__(self, clazz, func, method: RestMethod, content_type: str, is_instance_method: bool,
                  is_class_method: bool,
                  is_constructor: bool,
                  timeout: Optional[ClientTimeout] = None,
                  expire_on_exit: bool = False, uuid_param: Optional[str] = None):
-        annotations = func.__annotations__ if not is_class_method else func.__func__.__annotations__
+        annotations = func.__annotations__
         self._clazz = clazz
         self._is_class_method = is_class_method
         self._is_instance_method = is_instance_method
         self._is_static = not self._is_class_method and not self._is_instance_method
         self._expire_obj = expire_on_exit
         self._func = func
-        self._real_func = func if not is_class_method else func.__func__
+        self._real_func = func
         self._method = method
         self._timeout = timeout or ClientTimeout()
         if 'return' not in annotations:
             raise TypeError(f"No annotation for return type in {func}")
         self._arg_annotations = {name: typ for name, typ in annotations.items() if name != 'return'}
         self._async_arg_annotations = {
             name: typ for name, typ in self._arg_annotations.items()
```

### Comparing `bantam-2.0.9/src/bantam/autogen/main.py` & `bantam-2.1.0/src/bantam/autogen/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import importlib
 import sys
 
 from bantam.http import WebApplication
 
 
-def _qual_name(typ):
-    if type is None:
-        return None
-    if hasattr(typ, '__qualname__'):
-        return (typ.__module__ + '.' if typ.__module__ != 'builtins' else '') + typ.__qualname__
-    return str(typ)
+def _name(typ):
+    if typ is None or isinstance(typ, type(None)):
+        return 'None'
+    if hasattr(typ, '__name__'):
+        return typ.__name__
+    elif hasattr(typ, '__qualname__'):
+        return typ.__qualname__
+    module = typ.__module__
+    return str(typ)[len(module) + 1:].replace('NoneType', 'None')
 
 
 def main():
     if len(sys.argv) not in (2, 3):
         print(f"Usage: {sys.argv[0]} <module-name> [suffix-for-client-class]")
         sys.exit(1)
     module_name = sys.argv[1]
@@ -29,63 +32,71 @@
         sys.exit(2)
     by_class = {}
     for route, api in apis.items():
         class_name = route[1:].split('/')[0]
         assert class_name, f"Route has improper spec: '{route}'"
         by_class.setdefault(class_name, {})[route] = api
 
-    for class_name, route_mapping in by_class.items():
-        text = f"""
+    text = f"""
 import typing
+
 from bantam.client import WebInterface
 from abc import abstractmethod
 from bantam.http import web_api
 from bantam.api import RestMethod
+"""
+    imports = set()
+    for class_name, route_mapping in by_class.items():
+        text += f"""
 
 class {class_name}Interface(WebInterface):
 
     """
-        method_text = ""
-        imports = set()
         for route, api in route_mapping.items():
             target = route[1:].split('/', maxsplit=1)[1]
             args = api.arg_annotations
-            arg_text = ', '.join(f"{arg_name}: {_qual_name(typ)}" for arg_name, typ in args.items())
+            arg_text = ', '.join(f"{arg_name}: {_name(typ)}" for arg_name, typ in args.items())
             for typ in list(args.values()) + [api.return_type]:
                 if typ is None:
                     continue
                 elif typ.__module__ != 'builtins':
-                    imports.add(f"import {typ.__module__}")
+                    imports.add(f"from {typ.__module__} import {_name(typ).split('[', maxsplit=1)[0]}")
             web_api_args = \
-                f"method={api.method}, content_type='{api.content_type}', is_constructor={api.is_constructor},"\
-                f" uuid_param={api.uuid_param}"
-            return_type = f"{_qual_name(api.return_type)}"
+                f"method={api.method}, content_type='{api.content_type}', "
+            if api.is_constructor:
+                web_api_args += f"is_constructor=True, "
+            if api.uuid_param is not None:
+                web_api_args += f"uuid_param=\"{api.uuid_param}\""
+            return_type = f"{_name(api.return_type)}"
+            if api.has_streamed_response:
+                return_type = f"AsyncIterator[{return_type}]"
+                imports.add('from typing import AsyncIterator')
             if api.is_static:
                 addl_decorator = "@staticmethod\n    "
             elif api.is_class_method:
                 addl_decorator = "@classmethod\n    "
                 arg_text = f"cls, {arg_text}"
             else:
                 addl_decorator = ''
             if api.is_instance_method:
                 arg_text = f"self, {arg_text}"
-            method_text += f"""
+            assert web_api_args
+            text += f"""
     @web_api({web_api_args})
     {addl_decorator}@abstractmethod
     async def {target}({arg_text}) -> {return_type}:
         \"\"\"
         abstraction for {route} web-api route
         \"\"\"
-"""
-        sys.stdout.write('\n'.join(imports) + '\n')
-        sys.stdout.write(text)
-        sys.stdout.write(method_text)
-        sys.stdout.write(f"""
-        
-{class_name}{class_suffix} = {class_name}Interface.Client
-""")
-        sys.stdout.write('\n')
+    """
+        text += f"""
+
+{class_name}{class_suffix} = {class_name}Interface.Client()
+        """
+    sys.stdout.write('\n'.join(imports) + '\n')
+    sys.stdout.write(text)
+    sys.stdout.write('\n')
     return 0
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `bantam-2.0.9/src/bantam/client.py` & `bantam-2.1.0/src/bantam/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,352 +1,381 @@
 """
 Bantam provides and abstraction to easily declare Python clients to interact with a Bantam web application.
-Bantam even provide a means of auto-generating the code for clients.
 
-To auto-generate client code, an application *bantam_generate* is provided:
+To access client code, a server implementation must inherit from an abstract interface common to both client
+and server.  One defines an interface class (usually in its own file) such as:
 
-.. code-block:: bash
-
-   bantam_generate <module-name> [<suffix>]
-
-This will generate code to stdout for client classes that match the @web_api's defined in the provided module.  Each
-client class is named the same as the class it is derived from, unless the optional second argument is provided. If
-provided the class name will be appended with this suffix.
-
-You can also generate this code manually if desired, of course, following the pattern from auto-generation of code.
-This code provides an abstraction to the @web_api interface implementation, stand-alone from the implementation code
-if desired. (e.g. providing a stand-alone client package for install separate from the implementation server-side
-package.
+>>>  from bantam.client import WebInterface
+...  from bantam.api import RestMethod
+...  from bantam.decorators web_api
+...  from typing import AsyncIterator
+...  from abc import abstractmethod
+...
+...  class MyServerApiInterface(WebInterface):
+...     @classmethod
+...     @web_api(methos=RestMethod.GET, content_type='application/json')
+...     @abstractmethod
+...     async def constructor(cls) -> "MyServerApiInterface":
+...        '''
+...        Abstract constructor to create an instance of the class
+...        '''
+...
+...      @classmethod
+...      @web_api(method=RestMethod.GET, content_type='text/plain')
+...      @abstractmethod
+...      async def class_method_api(cls, parm1: str) -> Dict[str, int]:
+...          '''
+...           Abstract class method to be implemented WITH SAME @web_api DECORATION
+...          '''
+...
+...      @web_api(method=RestMethod.POST, content_type='application/json')
+...      @abstractmethod
+...      async def instance_method_api(self) -> AsyncIterator[str]:
+...          '''
+...          Abstract instance method that is an Async Iterator over string values. MUST
+...          HAVE SAME @web_api DECORATION AS SERVER IMPL DECLARATION
+...          '''
+...          # never called since abstract, but needed to tell Python that implementation
+...          # will be an async generator/iterator:
+...          yield None
+...
+
+One then defines the concrete class (which for best practice, has same name, sans 'Interface'):
+
+>>>  from bantam.client import WebInterface
+...  from bantam.api import RestMethod
+...  from bantam.decorators web_api
+...  from typing import AsyncIterator
+...
+...  class MyServerApi(MyServerApiInterface):
+...
+...     def __init__(self):
+...         self._message_bits = ['I', 'am', 'the', 'very', 'model']
+...
+...     @classmethod
+...     @web_api(methos=RestMethod.GET, content_type='application/json')
+...     async def constructor(cls) -> "MyServerApiInterface":
+...        '''
+...        Concreate constructor to create an instance of the class WITH SAEM @web_api DECORATOR AND
+...        SIGNATURE
+...        '''
+...        return MyServerApi()
+...
+...      @classmethod
+...      @web_api(method=RestMethod.GET, content_type='text/plain')
+...      async def class_method_api(cls, parm1: str) -> Dict[str, int]:
+...          '''
+...          Concreate class method to be implemented WITH SAME @web_api DECORATION AND,
+...          OF COURSE, SIGNATURE
+...          '''
+...          return {'param1': int(parm1)}
+...
+...      @web_api(method=RestMethod.POST, content_type='application/json')
+...      async def instance_method_api(self) -> AsyncIterator[str]:
+...          '''
+...          Concrete instance method that is an Async Iterator over string values.
+...          MUST HAVE SAME @web_api DECORATION AND SIGNATURE
+...          '''
+...          # never called since abstract, but needed to tell Python that implementation
+...          # will be an async generator/iterator:
+...          for text in self._message_bits:
+...              yield text
+...
+
+One can then declare a Client that acts as a proxy to make calls to the server, thereby keeping the
+http protocol details hidden (abstracted away frm the user):
+
+>>>  def async_call():
+...      client = MyServerApiInterface.Client(end_point='https://blahblahblah')
+...      instance = await client.constructor()
+...      async for text in instance.instance_method_api():
+...          print(text)
+...
+
+If you do not fallow the recommended practice of the interface have the same name as the concreate class, only with
+an "Interface" suffix, you will have to specify *impl_name=<name-of-concrete-class>* as a parameter to Client class
+method above.  The *end_point* parameter specifies the base url to the server that serves up MyServceApi class.
 
 """
-import json
 import inspect
+import json
 from abc import ABC
-from typing import TypeVar, Type, Optional, Any
+from functools import wraps
+from typing import Any, Dict, TypeVar, Optional, Type, AsyncIterator
 
 import aiohttp
 
 from bantam import conversions
-from bantam.api import RestMethod, API
+from bantam.api import API, RestMethod
 
+__all__ = ["WebInterface"]
 
-T = TypeVar('T', bound="WebClient")
+C = TypeVar('C', bound="WebInterface")
 
 
+# noinspection PyProtectedMember
 class WebInterface(ABC):
 
-    # noinspection PyPep8Naming
+    _clients: Dict[str, Any] = {}
+
     @classmethod
-    def Client(cls: Type[T], impl_name: Optional[str] = None):
+    def _generate_url_args(cls, kwargs, self_id: Optional[str] = None):
+        if self_id is None and not kwargs:
+            return ''
+        return (f'?self={self_id}&' if self_id is not None else '?') + \
+            '&'.join([f"{k}={conversions.to_str(v)}" for k, v in kwargs.items() if v is not None])
 
+    @classmethod
+    def _add_class_method(cls, clazz: Type, impl_name: str, end_point: str, method,
+                          common_headers: dict):
+        # class/static methods
         # noinspection PyProtectedMember
-        class ClientFactory:
-            _cache = {}
-
-            def __getitem__(self: T, end_point: str) -> Any:
-                if end_point in ClientFactory._cache:
-                    return ClientFactory._cache[end_point]
-                while end_point.endswith('/'):
-                    end_point = end_point[:-1]
-
-                # noinspection PyProtectedMember
-                class ClientImpl(cls):
-
-                    end_point = None
-                    _clazz = cls
-                    if not impl_name and not cls.__name__.endswith('Interface'):
-                        raise SyntaxError("You must either supply an explicit name in Client for implementing class, "
-                                          "or name the class <implement-class-name>Interface (aka wit a suffix of "
-                                          "'Interface'")
-                    else:
-                        _impl_name = impl_name or cls.__name__[:-9]
-
-                    def __init__(self, self_id: str):
-                        self._self_id = self_id
-
-                    @classmethod
-                    def add_instance_method(cls, name_: str, method_):
-                        # instance method
-                        if name_ in ('Client', '_construct'):
-                            return
-                        if not hasattr(method_, '_bantam_web_api'):
-                            raise SyntaxError(f"All methods of class WebClient most be decorated with '@web_api'")
-                        # noinspection PyProtectedMember
-                        if method_._bantam_web_api.has_streamed_request:
-                            raise SyntaxError(f"Streamed request for WebClient's are not supported at this time")
-                        # noinspection PyProtectedMember
-                        api: API = method_._bantam_web_api
-
-                        async def instance_method(this, *args, **kwargs_):
-                            nonlocal api
-                            arg_spec = inspect.getfullargspec(api._func)
-                            kwargs_.update({
-                                arg_spec.args[n]: arg for n, arg in enumerate(args)
-                            })
-                            rest_method = api.method
-                            while cls.end_point.endswith('/'):
-                                cls.end_point = cls.end_point[:-1]
-                            if rest_method.value == RestMethod.GET.value:
-                                url_args = cls._generate_url_args(self_id=this._self_id, kwargs=kwargs_)
-                                url = f"{cls.end_point}/{cls._impl_name}/{api.name}{url_args}"
-                                async with aiohttp.ClientSession(timeout=api.timeout) as session:
-                                    async with session.get(url) as resp:
-                                        data = (await resp.content.read()).decode('utf-8')
-                                        return conversions.from_str(data, api.return_type)
-                            else:
-                                url = f"{cls.end_point}/{cls._impl_name}/{api.name}?self={this._self_id}"
-                                payload = json.dumps({k: conversions.to_str(v) for k, v in kwargs_.items()})
-                                async with aiohttp.ClientSession(timeout=api.timeout) as session:
-                                    async with session.post(url, data=payload) as resp:
-                                        data = (await resp.content.read()).decode('utf-8')
-                                        return conversions.from_str(data, api.return_type)
-
-                        async def instance_method_streamed(this, *args, **kwargs_):
-                            nonlocal api
-                            arg_spec = inspect.getfullargspec(api._func)
-                            kwargs_.update({
-                                arg_spec.args[n]: arg for n, arg in enumerate(args)
-                            })
-                            method_api = api.method
-                            rest_method = method_api._bantam_web_api.method
-                            while cls.end_point.endswith('/'):
-                                cls.end_point = cls.end_point[:-1]
-                            if rest_method == RestMethod.GET:
-                                url_args = cls._generate_url_args(self_id=this._self_id, kwargs=kwargs_)
-                                url = f"{cls.end_point}/{cls._impl_name}/{api.name}{url_args}"
-                                async with aiohttp.ClientSession(timeout=api.timeout) as session:
-                                    async with session.get(url) as resp:
-                                        resp.raise_for_status()
-                                        async for data, _ in resp.content.iter_chunks():
-                                            if data:
-                                                data = data.decode('utf-8')
-                                                yield conversions.from_str(data, api.return_type)
-                            else:
-                                url = f"{cls.end_point}/{cls._impl_name}/{api.name}?self={this._self_id}"
-                                payload = json.dumps({k: conversions.to_str(v) for k, v in kwargs_.items()})
-                                async with aiohttp.ClientSession(timeout=api.timeout) as session:
-                                    async with session.post(url, data=payload) as resp:
-                                        resp.raise_for_status()
-                                        async for data, _ in resp.content.iter_chunks():
-                                            if data:
-                                                data = data.decode('utf-8')
-                                                yield conversions.from_str(data, api.return_type)
-
-                        if api.has_streamed_response:
-                            setattr(cls, name_, instance_method_streamed)
-                        else:
-                            setattr(cls, name_, instance_method)
-
-                    @classmethod
-                    def _generate_url_args(cls, kwargs, self_id: Optional[str] = None):
-                        if self_id is None and not kwargs:
-                            return ''
-                        return (f'?self={self_id}&' if self_id is not None else '?') + \
-                            '&'.join([f"{k}={conversions.to_str(v)}" for k, v in kwargs.items() if v is not None])
-
-                    @classmethod
-                    def add_static_method(cls, name_: str, method_):
-                        # class/static methods
-
-                        if not hasattr(method_, '_bantam_web_api'):
-                            raise SyntaxError(f"All methods of class WebClient most be decorated with '@web_api'")
-                        # noinspection PyProtectedMember
-                        if method_._bantam_web_api.has_streamed_request:
-                            raise SyntaxError(f"Streamed request for WebClient's are not supported at this time")
-                        # noinspection PyProtectedMember
-                        api: API = method_._bantam_web_api
-                        base_url = f"{cls.end_point}/{cls._impl_name}/{name_}"
-
-                        # noinspection PyDecorator
-                        @staticmethod
-                        async def static_method(*args, **kwargs_):
-                            nonlocal api
-                            arg_spec = inspect.getfullargspec(api._func)
-                            kwargs_.update({
-                                arg_spec.args[n]: arg for n, arg in enumerate(args)
-                            })
-                            rest_method = api._func._bantam_web_api.method
-                            while cls.end_point.endswith('/'):
-                                cls.end_point = cls.end_point[:-1]
-                            if rest_method.value == RestMethod.GET.value:
-                                url_args = cls._generate_url_args(kwargs=kwargs_)
-                                url = f"{base_url}{url_args}"
-                                async with aiohttp.ClientSession(timeout=api.timeout) as session:
-                                    async with session.get(url) as resp:
-                                        resp.raise_for_status()
-                                        data = (await resp.content.read()).decode('utf-8')
-                                        if api.is_constructor:
-                                            if hasattr(cls, 'jsonrepr'):
-                                                repr_ = cls.jsonrepr(data)
-                                                self_id = repr_[api.uuid_param or 'self_id']
-                                            else:
-                                                self_id = kwargs_[api.uuid_param or 'self_id']
-                                            return cls(self_id)
-                                        return conversions.from_str(data, api.return_type)
-                            else:
-                                payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
-                                                      for k, v in kwargs_.items()})
-                                async with aiohttp.ClientSession(timeout=api.timeout) as session:
-                                    async with session.post(base_url, data=payload) as resp:
-                                        resp.raise_for_status()
-                                        data = (await resp.content.read()).decode('utf-8')
-                                        if api.is_constructor:
-                                            self_id = json.loads(data)['self_id']
-                                            return cls(self_id)
-                                        return conversions.from_str(data, api.return_type)
-
-                        # noinspection PyDecorator
-                        @staticmethod
-                        async def static_method_streamed(*args, **kwargs_):
-                            nonlocal api
-                            arg_spec = inspect.getfullargspec(api._func)
-                            kwargs_.update({
-                                arg_spec.args[n]: arg for n, arg in enumerate(args)
-                            })
-                            rest_method = api._func._bantam_web_api.method
-                            while cls.end_point.endswith('/'):
-                                cls.end_point = cls.end_point[:-1]
-                            if rest_method.value == RestMethod.GET.value:
-                                url_args = cls._generate_url_args(kwargs=kwargs_)
-                                url = f"{base_url}{url_args}"
-                                async with aiohttp.ClientSession(timeout=api.timeout) as session:
-                                    async with session.get(url) as resp:
-                                        resp.raise_for_status()
-                                        async for data, _ in resp.content.iter_chunks():
-                                            if data:
-                                                data = data.decode('utf-8')
-                                                yield conversions.from_str(data, api.return_type)
-                            else:
-                                payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
-                                                      for k, v in kwargs_.items()})
-                                async with aiohttp.ClientSession(timeout=api.timeout) as session:
-                                    async with session.post(base_url, data=payload) as resp:
-                                        async for data, _ in resp.content.iter_chunks():
-                                            resp.raise_for_status()
-                                            if data:
-                                                data = data.decode('utf-8')
-                                                yield conversions.from_str(data, api.return_type)
-
-                        if api.has_streamed_response:
-                            setattr(ClientImpl, api.name, static_method_streamed)
-                        else:
-                            setattr(ClientImpl, api.name, static_method)
-
-                    @classmethod
-                    def add_class_method(cls, name_: str, method_):
-                        # class/static methods
-
-                        if not hasattr(method_, '_bantam_web_api'):
-                            raise SyntaxError(f"All methods of class WebClient most be decorated with '@web_api'")
-                        # noinspection PyProtectedMember
-                        if method_._bantam_web_api.has_streamed_request:
-                            raise SyntaxError(f"Streamed request for WebClient's are not supported at this time")
-                        # noinspection PyProtectedMember
-                        api: API = method_._bantam_web_api
-                        base_url = f"{cls.end_point}/{cls._impl_name}/{name_}"
-
-                        # noinspection PyDecorator,PyShadowingNames
-                        @classmethod
-                        async def class_method(cls, *args, **kwargs_):
-                            nonlocal api
-                            try:
-                                arg_spec = inspect.getfullargspec(api._func)
-                            except Exception:
-                                arg_spec = inspect.getfullargspec(api._func.__func__)
-                            kwargs_.update({
-                                arg_spec.args[n]: arg for n, arg in enumerate(args)
-                            })
-                            # noinspection PyBroadException
-                            rest_method = api._func._bantam_web_api.method
-                            while cls.end_point.endswith('/'):
-                                cls.end_point = cls.end_point[:-1]
-                            if rest_method.value == RestMethod.GET.value:
-                                url_args = cls._generate_url_args(kwargs=kwargs_)
-                                url = f"{base_url}{url_args}"
-                                async with aiohttp.ClientSession(timeout=api.timeout) as session:
-                                    async with session.get(url) as resp:
-                                        resp.raise_for_status()
-                                        data = (await resp.content.read()).decode('utf-8')
-                                        if api.is_constructor:
-                                            if hasattr(cls, 'jsonrepr'):
-                                                repr_ = cls.jsonrepr(data)
-                                                self_id = repr_[api.uuid_param or 'self_id']
-                                            else:
-                                                self_id = kwargs_[api.uuid_param or 'self_id']
-                                            return cls(self_id)
-                                        return conversions.from_str(data, api.return_type)
-                            else:
-                                payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
-                                                      for k, v in kwargs_.items()})
-                                async with aiohttp.ClientSession(timeout=api.timeout) as session:
-                                    async with session.post(base_url, data=payload) as resp:
-                                        resp.raise_for_status()
-                                        data = (await resp.content.read()).decode('utf-8')
-                                        if api.is_constructor:
-                                            self_id = json.loads(data)['self_id']
-                                            return cls(self_id)
-                                        return conversions.from_str(data, api.return_type)
-
-                        # noinspection PyDecorator
-                        @classmethod
-                        async def class_method_streamed(*args, **kwargs_):
-                            nonlocal api
-                            arg_spec = inspect.getfullargspec(api._func)
-                            kwargs_.update({
-                                arg_spec.args[n]: arg for n, arg in enumerate(args)
-                            })
-                            rest_method = api._func._bantam_web_api.method
-                            while cls.end_point.endswith('/'):
-                                cls.end_point = cls.end_point[:-1]
-                            if rest_method.value == RestMethod.GET.value:
-                                url_args = cls._generate_url_args(kwargs=kwargs_)
-                                url = f"{base_url}{url_args}"
-                                async with aiohttp.ClientSession(timeout=api.timeout) as session:
-                                    async with session.get(url) as resp:
-                                        resp.raise_for_status()
-                                        async for data, _ in resp.content.iter_chunks():
-                                            if data:
-                                                data = data.decode('utf-8')
-                                                yield conversions.from_str(data, api.return_type)
-                            else:
-                                payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
-                                                      for k, v in kwargs_.items()})
-                                async with aiohttp.ClientSession(timeout=api.timeout) as session:
-                                    async with session.post(base_url, data=payload) as resp:
-                                        async for data, _ in resp.content.iter_chunks():
-                                            resp.raise_for_status()
-                                            if data:
-                                                data = data.decode('utf-8')
-                                                yield conversions.from_str(data, api.return_type)
-
-                        if api.has_streamed_response:
-                            setattr(ClientImpl, api.name, class_method_streamed)
-                        else:
-                            setattr(ClientImpl, api.name, class_method)
-
-                    @classmethod
-                    def _construct(cls):
-                        for name, method in inspect.getmembers(
-                                cls._clazz,
-                                predicate=lambda x: inspect.ismethod(x) or inspect.isfunction(x)):
-                            if name in ('__init__', '_construct', 'Client', 'jsonrepr'):
-                                continue
-                            if not hasattr(method, '_bantam_web_api'):
-                                raise SyntaxError(f"classes inheriting from WebInterface should only implement "
-                                                  "method decorated with @web_api")
-                            if method._bantam_web_api.is_static:
-                                cls.add_static_method(name, method)
-                            elif method._bantam_web_api.is_class_method:
-                                cls.add_class_method(name, method)
+        # noinspection PyProtectedMember
+        name = method.__name__
+        api: API = method._bantam_web_api
+        base_url = f"{end_point}/{impl_name}/{name}"
+
+        # noinspection PyDecorator,PyShadowingNames
+        @classmethod
+        @wraps(method)
+        async def class_method(cls_, *args, **kwargs_):
+            nonlocal api, end_point
+            # noinspection PyBroadException
+            try:
+                arg_spec = inspect.getfullargspec(api._func)
+            except Exception:
+                arg_spec = inspect.getfullargspec(api._func.__func__)
+            kwargs_.update({
+                arg_spec.args[n + 1]: arg for n, arg in enumerate(args)
+            })
+            # noinspection PyBroadException
+            rest_method = api._func._bantam_web_api.method
+            if rest_method.value == RestMethod.GET.value:
+                url_args = cls._generate_url_args(kwargs=kwargs_)
+                url = f"{base_url}{url_args}"
+                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                    async with session.get(url) as resp:
+                        resp.raise_for_status()
+                        data = (await resp.content.read()).decode('utf-8')
+                        if api.is_constructor:
+                            if hasattr(clazz, 'jsonrepr'):
+                                repr_ = clazz.jsonrepr(data)
+                                self_id = repr_[api.uuid_param or 'uuid']
                             else:
-                                cls.add_instance_method(name, method)
+                                repr_ = json.loads(data)
+                                self_id = repr_[api.uuid_param or 'uuid']
+                            return cls_(self_id)
+                        return conversions.from_str(data, api.return_type)
+            else:
+                payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
+                                      for k, v in kwargs_.items()})
+                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                    async with session.post(base_url, data=payload) as resp:
+                        resp.raise_for_status()
+                        data = (await resp.content.read()).decode('utf-8')
+                        if api.is_constructor:
+                            self_id = json.loads(data)[api.uuid_param or 'uuid']
+                            return cls_(self_id)
+                        return conversions.from_str(data, api.return_type)
 
-                ClientImpl.end_point = end_point
+        setattr(clazz, name, class_method)
 
-                # abstractmethod implementations added dynamcially in ClientImple._cosntruct
-                # cannot be added before processed by interpreter, so have to create one more level
-                class ClientImplSane(ClientImpl):
-                    ClientImpl._construct()
-                ClientFactory._cache[end_point] = ClientImplSane
-                return ClientImplSane
+    @classmethod
+    def _add_class_method_streamed(cls, clazz: Type, impl_name: str, end_point: str, method,
+                                   common_headers: dict):
+        if not hasattr(method, '_bantam_web_api'):
+            raise SyntaxError(f"All methods of class WebClient most be decorated with '@web_api'")
+        # noinspection PyProtectedMember
+        if method._bantam_web_api.has_streamed_request:
+            raise SyntaxError(f"Streamed request for WebClient's are not supported at this time")
+        # noinspection PyProtectedMember
+
+        name = method.__name__
+        api: API = method._bantam_web_api
+        base_url = f"{end_point}/{impl_name}/{name}"
+
+        # noinspection PyDecorator,PyUnusedLocal
+        @classmethod
+        async def class_method_streamed(cls_, *args, **kwargs):
+            nonlocal api, end_point
+            # noinspection PyBroadException
+            try:
+                arg_spec = inspect.getfullargspec(api._func)
+            except Exception:
+                arg_spec = inspect.getfullargspec(api._func.__func__)
+            kwargs.update({
+                arg_spec.args[n + 1]: arg for n, arg in enumerate(args)
+            })
+            rest_method = api._func._bantam_web_api.method
+            if rest_method.value == RestMethod.GET.value:
+                url_args = cls._generate_url_args(kwargs=kwargs)
+                url = f"{base_url}{url_args}"
+                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                    async with session.get(url) as resp:
+                        resp.raise_for_status()
+                        async for data, _ in resp.content.iter_chunks():
+                            if data:
+                                if api.return_type == str and data[-1] == 0:
+                                    data = data[:-1]
+                                data = data.decode('utf-8')
+                                yield conversions.from_str(data, api.return_type)
+            else:
+                payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
+                                      for k, v in kwargs.items()})
+                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                    async with session.post(base_url, data=payload) as resp:
+                        async for data, _ in resp.content.iter_chunks():
+                            resp.raise_for_status()
+                            if data:
+                                data = data.decode('utf-8')
+                                yield conversions.from_str(data, api.return_type)
+
+        setattr(clazz, name, class_method_streamed)
+
+    @classmethod
+    def _add_instance_method(cls, clazz: Type, impl_name: str, end_point: str, method,
+                             common_headers: dict):
+        # class/static methods
+        # noinspection PyProtectedMember
+        # noinspection PyProtectedMember
+        name = method.__name__
+        api: API = method._bantam_web_api
+        base_url = f"{end_point}/{impl_name}/{name}"
+
+        # noinspection PyDecorator,PyShadowingNames
+        @wraps(method)
+        async def instance_method(self, *args, **kwargs_):
+            nonlocal api, end_point
+            # noinspection PyBroadException
+            try:
+                arg_spec = inspect.getfullargspec(api._func)
+            except Exception:
+                arg_spec = inspect.getfullargspec(api._func.__func__)
+            kwargs_.update({
+                arg_spec.args[n]: arg for n, arg in enumerate(args)
+            })
+            # noinspection PyBroadException
+            rest_method = api._func._bantam_web_api.method
+            if rest_method.value == RestMethod.GET.value:
+                url_args = cls._generate_url_args(self_id=self.self_id, kwargs=kwargs_)
+                url = f"{base_url}{url_args}"
+                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                    async with session.get(url) as resp:
+                        resp.raise_for_status()
+                        data = (await resp.content.read()).decode('utf-8')
+                        return conversions.from_str(data, api.return_type)
+            else:
+                kwargs_['self'] = self.self_id
+                payload = json.dumps({conversions.to_str(k): conversions.normalize_to_json_compat(v)
+                                      for k, v in kwargs_.items()})
+                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                    async with session.post(base_url, data=payload) as resp:
+                        resp.raise_for_status()
+                        data = (await resp.content.read()).decode('utf-8')
+                        if api.is_constructor:
+                            self_id = json.loads(data)['self_id']
+                            return clazz(self_id)
+                        return conversions.from_str(data, api.return_type)
+
+        setattr(clazz, name, instance_method)
+
+    @classmethod
+    def _add_instance_method_streamed(cls, clazz: Type, impl_name: str, end_point: str, method,
+                                      common_headers: dict):
+        # class/static methods
+        # noinspection PyProtectedMember
+        # noinspection PyProtectedMember
+        name = method.__name__
+        api: API = method._bantam_web_api
+        base_url = f"{end_point}/{impl_name}/{name}"
+
+        async def instance_method_streamed(self, *args, **kwargs_):
+            nonlocal api, end_point, base_url
+            arg_spec = inspect.getfullargspec(api._func)
+            kwargs_.update({
+                arg_spec.args[n + 1]: arg for n, arg in enumerate(args)
+            })
+            rest_method = api.method
+            if rest_method == RestMethod.GET:
+                url_args = cls._generate_url_args(self_id=self.self_id, kwargs=kwargs_)
+                url = f"{base_url}{url_args}"
+                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                    async with session.get(url) as resp:
+                        resp.raise_for_status()
+                        async for data, _ in resp.content.iter_chunks():
+                            if data:
+                                if api.return_type == str and data[-1] == 0:
+                                    data = data[:-1]
+                                data = data.decode('utf-8')
+                                yield conversions.from_str(data, api.return_type)
+            else:
+                url = f"{base_url}?self={self.self_id}"
+                kwargs_['self'] = self.self_id
+                payload = json.dumps({k: conversions.to_str(v) for k, v in kwargs_.items()})
+                async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
+                    async with session.post(url, data=payload) as resp:
+                        resp.raise_for_status()
+                        async for data, _ in resp.content.iter_chunks():
+                            if data:
+                                if api.return_type == str and data[-1] == 0:
+                                    data = data[:-1]
+                                data = data.decode('utf-8')
+                                yield conversions.from_str(data, api.return_type)
+        setattr(clazz, name, instance_method_streamed)
+
+    # noinspection PyPep8Naming
+    @classmethod
+    def Client(cls: C, end_point: str, impl_name: Optional[str] = None,
+               common_headers: Optional[dict] = None) -> C:
+        if cls == WebInterface:
+            raise Exception("Must call Client with concrete class of WebInterface, not WebInterface itself")
+        if impl_name is None:
+            if not cls.__name__.endswith('Interface'):
+                raise Exception("Call to Client must specify impl_name explicitly since class name does not end in "
+                                "'Interface'")
+            impl_name = cls.__name__[:-len('Interface')]
+        while end_point.endswith('/'):
+            end_point = end_point[:-1]
+        key = f"{cls.__name__}.{end_point}"
+        if key in WebInterface._clients:
+            return WebInterface._clients[key]
+
+        class Impl:
+
+            def __init__(self, self_id: str):
+                super().__init__()
+                self._id = self_id
+
+            @property
+            def self_id(self):
+                return self._id
+
+        non_class_methods = inspect.getmembers(cls, predicate=inspect.isfunction)
+        for name, method in non_class_methods:
+            if isinstance(inspect.getattr_static(cls, name), staticmethod):
+                if hasattr(method, '_bantam_web_api'):
+                    raise Exception(f"Static method {name} of {cls.__name__} cannot have @web_api decorator. "
+                                    "WebInterface's can only have instance and class methods that are @web_api's")
+                continue
+            if not inspect.iscoroutinefunction(method) and not inspect.isasyncgenfunction(method):
+                raise Exception(f"Function {name} of {cls.__name__} is not async as expected.")
+            if isinstance(inspect.getattr_static(cls, name), staticmethod):
+                raise Exception(f"Method {name} of {cls.__name__}")
+            else:
+                if inspect.isasyncgenfunction(method):
+                    cls._add_instance_method_streamed(Impl, impl_name, end_point, method, common_headers)
+                else:
+                    cls._add_instance_method(Impl, impl_name, end_point, method, common_headers)
+
+        class_methods = inspect.getmembers(cls, predicate=inspect.ismethod)
+        for name, method in class_methods:
+            if name == 'Client' or name.startswith('_'):
+                continue
+            if not inspect.iscoroutinefunction(method) and not inspect.isasyncgenfunction(method):
+                raise Exception(f"Function {name} of {cls.__name__} is not async as expected.")
+            if inspect.isasyncgenfunction(method):
+                cls._add_class_method_streamed(Impl, impl_name, end_point, method, common_headers)
+            else:
+                cls._add_class_method(Impl, impl_name, end_point, method, common_headers)
 
-        return ClientFactory()
+        WebInterface._clients[key] = Impl
+        return Impl
```

### Comparing `bantam-2.0.9/src/bantam/conversions.py` & `bantam-2.1.0/src/bantam/conversions.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         json_data = normalize_to_json_compat(val.value)
     elif type(val) in (str, int, float, bool):
         json_data = val
     elif type(val) in [dict] or (getattr(type(val), '_name', None) in ('Dict', 'Mapping')):
         json_data = {}
         for key, value in val.items():
             json_data[to_str(key)] = normalize_to_json_compat(value)
-    elif type(val) in [list] or (getattr(type(val), '_name', None) in ('List', )):
+    elif type(val) in [list, set, tuple] or (getattr(type(val), '_name', None) in ('List', 'Set', 'Tuple')):
         json_data = []
         for value in val:
             json_data.append(normalize_to_json_compat(value))
     else:
         raise RuntimeError(f"Unsupported type for conversion: {type(val)}")
     return json_data
 
@@ -39,14 +39,15 @@
         return None
     if hasattr(typ, '_name') and (str(typ).startswith('typing.Union') or str(typ).startswith('typing.Optional')):
         for arg in typ.__args__:
             if arg in (str, int, float, ) and type(json_data) == arg:
                 return json_data
             elif arg in (str, int, float):
                 continue
+            # noinspection PyBroadException
             try:
                 return normalize_from_json(json_data, arg)
             except Exception:
                 continue
     if _issubclass_safe(typ, Enum):
         for key in typ.__members__:
             t = type(typ.__members__[key].value)
@@ -56,32 +57,29 @@
                 return typ(v)
             except Exception:
                 continue
         return typ(json_data)
     elif typ == str:
         return json_data
     elif typ in (int, float):
-        return json_data
+        return typ(json_data)
     elif typ == bool:
         return str(json_data).lower() == 'true'
     elif getattr(typ, '_name', None) in ('Dict', 'Mapping'):
         key_typ, elem_typ = typ.__args__
         return {
             normalize_from_json(k, key_typ):  normalize_from_json(v, elem_typ)
             for k, v in json_data.items()
         }
     elif getattr(typ, '_name', None) in ('List', ):
-        elem_typ = typ.__args__[0]
-        return [normalize_from_json(value, elem_typ) for value in json_data]
+        return [normalize_from_json(value, typ.__args__[0]) for index, value in enumerate(json_data)]
     elif getattr(typ, '_name', None) in ('Set', ):
-        elem_typ = typ.__args__[0]
-        return {normalize_from_json(value, elem_typ) for value in json_data}
+        return {normalize_from_json(value, typ.__args__[0]) for index, value in enumerate(json_data)}
     elif getattr(typ, '_name', None) in ('Tuple', ):
-        elem_typ = typ.__args__[0]
-        return tuple(normalize_from_json(value, elem_typ) for value in json_data)
+        return tuple(normalize_from_json(value, typ.__args__[index]) for index, value in enumerate(json_data))
     elif hasattr(typ, '__dataclass_fields__'):
         return typ(**{
             name: normalize_from_json(json_data[name], field.type)
             for name, field in typ.__dataclass_fields__.items()
         })
     else:
         raise TypeError(f"Unsupported typ for web api: '{typ}'")
```

### Comparing `bantam-2.0.9/src/bantam/decorators.py` & `bantam-2.1.0/src/bantam/decorators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+import sys
 from typing import Any, Callable, Awaitable, Union, Optional, Dict
 
 from aiohttp.web import Request, Response
 from aiohttp.web_response import StreamResponse
 from aiohttp import ClientTimeout
 
 from bantam.api import RestMethod
@@ -46,36 +47,44 @@
     :param expire_obj: for instance methods only, epxire the object upon successful completion of that call
     :return: callable decorator
     """
     from .http import WebApplication
     if not isinstance(content_type, str):
         raise Exception("@web_api must provide one str argument which is the content type")
 
-    def wrapper(obj: Union[WebApi, staticmethod]):
-        is_static = isinstance(obj, staticmethod)
-        is_classmethod = isinstance(obj, classmethod)
-        if not (is_static or is_classmethod) and is_constructor:
-            raise TypeError("@web_api's that are declared constructors must be static methods")
-        if is_static and expire_obj:
+    def wrapper(func: Union[WebApi, staticmethod, classmethod]) -> Union[WebApi, staticmethod, classmethod]:
+        if not inspect.ismethod(func):
+            args = inspect.signature(func)
+            first_arg = list(args.parameters.keys())[0] if args else None
+            is_static = first_arg not in {'self', 'cls'}
+            is_class_method = first_arg == 'cls'
+        else:
+            is_static = isinstance(func, staticmethod)
+            is_class_method = isinstance(func, classmethod)
+        if not (is_static or is_class_method or is_class_method) and is_constructor:
+            raise TypeError("@web_api's that are declared constructors must be static or class methods")
+        if (is_static or is_class_method) and expire_obj:
             raise TypeError("@web_api's expire_obj param can only be set True for instance methods")
-        if is_static:
-            obj = obj.__func__
-        if not is_static and not is_classmethod and not inspect.ismethod(obj) and not inspect.isfunction(obj):
+        if not is_static and not is_class_method and not inspect.ismethod(func) and not inspect.isfunction(func):
             raise TypeError("@web_api should only be applied to @classmethod's, @staticmethods or instance methods")
-        if (not is_classmethod and obj.__name__.startswith('_'))\
-            or (is_classmethod and obj.__func__.__name__.startswith('_')):
+        if func.__name__.startswith('_'):
             raise TypeError("names of web_api methods must not start with underscore")
         # noinspection PyProtectedMember
         # clazz = WebApplication._instance_methods_class_map[obj] if not isinstance(obj, staticmethod) else None
-        obj._bantam_web_method = method
-        return WebApplication._func_wrapper(None,
-                                            obj,
+        func._bantam_web_method = method
+
+        def get_class_that_defined_method():
+            return func.__qualname__.split('.')[0]
+
+        return WebApplication._func_wrapper((func.__module__, get_class_that_defined_method())
+                                                if is_class_method else None,
+                                            func,
                                             timeout=timeout,
-                                            is_instance_method=not is_static and not is_classmethod,
-                                            is_class_method=is_classmethod,
+                                            is_instance_method=not is_static and not is_class_method,
+                                            is_class_method=is_class_method,
                                             method=method,
                                             content_type=content_type,
                                             is_constructor=is_constructor,
                                             expire_on_exit=expire_obj,
                                             uuid_param=uuid_param,
                                             preprocess=preprocess,
                                             postprocess=postprocess)
```

### Comparing `bantam-2.0.9/src/bantam/http.py` & `bantam-2.1.0/src/bantam/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,29 +293,31 @@
         :param reuse_port: tells the kernel to allow this endpoint to be bound to the same port as other existing
             endpoints are bound to, so long as they all set this flag when being created. This option is not supported
             on Windows.
         """
         # noinspection PyProtectedMember
         from aiohttp.web import _run_app as web_run_app
         for module in modules:
-            # ensures web api's are loaded:
-            mod = importlib.import_module(module)
+            if not module in sys.modules:
+                mod = importlib.import_module(module)
+            else:
+                mod = sys.modules.get(module)
             for api in list(self.module_mapping_get.get(module, {}).values()):
                 if api.name in ['_expire']:
                     continue
-                if api.is_class_method:
-                    class_name, method_name = api._real_func.__qualname__.split('.')
-                    api._func = getattr(getattr(mod, class_name), method_name)
+                #if api.is_class_method:
+                    #class_name, method_name = api._real_func.__qualname__.split('.')
+                    #api._func = getattr(getattr(mod, class_name), method_name)
                 self._process_module_classes(mod, api)
             for api in self.module_mapping_post.get(module, {}).values():
                 if api.name in ['_expire']:
                     continue
-                if api.is_class_method:
-                    class_name, method_name = api._real_func.__qualname__.split('.')
-                    api._func = getattr(getattr(mod, class_name), method_name)
+                #if api.is_class_method:
+                    #class_name, method_name = api._real_func.__qualname__.split('.')
+                    #api._func = getattr(getattr(mod, class_name), method_name)
                 self._process_module_classes(mod, api)
         allowed_get_routes = {}
         for module in [m for m in modules if m in self.module_mapping_get]:
             allowed_get_routes.update(self.module_mapping_get[module])
         for route, api_get in allowed_get_routes.items():
             log.debug(f">>>>>>>>>> GET ROUTE {route}")
             invoke = self.routes_get[route]
@@ -379,15 +381,15 @@
         # noinspection PyProtectedMember
         def process_class(clazz_: Type):
             if hasattr(clazz_, '_expire') or hasattr(clazz_, '_create'):
                 raise TypeError("Classes with @web_api applied cannot have methods named _expire nor _create")
 
             # noinspection PyDecorator
             @staticmethod
-            async def _create(*args, **kargs) -> str:
+            async def _create(*args, **kargs) -> clazz_:
                 if kargs.get('__uuid') or (api.uuid_param is not None and api.uuid_param in kargs):
                     self_id = kargs[api.uuid_param] if api.uuuid_param is not None else kargs['__uuid']
                     del kargs['__uuid']
                     if self_id in self.ObjectRepo.instances:
                         raise HTTPException(404, f"UUid {self_id} already in use. uuid's must be unique")
                 else:
                     self_id = str(uuid_pkg.uuid4())
@@ -398,25 +400,26 @@
                 return instance
 
             clazz_._create = _create
             if hasattr(clazz_, '__init__') and hasattr(clazz_.__init__, '__annotations__'):
                 clazz_._create.__annotations__ = clazz_.__init__.__annotations__ if hasattr(clazz_, '__init__') else {}
             else:
                 clazz._create.__annotations__ = {}
-            clazz_._create.__annotations__['return'] = str
 
             clazz_._create.__doc__ = clazz_.__init__.__doc__ if hasattr(clazz_, '__init__') else f"""
                 Create an instance of {clazz_.__name__} on server, returning a unique string id for the instance.
                 The instance will remain active until /{clazz_.__name__}/expire is invoked.  The sting is used for
                 instance-based ReST methods to act on the created instance on the server.
 
                 :return: unique string id of instance created
                 """
             clazz_._create.__qualname__ = f"{clazz_.__name__}._create"
+            clazz_._create.__annotations__['return'] = clazz_
             _create.__func__.__annotations__ = clazz_._create.__annotations__
+            _create.__annotations__ = clazz_._create.__annotations__
             # noinspection PyProtectedMember
             route_name = f"/{clazz_.__name__}/_create"
             api = API(
                 content_type='text/plain',
                 is_instance_method=False,
                 is_class_method=False,
                 is_constructor=True,
@@ -464,15 +467,15 @@
                 api._clazz = clazz
             if method_found and (api in self._instance_methods or api.is_constructor):
                 if clazz not in self._class_instance_methods or not self._class_instance_methods.get(clazz):
                     process_class(clazz)
                 self._class_instance_methods.setdefault(clazz, []).append(api)
                 self._instance_methods_class_map[api] = clazz
                 if api.is_constructor:
-                    if api._func.__annotations__.get('return') != clazz.__name__:
+                    if api._func.__annotations__.get('return') not in (clazz, clazz.__name__):
                         raise TypeError("@web_api's declared as constructors must return that class's type")
 
                 if api.expire_object:
                     async def wrapped(this, *args, **kargs):
                         try:
                             # noinspection PyProtectedMember
                             return await api._func(this, *args, **kargs)
@@ -481,15 +484,15 @@
                                 uuid = self.ObjectRepo.by_instance[this]
                                 del self.ObjectRepo.by_instance[this]
                                 del self.ObjectRepo.instances[uuid]
 
                     setattr(clazz, api.name, wrapped)
             elif method_found and api in self._all_apis:
                 if api.is_constructor:
-                    if api._func.__annotations__.get('return') != clazz.__name__:
+                    if api._func.__annotations__.get('return') not in (clazz, clazz.__name__):
                         raise TypeError("@web_api's declared as constructors must return that class's type")
                 self._class_instance_methods.setdefault(clazz, [])  # create an empty list of instance methods at least
 
     @classmethod
     def _func_wrapper(cls, clazz, func: WebApi,
                       is_instance_method: bool,
                       is_class_method: bool,
@@ -510,29 +513,26 @@
         """
         api = API(clazz, func, method=method, content_type=content_type, is_instance_method=is_instance_method,
                   is_class_method=is_class_method,
                   is_constructor=is_constructor, expire_on_exit=expire_on_exit, uuid_param=uuid_param, timeout=timeout)
         func._bantam_web_api = api
         if hasattr(func, '__func__'):
             func.__func__._bantam_web_api = api
+            func = func.__func__
         if is_instance_method:
-            if not inspect.iscoroutinefunction(func) and not inspect.isasyncgenfunction(func):
-                raise ValueError("the @web_api decorator can only be applied to classes with public "
-                                 f"methods that are coroutines (async); see {api.qualname}")
             cls._instance_methods.append(api)
-        elif not is_class_method:
-            if not inspect.iscoroutinefunction(func) and not inspect.isasyncgenfunction(func):
-                raise ValueError("the @web_api decorator can only be applied to methods that are coroutines (async)")
-        else:
-            if not inspect.iscoroutinefunction(func.__func__) and not inspect.isasyncgenfunction(func.__func__):
-                raise ValueError("the @web_api decorator can only be applied to methods that are coroutines (async)")
+        if not inspect.iscoroutinefunction(func) and not inspect.isasyncgenfunction(func):
+            raise ValueError("the @web_api decorator can only be applied to classes with public "
+                             f"methods that are coroutines (async); see {api.qualname}")
         cls._all_methods.append(api)
         name = api.qualname.replace('__init__', 'create').replace('._expire', '.expire')
         name_parts = name.split('.')[-2:]
         route = '/' + '/'.join(name_parts)
+        if '__isabstractmethod__' in func.__dict__:
+            return func
 
         async def invoke(app: WebApplication, request: Request):
             nonlocal preprocess, postprocess
             try:
                 preprocess = preprocess or app.preprocessor
                 try:
                     addl_args = (preprocess(request) or {}) if preprocess else {}
@@ -616,15 +616,21 @@
                         "A self request parameter is needed. No instance provided for call to instance method")
                 instance = cls.ObjectRepo.instances.get(self_id)
                 if instance is None:
                     raise ValueError(f"No instance found for request with 'self' id of {self_id}")
                 del kwargs['self']
                 result = api(instance, **kwargs)
             elif api.is_class_method:
-                result = api(api.__self__, *kwargs)
+                if isinstance(api.clazz, tuple):
+                    module_name, class_name = api.clazz
+                    api._clazz = getattr(sys.modules.get(module_name), class_name)
+                if 'cls' not in kwargs:
+                    result = api(**kwargs, cls=api.clazz)
+                else:
+                    result = api(**kwargs)
             else:
                 # call the underlying function:
                 result = api(**kwargs)
             if inspect.isasyncgen(result):
                 #################
                 #  streamed response through async generator:
                 #################
@@ -634,16 +640,16 @@
                 response = StreamResponse(status=200, reason='OK', headers={'Content-Type': content_type})
                 await response.prepare(request)
                 try:
                     # iterate to get the one (and hopefully only) yielded element:
                     # noinspection PyTypeChecker
                     async for res in result:
                         serialized = _serialize_return_value(res, encoding)
-                        if not isinstance(res, bytes):
-                            serialized += b'\n'
+                        if isinstance(res, str):
+                            serialized += b'\0'
                         await response.write(serialized)
                 except Exception as e:
                     print(str(e))
                     raise asyncio.CancelledError(f"Error in server-side logic: {e}") from e
                 await response.write_eof()
                 return response
             else:
@@ -731,17 +737,14 @@
                     kwargs = {key: await request.read()}
                 elif typ == AsyncLineIterator:
                     kwargs = {key: line_by_line_response(request)}
                 elif typ == AsyncChunkIterator:
                     kwargs = {key: streamed_bytes_arg_value(request)}
                 for k, v in kwargs.items():
                     assert type(v) == str, f"key {k}={v} is of type {str(type(v))}\n{kwargs}"
-                #kwargs = {k: _convert_request_param(v, api.arg_annotations[k]) if k != 'self' else v
-                #          for k, v in kwargs.items()}
-                # noinspection PyTypeChecker
                 kwargs.update({k: _convert_request_param(v, api.synchronous_arg_annotations[k]) if k != 'self' else v
                                for k, v in request.query.items() if k in api.synchronous_arg_annotations})
             else:
                 # treat payload as json string:
                 bytes_response = await request.read()
                 json_dict = json.loads(bytes_response.decode('utf-8'))
                 for k in [p for p in json_dict if p not in api.arg_annotations and p != 'self']:
@@ -755,14 +758,16 @@
             # call the underlying function:
             if addl_args:
                 kwargs.update(addl_args)
             for k, v in kwargs.items():
                 if k != 'self':
                     value_type = api.arg_annotations[k]
                     kwargs[k] = normalize_from_json(v, value_type)
+                else:
+                    kwargs[k] = v
             if api.is_instance_method:
                 self_id = kwargs.get('self')
                 if self_id is None:
                     raise ValueError("No instance provided for call to instance method")
                 instance = cls.ObjectRepo.instances.get(self_id)
                 if instance is None:
                     try:
@@ -773,15 +778,19 @@
                     except:
                         raise ValueError(f"No instance id found for request {self_id}")
                 del kwargs['self']
                 awaitable = api(instance, **kwargs)
                 if api.expire_object:
                     del cls.ObjectRepo.instances[self_id]
             elif api.is_class_method:
-                awaitable = api(**kwargs)
+
+                if isinstance(api.clazz, tuple):
+                    module_name, class_name = api.clazz
+                    api._clazz = getattr(sys.modules.get(module_name), class_name)
+                awaitable = api(**kwargs, cls=api.clazz)
             else:
                 awaitable = api(**kwargs)
             if inspect.isasyncgen(awaitable):
                 #################
                 #  streamed response through async generator:
                 #################
                 # underlying function has yielded a result rather than turning
@@ -791,27 +800,46 @@
                 response = StreamResponse(status=200, reason='OK', headers={'Content-Type': content_type})
                 await response.prepare(request)
                 try:
                     # iterate to get the one (and hopefully only) yielded element:
                     # noinspection PyTypeChecker
                     async for res in awaitable:
                         serialized = _serialize_return_value(res, encoding)
-                        if not isinstance(res, bytes):
-                            serialized += b'\n'
+                        if isinstance(res, str):
+                            serialized += b'\0'
                         await response.write(serialized)
                 except Exception as e:
                     print(str(e))
                     await async_q.put(None)
-                    raise RuntimeError(f"Execption in server-side logic: {e}") from e
+                    raise RuntimeError(f"Exception in server-side logic: {e}") from e
                 await response.write_eof()
             else:
                 #################
                 #  regular response
                 #################
-                result = _serialize_return_value(await awaitable, encoding)
+                if api.is_constructor:
+                    instance = await awaitable
+                    if api.clazz and hasattr(api.clazz, '__aenter__'):
+                        await instance.__aenter__()
+                    if hasattr(api.clazz, 'jsonrepr'):
+                        repr_ = api.clazz.jsonrepr(result)
+                        uuid = repr_.get(api.uuid_param)
+                        content_type = 'application/json'
+                        result = json.dumps(repr_)
+                    else:
+                        uuid = kwargs.get(api.uuid_param, str(uuid_pkg.uuid4()))
+                        result = json.dumps({'uuid': uuid})
+                    cls.ObjectRepo.instances[uuid] = instance
+                    cls.ObjectRepo.by_instance[instance] = uuid
+                    cls.ObjectRepo.expiry[uuid] = asyncio.create_task(cls.ObjectRepo.expire_obj(
+                        uuid, cls.ObjectRepo.DEFAULT_OBJECT_EXPIRATION))
+                    return Response(status=200, body=result if result is not None else b"Success",
+                                    content_type=content_type)
+                else:
+                    result = _serialize_return_value(await awaitable, encoding)
                 return Response(status=200, body=result if result is not None else b"Success",
                                 content_type=content_type)
 
         except TypeError as e:
             return Response(status=400, text=f"Improperly formatted query: {str(e)}")
         except HTTPException as e:
             return Response(status=e.status_code, text=str(e))
@@ -839,15 +867,15 @@
         raise TypeError(f"Converting web request string {value} of {type(value)} to Python type {typ}: {e}\n {text}")
 
 
 def _serialize_return_value(value: Any, encoding: str) -> bytes:
     """
     Serialize a Python value into bytes to return through a Rest API.  If a basic type such as str, int or float, a
     simple str conversion is done, then converted to bytes.  If more complex, the conversion will invoke the
-    'serialize' method of the value, raising TypeError if such a method does not exist or does not have a bare
+    '__str__' method of the value, raising TypeError if such a method does not exist or does not have a bare
     (no-parameter) signature.
 
     :param value: value to convert
     :return: bytes serialized from value
     """
     try:
         if value is None:
```

### Comparing `bantam-2.0.9/src/bantam/js.py` & `bantam-2.1.0/src/bantam/js.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 This prevents potential namespace collisions.  The signatures of the API mimic those defined in the Pyhon codebase,
 with the noted exception of the *onsuccess* and *onerror* callbacks as the first two parameters.
 This is typical of how plain javascript handles asynchronous transactions:  rather than returning a value or raising an
 exception, these callbacks are invoked instead, upon response from the server.
 
 
 """
+import inspect
 import re
 from aiohttp.web_response import Response, StreamResponse
 from typing import Callable, Awaitable, Union
 from typing import Dict, Tuple, List, IO, Type
 from urllib.request import Request
 
 from bantam.api import API, RestMethod
@@ -144,14 +145,16 @@
                 clazz_map = {c.__name__: c for c in WebApplication._class_instance_methods
                              if WebApplication._class_instance_methods[c]}
                 out.write(f"\n{parent_name}.{class_name} = class {{\n".encode(cls.ENCODING))
                 tab += "   "
 
                 if class_name in clazz_map:
                     clazz = clazz_map[class_name]
+                    if inspect.isabstract(clazz):
+                        continue
                     cls._generate_request(out, route=f"/{class_name}/_create",
                                           api=API(clazz, clazz._create, method=RestMethod.GET,
                                                   content_type="test/plain",
                                                   is_instance_method=False, is_constructor=True, expire_on_exit=False),
                                           tab=tab)
                     cls._generate_request(out, route=f"/{class_name}/expire",
                                           api=API(clazz, clazz._expire, method=RestMethod.GET,
@@ -254,18 +257,16 @@
         lines = [line for line in docs.splitlines() if not line.strip().startswith(':return')]
         docs = '\n'.join(lines) + '\n'
         out.write(docs.encode(cls.ENCODING))
 
     @classmethod
     def _generate_request(cls, out: IO, route: str, api: API, tab: str):
         func = api._func
-        if '__func__' in func:
-            func = func.__func__
         arg_count = func.__code__.co_argcount
-        if 'self' in func.__code__.co_varnames:
+        if 'self' in func.__code__.co_varnames or 'cls' in func.__code__.co_varnames:
             arg_count -= 1
 
         if not api.name.startswith('_') and arg_count != len(api.arg_annotations):
             raise Exception(f"Not all arguments of '{api.qualname}' have type hints.  This is required for web_api")
         if api.has_streamed_response is True:
             callback = 'onreceive'
             state = 3
@@ -443,15 +444,15 @@
                        bool: "'true'== val",
                        dict: "JSON.parse(val)",
                        list: "JSON.parse(val)",
                        None: "null"}.get(response_type) or 'request.response.substr(request.seenBytes)'
         if streamed_response and response_type not in [bytes, str, None]:
             convert_codeblock = f"""
 {tab}    // TODO: Can we clean this up a little?
-{tab}    let vals = request.response.substr(request.seenBytes).trim().split('\\n');
+{tab}    let vals = request.response.substr(request.seenBytes).trim().split('\\0');
 {tab}    for (var i = 0; i < vals.length; ++i) {{
 {tab}       let val = vals[i];
 {tab}       let done = (i == vals.length -1) && (request.readyState == XMLHttpRequest.DONE);
 {tab}       if (val !== ''){{
 {tab}          if (buffered != null){{{callback}(buffered, false); buffered = null;}}
 {tab}          buffered = {convert};
 {tab}          if (typeof buffered === 'numbered' && isNaN(buffered)){{
@@ -463,15 +464,15 @@
 {tab}    }}
 {tab}    if (buffered !== null && request.readyState == XMLHttpRequest.DONE){{{callback}(buffered, true);}}
 {tab}    request.seenBytes = request.response.length;"""
         elif streamed_response and response_type == str:
             convert_codeblock = f"""
 {tab}    // TODO: Can we clean this up a little?
 {tab}    let chunk = request.response.substr(request.seenBytes).trim();
-{tab}    let vals = chunk.length == 0?[]:chunk.split('\\n');
+{tab}    let vals = chunk.length == 0?[]:chunk.split('\\0');
 {tab}    if (buffered !== null){{{callback}(buffered, request.readyState == XMLHttpRequest.DONE); buffered = null; }}
 {tab}    for (var i = 0; i < vals.length-1 ; ++i) {{
 {tab}       let val = vals[i];
 {tab}       {callback}(val, false);
 {tab}    }}
 {tab}    if (vals.length > 0){{buffered = vals[vals.length-1];}}
 {tab}    if (buffered !== null && request.readyState == XMLHttpRequest.DONE){{{callback}(buffered, true);}}
```

### Comparing `bantam-2.0.9/src/bantam/js_async.py` & `bantam-2.1.0/src/bantam/js_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 
 The code maintains the same hierarchy in namespaces as modules in Python, albeit under a global *bantam* namespace.
 This prevents potential namespace collisions.  The javascript API mimics the signature of the Python API, including
 async generators/iterator usage.
 
 
 """
+import inspect
+import sys
+
 from aiohttp.web_response import Response, StreamResponse
 from typing import Callable, Awaitable, Union
 from typing import Dict, Tuple, List, IO
 from urllib.request import Request
 
 from bantam.api import API, APIDoc, RestMethod
 
@@ -130,15 +133,15 @@
             if (resp.done){
                 break;
             }
             if (return_is_bytes){
                yield resp.value;
             } else {
                let value = new TextDecoder().decode(resp.value);
-               for (var val of value.split('\\n')){
+               for (var val of value.split('\\0')){
                    if(val){
                       yield convert(val);
                    }
                }
            }
         }
     }
@@ -219,15 +222,15 @@
             if (resp.done){
                 break;
             }
             if (return_is_bytes){
                yield resp.value;
             } else {
                let value = new TextDecoder().decode(resp.value);
-               for (var val of value.split('\\n')){
+               for (var val of value.split('\\0')){
                    if(val){
                       yield convert(val);
                    }
                }
            }
         }
     }
@@ -332,21 +335,29 @@
         tab = ""
 
         def process_namespace(ns: cls.Namespace, parent_name: str):
             nonlocal tab
             for name_, child_ns in ns.child_namespaces.items():
                 out.write(f"{parent_name}.{name_} = class {{}}\n".encode(cls.ENCODING))
                 process_namespace(child_ns, parent_name + '.' + name_)
+            clazz_map = {c.__name__: c for c in WebApplication._class_instance_methods
+                         if WebApplication._class_instance_methods[c]}
             for class_name, routes in ns.classes.items():
+                if class_name in clazz_map:
+                    clazz = clazz_map[class_name]
+                    if inspect.isabstract(clazz):
+                        continue
                 out.write(f"\n{parent_name}.{class_name} = class {{\n".encode(cls.ENCODING))
-                clazz_map = {c.__name__: c for c in WebApplication._class_instance_methods
-                             if WebApplication._class_instance_methods[c]}
-                for api in [api for api in WebApplication._all_methods if (api.qualname.startswith(class_name)
+                for api in [api for api in WebApplication._all_methods if (api.qualname.split('.')[0] == class_name
                                                                            and api.clazz is not None)]:
                     if api.is_constructor:
+                        if isinstance(api.clazz, tuple):
+                            module_name, class_name = api.clazz
+                            module = sys.modules.get(module_name)
+                            api._clazz = getattr(module, class_name)
                         clazz_map[api.clazz.__name__] = api.clazz
                 if class_name in clazz_map:
                     clazz = clazz_map[class_name]
                     cls._generate_request(out, route=f"/{class_name}/_create",
                                           api=API(clazz, clazz._create, method=RestMethod.GET,
                                                   content_type="text/plain",
                                                   is_instance_method=False,
@@ -417,21 +428,22 @@
         if hasattr(api.return_type, '__dataclass_fields__'):
             convert = "convert_complex"
         elif str(api.return_type).startswith('typing.Dict') or str(api.return_type).startswith('typing.List'):
             convert = "convert_complex"
         else:
             convert = {str: "convert_str",
                        int: "convert_int",
-                       int: "convert_int",
                        float: "convert_float",
                        bool: "convert_bool",
                        bytes: "convert_bytes",
                        dict: "convert_complex",
                        list: "convert_complex",
-                       None: "convert_None"}[api.return_type]
+                       tuple: "convert_complex",
+                       set: "convert_complex",
+                       None: "convert_None"}.get(api.return_type, "convert_complex")
         tab += "   "
         self_param_code = f"{tab}  \"self\": this.self_id{',' if argnames else ''}" + '\n' if offset == 1 else ""
         param_code = ',\n'.join([f"{tab}   \"{argname}\": {argname}" for argname in argnames])
         param_code = f"""
 {tab}let params = {{
 {self_param_code}{param_code}
 {tab}}}"""
```

### Comparing `bantam-2.0.9/src/bantam/pythonclient.py` & `bantam-2.1.0/src/bantam/pythonclient.py`

 * *Files identical despite different names*

### Comparing `bantam-2.0.9/src/bantam.egg-info/PKG-INFO` & `bantam-2.1.0/src/bantam.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.0.9
+Version: 2.1.0
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
+Download-URL: https://github.com/bantam/dist/2.1.0
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
-Download-URL: https://github.com/bantam/dist/2.0.9
 Keywords: auto web api python
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
-License-File: LICENSE.txt
 
 
 Bantam is a Python package for building http-based micro-services.
 It abstracts away any knowledge of routes, mappings and translations
 between javascript and Python.  It even provides a means of
 auto-generating the javascript client interface to you app
 on the fly and serve it to web-based/javascript-based clients.
 
 See https://nak.github.io/bantam_docs/ for details.
 
     
-
```

### Comparing `bantam-2.0.9/src/bantam.egg-info/SOURCES.txt` & `bantam-2.1.0/src/bantam.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-LICENSE.txt
 README
-README.md
 requirements.txt
 setup.cfg
 setup.py
 src/bantam/__init__.py
 src/bantam/api.py
 src/bantam/client.py
 src/bantam/conversions.py
@@ -17,12 +15,13 @@
 src/bantam.egg-info/SOURCES.txt
 src/bantam.egg-info/dependency_links.txt
 src/bantam.egg-info/entry_points.txt
 src/bantam.egg-info/requires.txt
 src/bantam.egg-info/top_level.txt
 src/bantam/autogen/__init__.py
 src/bantam/autogen/main.py
-test/test_client.py
+test/test_client_get.py
+test/test_client_post.py
 test/test_conversions.py
 test/test_decorators.py
 test/test_js.py
 test/test_js_async.py
```

### Comparing `bantam-2.0.9/test/test_js.py` & `bantam-2.1.0/test/test_js.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 import json
 import os
-import subprocess
 import sys
 import webbrowser
 from contextlib import suppress
 from pathlib import Path
 from typing import AsyncGenerator, Optional, Dict, Any
 
 import pytest
@@ -43,16 +42,16 @@
         return f"called basic post operation on instance {self._value}: {param1} {param2} {param3} {param4}"
 
 
 class RestAPIExample:
 
     result_queue : Optional[asyncio.Queue] = None
 
-    @web_api(content_type='text/plain', method=RestMethod.GET)
     @staticmethod
+    @web_api(content_type='text/plain', method=RestMethod.GET)
     async def api_get_basic(param1: int, param2: bool, param3: float, param4: str = "text") -> str:
         """
         Some sort of doc
         :param param1:
         :param param2:
         :param param3:
         :param param4:
```

### Comparing `bantam-2.0.9/test/test_js_async.py` & `bantam-2.1.0/test/test_js_async.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from aiohttp.web_request import Request
 from aiohttp.web_response import Response
 from bantam.http import WebApplication
 
 
 import sys
 sys.path.insert(0, os.path.dirname(__file__))
-from example.class_rest_example import RestAPIExampleAsync
+from class_rest_get import RestAPIExampleAsync
 
 
 class TestJavascriptGenerator:
 
     @pytest.mark.asyncio
     async def test_generate_basic(self):
         def assert_preprocessor(request: Request) -> Dict[str, Any]:
@@ -54,15 +54,15 @@
             browser.open("http://localhost:8080/static/index_async.html")
             result = await RestAPIExampleAsync.result_queue.get()
             await asyncio.sleep(2.0)
             await app.shutdown()
             return result
 
         try:
-            completed, _ = await asyncio.wait([app.start(modules=['example.class_rest_example']),
+            completed, _ = await asyncio.wait([app.start(modules=['class_rest_get']),
                                                launch_browser()], timeout=100000, return_when=asyncio.FIRST_COMPLETED)
             results = [c.result() for c in completed if c is not None]
         except Exception as e:
             assert False, f"Exception processing javascript results: {traceback.format_exc()}"
         if any([isinstance(r, Exception) for r in results]):
             assert False, "At least one javascript test failed. See browser window for details"
         assert results[0] == "PASSED", \
```

