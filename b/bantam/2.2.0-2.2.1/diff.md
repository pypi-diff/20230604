# Comparing `tmp/bantam-2.2.0.tar.gz` & `tmp/bantam-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.2.0.tar", last modified: Sun Jun  4 14:54:06 2023, max compression
+gzip compressed data, was "bantam-2.2.1.tar", last modified: Sun Jun  4 16:08:02 2023, max compression
```

## Comparing `bantam-2.2.0.tar` & `bantam-2.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 14:54:06.511878 bantam-2.2.0/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-04 14:54:06.511878 bantam-2.2.0/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.2.0/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-03 15:15:17.000000 bantam-2.2.0/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-04 14:54:06.511878 bantam-2.2.0/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-04 14:50:20.000000 bantam-2.2.0/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 14:54:06.511878 bantam-2.2.0/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 14:54:06.511878 bantam-2.2.0/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4011 2023-06-04 04:49:42.000000 bantam-2.2.0/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    10329 2023-06-04 03:58:24.000000 bantam-2.2.0/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 14:54:06.511878 bantam-2.2.0/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.2.0/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.2.0/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    17999 2023-06-04 14:52:43.000000 bantam-2.2.0/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.2.0/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4399 2023-06-04 13:45:48.000000 bantam-2.2.0/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    43836 2023-06-04 14:40:10.000000 bantam-2.2.0/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.2.0/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.2.0/src/bantam/js_async.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.2.0/src/bantam/pythonclient.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 14:54:06.511878 bantam-2.2.0/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-04 14:54:06.000000 bantam-2.2.0/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-04 14:54:06.000000 bantam-2.2.0/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-04 14:54:06.000000 bantam-2.2.0/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-04 14:54:06.000000 bantam-2.2.0/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-04 14:54:06.000000 bantam-2.2.0/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-04 14:54:06.000000 bantam-2.2.0/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 14:54:06.511878 bantam-2.2.0/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4472 2023-06-04 02:18:21.000000 bantam-2.2.0/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4517 2023-06-04 02:21:15.000000 bantam-2.2.0/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4573 2023-06-04 14:26:39.000000 bantam-2.2.0/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.2.0/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.2.0/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.2.0/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     7531 2023-06-03 15:33:20.000000 bantam-2.2.0/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2845 2023-06-04 03:14:39.000000 bantam-2.2.0/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 16:08:02.367650 bantam-2.2.1/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-04 16:08:02.367650 bantam-2.2.1/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.2.1/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-03 15:15:17.000000 bantam-2.2.1/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-04 16:08:02.367650 bantam-2.2.1/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-04 16:07:54.000000 bantam-2.2.1/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 16:08:02.363650 bantam-2.2.1/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 16:08:02.367650 bantam-2.2.1/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4011 2023-06-04 04:49:42.000000 bantam-2.2.1/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    10356 2023-06-04 16:03:49.000000 bantam-2.2.1/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 16:08:02.367650 bantam-2.2.1/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.2.1/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.2.1/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    18406 2023-06-04 16:03:49.000000 bantam-2.2.1/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.2.1/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4399 2023-06-04 13:45:48.000000 bantam-2.2.1/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    44538 2023-06-04 16:03:49.000000 bantam-2.2.1/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.2.1/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.2.1/src/bantam/js_async.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.2.1/src/bantam/pythonclient.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 16:08:02.367650 bantam-2.2.1/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-04 16:08:02.000000 bantam-2.2.1/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-04 16:08:02.000000 bantam-2.2.1/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-04 16:08:02.000000 bantam-2.2.1/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-04 16:08:02.000000 bantam-2.2.1/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-04 16:08:02.000000 bantam-2.2.1/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-04 16:08:02.000000 bantam-2.2.1/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 16:08:02.367650 bantam-2.2.1/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4472 2023-06-04 02:18:21.000000 bantam-2.2.1/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4517 2023-06-04 02:21:15.000000 bantam-2.2.1/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4573 2023-06-04 14:26:39.000000 bantam-2.2.1/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.2.1/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.2.1/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.2.1/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     7531 2023-06-03 15:33:20.000000 bantam-2.2.1/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2845 2023-06-04 03:14:39.000000 bantam-2.2.1/test/test_js_async.py
```

### Comparing `bantam-2.2.0/PKG-INFO` & `bantam-2.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.2.0
+Version: 2.2.1
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.2.0
+Download-URL: https://github.com/bantam/dist/2.2.1
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.2.0/setup.py` & `bantam-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.2.0"
+VERSION = "2.2.1"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.2.0/src/bantam/__init__.py` & `bantam-2.2.1/src/bantam/__init__.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/src/bantam/api.py` & `bantam-2.2.1/src/bantam/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Callable, Awaitable, AsyncGenerator, Dict, List, Optional
+from typing import Callable, Awaitable, AsyncGenerator, Dict, List, Optional, Type
 
 from aiohttp import ClientTimeout
 
 AsyncChunkIterator = Callable[[int], Awaitable[AsyncGenerator[None, bytes]]]
 AsyncLineIterator = AsyncGenerator[None, str]
 
 
@@ -109,20 +109,20 @@
         return self._content_type
 
     @property
     def arg_annotations(self):
         return self._arg_annotations
 
     @property
-    def async_arg_annotations(self) -> Dict[str, str]:
+    def async_arg_annotations(self) -> Dict[str, Type]:
         return self._async_arg_annotations
 
     @property
-    def synchronous_arg_annotations(self) -> List[str]:
-        return [a for a in self._arg_annotations if a not in self._async_arg_annotations]
+    def synchronous_arg_annotations(self) -> Dict[str, Type]:
+        return {a: v for a, v in self._arg_annotations.items() if a not in self._async_arg_annotations}
 
     @property
     def return_type(self):
         return self._return_type
 
     @property
     def has_streamed_request(self) -> bool:
```

### Comparing `bantam-2.2.0/src/bantam/autogen/main.py` & `bantam-2.2.1/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/src/bantam/client.py` & `bantam-2.2.1/src/bantam/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 ...
 ...     def __init__(self):
 ...         self._message_bits = ['I', 'am', 'the', 'very', 'model']
 ...
 ...     @classmethod
 ...     async def constructor(cls) -> "MyServerApiInterface":
 ...        '''
-...        Concreate constructor to create an instance of the class WITH SAEM @web_api DECORATOR AND
+...        Concreate constructor to create an instance of the class WITH SAME @web_api DECORATOR AND
 ...        SIGNATURE
 ...        '''
 ...        return MyServerApi()
 ...
 ...      @classmethod
 ...      async def class_method_api(cls, parm1: str) -> Dict[str, int]:
 ...          '''
@@ -95,15 +95,15 @@
 method above.  The *end_point* parameter specifies the base url to the server that serves up MyServceApi class.
 
 """
 import inspect
 import json
 from abc import ABC
 from functools import wraps
-from typing import Any, Dict, TypeVar, Optional, Type, AsyncIterator
+from typing import Any, Dict, TypeVar, Optional, Type, AsyncIterator, Generic
 
 import aiohttp
 
 from bantam import conversions
 from bantam.api import API, RestMethod
 
 __all__ = ["WebInterface"]
@@ -372,9 +372,18 @@
             if not inspect.iscoroutinefunction(method) and not inspect.isasyncgenfunction(method):
                 raise Exception(f"Function {name} of {cls.__name__} is not async as expected.")
             if inspect.isasyncgenfunction(method):
                 cls._add_class_method_streamed(Impl, impl_name, end_point, method, common_headers)
             else:
                 cls._add_class_method(Impl, impl_name, end_point, method, common_headers)
 
-        WebInterface._clients[key] = Impl
-        return Impl
+        class ImplProper(Impl, Generic[C]):
+            """
+            provides proper typing on return value, without conflicting with Python's abstract class rules
+            which ignore dynamically added methods as above for the concrete implementations
+            """
+
+            def __init__(self, *args, **kwargs):
+                Impl.__init__(self, *args, **kwargs)
+
+        WebInterface._clients[key] = ImplProper[C]
+        return ImplProper[C]
```

### Comparing `bantam-2.2.0/src/bantam/conversions.py` & `bantam-2.2.1/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/src/bantam/decorators.py` & `bantam-2.2.1/src/bantam/decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/src/bantam/http.py` & `bantam-2.2.1/src/bantam/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,16 @@
 
 # noinspection PyUnresolvedReferences
 class WebApplication:
     """
     Main class for running a WebApplication server. See the documentation for *aiohttp* for information on the various
     parameters.  Additional parameters for this class are:
 
-    :static_path: root path to where static files will be kept, mapped to a route "/static", if provided
-    :js_bundle_name: the name of the javascript file, **without** exetension, where the client-side API
+    :param static_path: root path to where static files will be kept, mapped to a route "/static", if provided
+    :param js_bundle_name: the name of the javascript file, **without** extension, where the client-side API
        will be generated, if provided
     """
     _context: Dict[Awaitable, Request] = {}
     _class_instance_methods: Dict[Type, List[API]] = {}
     _instance_methods_class_map: Dict[API, Type] = {}
     _instance_methods: List[API] = []
     _all_methods: List[API] = []
@@ -226,15 +226,15 @@
     def register_route_get(cls, route: str, async_handler: AsyncApi, api: API, module: str) -> None:
         """
         Register the given handler as a GET call. This should be called from the @web_api decorator, and
         rarely if ever called directly
 
         :param route: route to register under
         :param async_handler: the raw handler for handling an incoming Request and returning a Response
-        :param api: the high-level deocrated web_api that will be invoked by the handler
+        :param api: the high-level decorated web_api that will be invoked by the handler
         :param module: module that is holding the @web_api
         """
         if route in cls.routes_get or route in cls.routes_post:
             existing = cls.callables_get.get(route) or cls.callables_post.get(route)
             if existing and (api.module != existing.module or api.name != existing.name):
                 raise cls.DuplicateRoute(
                     f"Route '{route}' associated with {api.module}.{api.name}"
@@ -260,50 +260,60 @@
             existing = cls.callables_get.get(route) or WebApplication.callables_post.get(route)
             raise cls.DuplicateRoute(f"Route '{route}' associated with {api.module}.{api._func.__name__}"
                                      f" already exists here {existing.module}.{existing.name} ")
         cls.routes_post[route] = async_method
         cls.callables_post[route] = api
         cls.module_mapping_post.setdefault(module, {})[route] = api
 
+    # noinspection PyProtectedMember
     @classmethod
     def preprocess_module(cls, module_: str):
         if module_ not in sys.modules:
             mod = importlib.import_module(module_)
         else:
             mod = sys.modules.get(module_)
         for class_name, clazz in inspect.getmembers(mod, predicate=inspect.isclass):
             from .client import WebInterface
             if issubclass(clazz, WebInterface):
                 ancestors = clazz.__mro__
                 for ancestor in ancestors:
                     if ancestor == clazz:
                         continue
                     methods = inspect.getmembers(ancestor, predicate=inspect.ismethod) + \
-                              inspect.getmembers(ancestor, predicate=inspect.isfunction)
+                        inspect.getmembers(ancestor, predicate=inspect.isfunction)
                     for method_name, method in methods:
                         immediate = getattr(clazz, method_name)
                         if hasattr(immediate, '__func__'):
                             immediate = immediate.__func__
                         if hasattr(method, '_bantam_web_api') and not hasattr(immediate, '_bantam_web_api'):
                             web_api(content_type=method._bantam_web_api.content_type,
                                     method=method._bantam_web_api.method,
                                     is_constructor=method._bantam_web_api.is_constructor,
                                     expire_obj=method._bantam_web_api.expire_object,
                                     timeout=method._bantam_web_api.timeout,
                                     uuid_param=method._bantam_web_api.uuid_param)(immediate)
                             immediate._bantam_web_api._clazz = clazz
-                            immediate._bantam_web_api._name = method._bantam_web_api.name  # handles case of _expire !-> expire
+                            # handles case of _expire !-> expire
+                            immediate._bantam_web_api._name = method._bantam_web_api.name
                         elif hasattr(method, '_bantam_web_api'):
-                            if method._bantam_web_api.method != immediate._bantam_web_api.method or \
-                                    method._bantam_web_api.content_type != immediate._bantam_web_api.content_type or \
-                                    method._bantam_web_api.is_constructor != immediate._bantam_web_api.is_constructor:
+                            has_diff_web_api = (
+                                method._bantam_web_api.method != immediate._bantam_web_api.method
+                                or method._bantam_web_api.content_type != immediate._bantam_web_api.content_type
+                                or method._bantam_web_api.is_constructor != immediate._bantam_web_api.is_constructor
+                            )
+                            if has_diff_web_api:
                                 raise ValueError(
                                     f"Mismatch in @web_api specifications in {class_name}.{method_name}"
                                     f" and {ancestor.__name__}.{method_name}"
                                 )
+                            elif method._bantam_web_api.arg_annotations != immediate._bantam_web_api.arg_annotations:
+                                raise TypeError(
+                                    f"Mismatch in name and/or type specifications between {class_name}.{method_name}"
+                                    f" and {ancestor.__name__}.{method_name}"
+                                )
 
     # noinspection PyProtectedMember
     async def start(self,
                     modules: List[str],
                     host: Optional[str] = None,
                     port: Optional[int] = None,
                     path: Optional[str] = None,
@@ -370,15 +380,15 @@
             js_path = static_path.joinpath('js')
             if not js_path.exists():
                 js_path.mkdir(parents=True)
             with open(js_path.joinpath(self._js_bundle_name + ".js"), 'bw') as out:
                 if self._using_async:
                     JavascriptGeneratorAsync.generate(
                         out=out, skip_html=False,
-                        allowed_routes =list(self.routes_get.keys()) + list(self.routes_post.keys())
+                        allowed_routes=list(self.routes_get.keys()) + list(self.routes_post.keys())
                     )
                 else:
                     JavascriptGenerator.generate(out=out, skip_html=False)
         self._started = True
         if self._static_path:
             with suppress(Exception):
                 self._generate_rest_docs()
@@ -413,23 +423,23 @@
         # noinspection PyProtectedMember
         def process_class(clazz_: Type):
             if hasattr(clazz_, '_expire') or hasattr(clazz_, '_create'):
                 raise TypeError("Classes with @web_api applied cannot have methods named _expire nor _create")
 
             # noinspection PyDecorator
             @staticmethod
-            async def _create(*args, **kargs) -> clazz_:
-                if kargs.get('__uuid') or (api.uuid_param is not None and api.uuid_param in kargs):
-                    self_id = kargs[api.uuid_param] if api.uuuid_param is not None else kargs['__uuid']
-                    del kargs['__uuid']
+            async def _create(*args, **kwargs) -> clazz_:
+                if kwargs.get('__uuid') or (create_api.uuid_param is not None and create_api.uuid_param in kwargs):
+                    self_id = kwargs[create_api.uuid_param] if create_api.uuuid_param is not None else kwargs['__uuid']
+                    del kwargs['__uuid']
                     if self_id in self.ObjectRepo.instances:
                         raise HTTPException(404, f"UUid {self_id} already in use. uuid's must be unique")
                 else:
                     self_id = str(uuid_pkg.uuid4())
-                instance = clazz_(*args, **kargs)
+                instance = clazz_(*args, **kwargs)
                 if hasattr(clazz_, '__aenter__'):
                     await instance.__aenter__()
                 self.ObjectRepo.instances[self_id] = instance
                 return instance
 
             clazz_._create = _create
             if hasattr(clazz_, '__init__') and hasattr(clazz_.__init__, '__annotations__'):
@@ -446,24 +456,24 @@
                 """
             clazz_._create.__qualname__ = f"{clazz_.__name__}._create"
             clazz_._create.__annotations__['return'] = clazz_
             _create.__func__.__annotations__ = clazz_._create.__annotations__
             _create.__annotations__ = clazz_._create.__annotations__
             # noinspection PyProtectedMember
             route_name = f"/{clazz_.__name__}/_create"
-            api = API(
+            create_api = API(
                 content_type='text/plain',
                 is_instance_method=False,
                 is_class_method=False,
                 is_constructor=True,
                 method=RestMethod.GET,
                 func=_create.__func__,
                 clazz=clazz_
             )
-            self.module_mapping_get.setdefault(clazz_.__module__, {})[route_name] = api
+            self.module_mapping_get.setdefault(clazz_.__module__, {})[route_name] = create_api
             self.routes_get[route_name] = clazz._create
             # self._all_apis[route_name] = api
             self._func_wrapper(clazz, clazz_._create, is_class_method=False, is_instance_method=False,
                                is_constructor=True,
                                expire_on_exit=False, method=RestMethod.GET, content_type="text/plain")
 
             async def _expire(this, new_lease_time: int = self.ObjectRepo.DEFAULT_OBJECT_EXPIRATION,
@@ -485,16 +495,16 @@
             clazz_._expire = _expire
             clazz_._expire.__doc__ = _expire.__doc__
             clazz_._expire.__name__ = 'expire'
             clazz_._expire.__qualname__ = f"{clazz_.__name__}.expire"
 
             # noinspection PyProtectedMember
             self._func_wrapper(clazz, clazz_._expire, is_class_method=False, is_instance_method=True,
-                              expire_on_exit=False,
-                              is_constructor=False, method=RestMethod.GET, content_type="text/plain")
+                               expire_on_exit=False,
+                               is_constructor=False, method=RestMethod.GET, content_type="text/plain")
 
         for clazz in [cl for _, cl in inspect.getmembers(mod) if inspect.isclass(cl)]:
             # noinspection PyProtectedMember
             method_found = any([item for item in inspect.getmembers(clazz) if item[1] == api._func])
             if method_found:
                 api._clazz = clazz
             if method_found and (api in self._instance_methods or api.is_constructor):
@@ -503,18 +513,18 @@
                 self._class_instance_methods.setdefault(clazz, []).append(api)
                 self._instance_methods_class_map[api] = clazz
                 if api.is_constructor:
                     if api._func.__annotations__.get('return') not in (clazz, clazz.__name__):
                         raise TypeError("@web_api's declared as constructors must return that class's type")
 
                 if api.expire_object:
-                    async def wrapped(this, *args, **kargs):
+                    async def wrapped(this, *args, **kwargs):
                         try:
                             # noinspection PyProtectedMember
-                            return await api._func(this, *args, **kargs)
+                            return await api._func(this, *args, **kwargs)
                         finally:
                             if this in self.ObjectRepo.by_instance:
                                 uuid = self.ObjectRepo.by_instance[this]
                                 del self.ObjectRepo.by_instance[this]
                                 del self.ObjectRepo.instances[uuid]
 
                     setattr(clazz, api.name, wrapped)
@@ -802,17 +812,17 @@
                     raise ValueError("No instance provided for call to instance method")
                 instance = cls.ObjectRepo.instances.get(self_id)
                 if instance is None:
                     try:
                         self_id = json.loads(self_id)['uuid']
                         instance = cls.ObjectRepo.instances.get(self_id)
                         if instance is None:
-                            raise Exception()
-                    except:
-                        raise ValueError(f"No instance id found for request {self_id}")
+                            raise ValueError(f"No instance id found for request {self_id}")
+                    except Exception:
+                        raise ValueError(f"Error in json representation of an instance: {self_id}")
                 del kwargs['self']
                 awaitable = api(instance, **kwargs)
                 if api.expire_object:
                     del cls.ObjectRepo.instances[self_id]
             elif api.is_class_method:
 
                 if isinstance(api.clazz, tuple):
```

### Comparing `bantam-2.2.0/src/bantam/js.py` & `bantam-2.2.1/src/bantam/js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/src/bantam/js_async.py` & `bantam-2.2.1/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/src/bantam/pythonclient.py` & `bantam-2.2.1/src/bantam/pythonclient.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/src/bantam.egg-info/PKG-INFO` & `bantam-2.2.1/src/bantam.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.2.0
+Version: 2.2.1
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.2.0
+Download-URL: https://github.com/bantam/dist/2.2.1
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.2.0/src/bantam.egg-info/SOURCES.txt` & `bantam-2.2.1/src/bantam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/test/test_client_get.py` & `bantam-2.2.1/test/test_client_get.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/test/test_client_post.py` & `bantam-2.2.1/test/test_client_post.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/test/test_client_post_inherited_apis.py` & `bantam-2.2.1/test/test_client_post_inherited_apis.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/test/test_conversions.py` & `bantam-2.2.1/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/test/test_decorators.py` & `bantam-2.2.1/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/test/test_js.py` & `bantam-2.2.1/test/test_js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.0/test/test_js_async.py` & `bantam-2.2.1/test/test_js_async.py`

 * *Files identical despite different names*

