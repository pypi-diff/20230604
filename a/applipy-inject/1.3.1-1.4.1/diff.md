# Comparing `tmp/applipy_inject-1.3.1.tar.gz` & `tmp/applipy_inject-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "applipy_inject-1.3.1.tar", last modified: Wed Aug 25 21:32:03 2021, max compression
+gzip compressed data, was "applipy_inject-1.4.1.tar", last modified: Sun Jun  4 08:36:01 2023, max compression
```

## Comparing `applipy_inject-1.3.1.tar` & `applipy_inject-1.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-25 21:32:03.750862 applipy_inject-1.3.1/
--rw-rw-rw-   0 root         (0) root         (0)      556 2021-08-25 21:31:54.000000 applipy_inject-1.3.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       34 2021-08-25 21:31:54.000000 applipy_inject-1.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7282 2021-08-25 21:32:03.750862 applipy_inject-1.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6577 2021-08-25 21:31:54.000000 applipy_inject-1.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-25 21:32:03.748862 applipy_inject-1.3.1/applipy_inject/
--rw-rw-rw-   0 root         (0) root         (0)      198 2021-08-25 21:31:54.000000 applipy_inject-1.3.1/applipy_inject/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14063 2021-08-25 21:31:54.000000 applipy_inject-1.3.1/applipy_inject/inject.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-25 21:31:54.000000 applipy_inject-1.3.1/applipy_inject/py.typed
--rw-rw-rw-   0 root         (0) root         (0)       22 2021-08-25 21:31:54.000000 applipy_inject-1.3.1/applipy_inject/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-25 21:32:03.750862 applipy_inject-1.3.1/applipy_inject.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7282 2021-08-25 21:32:03.000000 applipy_inject-1.3.1/applipy_inject.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      292 2021-08-25 21:32:03.000000 applipy_inject-1.3.1/applipy_inject.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-25 21:32:03.000000 applipy_inject-1.3.1/applipy_inject.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2021-08-25 21:32:03.000000 applipy_inject-1.3.1/applipy_inject.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-08-25 21:32:03.750862 applipy_inject-1.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1375 2021-08-25 21:31:54.000000 applipy_inject-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 08:36:01.094164 applipy_inject-1.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)      556 2023-06-04 08:35:53.000000 applipy_inject-1.4.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-04 08:35:53.000000 applipy_inject-1.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7263 2023-06-04 08:36:01.094164 applipy_inject-1.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6577 2023-06-04 08:35:53.000000 applipy_inject-1.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 08:36:01.093165 applipy_inject-1.4.1/applipy_inject/
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-04 08:35:53.000000 applipy_inject-1.4.1/applipy_inject/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14796 2023-06-04 08:35:53.000000 applipy_inject-1.4.1/applipy_inject/inject.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 08:35:53.000000 applipy_inject-1.4.1/applipy_inject/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-04 08:35:53.000000 applipy_inject-1.4.1/applipy_inject/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 08:36:01.094164 applipy_inject-1.4.1/applipy_inject.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7263 2023-06-04 08:36:01.000000 applipy_inject-1.4.1/applipy_inject.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-04 08:36:01.000000 applipy_inject-1.4.1/applipy_inject.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 08:36:01.000000 applipy_inject-1.4.1/applipy_inject.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-04 08:36:01.000000 applipy_inject-1.4.1/applipy_inject.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 08:36:01.094164 applipy_inject-1.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2023-06-04 08:35:53.000000 applipy_inject-1.4.1/setup.py
```

### Comparing `applipy_inject-1.3.1/LICENSE` & `applipy_inject-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `applipy_inject-1.3.1/PKG-INFO` & `applipy_inject-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: applipy_inject
-Version: 1.3.1
+Version: 1.4.1
 Summary: Library that provides a dependency injector that works with type hinting.
 Home-page: https://gitlab.com/applipy/applipy_inject
 Author: Alessio Linares
 Author-email: mail@alessio.cc
 License: Apache 2.0
 Project-URL: Source, https://gitlab.com/applipy/applipy_inject
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![pipeline status](https://gitlab.com/applipy/applipy_inject/badges/master/pipeline.svg)](https://gitlab.com/applipy/applipy_inject/-/pipelines?scope=branches&ref=master)
 [![coverage report](https://gitlab.com/applipy/applipy_inject/badges/master/coverage.svg)](https://gitlab.com/applipy/applipy_inject/-/graphs/master/charts)
 [![PyPI Status](https://img.shields.io/pypi/status/applipy-inject.svg)](https://pypi.org/project/applipy-inject/)
 [![PyPI Version](https://img.shields.io/pypi/v/applipy-inject.svg)](https://pypi.org/project/applipy-inject/)
@@ -276,9 +275,7 @@
     def __init__(self, a: Annotated[dict, name('conf')], b: str):
         ...
 
 
 def provide_int(x: Annotated[int, name('foo')], b: Annotated[str, name('foo')]) -> int:
     ...
 ```
-
-
```

### Comparing `applipy_inject-1.3.1/README.md` & `applipy_inject-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `applipy_inject-1.3.1/applipy_inject/inject.py` & `applipy_inject-1.4.1/applipy_inject/inject.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,24 @@
     Union,
     cast,
     overload,
     get_args,
     get_origin,
     get_type_hints
 )
+from types import UnionType, GenericAlias
 from collections import defaultdict
 from enum import Enum
 
 
 T = TypeVar('T')
 T_Co = TypeVar('T_Co', covariant=True)
 
 
-def _get_class_name(c: type) -> str:
+def _get_class_name(c: Any) -> str:
     module: Optional[str] = getattr(c, '__module__', None)
     name: Optional[str] = getattr(c, '__qualname__', None)
     if not name:
         name = getattr(c, '__name__', None)
         if not name:
             name = str(c)
 
@@ -37,16 +38,39 @@
     if args:
         name += '[' + ', '.join(_get_class_name(a) for a in args) + ']'
     if module and module != 'builtins':
         return module + '.' + name
     return name
 
 
-class name(str):
-    ...
+def _is_type(t: Any) -> bool:
+    return isinstance(t, type) or isinstance(t, GenericAlias)
+
+
+class name:
+    value: str
+
+    def __init__(self, value: str) -> None:
+        self.value = value
+
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, str):
+            return self.value == other
+        if isinstance(other, name):
+            return self.value == other.value
+        return False
+
+    def __hash__(self) -> int:
+        return hash(self.value)
+
+    def __repr__(self) -> str:
+        return self.value
+
+    def __str__(self) -> str:
+        return self.value
 
 
 _Name = name
 
 
 def with_names(provider: Callable[..., T], name: Union[dict[str, str], str]) -> Callable[..., T]:
 
@@ -56,15 +80,15 @@
     names: dict[str, Optional[str]]
     if isinstance(name, dict):
         names = defaultdict(lambda: None)
         names.update(name)
     else:
         names = defaultdict(lambda: cast(Optional[str], name))
 
-    if isinstance(provider, type):
+    if _is_type(provider):
         init = getattr(provider, '__init__')
         if init:
             annotations = get_type_hints(init, include_extras=True).copy()
             annotations['return'] = provider
         else:
             annotations = get_type_hints(provider, include_extras=True)
     else:
@@ -82,15 +106,15 @@
 def named(names: Union[dict[str, str], str]) -> Callable[[Callable[..., T]], Callable[..., T]]:
     def construct_wrapper(func: Callable[..., T]) -> Callable[..., T]:
         return with_names(func, names)
 
     return construct_wrapper
 
 
-class DependencyType(str, Enum):
+class DependencyType(Enum):
     Required = 'required'
     Optional = 'optional'
     Collection = 'collection'
 
 
 class Dependency:
 
@@ -154,15 +178,15 @@
 
     def _dependency_is_collection(self, dep_type: type) -> bool:
         origin = get_origin(dep_type)
         return origin is not None and (origin is list or origin is List)
 
     def _dependency_is_optional(self, dep_type: type) -> bool:
         origin = get_origin(dep_type)
-        if origin is not Union:
+        if not (origin is Union or origin is UnionType):
             return False
         args = get_args(dep_type)
         if len(args) != 2:
             return False
         return type(None) in args
 
     def _get_dependency_type(self, type_: type) -> DependencyType:
@@ -184,15 +208,15 @@
     def _is_provider(self,
                      provider_or_instance: Union[T, Callable[..., T]],
                      type_: Union[Type[T], Callable[..., T], Tuple[Type[T], ...], List[Type[T]]]) -> bool:
         return (
             (
                 isinstance(type_, (tuple, list))
                 and
-                all(isinstance(t, type) for t in type_)
+                all(_is_type(t) for t in type_)
                 and
                 all(self._is_provider(provider_or_instance, t) for t in type_)
             )
             or
             (
                 isinstance(type_, type)
                 and
@@ -211,61 +235,61 @@
                     type_
                 )
             )
         )
 
     @overload
     def bind(self, type_: Type[T],
-             provider_or_instance: None = None, name: Optional[str] = None, singleton: bool = False) -> None:
+             provider_or_instance: None = None, /, *, name: Optional[str] = None, singleton: bool = False) -> None:
         ...
 
     @overload
     def bind(self, type_: Callable[..., T],
-             provider_or_instance: None = None, name: Optional[str] = None, singleton: bool = False) -> None:
+             provider_or_instance: None = None, /, *, name: Optional[str] = None, singleton: bool = False) -> None:
         ...
 
     @overload
-    def bind(self, type_: Type[T], provider_or_instance: Callable[..., T],
+    def bind(self, type_: Type[T], provider_or_instance: Callable[..., T], /, *,
              name: Optional[str] = None, singleton: bool = False) -> None:
         ...
 
     @overload
-    def bind(self, type_: Tuple[type, ...], provider_or_instance: Callable[..., object],
+    def bind(self, type_: Tuple[type, ...], provider_or_instance: Callable[..., object], /, *,
              name: Optional[str] = None, singleton: bool = False) -> None:
         ...
 
     @overload
-    def bind(self, type_: List[type], provider_or_instance: Callable[..., object],
+    def bind(self, type_: List[type], provider_or_instance: Callable[..., object], /, *,
              name: Optional[str] = None, singleton: bool = False) -> None:
         ...
 
     @overload
-    def bind(self, type_: Type[T], provider_or_instance: T,
+    def bind(self, type_: Type[T], provider_or_instance: T, /, *,
              name: Optional[str] = None, singleton: bool = False) -> None:
         ...
 
     @overload
-    def bind(self, type_: Tuple[type, ...], provider_or_instance: object,
+    def bind(self, type_: Tuple[type, ...], provider_or_instance: object, /, *,
              name: Optional[str] = None, singleton: bool = False) -> None:
         ...
 
     @overload
-    def bind(self, type_: List[type], provider_or_instance: object,
+    def bind(self, type_: List[type], provider_or_instance: object, /, *,
              name: Optional[str] = None, singleton: bool = False) -> None:
         ...
 
     def bind(self,
              type_: Union[Type[T], Tuple[type, ...], List[type], Callable[..., T]],
-             provider_or_instance: Optional[Union[T, Callable[..., object], object]] = None,
+             provider_or_instance: Optional[Union[T, Callable[..., object], object]] = None, /, *,
              name: Optional[str] = None,
              singleton: bool = True) -> None:
         if provider_or_instance is None:
-            if isinstance(type_, type):
-                self.bind_type(type_, name=name, singleton=singleton)
-            elif callable(type_) and isinstance(get_type_hints(type_).get('return'), type):
+            if _is_type(type_):
+                self.bind_type(cast(type, type_), name=name, singleton=singleton)
+            elif callable(type_) and _is_type(get_type_hints(type_).get('return')):
                 self.bind_provider(get_type_hints(type_)['return'], type_, name=name, singleton=singleton)
             else:
                 raise TypeError('Cannot bind {}. Please be more explicit'.format(type_))
         elif self._is_provider(provider_or_instance, type_):
             self.bind_provider(cast(Union[Type[T], Tuple[type, ...], List[type]], type_),
                                cast(Callable[..., T], provider_or_instance),
                                name=name,
@@ -274,18 +298,19 @@
             self.bind_instance(cast(Union[Type[T], Tuple[Type[T], ...], List[Type[T]]], type_),
                                cast(T, provider_or_instance),
                                name=name)
 
     def bind_provider(self,
                       types: Union[Type[T], Tuple[type, ...], List[type]],
                       provider: Callable[..., T],
+                      /, *,
                       name: Optional[str] = None,
                       singleton: bool = True) -> None:
         func: Callable[..., T]
-        if isinstance(provider, type):
+        if _is_type(provider):
             func = cast(Callable[..., T], getattr(provider, '__init__'))
         else:
             func = provider
 
         if not isinstance(types, (tuple, list)):
             types = (types,)
 
@@ -296,15 +321,15 @@
         dependencies = []
         for var, typ in annotations.items():
             dep_name = None
             if get_origin(typ) == Annotated:
                 args = get_args(typ)
                 typ = args[0]
                 try:
-                    dep_name = next(x for x in reversed(args[1:]) if isinstance(x, _Name))
+                    dep_name = next(x.value for x in reversed(args[1:]) if isinstance(x, _Name))
                 except StopIteration:
                     ...
 
             dependencies.append(Dependency(dep_name,
                                            self._get_dependency_class(typ),
                                            var,
                                            self._get_dependency_type(typ)))
@@ -312,21 +337,23 @@
         item = Item[T](name, Provider(provider, dependencies), singleton)
 
         for type_ in types:
             self.providers[name, type_].add(item)
 
     def bind_type(self,
                   type_: type,
+                  /, *,
                   name: Optional[str] = None,
                   singleton: bool = True) -> None:
         self.bind_provider(type_, type_, name=name, singleton=singleton)
 
     def bind_instance(self,
                       types: Union[Type[T], Tuple[Type[T], ...], List[Type[T]]],
                       instance: T,
+                      /, *,
                       name: Optional[str] = None) -> None:
         item = Item[T](name, Provider(lambda: instance, ()), True, instance=instance)
 
         if not isinstance(types, (tuple, list)):
             types = (types,)
         for type_ in types:
             self.providers[name, type_].add(item)
@@ -355,17 +382,18 @@
                 dependencies: dict[str, Union[List[object], Optional[object], object]] = {}
                 for dependency in item.provider.dependencies:
                     if dependency.dep_type == DependencyType.Collection:
                         dependencies[dependency.varname] = self.get_all(dependency.type_,
                                                                         name=dependency.name,
                                                                         _requested=requested)
                     elif dependency.dep_type == DependencyType.Optional:
-                        dependencies[dependency.varname] = self.get_optional(dependency.type_,
-                                                                             name=dependency.name,
-                                                                             _requested=requested)
+                        dep: Any = self.get_optional(dependency.type_,
+                                                     name=dependency.name,
+                                                     _requested=requested)
+                        dependencies[dependency.varname] = dep
                     else:
                         dependencies[dependency.varname] = self.get(dependency.type_,
                                                                     name=dependency.name,
                                                                     _requested=requested)
                 try:
                     instance = item.instantiate(**dependencies)
                 except TypeError:
```

### Comparing `applipy_inject-1.3.1/applipy_inject.egg-info/PKG-INFO` & `applipy_inject-1.4.1/applipy_inject.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: applipy-inject
-Version: 1.3.1
+Version: 1.4.1
 Summary: Library that provides a dependency injector that works with type hinting.
 Home-page: https://gitlab.com/applipy/applipy_inject
 Author: Alessio Linares
 Author-email: mail@alessio.cc
 License: Apache 2.0
 Project-URL: Source, https://gitlab.com/applipy/applipy_inject
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![pipeline status](https://gitlab.com/applipy/applipy_inject/badges/master/pipeline.svg)](https://gitlab.com/applipy/applipy_inject/-/pipelines?scope=branches&ref=master)
 [![coverage report](https://gitlab.com/applipy/applipy_inject/badges/master/coverage.svg)](https://gitlab.com/applipy/applipy_inject/-/graphs/master/charts)
 [![PyPI Status](https://img.shields.io/pypi/status/applipy-inject.svg)](https://pypi.org/project/applipy-inject/)
 [![PyPI Version](https://img.shields.io/pypi/v/applipy-inject.svg)](https://pypi.org/project/applipy-inject/)
@@ -276,9 +275,7 @@
     def __init__(self, a: Annotated[dict, name('conf')], b: str):
         ...
 
 
 def provide_int(x: Annotated[int, name('foo')], b: Annotated[str, name('foo')]) -> int:
     ...
 ```
-
-
```

### Comparing `applipy_inject-1.3.1/setup.py` & `applipy_inject-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,12 +30,12 @@
     long_description_content_type='text/markdown',
     license='Apache 2.0',
     author='Alessio Linares',
     author_email='mail@alessio.cc',
     version=version,
     packages=find_packages(exclude=['doc', 'tests']),
     data_files=[],
-    python_requires='>=3.9',
+    python_requires='>=3.10',
     install_requires=[],
     scripts=[],
     package_data={'applipy_inject': ['py.typed']},
 )
```

