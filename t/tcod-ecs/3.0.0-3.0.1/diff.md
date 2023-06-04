# Comparing `tmp/tcod_ecs-3.0.0.tar.gz` & `tmp/tcod_ecs-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod_ecs-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tcod_ecs-3.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcod_ecs-3.0.0.tar` & `tcod_ecs-3.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1079 2023-05-29 16:49:45.307406 tcod_ecs-3.0.0/LICENSE
--rw-r--r--   0        0        0     8627 2023-05-29 16:49:45.307406 tcod_ecs-3.0.0/README.md
--rw-r--r--   0        0        0     3688 2023-05-29 16:49:45.307406 tcod_ecs-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    35405 2023-05-29 16:49:45.307406 tcod_ecs-3.0.0/tcod/ecs/__init__.py
--rw-r--r--   0        0        0      160 2023-05-29 16:49:53.175620 tcod_ecs-3.0.0/tcod/ecs/_version.py
--rw-r--r--   0        0        0        0 2023-05-29 16:49:45.307406 tcod_ecs-3.0.0/tcod/ecs/py.typed
--rw-r--r--   0        0        0     9822 1970-01-01 00:00:00.000000 tcod_ecs-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-04 11:34:17.745244 tcod_ecs-3.0.1/LICENSE
+-rw-r--r--   0        0        0     8627 2023-06-04 11:34:17.745244 tcod_ecs-3.0.1/README.md
+-rw-r--r--   0        0        0     3688 2023-06-04 11:34:17.745244 tcod_ecs-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    35784 2023-06-04 11:34:17.745244 tcod_ecs-3.0.1/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0      160 2023-06-04 11:34:26.389237 tcod_ecs-3.0.1/tcod/ecs/_version.py
+-rw-r--r--   0        0        0        0 2023-06-04 11:34:17.745244 tcod_ecs-3.0.1/tcod/ecs/py.typed
+-rw-r--r--   0        0        0     9822 1970-01-01 00:00:00.000000 tcod_ecs-3.0.1/PKG-INFO
```

### Comparing `tcod_ecs-3.0.0/LICENSE` & `tcod_ecs-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod_ecs-3.0.0/README.md` & `tcod_ecs-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tcod_ecs-3.0.0/pyproject.toml` & `tcod_ecs-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tcod_ecs-3.0.0/tcod/ecs/__init__.py` & `tcod_ecs-3.0.1/tcod/ecs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """A type-hinted Entity Component System based on Python dictionaries and sets."""
 from __future__ import annotations
 
 import sys
+import warnings
 from collections import defaultdict
-from functools import partial
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Final,
     Generic,
     Iterable,
@@ -626,14 +626,24 @@
         return EntityComponentRelationMapping(self.entity, key)
 
     def __delitem__(self, key: _ComponentKey[object]) -> None:
         """Remove all relations associated with this component key."""
         EntityComponentRelationMapping(self.entity, key).clear()
 
 
+def _defaultdict_of_set() -> defaultdict[_T1, set[_T2]]:
+    """Return a new defaultdict of sets."""
+    return defaultdict(set)
+
+
+def _defaultdict_of_dict() -> defaultdict[_T1, dict[_T2, _T3]]:
+    """Return a new defaultdict of dicts."""
+    return defaultdict(dict)
+
+
 class World:
     """A container for entities and components."""
 
     def __init__(self) -> None:
         """Initialize a new world."""
         self._components_by_type: defaultdict[_ComponentKey[object], dict[Entity, Any]] = defaultdict(dict)
         """Query table entity components.
@@ -654,25 +664,23 @@
         self._tags_by_entity: defaultdict[Entity, set[Any]] = defaultdict(set)
         """Random access entity tags.
 
         dict[Entity] = {all_tags_for_entity}
         """
 
         self._relation_tags_by_entity: defaultdict[Entity, defaultdict[object, set[Entity]]] = defaultdict(
-            partial(defaultdict, set)  # type: ignore[arg-type]
+            _defaultdict_of_set
         )
         """Random access tag multi-relations.
 
         dict[entity][tag] = {target_entities}
         """
         self._relation_components_by_entity: defaultdict[
             Entity, defaultdict[_ComponentKey[object], dict[Entity, Any]]
-        ] = defaultdict(
-            partial(defaultdict, dict)  # type: ignore[arg-type]
-        )
+        ] = defaultdict(_defaultdict_of_dict)
         """Random access relations owning components.
 
         dict[entity][ComponentKey][target_entity] = component
         """
         self._relations_lookup: defaultdict[
             tuple[Any, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None], set[Entity]
         ] = defaultdict(set)
@@ -711,28 +719,33 @@
         This entity has a `uid` of `None` and may be accessed that way.
         This syntax my be better for globals in general since it can use any hashable object.
 
         .. versionadded:: 1.1
 
         Example::
 
-            >>> world.global_.components[("turn", int)] = 0
-            >>> world[None].components[("turn", int)]  # Alternative syntax
+            >>> world[None].components[("turn", int)] = 0
+            >>> world[None].components[("turn", int)]
             0
         """
+        warnings.warn(
+            "The 'world.global_' attribute has been deprecated. Use 'world[None]' to access this entity.",
+            FutureWarning,
+            stacklevel=2,
+        )
         return Entity(self, None)
 
     def __setstate__(self, state: dict[str, Any]) -> None:
         """Unpickle this object and handle state migration."""
-        state.pop("global_", None)  # Migrate from version <=1.2.0.
+        global_: Entity | None = state.pop("global_", None)  # Migrate from version <=1.2.0.
 
         self.__dict__.update(state)
 
-        if self.global_.uid is not None:  # Migrate from version <=1.2.0.
-            self.global_._force_remap(None)
+        if global_ is not None and global_.uid is not None:  # Migrate from version <=1.2.0.
+            global_._force_remap(None)
 
     def __getitem__(self, uid: object) -> Entity:
         """Return an entity associated with a unique id.
 
         Example::
 
             >>> world = World()
```

### Comparing `tcod_ecs-3.0.0/PKG-INFO` & `tcod_ecs-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 3.0.0
+Version: 3.0.1
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

