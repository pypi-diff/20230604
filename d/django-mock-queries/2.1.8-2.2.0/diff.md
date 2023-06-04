# Comparing `tmp/django_mock_queries-2.1.8-py2.py3-none-any.whl.zip` & `tmp/django_mock_queries-2.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 19939 bytes, number of entries: 13
+Zip file size: 20284 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-04 20:17 django_mock_queries/__init__.py
--rw-rw-r--  2.0 unx     3153 b- defN 23-Jun-04 20:04 django_mock_queries/asserts.py
+-rw-rw-r--  2.0 unx     3091 b- defN 23-Jun-04 20:08 django_mock_queries/asserts.py
 -rw-rw-r--  2.0 unx     1673 b- defN 23-May-04 20:17 django_mock_queries/comparisons.py
 -rw-rw-r--  2.0 unx     2378 b- defN 23-May-04 20:17 django_mock_queries/constants.py
 -rw-rw-r--  2.0 unx       95 b- defN 23-May-04 20:17 django_mock_queries/exceptions.py
--rw-rw-r--  2.0 unx    17059 b- defN 23-Jun-04 20:04 django_mock_queries/mocks.py
--rw-rw-r--  2.0 unx    16646 b- defN 23-Jun-04 20:04 django_mock_queries/query.py
--rw-rw-r--  2.0 unx     9651 b- defN 23-Jun-04 20:04 django_mock_queries/utils.py
--rw-rw-r--  2.0 unx     1079 b- defN 23-Jun-04 20:05 django_mock_queries-2.1.8.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     8158 b- defN 23-Jun-04 20:05 django_mock_queries-2.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-04 20:05 django_mock_queries-2.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-Jun-04 20:05 django_mock_queries-2.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1148 b- defN 23-Jun-04 20:05 django_mock_queries-2.1.8.dist-info/RECORD
-13 files, 61170 bytes uncompressed, 17995 bytes compressed:  70.6%
+-rw-rw-r--  2.0 unx    17181 b- defN 23-Jun-04 20:08 django_mock_queries/mocks.py
+-rw-rw-r--  2.0 unx    16446 b- defN 23-Jun-04 20:08 django_mock_queries/query.py
+-rw-rw-r--  2.0 unx    11078 b- defN 23-Jun-04 20:08 django_mock_queries/utils.py
+-rw-rw-r--  2.0 unx     1079 b- defN 23-Jun-04 20:12 django_mock_queries-2.2.0.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     7925 b- defN 23-Jun-04 20:12 django_mock_queries-2.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-04 20:12 django_mock_queries-2.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-Jun-04 20:12 django_mock_queries-2.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1149 b- defN 23-Jun-04 20:12 django_mock_queries-2.2.0.dist-info/RECORD
+13 files, 62225 bytes uncompressed, 18340 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: django_mock_queries/query.py
 Comment: 
 
 Filename: django_mock_queries/utils.py
 Comment: 
 
-Filename: django_mock_queries-2.1.8.dist-info/LICENSE.txt
+Filename: django_mock_queries-2.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: django_mock_queries-2.1.8.dist-info/METADATA
+Filename: django_mock_queries-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: django_mock_queries-2.1.8.dist-info/WHEEL
+Filename: django_mock_queries-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: django_mock_queries-2.1.8.dist-info/top_level.txt
+Filename: django_mock_queries-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: django_mock_queries-2.1.8.dist-info/RECORD
+Filename: django_mock_queries-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_mock_queries/asserts.py

```diff
@@ -1,11 +1,8 @@
-try:
-    from unittest.mock import patch, Mock
-except ImportError:
-    from mock import patch, Mock
+from unittest.mock import patch, Mock
 
 from model_bakery import baker
 
 from .constants import *
 
 SkipField = locate('rest_framework.fields.SkipField')
```

## django_mock_queries/mocks.py

```diff
@@ -5,18 +5,15 @@
 from django.apps import apps
 from django.db import connections
 from django.db.backends.base import creation
 from django.db.models import Model
 from django.db.utils import ConnectionHandler, NotSupportedError
 from functools import partial
 from itertools import chain
-try:
-    from unittest.mock import Mock, MagicMock, patch, PropertyMock
-except ImportError:
-    from mock import Mock, MagicMock, patch, PropertyMock
+from unittest.mock import Mock, MagicMock, patch, PropertyMock
 
 from types import MethodType
 
 from .constants import DjangoModelDeletionCollector, DjangoDbRouter
 from .query import MockSet
 
 # noinspection PyUnresolvedReferences
@@ -87,15 +84,15 @@
     mock_connection = ConnectionHandler.__getitem__.return_value
     if disabled_features:
         for feature in disabled_features:
             setattr(mock_connection.features, feature, False)
     mock_ops = mock_connection.ops
 
     # noinspection PyUnusedLocal
-    def compiler(queryset, connection, using, **kwargs):
+    def compiler(queryset, using=None, connection=None, elide_empty=True, **kwargs):
         result = MagicMock(name='mock_connection.ops.compiler()')
         # noinspection PyProtectedMember
         result.execute_sql.side_effect = NotSupportedError(
             "Mock database tried to execute SQL for {} model.".format(
                 queryset.model._meta.object_name))
         result.has_results.side_effect = result.execute_sql.side_effect
         return result
@@ -103,15 +100,15 @@
     mock_ops.compiler.return_value.side_effect = compiler
     mock_ops.integer_field_range.return_value = (-sys.maxsize - 1, sys.maxsize)
     mock_ops.max_name_length.return_value = sys.maxsize
 
     Model.refresh_from_db = Mock()  # Make this into a noop.
 
 
-class MockMap(object):
+class MockMap:
     def __init__(self, original):
         """ Wrap a mock mapping around the original one-to-many relation. """
         self.map = {}
         self.original = original
 
     def __set__(self, instance, value):
         """ Set a related object for an instance. """
@@ -250,15 +247,15 @@
                     patchers.append(_patch_relation(
                         model, name, related_object
                     ))
 
     return PatcherChain(patchers, pass_mocks=False)
 
 
-class PatcherChain(object):
+class PatcherChain:
     """ Chain a list of mock patchers into one.
 
     The resulting patcher can be used just like one from the mock module:
     As a test method decorator, a test class decorator, a context manager,
     or by just calling start() and stop().
     """
 
@@ -324,15 +321,15 @@
         return [patcher.start() for patcher in self.patchers]
 
     def stop(self):
         for patcher in reversed(self.patchers):
             patcher.stop()
 
 
-class Mocker(object):
+class Mocker:
     """
     A decorator that patches multiple class methods with a magic mock instance that does nothing.
     """
 
     shared_mocks = {}
     shared_patchers = {}
     shared_original = {}
@@ -428,15 +425,15 @@
 class ModelMocker(Mocker):
     """
     A decorator that patches django base model's db read/write methods and wires them to a MockSet.
     """
 
     default_methods = ['objects', '_do_update']
 
-    if django.VERSION[0] == 3:
+    if django.VERSION[0] >= 3:
         default_methods += ['_base_manager._insert', ]
     else:
         default_methods += ['_meta.base_manager._insert', ]
 
     default_methods = tuple(default_methods)
 
     def __init__(self, cls, *methods, **kwargs):
@@ -465,15 +462,18 @@
 
         return self._obj_pk(obj)
 
     def _base_manager__insert(self, objects, *_, **__):
         obj = objects[0]
         self.objects.add(obj)
 
-        return [self._obj_pk(obj)]
+        # Do not set anything on the model instance itself, as we do not get any values from the database.
+        # The object ID is being set automatically.
+        # Reference: `django.db.models.base.Model._save_table`
+        return []
 
     def _do_update(self, *args, **_):
         _, _, pk_val, values, _, _ = args
         objects = self.objects.filter(pk=pk_val)
 
         if objects.exists():
             attrs = {field.name: value for field, _, value in values if value is not None}
```

## django_mock_queries/query.py

```diff
@@ -1,31 +1,28 @@
 import datetime
 import random
 from collections import OrderedDict, namedtuple
-from six import with_metaclass
-try:
-    from unittest.mock import Mock, MagicMock, PropertyMock
-except ImportError:
-    from mock import Mock, MagicMock, PropertyMock
+from unittest.mock import Mock, MagicMock, PropertyMock
 
 from .constants import *
 from .exceptions import *
 from .utils import (
-    matches, merge, intersect, get_attribute, validate_mock_set, is_list_like_iter, flatten_list, truncate, hash_dict
+    matches, get_attribute, validate_mock_set, is_list_like_iter, flatten_list, truncate,
+    hash_dict, filter_results
 )
 
 
 class MockSetMeta(type):
     def __call__(cls, *initial_items, **kwargs):
         obj = super(MockSetMeta, cls).__call__(**kwargs)
         obj.add(*initial_items)
         return obj
 
 
-class MockSet(with_metaclass(MockSetMeta, MagicMock)):
+class MockSet(MagicMock, metaclass=MockSetMeta):
     EVENT_ADDED = 'added'
     EVENT_UPDATED = 'updated'
     EVENT_SAVED = 'saved'
     EVENT_DELETED = 'deleted'
     SUPPORTED_EVENTS = [EVENT_ADDED, EVENT_UPDATED, EVENT_SAVED, EVENT_DELETED]
     RETURN_SELF_METHODS = [
         'all',
@@ -91,55 +88,51 @@
             for obj in models:
                 self._register_fields(obj)
 
         for model in models:
             self.items.append(model)
             self.fire(model, self.EVENT_ADDED, self.EVENT_SAVED)
 
-    def _filter_single_q(self, source, q_obj, negated):
-        if isinstance(q_obj, DjangoQ):
-            return self._filter_q(source, q_obj)
-        else:
-            return matches(negated=negated, *source, **{q_obj[0]: q_obj[1]})
-
-    def _filter_q(self, source, query):
-        results = []
-
-        for child in query.children:
-            filtered = self._filter_single_q(source, child, query.negated)
-
-            if filtered:
-                if not results or query.connector == CONNECTORS_OR:
-                    results = merge(results, filtered)
-                else:
-                    results = intersect(results, filtered)
-            elif query.connector == CONNECTORS_AND:
-                return []
-
-        return results
-
     def filter(self, *args, **attrs):
         results = list(self.items)
         for x in args:
             if not isinstance(x, DjangoQ):
                 raise ArgumentNotSupported()
 
             if len(x) > 0:
-                results = self._filter_q(results, x)
+                results = filter_results(results, x)
 
         return self._mockset_class()(*matches(*results, **attrs), clone=self)
 
     def exclude(self, *args, **attrs):
         excluded = set(self.filter(*args, **attrs))
         results = [item for item in self.items if item not in excluded]
         return self._mockset_class()(*results, clone=self)
 
     def exists(self):
         return len(self.items) > 0
 
+    def in_bulk(self, id_list=None, *, field_name='pk'):
+        result = {}
+        for model in self.items:
+            if id_list is None or getattr(model, field_name) in id_list:
+                result[getattr(model, field_name)] = model
+        return result
+
+    def annotate(self, **kwargs):
+        results = list(self.items)
+        for key, value in kwargs.items():
+            for row in results:
+                if not hasattr(row, '_annotated_fields'):
+                    row._annotated_fields = []
+                row._annotated_fields.append(key)
+                setattr(row, key, get_attribute(row, value)[0])
+
+        return MockSet(*results, clone=self)
+
     def aggregate(self, *args, **kwargs):
         result = {}
 
         for expr in set(args):
             kwargs['{0}__{1}'.format(expr.source_expressions[0].name, expr.function).lower()] = expr
 
         for alias, expr in kwargs.items():
@@ -468,15 +461,15 @@
 
 def create_model(*fields):
     if len(fields) == 0:
         raise ValueError('create_model() is called without fields specified')
     return MockModel(**{f: None for f in fields})
 
 
-class MockOptions(object):
+class MockOptions:
     def __init__(self, *field_names):
         self.load_fields(*field_names)
         self.get_latest_by = None
 
     def load_fields(self, *field_names):
         fields = {name: MockField(name) for name in field_names}
 
@@ -490,11 +483,11 @@
         for key in ('local_concrete_fields', 'concrete_fields', 'fields'):
             self.__dict__[key] = []
 
             for name, obj in fields.items():
                 self.__dict__[key].append(obj)
 
 
-class MockField(object):
+class MockField:
     def __init__(self, field):
         for key in ('name', 'attname'):
             self.__dict__[key] = field
```

## django_mock_queries/utils.py

```diff
@@ -1,13 +1,12 @@
 from datetime import datetime, date
 from django.core.exceptions import FieldError
-try:
-    from unittest.mock import Mock
-except ImportError:
-    from mock import Mock
+from django.db.models import F, Value, Case
+from django.db.models.functions import Coalesce
+from unittest.mock import Mock
 
 from .comparisons import *
 from .constants import *
 from .exceptions import *
 
 import django_mock_queries.query
 
@@ -26,23 +25,24 @@
 
     if name[-4:] == '_set':
         return {model_name: name}
     else:
         return {name: name}
 
 
-def find_field_names_from_meta(meta, **kwargs):
+def find_field_names_from_meta(meta, annotated=None, **kwargs):
     field_names = {}
+    annotated = annotated or []
     concrete_only = kwargs.get('concrete_only', False)
 
     if concrete_only:
-        fields_no_mapping = [f.attname for f in meta.concrete_fields]
+        fields_no_mapping = [f.attname for f in meta.concrete_fields] + annotated
         fields_with_mapping = []
     else:
-        fields_no_mapping = [f for f in meta._forward_fields_map.keys()]
+        fields_no_mapping = [f for f in meta._forward_fields_map.keys()] + annotated
         fields_with_mapping = [f for f in meta.fields_map.values()]
 
         for parent in meta.parents.keys():
             fields_no_mapping.extend([key for key in find_field_names(parent)[0]])
 
     for field in fields_no_mapping:
         field_names[field] = field
@@ -67,15 +67,19 @@
             lookup_fields, actual_fields = find_field_names(obj[0], **kwargs)
 
     return lookup_fields, actual_fields
 
 
 def find_field_names(obj, **kwargs):
     if hasattr(obj, '_meta'):
-        lookup_fields, actual_fields = find_field_names_from_meta(obj._meta, **kwargs)
+        lookup_fields, actual_fields = find_field_names_from_meta(
+            obj._meta,
+            annotated=getattr(obj, '_annotated_fields', []),
+            **kwargs
+        )
     else:
         lookup_fields, actual_fields = find_field_names_from_obj(obj, **kwargs)
 
     return lookup_fields, actual_fields
 
 
 def validate_field(field_name, model_fields, for_update=False):
@@ -101,14 +105,29 @@
     else:
         return getattr(obj, field_name, default)
 
 
 def get_attribute(obj, attr, default=None):
     result = obj
     comparison = None
+    if isinstance(attr, F):
+        attr = attr.deconstruct()[1][0]
+    elif isinstance(attr, Value):
+        return attr.value, None
+    elif isinstance(attr, Case):
+        for case in attr.cases:
+            if filter_results([obj], case.condition):
+                return get_attribute(obj, case.result)
+        else:
+            return get_attribute(obj, attr.default)
+    elif isinstance(attr, Coalesce):
+        for expr in attr.source_expressions:
+            res, comp = get_attribute(obj, expr)
+            if res is not None:
+                return res, comp
     parts = attr.split('__')
 
     for i, attr_part in enumerate(parts):
         if attr_part in COMPARISONS:
             comparison = attr_part
         elif attr_part in DATETIME_COMPARISONS and type(result) in [date, datetime]:
             comparison_type = parts[i + 1] if i + 1 < len(parts) else COMPARISON_EXACT
@@ -127,16 +146,15 @@
             result = get_field_value(result, field, default)
     return result, comparison
 
 
 def is_match(first, second, comparison=None):
     if isinstance(first, django_mock_queries.query.MockSet):
         return is_match_in_children(comparison, first, second)
-    if (isinstance(first, (int, str)) and
-            isinstance(second, django_mock_queries.query.MockSet)):
+    if (isinstance(first, (int, str)) and isinstance(second, django_mock_queries.query.MockSet)):
         second = convert_to_pks(second)
     if (isinstance(first, date) or isinstance(first, datetime)) \
             and isinstance(comparison, tuple) and len(comparison) == 2:
         first = extract(first, comparison[0])
         comparison = comparison[1]
     if not comparison:
         return first == second
@@ -286,7 +304,31 @@
 
 
 def hash_dict(obj, *fields):
     field_names = fields or find_field_names(obj, concrete_only=True)[1]
     obj_values = {f: get_field_value(obj, f) for f in field_names}
 
     return hash(tuple(sorted((k, v) for k, v in obj_values.items() if not fields or k in fields)))
+
+
+def filter_results(source, query):
+    results = []
+
+    for child in query.children:
+        filtered = _filter_single_q(source, child, query.negated)
+
+        if filtered:
+            if not results or query.connector == CONNECTORS_OR:
+                results = merge(results, filtered)
+            else:
+                results = intersect(results, filtered)
+        elif query.connector == CONNECTORS_AND:
+            return []
+
+    return results
+
+
+def _filter_single_q(source, q_obj, negated):
+    if isinstance(q_obj, DjangoQ):
+        return filter_results(source, q_obj)
+    else:
+        return matches(negated=negated, *source, **{q_obj[0]: q_obj[1]})
```

## Comparing `django_mock_queries-2.1.8.dist-info/LICENSE.txt` & `django_mock_queries-2.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `django_mock_queries-2.1.8.dist-info/METADATA` & `django_mock_queries-2.2.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 Metadata-Version: 2.1
 Name: django-mock-queries
-Version: 2.1.8
+Version: 2.2.0
 Summary: A django library for mocking queryset functions in memory for testing
 Home-page: https://github.com/stphivos/django-mock-queries
 Author: Phivos Stylianides
 Author-email: stphivos@gmail.com
 License: MIT
 Keywords: django orm mocking unit-testing tdd
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Requires-Dist: Django
 Requires-Dist: djangorestframework
-Requires-Dist: model-bakery (~=1.1.0) ; python_version < "3"
-Requires-Dist: mock ; python_version < "3.3"
-Requires-Dist: model-bakery (<1.4.0,>=1.0.0) ; python_version >= "3"
+Requires-Dist: model-bakery (>=1.0.0)
 
 [![Latest Version](https://img.shields.io/pypi/v/django_mock_queries.svg)](https://pypi.python.org/pypi/django_mock_queries)
-[![Build Status](https://travis-ci.org/stphivos/django-mock-queries.svg?branch=master)](https://travis-ci.org/stphivos/django-mock-queries)
+[![Build Status](https://github.com/stphivos/django-mock-queries/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/stphivos/django-mock-queries/actions/workflows/ci.yml)
 [![Code Coverage](https://codecov.io/github/stphivos/django-mock-queries/coverage.svg?branch=master)](https://codecov.io/github/stphivos/django-mock-queries?branch=master)
 [![Code Climate](https://codeclimate.com/github/stphivos/django-mock-queries/badges/gpa.svg)](https://codeclimate.com/github/stphivos/django-mock-queries)
 
 # Django Mock Queries
 
 A library for mocking Django queryset functions in memory for testing
 
@@ -55,95 +47,97 @@
 
 qs = MockSet(
     MockModel(mock_name='john', email='john@gmail.com'),
     MockModel(mock_name='jeff', email='jeff@hotmail.com'),
     MockModel(mock_name='bill', email='bill@gmail.com'),
 )
 
-print [x for x in qs.all().filter(email__icontains='gmail.com').select_related('address')]
+print([x for x in qs.all().filter(email__icontains='gmail.com').select_related('address')])
 # Outputs: [john, bill]
 
 qs = MockSet(
     MockModel(mock_name='model s', msrp=70000),
     MockModel(mock_name='model x', msrp=80000),
     MockModel(mock_name='model 3', msrp=35000),
 )
 
-print qs.all().aggregate(Avg('msrp'))
+print(qs.all().aggregate(Avg('msrp')))
 # Outputs: {'msrp__avg': 61666}
 
 qs = MockSet(
     MockModel(mock_name='model x', make='tesla', country='usa'),
     MockModel(mock_name='s-class', make='mercedes', country='germany'),
     MockModel(mock_name='s90', make='volvo', country='sweden'),
 )
 
-print [x for x in qs.all().filter(Q(make__iexact='tesla') | Q(country__iexact='germany'))]
+print([x for x in qs.all().filter(Q(make__iexact='tesla') | Q(country__iexact='germany'))])
 # Outputs: [model x, s-class]
 
 qs = MockSet(cls=MockModel)
-print qs.create(mock_name='my_object', foo='1', bar='a')
+print(qs.create(mock_name='my_object', foo='1', bar='a'))
 # Outputs: my_object
 
-print [x for x in qs]
+print([x for x in qs])
 # Outputs: [my_object]
 ```
 
 ### Test function that uses Django QuerySet:
 
 ```python
-"""
-Function that queries active users
-"""
-def active_users(self):
-    return User.objects.filter(is_active=True).all()
-
-"""
-Test function applies expected filters by patching Django's user model Manager or Queryset with a MockSet
-"""
-from mock import patch
+from unittest import TestCase
+from unittest.mock import patch
 from django_mock_queries.query import MockSet, MockModel
 
 
 class TestApi(TestCase):
+    """
+    Test function applies expected filters by patching Django's user model Manager or Queryset with a MockSet.
+    """
     users = MockSet()
     user_objects = patch('django.contrib.auth.models.User.objects', users)
 
+    def active_users(self):
+        """
+        Query active users.
+        """
+        return User.objects.filter(is_active=True).all()
+
     @user_objects
     def test_api_active_users_filters_by_is_active_true(self):
         self.users.add(
-        	MockModel(mock_name='active user', is_active=True),
-        	MockModel(mock_name='inactive user', is_active=False)
+            MockModel(mock_name='active user', is_active=True),
+            MockModel(mock_name='inactive user', is_active=False)
         )
 
-        for x in self.api.active_users():
-        	assert x.is_active
+        for user in self.active_users():
+            self.assertTrue(user.is_active)
 ```
 
 ### Test django-rest-framework model serializer:
 
 ```python
-"""
-Car model serializer that includes a nested serializer and a method field
-"""
 class CarSerializer(serializers.ModelSerializer):
+    """
+    Car model serializer that includes a nested serializer and a method field.
+    """
     make = ManufacturerSerializer()
     speed = serializers.SerializerMethodField()
 
     def get_speed(self, obj):
         return obj.format_speed()
 
     class Meta:
         model = Car
         fields = ('id', 'make', 'model', 'speed',)
 
-"""
-Test serializer returns fields with expected values and mock the result of nested serializer for field make
-"""
+
 def test_car_serializer_fields(self):
+    """
+    Test serializer returns fields with expected values and mock the result of nested serializer for field `make`.
+    """
     car = Car(id=1, make=Manufacturer(id=1, name='vw'), model='golf', speed=300)
 
     values = {
         'id': car.id,
         'model': car.model,
         'speed': car.formatted_speed(),
     }
@@ -153,14 +147,15 @@
         .returns('id', 'make', 'model', 'speed') \
         .values(**values) \
         .mocks('make') \
         .run()
 ```
 
 ### Full Example
+
 There is a full Django application in the `examples/users` folder. It shows how
 to configure `django_mock_queries` in your tests and run them with or without
 setting up a Django database. Running the mock tests without a database can be
 much faster when your Django application has a lot of database migrations.
 
 To run your Django tests without a database, add a new settings file, and call
 `monkey_patch_test_db()`. Use a wildcard import to get all the regular settings
@@ -243,16 +238,13 @@
 ```
 * Create pull request
 
 ## TODO
 
 * Add docs as a service like readthedocs with examples for every feature
 * Add support for missing QuerySet methods/Field lookups/Aggregation functions:
-    * Methods that return new QuerySets: annotate, reverse, none, extra, raw
-
-    * Methods that do not return QuerySets: bulk_create, in_bulk, as_manager
-
-    * Field lookups: search
-
-    * Aggregation functions: StdDev, Variance
+    * Methods that return new QuerySets: `annotate`, `reverse`, `none`, `extra`, `raw`
+    * Methods that do not return QuerySets: `bulk_create`, `in_bulk`, `as_manager`
+    * Field lookups: `search`
+    * Aggregation functions: `StdDev`, `Variance`
```

## Comparing `django_mock_queries-2.1.8.dist-info/RECORD` & `django_mock_queries-2.2.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 django_mock_queries/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-django_mock_queries/asserts.py,sha256=tDqhcwiSWV9Dz5RXKT3t7Yf9kPYXM8GbvXuMxhijal0,3153
+django_mock_queries/asserts.py,sha256=7vqLPUmn8hHCHQFs0wmL7-gx4ENIhpWpqrn_2nY1_wQ,3091
 django_mock_queries/comparisons.py,sha256=2xXEvS8F92_ztgN732BIj8GjKSJoLJknnKq1Q83JRuM,1673
 django_mock_queries/constants.py,sha256=ye7K1_nyDwKH47JKZB4mJYm-CiS_E262tBOA2QHvdPk,2378
 django_mock_queries/exceptions.py,sha256=v_2bnDLuwLj4WLmsXo9C01cyNj9l6JwbijmgeMxeMlY,95
-django_mock_queries/mocks.py,sha256=DWK1pl_6KpfIhfMfY_uj6kdrjJS8LbAgNrtozWez3GA,17059
-django_mock_queries/query.py,sha256=j9KcAZ96CSk6L8WYhr0_Ea1KgdjtTSpFPHiOs17-qLc,16646
-django_mock_queries/utils.py,sha256=b6BDD-Xb-eJ1Y5C6x14P1VpD-kq6CcacJh_WWi7grO0,9651
-django_mock_queries-2.1.8.dist-info/LICENSE.txt,sha256=f_84RcT1yYr0aFYLMrPai5ZD1KuJbWey0GaPKo6OMHc,1079
-django_mock_queries-2.1.8.dist-info/METADATA,sha256=E7luKOuJ5Ga0VPIPULQCB3hru2TfYCzrjkuKVoSFdpM,8158
-django_mock_queries-2.1.8.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-django_mock_queries-2.1.8.dist-info/top_level.txt,sha256=8n688Dr34MeMobrw0kdNl_jT2oYQy18i-Y2g1C-RYPs,20
-django_mock_queries-2.1.8.dist-info/RECORD,,
+django_mock_queries/mocks.py,sha256=r7QnruJVZf-pGH9ptxjMXJrq03ZO9WaWF0Su-Fq3Cag,17181
+django_mock_queries/query.py,sha256=4G7ID2H8mEwjoA9m5K5W4PNBbYNLp4RfDHofXZYaa8k,16446
+django_mock_queries/utils.py,sha256=Z1j5W_KzrGCpzaEZHIK3xppj5NTMt3jJBHS0Ng-k7Ew,11078
+django_mock_queries-2.2.0.dist-info/LICENSE.txt,sha256=f_84RcT1yYr0aFYLMrPai5ZD1KuJbWey0GaPKo6OMHc,1079
+django_mock_queries-2.2.0.dist-info/METADATA,sha256=ToS3_lzgN7WojJSefU1NYTU16CSg1uRdrFSNRA6BttI,7925
+django_mock_queries-2.2.0.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+django_mock_queries-2.2.0.dist-info/top_level.txt,sha256=8n688Dr34MeMobrw0kdNl_jT2oYQy18i-Y2g1C-RYPs,20
+django_mock_queries-2.2.0.dist-info/RECORD,,
```

