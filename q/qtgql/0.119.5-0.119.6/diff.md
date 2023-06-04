# Comparing `tmp/qtgql-0.119.5.tar.gz` & `tmp/qtgql-0.119.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.119.5.tar", max compression
+gzip compressed data, was "qtgql-0.119.6.tar", max compression
```

## Comparing `qtgql-0.119.5.tar` & `qtgql-0.119.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1064 2023-05-31 11:12:45.006711 qtgql-0.119.5/LICENSE
--rw-r--r--   0        0        0     1805 2023-05-31 11:12:45.006711 qtgql-0.119.5/README.md
--rw-r--r--   0        0        0     4424 2023-05-31 11:13:08.919134 qtgql-0.119.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0        0 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/compiler/__init__.py
--rw-r--r--   0        0        0     1761 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/compiler/builtin_scalars.py
--rw-r--r--   0        0        0    12381 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/compiler/operation.py
--rw-r--r--   0        0        0     3655 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/compiler/template.py
--rw-r--r--   0        0        0     2159 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/config.py
--rw-r--r--   0        0        0      420 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/cppref.py
--rw-r--r--   0        0        0       41 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/exceptions.py
--rw-r--r--   0        0        0     3187 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/graphql_ref.py
--rw-r--r--   0        0        0    17783 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/introspection.py
--rw-r--r--   0        0        0    10604 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/objecttype.py
--rw-r--r--   0        0        0        0 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/runtime/__init__.py
--rw-r--r--   0        0        0     1571 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/runtime/custom_scalars.py
--rw-r--r--   0        0        0      488 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0      536 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/templates/config.jinja.hpp
--rw-r--r--   0        0        0     3047 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/templates/macros.jinja.hpp
--rw-r--r--   0        0        0     4633 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3479 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0     1028 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-04 14:43:06.560257 qtgql-0.119.6/LICENSE
+-rw-r--r--   0        0        0     1805 2023-06-04 14:43:06.560257 qtgql-0.119.6/README.md
+-rw-r--r--   0        0        0     4445 2023-06-04 14:43:25.564415 qtgql-0.119.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/compiler/__init__.py
+-rw-r--r--   0        0        0     1761 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/compiler/builtin_scalars.py
+-rw-r--r--   0        0        0    13091 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/compiler/operation.py
+-rw-r--r--   0        0        0     3733 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/compiler/template.py
+-rw-r--r--   0        0        0     2159 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0      420 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/cppref.py
+-rw-r--r--   0        0        0       41 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/exceptions.py
+-rw-r--r--   0        0        0     3187 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/graphql_ref.py
+-rw-r--r--   0        0        0    17783 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/introspection.py
+-rw-r--r--   0        0        0    11078 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/objecttype.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/runtime/__init__.py
+-rw-r--r--   0        0        0     1571 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/runtime/custom_scalars.py
+-rw-r--r--   0        0        0      488 2023-06-04 14:43:06.576257 qtgql-0.119.6/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0      536 2023-06-04 14:43:06.576257 qtgql-0.119.6/qtgqlcodegen/templates/config.jinja.hpp
+-rw-r--r--   0        0        0     5016 2023-06-04 14:43:06.576257 qtgql-0.119.6/qtgqlcodegen/templates/macros.jinja.hpp
+-rw-r--r--   0        0        0     4857 2023-06-04 14:43:06.576257 qtgql-0.119.6/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     4077 2023-06-04 14:43:06.576257 qtgql-0.119.6/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0     1028 2023-06-04 14:43:06.576257 qtgql-0.119.6/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.6/PKG-INFO
```

### Comparing `qtgql-0.119.5/LICENSE` & `qtgql-0.119.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.5/README.md` & `qtgql-0.119.6/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.5/pyproject.toml` & `qtgql-0.119.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.119.5"
+version = "0.119.6"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
@@ -26,23 +26,24 @@
 
 
 
 [tool.poetry.group.dev.dependencies]
 pytest-cov = "^4.0.0"
 aiohttp = {extras = ["speedups"], version = "^3.8.3"}
 faker = ">=15.3.4,<19.0.0"
-mypy = "^1.0.1"
-strawberry-graphql = ">=0.158.2,<0.180.0"
-aqtinstall = "^3.1.6"
-conan = "^2.0.4"
-cmake = "3.25.0"
-pygithub = "^1.58.2"
-githubrelease = "^1.5.9"
-httpx = "0.18.2"
-autopub = "^0.2.2"
+mypy = ">=1.0.1"
+strawberry-graphql = ">=0.158.2"
+aqtinstall = ">=3.1.6"
+conan = ">=2.0.4"
+cmake = ">=3.25.0"
+pygithub = ">=1.58.2"
+githubrelease = ">=1.5.9"
+httpx = ">=0.18.2"
+autopub = ">=0.2.2"
+mimesis = ">=10.1.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.0.5"
 mike = "^1.1.2"
 markdown-include = "^0.8.0"
 mkdocstrings = {extras = ["python"], version = ">=0.19.1,<0.22.0"}
 pygments = "^2.14.0"
@@ -205,29 +206,29 @@
     "INP",
     "TRY",
     "SIM300",
     "SIM114",
     "DJ008",
 ]
 fix = true
-src = ["qtgql", "tests"]
+src = ["qtgqlcodegen", "tests"]
 [tool.ruff.flake8-annotations]
 suppress-none-returning = true
 
 [tool.ruff.pyupgrade]
 keep-runtime-typing = true
 
 
 [tool.pytest.ini_options]
-addopts = "--cov-config=pyproject.toml --ignore=qtgql/codegen/py/templates/"
+addopts = "--cov-config=pyproject.toml --ignore=qtgqlcodegen/codegen/py/templates/"
 markers = [
     "no_captcha: This test requires that `LOGIN_REQUIRE_CAPTCHA=False` on the server",
 ]
 [tool.coverage.run]
-omit = ['test_*', 'tests/*', 'qtgql/ext/*', '**/*.jinja.py']
+omit = ['test_*', 'tests/*', '**/*.jinja.py']
 relative_files = true
 
 [tool.coverage.report]
 show_missing = true
 exclude_lines = [
   "pragma: no cover",
   "def __repr__",
```

### Comparing `qtgql-0.119.5/qtgqlcodegen/cli.py` & `qtgql-0.119.6/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.5/qtgqlcodegen/compiler/builtin_scalars.py` & `qtgql-0.119.6/qtgqlcodegen/compiler/builtin_scalars.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.5/qtgqlcodegen/compiler/operation.py` & `qtgql-0.119.6/qtgqlcodegen/compiler/operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,52 +57,68 @@
 @attrs.define(frozen=True, slots=False)
 class QtGqlQueriedField:
     definition: QtGqlFieldDefinition
     operation: QtGqlOperationDefinition
     choices: frozendict[str, dict[str, QtGqlQueriedField]] = attrs.Factory(frozendict)
     selections: dict[str, QtGqlQueriedField] = attrs.Factory(dict)
     narrowed_type: Optional[QtGqlQueriedObjectType] = None
+    is_root: bool = False
 
     def __repr__(self):
         return (
             f"{self.definition.name}[{', '.join(self.selections.keys())}\n"
             + "...on".join([f"{k} {repr(v)}" for k, v in self.choices.items()])
             + "]"
         )
 
     @cached_property
     def type(self) -> GqlTypeHinter:
         return self.definition.type
 
     @cached_property
+    def type_name(self) -> str:
+        if self.type.is_object_type:
+            assert self.narrowed_type
+            return self.narrowed_type.name
+
+        if model_of := self.type.is_model:
+            if model_of.is_object_type:
+                assert self.narrowed_type
+                return f"qtgql::bases::ListModelABC<{self.narrowed_type.name}>"
+
+        return self.type.member_type
+
+    @cached_property
     def property_type(self) -> str:
         tp = self.definition.type
         if tp.is_object_type:
             assert self.narrowed_type
-            return self.narrowed_type.name
+            return f"{self.type_name} *"
 
         if cs := tp.is_custom_scalar:
             return cs.type_for_proxy
+
         if model_of := tp.is_model:
             if model_of.is_object_type:
-                assert self.narrowed_type
-                return f"qtgql::bases::ListModelABC<{self.narrowed_type.name}>"
-
-        return tp.member_type
+                return f"{self.type_name} *"
 
-    @property
-    def proxy_of(self) -> GqlTypeHinter:
-        ret = self.definition.type
-        assert ret
-        return ret
+        return self.type_name
 
-    @property
+    @cached_property
     def name(self) -> str:
+        if self.is_root:
+            return "data"
         return self.definition.name
 
+    @cached_property
+    def private_name(self):
+        if self.is_root:
+            return f"m_{self.name}"
+        return self.definition.private_name
+
     @classmethod
     def from_field(
         cls,
         field_definition: QtGqlFieldDefinition,
         selection_set: Optional[gql_lang.SelectionSetNode],
         operation: QtGqlOperationDefinition,
         parent_interface_field: Optional[QtGqlQueriedField] = UNSET,
@@ -111,15 +127,15 @@
         """Main purpose here is to find inner selections of fields, this could
         be an object type, interface, union or a list.
 
         Any other fields should not have inner selections.
         """
         assert parent_interface_field is not UNSET
         if not hasattr(selection_set, "selections"):
-            return cls(definition=field_definition, operation=operation)
+            return cls(definition=field_definition, operation=operation, is_root=is_root)
         assert selection_set
         tp = field_definition.type
         if (
             tp.is_model
         ):  # GraphQL's lists are basically the object beneath them in terms of selections.
             tp = tp.is_model
 
@@ -209,15 +225,15 @@
                         obj_def,
                         operation,
                         parent_interface_field,
                     )
                     selections[__f.name] = __f
             queried_obj = QtGqlQueriedObjectType(
                 definition=obj_def,
-                fields=selections,
+                fields_dict=selections,
             )
             operation.narrowed_types_map[queried_obj.name] = queried_obj
             narrowed_type = queried_obj
 
         def sorted_distinct_fields(
             fields: dict[str, QtGqlQueriedField],
         ) -> dict[str, QtGqlQueriedField]:
@@ -225,46 +241,55 @@
 
         return cls(
             definition=field_definition,
             selections=sorted_distinct_fields(selections),
             choices=frozendict({k: sorted_distinct_fields(v) for k, v in choices.items()}),
             operation=operation,
             narrowed_type=narrowed_type,
+            is_root=is_root,
         )
 
     def as_conf_string(self) -> str:
         return config_template(
             context=ConfigContext(self),
         )
 
 
 @define(slots=False)
 class QtGqlQueriedObjectType:
     definition: QtGqlObjectTypeDefinition = attrs.field(on_setattr=attrs.setters.frozen)
-    fields: dict[str, QtGqlQueriedField] = attrs.Factory(dict)
+    fields_dict: dict[str, QtGqlQueriedField] = attrs.Factory(dict)
     is_root_field: bool = False
 
     @cached_property
+    def fields(self) -> tuple[QtGqlQueriedField, ...]:
+        return tuple(self.fields_dict.values())
+
+    @cached_property
     def name(self) -> str:
-        return f"{self.definition.name}__{'$'.join(sorted(self.fields.keys()))}"
+        return f"{self.definition.name}__{'$'.join(sorted(self.fields_dict.keys()))}"
 
     @cached_property
     def doc_fields(self) -> str:
         return "{} {{\n  {}\n}}".format(
             self.definition.name,
-            "\n   ".join(self.fields.keys()),
+            "\n   ".join(self.fields_dict.keys()),
         )
 
     @cached_property
     def references(self) -> list[QtGqlQueriedField]:
-        return [f for f in self.fields.values() if f.type.is_object_type]
+        return [f for f in self.fields if f.type.is_object_type]
 
     @cached_property
     def models(self) -> list[QtGqlQueriedField]:
-        return [f for f in self.fields.values() if f.type.is_model]
+        return [f for f in self.fields if f.type.is_model]
+
+    @cached_property
+    def private_name(self) -> str:
+        return f"m_{self.name}"
 
 
 @define(slots=False)
 class QtGqlOperationDefinition:
     operation_def: gql_def.OperationDefinitionNode
     evaluator: SchemaEvaluator
     directives: list[str] = attrs.Factory(list)
```

### Comparing `qtgql-0.119.5/qtgqlcodegen/compiler/template.py` & `qtgql-0.119.6/qtgqlcodegen/compiler/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from typing import Any
 from typing import TYPE_CHECKING
 
 from attrs import define
 from jinja2 import Environment
 from jinja2 import PackageLoader
 from jinja2 import select_autoescape
 
@@ -60,14 +61,17 @@
     @property
     def custom_scalars(self) -> list[str]:
         return [scalar.graphql_name for scalar in self.config.custom_scalars.values()]
 
 
 @define(slots=False)
 class OperationTemplateContext:
+    def print(self, v: Any) -> None:
+        print(v)
+
     operation: QtGqlOperationDefinition
     config: QtGqlConfig
     debug: bool = False
 
     @property
     def ns(self) -> str:
         return self.operation.name.lower()
```

### Comparing `qtgql-0.119.5/qtgqlcodegen/config.py` & `qtgql-0.119.6/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.5/qtgqlcodegen/graphql_ref.py` & `qtgql-0.119.6/qtgqlcodegen/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.5/qtgqlcodegen/introspection.py` & `qtgql-0.119.6/qtgqlcodegen/introspection.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.5/qtgqlcodegen/objecttype.py` & `qtgql-0.119.6/qtgqlcodegen/objecttype.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,19 +63,19 @@
 class QtGqlVariableDefinition(Generic[T], QtGqlBaseTypedNode):
     default_value: Optional[T] = UNSET
 
     def json_repr(self, attr_name: Optional[str] = None) -> str:
         if not attr_name:
             attr_name = self.name
         if self.type.is_input_object_type:
-            return f"{attr_name}.to_json()"
+            return f"{attr_name}.value().to_json()"
         elif self.type.is_builtin_scalar:
             return f"{attr_name}.value()"
         elif enum_def := self.type.is_enum:
-            return f"Enums::{enum_def.map_name}[{attr_name}]"
+            return f"Enums::{enum_def.map_name}::name_by_value({attr_name}.value())"
         elif self.is_custom_scalar:
             raise NotImplementedError
 
         raise NotImplementedError(f"{self.type} is not supported as an input type ATM")
 
 
 @define(slots=False)
@@ -309,37 +309,52 @@
     @cached_property
     def is_custom_scalar(self) -> Optional[CustomScalarDefinition]:
         t_self = self.optional_maybe.type
         if t_self in self.scalars.values():
             return t_self
 
     @cached_property
-    def member_type(self) -> str:
-        """
-        :returns: Annotation of the field at the concrete type (for the type of the proxy use property type)
-        """
+    def type_name(self) -> str:
         t_self = self.optional_maybe
-
-        # int, str, float etc...
         if builtin_scalar := t_self.is_builtin_scalar:
             return builtin_scalar.tp
 
         if scalar := t_self.is_custom_scalar:
             return scalar.type_name
+
         if enum_def := t_self.is_enum:
             return enum_def.namespaced_name
-        if model_of := t_self.is_model:
+
+        if t_self.is_model:
             # map of instances based on operation hash.
-            return f"QMap<QUuid, QList<{model_of.member_type}>>"
+            raise NotImplementedError(
+                "models have no valid type for schema concretes, call member_type()",
+            )
+
         if object_def := t_self.is_object_type or t_self.is_interface:
-            return f"std::shared_ptr<{object_def.name}>"
+            return object_def.name
         if q_object_def := t_self.is_queried_object_type:
-            return f"{q_object_def.name}"
+            return q_object_def.name
         if t_self.is_union:
-            return "std::variant<" + ", ".join(th.member_type for th in t_self.of_type) + ">"
+            raise NotImplementedError
         if input_obj := t_self.is_input_object_type:
             return input_obj.name
-
         raise NotImplementedError  # pragma no cover
 
+    @cached_property
+    def member_type(self) -> str:
+        """
+        :returns: Annotation of the field at the concrete type (for the type of the proxy use property type)
+        """
+        t_self = self.optional_maybe
+
+        if model_of := t_self.is_model:
+            # map of instances based on operation hash.
+            return f"QMap<QUuid, QList<{model_of.member_type}>>"
+        if t_self.is_object_type or t_self.is_interface:
+            return f"std::shared_ptr<{self.type_name}>"
+        if q_object_def := t_self.is_queried_object_type:
+            return f"{q_object_def.name}"
+        return self.type_name
+
     def as_annotation(self, object_map=None):  # pragma: no cover
         raise NotImplementedError("not safe to call on this type")
```

### Comparing `qtgql-0.119.5/qtgqlcodegen/runtime/custom_scalars.py` & `qtgql-0.119.6/qtgqlcodegen/runtime/custom_scalars.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.5/qtgqlcodegen/templates/config.jinja.hpp` & `qtgql-0.119.6/qtgqlcodegen/templates/config.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.5/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.119.6/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -10,70 +10,69 @@
 
 {% for t in context.operation.narrowed_types %}
 class 👉 t.name 👈: public QObject{
 /*
 👉 t.doc_fields 👈
  */
     Q_OBJECT
+{% for f in t.fields -%}
+Q_PROPERTY(const 👉 f.property_type 👈 👉 f.name 👈 READ 👉 f.definition.getter_name 👈 NOTIFY 👉 f.definition.signal_name 👈);
+{% endfor %}
+signals:
+{%for f in t.fields -%}
+void 👉 f.definition.signal_name 👈();
+{% endfor %}
+
 {# members #}
 {% if context.debug -%}
 public: // WARNING: members are public because you have debug=True in your config file.
+{% else %}
+protected:
 {% endif %}
 std::shared_ptr<👉context.schema_ns👈::👉 t.definition.name 👈> m_inst;
-{% for ref in t.references -%}
-👉ref.narrowed_type.name👈 *m_👉ref.name👈 = nullptr;
+{% for ref_field in t.references -%}
+👉ref_field.property_type👈 m_👉ref_field.name👈 = {};
 {% endfor %}
 {%- for model_field in t.models -%}
-👉 model_field.property_type 👈 *m_👉model_field.name👈 = nullptr;
+👉 model_field.property_type 👈 m_👉model_field.name👈;
 {% endfor %}
 
 public:
 👉 t.name 👈(QObject* parent, const std::shared_ptr<👉 t.definition.name 👈> &inst ): m_inst{inst}, QObject::QObject(parent){
-{% for ref in t.references -%}
-{% if ref.type.is_optional() %}
-if (m_inst->👉ref.definition.getter_name 👈()){
-m_👉ref.name👈 = new 👉ref.narrowed_type.name👈(this, m_inst->👉ref.definition.getter_name 👈());
-}
-else{
-m_👉ref.name👈 = nullptr;
-}
-{% else %}
-m_👉ref.name👈 = new 👉ref.narrowed_type.name👈(this, m_inst->👉ref.definition.getter_name 👈());
-{% endif %}
+{% for field in t.fields -%}
+👉 macros.initialize_proxy_field(field) 👈
+{# updates logic -#}
+connect(m_inst.get(), &👉context.schema_ns👈::👉t.definition.name👈::👉 field.definition.signal_name 👈, this,
+        [&](){emit 👉 field.definition.signal_name 👈();});
 {% endfor %}
-{%- for model_field in t.models -%}
-auto init_list_👉 model_field.name 👈 =  std::make_unique<QList<👉model_field.narrowed_type.name👈*>>();
-for (const auto & node: m_inst->👉model_field.definition.getter_name 👈().value(OPERATION_ID)){
-    init_list_👉 model_field.name 👈->append(new 👉model_field.narrowed_type.name👈(this, node));
 }
-m_👉model_field.name👈 = new 👉 model_field.property_type 👈(this, std::move(init_list_👉 model_field.name 👈));
-{% endfor -%}
-}
-{%- for f in t.fields.values() %}
+{%- for f in t.fields %}
 {% if f.type.is_object_type or f.type.is_model %}
-[[nodiscard]] inline const 👉 f.property_type 👈 * 👉 f.definition.getter_name 👈() const {
+[[nodiscard]] inline const 👉 f.property_type 👈  👉 f.definition.getter_name 👈() const {
     return m_👉f.name👈;
 {% else %}
+{# TODO: this is probably redundan #}
 [[nodiscard]] inline const 👉 f.property_type 👈 & 👉 f.definition.getter_name 👈() const {
     {% if f.type.is_object_type %}
     return *m_👉f.name👈;
     {% else %}
     return m_inst->👉 f.definition.getter_name 👈();
     {% endif %}
 {% endif %}
 };
 {% endfor -%}
 };
 {% endfor %}
-
 class 👉 context.operation.name 👈: public qtgql::gqlwstransport::OperationHandlerABC {
     Q_OBJECT
-Q_PROPERTY(const 👉 context.operation.root_field.property_type 👈* data READ get_data NOTIFY dataChanged);
+Q_PROPERTY(const 👉 context.operation.root_field.property_type 👈 data READ get_data NOTIFY dataChanged);
+
+std::optional<👉 context.operation.root_field.property_type 👈> m_data = {};
+
 
-👉 context.operation.root_field.property_type 👈 *m_data = nullptr;
 
 inline const QString &ENV_NAME() override{
     static const auto ret = QString("👉 context.config.env_name 👈");
     return ret;
     }
 
 inline const qtgql::bases::OperationMetadata & OPERATION_METADATA() override{
@@ -92,30 +91,42 @@
 return OPERATION_ID;
 }
 
 
 void on_next(const QJsonObject &message) override{
     if (!m_data && message.contains("data")){
         auto data = message.value("data").toObject();
-        if (data.contains("👉 context.operation.root_field.name 👈")){
-            m_data = new 👉 context.operation.root_field.property_type 👈(this,
-👉context.schema_ns👈::👉 context.operation.root_field.definition.type.is_object_type.name 👈::from_json(
-        data.value("👉 context.operation.root_field.name 👈").toObject(), OPERATION_METADATA().selections, OPERATION_METADATA())
-);
+        if (data.contains("👉 context.operation.root_field.definition.name 👈")){
+{%- set do_after_deserialized -%} 👉 macros.initialize_proxy_field(context.operation.root_field) 👈 {% endset -%}
+            👉 macros.deserialize_field(context.operation.root_field.definition,
+                                    "auto concrete", False,
+                                    "OPERATION_METADATA().selections",
+                                    "OPERATION_METADATA()",
+                                    do_after_deserialized,
+                                    ) 👈
+        // initialize proxy
+
         }
     }
 }
-inline const 👉 context.operation.root_field.property_type 👈* get_data(){
-    return m_data;
+inline const 👉 context.operation.root_field.property_type 👈 get_data(){
+    return m_data.value();
+}
+inline void loose(){
+    {% if context.operation.root_field.type.is_object_type %}
+    👉 context.operation.root_field.type.is_object_type.name 👈::INST_STORE().get_node(m_data.value()->get_id()).value()->loose(OPERATION_METADATA());
+    {% else %}
+    throw "not implemented";
+    {% endif %}
 }
 
 {% if context.operation.variables %}
-void setVariables(
+void set_variables(
 {% for var in context.operation.variables -%}
-const std::optional<👉 var.type.member_type 👈>  👉 var.name 👈 {% if not loop.last %},{% endif %}
+const std::optional<👉 var.type.type_name 👈> & 👉 var.name 👈 {% if not loop.last %},{% endif %}
 {% endfor -%}){
 {% for var in context.operation.variables %}
 if (👉 var.name 👈.has_value()){
     m_variables.insert("👉 var.name 👈",  👉 var.json_repr() 👈);
 }
 {% endfor %}
 }
```

### Comparing `qtgql-0.119.5/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.119.6/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -40,82 +40,104 @@
 {% endif %}
 
 // ---------- Object Types ----------
 {% for type in context.types %}
 {%- set base_class -%}{% if type.has_id_field %}ObjectTypeABCWithID{% else %}ObjectTypeABC{% endif %}{%- endset -%}
 class 👉 type.name 👈 : public qtgql::bases::👉 base_class 👈{
 Q_OBJECT
+
 protected:
+👉 macros.concrete_type_fields(type) 👈
+public:
 static auto & INST_STORE() {
     static qtgql::bases::ObjectStore<👉 type.name 👈> _store;
     return _store;
 }
-
-👉 macros.concrete_type_fields(type) 👈
-public:
 inline static const QString TYPE_NAME = "👉 type.name 👈";
-
+static auto get_node(const QString & id){
+    return INST_STORE().get_node(id);
+}
 explicit 👉 type.name 👈 (QObject* parent = nullptr)
 : qtgql::bases::👉 base_class 👈::👉 base_class 👈(parent) {};
 
 
 static std::shared_ptr<👉 type.name 👈> from_json(const QJsonObject& data,
                                  const qtgql::bases::SelectionsConfig &config,
                                  const qtgql::bases::OperationMetadata& metadata){
 if (data.isEmpty()){
     return {};
 }
+{% if type.has_id_field %}
+if (config.selections.contains("id") && !data.value("id").isNull()) {
+    auto cached_maybe = get_node(data.value("id").toString());
+    if(cached_maybe.has_value()){
+        auto node = cached_maybe.value();
+        node->update(data, config);
+        return node;
+    }
+};
+{% endif %}
+
 auto inst = std::make_shared<👉 type.name 👈>();
 {% for f in type.fields -%}
 {% set assign_to %} inst->👉 f.private_name 👈 {% endset %}
 👉macros.deserialize_field(f, assign_to)👈
 {% endfor %}
 {% if type.id_is_optional %}
 if (inst->id) {
-  auto record = qtgql::bases::NodeRecord(node = inst, retainers = set())
-                    .retain(metadata.operation_name)
-                        cls.INST_STORE.add_record(record)
+INST_STORE().add_node(inst, metadata.operation_id);
 }
 {% elif type.has_id_field and not type.id_is_optional %}
-auto record = std::make_shared<qtgql::bases::NodeRecord<👉 type.name 👈>>(inst);
-record->retain(metadata.operation_id);
-INST_STORE().add_record(record);
+INST_STORE().add_node(inst, metadata.operation_id);
 {% endif %}
 return inst;
 };
 
-void loose(const qtgql::bases::OperationMetadata &metadata){throw "not implemented";};
+void loose(const qtgql::bases::OperationMetadata &metadata){
+    {% if type.has_id_field %}
+    INST_STORE().loose(m_id, metadata.operation_id);
+    {% else %}
+    throw "not implemented";
+    {% endif %}
+};
 void update(const QJsonObject &data,
-            const qtgql::bases::SelectionsConfig &selections){throw "not implemented";};
+            const qtgql::bases::SelectionsConfig &config){
+            {%for f in type.fields -%}
+            {% set fset %}👉f.setter_name👈{% endset %}{% set private_name %}👉f.private_name👈{% endset -%}
+            👉 macros.update_concrete_field(f, fset_name=fset, private_name=private_name) 👈
+            {% endfor %}
+};
 
 };
 {% endfor %}
 
-// ----------------------------------------- INPUT OBJECTS -----------------------------------------
+// ---------- INPUT OBJECTS ----------
 
 {% for type in context.input_objects %}
 /*
  * 👉 type.docstring 👈
  */
-
 struct 👉type.name👈: QObject{
+Q_OBJECT
+
+public:
 {% for f in type.fields %}
-👉f.annotation👈 m_👉f.name👈;
+std::optional<👉f.member_type👈> 👉f.name👈 = {};
 {% endfor -%}
-
-👉type.name👈(QObject* parent, {% for f in type.fields %} 👉f.name👈: 👉f.annotation👈 {% endfor %}): QObject::QObject(parent){
-    {% for f in type.fields %}
-    m_👉f.name👈 = 👉f.name👈;
-    {% endfor -%}
-};
-QJsonObject to_json(){
-    ret = {}
-    {% for f in type.fields %}{% set attr_name %}self.👉f.name👈{% endset %}
-    if 👉attr_name👈:
-    ret['👉f.name👈'] = 👉f.json_repr(attr_name)👈
+👉type.name👈(QObject* parent, {% for f in type.fields %} std::optional<👉f.member_type👈> &👉f.name👈{% if not loop.last %},{% endif %} {% endfor %}): QObject::QObject(parent){
+    {% for f in type.fields -%}
+    👉f.name👈 = 👉f.name👈;
     {% endfor %}
-    return ret
 };
+QJsonObject to_json() const{
+    auto ret = QJsonObject();
+    {% for f in type.fields %}{% set attr_name %}👉f.name👈{% endset %}
+    if (👉attr_name👈.has_value()){
+    ret.insert("👉f.name👈", 👉f.json_repr(attr_name)👈);
+    }
+    {% endfor %}
+    return ret;
 }
+};
 {% endfor %}
 
 }
```

### Comparing `qtgql-0.119.5/qtgqlcodegen/utils.py` & `qtgql-0.119.6/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.5/PKG-INFO` & `qtgql-0.119.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.119.5
+Version: 0.119.6
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

