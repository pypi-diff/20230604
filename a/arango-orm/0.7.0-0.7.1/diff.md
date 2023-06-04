# Comparing `tmp/arango-orm-0.7.0.tar.gz` & `tmp/arango_orm-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arango-orm-0.7.0.tar", last modified: Tue Apr 26 06:19:52 2022, max compression
+gzip compressed data, was "arango_orm-0.7.1.tar", max compression
```

## Comparing `arango-orm-0.7.0.tar` & `arango_orm-0.7.1.tar`

### file list

```diff
@@ -1,64 +1,15 @@
-drwxrwxr-x   0 kashif    (1000) kashif    (1000)        0 2022-04-26 06:19:52.457498 arango-orm-0.7.0/
-drwxrwxr-x   0 kashif    (1000) kashif    (1000)        0 2022-04-26 06:19:52.301492 arango-orm-0.7.0/.github/
-drwxrwxr-x   0 kashif    (1000) kashif    (1000)        0 2022-04-26 06:19:52.325493 arango-orm-0.7.0/.github/workflows/
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      716 2022-04-20 14:21:18.000000 arango-orm-0.7.0/.github/workflows/stale.yml
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     1113 2020-07-23 09:37:52.000000 arango-orm-0.7.0/.gitignore
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     6369 2022-04-26 06:17:22.000000 arango-orm-0.7.0/CHANGELOG.rst
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      140 2020-07-23 09:14:41.000000 arango-orm-0.7.0/Dockerfile
--rw-rw-r--   0 kashif    (1000) kashif    (1000)    35141 2017-09-16 01:26:41.000000 arango-orm-0.7.0/LICENSE.txt
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      457 2022-04-26 06:19:52.457498 arango-orm-0.7.0/PKG-INFO
--rw-rw-r--   0 kashif    (1000) kashif    (1000)    21401 2020-12-14 00:47:25.000000 arango-orm-0.7.0/README.rst
-drwxrwxr-x   0 kashif    (1000) kashif    (1000)        0 2022-04-26 06:19:52.373495 arango-orm-0.7.0/arango_orm/
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      236 2018-10-13 00:36:15.000000 arango-orm-0.7.0/arango_orm/__init__.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)    16024 2022-04-21 05:46:36.000000 arango-orm-0.7.0/arango_orm/collections.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     3309 2018-10-13 00:36:42.000000 arango-orm-0.7.0/arango_orm/connection_pool.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)    22473 2020-08-17 21:25:07.000000 arango-orm-0.7.0/arango_orm/database.py
-drwxrwxr-x   0 kashif    (1000) kashif    (1000)        0 2022-04-26 06:19:52.381495 arango-orm-0.7.0/arango_orm/event/
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      790 2017-12-28 20:28:29.000000 arango-orm-0.7.0/arango_orm/event/__init__.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      427 2019-03-27 21:44:12.000000 arango-orm-0.7.0/arango_orm/exceptions.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)       33 2017-09-04 22:16:09.000000 arango-orm-0.7.0/arango_orm/fields.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)    12783 2021-08-03 02:30:18.000000 arango-orm-0.7.0/arango_orm/graph.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     8642 2021-04-26 07:32:46.000000 arango-orm-0.7.0/arango_orm/query.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     2375 2017-12-29 11:43:52.000000 arango-orm-0.7.0/arango_orm/references.py
-drwxrwxr-x   0 kashif    (1000) kashif    (1000)        0 2022-04-26 06:19:52.381495 arango-orm-0.7.0/arango_orm.egg-info/
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      457 2022-04-26 06:19:51.000000 arango-orm-0.7.0/arango_orm.egg-info/PKG-INFO
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     1238 2022-04-26 06:19:52.000000 arango-orm-0.7.0/arango_orm.egg-info/SOURCES.txt
--rw-rw-r--   0 kashif    (1000) kashif    (1000)        1 2022-04-26 06:19:51.000000 arango-orm-0.7.0/arango_orm.egg-info/dependency_links.txt
--rw-rw-r--   0 kashif    (1000) kashif    (1000)       35 2022-04-26 06:19:51.000000 arango-orm-0.7.0/arango_orm.egg-info/requires.txt
--rw-rw-r--   0 kashif    (1000) kashif    (1000)       17 2022-04-26 06:19:51.000000 arango-orm-0.7.0/arango_orm.egg-info/top_level.txt
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      512 2020-07-23 09:14:41.000000 arango-orm-0.7.0/docker-compose.yml
-drwxrwxr-x   0 kashif    (1000) kashif    (1000)        0 2022-04-26 06:19:52.413496 arango-orm-0.7.0/docs/
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      634 2020-07-23 09:35:07.000000 arango-orm-0.7.0/docs/Makefile
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      307 2021-04-20 14:51:15.000000 arango-orm-0.7.0/docs/api-reference.rst
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     1956 2021-04-20 14:39:44.000000 arango-orm-0.7.0/docs/conf.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     4787 2021-04-20 03:08:09.000000 arango-orm-0.7.0/docs/getting-started.rst
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      861 2021-04-20 14:41:32.000000 arango-orm-0.7.0/docs/index.rst
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      795 2020-07-23 09:35:07.000000 arango-orm-0.7.0/docs/make.bat
-drwxrwxr-x   0 kashif    (1000) kashif    (1000)        0 2022-04-26 06:19:52.429497 arango-orm-0.7.0/examples/
--rw-rw-r--   0 kashif    (1000) kashif    (1000)   290424 2016-10-27 19:20:38.000000 arango-orm-0.7.0/examples/Universite_Database_and_Graph_Example.html
--rw-rw-r--   0 kashif    (1000) kashif    (1000)    15925 2016-10-27 19:20:38.000000 arango-orm-0.7.0/examples/Universite_Database_and_Graph_Example.ipynb
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     1417 2018-09-09 13:14:21.000000 arango-orm-0.7.0/examples/simple_teacher_student_graph.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     8441 2019-01-19 23:31:15.000000 arango-orm-0.7.0/examples/university_graph.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      517 2020-07-23 09:14:41.000000 arango-orm-0.7.0/getting-started.rst
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      707 2019-05-08 18:17:57.000000 arango-orm-0.7.0/recipes.md
--rw-rw-r--   0 kashif    (1000) kashif    (1000)       41 2022-04-26 06:15:12.000000 arango-orm-0.7.0/requirements.txt
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      109 2022-04-26 06:19:52.457498 arango-orm-0.7.0/setup.cfg
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      681 2022-04-26 06:17:37.000000 arango-orm-0.7.0/setup.py
-drwxrwxr-x   0 kashif    (1000) kashif    (1000)        0 2022-04-26 06:19:52.445497 arango-orm-0.7.0/temp_test/
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     2694 2016-09-30 15:40:33.000000 arango-orm-0.7.0/temp_test/test_code.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      974 2017-06-22 04:05:28.000000 arango-orm-0.7.0/temp_test/test_extra_fields.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     2318 2017-12-29 11:52:29.000000 arango-orm-0.7.0/temp_test/test_ref_relationships.py
-drwxrwxr-x   0 kashif    (1000) kashif    (1000)        0 2022-04-26 06:19:52.449498 arango-orm-0.7.0/tests/
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     2095 2020-08-17 21:48:24.000000 arango-orm-0.7.0/tests/__init__.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      782 2020-08-17 21:45:15.000000 arango-orm-0.7.0/tests/conftest.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     9859 2020-12-14 00:47:25.000000 arango-orm-0.7.0/tests/data.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     8156 2020-07-23 09:14:41.000000 arango-orm-0.7.0/tests/test_collections.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)    14430 2020-08-17 21:25:07.000000 arango-orm-0.7.0/tests/test_database.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     2647 2018-05-09 11:10:24.000000 arango-orm-0.7.0/tests/test_event.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     9392 2017-09-16 00:32:34.000000 arango-orm-0.7.0/tests/test_graph.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     1553 2020-12-13 20:37:52.000000 arango-orm-0.7.0/tests/test_inheritance_mapping.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     1517 2020-12-14 00:47:25.000000 arango-orm-0.7.0/tests/test_inheritance_multiple.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     1576 2020-12-13 20:37:52.000000 arango-orm-0.7.0/tests/test_inheritance_resolver.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)     7694 2018-09-28 11:12:36.000000 arango-orm-0.7.0/tests/test_query.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      233 2017-12-28 20:28:29.000000 arango-orm-0.7.0/tests/utils.py
--rw-rw-r--   0 kashif    (1000) kashif    (1000)      349 2017-12-28 20:28:29.000000 arango-orm-0.7.0/tox.ini
+-rw-r--r--   0        0        0    35141 2023-06-04 18:17:00.395211 arango_orm-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0    21405 2023-06-04 18:17:00.395211 arango_orm-0.7.1/README.rst
+-rw-r--r--   0        0        0      236 2023-06-04 18:17:00.395211 arango_orm-0.7.1/arango_orm/__init__.py
+-rw-r--r--   0        0        0    16436 2023-06-04 18:17:00.395211 arango_orm-0.7.1/arango_orm/collections.py
+-rw-r--r--   0        0        0     3463 2023-06-04 18:17:00.395211 arango_orm-0.7.1/arango_orm/connection_pool.py
+-rw-r--r--   0        0        0    22738 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/database.py
+-rw-r--r--   0        0        0      790 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/event/__init__.py
+-rw-r--r--   0        0        0      427 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/exceptions.py
+-rw-r--r--   0        0        0       33 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/fields.py
+-rw-r--r--   0        0        0    12783 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/graph.py
+-rw-r--r--   0        0        0     8908 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/query.py
+-rw-r--r--   0        0        0     2375 2023-06-04 18:17:00.399211 arango_orm-0.7.1/arango_orm/references.py
+-rw-r--r--   0        0        0      615 2023-06-04 18:17:00.399211 arango_orm-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    23097 1970-01-01 00:00:00.000000 arango_orm-0.7.1/setup.py
+-rw-r--r--   0        0        0    22070 1970-01-01 00:00:00.000000 arango_orm-0.7.1/PKG-INFO
```

### Comparing `arango-orm-0.7.0/LICENSE.txt` & `arango_orm-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arango-orm-0.7.0/README.rst` & `arango_orm-0.7.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     from arango_orm import Collection
     from arango_orm.fields import String, Date
 
     class Student(Collection):
 
         __collection__ = 'students'
-        _index = [{'type': 'hash', fields: ['name'], unique=False}]
+        _index = [{'type': 'hash', 'fields': ['name'], 'unique': True}]
 
         _key = String(required=True)  # registration number
         name = String(required=True, allow_none=False)
         dob = Date()
 
 
 Create Collection in the Database
```

### Comparing `arango-orm-0.7.0/arango_orm/collections.py` & `arango_orm-0.7.1/arango_orm/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,40 +92,50 @@
                     base_objects_dict = c.get_objects_dict()
                     for i, f in [(i, f) for i, f in base_objects_dict.items() if i not in objects_dict]:
                         objects_dict[i] = f
 
         return objects_dict
 
     @classmethod
-    def schema(cls,only:typing.List[str]=None):
-        '''schema caches Marshmellow Schemas on this class to preserve memory'''
-        if not hasattr(cls,'_cls_schema'):
-            objects_dict = cls.get_objects_dict()
+    def get_schema_class(cls):
+        '''Return schema class (not an instance)'''
+        if (not hasattr(cls,'_cls_schema') or
+            cls._cls_schema.__name__ != cls.__name__ + "Schema"): 
+            #print("Getting schema " + cls.__name__)
             cls._cls_schema = type(
-                cls.__name__ + "Schema", (ObjectSchema,), objects_dict
+                cls.__name__ + "Schema", (ObjectSchema,), cls.get_objects_dict()
             )
+        return cls._cls_schema
+
+    @classmethod
+    def schema(cls,only:typing.List[str]=None):
+        '''schema caches Marshmellow Schemas instance on this class to preserve memory'''
         
+        # check if exist schema or regenerate in case of class inheritance
+        cls.get_schema_class()
+
         # Extra fields related schema configuration
         unknown = EXCLUDE
         if cls._allow_extra_fields is True:
-            unknown = INCLUDE            
+            unknown = INCLUDE 
 
-        if not hasattr(cls,'_cls_schema_cache'):
+        if (not hasattr(cls,'_cls_schema_cache') or 
+            cls._cls_schema_cache[None].__class__.__name__ != cls.__name__ + "Schema"): 
             #print(f'making {cls.__name__} schema with only=None')
             SC = cls._cls_schema()
             SC.unknown = unknown
             SC.object_class = cls
             cls._cls_schema_cache = {None:SC}
 
         if only is not None:
             #create a unique schema for this input by using a hashable set
             if isinstance(only,(list,tuple)): 
                 onlyKey = str(set(only)) #garuntees order / uniquness and hashability
             else:
-                onlyKey = only 
+                onlyKey = only
 
             if onlyKey not in cls._cls_schema_cache:
                 SC = cls._cls_schema(only=only)
                 SC.unknown = unknown
                 SC.object_class = cls
                 cls._cls_schema_cache[onlyKey] = SC #asssign the unique schema for only
```

### Comparing `arango-orm-0.7.0/arango_orm/connection_pool.py` & `arango_orm-0.7.1/arango_orm/connection_pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,18 @@
         """Database.add wrapper."""
         return self._db.add(entity)
 
     def delete(self, entity, **kwargs):
         """Database.delete wrapper."""
         return self._db.delete(entity, **kwargs)
 
+    def bulk_delete(self, entity_list, **kwargs):
+        """Database.bulk_delete wrapper."""
+        return self._db.bulk_delete(entity_list, **kwargs)
+
     def update(self, entity, only_dirty=False, **kwargs):
         """Database.update wrapper."""
         return self._db.update(entity, only_dirty=only_dirty, **kwargs)
 
     def query(self, CollectionClass):
         """Database.query wrapper."""
         return self._db.query(CollectionClass)
```

### Comparing `arango-orm-0.7.0/arango_orm/database.py` & `arango_orm-0.7.1/arango_orm/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,21 @@
 
         collection = self._db.collection(entity.__collection__)
         res = collection.delete(entity._dump(only=("_key",))["_key"], **kwargs)
 
         dispatch(entity, "post_delete", db=self, result=res)
         return res
 
+    def bulk_delete(self, entity_list, **kwargs):
+        '''Bulk delete utility, based on delete method. Return a list of results.'''
+        res = []
+        for entity in entity_list:
+            res.append(self.delete(entity, **kwargs))
+        return res    
+
     def update(self, entity, only_dirty=False, **kwargs):
         "Update given document"
         collection = self._db.collection(entity.__collection__)
         data = entity._dump()
 
         if only_dirty:
             if not entity._dirty:
```

### Comparing `arango-orm-0.7.0/arango_orm/event/__init__.py` & `arango_orm-0.7.1/arango_orm/event/__init__.py`

 * *Files identical despite different names*

### Comparing `arango-orm-0.7.0/arango_orm/graph.py` & `arango_orm-0.7.1/arango_orm/graph.py`

 * *Files identical despite different names*

### Comparing `arango-orm-0.7.0/arango_orm/query.py` & `arango_orm-0.7.1/arango_orm/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,24 @@
         aql += "\n COLLECT WITH COUNT INTO rec_count RETURN rec_count"
         # print(aql)
 
         results = self._db.aql.execute(aql, bind_vars=self._bind_vars)
 
         return next(results)
 
+    def full_count(self):
+        "Return collection full count"
+
+        aql = self._make_aql()
+
+        aql += "\n RETURN rec"
+
+        cursor = self._db.aql.execute(aql, bind_vars=self._bind_vars, full_count=True)
+        return cursor.statistics()['fullCount']
+
     def by_key(self, key, **kwargs):
         "Return a single document using it's key"
 
         doc_dict = self._db.collection(
             self._CollectionClass.__collection__
         ).get(key, **kwargs)
         if doc_dict is None:
```

### Comparing `arango-orm-0.7.0/arango_orm/references.py` & `arango_orm-0.7.1/arango_orm/references.py`

 * *Files identical despite different names*

