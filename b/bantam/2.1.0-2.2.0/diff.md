# Comparing `tmp/bantam-2.1.0.tar.gz` & `tmp/bantam-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.1.0.tar", last modified: Sun Jun  4 04:51:05 2023, max compression
+gzip compressed data, was "bantam-2.2.0.tar", last modified: Sun Jun  4 14:54:06 2023, max compression
```

## Comparing `bantam-2.1.0.tar` & `bantam-2.2.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 04:51:05.775427 bantam-2.1.0/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-04 04:51:05.775427 bantam-2.1.0/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.1.0/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-03 15:15:17.000000 bantam-2.1.0/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-04 04:51:05.775427 bantam-2.1.0/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-04 04:15:36.000000 bantam-2.1.0/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 04:51:05.771427 bantam-2.1.0/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 04:51:05.775427 bantam-2.1.0/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4011 2023-06-04 04:49:42.000000 bantam-2.1.0/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    10329 2023-06-04 03:58:24.000000 bantam-2.1.0/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 04:51:05.775427 bantam-2.1.0/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.1.0/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.1.0/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    18033 2023-06-04 04:42:49.000000 bantam-2.1.0/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.1.0/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4594 2023-06-03 20:59:30.000000 bantam-2.1.0/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    41752 2023-06-04 03:57:52.000000 bantam-2.1.0/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    21983 2023-06-04 03:28:23.000000 bantam-2.1.0/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.1.0/src/bantam/js_async.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.1.0/src/bantam/pythonclient.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 04:51:05.775427 bantam-2.1.0/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-04 04:51:05.000000 bantam-2.1.0/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      641 2023-06-04 04:51:05.000000 bantam-2.1.0/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-04 04:51:05.000000 bantam-2.1.0/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-04 04:51:05.000000 bantam-2.1.0/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-04 04:51:05.000000 bantam-2.1.0/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-04 04:51:05.000000 bantam-2.1.0/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 04:51:05.775427 bantam-2.1.0/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4472 2023-06-04 02:18:21.000000 bantam-2.1.0/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4517 2023-06-04 02:21:15.000000 bantam-2.1.0/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.1.0/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.1.0/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     7531 2023-06-03 15:33:20.000000 bantam-2.1.0/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2845 2023-06-04 03:14:39.000000 bantam-2.1.0/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 14:54:06.511878 bantam-2.2.0/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-04 14:54:06.511878 bantam-2.2.0/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.2.0/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-03 15:15:17.000000 bantam-2.2.0/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-04 14:54:06.511878 bantam-2.2.0/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-04 14:50:20.000000 bantam-2.2.0/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 14:54:06.511878 bantam-2.2.0/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 14:54:06.511878 bantam-2.2.0/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4011 2023-06-04 04:49:42.000000 bantam-2.2.0/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    10329 2023-06-04 03:58:24.000000 bantam-2.2.0/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 14:54:06.511878 bantam-2.2.0/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.2.0/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.2.0/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    17999 2023-06-04 14:52:43.000000 bantam-2.2.0/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.2.0/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4399 2023-06-04 13:45:48.000000 bantam-2.2.0/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    43836 2023-06-04 14:40:10.000000 bantam-2.2.0/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.2.0/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.2.0/src/bantam/js_async.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.2.0/src/bantam/pythonclient.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 14:54:06.511878 bantam-2.2.0/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-04 14:54:06.000000 bantam-2.2.0/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-04 14:54:06.000000 bantam-2.2.0/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-04 14:54:06.000000 bantam-2.2.0/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-04 14:54:06.000000 bantam-2.2.0/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-04 14:54:06.000000 bantam-2.2.0/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-04 14:54:06.000000 bantam-2.2.0/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-04 14:54:06.511878 bantam-2.2.0/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4472 2023-06-04 02:18:21.000000 bantam-2.2.0/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4517 2023-06-04 02:21:15.000000 bantam-2.2.0/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4573 2023-06-04 14:26:39.000000 bantam-2.2.0/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.2.0/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.2.0/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.2.0/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     7531 2023-06-03 15:33:20.000000 bantam-2.2.0/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2845 2023-06-04 03:14:39.000000 bantam-2.2.0/test/test_js_async.py
```

### Comparing `bantam-2.1.0/PKG-INFO` & `bantam-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.1.0
+Version: 2.2.0
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.1.0
+Download-URL: https://github.com/bantam/dist/2.2.0
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.1.0/setup.py` & `bantam-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.1.0"
+VERSION = "2.2.0"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.1.0/src/bantam/__init__.py` & `bantam-2.2.0/src/bantam/__init__.py`

 * *Files identical despite different names*

### Comparing `bantam-2.1.0/src/bantam/api.py` & `bantam-2.2.0/src/bantam/api.py`

 * *Files identical despite different names*

### Comparing `bantam-2.1.0/src/bantam/autogen/main.py` & `bantam-2.2.0/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.1.0/src/bantam/client.py` & `bantam-2.2.0/src/bantam/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,45 +35,44 @@
 ...          HAVE SAME @web_api DECORATION AS SERVER IMPL DECLARATION
 ...          '''
 ...          # never called since abstract, but needed to tell Python that implementation
 ...          # will be an async generator/iterator:
 ...          yield None
 ...
 
-One then defines the concrete class (which for best practice, has same name, sans 'Interface'):
+One then defines the concrete class (which for best practice, has same name, sans 'Interface').  The
+@web_api decorators need not be specified as bantam will ensure they are inherited. (But if you do
+specify them explicitly, you must ensure they are maintained to be the same):
 
 >>>  from bantam.client import WebInterface
 ...  from bantam.api import RestMethod
 ...  from bantam.decorators web_api
 ...  from typing import AsyncIterator
 ...
 ...  class MyServerApi(MyServerApiInterface):
 ...
 ...     def __init__(self):
 ...         self._message_bits = ['I', 'am', 'the', 'very', 'model']
 ...
 ...     @classmethod
-...     @web_api(methos=RestMethod.GET, content_type='application/json')
 ...     async def constructor(cls) -> "MyServerApiInterface":
 ...        '''
 ...        Concreate constructor to create an instance of the class WITH SAEM @web_api DECORATOR AND
 ...        SIGNATURE
 ...        '''
 ...        return MyServerApi()
 ...
 ...      @classmethod
-...      @web_api(method=RestMethod.GET, content_type='text/plain')
 ...      async def class_method_api(cls, parm1: str) -> Dict[str, int]:
 ...          '''
 ...          Concreate class method to be implemented WITH SAME @web_api DECORATION AND,
 ...          OF COURSE, SIGNATURE
 ...          '''
 ...          return {'param1': int(parm1)}
 ...
-...      @web_api(method=RestMethod.POST, content_type='application/json')
 ...      async def instance_method_api(self) -> AsyncIterator[str]:
 ...          '''
 ...          Concrete instance method that is an Async Iterator over string values.
 ...          MUST HAVE SAME @web_api DECORATION AND SIGNATURE
 ...          '''
 ...          # never called since abstract, but needed to tell Python that implementation
 ...          # will be an async generator/iterator:
```

### Comparing `bantam-2.1.0/src/bantam/conversions.py` & `bantam-2.2.0/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.1.0/src/bantam/decorators.py` & `bantam-2.2.0/src/bantam/decorators.py`

 * *Files 13% similar despite different names*

```diff
@@ -64,17 +64,14 @@
             raise TypeError("@web_api's that are declared constructors must be static or class methods")
         if (is_static or is_class_method) and expire_obj:
             raise TypeError("@web_api's expire_obj param can only be set True for instance methods")
         if not is_static and not is_class_method and not inspect.ismethod(func) and not inspect.isfunction(func):
             raise TypeError("@web_api should only be applied to @classmethod's, @staticmethods or instance methods")
         if func.__name__.startswith('_'):
             raise TypeError("names of web_api methods must not start with underscore")
-        # noinspection PyProtectedMember
-        # clazz = WebApplication._instance_methods_class_map[obj] if not isinstance(obj, staticmethod) else None
-        func._bantam_web_method = method
 
         def get_class_that_defined_method():
             return func.__qualname__.split('.')[0]
 
         return WebApplication._func_wrapper((func.__module__, get_class_that_defined_method())
                                                 if is_class_method else None,
                                             func,
```

### Comparing `bantam-2.1.0/src/bantam/http.py` & `bantam-2.2.0/src/bantam/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -260,14 +260,51 @@
             existing = cls.callables_get.get(route) or WebApplication.callables_post.get(route)
             raise cls.DuplicateRoute(f"Route '{route}' associated with {api.module}.{api._func.__name__}"
                                      f" already exists here {existing.module}.{existing.name} ")
         cls.routes_post[route] = async_method
         cls.callables_post[route] = api
         cls.module_mapping_post.setdefault(module, {})[route] = api
 
+    @classmethod
+    def preprocess_module(cls, module_: str):
+        if module_ not in sys.modules:
+            mod = importlib.import_module(module_)
+        else:
+            mod = sys.modules.get(module_)
+        for class_name, clazz in inspect.getmembers(mod, predicate=inspect.isclass):
+            from .client import WebInterface
+            if issubclass(clazz, WebInterface):
+                ancestors = clazz.__mro__
+                for ancestor in ancestors:
+                    if ancestor == clazz:
+                        continue
+                    methods = inspect.getmembers(ancestor, predicate=inspect.ismethod) + \
+                              inspect.getmembers(ancestor, predicate=inspect.isfunction)
+                    for method_name, method in methods:
+                        immediate = getattr(clazz, method_name)
+                        if hasattr(immediate, '__func__'):
+                            immediate = immediate.__func__
+                        if hasattr(method, '_bantam_web_api') and not hasattr(immediate, '_bantam_web_api'):
+                            web_api(content_type=method._bantam_web_api.content_type,
+                                    method=method._bantam_web_api.method,
+                                    is_constructor=method._bantam_web_api.is_constructor,
+                                    expire_obj=method._bantam_web_api.expire_object,
+                                    timeout=method._bantam_web_api.timeout,
+                                    uuid_param=method._bantam_web_api.uuid_param)(immediate)
+                            immediate._bantam_web_api._clazz = clazz
+                            immediate._bantam_web_api._name = method._bantam_web_api.name  # handles case of _expire !-> expire
+                        elif hasattr(method, '_bantam_web_api'):
+                            if method._bantam_web_api.method != immediate._bantam_web_api.method or \
+                                    method._bantam_web_api.content_type != immediate._bantam_web_api.content_type or \
+                                    method._bantam_web_api.is_constructor != immediate._bantam_web_api.is_constructor:
+                                raise ValueError(
+                                    f"Mismatch in @web_api specifications in {class_name}.{method_name}"
+                                    f" and {ancestor.__name__}.{method_name}"
+                                )
+
     # noinspection PyProtectedMember
     async def start(self,
                     modules: List[str],
                     host: Optional[str] = None,
                     port: Optional[int] = None,
                     path: Optional[str] = None,
                     shutdown_timeout: float = 60.0,
@@ -293,31 +330,26 @@
         :param reuse_port: tells the kernel to allow this endpoint to be bound to the same port as other existing
             endpoints are bound to, so long as they all set this flag when being created. This option is not supported
             on Windows.
         """
         # noinspection PyProtectedMember
         from aiohttp.web import _run_app as web_run_app
         for module in modules:
-            if not module in sys.modules:
+            self.preprocess_module(module)
+            if module not in sys.modules:
                 mod = importlib.import_module(module)
             else:
                 mod = sys.modules.get(module)
             for api in list(self.module_mapping_get.get(module, {}).values()):
                 if api.name in ['_expire']:
                     continue
-                #if api.is_class_method:
-                    #class_name, method_name = api._real_func.__qualname__.split('.')
-                    #api._func = getattr(getattr(mod, class_name), method_name)
                 self._process_module_classes(mod, api)
             for api in self.module_mapping_post.get(module, {}).values():
                 if api.name in ['_expire']:
                     continue
-                #if api.is_class_method:
-                    #class_name, method_name = api._real_func.__qualname__.split('.')
-                    #api._func = getattr(getattr(mod, class_name), method_name)
                 self._process_module_classes(mod, api)
         allowed_get_routes = {}
         for module in [m for m in modules if m in self.module_mapping_get]:
             allowed_get_routes.update(self.module_mapping_get[module])
         for route, api_get in allowed_get_routes.items():
             log.debug(f">>>>>>>>>> GET ROUTE {route}")
             invoke = self.routes_get[route]
@@ -423,15 +455,15 @@
                 is_instance_method=False,
                 is_class_method=False,
                 is_constructor=True,
                 method=RestMethod.GET,
                 func=_create.__func__,
                 clazz=clazz_
             )
-            self.module_mapping_get.setdefault(clazz_.__module__)[route_name] = api
+            self.module_mapping_get.setdefault(clazz_.__module__, {})[route_name] = api
             self.routes_get[route_name] = clazz._create
             # self._all_apis[route_name] = api
             self._func_wrapper(clazz, clazz_._create, is_class_method=False, is_instance_method=False,
                                is_constructor=True,
                                expire_on_exit=False, method=RestMethod.GET, content_type="text/plain")
 
             async def _expire(this, new_lease_time: int = self.ObjectRepo.DEFAULT_OBJECT_EXPIRATION,
@@ -817,15 +849,15 @@
                 #  regular response
                 #################
                 if api.is_constructor:
                     instance = await awaitable
                     if api.clazz and hasattr(api.clazz, '__aenter__'):
                         await instance.__aenter__()
                     if hasattr(api.clazz, 'jsonrepr'):
-                        repr_ = api.clazz.jsonrepr(result)
+                        repr_ = api.clazz.jsonrepr(instance)
                         uuid = repr_.get(api.uuid_param)
                         content_type = 'application/json'
                         result = json.dumps(repr_)
                     else:
                         uuid = kwargs.get(api.uuid_param, str(uuid_pkg.uuid4()))
                         result = json.dumps({'uuid': uuid})
                     cls.ObjectRepo.instances[uuid] = instance
```

### Comparing `bantam-2.1.0/src/bantam/js.py` & `bantam-2.2.0/src/bantam/js.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,20 +149,21 @@
 
                 if class_name in clazz_map:
                     clazz = clazz_map[class_name]
                     if inspect.isabstract(clazz):
                         continue
                     cls._generate_request(out, route=f"/{class_name}/_create",
                                           api=API(clazz, clazz._create, method=RestMethod.GET,
-                                                  content_type="test/plain",
+                                                  content_type="test/plain", is_class_method=True,
                                                   is_instance_method=False, is_constructor=True, expire_on_exit=False),
                                           tab=tab)
                     cls._generate_request(out, route=f"/{class_name}/expire",
                                           api=API(clazz, clazz._expire, method=RestMethod.GET,
                                                   content_type="text/plain",
+                                                  is_class_method=True,
                                                   is_instance_method=True, is_constructor=False, expire_on_exit=False),
                                           tab=tab)
                 for method, route_, api in routes:
                     cls._generate_request(out, route_, api, tab)
                 tab = tab[:-3]
                 out.write("};\n".encode(cls.ENCODING))  # for class end
 
@@ -258,15 +259,16 @@
         docs = '\n'.join(lines) + '\n'
         out.write(docs.encode(cls.ENCODING))
 
     @classmethod
     def _generate_request(cls, out: IO, route: str, api: API, tab: str):
         func = api._func
         arg_count = func.__code__.co_argcount
-        if 'self' in func.__code__.co_varnames or 'cls' in func.__code__.co_varnames:
+        if 'self' in func.__code__.co_varnames or 'cls' in func.__code__.co_varnames\
+                or 'this' in func.__code__.co_varnames:
             arg_count -= 1
 
         if not api.name.startswith('_') and arg_count != len(api.arg_annotations):
             raise Exception(f"Not all arguments of '{api.qualname}' have type hints.  This is required for web_api")
         if api.has_streamed_response is True:
             callback = 'onreceive'
             state = 3
```

### Comparing `bantam-2.1.0/src/bantam/js_async.py` & `bantam-2.2.0/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.1.0/src/bantam/pythonclient.py` & `bantam-2.2.0/src/bantam/pythonclient.py`

 * *Files identical despite different names*

### Comparing `bantam-2.1.0/src/bantam.egg-info/PKG-INFO` & `bantam-2.2.0/src/bantam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.1.0
+Version: 2.2.0
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.1.0
+Download-URL: https://github.com/bantam/dist/2.2.0
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.1.0/src/bantam.egg-info/SOURCES.txt` & `bantam-2.2.0/src/bantam.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,11 +17,13 @@
 src/bantam.egg-info/entry_points.txt
 src/bantam.egg-info/requires.txt
 src/bantam.egg-info/top_level.txt
 src/bantam/autogen/__init__.py
 src/bantam/autogen/main.py
 test/test_client_get.py
 test/test_client_post.py
+test/test_client_post_inherited_apis.py
 test/test_conversions.py
 test/test_decorators.py
+test/test_http.py
 test/test_js.py
 test/test_js_async.py
```

### Comparing `bantam-2.1.0/test/test_client_get.py` & `bantam-2.2.0/test/test_client_get.py`

 * *Files identical despite different names*

### Comparing `bantam-2.1.0/test/test_client_post.py` & `bantam-2.2.0/test/test_client_post.py`

 * *Files identical despite different names*

### Comparing `bantam-2.1.0/test/test_conversions.py` & `bantam-2.2.0/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.1.0/test/test_decorators.py` & `bantam-2.2.0/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.1.0/test/test_js.py` & `bantam-2.2.0/test/test_js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.1.0/test/test_js_async.py` & `bantam-2.2.0/test/test_js_async.py`

 * *Files identical despite different names*

