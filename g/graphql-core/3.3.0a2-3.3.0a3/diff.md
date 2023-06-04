# Comparing `tmp/graphql_core-3.3.0a2.tar.gz` & `tmp/graphql_core-3.3.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_core-3.3.0a2.tar", max compression
+gzip compressed data, was "graphql_core-3.3.0a3.tar", max compression
```

## Comparing `graphql_core-3.3.0a2.tar` & `graphql_core-3.3.0a3.tar`

### file list

```diff
@@ -1,323 +1,337 @@
--rw-r--r--   0        0        0      544 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/.bumpversion.cfg
--rw-r--r--   0        0        0      292 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/.editorconfig
--rw-r--r--   0        0        0      218 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/.flake8
--rw-r--r--   0        0        0      341 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/.readthedocs.yaml
--rw-r--r--   0        0        0        7 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/CODEOWNERS
--rw-r--r--   0        0        0     1180 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/LICENSE
--rw-r--r--   0        0        0     9845 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/README.md
--rw-r--r--   0        0        0      728 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/SECURITY.md
--rw-r--r--   0        0        0      634 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/Makefile
--rw-r--r--   0        0        0    15100 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/conf.py
--rw-r--r--   0        0        0     5754 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/diffs.rst
--rw-r--r--   0        0        0      248 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/index.rst
--rw-r--r--   0        0        0     3254 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/intro.rst
--rw-r--r--   0        0        0      760 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/make.bat
--rw-r--r--   0        0        0      304 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/modules/error.rst
--rw-r--r--   0        0        0      657 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/modules/execution.rst
--rw-r--r--   0        0        0      397 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/modules/graphql.rst
--rw-r--r--   0        0        0     4305 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/modules/language.rst
--rw-r--r--   0        0        0      832 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/modules/pyutils.rst
--rw-r--r--   0        0        0     4374 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/modules/type.rst
--rw-r--r--   0        0        0     2421 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/modules/utilities.rst
--rw-r--r--   0        0        0     3255 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/modules/validation.rst
--rw-r--r--   0        0        0       40 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/requirements.txt
--rw-r--r--   0        0        0     1430 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/usage/extension.rst
--rw-r--r--   0        0        0      278 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/usage/index.rst
--rw-r--r--   0        0        0     2382 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/usage/introspection.rst
--rw-r--r--   0        0        0     2082 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/usage/methods.rst
--rw-r--r--   0        0        0     1258 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/usage/other.rst
--rw-r--r--   0        0        0     2706 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/usage/parser.rst
--rw-r--r--   0        0        0     3920 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/usage/queries.rst
--rw-r--r--   0        0        0     3899 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/usage/resolvers.rst
--rw-r--r--   0        0        0     7586 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/usage/schema.rst
--rw-r--r--   0        0        0     2632 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/usage/sdl.rst
--rw-r--r--   0        0        0     1719 2022-11-03 21:34:59.940112 graphql_core-3.3.0a2/docs/usage/validator.rst
--rw-r--r--   0        0        0    72150 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/poetry.lock
--rw-r--r--   0        0        0     4263 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/pyproject.toml
--rw-r--r--   0        0        0    20433 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/__init__.py
--rw-r--r--   0        0        0      432 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/error/__init__.py
--rw-r--r--   0        0        0     8790 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/error/graphql_error.py
--rw-r--r--   0        0        0     1859 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/error/located_error.py
--rw-r--r--   0        0        0      571 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/error/syntax_error.py
--rw-r--r--   0        0        0      959 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/execution/__init__.py
--rw-r--r--   0        0        0     5681 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/execution/collect_fields.py
--rw-r--r--   0        0        0    45456 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/execution/execute.py
--rw-r--r--   0        0        0     3769 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/execution/map_async_iterator.py
--rw-r--r--   0        0        0     2599 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/execution/middleware.py
--rw-r--r--   0        0        0     8128 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/execution/subscribe.py
--rw-r--r--   0        0        0     8741 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/execution/values.py
--rw-r--r--   0        0        0     6950 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/graphql.py
--rw-r--r--   0        0        0     4790 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/__init__.py
--rw-r--r--   0        0        0    20944 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/ast.py
--rw-r--r--   0        0        0     4949 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/block_string.py
--rw-r--r--   0        0        0      871 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/character_classes.py
--rw-r--r--   0        0        0      831 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/directive_locations.py
--rw-r--r--   0        0        0    19380 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/lexer.py
--rw-r--r--   0        0        0     1252 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/location.py
--rw-r--r--   0        0        0    43277 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/parser.py
--rw-r--r--   0        0        0     2927 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/predicates.py
--rw-r--r--   0        0        0     2714 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/print_location.py
--rw-r--r--   0        0        0     1738 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/print_string.py
--rw-r--r--   0        0        0    13290 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/printer.py
--rw-r--r--   0        0        0     2552 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/source.py
--rw-r--r--   0        0        0      542 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/token_kind.py
--rw-r--r--   0        0        0    13043 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/language/visitor.py
--rw-r--r--   0        0        0       66 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/py.typed
--rw-r--r--   0        0        0     1746 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/__init__.py
--rw-r--r--   0        0        0      272 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/awaitable_or_value.py
--rw-r--r--   0        0        0     1048 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/cached_property.py
--rw-r--r--   0        0        0      716 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/convert_case.py
--rw-r--r--   0        0        0     1960 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/description.py
--rw-r--r--   0        0        0      612 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/did_you_mean.py
--rw-r--r--   0        0        0      765 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/format_list.py
--rw-r--r--   0        0        0      129 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/frozen_error.py
--rw-r--r--   0        0        0      472 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/group_by.py
--rw-r--r--   0        0        0      279 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/identity_func.py
--rw-r--r--   0        0        0     5794 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/inspect.py
--rw-r--r--   0        0        0      968 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/is_awaitable.py
--rw-r--r--   0        0        0     1164 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/is_iterable.py
--rw-r--r--   0        0        0      251 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/merge_kwargs.py
--rw-r--r--   0        0        0      478 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/natural_compare.py
--rw-r--r--   0        0        0      975 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/path.py
--rw-r--r--   0        0        0      234 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/print_path_list.py
--rw-r--r--   0        0        0     2464 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/simple_pub_sub.py
--rw-r--r--   0        0        0     3571 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/suggestion_list.py
--rw-r--r--   0        0        0     1276 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/pyutils/undefined.py
--rw-r--r--   0        0        0     7150 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/type/__init__.py
--rw-r--r--   0        0        0     1053 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/type/assert_name.py
--rw-r--r--   0        0        0    65924 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/type/definition.py
--rw-r--r--   0        0        0     8681 2022-11-03 21:34:59.944112 graphql_core-3.3.0a2/src/graphql/type/directives.py
--rw-r--r--   0        0        0    22693 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/type/introspection.py
--rw-r--r--   0        0        0    10843 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/type/scalars.py
--rw-r--r--   0        0        0    20229 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/type/schema.py
--rw-r--r--   0        0        0    24144 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/type/validate.py
--rw-r--r--   0        0        0     3424 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/__init__.py
--rw-r--r--   0        0        0     4548 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/ast_from_value.py
--rw-r--r--   0        0        0     1596 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/ast_to_dict.py
--rw-r--r--   0        0        0     3616 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/build_ast_schema.py
--rw-r--r--   0        0        0    17051 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/build_client_schema.py
--rw-r--r--   0        0        0     5471 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/coerce_input_value.py
--rw-r--r--   0        0        0      571 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/concat_ast.py
--rw-r--r--   0        0        0    28978 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/extend_schema.py
--rw-r--r--   0        0        0    20733 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/find_breaking_changes.py
--rw-r--r--   0        0        0     7946 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/get_introspection_query.py
--rw-r--r--   0        0        0     1088 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/get_operation_ast.py
--rw-r--r--   0        0        0     1596 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/introspection_from_schema.py
--rw-r--r--   0        0        0     6351 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/lexicographic_sort_schema.py
--rw-r--r--   0        0        0     8797 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/print_schema.py
--rw-r--r--   0        0        0     3539 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/separate_operations.py
--rw-r--r--   0        0        0     1142 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/sort_value_node.py
--rw-r--r--   0        0        0     2933 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/strip_ignored_characters.py
--rw-r--r--   0        0        0     4054 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/type_comparators.py
--rw-r--r--   0        0        0     2003 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/type_from_ast.py
--rw-r--r--   0        0        0    10119 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/type_info.py
--rw-r--r--   0        0        0     5555 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/value_from_ast.py
--rw-r--r--   0        0        0     3116 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/utilities/value_from_ast_untyped.py
--rw-r--r--   0        0        0     5579 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/__init__.py
--rw-r--r--   0        0        0     1080 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/__init__.py
--rw-r--r--   0        0        0       46 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/custom/__init__.py
--rw-r--r--   0        0        0     4319 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/custom/no_deprecated.py
--rw-r--r--   0        0        0     1140 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/custom/no_schema_introspection.py
--rw-r--r--   0        0        0     1529 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/executable_definitions.py
--rw-r--r--   0        0        0     4636 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/fields_on_correct_type.py
--rw-r--r--   0        0        0     1850 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/fragments_on_composite_types.py
--rw-r--r--   0        0        0     3590 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/known_argument_names.py
--rw-r--r--   0        0        0     4458 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/known_directives.py
--rw-r--r--   0        0        0      795 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/known_fragment_names.py
--rw-r--r--   0        0        0     2956 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/known_type_names.py
--rw-r--r--   0        0        0     1237 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/lone_anonymous_operation.py
--rw-r--r--   0        0        0     1289 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/lone_schema_definition.py
--rw-r--r--   0        0        0     3114 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/no_fragment_cycles.py
--rw-r--r--   0        0        0     1736 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/no_undefined_variables.py
--rw-r--r--   0        0        0     1768 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/no_unused_fragments.py
--rw-r--r--   0        0        0     1804 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/no_unused_variables.py
--rw-r--r--   0        0        0    28442 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/overlapping_fields_can_be_merged.py
--rw-r--r--   0        0        0     2312 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/possible_fragment_spreads.py
--rw-r--r--   0        0        0     3696 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/possible_type_extensions.py
--rw-r--r--   0        0        0     4463 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/provided_required_arguments.py
--rw-r--r--   0        0        0     1434 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/scalar_leafs.py
--rw-r--r--   0        0        0     3205 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/single_field_subscriptions.py
--rw-r--r--   0        0        0     2873 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/unique_argument_definition_names.py
--rw-r--r--   0        0        0     1250 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/unique_argument_names.py
--rw-r--r--   0        0        0     1571 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/unique_directive_names.py
--rw-r--r--   0        0        0     3116 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/unique_directives_per_location.py
--rw-r--r--   0        0        0     2135 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/unique_enum_value_names.py
--rw-r--r--   0        0        0     2575 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/unique_field_definition_names.py
--rw-r--r--   0        0        0     1332 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/unique_fragment_names.py
--rw-r--r--   0        0        0     1424 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/unique_input_field_names.py
--rw-r--r--   0        0        0     1473 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/unique_operation_names.py
--rw-r--r--   0        0        0     2376 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/unique_operation_types.py
--rw-r--r--   0        0        0     1724 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/unique_type_names.py
--rw-r--r--   0        0        0     1090 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/unique_variable_names.py
--rw-r--r--   0        0        0     5677 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/values_of_correct_type.py
--rw-r--r--   0        0        0     1189 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/variables_are_input_types.py
--rw-r--r--   0        0        0     3630 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/rules/variables_in_allowed_position.py
--rw-r--r--   0        0        0     5679 2022-11-03 21:34:59.948112 graphql_core-3.3.0a2/src/graphql/validation/specified_rules.py
--rw-r--r--   0        0        0     4934 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/src/graphql/validation/validate.py
--rw-r--r--   0        0        0     8712 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/src/graphql/validation/validation_context.py
--rw-r--r--   0        0        0     1354 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/src/graphql/version.py
--rw-r--r--   0        0        0       24 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/__init__.py
--rw-r--r--   0        0        0      310 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/benchmarks/__init__.py
--rw-r--r--   0        0        0      376 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/benchmarks/test_build_ast_schema.py
--rw-r--r--   0        0        0      437 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/benchmarks/test_build_client_schema.py
--rw-r--r--   0        0        0     1190 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/benchmarks/test_execution_async.py
--rw-r--r--   0        0        0      860 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/benchmarks/test_execution_sync.py
--rw-r--r--   0        0        0      428 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/benchmarks/test_graphql_schema.py
--rw-r--r--   0        0        0      463 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/benchmarks/test_introspection_from_schema.py
--rw-r--r--   0        0        0      273 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/benchmarks/test_parser.py
--rw-r--r--   0        0        0      425 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/benchmarks/test_validate_gql.py
--rw-r--r--   0        0        0     1094 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/benchmarks/test_validate_invalid_gql.py
--rw-r--r--   0        0        0      321 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/benchmarks/test_validate_sdl.py
--rw-r--r--   0        0        0      744 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/benchmarks/test_visit.py
--rw-r--r--   0        0        0      622 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/conftest.py
--rw-r--r--   0        0        0       30 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/error/__init__.py
--rw-r--r--   0        0        0    13303 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/error/test_graphql_error.py
--rw-r--r--   0        0        0     1237 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/error/test_located_error.py
--rw-r--r--   0        0        0     2829 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/error/test_print_location.py
--rw-r--r--   0        0        0       34 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/__init__.py
--rw-r--r--   0        0        0    17446 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_abstract.py
--rw-r--r--   0        0        0     3930 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_customize.py
--rw-r--r--   0        0        0     7024 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_directives.py
--rw-r--r--   0        0        0     4559 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_execution_result.py
--rw-r--r--   0        0        0    33285 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_executor.py
--rw-r--r--   0        0        0     8183 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_lists.py
--rw-r--r--   0        0        0    14249 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_map_async_iterator.py
--rw-r--r--   0        0        0    11448 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_middleware.py
--rw-r--r--   0        0        0     6122 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_mutations.py
--rw-r--r--   0        0        0    22628 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_nonnull.py
--rw-r--r--   0        0        0     4273 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_parallel.py
--rw-r--r--   0        0        0     7888 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_resolve.py
--rw-r--r--   0        0        0     5990 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_schema.py
--rw-r--r--   0        0        0    25927 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_subscribe.py
--rw-r--r--   0        0        0     7073 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_sync.py
--rw-r--r--   0        0        0    14919 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_union_interface.py
--rw-r--r--   0        0        0    34877 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/execution/test_variables.py
--rw-r--r--   0        0        0      871 2022-11-03 21:34:59.952112 graphql_core-3.3.0a2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0   345926 2022-11-03 21:34:59.956112 graphql_core-3.3.0a2/tests/fixtures/github_schema.graphql
--rw-r--r--   0        0        0  1826295 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/fixtures/github_schema.json
--rw-r--r--   0        0        0      994 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/fixtures/kitchen_sink.graphql
--rw-r--r--   0        0        0     2876 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/fixtures/schema_kitchen_sink.graphql
--rw-r--r--   0        0        0       33 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/__init__.py
--rw-r--r--   0        0        0     8899 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_ast.py
--rw-r--r--   0        0        0     7040 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_block_string.py
--rw-r--r--   0        0        0     1815 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_block_string_fuzz.py
--rw-r--r--   0        0        0     2414 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_character_classes.py
--rw-r--r--   0        0        0    25037 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_lexer.py
--rw-r--r--   0        0        0     1707 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_location.py
--rw-r--r--   0        0        0    20266 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_parser.py
--rw-r--r--   0        0        0     5113 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_predicates.py
--rw-r--r--   0        0        0     2437 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_print_string.py
--rw-r--r--   0        0        0     6413 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_printer.py
--rw-r--r--   0        0        0    30299 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_schema_parser.py
--rw-r--r--   0        0        0     5208 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_schema_printer.py
--rw-r--r--   0        0        0     3594 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_source.py
--rw-r--r--   0        0        0    62240 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/language/test_visitor.py
--rw-r--r--   0        0        0       32 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/__init__.py
--rw-r--r--   0        0        0      697 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_cached_property.py
--rw-r--r--   0        0        0     2019 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_convert_case.py
--rw-r--r--   0        0        0    10738 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_description.py
--rw-r--r--   0        0        0      769 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_did_you_mean.py
--rw-r--r--   0        0        0     1040 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_format_list.py
--rw-r--r--   0        0        0      159 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_frozen_error.py
--rw-r--r--   0        0        0     1424 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_group_by.py
--rw-r--r--   0        0        0      635 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_identity_func.py
--rw-r--r--   0        0        0    12244 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_inspect.py
--rw-r--r--   0        0        0     3460 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_is_awaitable.py
--rw-r--r--   0        0        0     7744 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_is_iterable.py
--rw-r--r--   0        0        0      606 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_merge_kwargs.py
--rw-r--r--   0        0        0      860 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_natural_compare.py
--rw-r--r--   0        0        0      790 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_path.py
--rw-r--r--   0        0        0      426 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_print_path_list.py
--rw-r--r--   0        0        0     2976 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_simple_pub_sub.py
--rw-r--r--   0        0        0     2222 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_suggestion_list.py
--rw-r--r--   0        0        0     1263 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/pyutils/test_undefined.py
--rw-r--r--   0        0        0     3835 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/star_wars_data.py
--rw-r--r--   0        0        0     7871 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/star_wars_schema.py
--rw-r--r--   0        0        0    13482 2022-11-03 21:34:59.960112 graphql_core-3.3.0a2/tests/test_docs.py
--rw-r--r--   0        0        0    11566 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/test_star_wars_introspection.py
--rw-r--r--   0        0        0    13972 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/test_star_wars_query.py
--rw-r--r--   0        0        0     3121 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/test_star_wars_validation.py
--rw-r--r--   0        0        0    17879 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/test_user_registry.py
--rw-r--r--   0        0        0     4162 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/test_version.py
--rw-r--r--   0        0        0       29 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/type/__init__.py
--rw-r--r--   0        0        0     2776 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/type/test_assert_name.py
--rw-r--r--   0        0        0     5788 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/type/test_custom_scalars.py
--rw-r--r--   0        0        0    80489 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/type/test_definition.py
--rw-r--r--   0        0        0     9075 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/type/test_directives.py
--rw-r--r--   0        0        0    10707 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/type/test_enum.py
--rw-r--r--   0        0        0    13424 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/type/test_extensions.py
--rw-r--r--   0        0        0    61708 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/type/test_introspection.py
--rw-r--r--   0        0        0    21326 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/type/test_predicate.py
--rw-r--r--   0        0        0    28854 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/type/test_scalars.py
--rw-r--r--   0        0        0    19573 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/type/test_schema.py
--rw-r--r--   0        0        0    82963 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/type/test_validation.py
--rw-r--r--   0        0        0       34 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/__init__.py
--rw-r--r--   0        0        0     9413 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_ast_from_value.py
--rw-r--r--   0        0        0    26810 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_ast_to_dict.py
--rw-r--r--   0        0        0    36605 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_build_ast_schema.py
--rw-r--r--   0        0        0    35279 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_build_client_schema.py
--rw-r--r--   0        0        0    13789 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_coerce_input_value.py
--rw-r--r--   0        0        0      769 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_concat_ast.py
--rw-r--r--   0        0        0    44232 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_extend_schema.py
--rw-r--r--   0        0        0    37071 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_find_breaking_changes.py
--rw-r--r--   0        0        0     3340 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_get_introspection_query.py
--rw-r--r--   0        0        0     1989 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_get_operation_ast.py
--rw-r--r--   0        0        0     6616 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_introspection_from_schema.py
--rw-r--r--   0        0        0     7825 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_lexicographic_sort_schema.py
--rw-r--r--   0        0        0    26814 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_print_schema.py
--rw-r--r--   0        0        0     4839 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_separate_operations.py
--rw-r--r--   0        0        0     1320 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_sort_value_node.py
--rw-r--r--   0        0        0     8140 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_strip_ignored_characters.py
--rw-r--r--   0        0        0     9198 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_strip_ignored_characters_fuzz.py
--rw-r--r--   0        0        0     3962 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_type_comparators.py
--rw-r--r--   0        0        0     1371 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_type_from_ast.py
--rw-r--r--   0        0        0    20156 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_type_info.py
--rw-r--r--   0        0        0    10359 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_value_from_ast.py
--rw-r--r--   0        0        0     2788 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utilities/test_value_from_ast_untyped.py
--rw-r--r--   0        0        0      308 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utils/__init__.py
--rw-r--r--   0        0        0      207 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utils/dedent.py
--rw-r--r--   0        0        0      378 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utils/gen_fuzz_strings.py
--rw-r--r--   0        0        0     2268 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utils/test_dedent.py
--rw-r--r--   0        0        0     1570 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/utils/test_gen_fuzz_strings.py
--rw-r--r--   0        0        0      133 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/__init__.py
--rw-r--r--   0        0        0     3509 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/harness.py
--rw-r--r--   0        0        0     2235 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/test_executable_definitions.py
--rw-r--r--   0        0        0    12731 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/test_fields_on_correct_type.py
--rw-r--r--   0        0        0     3392 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/test_fragments_on_composite_types.py
--rw-r--r--   0        0        0     9805 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/test_known_argument_names.py
--rw-r--r--   0        0        0    14060 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/test_known_directives.py
--rw-r--r--   0        0        0     1845 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/test_known_fragment_names.py
--rw-r--r--   0        0        0    10758 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/test_known_type_names.py
--rw-r--r--   0        0        0     2603 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/test_lone_anonymous_operation.py
--rw-r--r--   0        0        0     3469 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/test_lone_schema_definition.py
--rw-r--r--   0        0        0     8895 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/test_no_deprecated.py
--rw-r--r--   0        0        0     7659 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/test_no_fragment_cycles.py
--rw-r--r--   0        0        0     3951 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/test_no_schema_introspection.py
--rw-r--r--   0        0        0    10185 2022-11-03 21:34:59.964112 graphql_core-3.3.0a2/tests/validation/test_no_undefined_variables.py
--rw-r--r--   0        0        0     4070 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_no_unused_fragments.py
--rw-r--r--   0        0        0     6265 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_no_unused_variables.py
--rw-r--r--   0        0        0    34545 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_overlapping_fields_can_be_merged.py
--rw-r--r--   0        0        0    10022 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_possible_fragment_spreads.py
--rw-r--r--   0        0        0     8735 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_possible_type_extensions.py
--rw-r--r--   0        0        0    10622 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_provided_required_arguments.py
--rw-r--r--   0        0        0     4161 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_scalar_leafs.py
--rw-r--r--   0        0        0     8228 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_single_field_subscriptions.py
--rw-r--r--   0        0        0     4194 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_unique_argument_definition_names.py
--rw-r--r--   0        0        0     3560 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_unique_argument_names.py
--rw-r--r--   0        0        0     2733 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_unique_directive_names.py
--rw-r--r--   0        0        0    10909 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_unique_directives_per_location.py
--rw-r--r--   0        0        0     4672 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_unique_enum_value_names.py
--rw-r--r--   0        0        0    11248 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_unique_field_definition_names.py
--rw-r--r--   0        0        0     2541 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_unique_fragment_names.py
--rw-r--r--   0        0        0     2610 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_unique_input_field_names.py
--rw-r--r--   0        0        0     2862 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_unique_operation_names.py
--rw-r--r--   0        0        0     9880 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_unique_operation_types.py
--rw-r--r--   0        0        0     4350 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_unique_type_names.py
--rw-r--r--   0        0        0     1334 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_unique_variable_names.py
--rw-r--r--   0        0        0     6307 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_validation.py
--rw-r--r--   0        0        0    36134 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_values_of_correct_type.py
--rw-r--r--   0        0        0     1514 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_variables_are_input_types.py
--rw-r--r--   0        0        0    10191 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tests/validation/test_variables_in_allowed_position.py
--rw-r--r--   0        0        0     1365 2022-11-03 21:34:59.968112 graphql_core-3.3.0a2/tox.ini
--rw-r--r--   0        0        0    11547 1970-01-01 00:00:00.000000 graphql_core-3.3.0a2/setup.py
--rw-r--r--   0        0        0    11266 1970-01-01 00:00:00.000000 graphql_core-3.3.0a2/PKG-INFO
+-rw-r--r--   0        0        0      544 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/.bumpversion.cfg
+-rw-r--r--   0        0        0      292 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/.editorconfig
+-rw-r--r--   0        0        0      218 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/.flake8
+-rw-r--r--   0        0        0      341 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/.readthedocs.yaml
+-rw-r--r--   0        0        0        7 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/CODEOWNERS
+-rw-r--r--   0        0        0     1180 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/LICENSE
+-rw-r--r--   0        0        0     9889 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/README.md
+-rw-r--r--   0        0        0      728 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/SECURITY.md
+-rw-r--r--   0        0        0      634 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/docs/Makefile
+-rw-r--r--   0        0        0    15407 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/docs/conf.py
+-rw-r--r--   0        0        0     5754 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/docs/diffs.rst
+-rw-r--r--   0        0        0      248 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/docs/index.rst
+-rw-r--r--   0        0        0     3254 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/docs/intro.rst
+-rw-r--r--   0        0        0      760 2023-06-04 19:57:31.180083 graphql_core-3.3.0a3/docs/make.bat
+-rw-r--r--   0        0        0      304 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/modules/error.rst
+-rw-r--r--   0        0        0     1397 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/modules/execution.rst
+-rw-r--r--   0        0        0      397 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/modules/graphql.rst
+-rw-r--r--   0        0        0     4457 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/modules/language.rst
+-rw-r--r--   0        0        0      832 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/modules/pyutils.rst
+-rw-r--r--   0        0        0     4492 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/modules/type.rst
+-rw-r--r--   0        0        0     2421 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/modules/utilities.rst
+-rw-r--r--   0        0        0     3255 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/modules/validation.rst
+-rw-r--r--   0        0        0       40 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/requirements.txt
+-rw-r--r--   0        0        0     1430 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/usage/extension.rst
+-rw-r--r--   0        0        0      278 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/usage/index.rst
+-rw-r--r--   0        0        0     2382 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/usage/introspection.rst
+-rw-r--r--   0        0        0     2082 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/usage/methods.rst
+-rw-r--r--   0        0        0     1258 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/usage/other.rst
+-rw-r--r--   0        0        0     2706 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/usage/parser.rst
+-rw-r--r--   0        0        0     3920 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/usage/queries.rst
+-rw-r--r--   0        0        0     3899 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/usage/resolvers.rst
+-rw-r--r--   0        0        0     7586 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/usage/schema.rst
+-rw-r--r--   0        0        0     2632 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/usage/sdl.rst
+-rw-r--r--   0        0        0     1719 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/docs/usage/validator.rst
+-rw-r--r--   0        0        0   100343 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/poetry.lock
+-rw-r--r--   0        0        0     4644 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/pyproject.toml
+-rw-r--r--   0        0        0    21762 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/__init__.py
+-rw-r--r--   0        0        0      432 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/error/__init__.py
+-rw-r--r--   0        0        0     8790 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/error/graphql_error.py
+-rw-r--r--   0        0        0     1859 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/error/located_error.py
+-rw-r--r--   0        0        0      571 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/error/syntax_error.py
+-rw-r--r--   0        0        0     2050 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/execution/__init__.py
+-rw-r--r--   0        0        0     2328 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/execution/async_iterables.py
+-rw-r--r--   0        0        0     8459 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/execution/collect_fields.py
+-rw-r--r--   0        0        0   103011 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/execution/execute.py
+-rw-r--r--   0        0        0     2599 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/execution/middleware.py
+-rw-r--r--   0        0        0     8741 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/execution/values.py
+-rw-r--r--   0        0        0     7078 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/graphql.py
+-rw-r--r--   0        0        0     5094 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/language/__init__.py
+-rw-r--r--   0        0        0    22384 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/language/ast.py
+-rw-r--r--   0        0        0     4949 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/language/block_string.py
+-rw-r--r--   0        0        0      871 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/language/character_classes.py
+-rw-r--r--   0        0        0      831 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/language/directive_locations.py
+-rw-r--r--   0        0        0    19447 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/language/lexer.py
+-rw-r--r--   0        0        0     1252 2023-06-04 19:57:31.184083 graphql_core-3.3.0a3/src/graphql/language/location.py
+-rw-r--r--   0        0        0    47129 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/language/parser.py
+-rw-r--r--   0        0        0     3216 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/language/predicates.py
+-rw-r--r--   0        0        0     2714 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/language/print_location.py
+-rw-r--r--   0        0        0     1738 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/language/print_string.py
+-rw-r--r--   0        0        0    14088 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/language/printer.py
+-rw-r--r--   0        0        0     2552 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/language/source.py
+-rw-r--r--   0        0        0      566 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/language/token_kind.py
+-rw-r--r--   0        0        0    13043 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/language/visitor.py
+-rw-r--r--   0        0        0       66 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/py.typed
+-rw-r--r--   0        0        0     1805 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/__init__.py
+-rw-r--r--   0        0        0     1428 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/async_reduce.py
+-rw-r--r--   0        0        0      272 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/awaitable_or_value.py
+-rw-r--r--   0        0        0     1048 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/cached_property.py
+-rw-r--r--   0        0        0      716 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/convert_case.py
+-rw-r--r--   0        0        0     1960 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/description.py
+-rw-r--r--   0        0        0      612 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/did_you_mean.py
+-rw-r--r--   0        0        0      765 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/format_list.py
+-rw-r--r--   0        0        0      129 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/frozen_error.py
+-rw-r--r--   0        0        0      472 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/group_by.py
+-rw-r--r--   0        0        0      279 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/identity_func.py
+-rw-r--r--   0        0        0     5794 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/inspect.py
+-rw-r--r--   0        0        0      972 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/is_awaitable.py
+-rw-r--r--   0        0        0     1164 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/is_iterable.py
+-rw-r--r--   0        0        0      251 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/merge_kwargs.py
+-rw-r--r--   0        0        0      478 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/natural_compare.py
+-rw-r--r--   0        0        0      975 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/path.py
+-rw-r--r--   0        0        0      234 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/print_path_list.py
+-rw-r--r--   0        0        0     2485 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/simple_pub_sub.py
+-rw-r--r--   0        0        0     3571 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/suggestion_list.py
+-rw-r--r--   0        0        0     1281 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/pyutils/undefined.py
+-rw-r--r--   0        0        0     7326 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/type/__init__.py
+-rw-r--r--   0        0        0     1053 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/type/assert_name.py
+-rw-r--r--   0        0        0    53077 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/type/definition.py
+-rw-r--r--   0        0        0     8834 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/type/directives.py
+-rw-r--r--   0        0        0    22693 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/type/introspection.py
+-rw-r--r--   0        0        0    10843 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/type/scalars.py
+-rw-r--r--   0        0        0    17941 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/type/schema.py
+-rw-r--r--   0        0        0    24140 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/type/validate.py
+-rw-r--r--   0        0        0     3424 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/__init__.py
+-rw-r--r--   0        0        0     4548 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/ast_from_value.py
+-rw-r--r--   0        0        0     1596 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/ast_to_dict.py
+-rw-r--r--   0        0        0     3504 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/build_ast_schema.py
+-rw-r--r--   0        0        0    17219 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/build_client_schema.py
+-rw-r--r--   0        0        0     5498 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/coerce_input_value.py
+-rw-r--r--   0        0        0      571 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/concat_ast.py
+-rw-r--r--   0        0        0    29899 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/extend_schema.py
+-rw-r--r--   0        0        0    20730 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/find_breaking_changes.py
+-rw-r--r--   0        0        0     7946 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/get_introspection_query.py
+-rw-r--r--   0        0        0     1088 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/get_operation_ast.py
+-rw-r--r--   0        0        0     1596 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/introspection_from_schema.py
+-rw-r--r--   0        0        0     6351 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/lexicographic_sort_schema.py
+-rw-r--r--   0        0        0     8797 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/print_schema.py
+-rw-r--r--   0        0        0     3539 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/separate_operations.py
+-rw-r--r--   0        0        0     1142 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/sort_value_node.py
+-rw-r--r--   0        0        0     2933 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/strip_ignored_characters.py
+-rw-r--r--   0        0        0     4054 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/type_comparators.py
+-rw-r--r--   0        0        0     2003 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/type_from_ast.py
+-rw-r--r--   0        0        0    10119 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/type_info.py
+-rw-r--r--   0        0        0     5555 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/value_from_ast.py
+-rw-r--r--   0        0        0     3116 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/utilities/value_from_ast_untyped.py
+-rw-r--r--   0        0        0     6125 2023-06-04 19:57:31.188083 graphql_core-3.3.0a3/src/graphql/validation/__init__.py
+-rw-r--r--   0        0        0     1080 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/__init__.py
+-rw-r--r--   0        0        0       46 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/custom/__init__.py
+-rw-r--r--   0        0        0     4319 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/custom/no_deprecated.py
+-rw-r--r--   0        0        0     1140 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/custom/no_schema_introspection.py
+-rw-r--r--   0        0        0     1930 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/defer_stream_directive_label.py
+-rw-r--r--   0        0        0     2456 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/defer_stream_directive_on_root_field.py
+-rw-r--r--   0        0        0     1529 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/executable_definitions.py
+-rw-r--r--   0        0        0     4636 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/fields_on_correct_type.py
+-rw-r--r--   0        0        0     1850 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/fragments_on_composite_types.py
+-rw-r--r--   0        0        0     3590 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/known_argument_names.py
+-rw-r--r--   0        0        0     4458 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/known_directives.py
+-rw-r--r--   0        0        0      795 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/known_fragment_names.py
+-rw-r--r--   0        0        0     2956 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/known_type_names.py
+-rw-r--r--   0        0        0     1237 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/lone_anonymous_operation.py
+-rw-r--r--   0        0        0     1289 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/lone_schema_definition.py
+-rw-r--r--   0        0        0     3114 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/no_fragment_cycles.py
+-rw-r--r--   0        0        0     1736 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/no_undefined_variables.py
+-rw-r--r--   0        0        0     1768 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/no_unused_fragments.py
+-rw-r--r--   0        0        0     1804 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/no_unused_variables.py
+-rw-r--r--   0        0        0    29499 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/overlapping_fields_can_be_merged.py
+-rw-r--r--   0        0        0     2312 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/possible_fragment_spreads.py
+-rw-r--r--   0        0        0     3696 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/possible_type_extensions.py
+-rw-r--r--   0        0        0     4462 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/provided_required_arguments.py
+-rw-r--r--   0        0        0     1434 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/scalar_leafs.py
+-rw-r--r--   0        0        0     3182 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/single_field_subscriptions.py
+-rw-r--r--   0        0        0     1793 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/stream_directive_on_list_field.py
+-rw-r--r--   0        0        0     2873 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/unique_argument_definition_names.py
+-rw-r--r--   0        0        0     1250 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/unique_argument_names.py
+-rw-r--r--   0        0        0     1571 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/unique_directive_names.py
+-rw-r--r--   0        0        0     3116 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/unique_directives_per_location.py
+-rw-r--r--   0        0        0     2135 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/unique_enum_value_names.py
+-rw-r--r--   0        0        0     2575 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/unique_field_definition_names.py
+-rw-r--r--   0        0        0     1332 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/unique_fragment_names.py
+-rw-r--r--   0        0        0     1424 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/unique_input_field_names.py
+-rw-r--r--   0        0        0     1473 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/unique_operation_names.py
+-rw-r--r--   0        0        0     2376 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/unique_operation_types.py
+-rw-r--r--   0        0        0     1724 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/unique_type_names.py
+-rw-r--r--   0        0        0     1090 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/unique_variable_names.py
+-rw-r--r--   0        0        0     5677 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/values_of_correct_type.py
+-rw-r--r--   0        0        0     1189 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/variables_are_input_types.py
+-rw-r--r--   0        0        0     3630 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/rules/variables_in_allowed_position.py
+-rw-r--r--   0        0        0     6219 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/specified_rules.py
+-rw-r--r--   0        0        0     4225 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/validate.py
+-rw-r--r--   0        0        0     8712 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/validation/validation_context.py
+-rw-r--r--   0        0        0     1354 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/src/graphql/version.py
+-rw-r--r--   0        0        0       24 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/__init__.py
+-rw-r--r--   0        0        0      310 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/benchmarks/__init__.py
+-rw-r--r--   0        0        0     1040 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/benchmarks/test_async_iterable.py
+-rw-r--r--   0        0        0      376 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/benchmarks/test_build_ast_schema.py
+-rw-r--r--   0        0        0      437 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/benchmarks/test_build_client_schema.py
+-rw-r--r--   0        0        0     1190 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/benchmarks/test_execution_async.py
+-rw-r--r--   0        0        0      860 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/benchmarks/test_execution_sync.py
+-rw-r--r--   0        0        0      428 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/benchmarks/test_graphql_schema.py
+-rw-r--r--   0        0        0      463 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/benchmarks/test_introspection_from_schema.py
+-rw-r--r--   0        0        0      358 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/benchmarks/test_parser.py
+-rw-r--r--   0        0        0      425 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/benchmarks/test_validate_gql.py
+-rw-r--r--   0        0        0     1094 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/benchmarks/test_validate_invalid_gql.py
+-rw-r--r--   0        0        0      321 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/benchmarks/test_validate_sdl.py
+-rw-r--r--   0        0        0      744 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/benchmarks/test_visit.py
+-rw-r--r--   0        0        0      622 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/conftest.py
+-rw-r--r--   0        0        0       30 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/error/__init__.py
+-rw-r--r--   0        0        0    13303 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/error/test_graphql_error.py
+-rw-r--r--   0        0        0     1237 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/error/test_located_error.py
+-rw-r--r--   0        0        0     2829 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/error/test_print_location.py
+-rw-r--r--   0        0        0       34 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/execution/__init__.py
+-rw-r--r--   0        0        0    17452 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/execution/test_abstract.py
+-rw-r--r--   0        0        0     4013 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/execution/test_customize.py
+-rw-r--r--   0        0        0    28846 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/execution/test_defer.py
+-rw-r--r--   0        0        0     7024 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/execution/test_directives.py
+-rw-r--r--   0        0        0     4558 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/execution/test_execution_result.py
+-rw-r--r--   0        0        0    31603 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/execution/test_executor.py
+-rw-r--r--   0        0        0     6251 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/execution/test_flatten_async_iterable.py
+-rw-r--r--   0        0        0    13557 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/execution/test_lists.py
+-rw-r--r--   0        0        0     9197 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/execution/test_map_async_iterable.py
+-rw-r--r--   0        0        0    11445 2023-06-04 19:57:31.192083 graphql_core-3.3.0a3/tests/execution/test_middleware.py
+-rw-r--r--   0        0        0    10141 2023-06-04 19:57:31.196083 graphql_core-3.3.0a3/tests/execution/test_mutations.py
+-rw-r--r--   0        0        0    22626 2023-06-04 19:57:31.196083 graphql_core-3.3.0a3/tests/execution/test_nonnull.py
+-rw-r--r--   0        0        0     5503 2023-06-04 19:57:31.196083 graphql_core-3.3.0a3/tests/execution/test_parallel.py
+-rw-r--r--   0        0        0     7888 2023-06-04 19:57:31.196083 graphql_core-3.3.0a3/tests/execution/test_resolve.py
+-rw-r--r--   0        0        0     5989 2023-06-04 19:57:31.196083 graphql_core-3.3.0a3/tests/execution/test_schema.py
+-rw-r--r--   0        0        0    56960 2023-06-04 19:57:31.196083 graphql_core-3.3.0a3/tests/execution/test_stream.py
+-rw-r--r--   0        0        0    38581 2023-06-04 19:57:31.196083 graphql_core-3.3.0a3/tests/execution/test_subscribe.py
+-rw-r--r--   0        0        0     8529 2023-06-04 19:57:31.196083 graphql_core-3.3.0a3/tests/execution/test_sync.py
+-rw-r--r--   0        0        0    14916 2023-06-04 19:57:31.196083 graphql_core-3.3.0a3/tests/execution/test_union_interface.py
+-rw-r--r--   0        0        0    34877 2023-06-04 19:57:31.196083 graphql_core-3.3.0a3/tests/execution/test_variables.py
+-rw-r--r--   0        0        0     1114 2023-06-04 19:57:31.196083 graphql_core-3.3.0a3/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0   345926 2023-06-04 19:57:31.200083 graphql_core-3.3.0a3/tests/fixtures/github_schema.graphql
+-rw-r--r--   0        0        0  1826295 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/fixtures/github_schema.json
+-rw-r--r--   0        0        0     1466 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/fixtures/kitchen_sink.graphql
+-rw-r--r--   0        0        0     2876 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/fixtures/schema_kitchen_sink.graphql
+-rw-r--r--   0        0        0       33 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/__init__.py
+-rw-r--r--   0        0        0     9897 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_ast.py
+-rw-r--r--   0        0        0     7040 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_block_string.py
+-rw-r--r--   0        0        0     1782 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_block_string_fuzz.py
+-rw-r--r--   0        0        0     2414 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_character_classes.py
+-rw-r--r--   0        0        0    25166 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_lexer.py
+-rw-r--r--   0        0        0     1707 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_location.py
+-rw-r--r--   0        0        0    31230 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_parser.py
+-rw-r--r--   0        0        0     5409 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_predicates.py
+-rw-r--r--   0        0        0     2437 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_print_string.py
+-rw-r--r--   0        0        0     7206 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_printer.py
+-rw-r--r--   0        0        0    30299 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_schema_parser.py
+-rw-r--r--   0        0        0     5208 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_schema_printer.py
+-rw-r--r--   0        0        0     3594 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_source.py
+-rw-r--r--   0        0        0    72552 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/language/test_visitor.py
+-rw-r--r--   0        0        0       32 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/__init__.py
+-rw-r--r--   0        0        0     2042 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_async_reduce.py
+-rw-r--r--   0        0        0      697 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_cached_property.py
+-rw-r--r--   0        0        0     2019 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_convert_case.py
+-rw-r--r--   0        0        0     8935 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_description.py
+-rw-r--r--   0        0        0      769 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_did_you_mean.py
+-rw-r--r--   0        0        0     1040 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_format_list.py
+-rw-r--r--   0        0        0      159 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_frozen_error.py
+-rw-r--r--   0        0        0     1424 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_group_by.py
+-rw-r--r--   0        0        0      635 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_identity_func.py
+-rw-r--r--   0        0        0    12244 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_inspect.py
+-rw-r--r--   0        0        0     3579 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_is_awaitable.py
+-rw-r--r--   0        0        0     7744 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_is_iterable.py
+-rw-r--r--   0        0        0      606 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_merge_kwargs.py
+-rw-r--r--   0        0        0      860 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_natural_compare.py
+-rw-r--r--   0        0        0      790 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_path.py
+-rw-r--r--   0        0        0      426 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_print_path_list.py
+-rw-r--r--   0        0        0     2960 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_simple_pub_sub.py
+-rw-r--r--   0        0        0     2222 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_suggestion_list.py
+-rw-r--r--   0        0        0     1628 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/pyutils/test_undefined.py
+-rw-r--r--   0        0        0     3835 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/star_wars_data.py
+-rw-r--r--   0        0        0     7871 2023-06-04 19:57:31.204084 graphql_core-3.3.0a3/tests/star_wars_schema.py
+-rw-r--r--   0        0        0    13482 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/test_docs.py
+-rw-r--r--   0        0        0    11566 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/test_star_wars_introspection.py
+-rw-r--r--   0        0        0    13972 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/test_star_wars_query.py
+-rw-r--r--   0        0        0     3121 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/test_star_wars_validation.py
+-rw-r--r--   0        0        0    17760 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/test_user_registry.py
+-rw-r--r--   0        0        0     4162 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/test_version.py
+-rw-r--r--   0        0        0       29 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/type/__init__.py
+-rw-r--r--   0        0        0     2524 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/type/test_assert_name.py
+-rw-r--r--   0        0        0     5788 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/type/test_custom_scalars.py
+-rw-r--r--   0        0        0    52328 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/type/test_definition.py
+-rw-r--r--   0        0        0     6956 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/type/test_directives.py
+-rw-r--r--   0        0        0    10707 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/type/test_enum.py
+-rw-r--r--   0        0        0    10095 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/type/test_extensions.py
+-rw-r--r--   0        0        0    61708 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/type/test_introspection.py
+-rw-r--r--   0        0        0    22321 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/type/test_predicate.py
+-rw-r--r--   0        0        0    28854 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/type/test_scalars.py
+-rw-r--r--   0        0        0    16843 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/type/test_schema.py
+-rw-r--r--   0        0        0    73423 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/type/test_validation.py
+-rw-r--r--   0        0        0       34 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/__init__.py
+-rw-r--r--   0        0        0     9413 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_ast_from_value.py
+-rw-r--r--   0        0        0    27485 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_ast_to_dict.py
+-rw-r--r--   0        0        0    36040 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_build_ast_schema.py
+-rw-r--r--   0        0        0    35279 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_build_client_schema.py
+-rw-r--r--   0        0        0    13789 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_coerce_input_value.py
+-rw-r--r--   0        0        0      769 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_concat_ast.py
+-rw-r--r--   0        0        0    43753 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_extend_schema.py
+-rw-r--r--   0        0        0    37071 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_find_breaking_changes.py
+-rw-r--r--   0        0        0     3340 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_get_introspection_query.py
+-rw-r--r--   0        0        0     1989 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_get_operation_ast.py
+-rw-r--r--   0        0        0     6548 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_introspection_from_schema.py
+-rw-r--r--   0        0        0     7825 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_lexicographic_sort_schema.py
+-rw-r--r--   0        0        0    26814 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_print_schema.py
+-rw-r--r--   0        0        0     4839 2023-06-04 19:57:31.208084 graphql_core-3.3.0a3/tests/utilities/test_separate_operations.py
+-rw-r--r--   0        0        0     1320 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utilities/test_sort_value_node.py
+-rw-r--r--   0        0        0     8332 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utilities/test_strip_ignored_characters.py
+-rw-r--r--   0        0        0     9165 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utilities/test_strip_ignored_characters_fuzz.py
+-rw-r--r--   0        0        0     3962 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utilities/test_type_comparators.py
+-rw-r--r--   0        0        0     1371 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utilities/test_type_from_ast.py
+-rw-r--r--   0        0        0    20156 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utilities/test_type_info.py
+-rw-r--r--   0        0        0    10359 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utilities/test_value_from_ast.py
+-rw-r--r--   0        0        0     2788 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utilities/test_value_from_ast_untyped.py
+-rw-r--r--   0        0        0      361 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utils/__init__.py
+-rw-r--r--   0        0        0      840 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utils/assert_equal_awaitables_or_values.py
+-rw-r--r--   0        0        0      327 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utils/assert_matching_values.py
+-rw-r--r--   0        0        0      207 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utils/dedent.py
+-rw-r--r--   0        0        0      378 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utils/gen_fuzz_strings.py
+-rw-r--r--   0        0        0     1631 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utils/test_assert_equal_awaitables_or_values.py
+-rw-r--r--   0        0        0      424 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utils/test_assert_matching_values.py
+-rw-r--r--   0        0        0     2268 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utils/test_dedent.py
+-rw-r--r--   0        0        0     1570 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/utils/test_gen_fuzz_strings.py
+-rw-r--r--   0        0        0      133 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/__init__.py
+-rw-r--r--   0        0        0     3510 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/harness.py
+-rw-r--r--   0        0        0     4825 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_defer_stream_directive_label.py
+-rw-r--r--   0        0        0     6925 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_defer_stream_directive_on_root_field.py
+-rw-r--r--   0        0        0     2235 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_executable_definitions.py
+-rw-r--r--   0        0        0    12731 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_fields_on_correct_type.py
+-rw-r--r--   0        0        0     3392 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_fragments_on_composite_types.py
+-rw-r--r--   0        0        0     9805 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_known_argument_names.py
+-rw-r--r--   0        0        0    14060 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_known_directives.py
+-rw-r--r--   0        0        0     1845 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_known_fragment_names.py
+-rw-r--r--   0        0        0    10758 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_known_type_names.py
+-rw-r--r--   0        0        0     2603 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_lone_anonymous_operation.py
+-rw-r--r--   0        0        0     3469 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_lone_schema_definition.py
+-rw-r--r--   0        0        0     8895 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_no_deprecated.py
+-rw-r--r--   0        0        0     7659 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_no_fragment_cycles.py
+-rw-r--r--   0        0        0     3951 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_no_schema_introspection.py
+-rw-r--r--   0        0        0    10185 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_no_undefined_variables.py
+-rw-r--r--   0        0        0     4070 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_no_unused_fragments.py
+-rw-r--r--   0        0        0     6265 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_no_unused_variables.py
+-rw-r--r--   0        0        0    38196 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_overlapping_fields_can_be_merged.py
+-rw-r--r--   0        0        0    10022 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_possible_fragment_spreads.py
+-rw-r--r--   0        0        0     8735 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_possible_type_extensions.py
+-rw-r--r--   0        0        0    10622 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_provided_required_arguments.py
+-rw-r--r--   0        0        0     4161 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_scalar_leafs.py
+-rw-r--r--   0        0        0     8228 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_single_field_subscriptions.py
+-rw-r--r--   0        0        0     2120 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_stream_directive_on_list_field.py
+-rw-r--r--   0        0        0     4194 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_unique_argument_definition_names.py
+-rw-r--r--   0        0        0     3560 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_unique_argument_names.py
+-rw-r--r--   0        0        0     2733 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_unique_directive_names.py
+-rw-r--r--   0        0        0    10909 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_unique_directives_per_location.py
+-rw-r--r--   0        0        0     4672 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_unique_enum_value_names.py
+-rw-r--r--   0        0        0    11248 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_unique_field_definition_names.py
+-rw-r--r--   0        0        0     2541 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_unique_fragment_names.py
+-rw-r--r--   0        0        0     2610 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_unique_input_field_names.py
+-rw-r--r--   0        0        0     2862 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_unique_operation_names.py
+-rw-r--r--   0        0        0     9880 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_unique_operation_types.py
+-rw-r--r--   0        0        0     4350 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_unique_type_names.py
+-rw-r--r--   0        0        0     1334 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_unique_variable_names.py
+-rw-r--r--   0        0        0     4962 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_validation.py
+-rw-r--r--   0        0        0    36134 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_values_of_correct_type.py
+-rw-r--r--   0        0        0     1514 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_variables_are_input_types.py
+-rw-r--r--   0        0        0    10191 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tests/validation/test_variables_in_allowed_position.py
+-rw-r--r--   0        0        0     1431 2023-06-04 19:57:31.212084 graphql_core-3.3.0a3/tox.ini
+-rw-r--r--   0        0        0    11011 1970-01-01 00:00:00.000000 graphql_core-3.3.0a3/PKG-INFO
```

### Comparing `graphql_core-3.3.0a2/.bumpversion.cfg` & `graphql_core-3.3.0a3/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 3.3.0a2
+current_version = 3.3.0a3
 commit = False
 tag = False
 
 [bumpversion:file:src/graphql/version.py]
 search = version = "{current_version}"
 replace = version = "{new_version}"
```

### Comparing `graphql_core-3.3.0a2/LICENSE` & `graphql_core-3.3.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/README.md` & `graphql_core-3.3.0a3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,28 @@
 ![Lint Status](https://github.com/graphql-python/graphql-core/actions/workflows/lint.yml/badge.svg)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 An extensive test suite with over 2300 unit tests and 100% coverage comprises a
 replication of the complete test suite of GraphQL.js, making sure this port is
 reliable and compatible with GraphQL.js.
 
-The current stable version 3.2.3 of GraphQL-core is up-to-date with GraphQL.js version 16.6.0.
+The current stable version 3.2.3 of GraphQL-core is up-to-date with GraphQL.js
+version 16.6.0 and supports Python version 3.6 and newer.
 
-You can also try out the latest alpha version 3.3.0a2 of GraphQL-core that is up-to-date with GraphQL.js version 17.0.0a1.
-Please note that this new minor version of GraphQL-core does not support Python 3.7 anymore.
-
-Note that for various reasons, GraphQL-core does not use SemVer like GraphQL.js. Changes in the major version of GraphQL.js are reflected in the minor version of GraphQL-core instead. This means there can be breaking changes in the API when the minor version changes, and only patch releases are fully backward compatible. Therefore, we recommend something like `=~ 3.2.0` as version specifier when including GraphQL-core as a dependency.
+You can also try out the latest alpha version 3.3.0a3 of GraphQL-core
+which is up-to-date with GraphQL.js version 17.0.0a2.
+Please note that this new minor version of GraphQL-core does not support
+Python 3.6 anymore.
+
+Note that for various reasons, GraphQL-core does not use SemVer like GraphQL.js.
+Changes in the major version of GraphQL.js are reflected in the minor version of
+GraphQL-core instead. This means there can be breaking changes in the API
+when the minor version changes, and only patch releases are fully backward compatible.
+Therefore, we recommend something like `=~ 3.2.0` as version specifier
+when including GraphQL-core as a dependency.
 
 
 ## Documentation
 
 A more detailed documentation for GraphQL-core 3 can be found at
 [graphql-core-3.readthedocs.io](https://graphql-core-3.readthedocs.io/).
 
@@ -125,17 +133,17 @@
 
 ```python
 ExecutionResult(data=None, errors=[GraphQLError(
     "Cannot query field 'BoyHowdy' on type 'RootQueryType'.",
     locations=[SourceLocation(line=1, column=3)])])
 ```
 
-The `graphql_sync` function assumes that all resolvers return values synchronously. By
-using coroutines as resolvers, you can also create results in an asynchronous fashion
-with the `graphql` function.
+The `graphql_sync` function assumes that all resolvers return values synchronously.
+By  using coroutines as resolvers, you can also create results in an asynchronous
+fashion with the `graphql` function.
 
 ```python
 import asyncio
 from graphql import (
     graphql, GraphQLSchema, GraphQLObjectType, GraphQLField, GraphQLString)
```

### Comparing `graphql_core-3.3.0a2/SECURITY.md` & `graphql_core-3.3.0a3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/Makefile` & `graphql_core-3.3.0a3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/conf.py` & `graphql_core-3.3.0a3/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,25 +47,25 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'GraphQL-core 3'
-copyright = '2022, Christoph Zwerschke'
+copyright = '2023, Christoph Zwerschke'
 author = 'Christoph Zwerschke'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 # version = '3.3'
 # The full version, including alpha/beta/rc tags.
-version = release = '3.3.0a2'
+version = release = '3.3.0a3'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = 'en'
@@ -134,26 +134,33 @@
 # ignore the following undocumented or internal references:
 ignore_references = set('''
 GNT GT KT T VT
 enum.Enum
 traceback
 types.TracebackType
 TypeMap
+AsyncPayloadRecord
 AwaitableOrValue
 EnterLeaveVisitor
+ExperimentalIncrementalExecutionResults
 FormattedSourceLocation
 GraphQLAbstractType
 GraphQLErrorExtensions
 GraphQLFieldResolver
 GraphQLTypeResolver
 GraphQLOutputType
 Middleware
 asyncio.events.AbstractEventLoop
-graphql.execution.map_async_iterator.MapAsyncIterator
+graphql.execution.collect_fields.FieldsAndPatches
+graphql.execution.map_async_iterable.map_async_iterable
 graphql.execution.Middleware
+graphql.execution.execute.DeferredFragmentRecord
+graphql.execution.execute.ExperimentalIncrementalExecutionResults
+graphql.execution.execute.StreamArguments
+graphql.execution.execute.StreamRecord
 graphql.language.lexer.EscapeSequence
 graphql.language.visitor.EnterLeaveVisitor
 graphql.type.schema.InterfaceImplementations
 graphql.validation.validation_context.VariableUsage
 graphql.validation.rules.known_argument_names.KnownArgumentNamesOnDirectivesRule
 graphql.validation.rules.provided_required_arguments.ProvidedRequiredArgumentsOnDirectivesRule
 '''.split())
```

### Comparing `graphql_core-3.3.0a2/docs/diffs.rst` & `graphql_core-3.3.0a3/docs/diffs.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/intro.rst` & `graphql_core-3.3.0a3/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/make.bat` & `graphql_core-3.3.0a3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/modules/language.rst` & `graphql_core-3.3.0a3/docs/modules/language.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,32 +27,36 @@
 .. autoclass:: DirectiveDefinitionNode
 .. autoclass:: DirectiveNode
 .. autoclass:: DocumentNode
 .. autoclass:: EnumTypeDefinitionNode
 .. autoclass:: EnumTypeExtensionNode
 .. autoclass:: EnumValueDefinitionNode
 .. autoclass:: EnumValueNode
+.. autoclass:: ErrorBoundaryNode
 .. autoclass:: ExecutableDefinitionNode
 .. autoclass:: FieldDefinitionNode
 .. autoclass:: FieldNode
 .. autoclass:: FloatValueNode
 .. autoclass:: FragmentDefinitionNode
 .. autoclass:: FragmentSpreadNode
 .. autoclass:: InlineFragmentNode
 .. autoclass:: InputObjectTypeDefinitionNode
 .. autoclass:: InputObjectTypeExtensionNode
 .. autoclass:: InputValueDefinitionNode
 .. autoclass:: IntValueNode
 .. autoclass:: InterfaceTypeDefinitionNode
 .. autoclass:: InterfaceTypeExtensionNode
+.. autoclass:: ListNullabilityOperatorNode
 .. autoclass:: ListTypeNode
 .. autoclass:: ListValueNode
 .. autoclass:: NameNode
 .. autoclass:: NamedTypeNode
+.. autoclass:: NonNullAssertionNode
 .. autoclass:: NonNullTypeNode
+.. autoclass:: NullabilityAssertionNode
 .. autoclass:: NullValueNode
 .. autoclass:: ObjectFieldNode
 .. autoclass:: ObjectTypeDefinitionNode
 .. autoclass:: ObjectTypeExtensionNode
 .. autoclass:: ObjectValueNode
 .. autoclass:: OperationDefinitionNode
 .. autoclass:: OperationType
```

### Comparing `graphql_core-3.3.0a2/docs/modules/pyutils.rst` & `graphql_core-3.3.0a3/docs/modules/pyutils.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/modules/type.rst` & `graphql_core-3.3.0a3/docs/modules/type.rst`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,18 @@
 
 Definitions
 ^^^^^^^^^^^
 
 .. autoclass:: GraphQLDirective
 .. autoclass:: GraphQLIncludeDirective
 .. autoclass:: GraphQLSkipDirective
+.. autoclass:: GraphQLDeferDirective
+.. autoclass:: GraphQLStreamDirective
 .. autoclass:: GraphQLDeprecatedDirective
+.. autoclass:: GraphQLSpecifiedByDirective
 
 .. data:: specified_directives
 
    A tuple with all directives from the GraphQL specification
 
 .. data:: DEFAULT_DEPRECATION_REASON
    :annotation: = 'No longer supported'
```

### Comparing `graphql_core-3.3.0a2/docs/modules/utilities.rst` & `graphql_core-3.3.0a3/docs/modules/utilities.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/modules/validation.rst` & `graphql_core-3.3.0a3/docs/modules/validation.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/usage/extension.rst` & `graphql_core-3.3.0a3/docs/usage/extension.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/usage/introspection.rst` & `graphql_core-3.3.0a3/docs/usage/introspection.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/usage/methods.rst` & `graphql_core-3.3.0a3/docs/usage/methods.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/usage/other.rst` & `graphql_core-3.3.0a3/docs/usage/other.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/usage/parser.rst` & `graphql_core-3.3.0a3/docs/usage/parser.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/usage/queries.rst` & `graphql_core-3.3.0a3/docs/usage/queries.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/usage/resolvers.rst` & `graphql_core-3.3.0a3/docs/usage/resolvers.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/usage/schema.rst` & `graphql_core-3.3.0a3/docs/usage/schema.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/usage/sdl.rst` & `graphql_core-3.3.0a3/docs/usage/sdl.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/docs/usage/validator.rst` & `graphql_core-3.3.0a3/docs/usage/validator.rst`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/pyproject.toml` & `graphql_core-3.3.0a3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "graphql-core"
-version = "3.3.0a2"
-description = """
+version = "3.3.0a3"
+description = """\
 GraphQL-core is a Python port of GraphQL.js,\
  the JavaScript reference implementation for GraphQL."""
 license = "MIT"
 authors = ["Christoph Zwerschke <cito@online.de>"]
 readme = "README.md"
 homepage = "https://github.com/graphql-python/graphql-core"
 repository = "https://github.com/graphql-python/graphql-core"
@@ -38,47 +38,61 @@
 
 [tool.poetry.urls]
 Changelog = "https://github.com/graphql-python/graphql-core/releases"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 typing-extensions = [
-    { version = "^4.4", python = "<3.10" }
+    { version = "^4.5", python = "<3.10" }
 ]
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.2"
-pytest-asyncio = ">=0.20,<1"
+pytest = "^7.3"
+pytest-asyncio = ">=0.21,<1"
 pytest-benchmark = "^4.0"
-pytest-cov = "^4.0"
-pytest-describe = "^2.0"
+pytest-cov = "^4.1"
+pytest-describe = "^2.1"
 pytest-timeout = "^2.1"
-tox = "^3.26"
+tox = [
+    { version = ">=4.5,<5", python = ">=3.8" },
+    { version = ">=3.28,<4", python = "<3.8" }
+]
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
-black = "22.10.0"
-flake8 = "^5.0"
+black = "23.3.0"
+flake8 = [
+    { version = ">=5,<7", python = ">=3.8.1" },
+    { version = ">=5,<6", python = "<3.8.1" }
+]
 flake8-bandit = "^4.1"
-flake8-bugbear = "22.9.23"
-isort = "^5.10"
-mypy = "0.982"
+flake8-bugbear = [
+    { version = "23.5.9", python = ">=3.8.1" },
+    { version = "23.3.12", python = "<3.8.1" },
+]
+isort = [
+    { version = "^5.12", python = ">=3.8" },
+    { version = "^5.11", python = "<3.8" }
+]
+mypy = "1.3.0"
 bump2version = ">=1.0,<2"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
-# Sphinx >= 4.4 has conflicting dependencies with Flake8
-sphinx = ">= 4.3,<6"
+sphinx = [
+    { version = ">=4,<7", python = ">=3.8" },
+    { version = ">=4,<6", python = "<3.8" }
+]
 sphinx_rtd_theme = ">=1,<2"
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 
 [tool.black]
 target-version = ["py37", "py38", "py39", "py310", "py311"]
@@ -116,15 +130,15 @@
 src_paths = ["src", "tests"]
 skip_glob = ["src/**/__init__.py"]
 profile = "black"
 force_single_line = false
 lines_after_imports = 2
 
 [tool.mypy]
-python_version = "3.10"
+python_version = "3.11"
 check_untyped_defs = true
 no_implicit_optional = true
 strict_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_untyped_defs = true
 
@@ -134,24 +148,24 @@
     "graphql.pyutils.frozen_list",
     "graphql.type.introspection",
     "tests.*"
 ]
 disallow_untyped_defs = false
 
 [tool.pytest.ini_options]
-minversion = "7.2"
+minversion = "7.3"
 # Only run benchmarks as tests.
 # To actually run the benchmarks, use --benchmark-enable on the command line.
 # To run the slow tests (fuzzing), add --run-slow on the command line.
 addopts = "--benchmark-disable"
 # Deactivate default name pattern for test classes (we use pytest_describe).
 python_classes = "PyTest*"
 # Handle all async fixtures and tests automatically by asyncio
 asyncio_mode = "auto"
 # Set a timeout in seconds for aborting tests that run too long.
 timeout = "100"
 # Ignore config options not (yet) available in older Python versions.
 filterwarnings = "ignore::pytest.PytestConfigWarning"
 
 [build-system]
-requires = ["poetry_core>=1.2,<2"]
+requires = ["poetry_core>=1.6,<2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `graphql_core-3.3.0a2/src/graphql/__init__.py` & `graphql_core-3.3.0a3/src/graphql/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     SKIP,
     REMOVE,
     IDLE,
     DirectiveLocation,
     # Predicates
     is_definition_node,
     is_executable_definition_node,
+    is_nullability_assertion_node,
     is_selection_node,
     is_value_node,
     is_const_value_node,
     is_type_node,
     is_type_system_definition_node,
     is_type_definition_node,
     is_type_system_extension_node,
@@ -106,14 +107,18 @@
     OperationType,
     VariableDefinitionNode,
     VariableNode,
     SelectionSetNode,
     SelectionNode,
     FieldNode,
     ArgumentNode,
+    NullabilityAssertionNode,
+    NonNullAssertionNode,
+    ErrorBoundaryNode,
+    ListNullabilityOperatorNode,
     ConstArgumentNode,
     FragmentSpreadNode,
     InlineFragmentNode,
     FragmentDefinitionNode,
     ValueNode,
     ConstValueNode,
     IntValueNode,
@@ -244,14 +249,16 @@
     # Int boundaries constants
     GRAPHQL_MAX_INT,
     GRAPHQL_MIN_INT,
     # Built-in Directives defined by the Spec
     specified_directives,
     GraphQLIncludeDirective,
     GraphQLSkipDirective,
+    GraphQLDeferDirective,
+    GraphQLStreamDirective,
     GraphQLDeprecatedDirective,
     GraphQLSpecifiedByDirective,
     # "Enum" of Type Kinds
     TypeKind,
     # Constant Deprecation Reason
     DEFAULT_DEPRECATION_REASON,
     # GraphQL Types for introspection.
@@ -309,15 +316,15 @@
     get_nullable_type,
     get_named_type,
     # Thunk handling
     resolve_thunk,
     # Validate GraphQL schema.
     validate_schema,
     assert_valid_schema,
-    #  Uphold the spec rules about naming
+    # Uphold the spec rules about naming
     assert_name,
     assert_enum_value_name,
     # Types
     GraphQLType,
     GraphQLInputType,
     GraphQLOutputType,
     GraphQLLeafType,
@@ -338,14 +345,15 @@
     GraphQLEnumValue,
     GraphQLEnumValueMap,
     GraphQLField,
     GraphQLFieldMap,
     GraphQLFieldResolver,
     GraphQLInputField,
     GraphQLInputFieldMap,
+    GraphQLInputFieldOutType,
     GraphQLScalarSerializer,
     GraphQLScalarValueParser,
     GraphQLScalarLiteralParser,
     GraphQLIsTypeOfFn,
     GraphQLResolveInfo,
     ResponsePath,
     GraphQLTypeResolver,
@@ -423,19 +431,30 @@
     default_type_resolver,
     get_argument_values,
     get_directive_values,
     get_variable_values,
     # Types
     ExecutionContext,
     ExecutionResult,
+    ExperimentalIncrementalExecutionResults,
+    InitialIncrementalExecutionResult,
+    SubsequentIncrementalExecutionResult,
+    IncrementalDeferResult,
+    IncrementalStreamResult,
+    IncrementalResult,
     FormattedExecutionResult,
+    FormattedInitialIncrementalExecutionResult,
+    FormattedSubsequentIncrementalExecutionResult,
+    FormattedIncrementalDeferResult,
+    FormattedIncrementalStreamResult,
+    FormattedIncrementalResult,
     # Subscription
     subscribe,
     create_source_event_stream,
-    MapAsyncIterator,
+    map_async_iterable,
     # Middleware
     Middleware,
     MiddlewareManager,
 )
 
 # The primary entry point into fulfilling a GraphQL request.
 from .graphql import graphql, graphql_sync
@@ -475,14 +494,16 @@
     "GraphQLBoolean",
     "GraphQLID",
     "GRAPHQL_MAX_INT",
     "GRAPHQL_MIN_INT",
     "specified_directives",
     "GraphQLIncludeDirective",
     "GraphQLSkipDirective",
+    "GraphQLDeferDirective",
+    "GraphQLStreamDirective",
     "GraphQLDeprecatedDirective",
     "GraphQLSpecifiedByDirective",
     "TypeKind",
     "DEFAULT_DEPRECATION_REASON",
     "introspection_types",
     "SchemaMetaFieldDef",
     "TypeMetaFieldDef",
@@ -558,14 +579,15 @@
     "GraphQLEnumValue",
     "GraphQLEnumValueMap",
     "GraphQLField",
     "GraphQLFieldMap",
     "GraphQLFieldResolver",
     "GraphQLInputField",
     "GraphQLInputFieldMap",
+    "GraphQLInputFieldOutType",
     "GraphQLScalarSerializer",
     "GraphQLScalarValueParser",
     "GraphQLScalarLiteralParser",
     "GraphQLIsTypeOfFn",
     "GraphQLResolveInfo",
     "ResponsePath",
     "GraphQLTypeResolver",
@@ -602,14 +624,15 @@
     "BREAK",
     "SKIP",
     "REMOVE",
     "IDLE",
     "DirectiveLocation",
     "is_definition_node",
     "is_executable_definition_node",
+    "is_nullability_assertion_node",
     "is_selection_node",
     "is_value_node",
     "is_const_value_node",
     "is_type_node",
     "is_type_system_definition_node",
     "is_type_definition_node",
     "is_type_system_extension_node",
@@ -626,14 +649,18 @@
     "OperationType",
     "VariableDefinitionNode",
     "VariableNode",
     "SelectionSetNode",
     "SelectionNode",
     "FieldNode",
     "ArgumentNode",
+    "NullabilityAssertionNode",
+    "NonNullAssertionNode",
+    "ErrorBoundaryNode",
+    "ListNullabilityOperatorNode",
     "ConstArgumentNode",
     "FragmentSpreadNode",
     "InlineFragmentNode",
     "FragmentDefinitionNode",
     "ValueNode",
     "ConstValueNode",
     "IntValueNode",
@@ -682,20 +709,31 @@
     "default_field_resolver",
     "default_type_resolver",
     "get_argument_values",
     "get_directive_values",
     "get_variable_values",
     "ExecutionContext",
     "ExecutionResult",
+    "ExperimentalIncrementalExecutionResults",
+    "InitialIncrementalExecutionResult",
+    "SubsequentIncrementalExecutionResult",
+    "IncrementalDeferResult",
+    "IncrementalStreamResult",
+    "IncrementalResult",
     "FormattedExecutionResult",
+    "FormattedInitialIncrementalExecutionResult",
+    "FormattedSubsequentIncrementalExecutionResult",
+    "FormattedIncrementalDeferResult",
+    "FormattedIncrementalStreamResult",
+    "FormattedIncrementalResult",
     "Middleware",
     "MiddlewareManager",
     "subscribe",
     "create_source_event_stream",
-    "MapAsyncIterator",
+    "map_async_iterable",
     "validate",
     "ValidationContext",
     "ValidationRule",
     "ASTValidationRule",
     "SDLValidationRule",
     "specified_rules",
     "ExecutableDefinitionsRule",
```

### Comparing `graphql_core-3.3.0a2/src/graphql/error/graphql_error.py` & `graphql_core-3.3.0a3/src/graphql/error/graphql_error.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/error/located_error.py` & `graphql_core-3.3.0a3/src/graphql/error/located_error.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/error/syntax_error.py` & `graphql_core-3.3.0a3/src/graphql/error/syntax_error.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/execution/collect_fields.py` & `graphql_core-3.3.0a3/src/graphql/execution/collect_fields.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,139 +1,232 @@
 from collections import defaultdict
-from typing import Any, Dict, List, Set, Union
+from typing import Any, Dict, List, NamedTuple, Optional, Set, Union
 
 from ..language import (
     FieldNode,
     FragmentDefinitionNode,
     FragmentSpreadNode,
     InlineFragmentNode,
     SelectionSetNode,
 )
 from ..type import (
+    GraphQLDeferDirective,
     GraphQLIncludeDirective,
     GraphQLObjectType,
     GraphQLSchema,
     GraphQLSkipDirective,
     is_abstract_type,
 )
 from ..utilities.type_from_ast import type_from_ast
 from .values import get_directive_values
 
 
-__all__ = ["collect_fields", "collect_subfields"]
+__all__ = ["collect_fields", "collect_subfields", "FieldsAndPatches"]
+
+
+class PatchFields(NamedTuple):
+    """Optionally labelled set of fields to be used as a patch."""
+
+    label: Optional[str]
+    fields: Dict[str, List[FieldNode]]
+
+
+class FieldsAndPatches(NamedTuple):
+    """Tuple of collected fields and patches to be applied."""
+
+    fields: Dict[str, List[FieldNode]]
+    patches: List[PatchFields]
 
 
 def collect_fields(
     schema: GraphQLSchema,
     fragments: Dict[str, FragmentDefinitionNode],
     variable_values: Dict[str, Any],
     runtime_type: GraphQLObjectType,
     selection_set: SelectionSetNode,
-) -> Dict[str, List[FieldNode]]:
+) -> FieldsAndPatches:
     """Collect fields.
 
     Given a selection_set, collects all the fields and returns them.
 
     collect_fields requires the "runtime type" of an object. For a field that
     returns an Interface or Union type, the "runtime type" will be the actual
     object type returned by that field.
 
     For internal use only.
     """
     fields: Dict[str, List[FieldNode]] = defaultdict(list)
+    patches: List[PatchFields] = []
     collect_fields_impl(
-        schema, fragments, variable_values, runtime_type, selection_set, fields, set()
+        schema,
+        fragments,
+        variable_values,
+        runtime_type,
+        selection_set,
+        fields,
+        patches,
+        set(),
     )
-    return fields
+    return FieldsAndPatches(fields, patches)
 
 
 def collect_subfields(
     schema: GraphQLSchema,
     fragments: Dict[str, FragmentDefinitionNode],
     variable_values: Dict[str, Any],
     return_type: GraphQLObjectType,
     field_nodes: List[FieldNode],
-) -> Dict[str, List[FieldNode]]:
+) -> FieldsAndPatches:
     """Collect subfields.
 
     Given a list of field nodes, collects all the subfields of the passed in fields,
     and returns them at the end.
 
     collect_subfields requires the "return type" of an object. For a field that
     returns an Interface or Union type, the "return type" will be the actual
     object type returned by that field.
 
     For internal use only.
     """
     sub_field_nodes: Dict[str, List[FieldNode]] = defaultdict(list)
     visited_fragment_names: Set[str] = set()
+
+    sub_patches: List[PatchFields] = []
+    sub_fields_and_patches = FieldsAndPatches(sub_field_nodes, sub_patches)
+
     for node in field_nodes:
         if node.selection_set:
             collect_fields_impl(
                 schema,
                 fragments,
                 variable_values,
                 return_type,
                 node.selection_set,
                 sub_field_nodes,
+                sub_patches,
                 visited_fragment_names,
             )
-    return sub_field_nodes
+    return sub_fields_and_patches
 
 
 def collect_fields_impl(
     schema: GraphQLSchema,
     fragments: Dict[str, FragmentDefinitionNode],
     variable_values: Dict[str, Any],
     runtime_type: GraphQLObjectType,
     selection_set: SelectionSetNode,
     fields: Dict[str, List[FieldNode]],
+    patches: List[PatchFields],
     visited_fragment_names: Set[str],
 ) -> None:
     """Collect fields (internal implementation)."""
+    patch_fields: Dict[str, List[FieldNode]]
+
     for selection in selection_set.selections:
         if isinstance(selection, FieldNode):
             if not should_include_node(variable_values, selection):
                 continue
             fields[get_field_entry_key(selection)].append(selection)
         elif isinstance(selection, InlineFragmentNode):
             if not should_include_node(
                 variable_values, selection
             ) or not does_fragment_condition_match(schema, selection, runtime_type):
                 continue
-            collect_fields_impl(
-                schema,
-                fragments,
-                variable_values,
-                runtime_type,
-                selection.selection_set,
-                fields,
-                visited_fragment_names,
-            )
+
+            defer = get_defer_values(variable_values, selection)
+            if defer:
+                patch_fields = defaultdict(list)
+                collect_fields_impl(
+                    schema,
+                    fragments,
+                    variable_values,
+                    runtime_type,
+                    selection.selection_set,
+                    patch_fields,
+                    patches,
+                    visited_fragment_names,
+                )
+                patches.append(PatchFields(defer.label, patch_fields))
+            else:
+                collect_fields_impl(
+                    schema,
+                    fragments,
+                    variable_values,
+                    runtime_type,
+                    selection.selection_set,
+                    fields,
+                    patches,
+                    visited_fragment_names,
+                )
         elif isinstance(selection, FragmentSpreadNode):  # pragma: no cover else
             frag_name = selection.name.value
-            if frag_name in visited_fragment_names or not should_include_node(
-                variable_values, selection
-            ):
+
+            if not should_include_node(variable_values, selection):
+                continue
+
+            defer = get_defer_values(variable_values, selection)
+            if frag_name in visited_fragment_names and not defer:
                 continue
-            visited_fragment_names.add(frag_name)
+
             fragment = fragments.get(frag_name)
             if not fragment or not does_fragment_condition_match(
                 schema, fragment, runtime_type
             ):
                 continue
-            collect_fields_impl(
-                schema,
-                fragments,
-                variable_values,
-                runtime_type,
-                fragment.selection_set,
-                fields,
-                visited_fragment_names,
-            )
+
+            if not defer:
+                visited_fragment_names.add(frag_name)
+
+            if defer:
+                patch_fields = defaultdict(list)
+                collect_fields_impl(
+                    schema,
+                    fragments,
+                    variable_values,
+                    runtime_type,
+                    fragment.selection_set,
+                    patch_fields,
+                    patches,
+                    visited_fragment_names,
+                )
+                patches.append(PatchFields(defer.label, patch_fields))
+            else:
+                collect_fields_impl(
+                    schema,
+                    fragments,
+                    variable_values,
+                    runtime_type,
+                    fragment.selection_set,
+                    fields,
+                    patches,
+                    visited_fragment_names,
+                )
+
+
+class DeferValues(NamedTuple):
+    """Values of an active defer directive."""
+
+    label: Optional[str]
+
+
+def get_defer_values(
+    variable_values: Dict[str, Any], node: Union[FragmentSpreadNode, InlineFragmentNode]
+) -> Optional[DeferValues]:
+    """Get values of defer directive if active.
+
+    Returns an object containing the `@defer` arguments if a field should be
+    deferred based on the experimental flag, defer directive present and
+    not disabled by the "if" argument.
+    """
+    defer = get_directive_values(GraphQLDeferDirective, node, variable_values)
+
+    if not defer or defer.get("if") is False:
+        return None
+
+    return DeferValues(defer.get("label"))
 
 
 def should_include_node(
     variable_values: Dict[str, Any],
     node: Union[FragmentSpreadNode, FieldNode, InlineFragmentNode],
 ) -> bool:
     """Check if node should be included
@@ -161,14 +254,15 @@
     type_condition_node = fragment.type_condition
     if not type_condition_node:
         return True
     conditional_type = type_from_ast(schema, type_condition_node)
     if conditional_type is type_:
         return True
     if is_abstract_type(conditional_type):
+        # noinspection PyTypeChecker
         return schema.is_sub_type(conditional_type, type_)
     return False
 
 
 def get_field_entry_key(node: FieldNode) -> str:
     """Implements the logic to compute the key of a given field's entry"""
     return node.alias.value if node.alias else node.name.value
```

### Comparing `graphql_core-3.3.0a2/src/graphql/execution/middleware.py` & `graphql_core-3.3.0a3/src/graphql/execution/middleware.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/execution/subscribe.py` & `graphql_core-3.3.0a3/src/graphql/graphql.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,209 +1,201 @@
-from inspect import isawaitable
-from typing import Any, AsyncIterable, AsyncIterator, Dict, Optional, Type, Union
+from asyncio import ensure_future
+from typing import Any, Awaitable, Callable, Dict, Optional, Type, Union, cast
 
-from ..error import GraphQLError, located_error
-from ..execution.collect_fields import collect_fields
-from ..execution.execute import (
-    ExecutionContext,
-    ExecutionResult,
-    assert_valid_execution_arguments,
-    execute,
+from .error import GraphQLError
+from .execution import ExecutionContext, ExecutionResult, Middleware, execute
+from .language import Source, parse
+from .pyutils import AwaitableOrValue
+from .pyutils import is_awaitable as default_is_awaitable
+from .type import (
+    GraphQLFieldResolver,
+    GraphQLSchema,
+    GraphQLTypeResolver,
+    validate_schema,
 )
-from ..execution.values import get_argument_values
-from ..language import DocumentNode
-from ..pyutils import Path, inspect
-from ..type import GraphQLFieldResolver, GraphQLSchema
-from .map_async_iterator import MapAsyncIterator
 
 
-__all__ = ["subscribe", "create_source_event_stream"]
+__all__ = ["graphql", "graphql_sync"]
 
 
-async def subscribe(
+async def graphql(
     schema: GraphQLSchema,
-    document: DocumentNode,
+    source: Union[str, Source],
     root_value: Any = None,
     context_value: Any = None,
     variable_values: Optional[Dict[str, Any]] = None,
     operation_name: Optional[str] = None,
     field_resolver: Optional[GraphQLFieldResolver] = None,
-    subscribe_field_resolver: Optional[GraphQLFieldResolver] = None,
+    type_resolver: Optional[GraphQLTypeResolver] = None,
+    middleware: Optional[Middleware] = None,
     execution_context_class: Optional[Type[ExecutionContext]] = None,
-) -> Union[AsyncIterator[ExecutionResult], ExecutionResult]:
-    """Create a GraphQL subscription.
-
-    Implements the "Subscribe" algorithm described in the GraphQL spec.
-
-    Returns a coroutine object which yields either an AsyncIterator (if successful) or
-    an ExecutionResult (client error). The coroutine will raise an exception if a server
-    error occurs.
-
-    If the client-provided arguments to this function do not result in a compliant
-    subscription, a GraphQL Response (ExecutionResult) with descriptive errors and no
-    data will be returned.
-
-    If the source stream could not be created due to faulty subscription resolver logic
-    or underlying systems, the coroutine object will yield a single ExecutionResult
-    containing ``errors`` and no ``data``.
-
-    If the operation succeeded, the coroutine will yield an AsyncIterator, which yields
-    a stream of ExecutionResults representing the response stream.
+    is_awaitable: Optional[Callable[[Any], bool]] = None,
+) -> ExecutionResult:
+    """Execute a GraphQL operation asynchronously.
+
+    This is the primary entry point function for fulfilling GraphQL operations by
+    parsing, validating, and executing a GraphQL document along side a GraphQL schema.
+
+    More sophisticated GraphQL servers, such as those which persist queries, may wish
+    to separate the validation and execution phases to a static time tooling step,
+    and a server runtime step.
+
+    This function does not support incremental delivery (`@defer` and `@stream`).
+
+    Accepts the following arguments:
+
+    :arg schema:
+      The GraphQL type system to use when validating and executing a query.
+    :arg source:
+      A GraphQL language formatted string representing the requested operation.
+    :arg root_value:
+      The value provided as the first argument to resolver functions on the top level
+      type (e.g. the query object type).
+    :arg context_value:
+      The context value is provided as an attribute of the second argument
+      (the resolve info) to resolver functions. It is used to pass shared information
+      useful at any point during query execution, for example the currently logged in
+      user and connections to databases or other services.
+    :arg variable_values:
+      A mapping of variable name to runtime value to use for all variables defined
+      in the request string.
+    :arg operation_name:
+      The name of the operation to use if request string contains multiple possible
+      operations. Can be omitted if request string contains only one operation.
+    :arg field_resolver:
+      A resolver function to use when one is not provided by the schema.
+      If not provided, the default field resolver is used (which looks for a value
+      or method on the source value with the field's name).
+    :arg type_resolver:
+      A type resolver function to use when none is provided by the schema.
+      If not provided, the default type resolver is used (which looks for a
+      ``__typename`` field or alternatively calls the
+      :meth:`~graphql.type.GraphQLObjectType.is_type_of` method).
+    :arg middleware:
+      The middleware to wrap the resolvers with
+    :arg execution_context_class:
+      The execution context class to use to build the context
+    :arg is_awaitable:
+      The predicate to be used for checking whether values are awaitable
     """
-    result_or_stream = await create_source_event_stream(
+    # Always return asynchronously for a consistent API.
+    result = graphql_impl(
         schema,
-        document,
+        source,
         root_value,
         context_value,
         variable_values,
         operation_name,
-        subscribe_field_resolver,
+        field_resolver,
+        type_resolver,
+        middleware,
         execution_context_class,
+        is_awaitable,
     )
-    if isinstance(result_or_stream, ExecutionResult):
-        return result_or_stream
 
-    async def map_source_to_response(payload: Any) -> ExecutionResult:
-        """Map source to response.
+    if default_is_awaitable(result):
+        return await cast(Awaitable[ExecutionResult], result)
 
-        For each payload yielded from a subscription, map it over the normal GraphQL
-        :func:`~graphql.execute` function, with ``payload`` as the ``root_value``.
-        This implements the "MapSourceToResponseEvent" algorithm described in the
-        GraphQL specification. The :func:`~graphql.execute` function provides the
-        "ExecuteSubscriptionEvent" algorithm, as it is nearly identical to the
-        "ExecuteQuery" algorithm, for which :func:`~graphql.execute` is also used.
-        """
-        result = execute(
-            schema,
-            document,
-            payload,
-            context_value,
-            variable_values,
-            operation_name,
-            field_resolver,
-            execution_context_class=execution_context_class,
-        )
-        return await result if isawaitable(result) else result
+    return cast(ExecutionResult, result)
 
-    # Map every source value to a ExecutionResult value as described above.
-    return MapAsyncIterator(result_or_stream, map_source_to_response)
 
+def assume_not_awaitable(_value: Any) -> bool:
+    """Replacement for is_awaitable if everything is assumed to be synchronous."""
+    return False
 
-async def create_source_event_stream(
+
+def graphql_sync(
     schema: GraphQLSchema,
-    document: DocumentNode,
+    source: Union[str, Source],
     root_value: Any = None,
     context_value: Any = None,
     variable_values: Optional[Dict[str, Any]] = None,
     operation_name: Optional[str] = None,
-    subscribe_field_resolver: Optional[GraphQLFieldResolver] = None,
+    field_resolver: Optional[GraphQLFieldResolver] = None,
+    type_resolver: Optional[GraphQLTypeResolver] = None,
+    middleware: Optional[Middleware] = None,
     execution_context_class: Optional[Type[ExecutionContext]] = None,
-) -> Union[AsyncIterable[Any], ExecutionResult]:
-    """Create source event stream
+    check_sync: bool = False,
+) -> ExecutionResult:
+    """Execute a GraphQL operation synchronously.
+
+    The graphql_sync function also fulfills GraphQL operations by parsing, validating,
+    and executing a GraphQL document along side a GraphQL schema. However, it guarantees
+    to complete synchronously (or throw an error) assuming that all field resolvers
+    are also synchronous.
 
-    Implements the "CreateSourceEventStream" algorithm described in the GraphQL
-    specification, resolving the subscription source event stream.
-
-    Returns a coroutine that yields an AsyncIterable.
-
-    If the client-provided arguments to this function do not result in a compliant
-    subscription, a GraphQL Response (ExecutionResult) with descriptive errors and no
-    data will be returned.
-
-    If the source stream could not be created due to faulty subscription resolver logic
-    or underlying systems, the coroutine object will yield a single ExecutionResult
-    containing ``errors`` and no ``data``.
-
-    A source event stream represents a sequence of events, each of which triggers a
-    GraphQL execution for that event.
-
-    This may be useful when hosting the stateful subscription service in a different
-    process or machine than the stateless GraphQL execution engine, or otherwise
-    separating these two steps. For more on this, see the "Supporting Subscriptions
-    at Scale" information in the GraphQL spec.
+    Set check_sync to True to still run checks that no awaitable values are returned.
     """
-    # If arguments are missing or incorrectly typed, this is an internal developer
-    # mistake which should throw an early error.
-    assert_valid_execution_arguments(schema, document, variable_values)
-
-    if not execution_context_class:
-        execution_context_class = ExecutionContext
-
-    # If a valid context cannot be created due to incorrect arguments,
-    # a "Response" with only errors is returned.
-    context = execution_context_class.build(
+    is_awaitable = (
+        check_sync
+        if callable(check_sync)
+        else (None if check_sync else assume_not_awaitable)
+    )
+    result = graphql_impl(
         schema,
-        document,
+        source,
         root_value,
         context_value,
         variable_values,
         operation_name,
-        subscribe_field_resolver=subscribe_field_resolver,
+        field_resolver,
+        type_resolver,
+        middleware,
+        execution_context_class,
+        is_awaitable,
     )
 
-    # Return early errors if execution context failed.
-    if isinstance(context, list):
-        return ExecutionResult(data=None, errors=context)
+    # Assert that the execution was synchronous.
+    if default_is_awaitable(result):
+        ensure_future(cast(Awaitable[ExecutionResult], result)).cancel()
+        raise RuntimeError("GraphQL execution failed to complete synchronously.")
 
+    return cast(ExecutionResult, result)
+
+
+def graphql_impl(
+    schema: GraphQLSchema,
+    source: Union[str, Source],
+    root_value: Any,
+    context_value: Any,
+    variable_values: Optional[Dict[str, Any]],
+    operation_name: Optional[str],
+    field_resolver: Optional[GraphQLFieldResolver],
+    type_resolver: Optional[GraphQLTypeResolver],
+    middleware: Optional[Middleware],
+    execution_context_class: Optional[Type[ExecutionContext]],
+    is_awaitable: Optional[Callable[[Any], bool]],
+) -> AwaitableOrValue[ExecutionResult]:
+    """Execute a query, return asynchronously only if necessary."""
+    # Validate Schema
+    schema_validation_errors = validate_schema(schema)
+    if schema_validation_errors:
+        return ExecutionResult(data=None, errors=schema_validation_errors)
+
+    # Parse
     try:
-        return await execute_subscription(context)
+        document = parse(source)
     except GraphQLError as error:
         return ExecutionResult(data=None, errors=[error])
 
+    # Validate
+    from .validation import validate
 
-async def execute_subscription(context: ExecutionContext) -> AsyncIterable[Any]:
-    schema = context.schema
+    validation_errors = validate(schema, document)
+    if validation_errors:
+        return ExecutionResult(data=None, errors=validation_errors)
 
-    root_type = schema.subscription_type
-    if root_type is None:
-        raise GraphQLError(
-            "Schema is not configured to execute subscription operation.",
-            context.operation,
-        )
-
-    root_fields = collect_fields(
+    # Execute
+    return execute(
         schema,
-        context.fragments,
-        context.variable_values,
-        root_type,
-        context.operation.selection_set,
+        document,
+        root_value,
+        context_value,
+        variable_values,
+        operation_name,
+        field_resolver,
+        type_resolver,
+        None,
+        middleware,
+        execution_context_class,
+        is_awaitable,
     )
-    response_name, field_nodes = next(iter(root_fields.items()))
-    field_name = field_nodes[0].name.value
-    field_def = schema.get_field(root_type, field_name)
-
-    if not field_def:
-        raise GraphQLError(
-            f"The subscription field '{field_name}' is not defined.", field_nodes
-        )
-
-    path = Path(None, response_name, root_type.name)
-    info = context.build_resolve_info(field_def, field_nodes, root_type, path)
-
-    # Implements the "ResolveFieldEventStream" algorithm from GraphQL specification.
-    # It differs from "ResolveFieldValue" due to providing a different `resolveFn`.
-
-    try:
-        # Build a dictionary of arguments from the field.arguments AST, using the
-        # variables scope to fulfill any variable references.
-        args = get_argument_values(field_def, field_nodes[0], context.variable_values)
-
-        # Call the `subscribe()` resolver or the default resolver to produce an
-        # AsyncIterable yielding raw payloads.
-        resolve_fn = field_def.subscribe or context.subscribe_field_resolver
-
-        event_stream = resolve_fn(context.root_value, info, **args)
-        if context.is_awaitable(event_stream):
-            event_stream = await event_stream
-        if isinstance(event_stream, Exception):
-            raise event_stream
-
-        # Assert field returned an event stream, otherwise yield an error.
-        if not isinstance(event_stream, AsyncIterable):
-            raise GraphQLError(
-                "Subscription field must return AsyncIterable."
-                f" Received: {inspect(event_stream)}."
-            )
-
-        return event_stream
-    except Exception as error:
-        raise located_error(error, field_nodes, path.as_list())
```

### Comparing `graphql_core-3.3.0a2/src/graphql/execution/values.py` & `graphql_core-3.3.0a3/src/graphql/execution/values.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/language/__init__.py` & `graphql_core-3.3.0a3/src/graphql/language/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     OperationDefinitionNode,
     OperationType,
     VariableDefinitionNode,
     VariableNode,
     SelectionSetNode,
     SelectionNode,
     FieldNode,
+    NullabilityAssertionNode,
+    NonNullAssertionNode,
+    ErrorBoundaryNode,
+    ListNullabilityOperatorNode,
     ArgumentNode,
     ConstArgumentNode,
     FragmentSpreadNode,
     InlineFragmentNode,
     FragmentDefinitionNode,
     ValueNode,
     ConstValueNode,
@@ -94,14 +98,15 @@
     UnionTypeExtensionNode,
     EnumTypeExtensionNode,
     InputObjectTypeExtensionNode,
 )
 from .predicates import (
     is_definition_node,
     is_executable_definition_node,
+    is_nullability_assertion_node,
     is_selection_node,
     is_value_node,
     is_const_value_node,
     is_type_node,
     is_type_system_definition_node,
     is_type_definition_node,
     is_type_system_extension_node,
@@ -143,14 +148,18 @@
     "OperationDefinitionNode",
     "OperationType",
     "VariableDefinitionNode",
     "VariableNode",
     "SelectionSetNode",
     "SelectionNode",
     "FieldNode",
+    "NullabilityAssertionNode",
+    "NonNullAssertionNode",
+    "ErrorBoundaryNode",
+    "ListNullabilityOperatorNode",
     "ArgumentNode",
     "ConstArgumentNode",
     "FragmentSpreadNode",
     "InlineFragmentNode",
     "FragmentDefinitionNode",
     "ValueNode",
     "ConstValueNode",
@@ -193,14 +202,15 @@
     "ObjectTypeExtensionNode",
     "InterfaceTypeExtensionNode",
     "UnionTypeExtensionNode",
     "EnumTypeExtensionNode",
     "InputObjectTypeExtensionNode",
     "is_definition_node",
     "is_executable_definition_node",
+    "is_nullability_assertion_node",
     "is_selection_node",
     "is_value_node",
     "is_const_value_node",
     "is_type_node",
     "is_type_system_definition_node",
     "is_type_definition_node",
     "is_type_system_extension_node",
```

### Comparing `graphql_core-3.3.0a2/src/graphql/language/ast.py` & `graphql_core-3.3.0a3/src/graphql/language/ast.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     "DefinitionNode",
     "ExecutableDefinitionNode",
     "OperationDefinitionNode",
     "VariableDefinitionNode",
     "SelectionSetNode",
     "SelectionNode",
     "FieldNode",
+    "NullabilityAssertionNode",
+    "NonNullAssertionNode",
+    "ErrorBoundaryNode",
+    "ListNullabilityOperatorNode",
     "ArgumentNode",
     "ConstArgumentNode",
     "FragmentSpreadNode",
     "InlineFragmentNode",
     "FragmentDefinitionNode",
     "ValueNode",
     "ConstValueNode",
@@ -236,15 +240,14 @@
         return not self == other
 
     def __hash__(self) -> int:
         return hash((self.start, self.end))
 
 
 class OperationType(Enum):
-
     QUERY = "query"
     MUTATION = "mutation"
     SUBSCRIPTION = "subscription"
 
 
 # Default map from node kinds to their node attributes (internal)
 QUERY_DOCUMENT_KEYS: Dict[str, Tuple[str, ...]] = {
@@ -255,16 +258,30 @@
         "variable_definitions",
         "directives",
         "selection_set",
     ),
     "variable_definition": ("variable", "type", "default_value", "directives"),
     "variable": ("name",),
     "selection_set": ("selections",),
-    "field": ("alias", "name", "arguments", "directives", "selection_set"),
+    "field": (
+        "alias",
+        "name",
+        "arguments",
+        "directives",
+        "selection_set",
+        # note: Client controlled Nullability is experimental and may be changed
+        # or removed in the future.
+        "nullability_assertion",
+    ),
     "argument": ("name", "value"),
+    # note: Client controlled Nullability is experimental and may be changed
+    # or removed in the future.
+    "list_nullability_operator": ("nullability_assertion",),
+    "non_null_assertion": ("nullability_assertion",),
+    "error_boundary": ("nullability_assertion",),
     "fragment_spread": ("name", "directives"),
     "inline_fragment": ("type_condition", "directives", "selection_set"),
     "fragment_definition": (
         # Note: fragment variable definitions are deprecated and will be removed in v3.3
         "name",
         "variable_definitions",
         "type_condition",
@@ -338,16 +355,25 @@
             value = kwargs.get(key)
             if isinstance(value, list):
                 value = tuple(value)
             setattr(self, key, value)
 
     def __repr__(self) -> str:
         """Get a simple representation of the node."""
-        name, loc = self.__class__.__name__, getattr(self, "loc", None)
-        return f"{name} at {loc}" if loc else name
+        rep = self.__class__.__name__
+        if isinstance(self, NameNode):
+            rep += f"({self.value!r})"
+        else:
+            name = getattr(self, "name", None)
+            if name:
+                rep += f"(name={name.value!r})"
+        loc = getattr(self, "loc", None)
+        if loc:
+            rep += f" at {loc}"
+        return rep
 
     def __eq__(self, other: Any) -> bool:
         """Test whether two nodes are equal (recursively)."""
         return (
             isinstance(other, Node)
             and self.__class__ == other.__class__
             and all(getattr(self, key) == getattr(other, key) for key in self.keys)
@@ -459,31 +485,50 @@
 class SelectionNode(Node):
     __slots__ = ("directives",)
 
     directives: Tuple[DirectiveNode, ...]
 
 
 class FieldNode(SelectionNode):
-    __slots__ = "alias", "name", "arguments", "selection_set"
+    __slots__ = "alias", "name", "arguments", "nullability_assertion", "selection_set"
 
     alias: Optional[NameNode]
     name: NameNode
     arguments: Tuple[ArgumentNode, ...]
+    # Note: Client Controlled Nullability is experimental
+    # and may be changed or removed in the future.
+    nullability_assertion: NullabilityAssertionNode
     selection_set: Optional[SelectionSetNode]
 
 
+class NullabilityAssertionNode(Node):
+    __slots__ = ("nullability_assertion",)
+    nullability_assertion: Optional["NullabilityAssertionNode"]
+
+
+class ListNullabilityOperatorNode(NullabilityAssertionNode):
+    pass
+
+
+class NonNullAssertionNode(NullabilityAssertionNode):
+    nullability_assertion: ListNullabilityOperatorNode
+
+
+class ErrorBoundaryNode(NullabilityAssertionNode):
+    nullability_assertion: ListNullabilityOperatorNode
+
+
 class ArgumentNode(Node):
     __slots__ = "name", "value"
 
     name: NameNode
     value: ValueNode
 
 
 class ConstArgumentNode(ArgumentNode):
-
     value: ConstValueNode
 
 
 # Fragments
 
 
 class FragmentSpreadNode(SelectionNode):
@@ -557,38 +602,35 @@
 class ListValueNode(ValueNode):
     __slots__ = ("values",)
 
     values: Tuple[ValueNode, ...]
 
 
 class ConstListValueNode(ListValueNode):
-
     values: Tuple[ConstValueNode, ...]
 
 
 class ObjectValueNode(ValueNode):
     __slots__ = ("fields",)
 
     fields: Tuple[ObjectFieldNode, ...]
 
 
 class ConstObjectValueNode(ObjectValueNode):
-
     fields: Tuple[ConstObjectFieldNode, ...]
 
 
 class ObjectFieldNode(Node):
     __slots__ = "name", "value"
 
     name: NameNode
     value: ValueNode
 
 
 class ConstObjectFieldNode(ObjectFieldNode):
-
     value: ConstValueNode
 
 
 ConstValueNode: TypeAlias = Union[
     IntValueNode,
     FloatValueNode,
     StringValueNode,
@@ -607,15 +649,14 @@
     __slots__ = "name", "arguments"
 
     name: NameNode
     arguments: Tuple[ArgumentNode, ...]
 
 
 class ConstDirectiveNode(DirectiveNode):
-
     arguments: Tuple[ConstArgumentNode, ...]
 
 
 # Type Reference
 
 
 class TypeNode(Node):
```

### Comparing `graphql_core-3.3.0a2/src/graphql/language/block_string.py` & `graphql_core-3.3.0a3/src/graphql/language/block_string.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/language/character_classes.py` & `graphql_core-3.3.0a3/src/graphql/language/character_classes.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/language/directive_locations.py` & `graphql_core-3.3.0a3/src/graphql/language/directive_locations.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/language/lexer.py` & `graphql_core-3.3.0a3/src/graphql/language/lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -454,14 +454,15 @@
 
         return self.create_token(TokenKind.NAME, start, position, body[start:position])
 
 
 _punctuator_token_kinds = frozenset(
     [
         TokenKind.BANG,
+        TokenKind.QUESTION_MARK,
         TokenKind.DOLLAR,
         TokenKind.AMP,
         TokenKind.PAREN_L,
         TokenKind.PAREN_R,
         TokenKind.SPREAD,
         TokenKind.COLON,
         TokenKind.EQUALS,
@@ -481,14 +482,15 @@
     For internal use only.
     """
     return kind in _punctuator_token_kinds
 
 
 _KIND_FOR_PUNCT = {
     "!": TokenKind.BANG,
+    "?": TokenKind.QUESTION_MARK,
     "$": TokenKind.DOLLAR,
     "&": TokenKind.AMP,
     "(": TokenKind.PAREN_L,
     ")": TokenKind.PAREN_R,
     ":": TokenKind.COLON,
     "=": TokenKind.EQUALS,
     "@": TokenKind.AT,
```

### Comparing `graphql_core-3.3.0a2/src/graphql/language/location.py` & `graphql_core-3.3.0a3/src/graphql/language/location.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/language/parser.py` & `graphql_core-3.3.0a3/src/graphql/language/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,32 +12,36 @@
     DirectiveDefinitionNode,
     DirectiveNode,
     DocumentNode,
     EnumTypeDefinitionNode,
     EnumTypeExtensionNode,
     EnumValueDefinitionNode,
     EnumValueNode,
+    ErrorBoundaryNode,
     FieldDefinitionNode,
     FieldNode,
     FloatValueNode,
     FragmentDefinitionNode,
     FragmentSpreadNode,
     InlineFragmentNode,
     InputObjectTypeDefinitionNode,
     InputObjectTypeExtensionNode,
     InputValueDefinitionNode,
     InterfaceTypeDefinitionNode,
     InterfaceTypeExtensionNode,
     IntValueNode,
+    ListNullabilityOperatorNode,
     ListTypeNode,
     ListValueNode,
     Location,
     NamedTypeNode,
     NameNode,
+    NonNullAssertionNode,
     NonNullTypeNode,
+    NullabilityAssertionNode,
     NullValueNode,
     ObjectFieldNode,
     ObjectTypeDefinitionNode,
     ObjectTypeExtensionNode,
     ObjectValueNode,
     OperationDefinitionNode,
     OperationType,
@@ -76,49 +80,79 @@
 
 SourceType: TypeAlias = Union[Source, str]
 
 
 def parse(
     source: SourceType,
     no_location: bool = False,
+    max_tokens: Optional[int] = None,
     allow_legacy_fragment_variables: bool = False,
+    experimental_client_controlled_nullability: bool = False,
 ) -> DocumentNode:
     """Given a GraphQL source, parse it into a Document.
 
     Throws GraphQLError if a syntax error is encountered.
 
     By default, the parser creates AST nodes that know the location in the source that
     they correspond to. The ``no_location`` option disables that behavior for
     performance or testing.
 
+    Parser CPU and memory usage is linear to the number of tokens in a document,
+    however in extreme cases it becomes quadratic due to memory exhaustion.
+    Parsing happens before validation so even invalid queries can burn lots of
+    CPU time and memory.
+    To prevent this you can set a maximum number of tokens allowed within a document.
+
     Legacy feature (will be removed in v3.3):
 
     If ``allow_legacy_fragment_variables`` is set to ``True``, the parser will
     understand and parse variable definitions contained in a fragment definition.
     They'll be represented in the
     :attr:`~graphql.language.FragmentDefinitionNode.variable_definitions` field
     of the :class:`~graphql.language.FragmentDefinitionNode`.
 
     The syntax is identical to normal, query-defined variables. For example::
 
         fragment A($var: Boolean = false) on T  {
           ...
         }
+
+    EXPERIMENTAL:
+
+    If enabled, the parser will understand and parse Client Controlled Nullability
+    Designators contained in Fields. They'll be represented in the
+    :attr:`~graphql.language.FieldNode.nullability_assertion` field
+    of the :class:`~graphql.language.FieldNode`.
+
+    The syntax looks like the following::
+
+       {
+         nullableField!
+         nonNullableField?
+         nonNullableSelectionSet? {
+           childField!
+        }
+      }
+
+    Note: this feature is experimental and may change or be removed in the future.
     """
     parser = Parser(
         source,
         no_location=no_location,
+        max_tokens=max_tokens,
         allow_legacy_fragment_variables=allow_legacy_fragment_variables,
+        experimental_client_controlled_nullability=experimental_client_controlled_nullability,  # noqa
     )
     return parser.parse_document()
 
 
 def parse_value(
     source: SourceType,
     no_location: bool = False,
+    max_tokens: Optional[int] = None,
     allow_legacy_fragment_variables: bool = False,
 ) -> ValueNode:
     """Parse the AST for a given string containing a GraphQL value.
 
     Throws GraphQLError if a syntax error is encountered.
 
     This is useful within tools that operate upon GraphQL Values directly and in
@@ -126,46 +160,50 @@
 
     Consider providing the results to the utility function:
     :func:`~graphql.utilities.value_from_ast`.
     """
     parser = Parser(
         source,
         no_location=no_location,
+        max_tokens=max_tokens,
         allow_legacy_fragment_variables=allow_legacy_fragment_variables,
     )
     parser.expect_token(TokenKind.SOF)
     value = parser.parse_value_literal(False)
     parser.expect_token(TokenKind.EOF)
     return value
 
 
 def parse_const_value(
     source: SourceType,
     no_location: bool = False,
+    max_tokens: Optional[int] = None,
     allow_legacy_fragment_variables: bool = False,
 ) -> ConstValueNode:
     """Parse the AST for a given string containing a GraphQL constant value.
 
     Similar to parse_value, but raises a arse error if it encounters a variable.
     The return type will be a constant value.
     """
     parser = Parser(
         source,
         no_location=no_location,
+        max_tokens=max_tokens,
         allow_legacy_fragment_variables=allow_legacy_fragment_variables,
     )
     parser.expect_token(TokenKind.SOF)
     value = parser.parse_const_value_literal()
     parser.expect_token(TokenKind.EOF)
     return value
 
 
 def parse_type(
     source: SourceType,
     no_location: bool = False,
+    max_tokens: Optional[int] = None,
     allow_legacy_fragment_variables: bool = False,
 ) -> TypeNode:
     """Parse the AST for a given string containing a GraphQL Type.
 
     Throws GraphQLError if a syntax error is encountered.
 
     This is useful within tools that operate upon GraphQL Types directly and
@@ -173,14 +211,15 @@
 
     Consider providing the results to the utility function:
     :func:`~graphql.utilities.value_from_ast`.
     """
     parser = Parser(
         source,
         no_location=no_location,
+        max_tokens=max_tokens,
         allow_legacy_fragment_variables=allow_legacy_fragment_variables,
     )
     parser.expect_token(TokenKind.SOF)
     type_ = parser.parse_type_reference()
     parser.expect_token(TokenKind.EOF)
     return type_
 
@@ -193,30 +232,40 @@
     such as experimental syntax or if certain features couldn't be contributed upstream.
 
     It's still part of the internal API and is versioned, so any changes to it are never
     considered breaking changes. If you still need to support multiple versions of the
     library, please use the `__version_info__` variable for version detection.
     """
 
-    _lexer: Lexer
     _no_location: bool
+    _max_tokens: Optional[int]
     _allow_legacy_fragment_variables: bool
+    _experimental_client_controlled_nullability: bool
+    _lexer: Lexer
+    _token_counter: int
 
     def __init__(
         self,
         source: SourceType,
         no_location: bool = False,
+        max_tokens: Optional[int] = None,
         allow_legacy_fragment_variables: bool = False,
+        experimental_client_controlled_nullability: bool = False,
     ):
         if not is_source(source):
             source = Source(cast(str, source))
 
-        self._lexer = Lexer(source)
         self._no_location = no_location
+        self._max_tokens = max_tokens
         self._allow_legacy_fragment_variables = allow_legacy_fragment_variables
+        self._experimental_client_controlled_nullability = (
+            experimental_client_controlled_nullability
+        )
+        self._lexer = Lexer(source)
+        self._token_counter = 0
 
     def parse_name(self) -> NameNode:
         """Convert a name lex token into a name parse node."""
         token = self.expect_token(TokenKind.NAME)
         return NameNode(value=token.value, loc=self.loc(token))
 
     # Implement the parsing rules in the Document section.
@@ -372,21 +421,54 @@
         else:
             alias = None
             name = name_or_alias
         return FieldNode(
             alias=alias,
             name=name,
             arguments=self.parse_arguments(False),
+            # Experimental support for Client Controlled Nullability changes
+            # the grammar of Field:
+            nullability_assertion=self.parse_nullability_assertion(),
             directives=self.parse_directives(False),
             selection_set=self.parse_selection_set()
             if self.peek(TokenKind.BRACE_L)
             else None,
             loc=self.loc(start),
         )
 
+    def parse_nullability_assertion(self) -> Optional[NullabilityAssertionNode]:
+        """NullabilityAssertion (grammar not yet finalized)
+
+        # Note: Client Controlled Nullability is experimental and may be changed or
+        # removed in the future.
+        """
+        if not self._experimental_client_controlled_nullability:
+            return None
+
+        start = self._lexer.token
+        nullability_assertion: Optional[NullabilityAssertionNode] = None
+
+        if self.expect_optional_token(TokenKind.BRACKET_L):
+            inner_modifier = self.parse_nullability_assertion()
+            self.expect_token(TokenKind.BRACKET_R)
+            nullability_assertion = ListNullabilityOperatorNode(
+                nullability_assertion=inner_modifier, loc=self.loc(start)
+            )
+
+        if self.expect_optional_token(TokenKind.BANG):
+            nullability_assertion = NonNullAssertionNode(
+                nullability_assertion=nullability_assertion, loc=self.loc(start)
+            )
+        elif self.expect_optional_token(TokenKind.QUESTION_MARK):
+            nullability_assertion = ErrorBoundaryNode(
+                nullability_assertion=nullability_assertion, loc=self.loc(start)
+            )
+
+        return nullability_assertion
+
     def parse_arguments(self, is_const: bool) -> List[ArgumentNode]:
         """Arguments[Const]: (Argument[?Const]+)"""
         item = self.parse_const_argument if is_const else self.parse_argument
         item = cast(Callable[[], ArgumentNode], item)
         return self.optional_many(TokenKind.PAREN_L, item, TokenKind.PAREN_R)
 
     def parse_argument(self, is_const: bool = False) -> ArgumentNode:
@@ -479,15 +561,15 @@
         method_name = self._parse_value_literal_method_names.get(self._lexer.token.kind)
         if method_name:  # pragma: no cover
             return getattr(self, f"parse_{method_name}")(is_const)
         raise self.unexpected()  # pragma: no cover
 
     def parse_string_literal(self, _is_const: bool = False) -> StringValueNode:
         token = self._lexer.token
-        self._lexer.advance()
+        self.advance_lexer()
         return StringValueNode(
             value=token.value,
             block=token.kind == TokenKind.BLOCK_STRING,
             loc=self.loc(token),
         )
 
     def parse_list(self, is_const: bool) -> ListValueNode:
@@ -516,26 +598,26 @@
         return ObjectValueNode(
             fields=self.any(TokenKind.BRACE_L, item, TokenKind.BRACE_R),
             loc=self.loc(start),
         )
 
     def parse_int(self, _is_const: bool = False) -> IntValueNode:
         token = self._lexer.token
-        self._lexer.advance()
+        self.advance_lexer()
         return IntValueNode(value=token.value, loc=self.loc(token))
 
     def parse_float(self, _is_const: bool = False) -> FloatValueNode:
         token = self._lexer.token
-        self._lexer.advance()
+        self.advance_lexer()
         return FloatValueNode(value=token.value, loc=self.loc(token))
 
     def parse_named_values(self, _is_const: bool = False) -> ValueNode:
         token = self._lexer.token
         value = token.value
-        self._lexer.advance()
+        self.advance_lexer()
         if value == "true":
             return BooleanValueNode(value=True, loc=self.loc(token))
         if value == "false":
             return BooleanValueNode(value=False, loc=self.loc(token))
         if value == "null":
             return NullValueNode(loc=self.loc(token))
         return EnumValueNode(value=value, loc=self.loc(token))
@@ -1022,15 +1104,15 @@
         """Expect the next token to be of the given kind.
 
         If the next token is of the given kind, return that token after advancing the
         lexer. Otherwise, do not change the parser state and throw an error.
         """
         token = self._lexer.token
         if token.kind == kind:
-            self._lexer.advance()
+            self.advance_lexer()
             return token
 
         raise GraphQLSyntaxError(
             self._lexer.source,
             token.start,
             f"Expected {get_token_kind_desc(kind)}, found {get_token_desc(token)}.",
         )
@@ -1039,28 +1121,28 @@
         """Expect the next token optionally to be of the given kind.
 
         If the next token is of the given kind, return True after advancing the lexer.
         Otherwise, do not change the parser state and return False.
         """
         token = self._lexer.token
         if token.kind == kind:
-            self._lexer.advance()
+            self.advance_lexer()
             return True
 
         return False
 
     def expect_keyword(self, value: str) -> None:
         """Expect the next token to be a given keyword.
 
         If the next token is a given keyword, advance the lexer.
         Otherwise, do not change the parser state and throw an error.
         """
         token = self._lexer.token
         if token.kind == TokenKind.NAME and token.value == value:
-            self._lexer.advance()
+            self.advance_lexer()
         else:
             raise GraphQLSyntaxError(
                 self._lexer.source,
                 token.start,
                 f"Expected '{value}', found {get_token_desc(token)}.",
             )
 
@@ -1068,15 +1150,15 @@
         """Expect the next token optionally to be a given keyword.
 
         If the next token is a given keyword, return True after advancing the lexer.
         Otherwise, do not change the parser state and return False.
         """
         token = self._lexer.token
         if token.kind == TokenKind.NAME and token.value == value:
-            self._lexer.advance()
+            self.advance_lexer()
             return True
 
         return False
 
     def unexpected(self, at_token: Optional[Token] = None) -> GraphQLError:
         """Create an error when an unexpected lexed token is encountered."""
         token = at_token or self._lexer.token
@@ -1156,14 +1238,28 @@
         append = nodes.append
         while True:
             append(parse_fn())
             if not expect_optional_token():
                 break
         return nodes
 
+    def advance_lexer(self) -> None:
+        """Advance the lexer."""
+        token = self._lexer.advance()
+        max_tokens = self._max_tokens
+        if max_tokens is not None and token.kind is not TokenKind.EOF:
+            self._token_counter += 1
+            if self._token_counter > max_tokens:
+                raise GraphQLSyntaxError(
+                    self._lexer.source,
+                    token.start,
+                    f"Document contains more that {max_tokens} tokens."
+                    " Parsing aborted.",
+                )
+
 
 def get_token_desc(token: Token) -> str:
     """Describe a token as a string for debugging."""
     value = token.value
     return get_token_kind_desc(token.kind) + (
         f" '{value}'" if value is not None else ""
     )
```

### Comparing `graphql_core-3.3.0a2/src/graphql/language/predicates.py` & `graphql_core-3.3.0a3/src/graphql/language/predicates.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Union
 
 from .ast import (
     DefinitionNode,
     ExecutableDefinitionNode,
     ListValueNode,
     Node,
+    NullabilityAssertionNode,
     ObjectValueNode,
     SchemaExtensionNode,
     SelectionNode,
     TypeDefinitionNode,
     TypeExtensionNode,
     TypeNode,
     TypeSystemDefinitionNode,
@@ -22,14 +23,15 @@
 except ImportError:  # Python < 3.10
     from typing_extensions import TypeGuard
 
 
 __all__ = [
     "is_definition_node",
     "is_executable_definition_node",
+    "is_nullability_assertion_node",
     "is_selection_node",
     "is_value_node",
     "is_const_value_node",
     "is_type_node",
     "is_type_system_definition_node",
     "is_type_definition_node",
     "is_type_system_extension_node",
@@ -48,14 +50,19 @@
 
 
 def is_selection_node(node: Node) -> TypeGuard[SelectionNode]:
     """Check whether the given node represents a selection."""
     return isinstance(node, SelectionNode)
 
 
+def is_nullability_assertion_node(node: Node) -> TypeGuard[NullabilityAssertionNode]:
+    """Check whether the given node represents a nullability assertion node."""
+    return isinstance(node, NullabilityAssertionNode)
+
+
 def is_value_node(node: Node) -> TypeGuard[ValueNode]:
     """Check whether the given node represents a value."""
     return isinstance(node, ValueNode)
 
 
 def is_const_value_node(node: Node) -> TypeGuard[ValueNode]:
     """Check whether the given node represents a constant value."""
```

### Comparing `graphql_core-3.3.0a2/src/graphql/language/print_location.py` & `graphql_core-3.3.0a3/src/graphql/language/print_location.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/language/print_string.py` & `graphql_core-3.3.0a3/src/graphql/language/print_string.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/language/printer.py` & `graphql_core-3.3.0a3/src/graphql/language/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     definitions: Strings
     description: str
     directives: str
     fields: Strings
     interfaces: Strings
     locations: Strings
     name: str
+    nullability_assertion: str
     operation: OperationType
     operation_types: Strings
     repeatable: bool
     selection_set: str
     selections: Strings
     type: str
     type_condition: str
@@ -96,26 +97,49 @@
 
     @staticmethod
     def leave_selection_set(node: PrintedNode, *_args: Any) -> str:
         return block(node.selections)
 
     @staticmethod
     def leave_field(node: PrintedNode, *_args: Any) -> str:
-        prefix = wrap("", node.alias, ": ") + node.name
+        prefix = join((wrap("", node.alias, ": "), node.name))
         args_line = prefix + wrap("(", join(node.arguments, ", "), ")")
 
         if len(args_line) > MAX_LINE_LENGTH:
             args_line = prefix + wrap("(\n", indent(join(node.arguments, "\n")), "\n)")
 
-        return join((args_line, join(node.directives, " "), node.selection_set), " ")
+        return join(
+            (
+                args_line,
+                #  Note: Client Controlled Nullability is experimental and may be
+                #  changed or removed in the future.
+                node.nullability_assertion,
+                wrap(" ", join(node.directives, " ")),
+                wrap(" ", node.selection_set),
+            ),
+        )
 
     @staticmethod
     def leave_argument(node: PrintedNode, *_args: Any) -> str:
         return f"{node.name}: {node.value}"
 
+    # Nullability Modifiers
+
+    @staticmethod
+    def leave_list_nullability_operator(node: PrintedNode, *_args: Any) -> str:
+        return join(("[", node.nullability_assertion, "]"))
+
+    @staticmethod
+    def leave_non_null_assertion(node: PrintedNode, *_args: Any) -> str:
+        return join((node.nullability_assertion, "!"))
+
+    @staticmethod
+    def leave_error_boundary(node: PrintedNode, *_args: Any) -> str:
+        return join((node.nullability_assertion, "?"))
+
     # Fragments
 
     @staticmethod
     def leave_fragment_spread(node: PrintedNode, *_args: Any) -> str:
         return f"...{node.name}{wrap(' ', join(node.directives, ' '))}"
 
     @staticmethod
```

### Comparing `graphql_core-3.3.0a2/src/graphql/language/source.py` & `graphql_core-3.3.0a3/src/graphql/language/source.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/language/token_kind.py` & `graphql_core-3.3.0a3/src/graphql/language/token_kind.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 class TokenKind(Enum):
     """The different kinds of tokens that the lexer emits"""
 
     SOF = "<SOF>"
     EOF = "<EOF>"
     BANG = "!"
+    QUESTION_MARK = "?"
     DOLLAR = "$"
     AMP = "&"
     PAREN_L = "("
     PAREN_R = ")"
     SPREAD = "..."
     COLON = ":"
     EQUALS = "="
```

### Comparing `graphql_core-3.3.0a2/src/graphql/language/visitor.py` & `graphql_core-3.3.0a3/src/graphql/language/visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     BREAK = True
     SKIP = False
     REMOVE = Ellipsis
 
 
 VisitorAction: TypeAlias = Optional[VisitorActionEnum]
 
-# Note that in GraphQL.js these are defined differently:
+# Note that in GraphQL.js these are defined *differently*:
 # BREAK = {}, SKIP = false, REMOVE = null, IDLE = undefined
 
 BREAK = VisitorActionEnum.BREAK
 SKIP = VisitorActionEnum.SKIP
 REMOVE = VisitorActionEnum.REMOVE
 IDLE = None
 
@@ -99,15 +99,15 @@
     :arg path: The key path to get to this node from the root node.
     :arg ancestors: All nodes and Arrays visited before reaching parent
         of this node. These correspond to array indices in ``path``.
         Note: ancestors includes arrays which contain the parent of visited node.
 
     You can also define node kind specific methods by suffixing them with an underscore
     followed by the kind of the node to be visited. For instance, to visit ``field``
-    nodes, you would defined the methods ``enter_field()`` and/or ``leave_field()``,
+    nodes, you would define the methods ``enter_field()`` and/or ``leave_field()``,
     with the same signature as above. If no kind specific method has been defined
     for a given node, the generic method is called.
     """
 
     # Provide special return values as attributes
     BREAK, SKIP, REMOVE, IDLE = BREAK, SKIP, REMOVE, IDLE
 
@@ -360,13 +360,12 @@
                                 ):
                                     return result
                         elif skipping[i] is node:
                             skipping[i] = None
                     return None
 
             else:
-
                 enter = leave = None
 
             enter_leave = EnterLeaveVisitor(enter, leave)
             self.enter_leave_map[kind] = enter_leave
             return enter_leave
```

### Comparing `graphql_core-3.3.0a2/src/graphql/pyutils/__init__.py` & `graphql_core-3.3.0a3/src/graphql/pyutils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 codebase.
 
 Each utility should belong in its own file and be the default export.
 
 These functions are not part of the module interface and are subject to change.
 """
 
+from .async_reduce import async_reduce
 from .convert_case import camel_to_snake, snake_to_camel
 from .cached_property import cached_property
 from .description import (
     Description,
     is_description,
     register_description,
     unregister_description,
@@ -30,14 +31,15 @@
 from .merge_kwargs import merge_kwargs
 from .path import Path
 from .print_path_list import print_path_list
 from .simple_pub_sub import SimplePubSub, SimplePubSubIterator
 from .undefined import Undefined, UndefinedType
 
 __all__ = [
+    "async_reduce",
     "camel_to_snake",
     "snake_to_camel",
     "cached_property",
     "did_you_mean",
     "or_list",
     "and_list",
     "Description",
```

### Comparing `graphql_core-3.3.0a2/src/graphql/pyutils/cached_property.py` & `graphql_core-3.3.0a3/src/graphql/pyutils/cached_property.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/pyutils/convert_case.py` & `graphql_core-3.3.0a3/src/graphql/pyutils/convert_case.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/pyutils/description.py` & `graphql_core-3.3.0a3/src/graphql/pyutils/description.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/pyutils/did_you_mean.py` & `graphql_core-3.3.0a3/src/graphql/pyutils/did_you_mean.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/pyutils/format_list.py` & `graphql_core-3.3.0a3/src/graphql/pyutils/format_list.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/pyutils/inspect.py` & `graphql_core-3.3.0a3/src/graphql/pyutils/inspect.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/pyutils/is_awaitable.py` & `graphql_core-3.3.0a3/src/graphql/pyutils/is_awaitable.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 __all__ = ["is_awaitable"]
 
 CO_ITERABLE_COROUTINE = inspect.CO_ITERABLE_COROUTINE
 
 
 def is_awaitable(value: Any) -> TypeGuard[Awaitable]:
-    """Return true if object can be passed to an ``await`` expression.
+    """Return True if object can be passed to an ``await`` expression.
 
-    Instead of testing if the object is an instance of abc.Awaitable, it checks
-    the existence of an `__await__` attribute. This is much faster.
+    Instead of testing whether the object is an instance of abc.Awaitable, we
+    check the existence of an `__await__` attribute. This is much faster.
     """
     return (
         # check for coroutine objects
         isinstance(value, CoroutineType)
         # check for old-style generator based coroutine objects
         or isinstance(value, GeneratorType)  # for Python < 3.11
         and bool(value.gi_code.co_flags & CO_ITERABLE_COROUTINE)
```

### Comparing `graphql_core-3.3.0a2/src/graphql/pyutils/is_iterable.py` & `graphql_core-3.3.0a3/src/graphql/pyutils/is_iterable.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/pyutils/path.py` & `graphql_core-3.3.0a3/src/graphql/pyutils/path.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/pyutils/simple_pub_sub.py` & `graphql_core-3.3.0a3/src/graphql/pyutils/simple_pub_sub.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations  # Python < 3.10
 
-from asyncio import Future, Queue, ensure_future, get_running_loop, sleep
-from inspect import isawaitable
+from asyncio import Future, Queue, create_task, get_running_loop, sleep
 from typing import Any, AsyncIterator, Callable, Optional, Set
 
+from .is_awaitable import is_awaitable
+
 
 __all__ = ["SimplePubSub", "SimplePubSubIterator"]
 
 
 class SimplePubSub:
     """A very simple publish-subscript system.
 
@@ -21,16 +22,16 @@
     def __init__(self) -> None:
         self.subscribers = set()
 
     def emit(self, event: Any) -> bool:
         """Emit an event."""
         for subscriber in self.subscribers:
             result = subscriber(event)
-            if isawaitable(result):
-                ensure_future(result)
+            if is_awaitable(result):
+                create_task(result)  # type: ignore
         return bool(self.subscribers)
 
     def get_subscriber(
         self, transform: Optional[Callable] = None
     ) -> SimplePubSubIterator:
         return SimplePubSubIterator(self, transform)
```

### Comparing `graphql_core-3.3.0a2/src/graphql/pyutils/suggestion_list.py` & `graphql_core-3.3.0a3/src/graphql/pyutils/suggestion_list.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/type/__init__.py` & `graphql_core-3.3.0a3/src/graphql/type/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     GraphQLArgumentMap,
     GraphQLEnumValue,
     GraphQLEnumValueMap,
     GraphQLField,
     GraphQLFieldMap,
     GraphQLInputField,
     GraphQLInputFieldMap,
+    GraphQLInputFieldOutType,
     GraphQLScalarSerializer,
     GraphQLScalarValueParser,
     GraphQLScalarLiteralParser,
     # Keyword Args
     GraphQLArgumentKwargs,
     GraphQLEnumTypeKwargs,
     GraphQLEnumValueKwargs,
@@ -128,14 +129,16 @@
     # Directives Definition
     GraphQLDirective,
     # Built-in Directives defined by the Spec
     is_specified_directive,
     specified_directives,
     GraphQLIncludeDirective,
     GraphQLSkipDirective,
+    GraphQLDeferDirective,
+    GraphQLStreamDirective,
     GraphQLDeprecatedDirective,
     GraphQLSpecifiedByDirective,
     # Keyword Args
     GraphQLDirectiveKwargs,
     # Constant Deprecation Reason
     DEFAULT_DEPRECATION_REASON,
 )
@@ -248,14 +251,15 @@
     "GraphQLArgumentMap",
     "GraphQLEnumValue",
     "GraphQLEnumValueMap",
     "GraphQLField",
     "GraphQLFieldMap",
     "GraphQLInputField",
     "GraphQLInputFieldMap",
+    "GraphQLInputFieldOutType",
     "GraphQLScalarSerializer",
     "GraphQLScalarValueParser",
     "GraphQLScalarLiteralParser",
     "GraphQLArgumentKwargs",
     "GraphQLEnumTypeKwargs",
     "GraphQLEnumValueKwargs",
     "GraphQLFieldKwargs",
@@ -274,14 +278,16 @@
     "is_directive",
     "assert_directive",
     "is_specified_directive",
     "specified_directives",
     "GraphQLDirective",
     "GraphQLIncludeDirective",
     "GraphQLSkipDirective",
+    "GraphQLDeferDirective",
+    "GraphQLStreamDirective",
     "GraphQLDeprecatedDirective",
     "GraphQLSpecifiedByDirective",
     "GraphQLDirectiveKwargs",
     "DEFAULT_DEPRECATION_REASON",
     "is_specified_scalar_type",
     "specified_scalar_types",
     "GraphQLInt",
```

### Comparing `graphql_core-3.3.0a2/src/graphql/type/assert_name.py` & `graphql_core-3.3.0a3/src/graphql/type/assert_name.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/type/directives.py` & `graphql_core-3.3.0a3/src/graphql/type/directives.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations  # Python < 3.10
 
 from typing import Any, Collection, Dict, Optional, Tuple, cast
 
 from ..language import DirectiveLocation, ast
-from ..pyutils import inspect, is_description
+from ..pyutils import inspect
 from .assert_name import assert_name
-from .definition import GraphQLArgument, GraphQLInputType, GraphQLNonNull, is_input_type
-from .scalars import GraphQLBoolean, GraphQLString
+from .definition import GraphQLArgument, GraphQLInputType, GraphQLNonNull
+from .scalars import GraphQLBoolean, GraphQLInt, GraphQLString
 
 
 try:
     from typing import TypedDict
 except ImportError:  # Python < 3.8
     from typing_extensions import TypedDict
 try:
@@ -19,18 +19,20 @@
     from typing_extensions import TypeGuard
 
 __all__ = [
     "is_directive",
     "assert_directive",
     "is_specified_directive",
     "specified_directives",
+    "GraphQLDeferDirective",
     "GraphQLDirective",
     "GraphQLDirectiveKwargs",
     "GraphQLIncludeDirective",
     "GraphQLSkipDirective",
+    "GraphQLStreamDirective",
     "GraphQLDeprecatedDirective",
     "GraphQLSpecifiedByDirective",
     "DirectiveLocation",
     "DEFAULT_DEPRECATION_REASON",
 ]
 
 
@@ -78,52 +80,29 @@
                 for value in locations
             )
         except (KeyError, TypeError):
             raise TypeError(
                 f"{name} locations must be specified"
                 " as a collection of DirectiveLocation enum values."
             )
-        if args is None:
-            args = {}
-        elif not isinstance(args, dict) or not all(
-            isinstance(key, str) for key in args
-        ):
-            raise TypeError(f"{name} args must be a dict with argument names as keys.")
-        elif not all(
-            isinstance(value, GraphQLArgument) or is_input_type(value)
-            for value in args.values()
-        ):
-            raise TypeError(
-                f"{name} args must be GraphQLArgument or input type objects."
-            )
-        else:
+        if args:
             args = {
                 assert_name(name): value
                 if isinstance(value, GraphQLArgument)
                 else GraphQLArgument(cast(GraphQLInputType, value))
                 for name, value in args.items()
             }
-        if not isinstance(is_repeatable, bool):
-            raise TypeError(f"{name} is_repeatable flag must be True or False.")
-        if ast_node and not isinstance(ast_node, ast.DirectiveDefinitionNode):
-            raise TypeError(f"{name} AST node must be a DirectiveDefinitionNode.")
-        if description is not None and not is_description(description):
-            raise TypeError(f"{name} description must be a string.")
-        if extensions is None:
-            extensions = {}
-        elif not isinstance(extensions, dict) or not all(
-            isinstance(key, str) for key in extensions
-        ):
-            raise TypeError(f"{name} extensions must be a dictionary with string keys.")
+        else:
+            args = {}
         self.name = name
         self.locations = locations
         self.args = args
         self.is_repeatable = is_repeatable
         self.description = description
-        self.extensions = extensions
+        self.extensions = extensions or {}
         self.ast_node = ast_node
 
     def __str__(self) -> str:
         return f"@{self.name}"
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}({self})>"
@@ -196,14 +175,51 @@
             GraphQLNonNull(GraphQLBoolean), description="Skipped when true."
         )
     },
     description="Directs the executor to skip this field or fragment"
     " when the `if` argument is true.",
 )
 
+# Used to conditionally defer fragments:
+GraphQLDeferDirective = GraphQLDirective(
+    name="defer",
+    description="Directs the executor to defer this fragment"
+    " when the `if` argument is true or undefined.",
+    locations=[DirectiveLocation.FRAGMENT_SPREAD, DirectiveLocation.INLINE_FRAGMENT],
+    args={
+        "if": GraphQLArgument(
+            GraphQLNonNull(GraphQLBoolean),
+            description="Deferred when true or undefined.",
+            default_value=True,
+        ),
+        "label": GraphQLArgument(GraphQLString, description="Unique name"),
+    },
+)
+
+# Used to conditionally stream list fields:
+GraphQLStreamDirective = GraphQLDirective(
+    name="stream",
+    description="Directs the executor to stream plural fields"
+    " when the `if` argument is true or undefined.",
+    locations=[DirectiveLocation.FIELD],
+    args={
+        "if": GraphQLArgument(
+            GraphQLNonNull(GraphQLBoolean),
+            description="Stream when true or undefined.",
+            default_value=True,
+        ),
+        "label": GraphQLArgument(GraphQLString, description="Unique name"),
+        "initialCount": GraphQLArgument(
+            GraphQLInt,
+            description="Number of items to return immediately",
+            default_value=0,
+        ),
+    },
+)
+
 
 # Constant string used for default reason for a deprecation:
 DEFAULT_DEPRECATION_REASON = "No longer supported"
 
 # Used to declare element of a GraphQL schema as deprecated:
 GraphQLDeprecatedDirective = GraphQLDirective(
     name="deprecated",
```

### Comparing `graphql_core-3.3.0a2/src/graphql/type/introspection.py` & `graphql_core-3.3.0a3/src/graphql/type/introspection.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/type/scalars.py` & `graphql_core-3.3.0a3/src/graphql/type/scalars.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/type/schema.py` & `graphql_core-3.3.0a3/src/graphql/type/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations  # Python < 3.10
 
 from copy import copy, deepcopy
 from typing import Any, Collection, Dict, List, NamedTuple, Optional, Set, Tuple, cast
 
 from ..error import GraphQLError
 from ..language import OperationType, ast
-from ..pyutils import inspect, is_collection, is_description
+from ..pyutils import inspect
 from .definition import (
     GraphQLAbstractType,
     GraphQLCompositeType,
     GraphQLField,
     GraphQLInterfaceType,
     GraphQLNamedType,
     GraphQLObjectType,
@@ -43,15 +43,14 @@
 __all__ = ["GraphQLSchema", "GraphQLSchemaKwargs", "is_schema", "assert_schema"]
 
 
 TypeMap: TypeAlias = Dict[str, GraphQLNamedType]
 
 
 class InterfaceImplementations(NamedTuple):
-
     objects: List[GraphQLObjectType]
     interfaces: List[GraphQLInterfaceType]
 
 
 class GraphQLSchemaKwargs(TypedDict, total=False):
     query: Optional[GraphQLObjectType]
     mutation: Optional[GraphQLObjectType]
@@ -145,70 +144,27 @@
         """Initialize GraphQL schema.
 
         If this schema was built from a source known to be valid, then it may be marked
         with ``assume_valid`` to avoid an additional type system validation.
         """
         self._validation_errors = [] if assume_valid else None
 
-        # Check for common mistakes during construction to produce clear and early
-        # error messages, but we leave the specific tests for the validation.
-        if query and not isinstance(query, GraphQLType):
-            raise TypeError("Expected query to be a GraphQL type.")
-        if mutation and not isinstance(mutation, GraphQLType):
-            raise TypeError("Expected mutation to be a GraphQL type.")
-        if subscription and not isinstance(subscription, GraphQLType):
-            raise TypeError("Expected subscription to be a GraphQL type.")
-        if types is None:
-            types = []
-        else:
-            if not is_collection(types) or not all(
-                isinstance(type_, GraphQLType) for type_ in types
-            ):
-                raise TypeError(
-                    "Schema types must be specified as a collection of GraphQL types."
-                )
-        if directives is not None:
-            # noinspection PyUnresolvedReferences
-            if not is_collection(directives):
-                raise TypeError("Schema directives must be a collection.")
-            if not isinstance(directives, tuple):
-                directives = tuple(directives)
-        if description is not None and not is_description(description):
-            raise TypeError("Schema description must be a string.")
-        if extensions is None:
-            extensions = {}
-        elif not isinstance(extensions, dict) or not all(
-            isinstance(key, str) for key in extensions
-        ):
-            raise TypeError("Schema extensions must be a dictionary with string keys.")
-        if ast_node and not isinstance(ast_node, ast.SchemaDefinitionNode):
-            raise TypeError("Schema AST node must be a SchemaDefinitionNode.")
-        if extension_ast_nodes:
-            if not is_collection(extension_ast_nodes) or not all(
-                isinstance(node, ast.SchemaExtensionNode)
-                for node in extension_ast_nodes
-            ):
-                raise TypeError(
-                    "Schema extension AST nodes must be specified"
-                    " as a collection of SchemaExtensionNode instances."
-                )
-            if not isinstance(extension_ast_nodes, tuple):
-                extension_ast_nodes = tuple(extension_ast_nodes)
-        else:
-            extension_ast_nodes = ()
-
         self.description = description
-        self.extensions = extensions
+        self.extensions = extensions or {}
         self.ast_node = ast_node
-        self.extension_ast_nodes = extension_ast_nodes
+        self.extension_ast_nodes = (
+            tuple(extension_ast_nodes) if extension_ast_nodes else ()
+        )
         self.query_type = query
         self.mutation_type = mutation
         self.subscription_type = subscription
         # Provide specified directives (e.g. @include and @skip) by default
-        self.directives = specified_directives if directives is None else directives
+        self.directives = (
+            specified_directives if directives is None else tuple(directives)
+        )
 
         # To preserve order of user-provided types, we first add them to the set
         # of "collected" types, so `collect_referenced_types` ignores them.
         if types:
             all_referenced_types = TypeSet.with_initial_types(types)
             collect_referenced_types = all_referenced_types.collect_referenced_types
             for type_ in types:
```

### Comparing `graphql_core-3.3.0a2/src/graphql/type/validate.py` & `graphql_core-3.3.0a3/src/graphql/type/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
     # First check to ensure the provided value is in fact a GraphQLSchema.
     assert_schema(schema)
 
     # If this Schema has already been validated, return the previous results.
     # noinspection PyProtectedMember
     errors = schema._validation_errors
     if errors is None:
-
         # Validate the schema, producing a list of errors.
         context = SchemaValidationContext(schema)
         context.validate_root_types()
         context.validate_directives()
         context.validate_types()
 
         # Persist the results of validation before returning to ensure validation does
@@ -192,15 +191,14 @@
                     " which is reserved by GraphQL introspection.",
                     ast_node,
                 )
 
     def validate_types(self) -> None:
         validate_input_object_circular_refs = InputObjectCircularRefsValidator(self)
         for type_ in self.schema.type_map.values():
-
             # Ensure all provided types are in fact GraphQL type.
             if not is_named_type(type_):
                 self.report_error(
                     f"Expected GraphQL named type but got: {inspect(type_)}.",
                     type_.ast_node if is_named_type(type_) else None,
                 )
                 continue
@@ -243,15 +241,14 @@
         if not fields:
             self.report_error(
                 f"Type {type_.name} must define one or more fields.",
                 [type_.ast_node, *type_.extension_ast_nodes],
             )
 
         for field_name, field in fields.items():
-
             # Ensure they are named correctly.
             self.validate_name(field, field_name)
 
             # Ensure the type is an output type
             if not is_output_type(field.type):
                 self.report_error(
                     f"The type of {type_.name}.{field_name}"
@@ -459,15 +456,14 @@
                 f"Input Object type {input_obj.name}"
                 " must define one or more fields.",
                 [input_obj.ast_node, *input_obj.extension_ast_nodes],
             )
 
         # Ensure the arguments are valid
         for field_name, field in fields.items():
-
             # Ensure they are named correctly.
             self.validate_name(field, field_name)
 
             # Ensure the type is an input type.
             if not is_input_type(field.type):
                 self.report_error(
                     f"The type of {input_obj.name}.{field_name}"
```

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/__init__.py` & `graphql_core-3.3.0a3/src/graphql/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/ast_from_value.py` & `graphql_core-3.3.0a3/src/graphql/utilities/ast_from_value.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/ast_to_dict.py` & `graphql_core-3.3.0a3/src/graphql/utilities/ast_to_dict.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/build_ast_schema.py` & `graphql_core-3.3.0a3/src/graphql/utilities/build_ast_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,17 +33,14 @@
     resolve methods, so execution will use default resolvers.
 
     When building a schema from a GraphQL service's introspection result, it might
     be safe to assume the schema is valid. Set ``assume_valid`` to ``True`` to assume
     the produced schema is valid. Set ``assume_valid_sdl`` to ``True`` to assume it is
     already a valid SDL document.
     """
-    if not isinstance(document_ast, DocumentNode):
-        raise TypeError("Must provide valid Document AST.")
-
     if not (assume_valid or assume_valid_sdl):
         from ..validation.validate import assert_valid_sdl
 
         assert_valid_sdl(document_ast)
 
     empty_schema_kwargs = GraphQLSchemaKwargs(
         query=None,
```

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/build_client_schema.py` & `graphql_core-3.3.0a3/src/graphql/utilities/build_client_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     but cannot be used to execute a query, as introspection does not represent the
     "resolver", "parse" or "serialize" functions or any other server-internal
     mechanisms.
 
     This function expects a complete introspection result. Don't forget to check the
     "errors" field of a server response before calling this function.
     """
+    # Even though the `introspection` argument is typed, in most cases it's received
+    # as an untyped value from the server, so we will do an additional check here.
     if not isinstance(introspection, dict) or not isinstance(
         introspection.get("__schema"), dict
     ):
         raise TypeError(
             "Invalid or incomplete introspection result. Ensure that you"
             " are passing the 'data' attribute of an introspection response"
             f" and no 'errors' were returned alongside: {inspect(introspection)}."
```

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/coerce_input_value.py` & `graphql_core-3.3.0a3/src/graphql/utilities/coerce_input_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,16 +126,17 @@
                         f"Field '{field_name}' is not defined by type '{type_.name}'."
                         + did_you_mean(suggestions)
                     ),
                 )
         return type_.out_type(coerced_dict)
 
     if is_leaf_type(type_):
-        # Scalars determine if a value is valid via `parse_value()`, which can throw to
-        # indicate failure. If it throws, maintain a reference to the original error.
+        # Scalars and Enums determine if an input value is valid via `parse_value()`,
+        # which can throw to indicate failure. If it throws, maintain a reference
+        # to the original error.
         type_ = cast(GraphQLScalarType, type_)
         try:
             parse_result = type_.parse_value(input_value)
         except GraphQLError as error:
             on_error(path.as_list() if path else [], input_value, error)
             return Undefined
         except Exception as error:
```

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/concat_ast.py` & `graphql_core-3.3.0a3/src/graphql/utilities/concat_ast.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/extend_schema.py` & `graphql_core-3.3.0a3/src/graphql/utilities/extend_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Collection,
     DefaultDict,
     Dict,
     List,
     Mapping,
     Optional,
     Tuple,
+    TypeVar,
     Union,
     cast,
 )
 
 from ..language import (
     DirectiveDefinitionNode,
     DirectiveLocation,
@@ -115,97 +116,122 @@
     When extending a schema with a known valid extension, it might be safe to assume the
     schema is valid. Set ``assume_valid`` to ``True`` to assume the produced schema is
     valid. Set ``assume_valid_sdl`` to ``True`` to assume it is already a valid SDL
     document.
     """
     assert_schema(schema)
 
-    if not isinstance(document_ast, DocumentNode):
-        raise TypeError("Must provide valid Document AST.")
-
     if not (assume_valid or assume_valid_sdl):
         from ..validation.validate import assert_valid_sdl_extension
 
         assert_valid_sdl_extension(document_ast, schema)
 
     schema_kwargs = schema.to_kwargs()
     extended_kwargs = ExtendSchemaImpl.extend_schema_args(
         schema_kwargs, document_ast, assume_valid
     )
     return (
         schema if schema_kwargs is extended_kwargs else GraphQLSchema(**extended_kwargs)
     )
 
 
+TEN = TypeVar("TEN", bound=TypeExtensionNode)
+
+
+class TypeExtensionsMap:
+    """Mappings from types to their extensions."""
+
+    scalar: DefaultDict[str, List[ScalarTypeExtensionNode]]
+    object: DefaultDict[str, List[ObjectTypeExtensionNode]]
+    interface: DefaultDict[str, List[InterfaceTypeExtensionNode]]
+    union: DefaultDict[str, List[UnionTypeExtensionNode]]
+    enum: DefaultDict[str, List[EnumTypeExtensionNode]]
+    input_object: DefaultDict[str, List[InputObjectTypeExtensionNode]]
+
+    def __init__(self) -> None:
+        self.scalar = defaultdict(list)
+        self.object = defaultdict(list)
+        self.interface = defaultdict(list)
+        self.union = defaultdict(list)
+        self.enum = defaultdict(list)
+        self.input_object = defaultdict(list)
+
+    def for_node(self, node: TEN) -> DefaultDict[str, List[TEN]]:
+        """Get type extensions map for the given node kind."""
+        kind = node.kind
+        try:
+            kind = kind.removesuffix("_type_extension")
+        except AttributeError:  # pragma: no cover (Python < 3.9)
+            if kind.endswith("_type_extension"):
+                kind = kind[:-15]
+        return getattr(self, kind)
+
+
 class ExtendSchemaImpl:
     """Helper class implementing the methods to extend a schema.
 
     Note: We use a class instead of an implementation with local functions
     and lambda functions so that the extended schema can be pickled.
 
     For internal use only.
     """
 
     type_map: Dict[str, GraphQLNamedType]
-    type_extensions_map: Dict[str, Any]
+    type_extensions: TypeExtensionsMap
 
-    def __init__(self, type_extensions_map: Dict[str, Any]):
+    def __init__(self, type_extensions: TypeExtensionsMap):
         self.type_map = {}
-        self.type_extensions_map = type_extensions_map
+        self.type_extensions = type_extensions
 
     @classmethod
     def extend_schema_args(
         cls,
         schema_kwargs: GraphQLSchemaKwargs,
         document_ast: DocumentNode,
         assume_valid: bool = False,
     ) -> GraphQLSchemaKwargs:
         """Extend the given schema arguments with extensions from a given document.
 
         For internal use only.
         """
-        # Note: schema_kwargs should become a TypedDict once we require Python 3.8
-
         # Collect the type definitions and extensions found in the document.
         type_defs: List[TypeDefinitionNode] = []
-        type_extensions_map: DefaultDict[str, Any] = defaultdict(list)
+
+        type_extensions = TypeExtensionsMap()
 
         # New directives and types are separate because a directives and types can have
         # the same name. For example, a type named "skip".
         directive_defs: List[DirectiveDefinitionNode] = []
 
         schema_def: Optional[SchemaDefinitionNode] = None
         # Schema extensions are collected which may add additional operation types.
         schema_extensions: List[SchemaExtensionNode] = []
 
+        is_schema_changed = False
         for def_ in document_ast.definitions:
             if isinstance(def_, SchemaDefinitionNode):
                 schema_def = def_
             elif isinstance(def_, SchemaExtensionNode):
                 schema_extensions.append(def_)
+            elif isinstance(def_, DirectiveDefinitionNode):
+                directive_defs.append(def_)
             elif isinstance(def_, TypeDefinitionNode):
                 type_defs.append(def_)
             elif isinstance(def_, TypeExtensionNode):
-                extended_type_name = def_.name.value
-                type_extensions_map[extended_type_name].append(def_)
-            elif isinstance(def_, DirectiveDefinitionNode):
-                directive_defs.append(def_)
+                type_extensions.for_node(def_)[def_.name.value].append(def_)
+            else:
+                continue
+            is_schema_changed = True
 
         # If this document contains no new types, extensions, or directives then return
         # the same unmodified GraphQLSchema instance.
-        if (
-            not type_extensions_map
-            and not type_defs
-            and not directive_defs
-            and not schema_extensions
-            and not schema_def
-        ):
+        if not is_schema_changed:
             return schema_kwargs
 
-        self = cls(type_extensions_map)
+        self = cls(type_extensions)
         for existing_type in schema_kwargs["types"] or ():
             self.type_map[existing_type.name] = self.extend_named_type(existing_type)
         for type_node in type_defs:
             name = type_node.name.value
             self.type_map[name] = std_type_map.get(name) or self.build_type(type_node)
 
         # Get the extended root operation types.
@@ -310,41 +336,41 @@
 
     # noinspection PyShadowingNames
     def extend_input_object_type(
         self,
         type_: GraphQLInputObjectType,
     ) -> GraphQLInputObjectType:
         kwargs = type_.to_kwargs()
-        extensions = tuple(self.type_extensions_map[kwargs["name"]])
+        extensions = tuple(self.type_extensions.input_object[kwargs["name"]])
 
         return GraphQLInputObjectType(
             **merge_kwargs(
                 kwargs,
                 fields=partial(
                     self.extend_input_object_type_fields, kwargs, extensions
                 ),
                 extension_ast_nodes=kwargs["extension_ast_nodes"] + extensions,
             )
         )
 
     def extend_enum_type(self, type_: GraphQLEnumType) -> GraphQLEnumType:
         kwargs = type_.to_kwargs()
-        extensions = tuple(self.type_extensions_map[kwargs["name"]])
+        extensions = tuple(self.type_extensions.enum[kwargs["name"]])
 
         return GraphQLEnumType(
             **merge_kwargs(
                 kwargs,
                 values={**kwargs["values"], **self.build_enum_value_map(extensions)},
                 extension_ast_nodes=kwargs["extension_ast_nodes"] + extensions,
             )
         )
 
     def extend_scalar_type(self, type_: GraphQLScalarType) -> GraphQLScalarType:
         kwargs = type_.to_kwargs()
-        extensions = tuple(self.type_extensions_map[kwargs["name"]])
+        extensions = tuple(self.type_extensions.scalar[kwargs["name"]])
 
         specified_by_url = kwargs["specified_by_url"]
         for extension_node in extensions:
             specified_by_url = get_specified_by_url(extension_node) or specified_by_url
 
         return GraphQLScalarType(
             **merge_kwargs(
@@ -372,15 +398,15 @@
             },
             **self.build_field_map(extensions),
         }
 
     # noinspection PyShadowingNames
     def extend_object_type(self, type_: GraphQLObjectType) -> GraphQLObjectType:
         kwargs = type_.to_kwargs()
-        extensions = tuple(self.type_extensions_map[kwargs["name"]])
+        extensions = tuple(self.type_extensions.object[kwargs["name"]])
 
         return GraphQLObjectType(
             **merge_kwargs(
                 kwargs,
                 interfaces=partial(
                     self.extend_object_type_interfaces, kwargs, extensions
                 ),
@@ -409,15 +435,15 @@
         }
 
     # noinspection PyShadowingNames
     def extend_interface_type(
         self, type_: GraphQLInterfaceType
     ) -> GraphQLInterfaceType:
         kwargs = type_.to_kwargs()
-        extensions = tuple(self.type_extensions_map[kwargs["name"]])
+        extensions = tuple(self.type_extensions.interface[kwargs["name"]])
 
         return GraphQLInterfaceType(
             **merge_kwargs(
                 kwargs,
                 interfaces=partial(
                     self.extend_interface_type_interfaces, kwargs, extensions
                 ),
@@ -432,15 +458,15 @@
         return [
             cast(GraphQLObjectType, self.replace_named_type(member_type))
             for member_type in kwargs["types"]
         ] + self.build_union_types(extensions)
 
     def extend_union_type(self, type_: GraphQLUnionType) -> GraphQLUnionType:
         kwargs = type_.to_kwargs()
-        extensions = tuple(self.type_extensions_map[kwargs["name"]])
+        extensions = tuple(self.type_extensions.union[kwargs["name"]])
 
         return GraphQLUnionType(
             **merge_kwargs(
                 kwargs,
                 types=partial(self.extend_union_type_types, kwargs, extensions),
                 extension_ast_nodes=kwargs["extension_ast_nodes"] + extensions,
             ),
@@ -625,15 +651,15 @@
             for node in nodes
             for type_ in node.types or []
         ]
 
     def build_object_type(
         self, ast_node: ObjectTypeDefinitionNode
     ) -> GraphQLObjectType:
-        extension_nodes = self.type_extensions_map[ast_node.name.value]
+        extension_nodes = self.type_extensions.object[ast_node.name.value]
         all_nodes: List[Union[ObjectTypeDefinitionNode, ObjectTypeExtensionNode]] = [
             ast_node,
             *extension_nodes,
         ]
         return GraphQLObjectType(
             name=ast_node.name.value,
             description=ast_node.description.value if ast_node.description else None,
@@ -643,43 +669,43 @@
             extension_ast_nodes=extension_nodes,
         )
 
     def build_interface_type(
         self,
         ast_node: InterfaceTypeDefinitionNode,
     ) -> GraphQLInterfaceType:
-        extension_nodes = self.type_extensions_map[ast_node.name.value]
+        extension_nodes = self.type_extensions.interface[ast_node.name.value]
         all_nodes: List[
             Union[InterfaceTypeDefinitionNode, InterfaceTypeExtensionNode]
         ] = [ast_node, *extension_nodes]
         return GraphQLInterfaceType(
             name=ast_node.name.value,
             description=ast_node.description.value if ast_node.description else None,
             interfaces=partial(self.build_interfaces, all_nodes),
             fields=partial(self.build_field_map, all_nodes),
             ast_node=ast_node,
             extension_ast_nodes=extension_nodes,
         )
 
     def build_enum_type(self, ast_node: EnumTypeDefinitionNode) -> GraphQLEnumType:
-        extension_nodes = self.type_extensions_map[ast_node.name.value]
+        extension_nodes = self.type_extensions.enum[ast_node.name.value]
         all_nodes: List[Union[EnumTypeDefinitionNode, EnumTypeExtensionNode]] = [
             ast_node,
             *extension_nodes,
         ]
         return GraphQLEnumType(
             name=ast_node.name.value,
             description=ast_node.description.value if ast_node.description else None,
             values=self.build_enum_value_map(all_nodes),
             ast_node=ast_node,
             extension_ast_nodes=extension_nodes,
         )
 
     def build_union_type(self, ast_node: UnionTypeDefinitionNode) -> GraphQLUnionType:
-        extension_nodes = self.type_extensions_map[ast_node.name.value]
+        extension_nodes = self.type_extensions.union[ast_node.name.value]
         all_nodes: List[Union[UnionTypeDefinitionNode, UnionTypeExtensionNode]] = [
             ast_node,
             *extension_nodes,
         ]
         return GraphQLUnionType(
             name=ast_node.name.value,
             description=ast_node.description.value if ast_node.description else None,
@@ -687,28 +713,28 @@
             ast_node=ast_node,
             extension_ast_nodes=extension_nodes,
         )
 
     def build_scalar_type(
         self, ast_node: ScalarTypeDefinitionNode
     ) -> GraphQLScalarType:
-        extension_nodes = self.type_extensions_map[ast_node.name.value]
+        extension_nodes = self.type_extensions.scalar[ast_node.name.value]
         return GraphQLScalarType(
             name=ast_node.name.value,
             description=ast_node.description.value if ast_node.description else None,
             specified_by_url=get_specified_by_url(ast_node),
             ast_node=ast_node,
             extension_ast_nodes=extension_nodes,
         )
 
     def build_input_object_type(
         self,
         ast_node: InputObjectTypeDefinitionNode,
     ) -> GraphQLInputObjectType:
-        extension_nodes = self.type_extensions_map[ast_node.name.value]
+        extension_nodes = self.type_extensions.input_object[ast_node.name.value]
         all_nodes: List[
             Union[InputObjectTypeDefinitionNode, InputObjectTypeExtensionNode]
         ] = [ast_node, *extension_nodes]
         return GraphQLInputObjectType(
             name=ast_node.name.value,
             description=ast_node.description.value if ast_node.description else None,
             fields=partial(self.build_input_field_map, all_nodes),
```

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/find_breaking_changes.py` & `graphql_core-3.3.0a3/src/graphql/utilities/find_breaking_changes.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     for directive in directives_diff.removed:
         schema_changes.append(
             BreakingChange(
                 BreakingChangeType.DIRECTIVE_REMOVED, f"{directive.name} was removed."
             )
         )
 
-    for (old_directive, new_directive) in directives_diff.persisted:
+    for old_directive, new_directive in directives_diff.persisted:
         args_diff = dict_diff(old_directive.args, new_directive.args)
 
         for arg_name, new_arg in args_diff.added.items():
             if is_required_argument(new_arg):
                 schema_changes.append(
                     BreakingChange(
                         BreakingChangeType.REQUIRED_DIRECTIVE_ARG_ADDED,
@@ -502,15 +502,14 @@
     raise TypeError(f"Unexpected type {inspect(old_type)}")
 
 
 def is_change_safe_for_input_object_field_or_field_arg(
     old_type: GraphQLType, new_type: GraphQLType
 ) -> bool:
     if is_list_type(old_type):
-
         return is_list_type(
             # if they're both lists, make sure underlying types are compatible
             new_type
         ) and is_change_safe_for_input_object_field_or_field_arg(
             old_type.of_type, new_type.of_type
         )
```

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/get_introspection_query.py` & `graphql_core-3.3.0a3/src/graphql/utilities/get_introspection_query.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/get_operation_ast.py` & `graphql_core-3.3.0a3/src/graphql/utilities/get_operation_ast.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/introspection_from_schema.py` & `graphql_core-3.3.0a3/src/graphql/utilities/introspection_from_schema.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/lexicographic_sort_schema.py` & `graphql_core-3.3.0a3/src/graphql/utilities/lexicographic_sort_schema.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/print_schema.py` & `graphql_core-3.3.0a3/src/graphql/utilities/print_schema.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/separate_operations.py` & `graphql_core-3.3.0a3/src/graphql/utilities/separate_operations.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/sort_value_node.py` & `graphql_core-3.3.0a3/src/graphql/utilities/sort_value_node.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/strip_ignored_characters.py` & `graphql_core-3.3.0a3/src/graphql/utilities/strip_ignored_characters.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/type_comparators.py` & `graphql_core-3.3.0a3/src/graphql/utilities/type_comparators.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/type_from_ast.py` & `graphql_core-3.3.0a3/src/graphql/utilities/type_from_ast.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/type_info.py` & `graphql_core-3.3.0a3/src/graphql/utilities/type_info.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/value_from_ast.py` & `graphql_core-3.3.0a3/src/graphql/utilities/value_from_ast.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/utilities/value_from_ast_untyped.py` & `graphql_core-3.3.0a3/src/graphql/utilities/value_from_ast_untyped.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/__init__.py` & `graphql_core-3.3.0a3/src/graphql/validation/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 )
 
 from .rules import ValidationRule, ASTValidationRule, SDLValidationRule
 
 # All validation rules in the GraphQL Specification.
 from .specified_rules import specified_rules
 
+# Spec Section: "Defer And Stream Directive Labels Are Unique"
+from .rules.defer_stream_directive_label import DeferStreamDirectiveLabel
+
+# Spec Section: "Defer And Stream Directives Are Used On Valid Root Field"
+from .rules.defer_stream_directive_on_root_field import DeferStreamDirectiveOnRootField
+
 # Spec Section: "Executable Definitions"
 from .rules.executable_definitions import ExecutableDefinitionsRule
 
 # Spec Section: "Field Selections on Objects, Interfaces, and Unions Types"
 from .rules.fields_on_correct_type import FieldsOnCorrectTypeRule
 
 # Spec Section: "Fragments on Composite Types"
@@ -64,14 +70,17 @@
 
 # Spec Section: "Leaf Field Selections"
 from .rules.scalar_leafs import ScalarLeafsRule
 
 # Spec Section: "Subscriptions with Single Root Field"
 from .rules.single_field_subscriptions import SingleFieldSubscriptionsRule
 
+# Spec Section: "Stream Directives Are Used On List Fields"
+from .rules.stream_directive_on_list_field import StreamDirectiveOnListField
+
 # Spec Section: "Argument Uniqueness"
 from .rules.unique_argument_names import UniqueArgumentNamesRule
 
 # Spec Section: "Directives Are Unique Per Location"
 from .rules.unique_directives_per_location import UniqueDirectivesPerLocationRule
 
 # Spec Section: "Fragment Name Uniqueness"
@@ -114,14 +123,16 @@
     "ASTValidationContext",
     "ASTValidationRule",
     "SDLValidationContext",
     "SDLValidationRule",
     "ValidationContext",
     "ValidationRule",
     "specified_rules",
+    "DeferStreamDirectiveLabel",
+    "DeferStreamDirectiveOnRootField",
     "ExecutableDefinitionsRule",
     "FieldsOnCorrectTypeRule",
     "FragmentsOnCompositeTypesRule",
     "KnownArgumentNamesRule",
     "KnownDirectivesRule",
     "KnownFragmentNamesRule",
     "KnownTypeNamesRule",
@@ -131,14 +142,15 @@
     "NoUnusedFragmentsRule",
     "NoUnusedVariablesRule",
     "OverlappingFieldsCanBeMergedRule",
     "PossibleFragmentSpreadsRule",
     "ProvidedRequiredArgumentsRule",
     "ScalarLeafsRule",
     "SingleFieldSubscriptionsRule",
+    "StreamDirectiveOnListField",
     "UniqueArgumentNamesRule",
     "UniqueDirectivesPerLocationRule",
     "UniqueFragmentNamesRule",
     "UniqueInputFieldNamesRule",
     "UniqueOperationNamesRule",
     "UniqueVariableNamesRule",
     "ValuesOfCorrectTypeRule",
```

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/__init__.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/custom/no_deprecated.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/custom/no_deprecated.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/custom/no_schema_introspection.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/custom/no_schema_introspection.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/executable_definitions.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/executable_definitions.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/fields_on_correct_type.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/fields_on_correct_type.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/fragments_on_composite_types.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/fragments_on_composite_types.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/known_argument_names.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/known_argument_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/known_directives.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/known_directives.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/known_fragment_names.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/known_fragment_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/known_type_names.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/known_type_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/lone_anonymous_operation.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/lone_anonymous_operation.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/lone_schema_definition.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/lone_schema_definition.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/no_fragment_cycles.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/no_fragment_cycles.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/no_undefined_variables.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/no_undefined_variables.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/no_unused_fragments.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/no_unused_fragments.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/no_unused_variables.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/no_unused_variables.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/overlapping_fields_can_be_merged.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/overlapping_fields_can_be_merged.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from itertools import chain
-from typing import Any, Dict, List, Optional, Tuple, Union, cast
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union, cast
 
 from ...error import GraphQLError
 from ...language import (
+    DirectiveNode,
     FieldNode,
     FragmentDefinitionNode,
     FragmentSpreadNode,
     InlineFragmentNode,
     ObjectFieldNode,
     ObjectValueNode,
     SelectionSetNode,
@@ -116,27 +117,27 @@
 # Given any selection set, a collection produces both a set of fields by
 # also including all inline fragments, as well as a list of fragments
 # referenced by fragment spreads.
 #
 # A) Each selection set represented in the document first compares "within" its
 # collected set of fields, finding any conflicts between every pair of
 # overlapping fields.
-# Note: This is the#only time* that a the fields "within" a set are compared
+# Note: This is the *only time* that the fields "within" a set are compared
 # to each other. After this only fields "between" sets are compared.
 #
 # B) Also, if any fragment is referenced in a selection set, then a
 # comparison is made "between" the original set of fields and the
 # referenced fragment.
 #
 # C) Also, if multiple fragments are referenced, then comparisons
 # are made "between" each referenced fragment.
 #
 # D) When comparing "between" a set of fields and a referenced fragment, first
 # a comparison is made between each field in the original set of fields and
-# each field in the the referenced set of fields.
+# each field in the referenced set of fields.
 #
 # E) Also, if any fragment is referenced in the referenced selection set,
 # then a comparison is made "between" the original set of fields and the
 # referenced fragment (recursively referring to step D).
 #
 # F) When comparing "between" two fragments, first a comparison is made between
 # each field in the first referenced set of fields and each field in the the
@@ -555,14 +556,23 @@
                 [node2],
             )
 
         # Two field calls must have the same arguments.
         if stringify_arguments(node1) != stringify_arguments(node2):
             return (response_name, "they have differing arguments"), [node1], [node2]
 
+    directives1 = node1.directives
+    directives2 = node2.directives
+    if not same_streams(directives1, directives2):
+        return (
+            (response_name, "they have differing stream directives"),
+            [node1],
+            [node2],
+        )
+
     if type1 and type2 and do_types_conflict(type1, type2):
         return (
             (response_name, f"they return conflicting types '{type1}' and '{type2}'"),
             [node1],
             [node2],
         )
 
@@ -583,24 +593,48 @@
             selection_set2,
         )
         return subfield_conflicts(conflicts, response_name, node1, node2)
 
     return None  # no conflict
 
 
-def stringify_arguments(field_node: FieldNode) -> str:
+def stringify_arguments(field_node: Union[FieldNode, DirectiveNode]) -> str:
     input_object_with_args = ObjectValueNode(
         fields=tuple(
             ObjectFieldNode(name=arg_node.name, value=arg_node.value)
             for arg_node in field_node.arguments
         )
     )
     return print_ast(sort_value_node(input_object_with_args))
 
 
+def get_stream_directive(
+    directives: Sequence[DirectiveNode],
+) -> Optional[DirectiveNode]:
+    for directive in directives:
+        if directive.name.value == "stream":
+            return directive
+    return None
+
+
+def same_streams(
+    directives1: Sequence[DirectiveNode], directives2: Sequence[DirectiveNode]
+) -> bool:
+    stream1 = get_stream_directive(directives1)
+    stream2 = get_stream_directive(directives2)
+    if not stream1 and not stream2:
+        # both fields do not have streams
+        return True
+    if stream1 and stream2:
+        # check if both fields have equivalent streams
+        return stringify_arguments(stream1) == stringify_arguments(stream2)
+    # fields have a mix of stream and no stream
+    return False
+
+
 def do_types_conflict(type1: GraphQLOutputType, type2: GraphQLOutputType) -> bool:
     """Check whether two types conflict
 
     Two types conflict if both types could not apply to a value simultaneously.
     Composite types are ignored as their individual field types will be compared later
     recursively. However List and Non-Null types must match.
     """
```

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/possible_fragment_spreads.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/possible_fragment_spreads.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/possible_type_extensions.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/possible_type_extensions.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/provided_required_arguments.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/provided_required_arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         self.required_args_map = required_args_map
 
     def leave_directive(self, directive_node: DirectiveNode, *_args: Any) -> None:
         # Validate on leave to allow for deeper errors to appear first.
         directive_name = directive_node.name.value
         required_args = self.required_args_map.get(directive_name)
         if required_args:
-
             arg_nodes = directive_node.arguments or ()
             arg_node_set = {arg.name.value for arg in arg_nodes}
             for arg_name in required_args:
                 if arg_name not in arg_node_set:
                     arg_type = required_args[arg_name].type
                     arg_type_str = (
                         str(arg_type)
```

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/scalar_leafs.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/scalar_leafs.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/single_field_subscriptions.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/single_field_subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             }
             fields = collect_fields(
                 schema,
                 fragments,
                 variable_values,
                 subscription_type,
                 node.selection_set,
-            )
+            ).fields
             if len(fields) > 1:
                 field_selection_lists = list(fields.values())
                 extra_field_selection_lists = field_selection_lists[1:]
                 extra_field_selection = [
                     field
                     for fields in extra_field_selection_lists
                     for field in (
@@ -66,16 +66,15 @@
                             else f"Subscription '{operation_name}'"
                         )
                         + " must select only one top level field.",
                         extra_field_selection,
                     )
                 )
             for field_nodes in fields.values():
-                field = field_nodes[0]
-                field_name = field.name.value
+                field_name = field_nodes[0].name.value
                 if field_name.startswith("__"):
                     self.report_error(
                         GraphQLError(
                             (
                                 "Anonymous Subscription"
                                 if operation_name is None
                                 else f"Subscription '{operation_name}'"
```

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/unique_argument_definition_names.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/unique_argument_definition_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/unique_argument_names.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/unique_argument_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/unique_directive_names.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/unique_directive_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/unique_directives_per_location.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/unique_directives_per_location.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/unique_enum_value_names.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/unique_enum_value_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/unique_field_definition_names.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/unique_field_definition_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/unique_fragment_names.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/unique_fragment_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/unique_input_field_names.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/unique_input_field_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/unique_operation_names.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/unique_operation_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/unique_operation_types.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/unique_operation_types.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/unique_type_names.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/unique_type_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/unique_variable_names.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/unique_variable_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/values_of_correct_type.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/values_of_correct_type.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/variables_are_input_types.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/variables_are_input_types.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/rules/variables_in_allowed_position.py` & `graphql_core-3.3.0a3/src/graphql/validation/rules/variables_in_allowed_position.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/specified_rules.py` & `graphql_core-3.3.0a3/src/graphql/validation/specified_rules.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from typing import Tuple, Type
 
 from .rules import ASTValidationRule
 
+# Spec Section: "Defer And Stream Directive Labels Are Unique"
+from .rules.defer_stream_directive_label import DeferStreamDirectiveLabel
+
+# Spec Section: "Defer And Stream Directives Are Used On Valid Root Field"
+from .rules.defer_stream_directive_on_root_field import DeferStreamDirectiveOnRootField
+
 # Spec Section: "Executable Definitions"
 from .rules.executable_definitions import ExecutableDefinitionsRule
 
 # Spec Section: "Field Selections on Objects, Interfaces, and Unions Types"
 from .rules.fields_on_correct_type import FieldsOnCorrectTypeRule
 
 # Spec Section: "Fragments on Composite Types"
@@ -58,17 +64,20 @@
 )
 
 # Spec Section: "Leaf Field Selections"
 from .rules.scalar_leafs import ScalarLeafsRule
 
 # Spec Section: "Subscriptions with Single Root Field"
 from .rules.single_field_subscriptions import SingleFieldSubscriptionsRule
-from .rules.unique_argument_definition_names import UniqueArgumentDefinitionNamesRule
+
+# Spec Section: "Stream Directives Are Used On List Fields"
+from .rules.stream_directive_on_list_field import StreamDirectiveOnListField
 
 # Spec Section: "Argument Uniqueness"
+from .rules.unique_argument_definition_names import UniqueArgumentDefinitionNamesRule
 from .rules.unique_argument_names import UniqueArgumentNamesRule
 from .rules.unique_directive_names import UniqueDirectiveNamesRule
 
 # Spec Section: "Directives Are Unique Per Location"
 from .rules.unique_directives_per_location import UniqueDirectivesPerLocationRule
 from .rules.unique_enum_value_names import UniqueEnumValueNamesRule
 from .rules.unique_field_definition_names import UniqueFieldDefinitionNamesRule
@@ -121,14 +130,17 @@
     PossibleFragmentSpreadsRule,
     NoFragmentCyclesRule,
     UniqueVariableNamesRule,
     NoUndefinedVariablesRule,
     NoUnusedVariablesRule,
     KnownDirectivesRule,
     UniqueDirectivesPerLocationRule,
+    DeferStreamDirectiveOnRootField,
+    DeferStreamDirectiveLabel,
+    StreamDirectiveOnListField,
     KnownArgumentNamesRule,
     UniqueArgumentNamesRule,
     ValuesOfCorrectTypeRule,
     ProvidedRequiredArgumentsRule,
     VariablesInAllowedPositionRule,
     OverlappingFieldsCanBeMergedRule,
     UniqueInputFieldNamesRule,
```

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/validate.py` & `graphql_core-3.3.0a3/src/graphql/validation/validate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from typing import Collection, List, Optional, Type
 
 from ..error import GraphQLError
 from ..language import DocumentNode, ParallelVisitor, visit
-from ..pyutils import inspect, is_collection
 from ..type import GraphQLSchema, assert_valid_schema
 from ..utilities import TypeInfo, TypeInfoVisitor
 from .rules import ASTValidationRule
 from .specified_rules import specified_rules, specified_sdl_rules
 from .validation_context import SDLValidationContext, ValidationContext
 
 
 __all__ = ["assert_valid_sdl", "assert_valid_sdl_extension", "validate", "validate_sdl"]
 
 
-class ValidationAbortedError(RuntimeError):
+class ValidationAbortedError(GraphQLError):
     """Error when a validation has been aborted (error limit reached)."""
 
 
+validation_aborted_error = ValidationAbortedError(
+    "Too many validation errors, error limit reached. Validation aborted."
+)
+
+
 def validate(
     schema: GraphQLSchema,
     document_ast: DocumentNode,
     rules: Optional[Collection[Type[ASTValidationRule]]] = None,
     max_errors: Optional[int] = None,
     type_info: Optional[TypeInfo] = None,
 ) -> List[GraphQLError]:
@@ -38,59 +42,41 @@
 
     Validate will stop validation after a ``max_errors`` limit has been reached.
     Attackers can send pathologically invalid queries to induce a DoS attack,
     so by default ``max_errors`` set to 100 errors.
 
     Providing a custom TypeInfo instance is deprecated and will be removed in v3.3.
     """
-    if not document_ast or not isinstance(document_ast, DocumentNode):
-        raise TypeError("Must provide document.")
     # If the schema used for validation is invalid, throw an error.
     assert_valid_schema(schema)
     if max_errors is None:
         max_errors = 100
-    elif not isinstance(max_errors, int):
-        raise TypeError("The maximum number of errors must be passed as an int.")
     if type_info is None:
         type_info = TypeInfo(schema)
-    elif not isinstance(type_info, TypeInfo):
-        raise TypeError(f"Not a TypeInfo object: {inspect(type_info)}.")
     if rules is None:
         rules = specified_rules
-    elif not is_collection(rules) or not all(
-        isinstance(rule, type) and issubclass(rule, ASTValidationRule) for rule in rules
-    ):
-        raise TypeError(
-            "Rules must be specified as a collection of ASTValidationRule subclasses."
-        )
 
     errors: List[GraphQLError] = []
 
     def on_error(error: GraphQLError) -> None:
         if len(errors) >= max_errors:  # type: ignore
-            errors.append(
-                GraphQLError(
-                    "Too many validation errors, error limit reached."
-                    " Validation aborted."
-                )
-            )
-            raise ValidationAbortedError
+            raise validation_aborted_error
         errors.append(error)
 
     context = ValidationContext(schema, document_ast, type_info, on_error)
 
     # This uses a specialized visitor which runs multiple visitors in parallel,
     # while maintaining the visitor skip and break API.
     visitors = [rule(context) for rule in rules]
 
     # Visit the whole document with each instance of all provided rules.
     try:
         visit(document_ast, TypeInfoVisitor(type_info, ParallelVisitor(visitors)))
     except ValidationAbortedError:
-        pass
+        errors.append(validation_aborted_error)
     return errors
 
 
 def validate_sdl(
     document_ast: DocumentNode,
     schema_to_extend: Optional[GraphQLSchema] = None,
     rules: Optional[Collection[Type[ASTValidationRule]]] = None,
```

### Comparing `graphql_core-3.3.0a2/src/graphql/validation/validation_context.py` & `graphql_core-3.3.0a3/src/graphql/validation/validation_context.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/src/graphql/version.py` & `graphql_core-3.3.0a3/src/graphql/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import re
 from typing import NamedTuple
 
 
 __all__ = ["version", "version_info", "version_js", "version_info_js"]
 
 
-version = "3.3.0a2"
+version = "3.3.0a3"
 
-version_js = "17.0.0a1"
+version_js = "17.0.0a2"
 
 
 _re_version = re.compile(r"(\d+)\.(\d+)\.(\d+)(\D*)(\d*)")
 
 
 class VersionInfo(NamedTuple):
     major: int
```

### Comparing `graphql_core-3.3.0a2/tests/benchmarks/test_execution_async.py` & `graphql_core-3.3.0a3/tests/benchmarks/test_execution_async.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/benchmarks/test_execution_sync.py` & `graphql_core-3.3.0a3/tests/benchmarks/test_execution_sync.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/benchmarks/test_validate_invalid_gql.py` & `graphql_core-3.3.0a3/tests/benchmarks/test_validate_invalid_gql.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/benchmarks/test_visit.py` & `graphql_core-3.3.0a3/tests/benchmarks/test_visit.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/conftest.py` & `graphql_core-3.3.0a3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/error/test_graphql_error.py` & `graphql_core-3.3.0a3/tests/error/test_graphql_error.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/error/test_located_error.py` & `graphql_core-3.3.0a3/tests/error/test_located_error.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/error/test_print_location.py` & `graphql_core-3.3.0a3/tests/error/test_print_location.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/execution/test_abstract.py` & `graphql_core-3.3.0a3/tests/execution/test_abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from inspect import isawaitable
 from typing import Any, NamedTuple, Optional
 
 from pytest import mark
 
 from graphql.execution import ExecutionResult, execute, execute_sync
 from graphql.language import parse
+from graphql.pyutils import is_awaitable
 from graphql.type import (
     GraphQLBoolean,
     GraphQLField,
     GraphQLInterfaceType,
     GraphQLList,
     GraphQLObjectType,
     GraphQLSchema,
@@ -39,15 +39,15 @@
     assert isinstance(sync, bool)
     assert isinstance(schema, GraphQLSchema)
     assert isinstance(query, str)
     document = parse(query)
     result = (execute_sync if sync else execute)(
         schema, document, root_value
     )  # type: ignore
-    if not sync and isawaitable(result):
+    if not sync and is_awaitable(result):
         result = await result
     assert isinstance(result, ExecutionResult)
     return result
 
 
 def get_is_type_of(type_, sync=True):
     """Get a sync or async is_type_of function for the given type."""
@@ -77,21 +77,19 @@
         async def type_error(*_args):
             raise error
 
     return type_error
 
 
 class Dog(NamedTuple):
-
     name: str
     woofs: bool
 
 
 class Cat(NamedTuple):
-
     name: str
     meows: bool
 
 
 def describe_execute_handles_synchronous_execution_of_abstract_types():
     @sync_and_async
     async def is_type_of_used_to_resolve_runtime_type_for_interface(sync):
@@ -408,15 +406,14 @@
                     "locations": [(3, 15)],
                     "path": ["pets", 1],
                 },
             ],
         )
 
     def describe_using_typename_on_source_object():
-
         expected = (
             {
                 "pets": [
                     {"name": "Odie", "woofs": True},
                     {"name": "Garfield", "meows": False},
                 ]
             },
@@ -479,15 +476,14 @@
                     pets = [Odie(), Garfield()]
 
                 return RootValueWithInheritance()
 
             assert False, f"Unknown access variant: {access}"  # pragma: no cover
 
         def describe_union_type():
-
             schema = build_schema(
                 """
                 type Query {
                   pets: [Pet]
                 }
 
                 union Pet = Cat | Dog
```

### Comparing `graphql_core-3.3.0a2/tests/execution/test_customize.py` & `graphql_core-3.3.0a3/tests/execution/test_customize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from inspect import isasyncgen
+
 from pytest import mark
 
-from graphql.execution import ExecutionContext, MapAsyncIterator, execute, subscribe
+from graphql.execution import ExecutionContext, execute, subscribe
 from graphql.language import parse
 from graphql.type import GraphQLField, GraphQLObjectType, GraphQLSchema, GraphQLString
 
 
 try:
     anext
 except NameError:  # pragma: no cover (Python < 3.10)
@@ -38,16 +40,20 @@
             GraphQLObjectType(
                 "Query",
                 {"foo": GraphQLField(GraphQLString, resolve=lambda *_args: "bar")},
             )
         )
 
         class TestExecutionContext(ExecutionContext):
-            def execute_field(self, parent_type, source, field_nodes, path):
-                result = super().execute_field(parent_type, source, field_nodes, path)
+            def execute_field(
+                self, parent_type, source, field_nodes, path, async_payload_record=None
+            ):
+                result = super().execute_field(
+                    parent_type, source, field_nodes, path, async_payload_record
+                )
                 return result * 2  # type: ignore
 
         assert execute(schema, query, execution_context_class=TestExecutionContext) == (
             {"foo": "barbar"},
             None,
         )
 
@@ -63,21 +69,21 @@
         )
 
         class Root:
             @staticmethod
             async def custom_foo():
                 yield {"foo": "FooValue"}
 
-        subscription = await subscribe(
+        subscription = subscribe(
             schema,
             document=parse("subscription { foo }"),
             root_value=Root(),
             subscribe_field_resolver=lambda root, _info: root.custom_foo(),
         )
-        assert isinstance(subscription, MapAsyncIterator)
+        assert isasyncgen(subscription)
 
         assert await anext(subscription) == (
             {"foo": "FooValue"},
             None,
         )
 
         await subscription.aclose()
@@ -107,16 +113,16 @@
                         subscribe=generate_foo,
                     )
                 },
             ),
         )
 
         document = parse("subscription { foo }")
-        subscription = await subscribe(
+        subscription = subscribe(
             schema,
             document,
             context_value={},
             execution_context_class=TestExecutionContext,
         )
-        assert isinstance(subscription, MapAsyncIterator)
+        assert isasyncgen(subscription)
 
         assert await anext(subscription) == ({"foo": "bar"}, None)
```

### Comparing `graphql_core-3.3.0a2/tests/execution/test_directives.py` & `graphql_core-3.3.0a3/tests/execution/test_directives.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/execution/test_execution_result.py` & `graphql_core-3.3.0a3/tests/execution/test_execution_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from pytest import raises
 
 from graphql.error import GraphQLError
 from graphql.execution import ExecutionResult
 
 
 def describe_execution_result():
-
     data = {"foo": "Some data"}
     error = GraphQLError("Some error")
     errors = [error]
     extensions = {"bar": "Some extension"}
 
     def initializes_properly():
         res = ExecutionResult(data, errors)
```

### Comparing `graphql_core-3.3.0a2/tests/execution/test_executor.py` & `graphql_core-3.3.0a3/tests/execution/test_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from typing import Any, Awaitable, Optional, cast
 
-from pytest import mark, raises
+from pytest import mark
 
 from graphql.error import GraphQLError
 from graphql.execution import execute, execute_sync
 from graphql.language import FieldNode, OperationDefinitionNode, parse
 from graphql.pyutils import Undefined, inspect
 from graphql.type import (
     GraphQLArgument,
@@ -22,67 +22,14 @@
     GraphQLString,
     GraphQLUnionType,
     ResponsePath,
 )
 
 
 def describe_execute_handles_basic_execution_tasks():
-    # noinspection PyTypeChecker
-    def throws_if_no_document_is_provided():
-        schema = GraphQLSchema(
-            GraphQLObjectType("Type", {"a": GraphQLField(GraphQLString)})
-        )
-
-        with raises(TypeError) as exc_info:
-            assert execute_sync(schema=schema, document=None)  # type: ignore
-
-        assert str(exc_info.value) == "Must provide document."
-
-    # noinspection PyTypeChecker
-    def throws_if_no_schema_is_provided():
-        document = parse("{ field }")
-
-        with raises(TypeError) as exc_info:
-            assert execute_sync(schema=None, document=document)  # type: ignore
-
-        assert str(exc_info.value) == "Expected None to be a GraphQL schema."
-
-    def throws_on_invalid_variables():
-        schema = GraphQLSchema(
-            GraphQLObjectType(
-                "Type",
-                {
-                    "fieldA": GraphQLField(
-                        GraphQLString, args={"argA": GraphQLArgument(GraphQLInt)}
-                    )
-                },
-            )
-        )
-        document = parse(
-            """
-            query ($a: Int) {
-              fieldA(argA: $a)
-            }
-            """
-        )
-        variable_values = "{'a': 1}"
-
-        with raises(TypeError) as exc_info:
-            assert execute_sync(
-                schema=schema,
-                document=document,
-                variable_values=variable_values,  # type: ignore
-            )
-
-        assert str(exc_info.value) == (
-            "Variable values must be provided as a dictionary"
-            " with variable names as keys. Perhaps look to see"
-            " if an unparsed JSON string was provided."
-        )
-
     def accepts_positional_arguments():
         schema = GraphQLSchema(
             GraphQLObjectType(
                 "Type",
                 {"a": GraphQLField(GraphQLString, resolve=lambda obj, *args: obj)},
             )
         )
```

### Comparing `graphql_core-3.3.0a2/tests/execution/test_middleware.py` & `graphql_core-3.3.0a3/tests/execution/test_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,14 @@
                 {
                     "first": GraphQLField(GraphQLString),
                     "second": GraphQLField(GraphQLString),
                 },
             )
 
             class ReverseMiddleware:
-
                 # noinspection PyMethodMayBeStatic
                 def resolve(self, next_, *args, **kwargs):
                     return next_(*args, **kwargs)[::-1]
 
             middlewares = MiddlewareManager(ReverseMiddleware())
             result = execute(
                 GraphQLSchema(test_type), doc, Data(), middleware=middlewares
@@ -181,15 +180,14 @@
                 "TestType", {"field": GraphQLField(GraphQLString)}
             )
 
             def reverse_middleware(next_, *args, **kwargs):
                 return next_(*args, **kwargs)[::-1]
 
             class CaptitalizeMiddleware:
-
                 # noinspection PyMethodMayBeStatic
                 def resolve(self, next_, *args, **kwargs):
                     return next_(*args, **kwargs).capitalize()
 
             middlewares = MiddlewareManager(reverse_middleware, CaptitalizeMiddleware())
             result = execute(
                 GraphQLSchema(test_type), doc, Data(), middleware=middlewares
@@ -215,15 +213,14 @@
                 "TestType", {"field": GraphQLField(GraphQLString)}
             )
 
             async def reverse_middleware(next_, *args, **kwargs):
                 return (await next_(*args, **kwargs))[::-1]
 
             class CaptitalizeMiddleware:
-
                 # noinspection PyMethodMayBeStatic
                 async def resolve(self, next_, *args, **kwargs):
                     return (await next_(*args, **kwargs)).capitalize()
 
             middlewares = MiddlewareManager(reverse_middleware, CaptitalizeMiddleware())
             awaitable_result = execute(
                 GraphQLSchema(test_type), doc, Data(), middleware=middlewares
```

### Comparing `graphql_core-3.3.0a2/tests/execution/test_nonnull.py` & `graphql_core-3.3.0a3/tests/execution/test_nonnull.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,14 @@
                         "path": ["sync"],
                         "locations": [(3, 15)],
                     }
                 ],
             )
 
     def describe_nulls_a_returned_object_that_contains_a_non_null_field():
-
         query = """
             {
               syncNest {
                 syncNonNull,
               }
             }
             """
@@ -508,15 +507,14 @@
                         "path": ["syncNonNull"],
                         "locations": [(3, 17)],
                     }
                 ],
             )
 
     def describe_handles_non_null_argument():
-
         # noinspection PyPep8Naming
         schema_with_non_null_arg = GraphQLSchema(
             GraphQLObjectType(
                 "Query",
                 {
                     "withNonNullArg": GraphQLField(
                         GraphQLString,
```

### Comparing `graphql_core-3.3.0a2/tests/execution/test_parallel.py` & `graphql_core-3.3.0a3/tests/execution/test_parallel.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,35 @@
         if not self.number:
             self.event.set()
         return await self.event.wait()
 
 
 def describe_parallel_execution():
     @mark.asyncio
+    async def resolve_single_field():
+        # make sure that the special case of resolving a single field works
+        async def resolve(*_args):
+            return True
+
+        schema = GraphQLSchema(
+            GraphQLObjectType(
+                "Query",
+                {
+                    "foo": GraphQLField(GraphQLBoolean, resolve=resolve),
+                },
+            )
+        )
+
+        awaitable_result = execute(schema, parse("{foo}"))
+        assert isinstance(awaitable_result, Awaitable)
+        result = await awaitable_result
+
+        assert result == ({"foo": True}, None)
+
+    @mark.asyncio
     async def resolve_fields_in_parallel():
         barrier = Barrier(2)
 
         async def resolve(*_args):
             return await barrier.wait()
 
         schema = GraphQLSchema(
@@ -55,14 +76,33 @@
         awaitable_result = execute(schema, ast)
         assert isinstance(awaitable_result, Awaitable)
         result = await asyncio.wait_for(awaitable_result, 1.0)
 
         assert result == ({"foo": True, "bar": True}, None)
 
     @mark.asyncio
+    async def resolve_single_element_list():
+        # make sure that the special case of resolving a single element list works
+        async def resolve(*_args):
+            return [True]
+
+        schema = GraphQLSchema(
+            GraphQLObjectType(
+                "Query",
+                {"foo": GraphQLField(GraphQLList(GraphQLBoolean), resolve=resolve)},
+            )
+        )
+
+        awaitable_result = execute(schema, parse("{foo}"))
+        assert isinstance(awaitable_result, Awaitable)
+        result = await awaitable_result
+
+        assert result == ({"foo": [True]}, None)
+
+    @mark.asyncio
     async def resolve_list_in_parallel():
         barrier = Barrier(2)
 
         async def resolve(*_args):
             return await barrier.wait()
 
         async def resolve_list(*args):
```

### Comparing `graphql_core-3.3.0a2/tests/execution/test_resolve.py` & `graphql_core-3.3.0a3/tests/execution/test_resolve.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/execution/test_schema.py` & `graphql_core-3.3.0a3/tests/execution/test_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     GraphQLString,
 )
 
 
 def describe_execute_handles_execution_with_a_complex_schema():
     def executes_using_a_schema():
         class Article:
-
             # noinspection PyShadowingBuiltins
             def __init__(self, id: int):
                 self.id = id
                 self.isPublished = True
                 self.author = JohnSmith()
                 self.title = f"My Article {id}"
                 self.body = "This is a post"
```

### Comparing `graphql_core-3.3.0a2/tests/execution/test_subscribe.py` & `graphql_core-3.3.0a3/tests/execution/test_subscribe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 import asyncio
-from typing import Any, Callable, Dict, List
+from typing import (
+    Any,
+    AsyncIterable,
+    AsyncIterator,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    TypeVar,
+    Union,
+)
 
 from pytest import mark, raises
 
 from graphql.execution import (
     ExecutionResult,
-    MapAsyncIterator,
     create_source_event_stream,
+    experimental_subscribe_incrementally,
     subscribe,
 )
-from graphql.language import parse
-from graphql.pyutils import SimplePubSub
+from graphql.language import DocumentNode, parse
+from graphql.pyutils import AwaitableOrValue, SimplePubSub, is_awaitable
 from graphql.type import (
     GraphQLArgument,
     GraphQLBoolean,
     GraphQLField,
     GraphQLInt,
     GraphQLList,
     GraphQLObjectType,
+    GraphQLResolveInfo,
     GraphQLSchema,
     GraphQLString,
 )
 
+from ..fixtures import cleanup
+from ..utils.assert_equal_awaitables_or_values import assert_equal_awaitables_or_values
+
 
 try:
     from typing import TypedDict
 except ImportError:  # Python < 3.8
     from typing_extensions import TypedDict
 
 try:
@@ -33,29 +47,37 @@
 except NameError:  # pragma: no cover (Python < 3.10)
     # noinspection PyShadowingBuiltins
     async def anext(iterator):
         """Return the next item from an async iterator."""
         return await iterator.__anext__()
 
 
+T = TypeVar("T")
+
 Email = TypedDict(
     "Email",
     {
         "from": str,
         "subject": str,
         "message": str,
         "unread": bool,
     },
 )
 
+
+async def async_subject(email: Email, _info: GraphQLResolveInfo) -> str:
+    return email["subject"]
+
+
 EmailType = GraphQLObjectType(
     "Email",
     {
         "from": GraphQLField(GraphQLString),
         "subject": GraphQLField(GraphQLString),
+        "asyncSubject": GraphQLField(GraphQLString, resolve=async_subject),
         "message": GraphQLField(GraphQLString),
         "unread": GraphQLField(GraphQLBoolean),
     },
 )
 
 InboxType = GraphQLObjectType(
     "Inbox",
@@ -90,26 +112,37 @@
                 args={"priority": GraphQLArgument(GraphQLInt)},
             )
         },
     ),
 )
 
 
-def create_subscription(pubsub: SimplePubSub):
+def create_subscription(
+    pubsub: SimplePubSub,
+    variable_values: Optional[Dict[str, Any]] = None,
+    original_subscribe: bool = False,
+) -> AwaitableOrValue[Union[AsyncIterator[ExecutionResult], ExecutionResult]]:
     document = parse(
         """
-        subscription ($priority: Int = 0) {
+        subscription ($priority: Int = 0,
+                      $shouldDefer: Boolean = false
+                      $asyncResolver: Boolean = false) {
           importantEmail(priority: $priority) {
             email {
               from
               subject
+              ... @include(if: $asyncResolver) {
+                asyncSubject
+              }
             }
-            inbox {
-              unread
-              total
+            ... @defer(if: $shouldDefer) {
+              inbox {
+                unread
+                total
+              }
             }
           }
         }
         """
     )
 
     emails: List[Email] = [
@@ -127,55 +160,66 @@
         return {"importantEmail": {"email": new_email, "inbox": data["inbox"]}}
 
     data: Dict[str, Any] = {
         "inbox": {"emails": emails},
         "importantEmail": pubsub.get_subscriber(transform),
     }
 
-    return subscribe(email_schema, document, data)
+    return (
+        subscribe if original_subscribe else experimental_subscribe_incrementally
+    )(  # type: ignore
+        email_schema, document, data, variable_values=variable_values
+    )
 
 
 DummyQueryType = GraphQLObjectType("Query", {"dummy": GraphQLField(GraphQLString)})
 
 
-async def subscribe_with_bad_fn(subscribe_fn: Callable) -> ExecutionResult:
+def subscribe_with_bad_fn(
+    subscribe_fn: Callable,
+) -> AwaitableOrValue[Union[ExecutionResult, AsyncIterable[Any]]]:
     schema = GraphQLSchema(
         query=DummyQueryType,
         subscription=GraphQLObjectType(
             "Subscription",
             {"foo": GraphQLField(GraphQLString, subscribe=subscribe_fn)},
         ),
     )
     document = parse("subscription { foo }")
-    result = await subscribe(schema, document)
+    return subscribe_with_bad_args(schema, document)
 
-    assert isinstance(result, ExecutionResult)
-    assert await create_source_event_stream(schema, document) == result
-    return result
+
+def subscribe_with_bad_args(
+    schema: GraphQLSchema,
+    document: DocumentNode,
+    variable_values: Optional[Dict[str, Any]] = None,
+):
+    return assert_equal_awaitables_or_values(
+        subscribe(schema, document, variable_values=variable_values),
+        create_source_event_stream(schema, document, variable_values=variable_values),
+    )
 
 
 # Check all error cases when initializing the subscription.
 def describe_subscription_initialization_phase():
     @mark.asyncio
     async def accepts_positional_arguments():
         document = parse(
             """
             subscription {
               importantEmail
             }
             """
         )
 
-        async def empty_async_iterator(_info):
+        async def empty_async_iterable(_info):
             for value in ():  # type: ignore
                 yield value  # pragma: no cover
 
-        ai = await subscribe(
-            email_schema, document, {"importantEmail": empty_async_iterator}
-        )
+        ai = subscribe(email_schema, document, {"importantEmail": empty_async_iterable})
 
         with raises(StopAsyncIteration):
             await anext(ai)
         await ai.aclose()  # type: ignore
 
     @mark.asyncio
     async def accepts_multiple_subscription_fields_defined_in_schema():
@@ -189,63 +233,70 @@
                 },
             ),
         )
 
         async def foo_generator(_info):
             yield {"foo": "FooValue"}
 
-        subscription = await subscribe(
+        subscription = subscribe(
             schema, parse("subscription { foo }"), {"foo": foo_generator}
         )
-        assert isinstance(subscription, MapAsyncIterator)
+        assert isinstance(subscription, AsyncIterator)
 
         assert await anext(subscription) == ({"foo": "FooValue"}, None)
 
-        await subscription.aclose()
+        await subscription.aclose()  # type: ignore
 
     @mark.asyncio
     async def accepts_type_definition_with_sync_subscribe_function():
         async def foo_generator(_obj, _info):
             yield {"foo": "FooValue"}
 
         schema = GraphQLSchema(
             query=DummyQueryType,
             subscription=GraphQLObjectType(
                 "Subscription",
                 {"foo": GraphQLField(GraphQLString, subscribe=foo_generator)},
             ),
         )
 
-        subscription = await subscribe(schema, parse("subscription { foo }"))
-        assert isinstance(subscription, MapAsyncIterator)
+        subscription = subscribe(schema, parse("subscription { foo }"))
+        assert isinstance(subscription, AsyncIterator)
 
         assert await anext(subscription) == ({"foo": "FooValue"}, None)
 
-        await subscription.aclose()
+        await subscription.aclose()  # type: ignore
 
     @mark.asyncio
     async def accepts_type_definition_with_async_subscribe_function():
         async def foo_generator(_obj, _info):
             await asyncio.sleep(0)
             yield {"foo": "FooValue"}
 
+        async def subscribe_fn(obj, info):
+            await asyncio.sleep(0)
+            return foo_generator(obj, info)
+
         schema = GraphQLSchema(
             query=DummyQueryType,
             subscription=GraphQLObjectType(
                 "Subscription",
-                {"foo": GraphQLField(GraphQLString, subscribe=foo_generator)},
+                {"foo": GraphQLField(GraphQLString, subscribe=subscribe_fn)},
             ),
         )
 
-        subscription = await subscribe(schema, parse("subscription { foo }"))
-        assert isinstance(subscription, MapAsyncIterator)
+        awaitable = subscribe(schema, parse("subscription { foo }"))
+        assert is_awaitable(awaitable)
+
+        subscription = await awaitable
+        assert isinstance(subscription, AsyncIterator)
 
         assert await anext(subscription) == ({"foo": "FooValue"}, None)
 
-        await subscription.aclose()
+        await subscription.aclose()  # type: ignore
 
     @mark.asyncio
     async def should_only_resolve_the_first_field_of_invalid_multi_field():
         did_resolve = {"foo": False, "bar": False}
 
         async def subscribe_foo(_obj, _info):
             did_resolve["foo"] = True
@@ -262,55 +313,32 @@
                 {
                     "foo": GraphQLField(GraphQLString, subscribe=subscribe_foo),
                     "bar": GraphQLField(GraphQLString, subscribe=subscribe_bar),
                 },
             ),
         )
 
-        subscription = await subscribe(schema, parse("subscription { foo bar }"))
-        assert isinstance(subscription, MapAsyncIterator)
+        subscription = subscribe(schema, parse("subscription { foo bar }"))
+        assert isinstance(subscription, AsyncIterator)
 
         assert await anext(subscription) == (
             {"foo": "FooValue", "bar": None},
             None,
         )
 
         assert did_resolve == {"foo": True, "bar": False}
 
-        await subscription.aclose()
-
-    @mark.asyncio
-    async def throws_an_error_if_some_of_required_arguments_are_missing():
-        document = parse("subscription { foo }")
-
-        schema = GraphQLSchema(
-            query=DummyQueryType,
-            subscription=GraphQLObjectType(
-                "Subscription", {"foo": GraphQLField(GraphQLString)}
-            ),
-        )
-
-        with raises(TypeError, match="^Expected None to be a GraphQL schema\\.$"):
-            await subscribe(None, document)  # type: ignore
-
-        with raises(TypeError, match="missing .* positional argument: 'schema'"):
-            await subscribe(document=document)  # type: ignore
-
-        with raises(TypeError, match="^Must provide document\\.$"):
-            await subscribe(schema, None)  # type: ignore
-
-        with raises(TypeError, match="missing .* positional argument: 'document'"):
-            await subscribe(schema=schema)  # type: ignore
+        await subscription.aclose()  # type: ignore
 
     @mark.asyncio
     async def resolves_to_an_error_if_schema_does_not_support_subscriptions():
         schema = GraphQLSchema(query=DummyQueryType)
         document = parse("subscription { unknownField }")
 
-        result = await subscribe(schema, document)
+        result = subscribe_with_bad_args(schema, document)
 
         assert result == (
             None,
             [
                 {
                     "message": "Schema is not configured to execute"
                     " subscription operation.",
@@ -325,15 +353,15 @@
             query=DummyQueryType,
             subscription=GraphQLObjectType(
                 "Subscription", {"foo": GraphQLField(GraphQLString)}
             ),
         )
         document = parse("subscription { unknownField }")
 
-        result = await subscribe(schema, document)
+        result = subscribe_with_bad_args(schema, document)
         assert result == (
             None,
             [
                 {
                     "message": "The subscription field 'unknownField' is not defined.",
                     "locations": [(1, 16)],
                 }
@@ -344,68 +372,88 @@
     async def should_pass_through_unexpected_errors_thrown_in_subscribe():
         schema = GraphQLSchema(
             query=DummyQueryType,
             subscription=GraphQLObjectType(
                 "Subscription", {"foo": GraphQLField(GraphQLString)}
             ),
         )
-        with raises(TypeError, match="^Must provide document\\.$"):
-            await subscribe(schema=schema, document={})  # type: ignore
+        with raises(AttributeError):
+            subscribe_with_bad_args(schema=schema, document={})  # type: ignore
 
     @mark.asyncio
     @mark.filterwarnings("ignore:.* was never awaited:RuntimeWarning")
     async def throws_an_error_if_subscribe_does_not_return_an_iterator():
-        assert await subscribe_with_bad_fn(lambda _obj, _info: "test") == (
+        expected_result = (
             None,
             [
                 {
                     "message": "Subscription field must return AsyncIterable."
                     " Received: 'test'.",
                     "locations": [(1, 16)],
                     "path": ["foo"],
                 }
             ],
         )
 
+        def sync_fn(_obj, _info):
+            return "test"
+
+        assert subscribe_with_bad_fn(sync_fn) == expected_result
+
+        async def async_fn(obj, info):
+            return sync_fn(obj, info)
+
+        result = subscribe_with_bad_fn(async_fn)
+        assert is_awaitable(result)
+        assert await result == expected_result
+
+        del result
+        cleanup()
+
     @mark.asyncio
     async def resolves_to_an_error_for_subscription_resolver_errors():
         expected_result = (
             None,
             [
                 {
                     "message": "test error",
                     "locations": [(1, 16)],
                     "path": ["foo"],
                 }
             ],
         )
 
         # Returning an error
-        def return_error(_obj, _info):
+        def return_error(*_args):
             return TypeError("test error")
 
-        assert await subscribe_with_bad_fn(return_error) == expected_result
+        assert subscribe_with_bad_fn(return_error) == expected_result
 
         # Throwing an error
         def throw_error(*_args):
             raise TypeError("test error")
 
-        assert await subscribe_with_bad_fn(throw_error) == expected_result
+        assert subscribe_with_bad_fn(throw_error) == expected_result
 
         # Resolving to an error
-        async def resolve_error(*_args):
-            return TypeError("test error")
+        async def resolve_to_error(*args):
+            return return_error(*args)
 
-        assert await subscribe_with_bad_fn(resolve_error) == expected_result
+        result = subscribe_with_bad_fn(resolve_to_error)
+        assert is_awaitable(result)
+        assert await result == expected_result
 
         # Rejecting with an error
-        async def reject_error(*_args):
-            return TypeError("test error")
 
-        assert await subscribe_with_bad_fn(reject_error) == expected_result
+        async def reject_with_error(*args):
+            return throw_error(*args)
+
+        result = subscribe_with_bad_fn(reject_with_error)
+        assert is_awaitable(result)
+        assert await result == expected_result
 
     @mark.asyncio
     async def resolves_to_an_error_if_variables_were_wrong_type():
         schema = GraphQLSchema(
             query=DummyQueryType,
             subscription=GraphQLObjectType(
                 "Subscription",
@@ -424,41 +472,43 @@
               foo(arg: $arg)
             }
             """
         )
 
         # If we receive variables that cannot be coerced correctly, subscribe() will
         # resolve to an ExecutionResult that contains an informative error description.
-        result = await subscribe(schema, document, variable_values=variable_values)
+        result = subscribe_with_bad_args(
+            schema, document, variable_values=variable_values
+        )
 
         assert result == (
             None,
             [
                 {
                     "message": "Variable '$arg' got invalid value 'meow';"
                     " Int cannot represent non-integer value: 'meow'",
                     "locations": [(2, 27)],
                 }
             ],
         )
 
-        assert result.errors[0].original_error is None  # type: ignore
+        assert result.errors[0].original_error is None
 
 
 # Once a subscription returns a valid AsyncIterator, it can still yield errors.
 def describe_subscription_publish_phase():
     @mark.asyncio
     async def produces_a_payload_for_multiple_subscribe_in_same_subscription():
         pubsub = SimplePubSub()
 
-        subscription = await create_subscription(pubsub)
-        assert isinstance(subscription, MapAsyncIterator)
+        subscription = create_subscription(pubsub)
+        assert isinstance(subscription, AsyncIterator)
 
-        second_subscription = await create_subscription(pubsub)
-        assert isinstance(subscription, MapAsyncIterator)
+        second_subscription = create_subscription(pubsub)
+        assert isinstance(subscription, AsyncIterator)
 
         payload1 = anext(subscription)
         payload2 = anext(second_subscription)
 
         assert (
             pubsub.emit(
                 {
@@ -478,18 +528,57 @@
             }
         }
 
         assert await payload1 == (expected_payload, None)
         assert await payload2 == (expected_payload, None)
 
     @mark.asyncio
+    async def produces_a_payload_when_queried_fields_are_async():
+        pubsub = SimplePubSub()
+        subscription = create_subscription(pubsub, {"asyncResolver": True})
+        assert isinstance(subscription, AsyncIterator)
+
+        assert (
+            pubsub.emit(
+                {
+                    "from": "yuzhi@graphql.org",
+                    "subject": "Alright",
+                    "message": "Tests are good",
+                    "unread": True,
+                }
+            )
+            is True
+        )
+
+        assert await anext(subscription) == (
+            {
+                "importantEmail": {
+                    "email": {
+                        "from": "yuzhi@graphql.org",
+                        "subject": "Alright",
+                        "asyncSubject": "Alright",
+                    },
+                    "inbox": {"unread": 1, "total": 2},
+                }
+            },
+            None,
+        )
+
+        try:
+            await subscription.aclose()  # type: ignore
+        except RuntimeError:  # Python < 3.8
+            pass
+        with raises(StopAsyncIteration):
+            await anext(subscription)
+
+    @mark.asyncio
     async def produces_a_payload_per_subscription_event():
         pubsub = SimplePubSub()
-        subscription = await create_subscription(pubsub)
-        assert isinstance(subscription, MapAsyncIterator)
+        subscription = create_subscription(pubsub)
+        assert isinstance(subscription, AsyncIterator)
 
         # Wait for the next subscription payload.
         payload = anext(subscription)
 
         # A new email arrives!
         assert (
             pubsub.emit(
@@ -536,15 +625,18 @@
                 }
             },
             None,
         )
 
         # The client decides to disconnect.
         # noinspection PyUnresolvedReferences
-        await subscription.aclose()
+        try:
+            await subscription.aclose()  # type: ignore
+        except RuntimeError:  # Python < 3.8
+            pass
 
         # Which may result in disconnecting upstream services as well.
         assert (
             pubsub.emit(
                 {
                     "from": "adam@graphql.org",
                     "subject": "Important",
@@ -556,18 +648,210 @@
         )  # No more listeners.
 
         # Awaiting subscription after closing it results in completed results.
         with raises(StopAsyncIteration):
             assert await anext(subscription)
 
     @mark.asyncio
+    async def produces_additional_payloads_for_subscriptions_with_defer():
+        pubsub = SimplePubSub()
+        subscription = create_subscription(pubsub, {"shouldDefer": True})
+        assert isinstance(subscription, AsyncIterator)
+
+        # Wait for the next subscription payload.
+        payload = anext(subscription)
+
+        # A new email arrives!
+        assert (
+            pubsub.emit(
+                {
+                    "from": "yuzhi@graphql.org",
+                    "subject": "Alright",
+                    "message": "Tests are good",
+                    "unread": True,
+                }
+            )
+            is True
+        )
+
+        # The previously waited on payload now has a value.
+        result = await payload
+        assert result.formatted == {
+            "data": {
+                "importantEmail": {
+                    "email": {
+                        "from": "yuzhi@graphql.org",
+                        "subject": "Alright",
+                    },
+                },
+            },
+            "hasNext": True,
+        }
+
+        # Wait for the next payload from @defer
+        result = await anext(subscription)
+        assert result.formatted == {
+            "incremental": [
+                {
+                    "data": {"inbox": {"total": 2, "unread": 1}},
+                    "path": ["importantEmail"],
+                }
+            ],
+            "hasNext": False,
+        }
+
+        # Another new email arrives,
+        # after all incrementally delivered payloads are received.
+        assert (
+            pubsub.emit(
+                {
+                    "from": "hyo@graphql.org",
+                    "subject": "Tools",
+                    "message": "I <3 making things",
+                    "unread": True,
+                }
+            )
+            is True
+        )
+
+        # The next waited on payload will have a value.
+        result = await anext(subscription)
+        assert result.formatted == {
+            "data": {
+                "importantEmail": {
+                    "email": {
+                        "from": "hyo@graphql.org",
+                        "subject": "Tools",
+                    },
+                },
+            },
+            "hasNext": True,
+        }
+
+        # Another new email arrives,
+        # before the incrementally delivered payloads from the last email was received.
+        assert (
+            pubsub.emit(
+                {
+                    "from": "adam@graphql.org",
+                    "subject": "Important",
+                    "message": "Read me please",
+                    "unread": True,
+                }
+            )
+            is True
+        )
+
+        # Deferred payload from previous event is received.
+        result = await anext(subscription)
+        assert result.formatted == {
+            "incremental": [
+                {
+                    "data": {"inbox": {"total": 3, "unread": 2}},
+                    "path": ["importantEmail"],
+                }
+            ],
+            "hasNext": False,
+        }
+
+        # Next payload from last event
+        result = await anext(subscription)
+        assert result.formatted == {
+            "data": {
+                "importantEmail": {
+                    "email": {
+                        "from": "adam@graphql.org",
+                        "subject": "Important",
+                    },
+                },
+            },
+            "hasNext": True,
+        }
+
+        # The client disconnects before the deferred payload is consumed.
+        try:
+            await subscription.aclose()  # type: ignore
+        except RuntimeError:  # Python < 3.8
+            pass
+
+        # Awaiting a subscription after closing it results in completed results.
+        with raises(StopAsyncIteration):
+            assert await anext(subscription)
+
+    @mark.asyncio
+    async def original_subscribe_function_returns_errors_with_defer():
+        pubsub = SimplePubSub()
+        subscription = create_subscription(pubsub, {"shouldDefer": True}, True)
+        assert isinstance(subscription, AsyncIterator)
+
+        # Wait for the next subscription payload.
+        payload = anext(subscription)
+
+        # A new email arrives!
+        assert (
+            pubsub.emit(
+                {
+                    "from": "yuzhi@graphql.org",
+                    "subject": "Alright",
+                    "message": "Tests are good",
+                    "unread": True,
+                }
+            )
+            is True
+        )
+
+        error_payload = (
+            None,
+            [
+                {
+                    "message": "Executing this GraphQL operation would unexpectedly"
+                    " produce multiple payloads"
+                    " (due to @defer or @stream directive)",
+                }
+            ],
+        )
+
+        # The previously waited on payload now has a value.
+        assert await payload == error_payload
+
+        # Wait for the next payload from @defer
+        assert await anext(subscription) == error_payload
+
+        # Another new email arrives,
+        # after all incrementally delivered payloads are received.
+        assert (
+            pubsub.emit(
+                {
+                    "from": "hyo@graphql.org",
+                    "subject": "Tools",
+                    "message": "I <3 making things",
+                    "unread": True,
+                }
+            )
+            is True
+        )
+
+        # The next waited on payload will have a value.
+        assert await anext(subscription) == error_payload
+
+        # The next waited on payload will have a value.
+        assert await anext(subscription) == error_payload
+
+        # The client disconnects before the deferred payload is consumed.
+        await subscription.aclose()  # type: ignore
+
+        # Awaiting a subscription after closing it results in completed results.
+        with raises(StopAsyncIteration):
+            assert await anext(subscription)
+
+    @mark.asyncio
     async def produces_a_payload_when_there_are_multiple_events():
         pubsub = SimplePubSub()
-        subscription = await create_subscription(pubsub)
-        assert isinstance(subscription, MapAsyncIterator)
+        subscription = create_subscription(pubsub)
+        assert isinstance(subscription, AsyncIterator)
 
         payload = anext(subscription)
 
         # A new email arrives!
         assert (
             pubsub.emit(
                 {
@@ -614,16 +898,16 @@
             },
             None,
         )
 
     @mark.asyncio
     async def should_not_trigger_when_subscription_is_already_done():
         pubsub = SimplePubSub()
-        subscription = await create_subscription(pubsub)
-        assert isinstance(subscription, MapAsyncIterator)
+        subscription = create_subscription(pubsub)
+        assert isinstance(subscription, AsyncIterator)
 
         payload = anext(subscription)
 
         # A new email arrives!
         assert (
             pubsub.emit(
                 {
@@ -643,15 +927,18 @@
                     "inbox": {"unread": 1, "total": 2},
                 }
             },
             None,
         )
 
         payload = anext(subscription)
-        await subscription.aclose()
+        try:
+            await subscription.aclose()  # type: ignore
+        except RuntimeError:  # Python < 3.8
+            pass
 
         # A new email arrives!
         assert (
             pubsub.emit(
                 {
                     "from": "yuzhi@graphql.org",
                     "subject": "Alright 2",
@@ -664,16 +951,16 @@
 
         with raises(StopAsyncIteration):
             await payload
 
     @mark.asyncio
     async def should_not_trigger_when_subscription_is_thrown():
         pubsub = SimplePubSub()
-        subscription = await create_subscription(pubsub)
-        assert isinstance(subscription, MapAsyncIterator)
+        subscription = create_subscription(pubsub)
+        assert isinstance(subscription, AsyncIterator)
 
         payload = anext(subscription)
 
         # A new email arrives!
         assert (
             pubsub.emit(
                 {
@@ -696,25 +983,25 @@
             None,
         )
 
         payload = anext(subscription)
 
         # Throw error
         with raises(RuntimeError) as exc_info:
-            await subscription.athrow(RuntimeError("ouch"))
+            await subscription.athrow(RuntimeError("ouch"))  # type: ignore
         assert str(exc_info.value) == "ouch"
 
         with raises(StopAsyncIteration):
             await payload
 
     @mark.asyncio
     async def event_order_is_correct_for_multiple_publishes():
         pubsub = SimplePubSub()
-        subscription = await create_subscription(pubsub)
-        assert isinstance(subscription, MapAsyncIterator)
+        subscription = create_subscription(pubsub)
+        assert isinstance(subscription, AsyncIterator)
 
         payload = anext(subscription)
 
         # A new email arrives!
         assert (
             pubsub.emit(
                 {
@@ -785,16 +1072,16 @@
                         resolve=resolve_message,
                     )
                 },
             ),
         )
 
         document = parse("subscription { newMessage }")
-        subscription = await subscribe(schema, document)
-        assert isinstance(subscription, MapAsyncIterator)
+        subscription = subscribe(schema, document)
+        assert isinstance(subscription, AsyncIterator)
 
         assert await anext(subscription) == ({"newMessage": "Hello"}, None)
 
         # An error in execution is presented as such.
         assert await anext(subscription) == (
             {"newMessage": None},
             [
@@ -830,29 +1117,29 @@
                         subscribe=generate_messages,
                     )
                 },
             ),
         )
 
         document = parse("subscription { newMessage }")
-        subscription = await subscribe(schema, document)
-        assert isinstance(subscription, MapAsyncIterator)
+        subscription = subscribe(schema, document)
+        assert isinstance(subscription, AsyncIterator)
 
-        assert await (anext(subscription)) == ({"newMessage": "Hello"}, None)
+        assert await anext(subscription) == ({"newMessage": "Hello"}, None)
 
         with raises(RuntimeError) as exc_info:
             await anext(subscription)
 
         assert str(exc_info.value) == "test error"
 
         with raises(StopAsyncIteration):
             await anext(subscription)
 
     @mark.asyncio
-    async def should_work_with_async_resolve_function():
+    async def should_work_with_sync_resolve_function():
         async def generate_messages(_obj, _info):
             yield "Hello"
 
         def resolve_message(message, _info):
             return message
 
         schema = GraphQLSchema(
@@ -866,11 +1153,149 @@
                         subscribe=generate_messages,
                     )
                 },
             ),
         )
 
         document = parse("subscription { newMessage }")
-        subscription = await subscribe(schema, document)
-        assert isinstance(subscription, MapAsyncIterator)
+        subscription = subscribe(schema, document)
+        assert isinstance(subscription, AsyncIterator)
 
         assert await anext(subscription) == ({"newMessage": "Hello"}, None)
+
+    @mark.asyncio
+    async def should_work_with_async_resolve_function():
+        async def generate_messages(_obj, _info):
+            await asyncio.sleep(0)
+            yield "Hello"
+
+        async def resolve_message(message, _info):
+            await asyncio.sleep(0)
+            return message
+
+        schema = GraphQLSchema(
+            query=QueryType,
+            subscription=GraphQLObjectType(
+                "Subscription",
+                {
+                    "newMessage": GraphQLField(
+                        GraphQLString,
+                        resolve=resolve_message,
+                        subscribe=generate_messages,
+                    )
+                },
+            ),
+        )
+
+        document = parse("subscription { newMessage }")
+        subscription = subscribe(schema, document)
+        assert isinstance(subscription, AsyncIterator)
+
+        assert await anext(subscription) == ({"newMessage": "Hello"}, None)
+
+    @mark.asyncio
+    async def should_work_with_custom_async_iterator():
+        class MessageGenerator:
+            resolved: List[str] = []
+
+            def __init__(self, values, _info):
+                self.values = values
+
+            def __aiter__(self):
+                return self
+
+            async def __anext__(self):
+                if not self.values:
+                    raise StopAsyncIteration
+                await asyncio.sleep(0)
+                return self.values.pop(0)
+
+            @classmethod
+            async def resolve(cls, message, _info):
+                await asyncio.sleep(0)
+                cls.resolved.append(message)
+                return message + "!"
+
+        schema = GraphQLSchema(
+            query=QueryType,
+            subscription=GraphQLObjectType(
+                "Subscription",
+                {
+                    "newMessage": GraphQLField(
+                        GraphQLString,
+                        resolve=MessageGenerator.resolve,
+                        subscribe=MessageGenerator,
+                    )
+                },
+            ),
+        )
+
+        document = parse("subscription { newMessage }")
+        subscription = subscribe(schema, document, ["Hello", "Dolly"])
+        assert isinstance(subscription, AsyncIterator)
+
+        assert [result async for result in subscription] == [
+            ({"newMessage": "Hello!"}, None),
+            ({"newMessage": "Dolly!"}, None),
+        ]
+
+        assert MessageGenerator.resolved == ["Hello", "Dolly"]
+
+        await subscription.aclose()  # type: ignore
+
+    @mark.asyncio
+    async def should_close_custom_async_iterator():
+        class MessageGenerator:
+            closed: bool = False
+            resolved: List[str] = []
+
+            def __init__(self, values, _info):
+                self.values = values
+
+            def __aiter__(self):
+                return self
+
+            async def __anext__(self):
+                if not self.values:
+                    raise StopAsyncIteration
+                await asyncio.sleep(0)
+                return self.values.pop(0)
+
+            @classmethod
+            async def resolve(cls, message, _info):
+                await asyncio.sleep(0)
+                cls.resolved.append(message)
+                return message + "!"
+
+            @classmethod
+            async def aclose(cls):
+                cls.closed = True
+
+        schema = GraphQLSchema(
+            query=QueryType,
+            subscription=GraphQLObjectType(
+                "Subscription",
+                {
+                    "newMessage": GraphQLField(
+                        GraphQLString,
+                        resolve=MessageGenerator.resolve,
+                        subscribe=MessageGenerator,
+                    )
+                },
+            ),
+        )
+
+        document = parse("subscription { newMessage }")
+        subscription = subscribe(schema, document, ["Hello", "Dolly"])
+        assert isinstance(subscription, AsyncIterator)
+
+        assert not MessageGenerator.closed
+
+        assert [result async for result in subscription] == [
+            ({"newMessage": "Hello!"}, None),
+            ({"newMessage": "Dolly!"}, None),
+        ]
+
+        assert MessageGenerator.closed
+        assert MessageGenerator.resolved == ["Hello", "Dolly"]
+
+        await subscription.aclose()
```

### Comparing `graphql_core-3.3.0a2/tests/execution/test_sync.py` & `graphql_core-3.3.0a3/tests/execution/test_sync.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from gc import collect
-from inspect import isawaitable
-
 from pytest import mark, raises
 
 from graphql import graphql_sync
 from graphql.execution import execute, execute_sync
 from graphql.language import parse
+from graphql.pyutils import is_awaitable
 from graphql.type import GraphQLField, GraphQLObjectType, GraphQLSchema, GraphQLString
 from graphql.validation import validate
 
+from ..fixtures import cleanup
+
 
 def describe_execute_synchronously_when_possible():
     def _resolve_sync(root_value, _info):
         return root_value
 
     async def _resolve_async(root_value, _info):
         return root_value
@@ -52,15 +52,15 @@
             None,
         )
 
     @mark.asyncio
     async def returns_an_awaitable_if_any_field_is_asynchronous():
         doc = "query Example { syncField, asyncField }"
         result = execute(schema, parse(doc), "rootValue")
-        assert isawaitable(result)
+        assert is_awaitable(result)
         assert await result == (
             {"syncField": "rootValue", "asyncField": "rootValue"},
             None,
         )
 
     def describe_execute_sync():
         def does_not_return_an_awaitable_for_sync_execution():
@@ -87,14 +87,16 @@
             doc = "query Example { syncField, asyncField }"
             with raises(RuntimeError) as exc_info:
                 execute_sync(
                     schema, document=parse(doc), root_value="rootValue", check_sync=True
                 )
             msg = str(exc_info.value)
             assert msg == "GraphQL execution failed to complete synchronously."
+            del exc_info
+            cleanup()
 
         @mark.asyncio
         @mark.filterwarnings("ignore:.* was never awaited:RuntimeWarning")
         async def throws_if_encountering_async_operation_without_check_sync():
             doc = "query Example { syncField, asyncField }"
             result = execute_sync(schema, document=parse(doc), root_value="rootValue")
             assert result == (
@@ -104,17 +106,54 @@
                         "message": "String cannot represent value:"
                         " <coroutine _resolve_async>",
                         "locations": [(1, 28)],
                         "path": ["asyncField"],
                     }
                 ],
             )
-            # garbage collect coroutine in order to not postpone the warning
             del result
-            collect()
+            cleanup()
+
+        @mark.asyncio
+        @mark.filterwarnings("ignore:.* was never awaited:RuntimeWarning")
+        async def throws_if_encountering_async_iterable_execution_with_check_sync():
+            doc = """
+                query Example {
+                  ...deferFrag @defer(label: "deferLabel")
+                }
+                fragment deferFrag on Query {
+                  syncField
+                }
+            """
+            with raises(RuntimeError) as exc_info:
+                execute_sync(
+                    schema, document=parse(doc), root_value="rootValue", check_sync=True
+                )
+            msg = str(exc_info.value)
+            assert msg == "GraphQL execution failed to complete synchronously."
+            del exc_info
+            cleanup()
+
+        @mark.asyncio
+        @mark.filterwarnings("ignore:.* was never awaited:RuntimeWarning")
+        async def throws_if_encountering_async_iterable_execution_without_check_sync():
+            doc = """
+                query Example {
+                  ...deferFrag @defer(label: "deferLabel")
+                }
+                fragment deferFrag on Query {
+                  syncField
+                }
+            """
+            with raises(RuntimeError) as exc_info:
+                execute_sync(schema, document=parse(doc), root_value="rootValue")
+            msg = str(exc_info.value)
+            assert msg == "GraphQL execution failed to complete synchronously."
+            del exc_info
+            cleanup()
 
     def describe_graphql_sync():
         def reports_errors_raised_during_schema_validation():
             bad_schema = GraphQLSchema()
             result = graphql_sync(schema=bad_schema, source="{ __typename }")
             assert result == (None, [{"message": "Query root type must be provided."}])
 
@@ -154,14 +193,16 @@
         @mark.filterwarnings("ignore:.* was never awaited:RuntimeWarning")
         async def throws_if_encountering_async_operation_with_check_sync():
             doc = "query Example { syncField, asyncField }"
             with raises(RuntimeError) as exc_info:
                 graphql_sync(schema, doc, "rootValue", check_sync=True)
             msg = str(exc_info.value)
             assert msg == "GraphQL execution failed to complete synchronously."
+            del exc_info
+            cleanup()
 
         @mark.asyncio
         @mark.filterwarnings("ignore:.* was never awaited:RuntimeWarning")
         async def throws_if_encountering_async_operation_without_check_sync():
             doc = "query Example { syncField, asyncField }"
             result = graphql_sync(schema, doc, "rootValue")
             assert result == (
@@ -171,10 +212,9 @@
                         "message": "String cannot represent value:"
                         " <coroutine _resolve_async>",
                         "locations": [(1, 28)],
                         "path": ["asyncField"],
                     }
                 ],
             )
-            # garbage collect coroutine in order to not postpone the warning
             del result
-            collect()
+            cleanup()
```

### Comparing `graphql_core-3.3.0a2/tests/execution/test_union_interface.py` & `graphql_core-3.3.0a3/tests/execution/test_union_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     GraphQLSchema,
     GraphQLString,
     GraphQLUnionType,
 )
 
 
 class Dog:
-
     name: str
     barks: bool
     mother: Optional[Dog]
     father: Optional[Dog]
     progeny: List[Dog]
 
     def __init__(self, name: str, barks: bool):
@@ -29,15 +28,14 @@
         self.barks = barks
         self.mother = None
         self.father = None
         self.progeny = []
 
 
 class Cat:
-
     name: str
     meows: bool
     mother: Optional[Cat]
     father: Optional[Cat]
     progeny: List[Cat]
 
     def __init__(self, name: str, meows: bool):
@@ -45,15 +43,14 @@
         self.meows = meows
         self.mother = None
         self.father = None
         self.progeny = []
 
 
 class Person:
-
     name: str
     pets: Optional[List[Union[Dog, Cat]]]
     friends: Optional[List[Union[Dog, Cat, Person]]]
 
     def __init__(
         self,
         name: str,
```

### Comparing `graphql_core-3.3.0a2/tests/execution/test_variables.py` & `graphql_core-3.3.0a3/tests/execution/test_variables.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/fixtures/__init__.py` & `graphql_core-3.3.0a3/tests/fixtures/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 """Fixtures for graphql tests"""
 import json
+from gc import collect
 from os.path import dirname, join
 
 from pytest import fixture
 
 
 __all__ = [
+    "cleanup",
     "kitchen_sink_query",
     "kitchen_sink_sdl",
     "big_schema_sdl",
     "big_schema_introspection_result",
 ]
 
 
+def cleanup(rounds=5):
+    """Run garbage collector.
+
+    This can be used to remove coroutines that were not awaited after running tests.
+    """
+    for _generation in range(rounds):
+        collect()
+
+
 def read_graphql(name):
     path = join(dirname(__file__), name + ".graphql")
     return open(path, encoding="utf-8").read()
 
 
 def read_json(name):
     path = join(dirname(__file__), name + ".json")
```

### Comparing `graphql_core-3.3.0a2/tests/fixtures/github_schema.graphql` & `graphql_core-3.3.0a3/tests/fixtures/github_schema.graphql`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/fixtures/github_schema.json` & `graphql_core-3.3.0a3/tests/fixtures/github_schema.json`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/fixtures/schema_kitchen_sink.graphql` & `graphql_core-3.3.0a3/tests/fixtures/schema_kitchen_sink.graphql`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/language/test_ast.py` & `graphql_core-3.3.0a3/tests/language/test_ast.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import weakref
 from copy import copy, deepcopy
+from typing import Optional
 
-from graphql.language import Location, Node, Source, Token, TokenKind
+from graphql.language import Location, NameNode, Node, Source, Token, TokenKind
 from graphql.pyutils import inspect
 
 
 class SampleTestNode(Node):
     __slots__ = "alpha", "beta"
 
     alpha: int
     beta: int
 
 
+class SampleNamedNode(Node):
+    __slots__ = "foo", "name"
+
+    foo: str
+    name: Optional[str]
+
+
 def describe_token_class():
     def initializes():
         token = Token(
             kind=TokenKind.NAME,
             start=11,
             end=12,
             line=1,
@@ -156,14 +164,33 @@
 
     def has_representation_with_loc():
         node = SampleTestNode(alpha=1, beta=2)
         assert repr(node) == "SampleTestNode"
         node = SampleTestNode(alpha=1, beta=2, loc=3)
         assert repr(node) == "SampleTestNode at 3"
 
+    def has_representation_when_named():
+        name_node = NameNode(value="baz")
+        node = SampleNamedNode(foo="bar", name=name_node)
+        assert repr(node) == "SampleNamedNode(name='baz')"
+        node = SampleNamedNode(alpha=1, beta=2, name=name_node, loc=3)
+        assert repr(node) == "SampleNamedNode(name='baz') at 3"
+
+    def has_representation_when_named_but_name_is_none():
+        node = SampleNamedNode(alpha=1, beta=2, name=None)
+        assert repr(node) == "SampleNamedNode"
+        node = SampleNamedNode(alpha=1, beta=2, name=None, loc=3)
+        assert repr(node) == "SampleNamedNode at 3"
+
+    def has_special_representation_when_it_is_a_name_node():
+        node = NameNode(value="foo")
+        assert repr(node) == "NameNode('foo')"
+        node = NameNode(value="foo", loc=3)
+        assert repr(node) == "NameNode('foo') at 3"
+
     def can_check_equality():
         node = SampleTestNode(alpha=1, beta=2)
         node2 = SampleTestNode(alpha=1, beta=2)
         assert node2 == node
         assert not node2 != node
         node2 = SampleTestNode(alpha=1, beta=1)
         assert node2 != node
```

### Comparing `graphql_core-3.3.0a2/tests/language/test_block_string.py` & `graphql_core-3.3.0a3/tests/language/test_block_string.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/language/test_block_string_fuzz.py` & `graphql_core-3.3.0a3/tests/language/test_block_string_fuzz.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from graphql.language import Lexer, Source, TokenKind
 from graphql.language.block_string import (
     is_printable_as_block_string,
     print_block_string,
 )
 
-from ..utils import dedent, gen_fuzz_strings, timeout_factor
+from ..utils import dedent, gen_fuzz_strings
 
 
 def lex_value(s: str) -> str:
     lexer = Lexer(Source(s))
     value = lexer.advance().value
     assert isinstance(value, str)
     assert lexer.advance().kind == TokenKind.EOF, "Expected EOF"
@@ -38,15 +38,15 @@
           to not equal {test_value!r}
         """
     )
 
 
 def describe_print_block_string():
     @mark.slow
-    @mark.timeout(80 * timeout_factor)
+    @mark.timeout(80)
     def correctly_print_random_strings():
         # Testing with length >7 is taking exponentially more time. However, it is
         # highly recommended testing with increased limit if you make any change.
         for fuzz_str in gen_fuzz_strings(allowed_chars='\n\t "a\\', max_length=7):
             if not is_printable_as_block_string(fuzz_str):
                 assert_non_printable_block_string(fuzz_str)
                 continue
```

### Comparing `graphql_core-3.3.0a2/tests/language/test_character_classes.py` & `graphql_core-3.3.0a3/tests/language/test_character_classes.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/language/test_lexer.py` & `graphql_core-3.3.0a3/tests/language/test_lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,14 +515,15 @@
         assert_syntax_error(
             "1.234_5", "Invalid number, expected digit but got: '_'.", (1, 6)
         )
 
     # noinspection PyArgumentEqualDefault
     def lexes_punctuation():
         assert lex_one("!") == Token(TokenKind.BANG, 0, 1, 1, 1, None)
+        assert lex_one("?") == Token(TokenKind.QUESTION_MARK, 0, 1, 1, 1, None)
         assert lex_one("$") == Token(TokenKind.DOLLAR, 0, 1, 1, 1, None)
         assert lex_one("(") == Token(TokenKind.PAREN_L, 0, 1, 1, 1, None)
         assert lex_one(")") == Token(TokenKind.PAREN_R, 0, 1, 1, 1, None)
         assert lex_one("...") == Token(TokenKind.SPREAD, 0, 3, 1, 1, None)
         assert lex_one(":") == Token(TokenKind.COLON, 0, 1, 1, 1, None)
         assert lex_one("=") == Token(TokenKind.EQUALS, 0, 1, 1, 1, None)
         assert lex_one("@") == Token(TokenKind.AT, 0, 1, 1, 1, None)
@@ -618,14 +619,15 @@
 
 def describe_is_punctuator_token_kind():
     def _is_punctuator_token(text: str) -> bool:
         return is_punctuator_token_kind(lex_one(text).kind)
 
     def returns_true_for_punctuator_tokens():
         assert _is_punctuator_token("!") is True
+        assert _is_punctuator_token("?") is True
         assert _is_punctuator_token("$") is True
         assert _is_punctuator_token("&") is True
         assert _is_punctuator_token("(") is True
         assert _is_punctuator_token(")") is True
         assert _is_punctuator_token("...") is True
         assert _is_punctuator_token(":") is True
         assert _is_punctuator_token("=") is True
```

### Comparing `graphql_core-3.3.0a2/tests/language/test_location.py` & `graphql_core-3.3.0a3/tests/language/test_location.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/language/test_parser.py` & `graphql_core-3.3.0a3/tests/language/test_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 from pytest import raises
 
 from graphql.error import GraphQLSyntaxError
 from graphql.language import (
     ArgumentNode,
     DefinitionNode,
     DocumentNode,
+    ErrorBoundaryNode,
     FieldNode,
     IntValueNode,
+    ListNullabilityOperatorNode,
     ListTypeNode,
     ListValueNode,
     NamedTypeNode,
     NameNode,
+    NonNullAssertionNode,
     NonNullTypeNode,
+    NullabilityAssertionNode,
     NullValueNode,
     ObjectFieldNode,
     ObjectValueNode,
     OperationDefinitionNode,
     OperationType,
     SelectionSetNode,
     Source,
@@ -42,23 +46,36 @@
 except ImportError:  # Python < 3.10
     from typing_extensions import TypeAlias
 
 
 Location: TypeAlias = Optional[Tuple[int, int]]
 
 
+def parse_ccn(source: str) -> DocumentNode:
+    return parse(source, experimental_client_controlled_nullability=True)
+
+
 def assert_syntax_error(text: str, message: str, location: Location) -> None:
     with raises(GraphQLSyntaxError) as exc_info:
         parse(text)
     error = exc_info.value
     assert error.message == f"Syntax Error: {message}"
     assert error.description == message
     assert error.locations == [location]
 
 
+def assert_syntax_error_ccn(text: str, message: str, location: Location) -> None:
+    with raises(GraphQLSyntaxError) as exc_info:
+        parse_ccn(text)
+    error = exc_info.value
+    assert error.message == f"Syntax Error: {message}"
+    assert error.description == message
+    assert error.locations == [location]
+
+
 def describe_parser():
     def parse_provides_useful_errors():
         with raises(GraphQLSyntaxError) as exc_info:
             parse("{")
         error = exc_info.value
         assert error.message == "Syntax Error: Expected Name, found <EOF>."
         assert error.positions == [1]
@@ -94,14 +111,30 @@
 
             MyQuery.graphql:1:6
             1 | query
               |      ^
             """
         )
 
+    def limits_maximum_number_of_tokens():
+        parse("{ foo }", max_tokens=3)
+        with raises(
+            GraphQLSyntaxError,
+            match="Syntax Error:"
+            r" Document contains more that 2 tokens\. Parsing aborted\.",
+        ):
+            parse("{ foo }", max_tokens=2)
+        parse('{ foo(bar: "baz") }', max_tokens=8)
+        with raises(
+            GraphQLSyntaxError,
+            match="Syntax Error:"
+            r" Document contains more that 7 tokens\. Parsing aborted\.",
+        ):
+            parse('{ foo(bar: "baz") }', max_tokens=7)
+
     def parses_variable_inline_values():
         parse("{ field(complex: { a: { b: [ $var ] } }) }")
 
     def parses_constant_default_values():
         assert_syntax_error(
             "query Foo($x: Complex = { a: { b: [ $var ] } }) { field }",
             "Unexpected variable '$var' in constant value.",
@@ -156,15 +189,15 @@
         assert len(arguments) == 1
         value = arguments[0].value
         assert isinstance(value, StringValueNode)
         assert value.value == "Has a \u0A0A multi-byte character."
 
     # noinspection PyShadowingNames
     def parses_kitchen_sink(kitchen_sink_query):  # noqa: F811
-        parse(kitchen_sink_query)
+        parse_ccn(kitchen_sink_query)
 
     def allows_non_keywords_anywhere_a_name_is_allowed():
         non_keywords = (
             "on",
             "fragment",
             "query",
             "mutation",
@@ -219,14 +252,222 @@
             """
             subscription Foo {
               subscriptionField
             }
             """
         )
 
+    def parses_required_field():
+        doc = parse_ccn("{ requiredField! }")
+        assert isinstance(doc, DocumentNode)
+        definitions = doc.definitions
+        assert isinstance(definitions, tuple)
+        assert len(definitions) == 1
+        definition = cast(OperationDefinitionNode, definitions[0])
+        selection_set: Optional[SelectionSetNode] = definition.selection_set
+        assert isinstance(selection_set, SelectionSetNode)
+        selections = selection_set.selections
+        assert isinstance(selections, tuple)
+        assert len(selections) == 1
+        field = selections[0]
+        assert isinstance(field, FieldNode)
+        nullability_assertion = field.nullability_assertion
+        assert isinstance(nullability_assertion, NonNullAssertionNode)
+        assert nullability_assertion.loc == (15, 16)
+        assert nullability_assertion.nullability_assertion is None
+
+    def parses_optional_field():
+        parse_ccn("{ optionalField? }")
+
+    def does_not_parse_field_with_multiple_designators():
+        assert_syntax_error_ccn(
+            "{ optionalField?! }", "Expected Name, found '!'.", (1, 17)
+        )
+        assert_syntax_error_ccn(
+            "{ optionalField!? }", "Expected Name, found '?'.", (1, 17)
+        )
+
+    def parses_required_with_alias():
+        parse_ccn("{ requiredField: field! }")
+
+    def parses_optional_with_alias():
+        parse_ccn("{ requiredField: field? }")
+
+    def does_not_parse_aliased_field_with_bang_on_left_of_colon():
+        assert_syntax_error_ccn(
+            "{ requiredField!: field }", "Expected Name, found ':'.", (1, 17)
+        )
+
+    def does_not_parse_aliased_field_with_question_mark_on_left_of_colon():
+        assert_syntax_error_ccn(
+            "{ requiredField?: field }", "Expected Name, found ':'.", (1, 17)
+        )
+
+    def does_not_parse_aliased_field_with_bang_on_left_and_right_of_colon():
+        assert_syntax_error_ccn(
+            "{ requiredField!: field! }", "Expected Name, found ':'.", (1, 17)
+        )
+
+    def does_not_parse_aliased_field_with_question_mark_on_left_and_right_of_colon():
+        assert_syntax_error_ccn(
+            "{ requiredField?: field? }", "Expected Name, found ':'.", (1, 17)
+        )
+
+    def does_not_parse_designator_on_query():
+        assert_syntax_error_ccn("query? { field }", "Expected '{', found '?'.", (1, 6))
+
+    def parses_required_within_fragment():
+        parse_ccn("fragment MyFragment on Query { field! }")
+
+    def parses_optional_within_fragment():
+        parse_ccn("fragment MyFragment on Query { field? }")
+
+    def parses_field_with_required_list_elements():
+        doc = parse_ccn("{ field[!] }")
+        assert isinstance(doc, DocumentNode)
+        definitions = doc.definitions
+        assert isinstance(definitions, tuple)
+        assert len(definitions) == 1
+        definition = cast(OperationDefinitionNode, definitions[0])
+        selection_set: Optional[SelectionSetNode] = definition.selection_set
+        assert isinstance(selection_set, SelectionSetNode)
+        selections = selection_set.selections
+        assert isinstance(selections, tuple)
+        assert len(selections) == 1
+        field = selections[0]
+        assert isinstance(field, FieldNode)
+        nullability_assertion: Optional[
+            NullabilityAssertionNode
+        ] = field.nullability_assertion
+        assert isinstance(nullability_assertion, ListNullabilityOperatorNode)
+        assert nullability_assertion.loc == (7, 10)
+        nullability_assertion = nullability_assertion.nullability_assertion
+        assert isinstance(nullability_assertion, NonNullAssertionNode)
+        assert nullability_assertion.loc == (8, 9)
+        assert nullability_assertion.nullability_assertion is None
+
+    def parses_field_with_optional_list_elements():
+        doc = parse_ccn("{ field[?] }")
+        assert isinstance(doc, DocumentNode)
+        definitions = doc.definitions
+        assert isinstance(definitions, tuple)
+        assert len(definitions) == 1
+        definition = cast(OperationDefinitionNode, definitions[0])
+        selection_set: Optional[SelectionSetNode] = definition.selection_set
+        assert isinstance(selection_set, SelectionSetNode)
+        selections = selection_set.selections
+        assert isinstance(selections, tuple)
+        assert len(selections) == 1
+        field = selections[0]
+        assert isinstance(field, FieldNode)
+        nullability_assertion: Optional[
+            NullabilityAssertionNode
+        ] = field.nullability_assertion
+        assert isinstance(nullability_assertion, ListNullabilityOperatorNode)
+        assert nullability_assertion.loc == (7, 10)
+        nullability_assertion = nullability_assertion.nullability_assertion
+        assert isinstance(nullability_assertion, ErrorBoundaryNode)
+        assert nullability_assertion.loc == (8, 9)
+        assert nullability_assertion.nullability_assertion is None
+
+    def parses_field_with_required_list():
+        doc = parse_ccn("{ field[]! }")
+        assert isinstance(doc, DocumentNode)
+        definitions = doc.definitions
+        assert isinstance(definitions, tuple)
+        assert len(definitions) == 1
+        definition = cast(OperationDefinitionNode, definitions[0])
+        selection_set: Optional[SelectionSetNode] = definition.selection_set
+        assert isinstance(selection_set, SelectionSetNode)
+        selections = selection_set.selections
+        assert isinstance(selections, tuple)
+        assert len(selections) == 1
+        field = selections[0]
+        assert isinstance(field, FieldNode)
+        nullability_assertion: Optional[
+            NullabilityAssertionNode
+        ] = field.nullability_assertion
+        assert isinstance(nullability_assertion, NonNullAssertionNode)
+        assert nullability_assertion.loc == (7, 10)
+        nullability_assertion = nullability_assertion.nullability_assertion
+        assert isinstance(nullability_assertion, ListNullabilityOperatorNode)
+        assert nullability_assertion.loc == (7, 9)
+        assert nullability_assertion.nullability_assertion is None
+
+    def parses_field_with_optional_list():
+        doc = parse_ccn("{ field[]? }")
+        assert isinstance(doc, DocumentNode)
+        definitions = doc.definitions
+        assert isinstance(definitions, tuple)
+        assert len(definitions) == 1
+        definition = cast(OperationDefinitionNode, definitions[0])
+        selection_set: Optional[SelectionSetNode] = definition.selection_set
+        assert isinstance(selection_set, SelectionSetNode)
+        selections = selection_set.selections
+        assert isinstance(selections, tuple)
+        assert len(selections) == 1
+        field = selections[0]
+        assert isinstance(field, FieldNode)
+        nullability_assertion: Optional[
+            NullabilityAssertionNode
+        ] = field.nullability_assertion
+        assert isinstance(nullability_assertion, ErrorBoundaryNode)
+        assert nullability_assertion.loc == (7, 10)
+        nullability_assertion = nullability_assertion.nullability_assertion
+        assert isinstance(nullability_assertion, ListNullabilityOperatorNode)
+        assert nullability_assertion.loc == (7, 9)
+        assert nullability_assertion.nullability_assertion is None
+
+    def parses_field_with_mixed_list_elements():
+        doc = parse_ccn("{ field[[[?]!]]! }")
+        assert isinstance(doc, DocumentNode)
+        definitions = doc.definitions
+        assert isinstance(definitions, tuple)
+        assert len(definitions) == 1
+        definition = cast(OperationDefinitionNode, definitions[0])
+        selection_set: Optional[SelectionSetNode] = definition.selection_set
+        assert isinstance(selection_set, SelectionSetNode)
+        selections = selection_set.selections
+        assert isinstance(selections, tuple)
+        assert len(selections) == 1
+        field = selections[0]
+        assert isinstance(field, FieldNode)
+        nullability_assertion: Optional[
+            NullabilityAssertionNode
+        ] = field.nullability_assertion
+        assert isinstance(nullability_assertion, NonNullAssertionNode)
+        assert nullability_assertion.loc == (7, 16)
+        nullability_assertion = nullability_assertion.nullability_assertion
+        assert isinstance(nullability_assertion, ListNullabilityOperatorNode)
+        assert nullability_assertion.loc == (7, 15)
+        nullability_assertion = nullability_assertion.nullability_assertion
+        assert isinstance(nullability_assertion, ListNullabilityOperatorNode)
+        assert nullability_assertion.loc == (8, 14)
+        nullability_assertion = nullability_assertion.nullability_assertion
+        assert isinstance(nullability_assertion, NonNullAssertionNode)
+        assert nullability_assertion.loc == (9, 13)
+        nullability_assertion = nullability_assertion.nullability_assertion
+        assert isinstance(nullability_assertion, ListNullabilityOperatorNode)
+        assert nullability_assertion.loc == (9, 12)
+        nullability_assertion = nullability_assertion.nullability_assertion
+        assert isinstance(nullability_assertion, ErrorBoundaryNode)
+        assert nullability_assertion.loc == (10, 11)
+        assert nullability_assertion.nullability_assertion is None
+
+    def does_not_parse_field_with_unbalanced_brackets():
+        assert_syntax_error_ccn("{ field[[] }", "Expected ']', found '}'.", (1, 12))
+        assert_syntax_error_ccn("{ field[]] }", "Expected Name, found ']'.", (1, 10))
+        assert_syntax_error_ccn("{ field] }", "Expected Name, found ']'.", (1, 8))
+        assert_syntax_error_ccn("{ field[ }", "Expected ']', found '}'.", (1, 10))
+
+    def does_not_parse_field_with_assorted_invalid_nullability_designators():
+        assert_syntax_error_ccn("{ field[][] }", "Expected Name, found '['.", (1, 10))
+        assert_syntax_error_ccn("{ field[!!] }", "Expected ']', found '!'.", (1, 10))
+        assert_syntax_error_ccn("{ field[]?! }", "Expected Name, found '!'.", (1, 11))
+
     def creates_ast():
         doc = parse(
             dedent(
                 """
                 {
                   node(id: 4) {
                     id,
@@ -273,14 +514,15 @@
         assert name.value == "id"
         value = argument.value
         assert isinstance(value, ValueNode)
         assert isinstance(value, IntValueNode)
         assert value.loc == (13, 14)
         assert value.value == "4"
         assert argument.loc == (9, 14)
+        assert field.nullability_assertion is None
         assert field.directives == ()
         selection_set = field.selection_set
         assert isinstance(selection_set, SelectionSetNode)
         selections = selection_set.selections
         assert isinstance(selections, tuple)
         assert len(selections) == 2
         field = selections[0]
@@ -288,36 +530,27 @@
         assert field.loc == (22, 24)
         assert field.alias is None
         name = field.name
         assert isinstance(name, NameNode)
         assert name.loc == (22, 24)
         assert name.value == "id"
         assert field.arguments == ()
-        assert field.directives == ()
-        assert field.selection_set is None
-        field = selections[0]
-        assert isinstance(field, FieldNode)
-        assert field.loc == (22, 24)
-        assert field.alias is None
-        name = field.name
-        assert isinstance(name, NameNode)
-        assert name.loc == (22, 24)
-        assert name.value == "id"
-        assert field.arguments == ()
+        assert field.nullability_assertion is None
         assert field.directives == ()
         assert field.selection_set is None
         field = selections[1]
         assert isinstance(field, FieldNode)
         assert field.loc == (30, 34)
         assert field.alias is None
         name = field.name
         assert isinstance(name, NameNode)
         assert name.loc == (30, 34)
         assert name.value == "name"
         assert field.arguments == ()
+        assert field.nullability_assertion is None
         assert field.directives == ()
         assert field.selection_set is None
 
     def creates_ast_from_nameless_query_without_variables():
         doc = parse(
             dedent(
                 """
@@ -352,14 +585,15 @@
         assert field.loc == (10, 27)
         assert field.alias is None
         name = field.name
         assert isinstance(name, NameNode)
         assert name.loc == (10, 14)
         assert name.value == "node"
         assert field.arguments == ()
+        assert field.nullability_assertion is None
         assert field.directives == ()
         selection_set = field.selection_set
         assert isinstance(selection_set, SelectionSetNode)
         assert selection_set.loc == (15, 27)
         selections = selection_set.selections
         assert isinstance(selections, tuple)
         assert len(selections) == 1
@@ -368,14 +602,15 @@
         assert field.loc == (21, 23)
         assert field.alias is None
         name = field.name
         assert isinstance(name, NameNode)
         assert name.loc == (21, 23)
         assert name.value == "id"
         assert field.arguments == ()
+        assert field.nullability_assertion is None
         assert field.directives == ()
         assert field.selection_set is None
 
     def allows_parsing_without_source_location_information():
         result = parse("{ id }", no_location=True)
         assert result.loc is None
```

### Comparing `graphql_core-3.3.0a2/tests/language/test_predicates.py` & `graphql_core-3.3.0a3/tests/language/test_predicates.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from graphql.language import (
     Node,
     ast,
     is_const_value_node,
     is_definition_node,
     is_executable_definition_node,
+    is_nullability_assertion_node,
     is_selection_node,
     is_type_definition_node,
     is_type_extension_node,
     is_type_node,
     is_type_system_definition_node,
     is_type_system_extension_node,
     is_value_node,
@@ -74,14 +75,22 @@
         assert filter_nodes(is_selection_node) == [
             "field",
             "fragment_spread",
             "inline_fragment",
             "selection",
         ]
 
+    def check_nullability_assertion_node():
+        assert filter_nodes(is_nullability_assertion_node) == [
+            "error_boundary",
+            "list_nullability_operator",
+            "non_null_assertion",
+            "nullability_assertion",
+        ]
+
     def check_value_node():
         assert filter_nodes(is_value_node) == [
             "boolean_value",
             "enum_value",
             "float_value",
             "int_value",
             "list_value",
```

### Comparing `graphql_core-3.3.0a2/tests/language/test_print_string.py` & `graphql_core-3.3.0a3/tests/language/test_print_string.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/language/test_printer.py` & `graphql_core-3.3.0a3/tests/language/test_printer.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,19 +126,25 @@
               id
             }
             """
         fragment_with_variable = parse(source, allow_legacy_fragment_variables=True)
         assert print_ast(fragment_with_variable) == dedent(source)
 
     def prints_kitchen_sink_without_altering_ast(kitchen_sink_query):  # noqa: F811
-        ast = parse(kitchen_sink_query, no_location=True)
+        ast = parse(
+            kitchen_sink_query,
+            no_location=True,
+            experimental_client_controlled_nullability=True,
+        )
 
         ast_before_print_call = deepcopy(ast)
         printed = print_ast(ast)
-        printed_ast = parse(printed, no_location=True)
+        printed_ast = parse(
+            printed, no_location=True, experimental_client_controlled_nullability=True
+        )
         assert printed_ast == ast
         assert deepcopy(ast) == ast_before_print_call
 
         assert printed == dedent(
             r'''
             query queryName($foo: ComplexType, $site: Site = MOBILE) @onQuery {
               whoever123is: node(id: [123, 456]) {
@@ -147,14 +153,27 @@
                   field2 {
                     id
                     alias: field1(first: 10, after: $foo) @include(if: $foo) {
                       id
                       ...frag @onFragmentSpread
                     }
                   }
+                  field3!
+                  field4?
+                  requiredField5: field5!
+                  requiredSelectionSet(first: 10)! @directive {
+                    field
+                  }
+                  unsetListItemsRequiredList: listField[]!
+                  requiredListItemsUnsetList: listField[!]
+                  requiredListItemsRequiredList: listField[!]!
+                  unsetListItemsOptionalList: listField[]?
+                  optionalListItemsUnsetList: listField[?]
+                  optionalListItemsOptionalList: listField[?]?
+                  multidimensionalList: listField[[[!]!]!]!
                 }
                 ... @skip(unless: $foo) {
                   id
                 }
                 ... {
                   id
                 }
```

### Comparing `graphql_core-3.3.0a2/tests/language/test_schema_parser.py` & `graphql_core-3.3.0a3/tests/language/test_schema_parser.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/language/test_schema_printer.py` & `graphql_core-3.3.0a3/tests/language/test_schema_printer.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/language/test_source.py` & `graphql_core-3.3.0a3/tests/language/test_source.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/language/test_visitor.py` & `graphql_core-3.3.0a3/tests/language/test_visitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from copy import copy
 from functools import partial
-from typing import List, Optional, cast
+from typing import Any, List, Optional, cast
 
 from pytest import mark, raises
 
 from graphql.language import (
     BREAK,
     REMOVE,
     SKIP,
@@ -728,18 +728,18 @@
             ["leave", "selection_set", None],
             ["leave", "fragment_definition", None],
             ["leave", "document", None],
         ]
 
     # noinspection PyShadowingNames
     def visits_kitchen_sink(kitchen_sink_query):  # noqa: F811
-        ast = parse(kitchen_sink_query)
-        visited: List = []
+        ast = parse(kitchen_sink_query, experimental_client_controlled_nullability=True)
+        visited: List[Any] = []
         record = visited.append
-        arg_stack: List = []
+        arg_stack: List[Any] = []
         push = arg_stack.append
         pop = arg_stack.pop
 
         class TestVisitor(Visitor):
             @staticmethod
             def enter(*args):
                 node, key, parent = args[:3]
@@ -874,14 +874,280 @@
             ["leave", "name", "name", "directive"],
             ["leave", "directive", 0, None],
             ["leave", "fragment_spread", 1, None],
             ["leave", "selection_set", "selection_set", "field"],
             ["leave", "field", 1, None],
             ["leave", "selection_set", "selection_set", "field"],
             ["leave", "field", 0, None],
+            ["enter", "field", 1, None],
+            ["enter", "name", "name", "field"],
+            ["leave", "name", "name", "field"],
+            ["enter", "non_null_assertion", "nullability_assertion", "field"],
+            ["leave", "non_null_assertion", "nullability_assertion", "field"],
+            ["leave", "field", 1, None],
+            ["enter", "field", 2, None],
+            ["enter", "name", "name", "field"],
+            ["leave", "name", "name", "field"],
+            ["enter", "error_boundary", "nullability_assertion", "field"],
+            ["leave", "error_boundary", "nullability_assertion", "field"],
+            ["leave", "field", 2, None],
+            ["enter", "field", 3, None],
+            ["enter", "name", "alias", "field"],
+            ["leave", "name", "alias", "field"],
+            ["enter", "name", "name", "field"],
+            ["leave", "name", "name", "field"],
+            ["enter", "non_null_assertion", "nullability_assertion", "field"],
+            ["leave", "non_null_assertion", "nullability_assertion", "field"],
+            ["leave", "field", 3, None],
+            ["enter", "field", 4, None],
+            ["enter", "name", "name", "field"],
+            ["leave", "name", "name", "field"],
+            ["enter", "argument", 0, None],
+            ["enter", "name", "name", "argument"],
+            ["leave", "name", "name", "argument"],
+            ["enter", "int_value", "value", "argument"],
+            ["leave", "int_value", "value", "argument"],
+            ["leave", "argument", 0, None],
+            ["enter", "directive", 0, None],
+            ["enter", "name", "name", "directive"],
+            ["leave", "name", "name", "directive"],
+            ["leave", "directive", 0, None],
+            ["enter", "selection_set", "selection_set", "field"],
+            ["enter", "field", 0, None],
+            ["enter", "name", "name", "field"],
+            ["leave", "name", "name", "field"],
+            ["leave", "field", 0, None],
+            ["leave", "selection_set", "selection_set", "field"],
+            ["enter", "non_null_assertion", "nullability_assertion", "field"],
+            ["leave", "non_null_assertion", "nullability_assertion", "field"],
+            ["leave", "field", 4, None],
+            ["enter", "field", 5, None],
+            ["enter", "name", "alias", "field"],
+            ["leave", "name", "alias", "field"],
+            ["enter", "name", "name", "field"],
+            ["leave", "name", "name", "field"],
+            ["enter", "non_null_assertion", "nullability_assertion", "field"],
+            [
+                "enter",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "non_null_assertion",
+            ],
+            [
+                "leave",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "non_null_assertion",
+            ],
+            ["leave", "non_null_assertion", "nullability_assertion", "field"],
+            ["leave", "field", 5, None],
+            ["enter", "field", 6, None],
+            ["enter", "name", "alias", "field"],
+            ["leave", "name", "alias", "field"],
+            ["enter", "name", "name", "field"],
+            ["leave", "name", "name", "field"],
+            ["enter", "list_nullability_operator", "nullability_assertion", "field"],
+            [
+                "enter",
+                "non_null_assertion",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            [
+                "leave",
+                "non_null_assertion",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            ["leave", "list_nullability_operator", "nullability_assertion", "field"],
+            ["leave", "field", 6, None],
+            ["enter", "field", 7, None],
+            ["enter", "name", "alias", "field"],
+            ["leave", "name", "alias", "field"],
+            ["enter", "name", "name", "field"],
+            ["leave", "name", "name", "field"],
+            ["enter", "non_null_assertion", "nullability_assertion", "field"],
+            [
+                "enter",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "non_null_assertion",
+            ],
+            [
+                "enter",
+                "non_null_assertion",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            [
+                "leave",
+                "non_null_assertion",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            [
+                "leave",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "non_null_assertion",
+            ],
+            ["leave", "non_null_assertion", "nullability_assertion", "field"],
+            ["leave", "field", 7, None],
+            ["enter", "field", 8, None],
+            ["enter", "name", "alias", "field"],
+            ["leave", "name", "alias", "field"],
+            ["enter", "name", "name", "field"],
+            ["leave", "name", "name", "field"],
+            ["enter", "error_boundary", "nullability_assertion", "field"],
+            [
+                "enter",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "error_boundary",
+            ],
+            [
+                "leave",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "error_boundary",
+            ],
+            ["leave", "error_boundary", "nullability_assertion", "field"],
+            ["leave", "field", 8, None],
+            ["enter", "field", 9, None],
+            ["enter", "name", "alias", "field"],
+            ["leave", "name", "alias", "field"],
+            ["enter", "name", "name", "field"],
+            ["leave", "name", "name", "field"],
+            ["enter", "list_nullability_operator", "nullability_assertion", "field"],
+            [
+                "enter",
+                "error_boundary",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            [
+                "leave",
+                "error_boundary",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            ["leave", "list_nullability_operator", "nullability_assertion", "field"],
+            ["leave", "field", 9, None],
+            ["enter", "field", 10, None],
+            ["enter", "name", "alias", "field"],
+            ["leave", "name", "alias", "field"],
+            ["enter", "name", "name", "field"],
+            ["leave", "name", "name", "field"],
+            ["enter", "error_boundary", "nullability_assertion", "field"],
+            [
+                "enter",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "error_boundary",
+            ],
+            [
+                "enter",
+                "error_boundary",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            [
+                "leave",
+                "error_boundary",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            [
+                "leave",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "error_boundary",
+            ],
+            ["leave", "error_boundary", "nullability_assertion", "field"],
+            ["leave", "field", 10, None],
+            ["enter", "field", 11, None],
+            ["enter", "name", "alias", "field"],
+            ["leave", "name", "alias", "field"],
+            ["enter", "name", "name", "field"],
+            ["leave", "name", "name", "field"],
+            ["enter", "non_null_assertion", "nullability_assertion", "field"],
+            [
+                "enter",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "non_null_assertion",
+            ],
+            [
+                "enter",
+                "non_null_assertion",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            [
+                "enter",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "non_null_assertion",
+            ],
+            [
+                "enter",
+                "non_null_assertion",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            [
+                "enter",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "non_null_assertion",
+            ],
+            [
+                "enter",
+                "non_null_assertion",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            [
+                "leave",
+                "non_null_assertion",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            [
+                "leave",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "non_null_assertion",
+            ],
+            [
+                "leave",
+                "non_null_assertion",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            [
+                "leave",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "non_null_assertion",
+            ],
+            [
+                "leave",
+                "non_null_assertion",
+                "nullability_assertion",
+                "list_nullability_operator",
+            ],
+            [
+                "leave",
+                "list_nullability_operator",
+                "nullability_assertion",
+                "non_null_assertion",
+            ],
+            ["leave", "non_null_assertion", "nullability_assertion", "field"],
+            ["leave", "field", 11, None],
             ["leave", "selection_set", "selection_set", "inline_fragment"],
             ["leave", "inline_fragment", 1, None],
             ["enter", "inline_fragment", 2, None],
             ["enter", "directive", 0, None],
             ["enter", "name", "name", "directive"],
             ["leave", "name", "name", "directive"],
             ["enter", "argument", 0, None],
```

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_cached_property.py` & `graphql_core-3.3.0a3/tests/pyutils/test_cached_property.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_convert_case.py` & `graphql_core-3.3.0a3/tests/pyutils/test_convert_case.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_description.py` & `graphql_core-3.3.0a3/tests/pyutils/test_description.py`

 * *Files 13% similar despite different names*

```diff
@@ -105,102 +105,74 @@
             unregister_description("foo")  # type: ignore
 
     def describe_graphql_types():
         def graphql_named_type():
             named_type = GraphQLNamedType(name="Foo", description="not lazy")
             assert named_type.name == "Foo"
             assert named_type.description == "not lazy"
-            with raises(TypeError, match="Expected name to be a string\\."):
-                GraphQLNamedType(name=lazy_string)
-            with raises(TypeError, match="The description must be a string\\."):
-                GraphQLNamedType(name="Foo", description=lazy_string)
             with registered(LazyString):
                 named_type = GraphQLNamedType(name="Foo", description=lazy_string)
                 assert named_type.description is lazy_string
                 assert str(named_type.description).endswith("lazy?")
-                with raises(TypeError, match="Expected name to be a string\\."):
-                    GraphQLNamedType(name=lazy_string)
 
         def graphql_field():
             field = GraphQLField(GraphQLString, description="not lazy")
             assert field.description == "not lazy"
             field = GraphQLField(GraphQLString, deprecation_reason="not lazy")
             assert field.deprecation_reason == "not lazy"
-            with raises(TypeError, match="The description must be a string\\."):
-                GraphQLField(GraphQLString, description=lazy_string)
-            with raises(TypeError, match="The deprecation reason must be a string\\."):
-                GraphQLField(GraphQLString, deprecation_reason=lazy_string)
+            GraphQLField(GraphQLString, description=lazy_string)
             with registered(LazyString):
                 field = GraphQLField(
                     GraphQLString,
                     description=lazy_string,
                     deprecation_reason=lazy_string,
                 )
                 assert field.description is lazy_string
                 assert str(field.description).endswith("lazy?")
                 assert field.deprecation_reason is lazy_string
                 assert str(field.deprecation_reason).endswith("lazy?")
 
         def graphql_argument():
             arg = GraphQLArgument(GraphQLString, description="not lazy")
             assert arg.description == "not lazy"
-            with raises(TypeError, match="Argument description must be a string\\."):
-                GraphQLArgument(GraphQLString, description=lazy_string)
             with registered(LazyString):
                 arg = GraphQLArgument(GraphQLString, description=lazy_string)
                 assert arg.description is lazy_string
                 assert str(arg.description).endswith("lazy?")
 
         def graphql_enum_value():
             value = GraphQLEnumValue(description="not lazy")
             assert value.description == "not lazy"
             value = GraphQLEnumValue(deprecation_reason="not lazy")
             assert value.deprecation_reason == "not lazy"
-            with raises(
-                TypeError, match="The description of the enum value must be a string\\."
-            ):
-                GraphQLEnumValue(description=lazy_string)
-            with raises(
-                TypeError,
-                match="The deprecation reason for the enum value must be a string\\.",
-            ):
-                GraphQLEnumValue(deprecation_reason=lazy_string)
             with registered(LazyString):
                 value = GraphQLEnumValue(
                     description=lazy_string, deprecation_reason=lazy_string
                 )
                 assert value.description is lazy_string
                 assert str(value.description).endswith("lazy?")
                 assert value.deprecation_reason is lazy_string
                 assert str(value.deprecation_reason).endswith("lazy?")
 
         def graphql_input_field():
             field = GraphQLInputField(GraphQLString, description="not lazy")
             assert field.description == "not lazy"
-            with raises(TypeError, match="Input field description must be a string\\."):
-                GraphQLInputField(GraphQLString, description=lazy_string)
             with registered(LazyString):
                 field = GraphQLInputField(GraphQLString, description=lazy_string)
                 assert field.description is lazy_string
                 assert str(field.description).endswith("lazy?")
 
         def graphql_directive():
             directive = GraphQLDirective("Foo", [], description="not lazy")
             assert directive.name == "Foo"
             assert directive.description == "not lazy"
-            with raises(TypeError, match="Expected name to be a string\\."):
-                GraphQLDirective(lazy_string, [])
-            with raises(TypeError, match="Foo description must be a string\\."):
-                GraphQLDirective("Foo", [], description=lazy_string)
             with registered(LazyString):
                 directive = GraphQLDirective("Foo", [], description=lazy_string)
                 assert directive.description is lazy_string
                 assert str(directive.description).endswith("lazy?")
-                with raises(TypeError, match="Expected name to be a string\\."):
-                    GraphQLDirective(lazy_string, [])
 
     def handels_introspection():
         class Lazy:
             def __init__(self, text: str):
                 self.text = text
                 self.evaluated = False
```

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_did_you_mean.py` & `graphql_core-3.3.0a3/tests/pyutils/test_did_you_mean.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_format_list.py` & `graphql_core-3.3.0a3/tests/pyutils/test_format_list.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_group_by.py` & `graphql_core-3.3.0a3/tests/pyutils/test_group_by.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_identity_func.py` & `graphql_core-3.3.0a3/tests/pyutils/test_identity_func.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_inspect.py` & `graphql_core-3.3.0a3/tests/pyutils/test_inspect.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_is_awaitable.py` & `graphql_core-3.3.0a3/tests/pyutils/test_is_awaitable.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,53 +57,63 @@
         def some_generator():
             yield True  # pragma: no cover
 
         assert not isawaitable(some_generator())
         assert not is_awaitable(some_generator())
 
     def declines_a_coroutine_function():
-        async def some_coroutine():
+        async def some_async_function():
             return True  # pragma: no cover
 
-        assert not isawaitable(some_coroutine)
-        assert not is_awaitable(some_coroutine)
+        assert not isawaitable(some_async_function)
+        assert not is_awaitable(some_async_function)
 
     @mark.asyncio
-    @mark.filterwarnings("ignore:.* was never awaited:RuntimeWarning")
     async def recognizes_a_coroutine_object():
-        async def some_coroutine():
-            return False  # pragma: no cover
+        async def some_async_function():
+            return True
 
-        assert isawaitable(some_coroutine())
-        assert is_awaitable(some_coroutine())
+        some_coroutine = some_async_function()
+
+        assert isawaitable(some_coroutine)
+        assert is_awaitable(some_coroutine)
+
+        assert await some_coroutine is True
 
     @mark.filterwarnings("ignore::Warning")  # Deprecation and Runtime warnings
     @mark.skipif(
         python_version >= (3, 11),
         reason="Generator-based coroutines not supported any more since Python 3.11",
     )
-    def recognizes_an_old_style_coroutine():  # pragma: no cover
-        @asyncio.coroutine
-        def some_old_style_coroutine():
-            yield False  # pragma: no cover
-
-        assert is_awaitable(some_old_style_coroutine())
-        assert is_awaitable(some_old_style_coroutine())
+    async def recognizes_an_old_style_coroutine():  # pragma: no cover
+        @asyncio.coroutine  # type: ignore
+        def some_function():
+            yield True
+
+        some_old_style_coroutine = some_function()
+        assert is_awaitable(some_old_style_coroutine)
+        assert is_awaitable(some_old_style_coroutine)
 
     @mark.asyncio
-    @mark.filterwarnings("ignore:.* was never awaited:RuntimeWarning")
     async def recognizes_a_future_object():
-        async def some_coroutine():
-            return False  # pragma: no cover
+        async def some_async_function():
+            return True
 
-        some_future = asyncio.ensure_future(some_coroutine())
+        some_coroutine = some_async_function()
+        some_future = asyncio.ensure_future(some_coroutine)
 
         assert is_awaitable(some_future)
         assert is_awaitable(some_future)
 
-    @mark.filterwarnings("ignore:.* was never awaited:RuntimeWarning")
-    def declines_an_async_generator():
-        async def some_async_generator():
-            yield True  # pragma: no cover
+        assert await some_future is True
+
+    @mark.asyncio
+    async def declines_an_async_generator():
+        async def some_async_generator_function():
+            yield True
+
+        some_async_generator = some_async_generator_function()
+
+        assert not isawaitable(some_async_generator)
+        assert not is_awaitable(some_async_generator)
 
-        assert not isawaitable(some_async_generator())
-        assert not is_awaitable(some_async_generator())
+        assert await some_async_generator.__anext__() is True
```

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_is_iterable.py` & `graphql_core-3.3.0a3/tests/pyutils/test_is_iterable.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_merge_kwargs.py` & `graphql_core-3.3.0a3/tests/pyutils/test_merge_kwargs.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_natural_compare.py` & `graphql_core-3.3.0a3/tests/pyutils/test_natural_compare.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_path.py` & `graphql_core-3.3.0a3/tests/pyutils/test_path.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_simple_pub_sub.py` & `graphql_core-3.3.0a3/tests/pyutils/test_simple_pub_sub.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from asyncio import sleep
-from inspect import isawaitable
 
 from pytest import mark, raises
 
-from graphql.pyutils import SimplePubSub
+from graphql.pyutils import SimplePubSub, is_awaitable
 
 
 def describe_simple_pub_sub():
     @mark.asyncio
     async def subscribe_async_iterator_mock():
         pubsub = SimplePubSub()
         iterator = pubsub.get_subscriber()
@@ -18,17 +17,17 @@
 
         # Read payloads
         assert await iterator.__anext__() == "Apple"
         assert await iterator.__anext__() == "Banana"
 
         # Read ahead
         i3 = await iterator.__anext__()
-        assert isawaitable(i3)
+        assert is_awaitable(i3)
         i4 = await iterator.__anext__()
-        assert isawaitable(i4)
+        assert is_awaitable(i4)
 
         # Publish
         assert pubsub.emit("Coconut") is True
         assert pubsub.emit("Durian") is True
 
         # Await out of order to get correct results
         assert await i4 == "Durian"
```

### Comparing `graphql_core-3.3.0a2/tests/pyutils/test_suggestion_list.py` & `graphql_core-3.3.0a3/tests/pyutils/test_suggestion_list.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/star_wars_data.py` & `graphql_core-3.3.0a3/tests/star_wars_data.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/star_wars_schema.py` & `graphql_core-3.3.0a3/tests/star_wars_schema.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/test_docs.py` & `graphql_core-3.3.0a3/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/test_star_wars_introspection.py` & `graphql_core-3.3.0a3/tests/test_star_wars_introspection.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/test_star_wars_query.py` & `graphql_core-3.3.0a3/tests/test_star_wars_query.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/test_star_wars_validation.py` & `graphql_core-3.3.0a3/tests/test_star_wars_validation.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/test_user_registry.py` & `graphql_core-3.3.0a3/tests/test_user_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 This is an additional end-to-end test and demo for running the basic GraphQL
 operations on a simulated user registry database backend.
 """
 
 from asyncio import create_task, sleep, wait
 from collections import defaultdict
 from enum import Enum
-from inspect import isawaitable
-from typing import Any, Dict, List, NamedTuple, Optional
+from typing import Any, AsyncIterable, Dict, List, NamedTuple, Optional
 
 from pytest import fixture, mark
 
 from graphql import (
     GraphQLArgument,
     GraphQLBoolean,
     GraphQLEnumType,
@@ -25,16 +24,15 @@
     GraphQLObjectType,
     GraphQLSchema,
     GraphQLString,
     graphql,
     parse,
     subscribe,
 )
-from graphql.execution.map_async_iterator import MapAsyncIterator
-from graphql.pyutils import SimplePubSub, SimplePubSubIterator
+from graphql.pyutils import SimplePubSub, SimplePubSubIterator, is_awaitable
 
 
 class User(NamedTuple):
     """A simple user object class."""
 
     firstName: str
     lastName: str
@@ -154,15 +152,15 @@
 
 
 # noinspection PyShadowingBuiltins
 async def subscribe_user(_root, info, id=None):
     """Subscribe to mutations of a specific user object or all user objects"""
     async_iterator = info.context["registry"].event_iterator(id)
     async for event in async_iterator:
-        yield await event if isawaitable(event) else event  # pragma: no cover exit
+        yield await event if is_awaitable(event) else event  # pragma: no cover exit
 
 
 # noinspection PyShadowingBuiltins,PyUnusedLocal
 async def resolve_subscription_user(event, info, id):
     """Resolver function for user subscriptions"""
     user = event["user"]
     mutation = MutationEnum(event["mutation"]).value
@@ -406,36 +404,36 @@
                     mutation
                     user { id, firstName, lastName, tweets, verified }
                 }
             }
             """
 
         variables = {"userId": "0"}
-        subscription_one = await subscribe(
+        subscription_one = subscribe(
             schema, parse(query), context_value=context, variable_values=variables
         )
-        assert isinstance(subscription_one, MapAsyncIterator)
+        assert isinstance(subscription_one, AsyncIterable)
 
         query = """
             subscription {
                 subscribeUser(id: null) {
                     mutation
                     user { id, firstName, lastName, tweets, verified }
                 }
             }
             """
 
-        subscription_all = await subscribe(schema, parse(query), context_value=context)
-        assert isinstance(subscription_all, MapAsyncIterator)
+        subscription_all = subscribe(schema, parse(query), context_value=context)
+        assert isinstance(subscription_all, AsyncIterable)
 
         received_one = []
         received_all = []
 
         async def mutate_users():
-            await sleep(0)  # make sure subscribers are running
+            await sleep(2 / 512)  # make sure subscribers are running
             await graphql(
                 schema,
                 """
                 mutation {createUser(data: {
                     firstName: "John"
                     lastName: "Doe"
                     tweets: 42
@@ -500,16 +498,15 @@
         async def receive_all():
             async for result in subscription_all:  # type: ignore # pragma: no cover
                 received_all.append(result)
                 if len(received_all) == 6:  # pragma: no cover else
                     break
 
         tasks = [
-            create_task(task()) if create_task else task()
-            for task in (mutate_users, receive_one, receive_all)
+            create_task(task()) for task in (mutate_users, receive_one, receive_all)
         ]
         done, pending = await wait(tasks, timeout=1)
         assert not pending
 
         expected_data: List[Dict[str, Any]] = [
             {
                 "mutation": "CREATED",
```

### Comparing `graphql_core-3.3.0a2/tests/test_version.py` & `graphql_core-3.3.0a3/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/type/test_assert_name.py` & `graphql_core-3.3.0a3/tests/type/test_assert_name.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,14 @@
 from graphql.type import assert_enum_value_name, assert_name
 
 
 def describe_assert_name():
     def pass_through_valid_name():
         assert assert_name("_ValidName123") == "_ValidName123"
 
-    def throws_for_non_strings():
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            assert_name({})  # type: ignore
-        msg = str(exc_info.value)
-        assert msg == "Expected name to be a string."
-
     def throws_on_empty_strings():
         with raises(GraphQLError) as exc_info:
             assert_name("")
         msg = str(exc_info.value)
         assert msg == "Expected name to be a non-empty string."
 
     def throws_for_names_with_invalid_characters():
```

### Comparing `graphql_core-3.3.0a2/tests/type/test_custom_scalars.py` & `graphql_core-3.3.0a3/tests/type/test_custom_scalars.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/type/test_directives.py` & `graphql_core-3.3.0a3/tests/type/test_directives.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pytest import raises
 
 from graphql.error import GraphQLError
-from graphql.language import DirectiveDefinitionNode, DirectiveLocation, Node
+from graphql.language import DirectiveDefinitionNode, DirectiveLocation
 from graphql.type import GraphQLArgument, GraphQLDirective, GraphQLInt, GraphQLString
 
 
 def describe_type_system_directive():
     def can_create_instance():
         arg = GraphQLArgument(GraphQLString, description="arg description")
         node = DirectiveDefinitionNode()
@@ -128,59 +128,25 @@
         assert str(exc_info.value) == "Expected name to be a non-empty string."
         with raises(GraphQLError) as exc_info:
             GraphQLDirective("bad-name", [])
         assert str(exc_info.value) == (
             "Names must only contain [_a-zA-Z0-9] but 'bad-name' does not."
         )
 
-    def rejects_a_directive_with_incorrectly_typed_args():
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            GraphQLDirective("Foo", locations=[], args=["arg"])  # type: ignore
-        assert str(exc_info.value) == (
-            "Foo args must be a dict with argument names as keys."
-        )
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            GraphQLDirective(
-                "Foo",
-                locations=[],
-                args={1: GraphQLArgument(GraphQLString)},  # type: ignore
-            )
-        assert str(exc_info.value) == (
-            "Foo args must be a dict with argument names as keys."
-        )
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            GraphQLDirective(
-                "Foo",
-                locations=[],
-                args={"arg": GraphQLDirective("Bar", [])},  # type: ignore
-            )
-        assert str(exc_info.value) == (
-            "Foo args must be GraphQLArgument or input type objects."
-        )
-
     def rejects_a_directive_with_incorrectly_named_args():
         with raises(GraphQLError) as exc_info:
             GraphQLDirective(
                 "Foo",
                 locations=[DirectiveLocation.QUERY],
                 args={"bad-name": GraphQLArgument(GraphQLString)},
             )
         assert str(exc_info.value) == (
             "Names must only contain [_a-zA-Z0-9] but 'bad-name' does not."
         )
 
-    def rejects_a_directive_with_incorrectly_typed_repeatable_flag():
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            GraphQLDirective("Foo", locations=[], is_repeatable=None)  # type: ignore
-        assert str(exc_info.value) == "Foo is_repeatable flag must be True or False."
-
     def rejects_a_directive_with_undefined_locations():
         with raises(TypeError) as exc_info:
             # noinspection PyTypeChecker
             GraphQLDirective("Foo", locations=None)  # type: ignore
         assert str(exc_info.value) == (
             "Foo locations must be specified"
             " as a collection of DirectiveLocation enum values."
@@ -197,23 +163,7 @@
         with raises(TypeError) as exc_info:
             # noinspection PyTypeChecker
             GraphQLDirective("Foo", locations=["bad"])  # type: ignore
         assert str(exc_info.value) == (
             "Foo locations must be specified"
             " as a collection of DirectiveLocation enum values."
         )
-
-    def rejects_a_directive_with_incorrectly_typed_description():
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            GraphQLDirective(
-                "Foo", locations=[], description={"bad": True}  # type: ignore
-            )
-        assert str(exc_info.value) == "Foo description must be a string."
-
-    def rejects_a_directive_with_incorrectly_typed_ast_node():
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            GraphQLDirective("Foo", locations=[], ast_node=Node())  # type: ignore
-        assert str(exc_info.value) == (
-            "Foo AST node must be a DirectiveDefinitionNode."
-        )
```

### Comparing `graphql_core-3.3.0a2/tests/type/test_enum.py` & `graphql_core-3.3.0a3/tests/type/test_enum.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/type/test_extensions.py` & `graphql_core-3.3.0a3/tests/type/test_extensions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from typing import Any, Dict, cast
-
-from pytest import mark, param, raises
+from pytest import param
 
 from graphql.type import (
     GraphQLArgument,
     GraphQLDirective,
     GraphQLEnumType,
     GraphQLEnumValue,
     GraphQLField,
@@ -19,38 +17,28 @@
 
 
 dummy_type = GraphQLScalarType("DummyScalar")
 
 bad_extensions = [param([], id="list"), param({1: "ext"}, id="non_string_key")]
 
 
-def bad_extensions_msg(name: str) -> str:
-    return f"{name} extensions must be a dictionary with string keys."
-
-
 def describe_type_system_extensions():
     def describe_graphql_scalar_type():
         def without_extensions():
             some_scalar = GraphQLScalarType("SomeScalar")
             assert some_scalar.extensions == {}
             assert some_scalar.to_kwargs()["extensions"] == {}
 
         def with_extensions():
             scalar_extensions = {"SomeScalarExt": "scalar"}
             some_scalar = GraphQLScalarType("SomeScalar", extensions=scalar_extensions)
 
             assert some_scalar.extensions is scalar_extensions
             assert some_scalar.to_kwargs()["extensions"] is scalar_extensions
 
-        @mark.parametrize("extensions", bad_extensions)
-        def with_bad_extensions(extensions):
-            with raises(TypeError, match=bad_extensions_msg("SomeScalar")):
-                # noinspection PyTypeChecker
-                GraphQLScalarType("SomeScalar", extensions=extensions)
-
     def describe_graphql_object_type():
         def without_extensions():
             some_object = GraphQLObjectType(
                 "SomeObject",
                 {
                     "someField": GraphQLField(
                         dummy_type, {"someArg": GraphQLArgument(dummy_type)}
@@ -95,26 +83,14 @@
             some_arg = some_field.args["someArg"]
             assert some_arg.extensions is arg_extensions
 
             assert some_object.to_kwargs()["extensions"] is object_extensions
             assert some_field.to_kwargs()["extensions"] is field_extensions
             assert some_arg.to_kwargs()["extensions"] is arg_extensions
 
-        @mark.parametrize("extensions", bad_extensions)
-        def with_bad_extensions(extensions):
-            with raises(TypeError, match=bad_extensions_msg("SomeObject")):
-                # noinspection PyTypeChecker
-                GraphQLObjectType("SomeObject", {}, extensions=extensions)
-            with raises(TypeError, match=bad_extensions_msg("Field")):
-                # noinspection PyTypeChecker
-                GraphQLField(dummy_type, extensions=extensions)
-            with raises(TypeError, match=bad_extensions_msg("Argument")):
-                # noinspection PyTypeChecker
-                GraphQLArgument(dummy_type, extensions=extensions)
-
     def describe_graphql_interface_type():
         def without_extensions():
             some_interface = GraphQLInterfaceType(
                 "SomeInterface",
                 {
                     "someField": GraphQLField(
                         dummy_type, {"someArg": GraphQLArgument(dummy_type)}
@@ -159,20 +135,14 @@
             some_arg = some_field.args["someArg"]
             assert some_arg.extensions is arg_extensions
 
             assert some_interface.to_kwargs()["extensions"] is interface_extensions
             assert some_field.to_kwargs()["extensions"] is field_extensions
             assert some_arg.to_kwargs()["extensions"] is arg_extensions
 
-        @mark.parametrize("extensions", bad_extensions)
-        def with_bad_extensions(extensions):
-            with raises(TypeError, match=bad_extensions_msg("SomeInterface")):
-                # noinspection PyTypeChecker
-                GraphQLInterfaceType("SomeInterface", {}, extensions=extensions)
-
     def describe_graphql_union_type():
         def without_extensions():
             some_union = GraphQLUnionType("SomeUnion", [])
 
             assert some_union.extensions == {}
 
             assert some_union.to_kwargs()["extensions"] == {}
@@ -182,20 +152,14 @@
 
             some_union = GraphQLUnionType("SomeUnion", [], extensions=union_extensions)
 
             assert some_union.extensions is union_extensions
 
             assert some_union.to_kwargs()["extensions"] is union_extensions
 
-        @mark.parametrize("extensions", bad_extensions)
-        def with_bad_extensions(extensions):
-            with raises(TypeError, match=bad_extensions_msg("SomeUnion")):
-                # noinspection PyTypeChecker
-                GraphQLUnionType("SomeUnion", [], extensions=extensions)
-
     def describe_graphql_enum_type():
         def without_extensions():
             some_enum = GraphQLEnumType("SomeEnum", {"SOME_VALUE": None})
 
             assert some_enum.extensions == {}
             some_value = some_enum.values["SOME_VALUE"]
             assert some_value.extensions == {}
@@ -216,25 +180,14 @@
             assert some_enum.extensions is enum_extensions
             some_value = some_enum.values["SOME_VALUE"]
             assert some_value.extensions is value_extensions
 
             assert some_enum.to_kwargs()["extensions"] is enum_extensions
             assert some_value.to_kwargs()["extensions"] is value_extensions
 
-        @mark.parametrize("extensions", bad_extensions)
-        def with_bad_extensions(extensions):
-            with raises(TypeError, match=bad_extensions_msg("SomeEnum")):
-                # noinspection PyTypeChecker
-                GraphQLEnumType(
-                    "SomeEnum", cast(Dict[str, Any], {}), extensions=extensions
-                )
-            with raises(TypeError, match=bad_extensions_msg("Enum value")):
-                # noinspection PyTypeChecker
-                GraphQLEnumValue(extensions=extensions)
-
     def describe_graphql_input_object_type():
         def without_extensions():
             some_input_object = GraphQLInputObjectType(
                 "SomeInputObject", {"someInputField": GraphQLInputField(dummy_type)}
             )
 
             assert some_input_object.extensions == {}
@@ -263,23 +216,14 @@
             assert some_input_field.extensions is input_field_extensions
 
             assert (
                 some_input_object.to_kwargs()["extensions"] is input_object_extensions
             )
             assert some_input_field.to_kwargs()["extensions"] is input_field_extensions
 
-        @mark.parametrize("extensions", bad_extensions)
-        def with_bad_extensions(extensions):
-            with raises(TypeError, match=bad_extensions_msg("SomeInputObject")):
-                # noinspection PyTypeChecker
-                GraphQLInputObjectType("SomeInputObject", {}, extensions=extensions)
-            with raises(TypeError, match=bad_extensions_msg("Input field")):
-                # noinspection PyTypeChecker
-                GraphQLInputField(dummy_type, extensions=extensions)
-
     def describe_graphql_directive():
         def without_extensions():
             some_directive = GraphQLDirective(
                 "SomeDirective", [], {"someArg": GraphQLArgument(dummy_type)}
             )
 
             assert some_directive.extensions == {}
@@ -303,20 +247,14 @@
             assert some_directive.extensions is directive_extensions
             some_arg = some_directive.args["someArg"]
             assert some_arg.extensions is arg_extensions
 
             assert some_directive.to_kwargs()["extensions"] is directive_extensions
             assert some_arg.to_kwargs()["extensions"] is arg_extensions
 
-        @mark.parametrize("extensions", bad_extensions)
-        def with_bad_extensions(extensions):
-            with raises(TypeError, match=bad_extensions_msg("Directive")):
-                # noinspection PyTypeChecker
-                GraphQLDirective("SomeDirective", [], extensions=extensions)
-
     def describe_graphql_schema():
         def without_extensions():
             schema = GraphQLSchema()
 
             assert schema.extensions == {}
             assert schema.to_kwargs()["extensions"] == {}
 
@@ -324,13 +262,7 @@
             schema_extensions = {"schemaExtension": "schema"}
 
             schema = GraphQLSchema(extensions=schema_extensions)
 
             assert schema.extensions is schema_extensions
 
             assert schema.to_kwargs()["extensions"] is schema_extensions
-
-        @mark.parametrize("extensions", bad_extensions)
-        def with_bad_extensions(extensions):
-            with raises(TypeError, match=bad_extensions_msg("Schema")):
-                # noinspection PyTypeChecker
-                GraphQLSchema(extensions=extensions)
```

### Comparing `graphql_core-3.3.0a2/tests/type/test_introspection.py` & `graphql_core-3.3.0a3/tests/type/test_introspection.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/type/test_predicate.py` & `graphql_core-3.3.0a3/tests/type/test_predicate.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     GraphQLInputObjectType,
     GraphQLInt,
     GraphQLInterfaceType,
     GraphQLList,
     GraphQLNonNull,
     GraphQLObjectType,
     GraphQLScalarType,
+    GraphQLSchema,
     GraphQLSkipDirective,
     GraphQLString,
     GraphQLUnionType,
     assert_abstract_type,
     assert_composite_type,
     assert_directive,
     assert_enum_type,
@@ -34,14 +35,15 @@
     assert_list_type,
     assert_named_type,
     assert_non_null_type,
     assert_nullable_type,
     assert_object_type,
     assert_output_type,
     assert_scalar_type,
+    assert_schema,
     assert_type,
     assert_union_type,
     assert_wrapping_type,
     get_named_type,
     get_nullable_type,
     is_abstract_type,
     is_composite_type,
@@ -56,14 +58,15 @@
     is_non_null_type,
     is_nullable_type,
     is_object_type,
     is_output_type,
     is_required_argument,
     is_required_input_field,
     is_scalar_type,
+    is_schema,
     is_specified_directive,
     is_specified_scalar_type,
     is_type,
     is_union_type,
     is_wrapping_type,
 )
 
@@ -533,7 +536,34 @@
             def returns_true_for_specified_directives():
                 assert is_specified_directive(GraphQLIncludeDirective) is True
                 assert is_specified_directive(GraphQLSkipDirective) is True
                 assert is_specified_directive(GraphQLDeprecatedDirective) is True
 
             def returns_false_for_custom_directive():
                 assert is_specified_directive(Directive) is False
+
+
+def describe_schema_predicates():
+    schema = GraphQLSchema()
+
+    def describe_is_schema_and_assert_schema():
+        def returns_true_for_schema():
+            assert is_schema(schema) is True
+            assert assert_schema(schema) is schema
+
+        def returns_false_for_schema_class_rather_than_instance():
+            assert is_schema(GraphQLSchema) is False
+            with raises(TypeError):
+                assert_schema(GraphQLSchema)
+
+        def returns_false_for_non_schema():
+            assert is_schema(EnumType) is False
+            with raises(TypeError):
+                assert_schema(EnumType)
+            assert is_schema(ScalarType) is False
+            with raises(TypeError):
+                assert_schema(ScalarType)
+
+        def return_false_for_random_garbage():
+            assert is_schema({"what": "is this"}) is False
+            with raises(TypeError):
+                assert_schema({"what": "is this"})
```

### Comparing `graphql_core-3.3.0a2/tests/type/test_scalars.py` & `graphql_core-3.3.0a3/tests/type/test_scalars.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/type/test_schema.py` & `graphql_core-3.3.0a3/tests/type/test_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 from pytest import raises
 
 from graphql.language import (
     DirectiveLocation,
     SchemaDefinitionNode,
     SchemaExtensionNode,
-    TypeDefinitionNode,
-    TypeExtensionNode,
 )
 from graphql.type import (
     GraphQLArgument,
     GraphQLBoolean,
     GraphQLDirective,
     GraphQLField,
     GraphQLFieldMap,
@@ -172,20 +170,14 @@
         schema = GraphQLSchema(directives=directives_list)
         assert isinstance(schema.directives, tuple)
         assert schema.directives == tuple(directives_list)
         directives_tuple = schema.directives
         schema = GraphQLSchema(directives=directives_tuple)
         assert schema.directives is directives_tuple
 
-    def rejects_a_schema_with_incorrectly_typed_description():
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            GraphQLSchema(description=[])  # type: ignore
-        assert str(exc_info.value) == "Schema description must be a string."
-
     def describe_type_map():
         def includes_interface_possible_types_in_the_type_map():
             SomeInterface = GraphQLInterfaceType("SomeInterface", {})
             SomeSubtype = GraphQLObjectType(
                 "SomeSubtype", {}, interfaces=[SomeInterface]
             )
             schema = GraphQLSchema(
@@ -353,45 +345,14 @@
 
     def describe_validity():
         def describe_when_not_assumed_valid():
             def configures_the_schema_to_still_needing_validation():
                 # noinspection PyProtectedMember
                 assert GraphQLSchema(assume_valid=False).validation_errors is None
 
-            def checks_the_configuration_for_mistakes():
-                def query():
-                    pass
-
-                with raises(Exception):
-                    # noinspection PyTypeChecker
-                    GraphQLSchema(query)  # type: ignore
-                with raises(Exception):
-                    GraphQLSchema(types={})
-                with raises(Exception):
-                    GraphQLSchema(directives={})
-
-            def check_that_query_mutation_and_subscription_are_graphql_types():
-                directive = GraphQLDirective("foo", [])
-                with raises(TypeError) as exc_info:
-                    # noinspection PyTypeChecker
-                    GraphQLSchema(query=directive)  # type: ignore
-                assert str(exc_info.value) == "Expected query to be a GraphQL type."
-                with raises(TypeError) as exc_info:
-                    # noinspection PyTypeChecker
-                    GraphQLSchema(mutation=directive)  # type: ignore
-                assert str(exc_info.value) == (
-                    "Expected mutation to be a GraphQL type."
-                )
-                with raises(TypeError) as exc_info:
-                    # noinspection PyTypeChecker
-                    GraphQLSchema(subscription=directive)  # type: ignore
-                assert str(exc_info.value) == (
-                    "Expected subscription to be a GraphQL type."
-                )
-
     def describe_a_schema_must_contain_uniquely_named_types():
         def rejects_a_schema_which_redefines_a_built_in_type():
             # temporarily allow redefinition of the String scalar type
             reserved_types = GraphQLNamedType.reserved_types
             GraphQLScalarType.reserved_types = {}
             try:
                 # create a redefined String scalar type
@@ -472,36 +433,14 @@
                 GraphQLObjectType("Query", {}),
                 ast_node=ast_node,
                 extension_ast_nodes=extension_ast_nodes,
             )
             assert schema.ast_node is ast_node
             assert schema.extension_ast_nodes == tuple(extension_ast_nodes)
 
-        def rejects_a_schema_with_an_incorrect_ast_node():
-            with raises(TypeError) as exc_info:
-                # noinspection PyTypeChecker
-                GraphQLSchema(
-                    GraphQLObjectType("Query", {}),
-                    ast_node=TypeDefinitionNode(),  # type: ignore
-                )
-            msg = str(exc_info.value)
-            assert msg == "Schema AST node must be a SchemaDefinitionNode."
-
-        def rejects_a_scalar_type_with_incorrect_extension_ast_nodes():
-            with raises(TypeError) as exc_info:
-                # noinspection PyTypeChecker
-                GraphQLSchema(
-                    GraphQLObjectType("Query", {}),
-                    extension_ast_nodes=[TypeExtensionNode()],  # type: ignore
-                )
-            assert str(exc_info.value) == (
-                "Schema extension AST nodes must be specified"
-                " as a collection of SchemaExtensionNode instances."
-            )
-
     def can_deep_copy_a_schema():
         source = """
             schema {
               query: Farm
               mutation: Work
             }
```

### Comparing `graphql_core-3.3.0a2/tests/type/test_validation.py` & `graphql_core-3.3.0a3/tests/type/test_validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from operator import attrgetter
-from typing import Any, List, Union
+from typing import List, Union
 
 from pytest import mark, raises
 
 from graphql.language import DirectiveLocation, parse
 from graphql.pyutils import inspect
 from graphql.type import (
     GraphQLArgument,
     GraphQLDirective,
     GraphQLEnumType,
     GraphQLField,
     GraphQLInputField,
     GraphQLInputObjectType,
     GraphQLInputType,
-    GraphQLInt,
     GraphQLInterfaceType,
     GraphQLList,
     GraphQLNamedType,
     GraphQLNonNull,
     GraphQLObjectType,
     GraphQLOutputType,
     GraphQLSchema,
@@ -27,16 +26,14 @@
     assert_enum_type,
     assert_input_object_type,
     assert_interface_type,
     assert_object_type,
     assert_scalar_type,
     assert_union_type,
     assert_valid_schema,
-    is_input_type,
-    is_output_type,
     validate_schema,
 )
 from graphql.utilities import build_schema, extend_schema
 
 from ..utils import dedent
 
 
@@ -418,23 +415,14 @@
                 " if provided, it cannot be SomeEnum.",
                 "locations": [(3, 33)],
             },
         ]
 
     def rejects_a_schema_whose_types_are_incorrectly_type():
         # invalid schema cannot be built with Python
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            GraphQLSchema(
-                SomeObjectType,
-                types=[{"name": "SomeType"}, SomeDirective],  # type: ignore
-            )
-        assert str(exc_info.value) == (
-            "Schema types must be specified as a collection of GraphQL types."
-        )
         # construct invalid schema manually
         schema = GraphQLSchema(SomeObjectType)
         schema.type_map = {
             "SomeType": {"name": "SomeType"},  # type: ignore
             "SomeDirective": SomeDirective,  # type: ignore
         }
         assert validate_schema(schema) == [
@@ -709,40 +697,14 @@
                 "message": "Union type BadUnion can only include type TypeB once.",
                 "locations": [(16, 17), (1, 25)],
             },
         ]
 
     def rejects_a_union_type_with_non_object_member_types():
         # invalid schema cannot be built with Python
-        with raises(TypeError) as exc_info:
-            build_schema(
-                """
-                type Query {
-                  test: BadUnion
-                }
-
-                type TypeA {
-                  field: String
-                }
-
-                type TypeB {
-                  field: String
-                }
-
-                union BadUnion =
-                  | TypeA
-                  | String
-                  | TypeB
-                """
-            )
-        assert str(exc_info.value) == (
-            "BadUnion types must be specified"
-            " as a collection of GraphQLObjectType instances."
-        )
-        # construct invalid schema manually
         schema = build_schema(
             """
             type Query {
               test: BadUnion
             }
 
             type TypeA {
@@ -751,36 +713,21 @@
 
             type TypeB {
               field: String
             }
 
             union BadUnion =
               | TypeA
-              | TypeA
+              | String
               | TypeB
             """
         )
-        with raises(TypeError) as exc_info:
-            extend_schema(schema, parse("extend union BadUnion = Int"))
-        assert str(exc_info.value) == (
-            "BadUnion types must be specified"
-            " as a collection of GraphQLObjectType instances."
-        )
-        schema = extend_schema(schema, parse("extend union BadUnion = TypeB"))
-        bad_union: Any = schema.get_type("BadUnion")
-        types = bad_union.types
-        assert isinstance(types, tuple)
-        types = list(types)
-        assert types[1].name == "TypeA"
-        types[1] = GraphQLString
-        assert types[3].name == "TypeB"
-        types[3] = GraphQLInt
-        bad_union.types = tuple(types)
-        bad_union.ast_node.types[1].name.value = "String"
-        bad_union.extension_ast_nodes[0].types[0].name.value = "Int"
+
+        schema = extend_schema(schema, parse("extend union BadUnion = Int"))
+
         assert validate_schema(schema) == [
             {
                 "message": "Union type BadUnion can only include Object types,"
                 " it cannot include String.",
                 "locations": [(16, 17)],
             },
             {
@@ -800,25 +747,15 @@
             SomeInputObjectType,
         ]
         for member_type in bad_union_member_types:
             # invalid union type cannot be built with Python
             bad_union = GraphQLUnionType(
                 "BadUnion", types=[member_type]  # type: ignore
             )
-            with raises(TypeError) as exc_info:
-                schema_with_field_type(bad_union)
-            assert str(exc_info.value) == (
-                "BadUnion types must be specified"
-                " as a collection of GraphQLObjectType instances."
-            )
-            # noinspection PyPropertyAccess
-            bad_union.types = []
             bad_schema = schema_with_field_type(bad_union)
-            # noinspection PyPropertyAccess
-            bad_union.types = [member_type]
             assert validate_schema(bad_schema) == [
                 {
                     "message": "Union type BadUnion can only include Object types,"
                     + f" it cannot include {inspect(member_type)}."
                 }
             ]
 
@@ -957,62 +894,33 @@
                 " within itself through a series of non-null fields:"
                 " 'nonNullSelf'.",
                 "locations": [(17, 15)],
             },
         ]
 
     def rejects_an_input_object_type_with_incorrectly_typed_fields():
-        # invalid schema cannot be built with Python
-        with raises(TypeError) as exc_info:
-            build_schema(
-                """
-                type Query {
-                  field(arg: SomeInputObject): String
-                }
-
-                type SomeObject {
-                  field: String
-                }
-
-                union SomeUnion = SomeObject
-
-                input SomeInputObject {
-                  badObject: SomeObject
-                  badUnion: SomeUnion
-                  goodInputObject: SomeInputObject
-                }
-                """
-            )
-        assert str(exc_info.value) == (
-            "SomeInputObject fields cannot be resolved."
-            " Input field type must be a GraphQL input type."
-        )
-        # construct invalid schema manually
         schema = build_schema(
             """
             type Query {
               field(arg: SomeInputObject): String
             }
 
             type SomeObject {
               field: String
             }
 
             union SomeUnion = SomeObject
 
             input SomeInputObject {
-              badObject: SomeInputObject
-              badUnion: SomeInputObject
+              badObject: SomeObject
+              badUnion: SomeUnion
               goodInputObject: SomeInputObject
             }
             """
         )
-        some_input_obj: Any = schema.get_type("SomeInputObject")
-        some_input_obj.fields["badObject"].type = schema.get_type("SomeObject")
-        some_input_obj.fields["badUnion"].type = schema.get_type("SomeUnion")
         assert validate_schema(schema) == [
             {
                 "message": "The type of SomeInputObject.badObject must be Input Type"
                 " but got: SomeObject.",
                 "locations": [(13, 26)],
             },
             {
@@ -1086,25 +994,17 @@
                 " which is reserved by GraphQL introspection."
             }
         ]
 
 
 def describe_type_system_object_fields_must_have_output_types():
     def _schema_with_object_field(type_: GraphQLOutputType) -> GraphQLSchema:
-        if is_output_type(type_):
-            field = GraphQLField(type_)
-        else:
-            # invalid field cannot be built with Python directly
-            with raises(TypeError) as exc_info:
-                GraphQLField(type_)
-            assert str(exc_info.value) == "Field type must be an output type."
-            # therefore we need to monkey-patch a valid field
-            field = GraphQLField(GraphQLString)
-            field.type = type_
-        bad_object_type = GraphQLObjectType("BadObject", {"badField": field})
+        bad_object_type = GraphQLObjectType(
+            "BadObject", {"badField": GraphQLField(type_)}
+        )
         return GraphQLSchema(
             GraphQLObjectType("Query", {"f": GraphQLField(bad_object_type)}),
             types=[SomeObjectType],
         )
 
     @mark.parametrize("type_", output_types, ids=get_name)
     def accepts_an_output_type_as_an_object_field_type(type_):
@@ -1139,44 +1039,25 @@
                 "message": "The type of BadObject.badField must be Output Type"
                 f" but got: {inspect(type_)}.",
             },
             {"message": f"Expected GraphQL named type but got: {inspect(type_)}."},
         ]
 
     def rejects_with_relevant_locations_for_a_non_output_type():
-        # invalid schema cannot be built with Python
-        with raises(TypeError) as exc_info:
-            build_schema(
-                """
-                type Query {
-                  field: [SomeInputObject]
-                }
-
-                input SomeInputObject {
-                  field: String
-                }
-                """
-            )
-        assert str(exc_info.value) == (
-            "Query fields cannot be resolved. Field type must be an output type."
-        )
-        # therefore we need to monkey-patch a valid schema
         schema = build_schema(
             """
             type Query {
-              field: [String]
+              field: [SomeInputObject]
             }
 
             input SomeInputObject {
               field: String
             }
             """
         )
-        some_input_obj = schema.get_type("SomeInputObject")
-        schema.query_type.fields["field"].type.of_type = some_input_obj  # type: ignore
         assert validate_schema(schema) == [
             {
                 "message": "The type of Query.field must be Output Type"
                 " but got: [SomeInputObject].",
                 "locations": [(3, 22)],
             }
         ]
@@ -1196,35 +1077,35 @@
             {
                 "message": "Type BadObject must only implement Interface types,"
                 " it cannot implement None."
             }
         ]
 
     def rejects_an_object_implementing_a_non_interface_type():
-        # invalid schema cannot be built with Python
-        with raises(TypeError) as exc_info:
-            build_schema(
-                """
-                type Query {
-                  test: BadObject
-                }
+        schema = build_schema(
+            """
+            type Query {
+              test: BadObject
+            }
 
-                input SomeInputObject {
-                  field: String
-                }
+            input SomeInputObject {
+              field: String
+            }
 
-                type BadObject implements SomeInputObject {
-                  field: String
-                }
-                """
-            )
-        assert str(exc_info.value) == (
-            "BadObject interfaces must be specified"
-            " as a collection of GraphQLInterfaceType instances."
+            type BadObject implements SomeInputObject {
+              field: String
+            }
+            """
         )
+        assert validate_schema(schema) == [
+            {
+                "message": "Type BadObject must only implement Interface types,"
+                " it cannot implement SomeInputObject."
+            }
+        ]
 
     def rejects_an_object_implementing_the_same_interface_twice():
         schema = build_schema(
             """
             type Query {
               test: AnotherObject
             }
@@ -1404,26 +1285,15 @@
                 "locations": [(3, 38), (15, 38)],
             }
         ]
 
 
 def describe_type_system_interface_fields_must_have_output_types():
     def _schema_with_interface_field(type_: GraphQLOutputType) -> GraphQLSchema:
-        if is_output_type(type_):
-            field = GraphQLField(type_)
-        else:
-            # invalid field cannot be built with Python directly
-            with raises(TypeError) as exc_info:
-                GraphQLField(type_)
-            assert str(exc_info.value) == "Field type must be an output type."
-            # therefore we need to monkey-patch a valid field
-            field = GraphQLField(GraphQLString)
-            field.type = type_
-        fields = {"badField": field}
-
+        fields = {"badField": GraphQLField(type_)}
         bad_interface_type = GraphQLInterfaceType("BadInterface", fields)
         bad_implementing_type = GraphQLObjectType(
             "BadImplementing",
             fields,
             interfaces=[bad_interface_type],
         )
         return GraphQLSchema(
@@ -1476,65 +1346,33 @@
                 "message": "The type of BadInterface.badField must be Output Type"
                 f" but got: {inspect(type_)}.",
             },
             {"message": f"Expected GraphQL named type but got: {inspect(type_)}."},
         ]
 
     def rejects_a_non_output_type_as_an_interface_field_with_locations():
-        # invalid schema cannot be built with Python
-        with raises(TypeError) as exc_info:
-            build_schema(
-                """
-                type Query {
-                  test: SomeInterface
-                }
-
-                interface SomeInterface {
-                  field: SomeInputObject
-                }
-
-                input SomeInputObject {
-                  foo: String
-                }
-
-                type SomeObject implements SomeInterface {
-                  field: SomeInputObject
-                }
-                """
-            )
-        assert str(exc_info.value) == (
-            "SomeInterface fields cannot be resolved."
-            " Field type must be an output type."
-        )
-        # therefore we need to monkey-patch a valid schema
         schema = build_schema(
             """
             type Query {
               test: SomeInterface
             }
 
             interface SomeInterface {
-              field: String
+              field: SomeInputObject
             }
 
             input SomeInputObject {
               foo: String
             }
 
             type SomeObject implements SomeInterface {
-              field: String
+              field: SomeInputObject
             }
             """
         )
-        # therefore we need to monkey-patch a valid schema
-        some_input_obj = schema.get_type("SomeInputObject")
-        some_interface: Any = schema.get_type("SomeInterface")
-        some_interface.fields["field"].type = some_input_obj
-        some_object: Any = schema.get_type("SomeObject")
-        some_object.fields["field"].type = some_input_obj
         assert validate_schema(schema) == [
             {
                 "message": "The type of SomeInterface.field must be Output Type"
                 " but got: SomeInputObject.",
                 "locations": [(7, 22)],
             },
             {
@@ -1557,25 +1395,15 @@
             """
         )
         assert validate_schema(schema) == []
 
 
 def describe_type_system_arguments_must_have_input_types():
     def _schema_with_arg(type_: GraphQLInputType) -> GraphQLSchema:
-        if is_input_type(type_):
-            argument = GraphQLArgument(type_)
-        else:
-            # invalid argument cannot be built with Python directly
-            with raises(TypeError) as exc_info:
-                GraphQLArgument(type_)
-            assert str(exc_info.value) == "Argument type must be a GraphQL input type."
-            # therefore we need to monkey-patch a valid argument
-            argument = GraphQLArgument(GraphQLString)
-            argument.type = type_
-        args = {"badArg": argument}
+        args = {"badArg": GraphQLArgument(type_)}
         bad_object_type = GraphQLObjectType(
             "BadObject",
             {"badField": GraphQLField(GraphQLString, args)},
         )
         return GraphQLSchema(
             GraphQLObjectType("Query", {"f": GraphQLField(bad_object_type)}),
             directives=[
@@ -1663,70 +1491,38 @@
                 "message": "Required argument Query.test(badArg:)"
                 " cannot be deprecated.",
                 "locations": [(10, 33), (10, 25)],
             },
         ]
 
     def rejects_a_non_input_type_as_a_field_arg_with_locations():
-        # invalid schema cannot be built with Python
-        with raises(TypeError) as exc_info:
-            build_schema(
-                """
-                type Query {
-                  test(arg: SomeObject): String
-                }
-
-                type SomeObject {
-                  foo: String
-                }
-                """
-            )
-        assert str(exc_info.value) == (
-            "Query fields cannot be resolved."
-            " Argument type must be a GraphQL input type."
-        )
-        # therefore we need to monkey-patch a valid schema
         schema = build_schema(
             """
             type Query {
-              test(arg: String): String
+              test(arg: SomeObject): String
             }
 
             type SomeObject {
               foo: String
             }
             """
         )
-        some_object = schema.get_type("SomeObject")
-        schema.query_type.fields["test"].args["arg"].type = some_object  # type: ignore
         assert validate_schema(schema) == [
             {
                 "message": "The type of Query.test(arg:) must be Input Type"
                 " but got: SomeObject.",
                 "locations": [(3, 25)],
             },
         ]
 
 
 def describe_type_system_input_object_fields_must_have_input_types():
     def _schema_with_input_field(type_: GraphQLInputType) -> GraphQLSchema:
-        if is_input_type(type_):
-            input_field = GraphQLInputField(type_)
-        else:
-            # invalid input field cannot be built with Python directly
-            with raises(TypeError) as exc_info:
-                GraphQLInputField(type_)
-            assert str(exc_info.value) == (
-                "Input field type must be a GraphQL input type."
-            )
-            # therefore we need to monkey-patch a valid input field
-            input_field = GraphQLInputField(GraphQLString)
-            input_field.type = type_
         bad_input_object_type = GraphQLInputObjectType(
-            "BadInputObject", {"badField": input_field}
+            "BadInputObject", {"badField": GraphQLInputField(type_)}
         )
         return GraphQLSchema(
             GraphQLObjectType(
                 "Query",
                 {
                     "f": GraphQLField(
                         GraphQLString,
@@ -1769,54 +1565,29 @@
                 "message": "The type of BadInputObject.badField must be Input Type"
                 f" but got: {inspect(type_)}."
             },
             {"message": f"Expected GraphQL named type but got: {inspect(type_)}."},
         ]
 
     def rejects_with_relevant_locations_for_a_non_input_type():
-        # invalid schema cannot be built with Python
-        with raises(TypeError) as exc_info:
-            build_schema(
-                """
-                type Query {
-                  test(arg: SomeInputObject): String
-                }
-
-                input SomeInputObject {
-                  foo: SomeObject
-                }
-
-                type SomeObject {
-                  bar: String
-                }
-                """
-            )
-        assert str(exc_info.value) == (
-            "SomeInputObject fields cannot be resolved."
-            " Input field type must be a GraphQL input type."
-        )
-        # therefore we need to monkey-patch a valid schema
         schema = build_schema(
             """
             type Query {
               test(arg: SomeInputObject): String
             }
 
             input SomeInputObject {
-              foo: String
+              foo: SomeObject
             }
 
             type SomeObject {
               bar: String
             }
             """
         )
-        some_object = schema.get_type("SomeObject")
-        some_input_object: Any = schema.get_type("SomeInputObject")
-        some_input_object.fields["foo"].type = some_object
         assert validate_schema(schema) == [
             {
                 "message": "The type of SomeInputObject.foo must be Input Type"
                 " but got: SomeObject.",
                 "locations": [(7, 20)],
             }
         ]
@@ -2413,47 +2184,28 @@
               field: SomeObject
             }
             """
         )
         assert validate_schema(schema) == []
 
     def rejects_an_interface_implementing_a_non_interface_type():
-        # invalid schema cannot be built with Python
-        with raises(TypeError) as exc_info:
-            build_schema(
-                """
-                type Query {
-                  field: String
-                }
+        schema = build_schema(
+            """
+            type Query {
+              field: String
+            }
 
-                input SomeInputObject {
-                  field: String
-                }
+            input SomeInputObject {
+              field: String
+            }
 
-                interface BadInterface implements SomeInputObject {
-                  field: String
-                }
-                """
-            )
-        assert str(exc_info.value) == (
-            "BadInterface interfaces must be specified as a collection"
-            " of GraphQLInterfaceType instances."
-        )
-        # therefore we construct the invalid schema manually
-        some_input_obj = GraphQLInputObjectType(
-            "SomeInputObject", {"field": GraphQLInputField(GraphQLString)}
-        )
-        bad_interface = GraphQLInterfaceType(
-            "BadInterface", {"field": GraphQLField(GraphQLString)}
-        )
-        # noinspection PyTypeChecker
-        bad_interface.interfaces = (some_input_obj,)
-        schema = GraphQLSchema(
-            GraphQLObjectType("Query", {"field": GraphQLField(GraphQLString)}),
-            types=[bad_interface],
+            interface BadInterface implements SomeInputObject {
+              field: String
+            }
+            """
         )
         assert validate_schema(schema) == [
             {
                 "message": "Type BadInterface must only implement Interface types,"
                 " it cannot implement SomeInputObject.",
             }
         ]
```

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_ast_from_value.py` & `graphql_core-3.3.0a3/tests/utilities/test_ast_from_value.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_ast_to_dict.py` & `graphql_core-3.3.0a3/tests/utilities/test_ast_to_dict.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
             "selections": [
                 {
                     "kind": "field",
                     "name": "foo",
                     "alias": None,
                     "arguments": [],
                     "directives": None,
+                    "nullability_assertion": None,
                     "selection_set": res,
                 }
             ],
         }
 
     def converts_simple_schema_to_dict():
         ast = parse(
@@ -279,23 +280,25 @@
                                             "name": {"kind": "name", "value": "ep"},
                                         },
                                     }
                                 ],
                                 "directives": [],
                                 "kind": "field",
                                 "name": {"kind": "name", "value": "hero"},
+                                "nullability_assertion": None,
                                 "selection_set": {
                                     "kind": "selection_set",
                                     "selections": [
                                         {
                                             "alias": None,
                                             "arguments": [],
                                             "directives": [],
                                             "kind": "field",
                                             "name": {"kind": "name", "value": "name"},
+                                            "nullability_assertion": None,
                                             "selection_set": None,
                                         },
                                         {
                                             "directives": [],
                                             "kind": "inline_fragment",
                                             "selection_set": {
                                                 "kind": "selection_set",
@@ -305,14 +308,15 @@
                                                         "arguments": [],
                                                         "directives": [],
                                                         "kind": "field",
                                                         "name": {
                                                             "kind": "name",
                                                             "value": "primaryFunction",
                                                         },
+                                                        "nullability_assertion": None,
                                                         "selection_set": None,
                                                     }
                                                 ],
                                             },
                                             "type_condition": {
                                                 "kind": "named_type",
                                                 "name": {
@@ -332,14 +336,15 @@
                                                         "arguments": [],
                                                         "directives": [],
                                                         "kind": "field",
                                                         "name": {
                                                             "kind": "name",
                                                             "value": "height",
                                                         },
+                                                        "nullability_assertion": None,
                                                         "selection_set": None,
                                                     }
                                                 ],
                                             },
                                             "type_condition": {
                                                 "kind": "named_type",
                                                 "name": {
@@ -437,14 +442,15 @@
                                 "kind": "field",
                                 "loc": {"end": 279, "start": 65},
                                 "name": {
                                     "kind": "name",
                                     "loc": {"end": 69, "start": 65},
                                     "value": "hero",
                                 },
+                                "nullability_assertion": None,
                                 "selection_set": {
                                     "kind": "selection_set",
                                     "loc": {"end": 279, "start": 84},
                                     "selections": [
                                         {
                                             "alias": None,
                                             "arguments": [],
@@ -452,14 +458,15 @@
                                             "kind": "field",
                                             "loc": {"end": 106, "start": 102},
                                             "name": {
                                                 "kind": "name",
                                                 "loc": {"end": 106, "start": 102},
                                                 "value": "name",
                                             },
+                                            "nullability_assertion": None,
                                             "selection_set": None,
                                         },
                                         {
                                             "directives": [],
                                             "kind": "inline_fragment",
                                             "loc": {"end": 189, "start": 123},
                                             "selection_set": {
@@ -479,14 +486,15 @@
                                                             "kind": "name",
                                                             "loc": {
                                                                 "end": 171,
                                                                 "start": 156,
                                                             },
                                                             "value": "primaryFunction",
                                                         },
+                                                        "nullability_assertion": None,
                                                         "selection_set": None,
                                                     }
                                                 ],
                                             },
                                             "type_condition": {
                                                 "kind": "named_type",
                                                 "loc": {"end": 135, "start": 130},
@@ -518,14 +526,15 @@
                                                             "kind": "name",
                                                             "loc": {
                                                                 "end": 245,
                                                                 "start": 239,
                                                             },
                                                             "value": "height",
                                                         },
+                                                        "nullability_assertion": None,
                                                         "selection_set": None,
                                                     }
                                                 ],
                                             },
                                             "type_condition": {
                                                 "kind": "named_type",
                                                 "loc": {"end": 218, "start": 213},
```

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_build_ast_schema.py` & `graphql_core-3.3.0a3/tests/utilities/test_build_ast_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     introspection_types,
     validate_schema,
 )
 from graphql.utilities import build_ast_schema, build_schema, print_schema, print_type
 
 from ..fixtures import big_schema_sdl  # noqa: F401
 from ..star_wars_schema import star_wars_schema
-from ..utils import dedent, timeout_factor
+from ..utils import dedent
 
 
 try:
     from typing import TypeAlias
 except ImportError:  # Python < 3.10
     from typing_extensions import TypeAlias
 
@@ -490,28 +490,25 @@
             }
             """
         )
         assert cycle_sdl(sdl) == sdl
 
     def can_build_recursive_union():
         # invalid schema cannot be built with Python
-        with raises(TypeError) as exc_info:
-            build_schema(
-                """
-                union Hello = Hello
+        schema = build_schema(
+            """
+            union Hello = Hello
 
-                type Query {
-                  hello: Hello
-                }
-                """
-            )
-        assert (
-            str(exc_info.value) == "Hello types must be specified"
-            " as a collection of GraphQLObjectType instances."
+            type Query {
+              hello: Hello
+            }
+            """
         )
+        errors = validate_schema(schema)
+        assert errors and isinstance(errors, list)
 
     def custom_scalar():
         sdl = dedent(
             """
             scalar CustomScalar
 
             type Query {
@@ -1184,22 +1181,14 @@
               unknown: UnknownType
             }
             """
         with raises(TypeError) as exc_info:
             build_schema(sdl, assume_valid_sdl=True)
         assert str(exc_info.value).endswith("Unknown type: 'UnknownType'.")
 
-    def rejects_invalid_ast():
-        with raises(TypeError) as exc_info:
-            build_ast_schema(None)  # type: ignore
-        assert str(exc_info.value) == "Must provide valid Document AST."
-        with raises(TypeError) as exc_info:
-            build_ast_schema({})  # type: ignore
-        assert str(exc_info.value) == "Must provide valid Document AST."
-
     def describe_deepcopy_and_pickle():  # pragma: no cover
         sdl = print_schema(star_wars_schema)
 
         def can_deep_copy_schema():
             schema = build_schema(sdl, assume_valid_sdl=True)
             # create a deepcopy of the schema
             copied = deepcopy(schema)
@@ -1235,27 +1224,27 @@
             # create a deepcopy of the unpickled schema
             copied = deepcopy(loaded)
             # check that printing the copied schema gives the same SDL
             assert print_schema(copied) == sdl
 
     @mark.slow
     def describe_deepcopy_and_pickle_big():  # pragma: no cover
-        @mark.timeout(20 * timeout_factor)
+        @mark.timeout(20)
         def can_deep_copy_big_schema(big_schema_sdl):  # noqa: F811
             # use our printing conventions
             big_schema_sdl = cycle_sdl(big_schema_sdl)
 
             # create a schema from the big SDL
             schema = build_schema(big_schema_sdl, assume_valid_sdl=True)
             # create a deepcopy of the schema
             copied = deepcopy(schema)
             # check that printing the copied schema gives the same SDL
             assert print_schema(copied) == big_schema_sdl
 
-        @mark.timeout(60 * timeout_factor)
+        @mark.timeout(60)
         def can_pickle_and_unpickle_big_schema(big_schema_sdl):  # noqa: F811
             # use our printing conventions
             big_schema_sdl = cycle_sdl(big_schema_sdl)
 
             limit = sys.getrecursionlimit()
             sys.setrecursionlimit(max(limit, 4000))  # needed for pickle
 
@@ -1279,15 +1268,15 @@
                 assert len(dumped) < 25 * len(big_schema_sdl)
                 loaded = pickle.loads(dumped)
                 assert print_schema(loaded) == big_schema_sdl
 
             finally:
                 sys.setrecursionlimit(limit)
 
-        @mark.timeout(60 * timeout_factor)
+        @mark.timeout(60)
         def can_deep_copy_pickled_big_schema(big_schema_sdl):  # noqa: F811
             # use our printing conventions
             big_schema_sdl = cycle_sdl(big_schema_sdl)
 
             limit = sys.getrecursionlimit()
             sys.setrecursionlimit(max(limit, 4000))  # needed for pickle
```

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_build_client_schema.py` & `graphql_core-3.3.0a3/tests/utilities/test_build_client_schema.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_coerce_input_value.py` & `graphql_core-3.3.0a3/tests/utilities/test_coerce_input_value.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_concat_ast.py` & `graphql_core-3.3.0a3/tests/utilities/test_concat_ast.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_extend_schema.py` & `graphql_core-3.3.0a3/tests/utilities/test_extend_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,20 +310,25 @@
             """
         )
         extend_ast = parse(
             """
             extend union SomeUnion = SomeUnion
             """
         )
-        # invalid schema cannot be built with Python
-        with raises(TypeError) as exc_info:
-            extend_schema(schema, extend_ast)
-        assert str(exc_info.value) == (
-            "SomeUnion types must be specified"
-            " as a collection of GraphQLObjectType instances."
+        extended_schema = extend_schema(schema, extend_ast)
+
+        assert validate_schema(extended_schema)
+        expect_schema_changes(
+            schema,
+            extended_schema,
+            dedent(
+                """
+                union SomeUnion = SomeUnion
+                """
+            ),
         )
 
     def extends_inputs_by_adding_new_fields():
         schema = build_schema(
             '''
             type Query {
               someInput(arg: SomeInput): String
@@ -1330,27 +1335,14 @@
             }
             """
         )
         with raises(TypeError) as exc_info:
             extend_schema(schema, ast, assume_valid_sdl=True)
         assert str(exc_info.value).endswith("Unknown type: 'UnknownType'.")
 
-    def rejects_invalid_ast():
-        schema = GraphQLSchema()
-
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            extend_schema(schema, None)  # type: ignore
-        assert str(exc_info.value) == "Must provide valid Document AST."
-
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            extend_schema(schema, {})  # type: ignore
-        assert str(exc_info.value) == "Must provide valid Document AST."
-
     def does_not_allow_replacing_a_default_directive():
         schema = GraphQLSchema()
         extend_ast = parse(
             """
             directive @include(if: Boolean!) on FIELD | FRAGMENT_SPREAD
             """
         )
```

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_find_breaking_changes.py` & `graphql_core-3.3.0a3/tests/utilities/test_find_breaking_changes.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_get_introspection_query.py` & `graphql_core-3.3.0a3/tests/utilities/test_get_introspection_query.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_get_operation_ast.py` & `graphql_core-3.3.0a3/tests/utilities/test_get_operation_ast.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_introspection_from_schema.py` & `graphql_core-3.3.0a3/tests/utilities/test_introspection_from_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,23 +10,22 @@
     build_client_schema,
     build_schema,
     introspection_from_schema,
     print_schema,
 )
 
 from ..fixtures import big_schema_introspection_result, big_schema_sdl  # noqa: F401
-from ..utils import dedent, timeout_factor
+from ..utils import dedent
 
 
 def introspection_to_sdl(introspection: IntrospectionQuery) -> str:
     return print_schema(build_client_schema(introspection))
 
 
 def describe_introspection_from_schema():
-
     schema = GraphQLSchema(
         GraphQLObjectType(
             "Simple",
             {
                 "string": GraphQLField(
                     GraphQLString, description="This is a string field"
                 )
@@ -105,26 +104,26 @@
             # create a deepcopy of the unpickled schema
             copied = deepcopy(loaded)
             # check that introspecting the copied schema gives the same result
             assert introspection_from_schema(copied) == introspected_schema
 
     @mark.slow
     def describe_deepcopy_and_pickle_big():  # pragma: no cover
-        @mark.timeout(20 * timeout_factor)
+        @mark.timeout(20)
         def can_deep_copy_big_schema(big_schema_sdl):  # noqa: F811
             # introspect the original big schema
             big_schema = build_schema(big_schema_sdl)
             expected_introspection = introspection_from_schema(big_schema)
 
             # create a deepcopy of the schema
             copied = deepcopy(big_schema)
             # check that introspecting the copied schema gives the same result
             assert introspection_from_schema(copied) == expected_introspection
 
-        @mark.timeout(60 * timeout_factor)
+        @mark.timeout(60)
         def can_pickle_and_unpickle_big_schema(big_schema_sdl):  # noqa: F811
             # introspect the original big schema
             big_schema = build_schema(big_schema_sdl)
             expected_introspection = introspection_from_schema(big_schema)
             size_introspection = len(str(expected_introspection))
 
             limit = sys.getrecursionlimit()
@@ -150,15 +149,15 @@
 
                 # check that introspecting the re-pickled schema gives the same result
                 assert introspection_from_schema(loaded) == expected_introspection
 
             finally:
                 sys.setrecursionlimit(limit)
 
-        @mark.timeout(60 * timeout_factor)
+        @mark.timeout(60)
         def can_deep_copy_pickled_big_schema(big_schema_sdl):  # noqa: F811
             # introspect the original big schema
             big_schema = build_schema(big_schema_sdl)
             expected_introspection = introspection_from_schema(big_schema)
 
             limit = sys.getrecursionlimit()
             sys.setrecursionlimit(max(limit, 4000))  # needed for pickle
```

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_lexicographic_sort_schema.py` & `graphql_core-3.3.0a3/tests/utilities/test_lexicographic_sort_schema.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_print_schema.py` & `graphql_core-3.3.0a3/tests/utilities/test_print_schema.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_separate_operations.py` & `graphql_core-3.3.0a3/tests/utilities/test_separate_operations.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_sort_value_node.py` & `graphql_core-3.3.0a3/tests/utilities/test_sort_value_node.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_strip_ignored_characters.py` & `graphql_core-3.3.0a3/tests/utilities/test_strip_ignored_characters.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,16 +209,24 @@
     # noinspection PyShadowingNames
     def strips_kitchen_sink_query_but_maintains_the_exact_same_ast(
         kitchen_sink_query,  # noqa: F811
     ):
         stripped_query = strip_ignored_characters(kitchen_sink_query)
         assert strip_ignored_characters(stripped_query) == stripped_query
 
-        query_ast = parse(kitchen_sink_query, no_location=True)
-        stripped_ast = parse(stripped_query, no_location=True)
+        query_ast = parse(
+            kitchen_sink_query,
+            no_location=True,
+            experimental_client_controlled_nullability=True,
+        )
+        stripped_ast = parse(
+            stripped_query,
+            no_location=True,
+            experimental_client_controlled_nullability=True,
+        )
         assert stripped_ast == query_ast
 
     # noinspection PyShadowingNames
     def strips_kitchen_sink_sdl_but_maintains_the_exact_same_ast(
         kitchen_sink_sdl,  # noqa: F811
     ):
         stripped_sdl = strip_ignored_characters(kitchen_sink_sdl)
```

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_strip_ignored_characters_fuzz.py` & `graphql_core-3.3.0a3/tests/utilities/test_strip_ignored_characters_fuzz.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pytest import mark
 
 from graphql.error import GraphQLSyntaxError
 from graphql.language import Lexer, Source, TokenKind
 from graphql.utilities import strip_ignored_characters
 
-from ..utils import dedent, gen_fuzz_strings, timeout_factor
+from ..utils import dedent, gen_fuzz_strings
 
 
 ignored_tokens = [
     # UnicodeBOM
     "\uFEFF",  # Byte Order Mark (U+FEFF)
     # WhiteSpace
     "\t",  # Horizontal Tab (U+0009)
@@ -224,15 +224,15 @@
                 ).to_stay_the_same()
 
         ExpectStripped(
             '"""|' + "".join(ignored_tokens_without_formatting) + '|"""'
         ).to_stay_the_same()
 
     @mark.slow
-    @mark.timeout(80 * timeout_factor)
+    @mark.timeout(80)
     def strips_ignored_characters_inside_random_block_strings():
         # Testing with length >7 is taking exponentially more time. However it is
         # highly recommended to test with increased limit if you make any change.
         for fuzz_str in gen_fuzz_strings(allowed_chars='\n\t "a\\', max_length=7):
             test_str = f'"""{fuzz_str}"""'
 
             try:
```

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_type_comparators.py` & `graphql_core-3.3.0a3/tests/utilities/test_type_comparators.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_type_from_ast.py` & `graphql_core-3.3.0a3/tests/utilities/test_type_from_ast.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_type_info.py` & `graphql_core-3.3.0a3/tests/utilities/test_type_info.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_value_from_ast.py` & `graphql_core-3.3.0a3/tests/utilities/test_value_from_ast.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utilities/test_value_from_ast_untyped.py` & `graphql_core-3.3.0a3/tests/utilities/test_value_from_ast_untyped.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utils/test_dedent.py` & `graphql_core-3.3.0a3/tests/utils/test_dedent.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/utils/test_gen_fuzz_strings.py` & `graphql_core-3.3.0a3/tests/utils/test_gen_fuzz_strings.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/harness.py` & `graphql_core-3.3.0a3/tests/validation/harness.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     }
 
     union CatOrDog = Cat | Dog
 
     type Human {
       name(surname: Boolean): String
       pets: [Pet]
-      relatives: [Human]
+      relatives: [Human]!
     }
 
     enum FurColor {
       BROWN
       BLACK
       TAN
       SPOTTED
```

### Comparing `graphql_core-3.3.0a2/tests/validation/test_executable_definitions.py` & `graphql_core-3.3.0a3/tests/validation/test_executable_definitions.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_fields_on_correct_type.py` & `graphql_core-3.3.0a3/tests/validation/test_fields_on_correct_type.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_fragments_on_composite_types.py` & `graphql_core-3.3.0a3/tests/validation/test_fragments_on_composite_types.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_known_argument_names.py` & `graphql_core-3.3.0a3/tests/validation/test_known_argument_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_known_directives.py` & `graphql_core-3.3.0a3/tests/validation/test_known_directives.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_known_fragment_names.py` & `graphql_core-3.3.0a3/tests/validation/test_known_fragment_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_known_type_names.py` & `graphql_core-3.3.0a3/tests/validation/test_known_type_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_lone_anonymous_operation.py` & `graphql_core-3.3.0a3/tests/validation/test_lone_anonymous_operation.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_lone_schema_definition.py` & `graphql_core-3.3.0a3/tests/validation/test_lone_schema_definition.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_no_deprecated.py` & `graphql_core-3.3.0a3/tests/validation/test_no_deprecated.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_no_fragment_cycles.py` & `graphql_core-3.3.0a3/tests/validation/test_no_fragment_cycles.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_no_schema_introspection.py` & `graphql_core-3.3.0a3/tests/validation/test_no_schema_introspection.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_no_undefined_variables.py` & `graphql_core-3.3.0a3/tests/validation/test_no_undefined_variables.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_no_unused_fragments.py` & `graphql_core-3.3.0a3/tests/validation/test_no_unused_fragments.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_no_unused_variables.py` & `graphql_core-3.3.0a3/tests/validation/test_no_unused_variables.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_overlapping_fields_can_be_merged.py` & `graphql_core-3.3.0a3/tests/validation/test_overlapping_fields_can_be_merged.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,14 +81,124 @@
             fragment differentDirectivesWithDifferentAliases on Dog {
               name @include(if: true)
               name @include(if: false)
             }
             """
         )
 
+    def same_stream_directives_supported():
+        assert_valid(
+            """
+            fragment differentDirectivesWithDifferentAliases on Dog {
+              name @stream(label: "streamLabel", initialCount: 1)
+              name @stream(label: "streamLabel", initialCount: 1)
+            }
+            """
+        )
+
+    def different_stream_directive_label():
+        assert_errors(
+            """
+            fragment conflictingArgs on Dog {
+              name @stream(label: "streamLabel", initialCount: 1)
+              name @stream(label: "anotherLabel", initialCount: 1)
+            }
+            """,
+            [
+                {
+                    "message": "Fields 'name' conflict because they have differing"
+                    " stream directives. Use different aliases on the fields"
+                    " to fetch both if this was intentional.",
+                    "locations": [(3, 15), (4, 15)],
+                }
+            ],
+        )
+
+    def different_stream_directive_initial_count():
+        assert_errors(
+            """
+            fragment conflictingArgs on Dog {
+              name @stream(label: "streamLabel", initialCount: 1)
+              name @stream(label: "streamLabel", initialCount: 2)
+            }
+            """,
+            [
+                {
+                    "message": "Fields 'name' conflict because they have differing"
+                    " stream directives. Use different aliases on the fields"
+                    " to fetch both if this was intentional.",
+                    "locations": [(3, 15), (4, 15)],
+                }
+            ],
+        )
+
+    def different_stream_directive_first_missing_args():
+        assert_errors(
+            """
+            fragment conflictingArgs on Dog {
+              name @stream
+              name @stream(label: "streamLabel", initialCount: 1)
+            }
+            """,
+            [
+                {
+                    "message": "Fields 'name' conflict because they have differing"
+                    " stream directives. Use different aliases on the fields"
+                    " to fetch both if this was intentional.",
+                    "locations": [(3, 15), (4, 15)],
+                }
+            ],
+        )
+
+    def different_stream_directive_second_missing_args():
+        assert_errors(
+            """
+            fragment conflictingArgs on Dog {
+              name @stream(label: "streamLabel", initialCount: 1)
+              name @stream
+            }
+            """,
+            [
+                {
+                    "message": "Fields 'name' conflict because they have differing"
+                    " stream directives. Use different aliases on the fields"
+                    " to fetch both if this was intentional.",
+                    "locations": [(3, 15), (4, 15)],
+                }
+            ],
+        )
+
+    def mix_of_stream_and_no_stream():
+        assert_errors(
+            """
+            fragment conflictingArgs on Dog {
+              name @stream
+              name
+            }
+            """,
+            [
+                {
+                    "message": "Fields 'name' conflict because they have differing"
+                    " stream directives. Use different aliases on the fields"
+                    " to fetch both if this was intentional.",
+                    "locations": [(3, 15), (4, 15)],
+                }
+            ],
+        )
+
+    def same_stream_directive_both_missing_args():
+        assert_valid(
+            """
+            fragment conflictingArgs on Dog {
+              name @stream
+              name @stream
+            }
+            """
+        )
+
     def same_aliases_with_different_field_targets():
         assert_errors(
             """
             fragment sameAliasesWithDifferentFieldTargets on Dog {
               fido: name
               fido: nickname
             }
@@ -573,15 +683,14 @@
               field
               ...OtherUnknown
             }
             """
         )
 
     def describe_return_types_must_be_unambiguous():
-
         schema = build_schema(
             """
             interface SomeBox {
               deepBox: SomeBox
               unrelatedField: String
             }
```

### Comparing `graphql_core-3.3.0a2/tests/validation/test_possible_fragment_spreads.py` & `graphql_core-3.3.0a3/tests/validation/test_possible_fragment_spreads.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_possible_type_extensions.py` & `graphql_core-3.3.0a3/tests/validation/test_possible_type_extensions.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_provided_required_arguments.py` & `graphql_core-3.3.0a3/tests/validation/test_provided_required_arguments.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_scalar_leafs.py` & `graphql_core-3.3.0a3/tests/validation/test_scalar_leafs.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_single_field_subscriptions.py` & `graphql_core-3.3.0a3/tests/validation/test_single_field_subscriptions.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_unique_argument_definition_names.py` & `graphql_core-3.3.0a3/tests/validation/test_unique_argument_definition_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_unique_argument_names.py` & `graphql_core-3.3.0a3/tests/validation/test_unique_argument_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_unique_directive_names.py` & `graphql_core-3.3.0a3/tests/validation/test_unique_directive_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_unique_directives_per_location.py` & `graphql_core-3.3.0a3/tests/validation/test_unique_directives_per_location.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_unique_enum_value_names.py` & `graphql_core-3.3.0a3/tests/validation/test_unique_enum_value_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_unique_field_definition_names.py` & `graphql_core-3.3.0a3/tests/validation/test_unique_field_definition_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_unique_fragment_names.py` & `graphql_core-3.3.0a3/tests/validation/test_unique_fragment_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_unique_input_field_names.py` & `graphql_core-3.3.0a3/tests/validation/test_unique_input_field_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_unique_operation_names.py` & `graphql_core-3.3.0a3/tests/validation/test_unique_operation_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_unique_operation_types.py` & `graphql_core-3.3.0a3/tests/validation/test_unique_operation_types.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_unique_type_names.py` & `graphql_core-3.3.0a3/tests/validation/test_unique_type_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_unique_variable_names.py` & `graphql_core-3.3.0a3/tests/validation/test_unique_variable_names.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_validation.py` & `graphql_core-3.3.0a3/tests/validation/test_validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,50 +5,14 @@
 from graphql.utilities import TypeInfo, build_schema
 from graphql.validation import ValidationRule, validate
 
 from .harness import test_schema
 
 
 def describe_validate_supports_full_validation():
-    def rejects_invalid_documents():
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            assert validate(test_schema, None)  # type: ignore
-        assert str(exc_info.value) == "Must provide document."
-
-    def rejects_invalid_type_info():
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            assert validate(
-                test_schema, parse("query { name }"), type_info={}  # type: ignore
-            )
-        assert str(exc_info.value) == "Not a TypeInfo object: {}."
-
-    def rejects_invalid_rules():
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            assert validate(
-                test_schema, parse("query { name }"), rules=[None]  # type: ignore
-            )
-        assert (
-            str(exc_info.value) == "Rules must be specified as a collection"
-            " of ASTValidationRule subclasses."
-        )
-
-    def rejects_invalid_max_errors():
-        with raises(TypeError) as exc_info:
-            # noinspection PyTypeChecker
-            assert validate(
-                test_schema, parse("query { name }"), max_errors=2.5  # type: ignore
-            )
-        assert (
-            str(exc_info.value)
-            == "The maximum number of errors must be passed as an int."
-        )
-
     def validates_queries():
         doc = parse(
             """
             query {
               human {
                 pets {
                   ... on Cat {
```

### Comparing `graphql_core-3.3.0a2/tests/validation/test_values_of_correct_type.py` & `graphql_core-3.3.0a3/tests/validation/test_values_of_correct_type.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_variables_are_input_types.py` & `graphql_core-3.3.0a3/tests/validation/test_variables_are_input_types.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tests/validation/test_variables_in_allowed_position.py` & `graphql_core-3.3.0a3/tests/validation/test_variables_in_allowed_position.py`

 * *Files identical despite different names*

### Comparing `graphql_core-3.3.0a2/tox.ini` & `graphql_core-3.3.0a3/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 [tox]
 envlist = py3{7,8,9,10,11}, pypy39, black, flake8, isort, mypy, docs
 isolated_build = true
 
 [gh-actions]
 python =
-    3: py39
+    3: py311
     3.7: py37
     3.8: py38
     3.9: py39
-    3.10: py310<g
+    3.10: py310
     3.11: py311
     pypy3: pypy39
     pypy3.9: pypy39
 
 [testenv:black]
-basepython = python3.10
-deps = black==22.10.0
+basepython = python3.11
+deps = black==23.3.0
 commands  =
     black src tests -t py310 --check
 
 [testenv:flake8]
-basepython = python3.10
+basepython = python3.11
 deps =
-    flake8>=5,<6
-    flake8-bandit>=4.1,<6
-    flake8-bugbear==22.9.23
+    flake8>=6,<7
+    flake8-bandit>=4.1,<5
+    flake8-bugbear==23.5.9
 commands =
     flake8 src tests
 
 [testenv:isort]
-basepython = python3.10
-deps = isort>=5.10,<6
+basepython = python3.11
+deps = isort>=5.12,<6
 commands =
     isort src tests --check-only
 
 [testenv:mypy]
-basepython = python3.10
+basepython = python3.11
 deps =
-    mypy==0.982
-    pytest>=7.2,<8
+    mypy==1.3.0
+    pytest>=7.3,<8
 commands =
     mypy src tests
 
 [testenv:docs]
 basepython = python3.10
 deps =
-    sphinx>=5.2.1,<6
-    sphinx_rtd_theme>=1,<2
+    sphinx>=5.3,<6
+    sphinx_rtd_theme>=1.1,<2
 commands =
     sphinx-build -b html -nEW docs docs/_build/html
 
 [testenv]
 deps =
-    pytest>=7.2,<8
-    pytest-asyncio>=0.20,<1
+    pytest>=7.3,<8
+    pytest-asyncio>=0.21,<1
     pytest-benchmark>=4,<5
-    pytest-cov>=4,<5
-    pytest-describe>=2,<3
-    pytest-timeout>=2,<3
-    py37,py38,py39,pypy39: typing-extensions>=4.4,<5
+    pytest-cov>=4.1,<5
+    pytest-describe>=2.1,<3
+    pytest-timeout>=2.1,<3
+    py37,py38,py39,pypy39: typing-extensions>=4.5,<5
 commands =
     # to also run the time-consuming tests: tox -e py310 -- --run-slow
     # to run the benchmarks: tox -e py310 -- -k benchmarks --benchmark-enable
-    pytest tests {posargs: --cov-report=term-missing --cov=graphql --cov=tests --cov-fail-under=100}
+    py37,py38,py39,py311,pypy39: pytest tests {posargs}
+    py310: pytest tests {posargs: --cov-report=term-missing --cov=graphql --cov=tests --cov-fail-under=100}
```

### Comparing `graphql_core-3.3.0a2/setup.py` & `graphql_core-3.3.0a3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,285 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: graphql-core
+Version: 3.3.0a3
+Summary: GraphQL-core is a Python port of GraphQL.js,the JavaScript reference implementation for GraphQL.
+Home-page: https://github.com/graphql-python/graphql-core
+License: MIT
+Keywords: graphql
+Author: Christoph Zwerschke
+Author-email: cito@online.de
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: typing-extensions (>=4.5,<5.0) ; python_version < "3.10"
+Project-URL: Changelog, https://github.com/graphql-python/graphql-core/releases
+Project-URL: Documentation, https://graphql-core-3.readthedocs.io/
+Project-URL: Repository, https://github.com/graphql-python/graphql-core
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# GraphQL-core 3
 
-packages = \
-['docs',
- 'graphql',
- 'graphql.error',
- 'graphql.execution',
- 'graphql.language',
- 'graphql.pyutils',
- 'graphql.type',
- 'graphql.utilities',
- 'graphql.validation',
- 'graphql.validation.rules',
- 'graphql.validation.rules.custom',
- 'tests',
- 'tests.benchmarks',
- 'tests.error',
- 'tests.execution',
- 'tests.fixtures',
- 'tests.language',
- 'tests.pyutils',
- 'tests.type',
- 'tests.utilities',
- 'tests.utils',
- 'tests.validation']
-
-package_data = \
-{'': ['*'], 'docs': ['modules/*', 'usage/*']}
-
-modules = \
-['.bumpversion',
- '.editorconfig',
- '.flake8',
- '.readthedocs',
- 'poetry',
- 'tox',
- 'CODEOWNERS',
- 'SECURITY']
-extras_require = \
-{':python_version < "3.10"': ['typing-extensions>=4.4,<5.0']}
-
-setup_kwargs = {
-    'name': 'graphql-core',
-    'version': '3.3.0a2',
-    'description': 'GraphQL-core is a Python port of GraphQL.js,the JavaScript reference implementation for GraphQL.',
-    'long_description': '# GraphQL-core 3\n\nGraphQL-core 3 is a Python 3.6+ port of [GraphQL.js](https://github.com/graphql/graphql-js),\nthe JavaScript reference implementation for [GraphQL](https://graphql.org/),\na query language for APIs created by Facebook.\n\n[![PyPI version](https://badge.fury.io/py/graphql-core.svg)](https://badge.fury.io/py/graphql-core)\n[![Documentation Status](https://readthedocs.org/projects/graphql-core-3/badge/)](https://graphql-core-3.readthedocs.io)\n![Test Status](https://github.com/graphql-python/graphql-core/actions/workflows/test.yml/badge.svg)\n![Lint Status](https://github.com/graphql-python/graphql-core/actions/workflows/lint.yml/badge.svg)\n[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n\nAn extensive test suite with over 2300 unit tests and 100% coverage comprises a\nreplication of the complete test suite of GraphQL.js, making sure this port is\nreliable and compatible with GraphQL.js.\n\nThe current stable version 3.2.3 of GraphQL-core is up-to-date with GraphQL.js version 16.6.0.\n\nYou can also try out the latest alpha version 3.3.0a2 of GraphQL-core that is up-to-date with GraphQL.js version 17.0.0a1.\nPlease note that this new minor version of GraphQL-core does not support Python 3.7 anymore.\n\nNote that for various reasons, GraphQL-core does not use SemVer like GraphQL.js. Changes in the major version of GraphQL.js are reflected in the minor version of GraphQL-core instead. This means there can be breaking changes in the API when the minor version changes, and only patch releases are fully backward compatible. Therefore, we recommend something like `=~ 3.2.0` as version specifier when including GraphQL-core as a dependency.\n\n\n## Documentation\n\nA more detailed documentation for GraphQL-core 3 can be found at\n[graphql-core-3.readthedocs.io](https://graphql-core-3.readthedocs.io/).\n\nThe documentation for GraphQL.js can be found at [graphql.org/graphql-js/](https://graphql.org/graphql-js/).\n\nThe documentation for GraphQL itself can be found at [graphql.org](https://graphql.org/).\n\nThere will be also [blog articles](https://cito.github.io/tags/graphql/) with more usage\nexamples.\n\n\n## Getting started\n\nA general overview of GraphQL is available in the\n[README](https://github.com/graphql/graphql-spec/blob/main/README.md) for the\n[Specification for GraphQL](https://github.com/graphql/graphql-spec). That overview\ndescribes a simple set of GraphQL examples that exist as [tests](tests) in this\nrepository. A good way to get started with this repository is to walk through that\nREADME and the corresponding tests in parallel.\n\n\n## Installation\n\nGraphQL-core 3 can be installed from PyPI using the built-in pip command:\n\n    python -m pip install graphql-core\n\nYou can also use [poetry](https://github.com/python-poetry/poetry) for installation in a\nvirtual environment:\n\n    poetry install\n\n\n## Usage\n\nGraphQL-core provides two important capabilities: building a type schema and\nserving queries against that type schema.\n\nFirst, build a GraphQL type schema which maps to your codebase:\n\n```python\nfrom graphql import (\n    GraphQLSchema, GraphQLObjectType, GraphQLField, GraphQLString)\n\nschema = GraphQLSchema(\n    query=GraphQLObjectType(\n        name=\'RootQueryType\',\n        fields={\n            \'hello\': GraphQLField(\n                GraphQLString,\n                resolve=lambda obj, info: \'world\')\n        }))\n```\n\nThis defines a simple schema, with one type and one field, that resolves to a fixed\nvalue. The `resolve` function can return a value, a co-routine object or a list of\nthese. It takes two positional arguments; the first one provides the root or the\nresolved parent field, the second one provides a `GraphQLResolveInfo` object which\ncontains information about the execution state of the query, including a `context`\nattribute holding per-request state such as authentication information or database\nsession. Any GraphQL arguments are passed to the `resolve` functions as individual\nkeyword arguments.\n\nNote that the signature of the resolver functions is a bit different in GraphQL.js,\nwhere the context is passed separately and arguments are passed as a single object.\nAlso note that GraphQL fields must be passed as a `GraphQLField` object explicitly.\nSimilarly, GraphQL arguments must be passed as `GraphQLArgument` objects.\n\nA more complex example is included in the top-level [tests](tests) directory.\n\nThen, serve the result of a query against that type schema.\n\n```python\nfrom graphql import graphql_sync\n\nsource = \'{ hello }\'\n\nprint(graphql_sync(schema, source))\n```\n\nThis runs a query fetching the one field defined, and then prints the result:\n\n```python\nExecutionResult(data={\'hello\': \'world\'}, errors=None)\n```\n\nThe `graphql_sync` function will first ensure the query is syntactically and\nsemantically valid before executing it, reporting errors otherwise.\n\n```python\nfrom graphql import graphql_sync\n\nsource = \'{ BoyHowdy }\'\n\nprint(graphql_sync(schema, source))\n```\n\nBecause we queried a non-existing field, we will get the following result:\n\n```python\nExecutionResult(data=None, errors=[GraphQLError(\n    "Cannot query field \'BoyHowdy\' on type \'RootQueryType\'.",\n    locations=[SourceLocation(line=1, column=3)])])\n```\n\nThe `graphql_sync` function assumes that all resolvers return values synchronously. By\nusing coroutines as resolvers, you can also create results in an asynchronous fashion\nwith the `graphql` function.\n\n```python\nimport asyncio\nfrom graphql import (\n    graphql, GraphQLSchema, GraphQLObjectType, GraphQLField, GraphQLString)\n\n\nasync def resolve_hello(obj, info):\n    await asyncio.sleep(3)\n    return \'world\'\n\nschema = GraphQLSchema(\n    query=GraphQLObjectType(\n        name=\'RootQueryType\',\n        fields={\n            \'hello\': GraphQLField(\n                GraphQLString,\n                resolve=resolve_hello)\n        }))\n\n\nasync def main():\n    query = \'{ hello }\'\n    print(\'Fetching the result...\')\n    result = await graphql(schema, query)\n    print(result)\n\n\nasyncio.run(main())\n```\n\n\n## Goals and restrictions\n\nGraphQL-core tries to reproduce the code of the reference implementation GraphQL.js\nin Python as closely as possible and to stay up-to-date with the latest development of\nGraphQL.js.\n\nGraphQL-core 3 (formerly known as GraphQL-core-next) has been created as a modern\nalternative to [GraphQL-core 2](https://github.com/graphql-python/graphql-core-legacy),\na prior work by Syrus Akbary, based on an older version of GraphQL.js and also\ntargeting older Python versions. Some parts of GraphQL-core 3 have been inspired by\nGraphQL-core 2 or directly taken over with only slight modifications, but most of the\ncode has been re-implemented from scratch, replicating the latest code in GraphQL.js\nvery closely and adding type hints for Python.\n\nDesign goals for the GraphQL-core 3 library were:\n\n* to be a simple, cruft-free, state-of-the-art GraphQL implementation for current\n  Python versions\n* to be very close to the GraphQL.js reference implementation, while still providing\n  a Pythonic API and code style\n* to make extensive use of Python type hints, similar to how GraphQL.js used Flow\n  (and is now using TypeScript)\n* to use [black](https://github.com/ambv/black) to achieve a consistent code style\n  while saving time and mental energy for more important matters\n* to replicate the complete Mocha-based test suite of GraphQL.js\n  using [pytest](https://docs.pytest.org/)\n  with [pytest-describe](https://pypi.org/project/pytest-describe/)\n\nSome restrictions (mostly in line with the design goals):\n\n* requires Python 3.6 or newer\n* does not support some already deprecated methods and options of GraphQL.js\n* supports asynchronous operations only via async.io\n  (does not support the additional executors in GraphQL-core)\n\n\n## Integration with other libraries and roadmap\n\n* [Graphene](http://graphene-python.org/) is a more high-level framework for building\n  GraphQL APIs in Python, and there is already a whole ecosystem of libraries, server\n  integrations and tools built on top of Graphene. Most of this Graphene ecosystem has\n  also been created by Syrus Akbary, who meanwhile has handed over the maintenance\n  and future development to members of the GraphQL-Python community.\n\n  The current version 2 of Graphene is using Graphql-core 2 as core library for much of\n  the heavy lifting. Note that Graphene 2 is not compatible with GraphQL-core 3.\n  The  new version 3 of Graphene will use GraphQL-core 3 instead of GraphQL-core 2.\n\n* [Ariadne](https://github.com/mirumee/ariadne) is a Python library for implementing\n  GraphQL servers using schema-first approach created by Mirumee Software.\n\n  Ariadne is already using GraphQL-core 3 as its GraphQL implementation.\n\n* [Strawberry](https://github.com/strawberry-graphql/strawberry), created by Patrick\n  Arminio, is a new GraphQL library for Python 3, inspired by dataclasses,\n  that is also using GraphQL-core 3 as underpinning.\n\n\n## Changelog\n\nChanges are tracked as\n[GitHub releases](https://github.com/graphql-python/graphql-core/releases).\n\n\n## Credits and history\n\nThe GraphQL-core 3 library\n* has been created and is maintained by Christoph Zwerschke\n* uses ideas and code from GraphQL-core 2, a prior work by Syrus Akbary\n* is a Python port of GraphQL.js which has been developed by Lee Byron and others\n  at Facebook, Inc. and is now maintained\n  by the [GraphQL foundation](https://gql.foundation/join/)\n\nPlease watch the recording of Lee Byron\'s short keynote on the\n[history of GraphQL](https://www.youtube.com/watch?v=VjHWkBr3tjI)\nat the open source leadership summit 2019 to better understand\nhow and why GraphQL was created at Facebook and then became open sourced\nand ported to many different programming languages.\n\n\n## License\n\nGraphQL-core 3 is\n[MIT-licensed](./LICENSE),\njust like GraphQL.js.\n',
-    'author': 'Christoph Zwerschke',
-    'author_email': 'cito@online.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/graphql-python/graphql-core',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'py_modules': modules,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+GraphQL-core 3 is a Python 3.6+ port of [GraphQL.js](https://github.com/graphql/graphql-js),
+the JavaScript reference implementation for [GraphQL](https://graphql.org/),
+a query language for APIs created by Facebook.
 
+[![PyPI version](https://badge.fury.io/py/graphql-core.svg)](https://badge.fury.io/py/graphql-core)
+[![Documentation Status](https://readthedocs.org/projects/graphql-core-3/badge/)](https://graphql-core-3.readthedocs.io)
+![Test Status](https://github.com/graphql-python/graphql-core/actions/workflows/test.yml/badge.svg)
+![Lint Status](https://github.com/graphql-python/graphql-core/actions/workflows/lint.yml/badge.svg)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+
+An extensive test suite with over 2300 unit tests and 100% coverage comprises a
+replication of the complete test suite of GraphQL.js, making sure this port is
+reliable and compatible with GraphQL.js.
+
+The current stable version 3.2.3 of GraphQL-core is up-to-date with GraphQL.js
+version 16.6.0 and supports Python version 3.6 and newer.
+
+You can also try out the latest alpha version 3.3.0a3 of GraphQL-core
+which is up-to-date with GraphQL.js version 17.0.0a2.
+Please note that this new minor version of GraphQL-core does not support
+Python 3.6 anymore.
+
+Note that for various reasons, GraphQL-core does not use SemVer like GraphQL.js.
+Changes in the major version of GraphQL.js are reflected in the minor version of
+GraphQL-core instead. This means there can be breaking changes in the API
+when the minor version changes, and only patch releases are fully backward compatible.
+Therefore, we recommend something like `=~ 3.2.0` as version specifier
+when including GraphQL-core as a dependency.
+
+
+## Documentation
+
+A more detailed documentation for GraphQL-core 3 can be found at
+[graphql-core-3.readthedocs.io](https://graphql-core-3.readthedocs.io/).
+
+The documentation for GraphQL.js can be found at [graphql.org/graphql-js/](https://graphql.org/graphql-js/).
+
+The documentation for GraphQL itself can be found at [graphql.org](https://graphql.org/).
+
+There will be also [blog articles](https://cito.github.io/tags/graphql/) with more usage
+examples.
+
+
+## Getting started
+
+A general overview of GraphQL is available in the
+[README](https://github.com/graphql/graphql-spec/blob/main/README.md) for the
+[Specification for GraphQL](https://github.com/graphql/graphql-spec). That overview
+describes a simple set of GraphQL examples that exist as [tests](tests) in this
+repository. A good way to get started with this repository is to walk through that
+README and the corresponding tests in parallel.
+
+
+## Installation
+
+GraphQL-core 3 can be installed from PyPI using the built-in pip command:
+
+    python -m pip install graphql-core
+
+You can also use [poetry](https://github.com/python-poetry/poetry) for installation in a
+virtual environment:
+
+    poetry install
+
+
+## Usage
+
+GraphQL-core provides two important capabilities: building a type schema and
+serving queries against that type schema.
+
+First, build a GraphQL type schema which maps to your codebase:
+
+```python
+from graphql import (
+    GraphQLSchema, GraphQLObjectType, GraphQLField, GraphQLString)
+
+schema = GraphQLSchema(
+    query=GraphQLObjectType(
+        name='RootQueryType',
+        fields={
+            'hello': GraphQLField(
+                GraphQLString,
+                resolve=lambda obj, info: 'world')
+        }))
+```
+
+This defines a simple schema, with one type and one field, that resolves to a fixed
+value. The `resolve` function can return a value, a co-routine object or a list of
+these. It takes two positional arguments; the first one provides the root or the
+resolved parent field, the second one provides a `GraphQLResolveInfo` object which
+contains information about the execution state of the query, including a `context`
+attribute holding per-request state such as authentication information or database
+session. Any GraphQL arguments are passed to the `resolve` functions as individual
+keyword arguments.
+
+Note that the signature of the resolver functions is a bit different in GraphQL.js,
+where the context is passed separately and arguments are passed as a single object.
+Also note that GraphQL fields must be passed as a `GraphQLField` object explicitly.
+Similarly, GraphQL arguments must be passed as `GraphQLArgument` objects.
+
+A more complex example is included in the top-level [tests](tests) directory.
+
+Then, serve the result of a query against that type schema.
+
+```python
+from graphql import graphql_sync
+
+source = '{ hello }'
+
+print(graphql_sync(schema, source))
+```
+
+This runs a query fetching the one field defined, and then prints the result:
+
+```python
+ExecutionResult(data={'hello': 'world'}, errors=None)
+```
+
+The `graphql_sync` function will first ensure the query is syntactically and
+semantically valid before executing it, reporting errors otherwise.
+
+```python
+from graphql import graphql_sync
+
+source = '{ BoyHowdy }'
+
+print(graphql_sync(schema, source))
+```
+
+Because we queried a non-existing field, we will get the following result:
+
+```python
+ExecutionResult(data=None, errors=[GraphQLError(
+    "Cannot query field 'BoyHowdy' on type 'RootQueryType'.",
+    locations=[SourceLocation(line=1, column=3)])])
+```
+
+The `graphql_sync` function assumes that all resolvers return values synchronously.
+By  using coroutines as resolvers, you can also create results in an asynchronous
+fashion with the `graphql` function.
+
+```python
+import asyncio
+from graphql import (
+    graphql, GraphQLSchema, GraphQLObjectType, GraphQLField, GraphQLString)
+
+
+async def resolve_hello(obj, info):
+    await asyncio.sleep(3)
+    return 'world'
+
+schema = GraphQLSchema(
+    query=GraphQLObjectType(
+        name='RootQueryType',
+        fields={
+            'hello': GraphQLField(
+                GraphQLString,
+                resolve=resolve_hello)
+        }))
+
+
+async def main():
+    query = '{ hello }'
+    print('Fetching the result...')
+    result = await graphql(schema, query)
+    print(result)
+
+
+asyncio.run(main())
+```
+
+
+## Goals and restrictions
+
+GraphQL-core tries to reproduce the code of the reference implementation GraphQL.js
+in Python as closely as possible and to stay up-to-date with the latest development of
+GraphQL.js.
+
+GraphQL-core 3 (formerly known as GraphQL-core-next) has been created as a modern
+alternative to [GraphQL-core 2](https://github.com/graphql-python/graphql-core-legacy),
+a prior work by Syrus Akbary, based on an older version of GraphQL.js and also
+targeting older Python versions. Some parts of GraphQL-core 3 have been inspired by
+GraphQL-core 2 or directly taken over with only slight modifications, but most of the
+code has been re-implemented from scratch, replicating the latest code in GraphQL.js
+very closely and adding type hints for Python.
+
+Design goals for the GraphQL-core 3 library were:
+
+* to be a simple, cruft-free, state-of-the-art GraphQL implementation for current
+  Python versions
+* to be very close to the GraphQL.js reference implementation, while still providing
+  a Pythonic API and code style
+* to make extensive use of Python type hints, similar to how GraphQL.js used Flow
+  (and is now using TypeScript)
+* to use [black](https://github.com/ambv/black) to achieve a consistent code style
+  while saving time and mental energy for more important matters
+* to replicate the complete Mocha-based test suite of GraphQL.js
+  using [pytest](https://docs.pytest.org/)
+  with [pytest-describe](https://pypi.org/project/pytest-describe/)
+
+Some restrictions (mostly in line with the design goals):
+
+* requires Python 3.6 or newer
+* does not support some already deprecated methods and options of GraphQL.js
+* supports asynchronous operations only via async.io
+  (does not support the additional executors in GraphQL-core)
+
+
+## Integration with other libraries and roadmap
+
+* [Graphene](http://graphene-python.org/) is a more high-level framework for building
+  GraphQL APIs in Python, and there is already a whole ecosystem of libraries, server
+  integrations and tools built on top of Graphene. Most of this Graphene ecosystem has
+  also been created by Syrus Akbary, who meanwhile has handed over the maintenance
+  and future development to members of the GraphQL-Python community.
+
+  The current version 2 of Graphene is using Graphql-core 2 as core library for much of
+  the heavy lifting. Note that Graphene 2 is not compatible with GraphQL-core 3.
+  The  new version 3 of Graphene will use GraphQL-core 3 instead of GraphQL-core 2.
+
+* [Ariadne](https://github.com/mirumee/ariadne) is a Python library for implementing
+  GraphQL servers using schema-first approach created by Mirumee Software.
+
+  Ariadne is already using GraphQL-core 3 as its GraphQL implementation.
+
+* [Strawberry](https://github.com/strawberry-graphql/strawberry), created by Patrick
+  Arminio, is a new GraphQL library for Python 3, inspired by dataclasses,
+  that is also using GraphQL-core 3 as underpinning.
+
+
+## Changelog
+
+Changes are tracked as
+[GitHub releases](https://github.com/graphql-python/graphql-core/releases).
+
+
+## Credits and history
+
+The GraphQL-core 3 library
+* has been created and is maintained by Christoph Zwerschke
+* uses ideas and code from GraphQL-core 2, a prior work by Syrus Akbary
+* is a Python port of GraphQL.js which has been developed by Lee Byron and others
+  at Facebook, Inc. and is now maintained
+  by the [GraphQL foundation](https://gql.foundation/join/)
+
+Please watch the recording of Lee Byron's short keynote on the
+[history of GraphQL](https://www.youtube.com/watch?v=VjHWkBr3tjI)
+at the open source leadership summit 2019 to better understand
+how and why GraphQL was created at Facebook and then became open sourced
+and ported to many different programming languages.
+
+
+## License
+
+GraphQL-core 3 is
+[MIT-licensed](./LICENSE),
+just like GraphQL.js.
 
-setup(**setup_kwargs)
```

