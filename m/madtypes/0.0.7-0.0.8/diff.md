# Comparing `tmp/madtypes-0.0.7.tar.gz` & `tmp/madtypes-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madtypes-0.0.7.tar", last modified: Thu Jun  1 09:13:06 2023, max compression
+gzip compressed data, was "madtypes-0.0.8.tar", last modified: Sun Jun  4 13:01:44 2023, max compression
```

## Comparing `madtypes-0.0.7.tar` & `madtypes-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:13:06.890889 madtypes-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-06-01 09:13:06.890889 madtypes-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-01 09:12:55.000000 madtypes-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:13:06.886889 madtypes-0.0.7/madtypes/
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-06-01 09:12:55.000000 madtypes-0.0.7/madtypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:13:06.890889 madtypes-0.0.7/madtypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-06-01 09:13:06.000000 madtypes-0.0.7/madtypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-01 09:13:06.000000 madtypes-0.0.7/madtypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:13:06.000000 madtypes-0.0.7/madtypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 09:13:06.000000 madtypes-0.0.7/madtypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:13:06.890889 madtypes-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-01 09:12:55.000000 madtypes-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:13:06.890889 madtypes-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-06-01 09:12:55.000000 madtypes-0.0.7/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:01:44.505500 madtypes-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-04 13:01:44.505500 madtypes-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-04 13:01:33.000000 madtypes-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:01:44.505500 madtypes-0.0.8/madtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-04 13:01:33.000000 madtypes-0.0.8/madtypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:01:44.505500 madtypes-0.0.8/madtypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-04 13:01:44.000000 madtypes-0.0.8/madtypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-04 13:01:44.000000 madtypes-0.0.8/madtypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:01:44.000000 madtypes-0.0.8/madtypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 13:01:44.000000 madtypes-0.0.8/madtypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 13:01:44.505500 madtypes-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-04 13:01:33.000000 madtypes-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:01:44.505500 madtypes-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-04 13:01:33.000000 madtypes-0.0.8/tests/test_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-06-04 13:01:33.000000 madtypes-0.0.8/tests/test_json_schema.py
```

### Comparing `madtypes-0.0.7/madtypes/__init__.py` & `madtypes-0.0.8/madtypes/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-from typing import get_args, get_origin, Union, Type
+import re
 from enum import Enum
+from typing import get_args, get_origin, Union, Type
 import inspect
-import re
 
-TYPE_TO_STRING: dict[type, str] = {
-    str: "string",
-    int: "integer",
-    list: "array",
-    float: "number",
-    tuple: "array",
-}
+
+def DOES_NOTHING(__self__, *__values__, **__keyvalues__):
+    pass
 
 
 def is_optional_type(annotation):
     return getattr(annotation, "__origin__", None) is Union and type(
         None
     ) in getattr(annotation, "__args__", ())
 
@@ -39,137 +35,191 @@
                 # Parametrized list annotation
                 inner_annotation = args[0]
                 return all(
                     type_check(item, inner_annotation) for item in value
                 )
 
 
-class Annotation(type):
-    def __new__(cls, name, bases, attrs):
-        # Retrieve the annotation from the class attributes
-        annotation = attrs.get("annotation")
-        pattern = attrs.get("pattern", None)
-
-        # Override the __new__ method of the list class
-        def new_method(cls, *values, **kwargs):
-            # Check the type of each value before initializing
-            if pattern and (annotation != str and annotation != bytes):
-                raise SyntaxError(
-                    f"pattern attribute can only be applied upon `str` or `bytes`, was `{annotation}`"
-                )
-            for value in values:
-                if not type_check(value, annotation):
-                    raise TypeError(
-                        f"All values must be compatible with the annotation '{annotation}'"
+def generate_annotations_dict(cls):
+    annotations_dict = cls.__annotations__
+
+    for base in cls.__bases__:
+        if hasattr(base, "__annotations__"):
+            for key, value in base.__annotations__.items():
+                if key in annotations_dict and annotations_dict[key] != value:
+                    raise SyntaxError(
+                        f"Conflicting annotations for key '{key}' in base classes"
                     )
+                annotations_dict[key] = value
+
+    return annotations_dict
+
 
-                if pattern and not re.fullmatch(pattern, value):
+def typecheck_dict_initialization(method):
+    """Decorator for dict.__init__"""
+
+    def wrapper(self, *values, **key_values):
+        # todo:
+        # values make no sense in dict except for user defined behavior
+        # in which case type_check should be applied using the method annotation
+
+        _annotations_ = generate_annotations_dict(self.__class__)
+
+        for key, value in key_values.items():
+            if key not in _annotations_:
+                raise TypeError(f"{key} is not part of {self.__class__}")
+            elif not type_check(value, _annotations_[key]):
+                raise TypeError(
+                    f"{value} is not compatible with {_annotations_[key]}"
+                )
+        for key, value in _annotations_.items():
+            if key not in key_values:
+                if not is_optional_type(value):
                     raise TypeError(
-                        f"`{values[0]}` did not match provided pattern `{pattern}`"
+                        f"{key} is mandatory key of {self.__class__}"
                     )
 
-            # Create the instance and initialize it with the values
-            instance = super(cls, cls).__new__(cls, *values, **kwargs)
-            return instance
-
-        # Assign the overridden __new__ method to the class
-        attrs["__new__"] = new_method
-        return super().__new__(cls, name, bases, attrs)
+        if getattr(self, "is_valid", False):
+            self.is_valid(*values, **key_values)
+        if method != DOES_NOTHING:
+            # if user overwrites __init__ it is up to him to super
+            method(self, *values, **key_values)
+        else:
+            super(self.__class__, self).__init__(*values, **key_values)
+
+    return wrapper
 
 
 def subtract_fields(*fields):
     def decorator(cls):
         new_annotations = cls.__annotations__.copy()
         new_cls_dict = dict(cls.__dict__)
 
         for field in fields:
             if field in new_annotations:
                 del new_annotations[field]
-            if field in new_cls_dict:
-                del new_cls_dict[field]  # pragma: no cover (tested by getattr)
 
         new_cls_dict["__annotations__"] = new_annotations
 
         new_cls = type(cls.__name__, cls.__bases__, new_cls_dict)
         return new_cls
 
     return decorator
 
 
-class Schema(dict):
-    @classmethod
-    def get_fields(cls):
-        fields = list(cls.__annotations__.items())
-
-        # Check if the class inherits from another Schema
-        for base in cls.__bases__:
-            if issubclass(base, Schema):
-                # Retrieve the fields from the parent class
-                fields.extend(base.get_fields())
-
-        return fields
-
-    def __init__(self, **kwargs):
-        fields = dict(self.get_fields())
-        for key, value in kwargs.items():
-            if key not in fields:
-                raise TypeError(
-                    f"{key} is not a key for {type(self).__name__}"
-                )
-        for key, value in fields.items():
-            if key in kwargs:
-                if type_check(kwargs[key], value):
-                    super().__setitem__(key, kwargs[key])
-                else:
+def insert_typecheck_for(_type_):
+    def typecheck_primitive_initialization(method):
+        """Decorator for string.__init__"""
+
+        def wrapper(self, *values, **key_values):
+            if method != DOES_NOTHING:
+                method(*values, **key_values)
+            else:
+                if (
+                    (_type_ == str or _type_ == bytes)
+                    and getattr(self, "pattern", False)
+                    and (
+                        not values[0]
+                        or not re.fullmatch(
+                            getattr(self, "pattern"), values[0]
+                        )
+                    )
+                ):
+                    if len(values) != 0:
+                        raise TypeError(
+                            f"{values[0]} did not match {self.pattern}"
+                        )
+
+                annotation = self.annotation if self.annotation else _type_
+                if len(values) == 0:
+                    if is_optional_type(annotation):
+                        _type_.__init__(None)
+                    else:
+                        raise TypeError(
+                            "Value mandatory for annotation {annotation}"
+                        )
+                elif not type_check(values[0], annotation):
                     raise TypeError(
-                        f"{kwargs[key]} is not an instance of {value}"
+                        "Value `{values[0]}` is not compatible with `{annotation}`"
                     )
-            else:
-                optional = is_optional_type(value)
-                if not optional:
-                    raise TypeError(f"{key} is a mandatory field")
-        if not self.is_valid(**kwargs):
-            raise TypeError(f"{kwargs} did not pass object validation")
-
-    def is_valid(self, **__kwargs__) -> bool:
-        """Validation at Object scope, for validation based on multiple fields."""
-        return True
-
-    def __getattr__(self, name):
-        if name in self:
-            return self[name]
-        # I don't know how to trigger the next line, it's more of an `in-case'
-        return super().__getattribute__(name)  # pragma: no cover
-
-    def __setattr__(self, name, value):
-        annotation = self.__annotations__[name]
-
-        if not isinstance(value, annotation):
-            raise TypeError(f"{value} is not an instance of {annotation}")
-        self[name] = value
-
-    @classmethod
-    def required_fields(cls) -> list[str]:
-        return [
-            name
-            for name, field in cls.get_fields()
-            if not is_optional_type(field)
-        ]
-
-
-class Immutable(Schema):
-    def __setattr__(self, __name__, __value__):
-        raise TypeError("'Immutable' object does not support item assignment")
 
-    def __setitem__(self, __key__, __value__):
-        raise TypeError("'Immutable' object does not support item assignment")
+        return wrapper
+
+    return typecheck_primitive_initialization
+
+
+def __getattr__(self, name):
+    if name in self:
+        return self[name]
+    return super(self.__class__).__getattribute__(name)
+
+
+def __setattr__(self, name, value):
+    if not type_check(value, self.__annotations__[name]):
+        raise TypeError(
+            f"value `{value}` does not fit {self.__annotations__[name]} for key {name}"
+        )
+    self[name] = value
+
+
+resolution = {
+    dict: {
+        "__init__": typecheck_dict_initialization,
+    },
+    str: {"__init__": insert_typecheck_for(str)},
+    int: {"__init__": insert_typecheck_for(int)},
+    float: {"__init__": insert_typecheck_for(float)},
+}
+
+
+@classmethod
+def required_fields(cls) -> list[str]:
+    return [
+        name
+        for name, field in cls.get_fields().items()
+        if not is_optional_type(field)
+    ]
+
+
+@classmethod
+def get_fields(cls):
+    return generate_annotations_dict(cls)
+
+
+class MadType(type):
+    def __new__(cls, name, bases, attributes):
+        # type is considered the first of bases
+        # it is not supported to inherit from different types
+        _type_ = bases[0]
+        if _type_ == dict or issubclass(_type_, dict):
+            attributes["__getattr__"] = __getattr__
+            attributes["__setattr__"] = __setattr__
+            attributes["__init__"] = typecheck_dict_initialization(
+                attributes.get("__init__", DOES_NOTHING)
+            )
+            attributes["required_fields"] = required_fields
+            attributes["get_fields"] = get_fields
+        else:
+            attributes["__init__"] = insert_typecheck_for(_type_)(
+                attributes.get("__init__", DOES_NOTHING)
+            )
+        return super().__new__(cls, name, bases, attributes)
+
+
+TYPE_TO_STRING: dict[type, str] = {
+    str: "string",
+    int: "integer",
+    list: "array",
+    float: "number",
+    tuple: "array",
+}
 
 
 def json_schema(
-    annotation: Union[Type["Type"], Type["Annotation"], Type["Schema"]],
+    annotation: Type["Type"],
     **kwargs,
 ) -> dict:
     result = kwargs
     origin = get_origin(annotation)
     origin = annotation if not origin else origin
     args = get_args(annotation)
     if origin in TYPE_TO_STRING:
@@ -188,31 +238,34 @@
             enum_type = TYPE_TO_STRING[type(first_enum_member.value)]
             result.update(
                 {
                     "type": enum_type,
                     "enum": [enu.value for enu in iter(origin)],
                 }
             )
-
-        if issubclass(origin, Schema):
+            return result
+        if getattr(origin, "annotation", False):
+            extra = {
+                key: value
+                for key, value in origin.__dict__.items()
+                if not callable(value) and not key.startswith("__")
+            }
+            return json_schema(origin.annotation, **extra)
+        elif issubclass(origin, dict):
             result.update(
                 {
                     "type": "object",
                     "properties": {
-                        name: json_schema(field)
-                        for name, field in origin.get_fields()
+                        name: json_schema(annotation)
+                        for name, annotation in origin.__annotations__.items()
                     },
                 }
             )
+
             required = origin.required_fields()
             if len(required) > 0:
                 result.update({"required": required})
-        if getattr(origin, "annotation", False):
-            extra = {
-                key: value
-                for key, value in origin.__dict__.items()
-                if not callable(value) and not key.startswith("__")
-            }
-            return json_schema(origin.annotation, **extra)
+
+            return result
     if is_optional_type(annotation):
         return json_schema(remove_optional(annotation))
     return result
```

### Comparing `madtypes-0.0.7/setup.py` & `madtypes-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="madtypes",
-    version="0.0.7",
+    version="0.0.8",
     author="6r17",
     author_email="patrick.borowy@proton.me",
     description="Python typing that raise TypeError at runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/6r17/madtypes",
     packages=find_packages(include=["madtypes"]),
```

