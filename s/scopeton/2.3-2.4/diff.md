# Comparing `tmp/scopeton-2.3.tar.gz` & `tmp/scopeton-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scopeton-2.3.tar", last modified: Sun Jan 17 14:44:39 2021, max compression
+gzip compressed data, was "scopeton-2.4.tar", last modified: Sun Jun  4 19:11:10 2023, max compression
```

## Comparing `scopeton-2.3.tar` & `scopeton-2.4.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2021-01-17 14:44:39.360335 scopeton-2.3/
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      344 2021-01-17 14:44:39.360335 scopeton-2.3/PKG-INFO
-drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2021-01-17 14:44:39.360335 scopeton-2.3/scopeton/
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       38 2020-12-10 19:44:35.182924 scopeton-2.3/scopeton/__init__.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1068 2020-12-10 19:44:35.182924 scopeton-2.3/scopeton/compat.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       33 2020-12-10 19:44:35.182924 scopeton-2.3/scopeton/constants.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1043 2020-12-10 19:44:35.182924 scopeton-2.3/scopeton/decorators.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       16 2020-12-10 19:44:35.182924 scopeton-2.3/scopeton/glob.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1110 2020-12-10 19:44:35.182924 scopeton-2.3/scopeton/objects.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     3105 2020-12-10 20:16:27.016864 scopeton-2.3/scopeton/qualifier_tree.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     4094 2021-01-17 14:42:22.682997 scopeton-2.3/scopeton/scope.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1320 2021-01-17 14:42:36.291130 scopeton-2.3/scopeton/scopeTools.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       39 2020-12-10 19:44:35.182924 scopeton-2.3/setup.cfg
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      500 2021-01-17 14:43:39.519749 scopeton-2.3/setup.py
+drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-06-04 19:11:10.741039 scopeton-2.4/
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1086 2023-04-16 07:04:25.000000 scopeton-2.4/LICENSE.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      314 2023-06-04 19:11:10.741039 scopeton-2.4/PKG-INFO
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     2472 2023-04-16 07:49:04.000000 scopeton-2.4/README.md
+drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-06-04 19:11:10.741039 scopeton-2.4/scopeton/
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       38 2023-04-16 07:04:25.000000 scopeton-2.4/scopeton/__init__.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1068 2023-04-16 07:04:25.000000 scopeton-2.4/scopeton/compat.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       67 2023-06-04 18:13:09.000000 scopeton-2.4/scopeton/constants.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1113 2023-06-04 18:58:02.000000 scopeton-2.4/scopeton/decorators.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       46 2023-06-04 18:11:40.000000 scopeton-2.4/scopeton/glob.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1110 2023-04-16 07:04:25.000000 scopeton-2.4/scopeton/objects.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     3105 2023-04-16 07:04:25.000000 scopeton-2.4/scopeton/qualifier_tree.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     5008 2023-06-04 19:09:04.000000 scopeton-2.4/scopeton/scope.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1320 2023-04-16 07:04:25.000000 scopeton-2.4/scopeton/scopeTools.py
+drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-06-04 19:11:10.741039 scopeton-2.4/scopeton.egg-info/
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      314 2023-06-04 19:11:10.000000 scopeton-2.4/scopeton.egg-info/PKG-INFO
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      389 2023-06-04 19:11:10.000000 scopeton-2.4/scopeton.egg-info/SOURCES.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        1 2023-06-04 19:11:10.000000 scopeton-2.4/scopeton.egg-info/dependency_links.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        7 2023-06-04 19:11:10.000000 scopeton-2.4/scopeton.egg-info/requires.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        9 2023-06-04 19:11:10.000000 scopeton-2.4/scopeton.egg-info/top_level.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       79 2023-06-04 19:11:10.741039 scopeton-2.4/setup.cfg
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      500 2023-06-04 19:10:25.000000 scopeton-2.4/setup.py
```

### Comparing `scopeton-2.3/scopeton/compat.py` & `scopeton-2.4/scopeton/compat.py`

 * *Files identical despite different names*

### Comparing `scopeton-2.3/scopeton/decorators.py` & `scopeton-2.4/scopeton/decorators.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 from scopeton.scopeTools import ScopetonException
 
 
 def Inject():
     def inject_decorator(fn):
         annotations_signature = compat.getMethodSignature(fn).annotations
         args_signature = compat.getMethodSignature(fn).args
-        # TODO: add exception description
-        def inject_wrapper(*args, **kwargs):
+        if fn.__name__ != '__init__':
+            setattr(fn, constants.INJECT_BEFORE, 1)
+            return fn
+
+        def inject_wrapper(*args, **kwags):
             scope = glob.lastScope
             nkwargs = {}
             nargs = [args[0]]
             for arg_name in args_signature:
                 if arg_name == "self":
                     continue
                 if arg_name not in annotations_signature:
```

### Comparing `scopeton-2.3/scopeton/objects.py` & `scopeton-2.4/scopeton/objects.py`

 * *Files identical despite different names*

### Comparing `scopeton-2.3/scopeton/qualifier_tree.py` & `scopeton-2.4/scopeton/qualifier_tree.py`

 * *Files identical despite different names*

### Comparing `scopeton-2.3/scopeton/scope.py` & `scopeton-2.4/scopeton/scope.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import logging
 from threading import RLock
 
 import typing
 
-from scopeton import compat, glob
+from scopeton import compat, glob, constants
 from scopeton.objects import Bean
 from scopeton.qualifier_tree import QualifierTree
 from scopeton.scopeTools import getBean_qualifier, callMethodByName, getClassTree, flatten, ScopetonException
 
 T = typing.TypeVar("T")
 
+
 class Scope(object):
     '''this is servicelocator pattern implementation'''
+
     def __init__(self, lock=False, initMethod="postConstruct", destroyMethod="preDestroy", parent=None):
         self._singletons = QualifierTree()
         self._beans = QualifierTree()
-        self.lock = lock or RLock()       # type: RLock
+        self.lock = lock or RLock()  # type: RLock
         self.initMethod = initMethod
         self.destroyMethod = destroyMethod
-        self.parent = parent  #type:  Scope
+        self.parent = parent  # type:  Scope
         self.servicesStarted = False
         self.children = []  # type: typing.List[Scope]
         self.registerInstance(self.__class__, self)
         if parent:
             parent.children.append(self)
 
     def getInstance(self, name: typing.Type[T]) -> T:
@@ -45,21 +47,25 @@
         bean = self._beans.find_one_by_qualifier_name(suitableQualifier)
         glob.lastScope = self
         if compat.hasInject(bean.cls.__init__):
             instance = bean.cls()
         elif len(compat.getMethodSignature(bean.cls.__init__).args) == 2:
             instance = bean.cls(self)
         elif len(compat.getMethodSignature(bean.cls.__init__).args) > 2:
-            raise ScopetonException("Invalid number of parameters for bean constructor, maybe @Inject() decorator forgotten: {}".format(compat.getMethodSignature(bean.cls.__init__).args))
+            raise ScopetonException(
+                "Invalid number of parameters for bean constructor, maybe @Inject() decorator forgotten: {}".format(
+                    compat.getMethodSignature(bean.cls.__init__).args))
         else:
             instance = bean.cls()
 
         if bean.singleton:
             self.registerInstance(suitableQualifier, instance)
 
+        self._inject_injectables(instance)
+
         return instance
 
     def registerInstance(self, name, instance):
         qualifier = getBean_qualifier(name)
         suitableQualifier = self._beans.find_suitable_qualifier(qualifier)
         logging.debug("Suitable qualifier for {} is: {}".format(qualifier, suitableQualifier))
         self._singletons.register(suitableQualifier, instance)
@@ -75,15 +81,14 @@
         logging.debug("Removing scope: {}".format(self))
         self.stopServices()
         for k in self.children[:]:
             k.remove()
         if self.parent:
             self.parent.children.remove(self)
 
-
     def _registerBean(self, bean):
         """
         :type bean: Bean
         """
         for name in bean.qualifier_tree:
             logging.debug("Registering: {} as {}".format(name, bean))
             self._beans.register(name, bean)
@@ -103,7 +108,23 @@
             self.servicesStarted = False
             for bean in self._beans.get_all_objects():
                 if bean.service:
                     callMethodByName(self.getInstance(bean), self.destroyMethod)
             for childScope in self.children:
                 childScope.stopServices()
 
+    def _inject_injectables(self, instance):
+        for fn in compat.getMethods(instance):
+            if hasattr(fn[1], constants.INJECT_BEFORE):
+                annotations_signature = compat.getMethodSignature(fn[1]).annotations
+                args_signature = compat.getMethodSignature(fn[1]).args
+                nargs = []
+                for arg_name in args_signature:
+                    if arg_name == "self":
+                        continue
+                    if arg_name not in annotations_signature:
+                        raise ScopetonException("Not annotated inject argument: {}".format(arg_name))
+                    arg_type = annotations_signature[arg_name]
+                    arg_to_inject = self.getInstance(arg_type)
+                    nargs.append(arg_to_inject)
+                fn[1](*nargs)
+
```

### Comparing `scopeton-2.3/scopeton/scopeTools.py` & `scopeton-2.4/scopeton/scopeTools.py`

 * *Files identical despite different names*

