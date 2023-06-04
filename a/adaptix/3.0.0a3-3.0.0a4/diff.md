# Comparing `tmp/adaptix-3.0.0a3.tar.gz` & `tmp/adaptix-3.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptix-3.0.0a3.tar", last modified: Sun Apr  9 16:52:08 2023, max compression
+gzip compressed data, was "adaptix-3.0.0a4.tar", last modified: Sun Jun  4 18:43:08 2023, max compression
```

## Comparing `adaptix-3.0.0a3.tar` & `adaptix-3.0.0a4.tar`

### file list

```diff
@@ -1,86 +1,91 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.111447 adaptix-3.0.0a3/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11357 2021-06-13 21:15:36.000000 adaptix-3.0.0a3/LICENSE
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4466 2023-04-09 16:52:08.111447 adaptix-3.0.0a3/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3076 2023-04-09 16:47:10.000000 adaptix-3.0.0a3/README.md
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2153 2023-04-09 16:45:47.000000 adaptix-3.0.0a3/pyproject.toml
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2023-04-09 16:52:08.111447 adaptix-3.0.0a3/setup.cfg
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.091447 adaptix-3.0.0a3/src/
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.095447 adaptix-3.0.0a3/src/adaptix/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1541 2023-04-08 09:30:44.000000 adaptix-3.0.0a3/src/adaptix/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.099447 adaptix-3.0.0a3/src/adaptix/_internal/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.099447 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      313 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2252 2023-03-11 08:07:13.000000 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/code_builder.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1517 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/compiler.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      559 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/context_namespace.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1586 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/prefix_mangler.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2206 2023-03-03 19:55:26.000000 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      573 2023-02-24 21:22:09.000000 adaptix-3.0.0a3/src/adaptix/_internal/common.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.099447 adaptix-3.0.0a3/src/adaptix/_internal/facade/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      283 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/facade/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11128 2023-04-02 19:56:21.000000 adaptix-3.0.0a3/src/adaptix/_internal/facade/provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7574 2023-04-05 08:41:54.000000 adaptix-3.0.0a3/src/adaptix/_internal/facade/retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1845 2023-04-02 21:56:31.000000 adaptix-3.0.0a3/src/adaptix/_internal/feature_requirement.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1349 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/load_error.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.099447 adaptix-3.0.0a3/src/adaptix/_internal/model_tools/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      673 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/model_tools/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7831 2023-03-12 10:02:27.000000 adaptix-3.0.0a3/src/adaptix/_internal/model_tools/definitions.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    14421 2023-04-08 14:50:16.000000 adaptix-3.0.0a3/src/adaptix/_internal/model_tools/introspection.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.103447 adaptix-3.0.0a3/src/adaptix/_internal/provider/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2201 2023-04-02 22:23:58.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10588 2023-04-04 21:35:50.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/concrete_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2355 2023-03-03 19:55:26.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/essential.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    21566 2023-04-08 10:27:34.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/generic_provider.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.107447 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1316 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7716 2023-03-12 06:49:43.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/basic_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4287 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/crown_definitions.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      883 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/definitions.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6667 2023-03-24 07:52:20.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/dumper_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5609 2023-03-24 20:20:12.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/figure_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2145 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/input_creation_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    14884 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/input_extraction_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     8056 2023-03-24 20:56:07.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/loader_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10405 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/output_creation_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     9932 2023-03-11 08:07:13.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/output_extraction_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      610 2023-03-28 18:27:05.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/request_filtering.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.107447 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      240 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2013 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/base.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    13397 2023-03-24 07:52:20.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/component.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5010 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/crown_builder.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2907 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2862 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_style.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4238 2023-03-24 20:55:51.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/overlay_schema.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3897 2023-03-21 22:13:56.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/provider_basics.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2731 2023-04-02 22:30:42.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/provider_template.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1400 2023-03-10 23:07:49.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/request_cls.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    12026 2023-04-08 10:12:42.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/request_filtering.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6191 2023-03-21 22:13:56.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/static_provider.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.111447 adaptix-3.0.0a3/src/adaptix/_internal/retort/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      319 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/retort/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3217 2023-03-21 22:13:56.000000 adaptix-3.0.0a3/src/adaptix/_internal/retort/base_retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7318 2023-04-04 19:15:15.000000 adaptix-3.0.0a3/src/adaptix/_internal/retort/mediator.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1541 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/retort/operating_retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4066 2023-03-03 19:55:26.000000 adaptix-3.0.0a3/src/adaptix/_internal/struct_path.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.111447 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      382 2023-03-11 08:07:13.000000 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2878 2023-03-11 21:00:18.000000 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/basic_utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2918 2023-03-12 10:01:39.000000 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/generic_resolver.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2206 2023-03-21 22:13:56.000000 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/implicit_params.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      557 2023-04-04 19:15:15.000000 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/norm_utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    20650 2023-04-08 16:16:31.000000 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/normalize_type.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7307 2023-04-02 21:48:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      648 2023-03-04 08:02:22.000000 adaptix-3.0.0a3/src/adaptix/load_error.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.111447 adaptix-3.0.0a3/src/adaptix/provider/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1096 2023-04-07 22:37:17.000000 adaptix-3.0.0a3/src/adaptix/provider/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      163 2023-03-03 19:55:26.000000 adaptix-3.0.0a3/src/adaptix/provider/static_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/py.typed
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      167 2023-03-03 19:55:26.000000 adaptix-3.0.0a3/src/adaptix/retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      441 2023-03-03 19:55:26.000000 adaptix-3.0.0a3/src/adaptix/struct_path.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.099447 adaptix-3.0.0a3/src/adaptix.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4466 2023-04-09 16:52:08.000000 adaptix-3.0.0a3/src/adaptix.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3092 2023-04-09 16:52:08.000000 adaptix-3.0.0a3/src/adaptix.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-04-09 16:52:08.000000 adaptix-3.0.0a3/src/adaptix.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        8 2023-04-09 16:52:08.000000 adaptix-3.0.0a3/src/adaptix.egg-info/top_level.txt
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.085407 adaptix-3.0.0a4/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    11357 2021-06-13 21:15:36.000000 adaptix-3.0.0a4/LICENSE
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4438 2023-06-04 18:43:08.085407 adaptix-3.0.0a4/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3048 2023-05-13 19:32:55.000000 adaptix-3.0.0a4/README.md
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2161 2023-06-04 18:37:34.000000 adaptix-3.0.0a4/pyproject.toml
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2023-06-04 18:43:08.085407 adaptix-3.0.0a4/setup.cfg
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.081406 adaptix-3.0.0a4/src/
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.081406 adaptix-3.0.0a4/src/adaptix/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1541 2023-05-20 17:42:58.000000 adaptix-3.0.0a4/src/adaptix/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.081406 adaptix-3.0.0a4/src/adaptix/_internal/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-02-18 14:53:08.000000 adaptix-3.0.0a4/src/adaptix/_internal/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.081406 adaptix-3.0.0a4/src/adaptix/_internal/code_tools/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-05-09 18:59:25.000000 adaptix-3.0.0a4/src/adaptix/_internal/code_tools/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2252 2023-03-11 08:07:13.000000 adaptix-3.0.0a4/src/adaptix/_internal/code_tools/code_builder.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1517 2023-02-18 14:53:08.000000 adaptix-3.0.0a4/src/adaptix/_internal/code_tools/compiler.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      559 2023-02-18 14:53:08.000000 adaptix-3.0.0a4/src/adaptix/_internal/code_tools/context_namespace.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1586 2023-02-18 14:53:08.000000 adaptix-3.0.0a4/src/adaptix/_internal/code_tools/prefix_mangler.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2351 2023-04-21 17:57:54.000000 adaptix-3.0.0a4/src/adaptix/_internal/code_tools/utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      573 2023-02-24 21:22:09.000000 adaptix-3.0.0a4/src/adaptix/_internal/common.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2512 2023-05-01 17:43:50.000000 adaptix-3.0.0a4/src/adaptix/_internal/essential.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.081406 adaptix-3.0.0a4/src/adaptix/_internal/facade/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      283 2023-02-18 14:53:08.000000 adaptix-3.0.0a4/src/adaptix/_internal/facade/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    12792 2023-05-13 21:43:47.000000 adaptix-3.0.0a4/src/adaptix/_internal/facade/provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7931 2023-05-13 13:01:37.000000 adaptix-3.0.0a4/src/adaptix/_internal/facade/retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1845 2023-04-02 21:56:31.000000 adaptix-3.0.0a4/src/adaptix/_internal/feature_requirement.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1349 2023-02-18 14:53:08.000000 adaptix-3.0.0a4/src/adaptix/_internal/load_error.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.081406 adaptix-3.0.0a4/src/adaptix/_internal/model_tools/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-05-12 16:18:06.000000 adaptix-3.0.0a4/src/adaptix/_internal/model_tools/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7883 2023-05-12 18:22:07.000000 adaptix-3.0.0a4/src/adaptix/_internal/model_tools/definitions.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    14273 2023-05-12 16:12:12.000000 adaptix-3.0.0a4/src/adaptix/_internal/model_tools/introspection.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.085407 adaptix-3.0.0a4/src/adaptix/_internal/provider/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-05-09 18:59:25.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10551 2023-05-12 15:33:46.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/concrete_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3779 2023-05-12 15:33:46.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/enum_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    19591 2023-05-09 18:59:35.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/generic_provider.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.085407 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-05-09 18:59:25.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7784 2023-05-21 19:13:30.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/basic_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4265 2023-05-20 15:02:26.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/crown_definitions.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      983 2023-05-12 16:12:06.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/definitions.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6298 2023-05-12 16:12:12.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/dumper_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1178 2023-05-12 15:34:28.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/fields.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2199 2023-05-12 16:11:18.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/input_creation_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    15215 2023-05-13 12:01:43.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/input_extraction_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7538 2023-05-12 16:12:12.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/loader_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    12027 2023-05-13 12:01:43.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/output_creation_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10410 2023-05-12 16:11:18.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/output_extraction_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      607 2023-05-12 16:12:06.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/request_filtering.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7057 2023-05-21 19:13:30.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/shape_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      788 2023-05-12 15:36:38.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/model/special_cases_optimization.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.085407 adaptix-3.0.0a4/src/adaptix/_internal/provider/name_layout/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-05-12 15:29:59.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/name_layout/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2007 2023-05-20 17:47:49.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/name_layout/base.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    13993 2023-05-20 17:48:02.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/name_layout/component.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5019 2023-05-13 11:55:16.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/name_layout/crown_builder.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3873 2023-05-20 17:47:56.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/name_layout/name_mapping.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2949 2023-05-20 17:47:42.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/name_layout/provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2920 2023-05-13 21:45:05.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/name_style.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4224 2023-05-12 15:33:46.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/overlay_schema.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3451 2023-05-12 15:33:46.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/provider_template.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3264 2023-05-12 15:33:46.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/provider_wrapper.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1420 2023-05-12 15:29:35.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/request_cls.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    14081 2023-06-04 18:33:53.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/request_filtering.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6257 2023-05-13 15:54:25.000000 adaptix-3.0.0a4/src/adaptix/_internal/provider/static_provider.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.085407 adaptix-3.0.0a4/src/adaptix/_internal/retort/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      319 2023-02-18 14:53:08.000000 adaptix-3.0.0a4/src/adaptix/_internal/retort/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3051 2023-05-12 21:48:03.000000 adaptix-3.0.0a4/src/adaptix/_internal/retort/base_retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7534 2023-05-22 21:32:37.000000 adaptix-3.0.0a4/src/adaptix/_internal/retort/mediator.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1576 2023-05-13 11:31:01.000000 adaptix-3.0.0a4/src/adaptix/_internal/retort/operating_retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4067 2023-05-21 19:06:50.000000 adaptix-3.0.0a4/src/adaptix/_internal/struct_path.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.085407 adaptix-3.0.0a4/src/adaptix/_internal/type_tools/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      419 2023-06-04 18:32:19.000000 adaptix-3.0.0a4/src/adaptix/_internal/type_tools/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3556 2023-06-04 17:30:47.000000 adaptix-3.0.0a4/src/adaptix/_internal/type_tools/basic_utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      962 2023-06-04 17:35:03.000000 adaptix-3.0.0a4/src/adaptix/_internal/type_tools/constants.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2918 2023-06-04 09:40:41.000000 adaptix-3.0.0a4/src/adaptix/_internal/type_tools/generic_resolver.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1694 2023-06-04 15:44:23.000000 adaptix-3.0.0a4/src/adaptix/_internal/type_tools/implicit_params.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      557 2023-04-04 19:15:15.000000 adaptix-3.0.0a4/src/adaptix/_internal/type_tools/norm_utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    20652 2023-05-13 15:14:52.000000 adaptix-3.0.0a4/src/adaptix/_internal/type_tools/normalize_type.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7745 2023-06-04 18:30:48.000000 adaptix-3.0.0a4/src/adaptix/_internal/utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      648 2023-03-04 08:02:22.000000 adaptix-3.0.0a4/src/adaptix/load_error.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.085407 adaptix-3.0.0a4/src/adaptix/provider/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      948 2023-05-13 16:03:34.000000 adaptix-3.0.0a4/src/adaptix/provider/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      163 2023-03-03 19:55:26.000000 adaptix-3.0.0a4/src/adaptix/provider/static_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-02-18 14:53:08.000000 adaptix-3.0.0a4/src/adaptix/py.typed
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      167 2023-03-03 19:55:26.000000 adaptix-3.0.0a4/src/adaptix/retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      441 2023-03-03 19:55:26.000000 adaptix-3.0.0a4/src/adaptix/struct_path.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-04 18:43:08.081406 adaptix-3.0.0a4/src/adaptix.egg-info/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4438 2023-06-04 18:43:08.000000 adaptix-3.0.0a4/src/adaptix.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3350 2023-06-04 18:43:08.000000 adaptix-3.0.0a4/src/adaptix.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-06-04 18:43:08.000000 adaptix-3.0.0a4/src/adaptix.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        8 2023-06-04 18:43:08.000000 adaptix-3.0.0a4/src/adaptix.egg-info/top_level.txt
```

### Comparing `adaptix-3.0.0a3/LICENSE` & `adaptix-3.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a3/PKG-INFO` & `adaptix-3.0.0a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptix
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: An utility class for creating instances of dataclasses
 Author-email: "A. Tikhonov" <17@itishka.org>
 Project-URL: Homepage, https://github.com/reagento/dataclass_factory
 Project-URL: Bug Tracker, https://github.com/reagento/dataclass_factory/issues
 Project-URL: Documentation, https://adaptix.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/reagento/dataclass_factory/
 Project-URL: Download, https://github.com/reagento/dataclass_factory/#files
@@ -25,15 +25,15 @@
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Adaptix
 
-[![PyPI version](https://badge.fury.io/py/adaptix.svg)](https://badge.fury.io/py/dataclass-factory)
+[![PyPI version](https://img.shields.io/pypi/v/adaptix.svg)](https://badge.fury.io/py/dataclass-factory)
 [![downloads](https://img.shields.io/pypi/dm/adaptix.svg)](https://pypistats.org/packages/adaptix)
 [![versions](https://img.shields.io/pypi/pyversions/adaptix.svg)](https://github.com/reagento/dataclass_factory)
 [![license](https://img.shields.io/github/license/reagento/dataclass_factory.svg)](https://github.com/reagento/dataclass_factory/blob/master/LICENSE)
 
 An extremely flexible and configurable data model conversion library.
 
 📑 [Documentation](https://adaptix.readthedocs.io/)
@@ -67,18 +67,14 @@
 retort = Retort()
 
 book = retort.load(data, Book)
 assert book == Book(title="Fahrenheit 451", price=100)
 assert retort.dump(book) == data
 ```
 
-## Requirements
-
-* Python 3.8
-
 ## Use cases
 
 * Validation and transformation of received data for your API.
 * Config loading/dumping via codec that produces/takes dict.
 * Storing JSON in a database and representing it as a model inside the application code.
 * Creating API clients that convert a model to JSON sending to the server.
 * Persisting entities at cache storage.
@@ -91,15 +87,15 @@
   that allow preserving [SRP](https://blog.cleancoder.com/uncle-bob/2014/05/08/SingleReponsibilityPrinciple.html)
   and have different representations for one model.
 * Speed. It is one of the fastest data parsing and serialization libraries.
 * There is no forced model representation, adaptix can adjust to your needs.
 * Support [dozens](https://adaptix.readthedocs.io/en/latest/specific_types_behavior.html) of types,
   including different model kinds:
   ``@dataclass``, ``TypedDict``, ``NamedTuple``, and [``attrs``](https://www.attrs.org/en/stable/)
-* Working with cyclic-referenced structures (such as linked lists or trees).
+* Working with self-referenced data types (such as linked lists or trees).
 * Saving [path](https://adaptix.readthedocs.io/en/latest/tutorial.html#struct-path)
   where an exception is raised (including unexpected errors).
 * Easy [integration](https://adaptix.readthedocs.io/en/latest/tutorial.html#struct-path)
   with Sentry, Datadog, and other monitoring systems.
 * Machine-readable [errors](https://adaptix.readthedocs.io/en/latest/tutorial.html#error-handling)
   that could be dumped.
 * Support for user-defined generic models.
```

### Comparing `adaptix-3.0.0a3/README.md` & `adaptix-3.0.0a4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Adaptix
 
-[![PyPI version](https://badge.fury.io/py/adaptix.svg)](https://badge.fury.io/py/dataclass-factory)
+[![PyPI version](https://img.shields.io/pypi/v/adaptix.svg)](https://badge.fury.io/py/dataclass-factory)
 [![downloads](https://img.shields.io/pypi/dm/adaptix.svg)](https://pypistats.org/packages/adaptix)
 [![versions](https://img.shields.io/pypi/pyversions/adaptix.svg)](https://github.com/reagento/dataclass_factory)
 [![license](https://img.shields.io/github/license/reagento/dataclass_factory.svg)](https://github.com/reagento/dataclass_factory/blob/master/LICENSE)
 
 An extremely flexible and configurable data model conversion library.
 
 📑 [Documentation](https://adaptix.readthedocs.io/)
@@ -38,18 +38,14 @@
 retort = Retort()
 
 book = retort.load(data, Book)
 assert book == Book(title="Fahrenheit 451", price=100)
 assert retort.dump(book) == data
 ```
 
-## Requirements
-
-* Python 3.8
-
 ## Use cases
 
 * Validation and transformation of received data for your API.
 * Config loading/dumping via codec that produces/takes dict.
 * Storing JSON in a database and representing it as a model inside the application code.
 * Creating API clients that convert a model to JSON sending to the server.
 * Persisting entities at cache storage.
@@ -62,15 +58,15 @@
   that allow preserving [SRP](https://blog.cleancoder.com/uncle-bob/2014/05/08/SingleReponsibilityPrinciple.html)
   and have different representations for one model.
 * Speed. It is one of the fastest data parsing and serialization libraries.
 * There is no forced model representation, adaptix can adjust to your needs.
 * Support [dozens](https://adaptix.readthedocs.io/en/latest/specific_types_behavior.html) of types,
   including different model kinds:
   ``@dataclass``, ``TypedDict``, ``NamedTuple``, and [``attrs``](https://www.attrs.org/en/stable/)
-* Working with cyclic-referenced structures (such as linked lists or trees).
+* Working with self-referenced data types (such as linked lists or trees).
 * Saving [path](https://adaptix.readthedocs.io/en/latest/tutorial.html#struct-path)
   where an exception is raised (including unexpected errors).
 * Easy [integration](https://adaptix.readthedocs.io/en/latest/tutorial.html#struct-path)
   with Sentry, Datadog, and other monitoring systems.
 * Machine-readable [errors](https://adaptix.readthedocs.io/en/latest/tutorial.html#error-handling)
   that could be dumped.
 * Support for user-defined generic models.
```

### Comparing `adaptix-3.0.0a3/pyproject.toml` & `adaptix-3.0.0a4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools==65.1.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'adaptix'
-version = '3.0.0a3'
+version = '3.0.0a4'
 description = 'An utility class for creating instances of dataclasses'
 readme = 'README.md'
 requires-python = '>=3.8'
 
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python :: 3',
@@ -55,15 +55,15 @@
 [tool.pytest.ini_options]
 python_classes = 'WeDoNotUseClassTestCase'
 python_files = ['test_*.py', '*_test.py', 'bench_*.py', 'tests_helpers.py']
 testpaths = ['tests', 'tests_helpers', 'examples']
 filterwarnings = ['ignore::adaptix.TypedDictAt38Warning']
 
 [tool.bandit]
-skips = ['B102', 'B404', 'B603', 'B607']
+skips = ['B102', 'B106', 'B404', 'B603', 'B607']
 
 [tool.bandit.assert_used]
 skips = ['*/test_*.py', '*/*_test.py', 'docs/examples/*', '*/bench_*.py']
 
 [tool.vulture]
 min_confidence = 60
 ignore_decorators = ['@_aspect_storage.add', '@overload', '@abstractmethod']
```

### Comparing `adaptix-3.0.0a3/src/adaptix/__init__.py` & `adaptix-3.0.0a4/src/adaptix/__init__.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/code_tools/code_builder.py` & `adaptix-3.0.0a4/src/adaptix/_internal/code_tools/code_builder.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/code_tools/compiler.py` & `adaptix-3.0.0a4/src/adaptix/_internal/code_tools/compiler.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/code_tools/context_namespace.py` & `adaptix-3.0.0a4/src/adaptix/_internal/code_tools/context_namespace.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/code_tools/prefix_mangler.py` & `adaptix-3.0.0a4/src/adaptix/_internal/code_tools/prefix_mangler.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/code_tools/utils.py` & `adaptix-3.0.0a4/src/adaptix/_internal/code_tools/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -82,7 +82,14 @@
 
 
 def get_literal_from_factory(obj: object) -> Optional[str]:
     try:
         return _CLS_TO_FACTORY_LITERAL.get(obj, None)
     except TypeError:
         return None
+
+
+_SINGLETONS = {None, Ellipsis, NotImplemented}
+
+
+def is_singleton(obj: object) -> bool:
+    return obj in _SINGLETONS or isinstance(obj, bool)
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/common.py` & `adaptix-3.0.0a4/src/adaptix/_internal/common.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/facade/provider.py` & `adaptix-3.0.0a4/src/adaptix/_internal/facade/provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 from __future__ import annotations
 
-import re
 from enum import Enum, EnumMeta
 from types import MappingProxyType
-from typing import Any, Callable, Iterable, List, Mapping, Optional, Sequence, Tuple, TypeVar, Union
+from typing import Any, Callable, Iterable, List, Mapping, Optional, Sequence, TypeVar, Union
 
 from ..common import Catchable, Dumper, Loader, TypeHint, VarTuple
-from ..model_tools import Default, DescriptorAccessor, NoDefault, OutputField, get_callable_figure
-from ..provider import (
-    BoundingProvider,
-    Chain,
-    ChainingProvider,
-    DumperRequest,
-    EnumExactValueProvider,
-    EnumNameProvider,
-    EnumValueProvider,
-    LoaderRequest,
-    LoadError,
-    ModelLoaderProvider,
-    NameSanitizer,
-    NameStyle,
-    OrRequestChecker,
-    PropertyAdder,
-    Provider,
-    ValidationError,
-    ValueProvider,
-    create_request_checker,
-)
-from ..provider.model.loader_provider import InlinedInputExtractionMaker, make_input_creation
+from ..essential import Provider
+from ..load_error import LoadError, ValidationError
+from ..model_tools.definitions import Default, DescriptorAccessor, NoDefault, OutputField
+from ..model_tools.introspection import get_callable_shape
+from ..provider.enum_provider import EnumExactValueProvider, EnumNameProvider, EnumValueProvider
+from ..provider.model.basic_gen import NameSanitizer
+from ..provider.model.loader_provider import InlinedInputExtractionMaker, ModelLoaderProvider, make_input_creation
+from ..provider.model.shape_provider import PropertyAdder
+from ..provider.model.special_cases_optimization import as_is_stub
 from ..provider.name_layout.base import ExtraIn, ExtraOut
-from ..provider.name_layout.component import (
-    ExtraMoveAndPoliciesOverlay,
-    NameMapStack,
-    RawKey,
-    RawPath,
-    SievesOverlay,
-    StructureOverlay,
+from ..provider.name_layout.component import ExtraMoveAndPoliciesOverlay, SievesOverlay, StructureOverlay
+from ..provider.name_layout.name_mapping import (
+    AsListNameMappingProvider,
+    ConstNameMappingProvider,
+    DictNameMappingProvider,
+    FuncNameMappingProvider,
+    NameMap,
 )
+from ..provider.name_style import NameStyle
 from ..provider.overlay_schema import OverlayProvider
-from ..provider.request_filtering import Pred, RequestPattern
+from ..provider.provider_template import ValueProvider
+from ..provider.provider_wrapper import BoundingProvider, Chain, ChainingProvider
+from ..provider.request_cls import DumperRequest, LoaderRequest
+from ..provider.request_filtering import (
+    AnyRequestChecker,
+    OrRequestChecker,
+    Pred,
+    RequestChecker,
+    RequestPattern,
+    create_request_checker,
+)
 from ..utils import Omittable, Omitted
 
 T = TypeVar('T')
 
 
 def bound(pred: Pred, provider: Provider) -> Provider:
     if pred == Omitted():
@@ -111,111 +108,145 @@
 
 def as_is_loader(pred: Pred) -> Provider:
     """Provider that creates loader which does nothing with input data.
 
     :param pred: Predicate specifying where loader should be used. See :ref:`predicate-system` for details.
     :return: desired provider
     """
-    return loader(pred, lambda x: x)
+    return loader(pred, as_is_stub)
 
 
 def as_is_dumper(pred: Pred) -> Provider:
     """Provider that creates dumper which does nothing with input data.
 
     :param pred: Predicate specifying where dumper should be used. See :ref:`predicate-system` for details.
     :return: desired provider
     """
-    return dumper(pred, lambda x: x)
+    return dumper(pred, as_is_stub)
 
 
 def constructor(pred: Pred, func: Callable) -> Provider:
-    input_figure = get_callable_figure(func).input
+    input_shape = get_callable_shape(func).input
     return bound(
         pred,
         ModelLoaderProvider(
             NameSanitizer(),
-            InlinedInputExtractionMaker(input_figure),
+            InlinedInputExtractionMaker(input_shape),
             make_input_creation,
         ),
     )
 
 
-NameMap = Mapping[Union[str, re.Pattern], Union[RawKey, Iterable[RawKey]]]
+def _add_as_list(providers: VarTuple[Provider], as_list: bool) -> VarTuple[Provider]:
+    if as_list:
+        return providers + (AsListNameMappingProvider(), )
+    return providers
 
 
-def _convert_name_map_to_stack(name_map: NameMap) -> NameMapStack:
-    result: List[Tuple[re.Pattern, RawPath]] = []
-    for pattern, path in name_map.items():
-        path_tuple: VarTuple[RawKey]
-        if isinstance(path, (str, int)) or path is Ellipsis:
-            path_tuple = (path, )
-        else:
-            path_tuple = tuple(path)
-            if not path_tuple:
-                raise ValueError(f"Path for field {pattern!r} can not be empty iterable")
-
-        result.append(
-            (
-                pattern if isinstance(pattern, re.Pattern) else re.compile(pattern),
-                path_tuple
-            )
+def _name_mapping_convert_map(name_map: Omittable[NameMap]) -> VarTuple[Provider]:
+    if isinstance(name_map, Omitted):
+        return ()
+    if isinstance(name_map, Mapping):
+        return (
+            DictNameMappingProvider(name_map),
         )
-
+    result: List[Provider] = []
+    for element in name_map:
+        if isinstance(element, Mapping):
+            result.append(
+                DictNameMappingProvider(element)
+            )
+        elif isinstance(element, tuple):
+            pred, value = element
+            result.append(
+                FuncNameMappingProvider(create_request_checker(pred), value)
+                if callable(value) else
+                ConstNameMappingProvider(create_request_checker(pred), value)
+            )
+        else:
+            result.append(element)
     return tuple(result)
 
 
+def _name_mapping_convert_preds(value: Omittable[Union[Iterable[Pred], Pred]]) -> Omittable[RequestChecker]:
+    if isinstance(value, Omitted):
+        return value
+    if isinstance(value, Iterable) and not isinstance(value, str):
+        return OrRequestChecker([create_request_checker(el) for el in value])
+    return create_request_checker(value)
+
+
+def _name_mapping_convert_omit_default(
+    value: Omittable[Union[Iterable[Pred], Pred, bool]]
+) -> Omittable[RequestChecker]:
+    if isinstance(value, bool):
+        return AnyRequestChecker() if value else ~AnyRequestChecker()
+    return _name_mapping_convert_preds(value)
+
+
 def name_mapping(
     pred: Omittable[Pred] = Omitted(),
     *,
     # filtering which fields are presented
-    skip: Omittable[Iterable[str]] = Omitted(),
-    only: Omittable[Optional[Iterable[str]]] = Omitted(),
-    only_mapped: Omittable[bool] = Omitted(),
+    skip: Omittable[Union[Iterable[Pred], Pred]] = Omitted(),
+    only: Omittable[Union[Iterable[Pred], Pred]] = Omitted(),
     # mutating names of presented fields
     map: Omittable[NameMap] = Omitted(),  # noqa: A002
+    as_list: bool = False,
     trim_trailing_underscore: Omittable[bool] = Omitted(),
     name_style: Omittable[Optional[NameStyle]] = Omitted(),
     # filtering of dumped data
-    omit_default: Omittable[bool] = Omitted(),
+    omit_default: Omittable[Union[Iterable[Pred], Pred, bool]] = Omitted(),
     # policy for data that does not map to fields
     extra_in: Omittable[ExtraIn] = Omitted(),
     extra_out: Omittable[ExtraOut] = Omitted(),
     # chaining with next matching provider
     chain: Optional[Chain] = Chain.FIRST,
 ) -> Provider:
     """A name mapping decides which fields will be presented
     to the outside world and how they will look.
 
     The mapping process consists of two stages:
     1. Determining which fields are presented
     2. Mutating names of presented fields
 
-    `skip` parameter has higher priority than `only` and `only_mapped`.
+    `skip` parameter has higher priority than `only`.
 
     Mutating parameters works in that way:
     Mapper tries to use the value from the map.
     If the field is not presented in the map,
     trim trailing underscore and convert name style.
 
     The field must follow snake_case to could be converted.
+
+    :param only:
+    :param pred:
+    :param skip:
+    :param map:
+    :param as_list:
+    :param trim_trailing_underscore:
+    :param name_style:
+    :param omit_default:
+    :param extra_in:
+    :param extra_out:
+    :param chain:
     """
     return bound(
         pred,
         OverlayProvider(
             overlays=[
                 StructureOverlay(
-                    skip=skip,
-                    only=only,
-                    only_mapped=only_mapped,
-                    map=Omitted() if isinstance(map, Omitted) else _convert_name_map_to_stack(map),
+                    skip=_name_mapping_convert_preds(skip),
+                    only=_name_mapping_convert_preds(only),
+                    map=_add_as_list(_name_mapping_convert_map(map), as_list),
                     trim_trailing_underscore=trim_trailing_underscore,
                     name_style=name_style,
                 ),
                 SievesOverlay(
-                    omit_default=omit_default,
+                    omit_default=_name_mapping_convert_omit_default(omit_default),
                 ),
                 ExtraMoveAndPoliciesOverlay(
                     extra_in=extra_in,
                     extra_out=extra_out,
                 ),
             ],
             chain=chain,
@@ -234,26 +265,26 @@
     default: Default = NoDefault(),
     access_error: Optional[Catchable] = None,
     metadata: Mapping[Any, Any] = MappingProxyType({}),
 ) -> Provider:
     attr_name = _ensure_attr_name(prop)
 
     field = OutputField(
-        name=attr_name,
+        id=attr_name,
         type=tp,
         accessor=DescriptorAccessor(attr_name, access_error),
         default=default,
         metadata=metadata,
     )
 
     return bound(
         pred,
         PropertyAdder(
             output_fields=[field],
-            infer_types_for=[field.name] if tp == Omitted() else [],
+            infer_types_for=[field.id] if tp == Omitted() else [],
         )
     )
 
 
 def _ensure_attr_name(prop: NameOrProp) -> str:
     if isinstance(prop, str):
         return prop
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/facade/retort.py` & `adaptix-3.0.0a4/src/adaptix/_internal/facade/retort.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,63 +5,62 @@
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 from itertools import chain
 from pathlib import Path, PosixPath, PurePath, PurePosixPath, PureWindowsPath, WindowsPath
 from typing import Any, ByteString, Iterable, Mapping, MutableMapping, Optional, Type, TypeVar, overload
 from uuid import UUID
 
 from ..common import Dumper, Loader, TypeHint, VarTuple
-from ..provider import (
-    ATTRS_FIGURE_PROVIDER,
-    CLASS_INIT_FIGURE_PROVIDER,
-    DATACLASS_FIGURE_PROVIDER,
-    NAMED_TUPLE_FIGURE_PROVIDER,
-    TYPED_DICT_FIGURE_PROVIDER,
-    ABCProxy,
-    BuiltinInputExtractionMaker,
-    BuiltinOutputCreationMaker,
+from ..essential import Provider, Request
+from ..provider.concrete_provider import (
+    BOOL_LOADER_PROVIDER,
+    COMPLEX_LOADER_PROVIDER,
+    DECIMAL_LOADER_PROVIDER,
+    FLOAT_LOADER_PROVIDER,
+    FRACTION_LOADER_PROVIDER,
+    INT_LOADER_PROVIDER,
+    STR_LOADER_PROVIDER,
     BytearrayBase64Provider,
     BytesBase64Provider,
-    DictProvider,
-    DumperRequest,
-    EnumExactValueProvider,
     IsoFormatProvider,
-    IterableProvider,
-    LiteralProvider,
-    LoaderRequest,
-    ModelDumperProvider,
-    ModelLoaderProvider,
-    NameSanitizer,
-    NewTypeUnwrappingProvider,
     NoneProvider,
-    Provider,
     RegexPatternProvider,
-    Request,
     SecondsTimedeltaProvider,
-    TypeHintLoc,
+)
+from ..provider.enum_provider import EnumExactValueProvider
+from ..provider.generic_provider import (
+    DictProvider,
+    IterableProvider,
+    LiteralProvider,
+    NewTypeUnwrappingProvider,
     TypeHintTagsUnwrappingProvider,
     UnionProvider,
-    ValueProvider,
 )
-from ..provider.concrete_provider import (
-    BOOL_LOADER_PROVIDER,
-    COMPLEX_LOADER_PROVIDER,
-    DECIMAL_LOADER_PROVIDER,
-    FLOAT_LOADER_PROVIDER,
-    FRACTION_LOADER_PROVIDER,
-    INT_LOADER_PROVIDER,
-    STR_LOADER_PROVIDER,
+from ..provider.model.basic_gen import NameSanitizer
+from ..provider.model.crown_definitions import ExtraSkip
+from ..provider.model.dumper_provider import BuiltinOutputCreationMaker, ModelDumperProvider, make_output_extraction
+from ..provider.model.loader_provider import BuiltinInputExtractionMaker, ModelLoaderProvider, make_input_creation
+from ..provider.model.shape_provider import (
+    ATTRS_SHAPE_PROVIDER,
+    CLASS_INIT_SHAPE_PROVIDER,
+    DATACLASS_SHAPE_PROVIDER,
+    NAMED_TUPLE_SHAPE_PROVIDER,
+    TYPED_DICT_SHAPE_PROVIDER,
 )
-from ..provider.model import ExtraSkip, make_input_creation, make_output_extraction
-from ..provider.name_layout import (
-    BuiltinExtraMoveAndPoliciesMaker,
-    BuiltinNameLayoutProvider,
-    BuiltinSievesMaker,
-    BuiltinStructureMaker,
+from ..provider.name_layout.component import BuiltinExtraMoveAndPoliciesMaker, BuiltinSievesMaker, BuiltinStructureMaker
+from ..provider.name_layout.provider import BuiltinNameLayoutProvider
+from ..provider.provider_template import ABCProxy, ValueProvider
+from ..provider.request_cls import (
+    DebugPathRequest,
+    DumperRequest,
+    LoaderRequest,
+    LocMap,
+    StrictCoercionRequest,
+    TypeHintLoc,
 )
-from ..provider.request_cls import DebugPathRequest, LocMap, StrictCoercionRequest
+from ..provider.request_filtering import AnyRequestChecker
 from ..retort import OperatingRetort
 from .provider import as_is_dumper, as_is_loader, dumper, loader, name_mapping
 
 
 class FilledRetort(OperatingRetort, ABC):
     """A retort contains builtin providers"""
 
@@ -72,15 +71,15 @@
         as_is_dumper(Any),
 
         IsoFormatProvider(datetime),
         IsoFormatProvider(date),
         IsoFormatProvider(time),
         SecondsTimedeltaProvider(),
 
-        EnumExactValueProvider(),  # it has higher priority than int for IntEnum
+        EnumExactValueProvider(),  # it has higher priority than scalar types for Enum with mixins
 
         INT_LOADER_PROVIDER,
         as_is_dumper(int),
 
         FLOAT_LOADER_PROVIDER,
         as_is_dumper(float),
 
@@ -127,37 +126,36 @@
         ABCProxy(Mapping, dict),
         ABCProxy(MutableMapping, dict),
         ABCProxy(ByteString, bytes),
 
         name_mapping(
             chain=None,
             skip=(),
-            only_mapped=False,
-            only=None,
+            only=AnyRequestChecker(),
             map={},
             trim_trailing_underscore=True,
             name_style=None,
-            omit_default=True,
+            omit_default=False,
             extra_in=ExtraSkip(),
             extra_out=ExtraSkip(),
         ),
         BuiltinNameLayoutProvider(
             structure_maker=BuiltinStructureMaker(),
             sieves_maker=BuiltinSievesMaker(),
             extra_move_maker=BuiltinExtraMoveAndPoliciesMaker(),
             extra_policies_maker=BuiltinExtraMoveAndPoliciesMaker(),
         ),
         ModelLoaderProvider(NameSanitizer(), BuiltinInputExtractionMaker(), make_input_creation),
         ModelDumperProvider(NameSanitizer(), make_output_extraction, BuiltinOutputCreationMaker()),
 
-        NAMED_TUPLE_FIGURE_PROVIDER,
-        TYPED_DICT_FIGURE_PROVIDER,
-        DATACLASS_FIGURE_PROVIDER,
-        CLASS_INIT_FIGURE_PROVIDER,
-        ATTRS_FIGURE_PROVIDER,
+        NAMED_TUPLE_SHAPE_PROVIDER,
+        TYPED_DICT_SHAPE_PROVIDER,
+        DATACLASS_SHAPE_PROVIDER,
+        CLASS_INIT_SHAPE_PROVIDER,
+        ATTRS_SHAPE_PROVIDER,
 
         NewTypeUnwrappingProvider(),
         TypeHintTagsUnwrappingProvider(),
     ]
 
 
 T = TypeVar('T')
@@ -167,15 +165,15 @@
 
 class AdornedRetort(OperatingRetort):
     """A retort implementing high-level user interface"""
 
     def __init__(
         self,
         *,
-        recipe: Optional[Iterable[Provider]] = None,
+        recipe: Iterable[Provider] = (),
         strict_coercion: bool = True,
         debug_path: bool = True,
     ):
         self._strict_coercion = strict_coercion
         self._debug_path = debug_path
         super().__init__(recipe)
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/feature_requirement.py` & `adaptix-3.0.0a4/src/adaptix/_internal/feature_requirement.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/load_error.py` & `adaptix-3.0.0a4/src/adaptix/_internal/load_error.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/model_tools/definitions.py` & `adaptix-3.0.0a4/src/adaptix/_internal/model_tools/definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         super().__init__(attr_name, access_error)
 
     @property
     def is_required(self) -> bool:
         return self.access_error is None
 
     def __repr__(self):
-        return f"{type(self)}(attr_name={self.attr_name}, is_required={self.is_required})"
+        return f"{type(self).__name__}(attr_name={self.attr_name}, is_required={self.is_required})"
 
 
 @dataclass(frozen=True)
 class ItemAccessor(Accessor):
     item_name: str
     is_required: bool
 
@@ -114,27 +114,31 @@
     def path_element(self) -> PathElement:
         return self.item_name
 
     def __hash__(self):
         return hash((self.item_name, self.is_required))
 
 
+def is_valid_field_id(value: str) -> bool:
+    return value.isidentifier()
+
+
 @dataclass(frozen=True)
 class BaseField:
     type: TypeHint
-    name: str
+    id: str
     default: Default
     # Mapping almost never defines __hash__,
     # so it will be more convenient to exclude this field
     # from hash computation
     metadata: Mapping[Any, Any] = field(hash=False)
 
     def __post_init__(self):
-        if not self.name.isidentifier():
-            raise ValueError(f"name of field must be python identifier, now it is a {self.name!r}")
+        if not is_valid_field_id(self.id):
+            raise ValueError(f"name of field must be python identifier, now it is a {self.id!r}")
 
 
 class ParamKind(Enum):
     POS_ONLY = 0
     POS_OR_KW = 1
     KW_ONLY = 3  # 2 is for VAR_POS
 
@@ -168,47 +172,47 @@
 
     @property
     def is_required(self) -> bool:
         return self.accessor.access_error is None
 
 
 @dataclass(frozen=True)
-class BaseFigure:
+class BaseShape:
     """Signature of class. Divided into 2 parts: input and output.
-    See doc :class InputFigure: and :class OutputFigure: for more details
+    See doc :class InputShape: and :class OutputShape: for more details
     """
     fields: VarTuple[BaseField]
     overriden_types: FrozenSet[str]
     fields_dict: Mapping[str, BaseField] = field(init=False, hash=False, repr=False, compare=False)
 
     def _validate(self):
-        field_names = {fld.name for fld in self.fields}
-        if len(field_names) != len(self.fields):
+        field_ids = {fld.id for fld in self.fields}
+        if len(field_ids) != len(self.fields):
             duplicates = {
-                fld.name for fld in self.fields
-                if fld.name in field_names
+                fld.id for fld in self.fields
+                if fld.id in field_ids
             }
             raise ValueError(f"Field names {duplicates} are duplicated")
 
-        wild_overriden_types = self.overriden_types - field_names
+        wild_overriden_types = self.overriden_types - field_ids
         if wild_overriden_types:
             raise ValueError(f"overriden_types contains non existing fields {wild_overriden_types} ")
 
     def __post_init__(self):
         self._validate()
-        super().__setattr__('fields_dict', {fld.name: fld for fld in self.fields})
+        super().__setattr__('fields_dict', {fld.id: fld for fld in self.fields})
 
 
 @dataclass(frozen=True)
 class ParamKwargs:
     type: TypeHint
 
 
 @dataclass(frozen=True)
-class InputFigure(BaseFigure, Generic[T]):
+class InputShape(BaseShape, Generic[T]):
     """Description of desired object creation
 
     :param constructor: callable that produces an instance of the class.
     :param fields: parameters of the constructor
     """
     fields: VarTuple[InputField]
     kwargs: Optional[ParamKwargs]
@@ -245,35 +249,35 @@
                 raise ValueError(
                     f"All not required fields must be after required ones"
                     f" except {ParamKind.KW_ONLY} fields"
                 )
 
 
 @dataclass(frozen=True)
-class OutputFigure(BaseFigure):
+class OutputShape(BaseShape):
     """Description of extraction data from an object
 
     :param fields: fields (can be not only attributes) of object
     """
     fields: VarTuple[OutputField]
     fields_dict: Mapping[str, OutputField] = field(init=False, hash=False, repr=False, compare=False)
 
 
-Inp = TypeVar('Inp', bound=Optional[InputFigure])
-Out = TypeVar('Out', bound=Optional[OutputFigure])
+Inp = TypeVar('Inp', bound=Optional[InputShape])
+Out = TypeVar('Out', bound=Optional[OutputShape])
 
 
 @dataclass
-class Figure(Generic[Inp, Out]):
+class Shape(Generic[Inp, Out]):
     input: Inp
     output: Out
 
 
-FullFigure = Figure[InputFigure, OutputFigure]
-FigureIntrospector = Callable[[Any], Figure]
+FullShape = Shape[InputShape, OutputShape]
+ShapeIntrospector = Callable[[Any], Shape]
 
 
 class IntrospectionImpossible(Exception):
     pass
 
 
 class NoTargetPackage(IntrospectionImpossible):
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/model_tools/introspection.py` & `adaptix-3.0.0a4/src/adaptix/_internal/model_tools/introspection.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 from ..feature_requirement import HAS_ATTRS_PKG, HAS_PY_39
 from ..model_tools.definitions import (
     AttrAccessor,
     BaseField,
     Default,
     DefaultFactory,
     DefaultValue,
-    Figure,
-    FullFigure,
+    FullShape,
     InputField,
-    InputFigure,
+    InputShape,
     IntrospectionImpossible,
     ItemAccessor,
     NoDefault,
     NoTargetPackage,
     OutputField,
-    OutputFigure,
+    OutputShape,
     ParamKind,
     ParamKwargs,
+    Shape,
 )
 from ..type_tools import get_all_type_hints, is_named_tuple_class, is_typed_dict_class
 
 try:
     import attrs
 except ImportError:
     attrs = None  # type: ignore[assignment]
@@ -44,47 +44,47 @@
 }
 
 
 def _is_empty(value):
     return value is Signature.empty
 
 
-def get_callable_figure(func, params_slice=slice(0, None)) -> Figure[InputFigure, None]:
+def get_callable_shape(func, params_slice=slice(0, None)) -> Shape[InputShape, None]:
     try:
         signature = inspect.signature(func)
     except TypeError:
         raise IntrospectionImpossible
 
     params = list(signature.parameters.values())[params_slice]
     kinds = [p.kind for p in params]
 
     if Parameter.VAR_POSITIONAL in kinds:
         raise IntrospectionImpossible(
-            f'Can not create InputFigure'
+            f'Can not create InputShape'
             f' from the function that has {Parameter.VAR_POSITIONAL}'
             f' parameter'
         )
 
     param_kwargs = next(
         (
             ParamKwargs(Any if _is_empty(param.annotation) else param.annotation)
             for param in params if param.kind == Parameter.VAR_KEYWORD
         ),
         None,
     )
 
     type_hints = get_all_type_hints(func)
 
-    return Figure(
-        input=InputFigure(
+    return Shape(
+        input=InputShape(
             constructor=func,
             fields=tuple(
                 InputField(
                     type=type_hints.get(param.name, Any),
-                    name=param.name,
+                    id=param.name,
                     is_required=_is_empty(param.default) or param.kind == Parameter.POSITIONAL_ONLY,
                     default=NoDefault() if _is_empty(param.default) else DefaultValue(param.default),
                     metadata=MappingProxyType({}),
                     param_kind=_PARAM_KIND_CONV[param.kind],
                     param_name=param.name,
                 )
                 for param in params
@@ -101,60 +101,60 @@
     )
 
 
 # ======================
 #       NamedTuple
 # ======================
 
-def get_named_tuple_figure(tp) -> FullFigure:
+def get_named_tuple_shape(tp) -> FullShape:
     # pylint: disable=protected-access
     if not is_named_tuple_class(tp):
         raise IntrospectionImpossible
 
     type_hints = get_all_type_hints(tp)
     if tuple in tp.__bases__:
         overriden_types = frozenset(tp._fields)
     else:
         overriden_types = frozenset(tp.__annotations__.keys() & set(tp._fields))
 
     # noinspection PyProtectedMember
-    input_figure = InputFigure(
+    input_shape = InputShape(
         constructor=tp,
         kwargs=None,
         fields=tuple(
             InputField(
-                name=field_name,
-                type=type_hints.get(field_name, Any),
+                id=field_id,
+                type=type_hints.get(field_id, Any),
                 default=(
-                    DefaultValue(tp._field_defaults[field_name])
-                    if field_name in tp._field_defaults else
+                    DefaultValue(tp._field_defaults[field_id])
+                    if field_id in tp._field_defaults else
                     NoDefault()
                 ),
-                is_required=field_name not in tp._field_defaults,
-                param_name=field_name,
+                is_required=field_id not in tp._field_defaults,
+                param_name=field_id,
                 metadata=MappingProxyType({}),
                 param_kind=ParamKind.POS_OR_KW,
             )
-            for field_name in tp._fields
+            for field_id in tp._fields
         ),
         overriden_types=overriden_types,
     )
 
-    return Figure(
-        input=input_figure,
-        output=OutputFigure(
+    return Shape(
+        input=input_shape,
+        output=OutputShape(
             fields=tuple(
                 OutputField(
-                    name=fld.name,
+                    id=fld.id,
                     type=fld.type,
                     default=fld.default,
                     metadata=fld.metadata,
-                    accessor=AttrAccessor(attr_name=fld.name, is_required=True),
+                    accessor=AttrAccessor(attr_name=fld.id, is_required=True),
                 )
-                for fld in input_figure.fields
+                for fld in input_shape.fields
             ),
             overriden_types=overriden_types,
         )
     )
 
 
 # =====================
@@ -186,45 +186,45 @@
 
 def _get_td_hints(tp):
     elements = list(get_all_type_hints(tp).items())
     elements.sort(key=lambda v: v[0])
     return elements
 
 
-def get_typed_dict_figure(tp) -> FullFigure:
+def get_typed_dict_shape(tp) -> FullShape:
     # __annotations__ of TypedDict contains also parents type hints unlike any other classes,
     # so overriden_types always contains all fields
     if not is_typed_dict_class(tp):
         raise IntrospectionImpossible
 
     requirement_determinant = _td_make_requirement_determinant(tp)
     type_hints = _get_td_hints(tp)
-    return Figure(
-        input=InputFigure(
+    return Shape(
+        input=InputShape(
             constructor=tp,
             fields=tuple(
                 InputField(
                     type=tp,
-                    name=name,
+                    id=name,
                     default=NoDefault(),
                     is_required=requirement_determinant(name),
                     metadata=MappingProxyType({}),
                     param_kind=ParamKind.KW_ONLY,
                     param_name=name,
                 )
                 for name, tp in type_hints
             ),
             kwargs=None,
             overriden_types=frozenset(tp.__annotations__.keys()),
         ),
-        output=OutputFigure(
+        output=OutputShape(
             fields=tuple(
                 OutputField(
                     type=tp,
-                    name=name,
+                    id=name,
                     default=NoDefault(),
                     accessor=ItemAccessor(name, requirement_determinant(name)),
                     metadata=MappingProxyType({}),
                 )
                 for name, tp in type_hints
             ),
             overriden_types=frozenset(tp.__annotations__.keys()),
@@ -252,24 +252,24 @@
     return NoDefault()
 
 
 def create_inp_field_from_dc_fields(dc_field: DCField, type_hints):
     default = get_dc_default(dc_field)
     return InputField(
         type=type_hints[dc_field.name],
-        name=dc_field.name,
+        id=dc_field.name,
         default=default,
         is_required=default == NoDefault(),
         metadata=dc_field.metadata,
         param_kind=ParamKind.POS_OR_KW,
         param_name=dc_field.name,
     )
 
 
-def get_dataclass_figure(tp) -> FullFigure:
+def get_dataclass_shape(tp) -> FullShape:
     """This function does not work properly if __init__ signature differs from
     that would be created by dataclass decorator.
 
     It happens because we can not distinguish __init__ that generated
     by @dataclass and __init__ that created by other ways.
     And we can not analyze only __init__ signature
     because @dataclass uses private constant
@@ -282,32 +282,32 @@
     name_to_dc_field = all_dc_fields(tp)
     dc_fields_public = dc_fields(tp)
     init_params = list(
         inspect.signature(tp.__init__).parameters.keys()
     )[1:]
     type_hints = get_all_type_hints(tp)
 
-    return Figure(
-        input=InputFigure(
+    return Shape(
+        input=InputShape(
             constructor=tp,
             fields=tuple(
-                create_inp_field_from_dc_fields(name_to_dc_field[field_name], type_hints)
-                for field_name in init_params
+                create_inp_field_from_dc_fields(name_to_dc_field[field_id], type_hints)
+                for field_id in init_params
             ),
             kwargs=None,
             overriden_types=frozenset(
-                field_name for field_name in init_params
-                if field_name in tp.__annotations__
+                field_id for field_id in init_params
+                if field_id in tp.__annotations__
             ),
         ),
-        output=OutputFigure(
+        output=OutputShape(
             fields=tuple(
                 OutputField(
                     type=type_hints[field.name],
-                    name=field.name,
+                    id=field.name,
                     default=get_dc_default(name_to_dc_field[field.name]),
                     accessor=AttrAccessor(field.name, True),
                     metadata=field.metadata,
                 )
                 for field in dc_fields_public
             ),
             overriden_types=frozenset(
@@ -318,27 +318,27 @@
     )
 
 
 # ======================
 #       ClassInit
 # ======================
 
-def get_class_init_figure(tp) -> Figure[InputFigure, None]:
+def get_class_init_shape(tp) -> Shape[InputShape, None]:
     if not isinstance(tp, type):
         raise IntrospectionImpossible
 
-    figure = get_callable_figure(
+    shape = get_callable_shape(
         tp.__init__,  # type: ignore[misc]
         slice(1, None)
     )
 
     return replace(
-        figure,
+        shape,
         input=replace(
-            figure.input,
+            shape.input,
             constructor=tp,
         )
     )
 
 # =================
 #       Attrs
 # =================
@@ -371,48 +371,48 @@
 
 def _process_attr_input_field(
     field: InputField,
     param_name_to_base_field: Dict[str, BaseField],
     has_custom_init: bool,
 ):
     try:
-        base_field = param_name_to_base_field[field.name]
+        base_field = param_name_to_base_field[field.id]
     except KeyError:
         return field
 
-    # When input figure is generating we rely on __init__ signature,
+    # When input shape is generating we rely on __init__ signature,
     # but when field type is None attrs thinks that there is no type hint,
     # so if there is no custom __init__ (that can do not set type for this attribute),
     # we should use NoneType as type of field
     if not has_custom_init and field.type == Any and base_field.type == NoneType:
         field = replace(field, type=NoneType)
 
     return replace(
         field,
         default=(
             base_field.default
             if isinstance(field.default, DefaultValue) and field.default.value is attrs.NOTHING else
             field.default
         ),
         metadata=base_field.metadata,
-        name=base_field.name,
+        id=base_field.id,
     )
 
 
 def _get_attrs_param_name(attrs_field):
     if hasattr(attrs_field, 'alias'):
         return attrs_field.alias
     return (
         attrs_field.name[1:]
         if attrs_field.name.startswith("_") and not attrs_field.name.startswith("__") else
         attrs_field.name
     )
 
 
-def get_attrs_figure(tp) -> FullFigure:
+def get_attrs_shape(tp) -> FullShape:
     if not HAS_ATTRS_PKG:
         raise NoTargetPackage
 
     try:
         is_attrs = attrs.has(tp)
     except TypeError:
         raise IntrospectionImpossible
@@ -431,51 +431,51 @@
     }
     param_name_to_base_field = {
         _get_attrs_param_name(attrs_fld): BaseField(
             # if field is not annotated, type attribute will store None value
             type=_get_attrs_field_type(attrs_fld, type_hints),
             default=_get_attrs_default(attrs_fld),
             metadata=attrs_fld.metadata,
-            name=attrs_fld.name,
+            id=attrs_fld.name,
         )
         for attrs_fld in attrs_fields
     }
 
     has_custom_init = hasattr(tp, '__attrs_init__')
 
-    figure = get_class_init_figure(tp)
+    shape = get_class_init_shape(tp)
     input_fields = tuple(
         _process_attr_input_field(field, param_name_to_base_field, has_custom_init)
-        for field in figure.input.fields
+        for field in shape.input.fields
     )
-    input_figure = replace(
-        figure.input,
+    input_shape = replace(
+        shape.input,
         fields=input_fields,
         overriden_types=frozenset(
-            (fld.name for fld in input_fields)
+            (fld.id for fld in input_fields)
             if has_custom_init else
-            (fld.name for fld in input_fields if not attrs_fields_dict[fld.name].inherited)
+            (fld.id for fld in input_fields if not attrs_fields_dict[fld.id].inherited)
         ),
     )
     output_fields = tuple(
         OutputField(
-            name=field.name,
-            type=_get_attrs_field_type(field, type_hints),
+            id=field.id,
+            type=field.type,
             default=(
-                input_figure.fields_dict[field.name].default
-                if field.name in input_figure.fields_dict else
+                input_shape.fields_dict[field.id].default
+                if field.id in input_shape.fields_dict else
                 NoDefault()
             ),
             metadata=field.metadata,
-            accessor=AttrAccessor(field.name, is_required=True),
+            accessor=AttrAccessor(field.id, is_required=True),
         )
         for field in param_name_to_base_field.values()
     )
-    return Figure(
-        input=input_figure,
-        output=OutputFigure(
+    return Shape(
+        input=input_shape,
+        output=OutputShape(
             fields=output_fields,
             overriden_types=frozenset(
-                fld.name for fld in output_fields if not attrs_fields_dict[fld.name].inherited
+                fld.id for fld in output_fields if not attrs_fields_dict[fld.id].inherited
             ),
         ),
     )
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/concrete_provider.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/concrete_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from dataclasses import dataclass, replace
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal, InvalidOperation
 from fractions import Fraction
 from typing import Generic, Type, TypeVar, Union
 
 from ..common import Dumper, Loader
+from ..essential import CannotProvide, Mediator
 from ..load_error import DatetimeFormatMismatch, TypeLoadError, ValueLoadError
-from .essential import CannotProvide, Mediator
+from .model.special_cases_optimization import none_loader
 from .provider_template import DumperProvider, LoaderProvider, ProviderWithAttachableRC, for_predicate
 from .request_cls import DumperRequest, LoaderRequest, StrictCoercionRequest, TypeHintLoc
 from .request_filtering import create_request_checker
 
 T = TypeVar('T')
 
 
@@ -89,20 +90,14 @@
 
         return timedelta_loader
 
     def _provide_dumper(self, mediator: Mediator, request: DumperRequest) -> Dumper:
         return timedelta.total_seconds
 
 
-def none_loader(data):
-    if data is None:
-        return None
-    raise TypeLoadError(None)
-
-
 @for_predicate(None)
 class NoneProvider(LoaderProvider, DumperProvider):
     def _provide_loader(self, mediator: Mediator, request: LoaderRequest) -> Loader:
         return none_loader
 
     def _provide_dumper(self, mediator: Mediator, request: DumperRequest) -> Dumper:
         return stub
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/essential.py` & `adaptix-3.0.0a4/src/adaptix/_internal/essential.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,18 +43,19 @@
     """Mediator is an object that gives provider access to other providers
     and that stores state of the current search.
 
     Mediator is a proxy to providers of retort.
     """
 
     @abstractmethod
-    def provide(self, request: Request[T]) -> T:
+    def provide(self, request: Request[T], *, extra_stack: Sequence[Request[Any]] = ()) -> T:
         """Get response of sent request.
 
         :param request: A request instance
+        :param extra_stack: Additional stack that will be added to :attr:`.request_stack` before passed request
         :return: Result of the request processing
         :raise CannotProvide: A provider able to process the request does not found
         """
 
     @abstractmethod
     def provide_from_next(self) -> V:
         """Forward current request to providers
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/generic_provider.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/generic_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import collections.abc
-from abc import ABC
 from dataclasses import dataclass, replace
-from enum import EnumMeta, Flag
 from inspect import isabstract
 from typing import Any, Callable, Collection, Container, Dict, Iterable, Literal, Mapping, Tuple, Union
 
-from ..common import Dumper, Loader, TypeHint
-from ..load_error import BadVariantError, ExcludedTypeLoadError, LoadError, MsgError, TypeLoadError, UnionLoadError
+from ..common import Dumper, Loader
+from ..essential import CannotProvide, Mediator
+from ..load_error import ExcludedTypeLoadError, LoadError, TypeLoadError, UnionLoadError
 from ..struct_path import append_path
 from ..type_tools import BaseNormType, is_new_type, is_subclass_soft, normalize_type, strip_tags
 from ..utils import ClassDispatcher
-from .essential import CannotProvide, Mediator, Request
+from .model.special_cases_optimization import as_is_stub
 from .provider_template import DumperProvider, LoaderProvider, for_predicate
 from .request_cls import (
     DebugPathRequest,
     DumperRequest,
     GenericParamLoc,
     LoaderRequest,
     LocatedRequest,
     LocMap,
     StrictCoercionRequest,
     TypeHintLoc,
     get_type_from_request,
 )
-from .request_filtering import DirectMediator, RequestChecker
 from .static_provider import StaticProvider, static_provision_action
 
 
 def stub(arg):
     return arg
 
 
@@ -112,32 +110,64 @@
         return stub
 
 
 @for_predicate(Union)
 class UnionProvider(LoaderProvider, DumperProvider):
     def _provide_loader(self, mediator: Mediator, request: LoaderRequest) -> Loader:
         norm = normalize_type(get_type_from_request(request))
+        debug_path = mediator.provide(DebugPathRequest(loc_map=request.loc_map))
+
+        if self._is_single_optional(norm):
+            non_optional = next(case for case in norm.args if case.origin is not None)
+            non_optional_loader = mediator.provide(
+                LoaderRequest(
+                    loc_map=LocMap(
+                        TypeHintLoc(type=non_optional.source),
+                        GenericParamLoc(pos=0),
+                    )
+                )
+            )
+            if debug_path:
+                return self._single_optional_dp_loader(non_optional_loader)
+            return self._single_optional_non_dp_loader(non_optional_loader)
 
         loaders = tuple(
             mediator.provide(
                 LoaderRequest(
                     loc_map=LocMap(
                         TypeHintLoc(type=tp.source),
                         GenericParamLoc(pos=i),
                     )
                 )
             )
             for i, tp in enumerate(norm.args)
         )
-        debug_path = mediator.provide(DebugPathRequest(loc_map=request.loc_map))
-
         if debug_path:
             return self._get_loader_dp(loaders)
         return self._get_loader_non_dp(loaders)
 
+    def _single_optional_non_dp_loader(self, loader: Loader) -> Loader:
+        def optional_non_dp_loader(data):
+            if data is None:
+                return None
+            return loader(data)
+
+        return optional_non_dp_loader
+
+    def _single_optional_dp_loader(self, loader: Loader) -> Loader:
+        def optional_dp_loader(data):
+            if data is None:
+                return None
+            try:
+                return loader(data)
+            except LoadError as e:
+                raise UnionLoadError([TypeLoadError(None), e])
+
+        return optional_dp_loader
+
     def _get_loader_dp(self, loader_iter: Iterable[Loader]) -> Loader:
         def union_loader_dp(data):
             errors = []
             for loader in loader_iter:
                 try:
                     return loader(data)
                 except LoadError as e:
@@ -176,14 +206,16 @@
                 DumperRequest(
                     loc_map=LocMap(
                         TypeHintLoc(type=non_optional.source),
                         GenericParamLoc(pos=0),
                     )
                 )
             )
+            if non_optional_dumper == as_is_stub:
+                return as_is_stub
             return self._get_single_optional_dumper(non_optional_dumper)
 
         non_class_origins = [case.source for case in norm.args if not self._is_class_origin(case.origin)]
         if non_class_origins:
             raise ValueError(
                 f"Can not create dumper for {request_type}."
                 f" All cases of union must be class, but found {non_class_origins}"
@@ -196,31 +228,35 @@
                         TypeHintLoc(type=tp.source),
                         GenericParamLoc(pos=i),
                     )
                 )
             )
             for i, tp in enumerate(norm.args)
         )
+        if all(dumper == as_is_stub for dumper in dumpers):
+            return as_is_stub
 
-        dumper_type_dispatcher = ClassDispatcher({case.origin: dumper for case, dumper in zip(norm.args, dumpers)})
+        dumper_type_dispatcher = ClassDispatcher(
+            {type(None) if case.origin is None else case.origin: dumper for case, dumper in zip(norm.args, dumpers)}
+        )
         return self._get_dumper(dumper_type_dispatcher)
 
     def _get_dumper(self, dumper_type_dispatcher: ClassDispatcher[Any, Dumper]) -> Dumper:
         def union_dumper(data):
             return dumper_type_dispatcher.dispatch(type(data))(data)
 
         return union_dumper
 
     def _get_single_optional_dumper(self, dumper: Dumper) -> Dumper:
-        def union_so_dumper(data):
+        def optional_dumper(data):
             if data is None:
                 return None
             return dumper(data)
 
-        return union_so_dumper
+        return optional_dumper
 
 
 CollectionsMapping = collections.abc.Mapping
 
 
 @for_predicate(Iterable)
 class IterableProvider(LoaderProvider, DumperProvider):
@@ -551,118 +587,7 @@
             result = {}
             for k, v in data.items():
                 result[key_dumper(k)] = value_dumper(v)
 
             return result
 
         return dict_dumper
-
-
-class AnyEnumRC(RequestChecker):
-    def check_request(self, mediator: DirectMediator, request: Request) -> None:
-        if not isinstance(request, LocatedRequest):
-            raise CannotProvide
-
-        norm = normalize_type(get_type_from_request(request))
-
-        if not isinstance(norm.origin, EnumMeta):
-            raise CannotProvide
-
-
-class BaseEnumProvider(LoaderProvider, DumperProvider, ABC):
-    _request_checker = AnyEnumRC()
-
-
-def _enum_name_dumper(data):
-    return data.name
-
-
-class EnumNameProvider(BaseEnumProvider):
-    """This provider represents enum members to the outside world by their name"""
-
-    def _provide_loader(self, mediator: Mediator, request: LoaderRequest) -> Loader:
-        enum = get_type_from_request(request)
-
-        if issubclass(enum, Flag):
-            raise ValueError(f"Can not use {type(self).__name__} with Flag subclass {enum}")
-
-        variants = [case.name for case in enum]
-
-        def enum_loader(data):
-            try:
-                return enum[data]
-            except KeyError:
-                raise BadVariantError(variants)
-            except TypeError:
-                raise BadVariantError(variants)
-
-        return enum_loader
-
-    def _provide_dumper(self, mediator: Mediator, request: DumperRequest) -> Dumper:
-        return _enum_name_dumper
-
-
-class EnumValueProvider(BaseEnumProvider):
-    def __init__(self, value_type: TypeHint):
-        self._value_type = value_type
-
-    def _provide_loader(self, mediator: Mediator, request: LoaderRequest) -> Loader:
-        enum = get_type_from_request(request)
-        value_loader = mediator.provide(
-            LoaderRequest(
-                loc_map=LocMap(
-                    TypeHintLoc(type=self._value_type),
-                )
-            ),
-        )
-
-        def enum_loader(data):
-            loaded_value = value_loader(data)
-            try:
-                return enum(loaded_value)
-            except ValueError:
-                raise MsgError("Bad enum value")
-
-        return enum_loader
-
-    def _provide_dumper(self, mediator: Mediator, request: DumperRequest) -> Dumper:
-        value_dumper = mediator.provide(
-            DumperRequest(
-                loc_map=LocMap(
-                    TypeHintLoc(type=self._value_type)
-                )
-            )
-        )
-
-        def enum_dumper(data):
-            return value_dumper(data.value)
-
-        return enum_dumper
-
-
-def _enum_exact_value_dumper(data):
-    return data.value
-
-
-class EnumExactValueProvider(BaseEnumProvider):
-    """This provider represents enum members to the outside world
-    by their value without any processing
-    """
-
-    def _provide_loader(self, mediator: Mediator, request: LoaderRequest) -> Loader:
-        enum = get_type_from_request(request)
-        variants = [case.value for case in enum]
-
-        def enum_exact_loader(data):
-            # since MyEnum(MyEnum.MY_CASE) == MyEnum.MY_CASE
-            if isinstance(data, enum):
-                raise BadVariantError(variants)
-
-            try:
-                return enum(data)
-            except ValueError:
-                raise BadVariantError(variants)
-
-        return enum_exact_loader
-
-    def _provide_dumper(self, mediator: Mediator, request: DumperRequest) -> Dumper:
-        return _enum_exact_value_dumper
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/basic_gen.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/model/basic_gen.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,26 +13,28 @@
     Sequence,
     Set,
     Tuple,
     TypeVar,
     Union,
 )
 
-from ...code_tools import ClosureCompiler, CodeBuilder, get_literal_expr
-from ...model_tools import InputField, OutputField
-from ..essential import Mediator, Request
+from ...code_tools.code_builder import CodeBuilder
+from ...code_tools.compiler import ClosureCompiler
+from ...code_tools.utils import get_literal_expr
+from ...essential import Mediator, Request
+from ...model_tools.definitions import InputField, OutputField
 from ..static_provider import StaticProvider, static_provision_action
 from .crown_definitions import (
     BaseCrown,
     BaseDictCrown,
     BaseFieldCrown,
-    BaseFigure,
     BaseListCrown,
     BaseNameLayout,
     BaseNoneCrown,
+    BaseShape,
     ExtraCollect,
     ExtraTargets,
     InpCrown,
     InpDictCrown,
     InpExtraMove,
     InpFieldCrown,
     InpListCrown,
@@ -91,15 +93,15 @@
         )
     if isinstance(crown, BaseListCrown):
         return _concatenate_iters(
             _inner_collect_used_direct_fields(sub_crown)
             for sub_crown in crown.map
         )
     if isinstance(crown, BaseFieldCrown):
-        return [crown.name]
+        return [crown.id]
     if isinstance(crown, BaseNoneCrown):
         return []
     raise TypeError
 
 
 def _collect_used_direct_fields(crown: BaseCrown) -> Set[str]:
     lst = _inner_collect_used_direct_fields(crown)
@@ -109,24 +111,24 @@
         if f_name in used_set:
             raise ValueError(f"Field {f_name!r} is duplicated at crown")
         used_set.add(f_name)
 
     return used_set
 
 
-def get_skipped_fields(figure: BaseFigure, name_layout: BaseNameLayout) -> Collection[str]:
+def get_skipped_fields(shape: BaseShape, name_layout: BaseNameLayout) -> Collection[str]:
     used_direct_fields = _collect_used_direct_fields(name_layout.crown)
     if isinstance(name_layout.extra_move, ExtraTargets):
         extra_targets = name_layout.extra_move.fields
     else:
         extra_targets = ()
 
     return [
-        field.name for field in figure.fields
-        if field.name not in used_direct_fields and field.name not in extra_targets
+        field.id for field in shape.fields
+        if field.id not in used_direct_fields and field.id not in extra_targets
     ]
 
 
 def _inner_get_extra_targets_at_crown(extra_targets: Container[str], crown: BaseCrown) -> Collection[str]:
     if isinstance(crown, BaseDictCrown):
         return _concatenate_iters(
             _inner_get_extra_targets_at_crown(extra_targets, sub_crown)
@@ -134,15 +136,15 @@
         )
     if isinstance(crown, BaseListCrown):
         return _concatenate_iters(
             _inner_get_extra_targets_at_crown(extra_targets, sub_crown)
             for sub_crown in crown.map
         )
     if isinstance(crown, BaseFieldCrown):
-        return [crown.name] if crown.name in extra_targets else []
+        return [crown.id] if crown.id in extra_targets else []
     if isinstance(crown, BaseNoneCrown):
         return []
     raise TypeError
 
 
 def get_extra_targets_at_crown(name_layout: BaseNameLayout) -> Collection[str]:
     if not isinstance(name_layout.extra_move, ExtraTargets):
@@ -159,50 +161,50 @@
         return _concatenate_iters(
             get_optional_fields_at_list_crown(fields_map, sub_crown)
             for sub_crown in crown.map.values()
         )
     if isinstance(crown, BaseListCrown):
         return _concatenate_iters(
             (
-                [sub_crown.name]
-                if fields_map[sub_crown.name].is_optional else
+                [sub_crown.id]
+                if fields_map[sub_crown.id].is_optional else
                 []
             )
             if isinstance(sub_crown, BaseFieldCrown) else
             get_optional_fields_at_list_crown(fields_map, sub_crown)
             for sub_crown in crown.map
         )
     if isinstance(crown, (BaseFieldCrown, BaseNoneCrown)):
         return []
     raise TypeError
 
 
-def get_wild_extra_targets(figure: BaseFigure, extra_move: Union[InpExtraMove, OutExtraMove]) -> Collection[str]:
+def get_wild_extra_targets(shape: BaseShape, extra_move: Union[InpExtraMove, OutExtraMove]) -> Collection[str]:
     if not isinstance(extra_move, ExtraTargets):
         return []
 
     return [
         target for target in extra_move.fields
-        if target not in figure.fields_dict.keys()
+        if target not in shape.fields_dict.keys()
     ]
 
 
-Fig = TypeVar('Fig', bound=BaseFigure)
+ShapeT = TypeVar('ShapeT', bound=BaseShape)
 
 
-def strip_figure_fields(figure: Fig, skipped_fields: Collection[str]) -> Fig:
+def strip_shape_fields(shape: ShapeT, skipped_fields: Collection[str]) -> ShapeT:
     return replace(
-        figure,
+        shape,
         fields=tuple(
-            field for field in figure.fields
-            if field.name not in skipped_fields
+            field for field in shape.fields
+            if field.id not in skipped_fields
         ),
         overriden_types=frozenset(
-            field.name for field in figure.fields
-            if field.name not in skipped_fields
+            field.id for field in shape.fields
+            if field.id not in skipped_fields
         )
     )
 
 
 class NameSanitizer:
     _AVAILABLE_CHARS = set(string.ascii_letters + string.digits)
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/crown_definitions.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/model/crown_definitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, Generic, Mapping, MutableMapping, Sequence, TypeVar, Union
+from typing import Any, Callable, Dict, Generic, Mapping, Sequence, TypeVar, Union
 
 from ...common import VarTuple
-from ...model_tools import BaseFigure, DefaultFactory, DefaultValue, InputFigure, OutputFigure
+from ...model_tools.definitions import BaseShape, DefaultFactory, DefaultValue, InputShape, OutputShape
 from ...utils import SingletonMeta
 from ..request_cls import LocatedRequest
 
 T = TypeVar('T')
 
 CrownPathElem = Union[str, int]
 CrownPath = VarTuple[CrownPathElem]  # subset of struct_path.Path
@@ -48,15 +48,15 @@
 @dataclass
 class BaseNoneCrown:
     pass
 
 
 @dataclass
 class BaseFieldCrown:
-    name: str
+    id: str
 
 
 BranchBaseCrown = Union[BaseDictCrown, BaseListCrown]
 LeafBaseCrown = Union[BaseFieldCrown, BaseNoneCrown]
 BaseCrown = Union[BranchBaseCrown, LeafBaseCrown]
 
 # --------  Input Crown -------- #
@@ -141,15 +141,15 @@
 
 
 @dataclass(frozen=True)
 class ExtraTargets:
     fields: VarTuple[str]
 
 
-Saturator = Callable[[T, MutableMapping[str, Any]], None]
+Saturator = Callable[[T, Mapping[str, Any]], None]
 Extractor = Callable[[T], Mapping[str, Any]]
 
 
 @dataclass(frozen=True)
 class ExtraSaturate(Generic[T]):
     func: Saturator[T]
 
@@ -168,30 +168,30 @@
 class BaseNameLayout:
     crown: BranchBaseCrown
     extra_move: BaseExtraMove
 
 
 @dataclass(frozen=True)
 class BaseNameLayoutRequest(LocatedRequest[T], Generic[T]):
-    figure: BaseFigure
+    shape: BaseShape
 
 
 @dataclass(frozen=True)
 class InputNameLayout(BaseNameLayout):
     crown: BranchInpCrown
     extra_move: InpExtraMove
 
 
 @dataclass(frozen=True)
 class InputNameLayoutRequest(BaseNameLayoutRequest[InputNameLayout]):
-    figure: InputFigure
+    shape: InputShape
 
 
 @dataclass(frozen=True)
 class OutputNameLayout(BaseNameLayout):
     crown: BranchOutCrown
     extra_move: OutExtraMove
 
 
 @dataclass(frozen=True)
 class OutputNameLayoutRequest(BaseNameLayoutRequest[OutputNameLayout]):
-    figure: OutputFigure
+    shape: OutputShape
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/dumper_provider.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/model/dumper_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,135 +1,125 @@
 from typing import Protocol, Tuple
 
-from ...code_tools import BasicClosureCompiler, BuiltinContextNamespace
+from ...code_tools.compiler import BasicClosureCompiler
+from ...code_tools.context_namespace import BuiltinContextNamespace
 from ...common import Dumper
-from ..essential import CannotProvide, Mediator
+from ...essential import CannotProvide, Mediator
 from ..provider_template import DumperProvider
-from ..request_cls import DebugPathRequest, DumperRequest, FieldLoc, LocMap, OutputFieldLoc, TypeHintLoc
+from ..request_cls import DebugPathRequest, DumperRequest, TypeHintLoc
 from .basic_gen import (
     CodeGenHookRequest,
     NameSanitizer,
     compile_closure_with_globals_capturing,
     get_extra_targets_at_crown,
     get_optional_fields_at_list_crown,
     get_skipped_fields,
     get_wild_extra_targets,
-    strip_figure_fields,
+    strip_shape_fields,
     stub_code_gen_hook,
 )
 from .crown_definitions import OutExtraMove, OutputNameLayout, OutputNameLayoutRequest
-from .definitions import CodeGenerator, OutputFigure, OutputFigureRequest, VarBinder
-from .figure_provider import provide_generic_resolved_figure
+from .definitions import CodeGenerator, OutputShape, OutputShapeRequest, VarBinder
+from .fields import output_field_to_loc_map
 from .output_creation_gen import BuiltinOutputCreationGen
 from .output_extraction_gen import BuiltinOutputExtractionGen
+from .shape_provider import provide_generic_resolved_shape
 
 
 class OutputExtractionMaker(Protocol):
     def __call__(
         self,
         mediator: Mediator,
         request: DumperRequest,
-        figure: OutputFigure,
+        shape: OutputShape,
         extra_move: OutExtraMove,
     ) -> CodeGenerator:
         ...
 
 
 class OutputCreationMaker(Protocol):
     def __call__(
         self,
         mediator: Mediator,
         request: DumperRequest,
-    ) -> Tuple[CodeGenerator, OutputFigure, OutExtraMove]:
+    ) -> Tuple[CodeGenerator, OutputShape, OutExtraMove]:
         ...
 
 
 def make_output_extraction(
     mediator: Mediator,
     request: DumperRequest,
-    figure: OutputFigure,
+    shape: OutputShape,
     extra_move: OutExtraMove,
 ) -> CodeGenerator:
     field_dumpers = {
-        field.name: mediator.provide(
+        field.id: mediator.provide(
             DumperRequest(
-                loc_map=LocMap(
-                    TypeHintLoc(
-                        type=field.type,
-                    ),
-                    FieldLoc(
-                        name=field.name,
-                        default=field.default,
-                        metadata=field.metadata,
-                    ),
-                    OutputFieldLoc(
-                        accessor=field.accessor,
-                    )
-                ),
+                loc_map=output_field_to_loc_map(field),
             )
         )
-        for field in figure.fields
+        for field in shape.fields
     }
     debug_path = mediator.provide(DebugPathRequest(loc_map=request.loc_map))
     return BuiltinOutputExtractionGen(
-        figure=figure,
+        shape=shape,
         extra_move=extra_move,
         debug_path=debug_path,
         fields_dumpers=field_dumpers,
     )
 
 
 class BuiltinOutputCreationMaker(OutputCreationMaker):
-    def __call__(self, mediator: Mediator, request: DumperRequest) -> Tuple[CodeGenerator, OutputFigure, OutExtraMove]:
-        figure = provide_generic_resolved_figure(mediator, OutputFigureRequest(loc_map=request.loc_map))
+    def __call__(self, mediator: Mediator, request: DumperRequest) -> Tuple[CodeGenerator, OutputShape, OutExtraMove]:
+        shape = provide_generic_resolved_shape(mediator, OutputShapeRequest(loc_map=request.loc_map))
 
         name_layout = mediator.provide(
             OutputNameLayoutRequest(
                 loc_map=request.loc_map,
-                figure=figure,
+                shape=shape,
             )
         )
 
-        processed_figure = self._process_figure(figure, name_layout)
+        processed_shape = self._process_shape(shape, name_layout)
         debug_path = mediator.provide(DebugPathRequest(loc_map=request.loc_map))
-        creation_gen = self._create_creation_gen(debug_path, processed_figure, name_layout)
-        return creation_gen, processed_figure, name_layout.extra_move
+        creation_gen = self._create_creation_gen(debug_path, processed_shape, name_layout)
+        return creation_gen, processed_shape, name_layout.extra_move
 
-    def _process_figure(self, figure: OutputFigure, name_layout: OutputNameLayout) -> OutputFigure:
+    def _process_shape(self, shape: OutputShape, name_layout: OutputNameLayout) -> OutputShape:
         optional_fields_at_list_crown = get_optional_fields_at_list_crown(
-            {field.name: field for field in figure.fields},
+            {field.id: field for field in shape.fields},
             name_layout.crown,
         )
         if optional_fields_at_list_crown:
             raise ValueError(
                 f"Optional fields {optional_fields_at_list_crown} are found at list crown"
             )
 
-        wild_extra_targets = get_wild_extra_targets(figure, name_layout.extra_move)
+        wild_extra_targets = get_wild_extra_targets(shape, name_layout.extra_move)
         if wild_extra_targets:
             raise ValueError(
                 f"ExtraTargets {wild_extra_targets} are attached to non-existing fields"
             )
 
         extra_targets_at_crown = get_extra_targets_at_crown(name_layout)
         if extra_targets_at_crown:
             raise ValueError(
                 f"Extra targets {extra_targets_at_crown} are found at crown"
             )
 
-        return strip_figure_fields(figure, get_skipped_fields(figure, name_layout))
+        return strip_shape_fields(shape, get_skipped_fields(shape, name_layout))
 
     def _create_creation_gen(
         self,
         debug_path: bool,
-        figure: OutputFigure,
+        shape: OutputShape,
         name_layout: OutputNameLayout,
     ) -> CodeGenerator:
         return BuiltinOutputCreationGen(
-            figure=figure,
+            shape=shape,
             name_layout=name_layout,
             debug_path=debug_path,
         )
 
 
 class ModelDumperProvider(DumperProvider):
     def __init__(
@@ -139,16 +129,16 @@
         creation_maker: OutputCreationMaker,
     ):
         self._name_sanitizer = name_sanitizer
         self._extraction_maker = extraction_maker
         self._creation_maker = creation_maker
 
     def _provide_dumper(self, mediator: Mediator, request: DumperRequest) -> Dumper:
-        creation_gen, figure, extra_move = self._creation_maker(mediator, request)
-        extraction_gen = self._extraction_maker(mediator, request, figure, extra_move)
+        creation_gen, shape, extra_move = self._creation_maker(mediator, request)
+        extraction_gen = self._extraction_maker(mediator, request, shape, extra_move)
 
         try:
             code_gen_hook = mediator.provide(CodeGenHookRequest())
         except CannotProvide:
             code_gen_hook = stub_code_gen_hook
 
         binder = self._get_binder()
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/figure_provider.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/model/shape_provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,72 @@
 import inspect
 from dataclasses import replace
 from typing import Any, Container, Generic, Iterable, Optional, TypeVar, Union, cast
 
 from ...common import TypeHint
-from ...model_tools import (
+from ...essential import CannotProvide, Mediator
+from ...model_tools.definitions import (
     DescriptorAccessor,
+    InputShape,
     IntrospectionImpossible,
     OutputField,
-    OutputFigure,
-    get_attrs_figure,
-    get_class_init_figure,
-    get_dataclass_figure,
-    get_named_tuple_figure,
-    get_typed_dict_figure,
+    OutputShape,
+    ShapeIntrospector,
+)
+from ...model_tools.introspection import (
+    get_attrs_shape,
+    get_class_init_shape,
+    get_dataclass_shape,
+    get_named_tuple_shape,
+    get_typed_dict_shape,
 )
-from ...model_tools.definitions import FigureIntrospector, InputFigure
 from ...type_tools.generic_resolver import GenericResolver, MembersStorage
-from ..essential import CannotProvide, Mediator
+from ..provider_template import ProviderWithAttachableRC
 from ..request_cls import LocatedRequest, TypeHintLoc
+from ..request_filtering import create_request_checker
 from ..static_provider import StaticProvider, static_provision_action
-from .definitions import InputFigureRequest, OutputFigureRequest
+from .definitions import InputShapeRequest, OutputShapeRequest
 
 
-class FigureProvider(StaticProvider):
-    def __init__(self, introspector: FigureIntrospector):
+class ShapeProvider(StaticProvider):
+    def __init__(self, introspector: ShapeIntrospector):
         self._introspector = introspector
 
     @static_provision_action
-    def _provide_input_figure(self, mediator: Mediator, request: InputFigureRequest) -> InputFigure:
+    def _provide_input_shape(self, mediator: Mediator, request: InputShapeRequest) -> InputShape:
         loc = request.loc_map.get_or_raise(TypeHintLoc, CannotProvide)
         try:
-            figure = self._introspector(loc.type)
+            shape = self._introspector(loc.type)
         except IntrospectionImpossible:
             raise CannotProvide
 
-        if figure.input is None:
+        if shape.input is None:
             raise CannotProvide
 
-        return figure.input
+        return shape.input
 
     @static_provision_action
-    def _provide_output_figure(self, mediator: Mediator, request: OutputFigureRequest) -> OutputFigure:
+    def _provide_output_shape(self, mediator: Mediator, request: OutputShapeRequest) -> OutputShape:
         loc = request.loc_map.get_or_raise(TypeHintLoc, CannotProvide)
         try:
-            figure = self._introspector(loc.type)
+            shape = self._introspector(loc.type)
         except IntrospectionImpossible:
             raise CannotProvide
 
-        if figure.output is None:
+        if shape.output is None:
             raise CannotProvide
 
-        return figure.output
+        return shape.output
 
 
-NAMED_TUPLE_FIGURE_PROVIDER = FigureProvider(get_named_tuple_figure)
-TYPED_DICT_FIGURE_PROVIDER = FigureProvider(get_typed_dict_figure)
-DATACLASS_FIGURE_PROVIDER = FigureProvider(get_dataclass_figure)
-CLASS_INIT_FIGURE_PROVIDER = FigureProvider(get_class_init_figure)
-ATTRS_FIGURE_PROVIDER = FigureProvider(get_attrs_figure)
+NAMED_TUPLE_SHAPE_PROVIDER = ShapeProvider(get_named_tuple_shape)
+TYPED_DICT_SHAPE_PROVIDER = ShapeProvider(get_typed_dict_shape)
+DATACLASS_SHAPE_PROVIDER = ShapeProvider(get_dataclass_shape)
+CLASS_INIT_SHAPE_PROVIDER = ShapeProvider(get_class_init_shape)
+ATTRS_SHAPE_PROVIDER = ShapeProvider(get_attrs_shape)
 
 
 class PropertyAdder(StaticProvider):
     def __init__(
         self,
         output_fields: Iterable[OutputField],
         infer_types_for: Container[str],
@@ -75,25 +80,25 @@
         if bad_fields_accessors:
             raise ValueError(
                 f"Fields {bad_fields_accessors} has bad accessors,"
                 f" all fields must use DescriptorAccessor"
             )
 
     @static_provision_action
-    def _provide_output_figure(self, mediator: Mediator[OutputFigure], request: OutputFigureRequest) -> OutputFigure:
+    def _provide_output_shape(self, mediator: Mediator[OutputShape], request: OutputShapeRequest) -> OutputShape:
         tp = request.loc_map.get_or_raise(TypeHintLoc, CannotProvide).type
-        figure = mediator.provide_from_next()
+        shape = mediator.provide_from_next()
 
         additional_fields = tuple(
             replace(field, type=self._infer_property_type(tp, self._get_attr_name(field)))
-            if field.name in self._infer_types_for else
+            if field.id in self._infer_types_for else
             field
             for field in self._output_fields
         )
-        return replace(figure, fields=figure.fields + additional_fields)
+        return replace(shape, fields=shape.fields + additional_fields)
 
     def _get_attr_name(self, field: OutputField) -> str:
         return cast(DescriptorAccessor, field.accessor).attr_name
 
     def _infer_property_type(self, tp: TypeHint, attr_name: str) -> TypeHint:
         prop = getattr(tp, attr_name)
 
@@ -106,55 +111,95 @@
         signature = inspect.signature(prop.fget)
 
         if signature.return_annotation is inspect.Signature.empty:
             return Any
         return signature.return_annotation
 
 
-Fig = TypeVar('Fig', bound=Union[InputFigure, OutputFigure])
+ShapeT = TypeVar('ShapeT', bound=Union[InputShape, OutputShape])
 
 
-class FigureGenericResolver(Generic[Fig]):
-    def __init__(self, mediator: Mediator, initial_request: LocatedRequest[Fig]):
+class ShapeGenericResolver(Generic[ShapeT]):
+    def __init__(self, mediator: Mediator, initial_request: LocatedRequest[ShapeT]):
         self._mediator = mediator
         self._initial_request = initial_request
 
-    def provide(self) -> Fig:
+    def provide(self) -> ShapeT:
         resolver = GenericResolver(self._get_members)
         members_storage = resolver.get_resolved_members(
             self._initial_request.loc_map[TypeHintLoc].type
         )
         if members_storage.meta is None:
             raise CannotProvide
         return replace(
             members_storage.meta,
             fields=tuple(
-                replace(fld, type=members_storage.members[fld.name])
+                replace(fld, type=members_storage.members[fld.id])
                 for fld in members_storage.meta.fields
             )
         )
 
-    def _get_members(self, tp) -> MembersStorage[str, Optional[Fig]]:
+    def _get_members(self, tp) -> MembersStorage[str, Optional[ShapeT]]:
         try:
-            figure = self._mediator.provide(
+            shape = self._mediator.provide(
                 replace(
                     self._initial_request,
                     loc_map=self._initial_request.loc_map.add(TypeHintLoc(type=tp)),
                 )
             )
         except CannotProvide:
             return MembersStorage(
                 meta=None,
                 members={},
                 overriden=frozenset(),
             )
         return MembersStorage(
-            meta=figure,
-            members={field.name: field.type for field in figure.fields},
-            overriden=figure.overriden_types,
+            meta=shape,
+            members={field.id: field.type for field in shape.fields},
+            overriden=shape.overriden_types,
         )
 
 
-def provide_generic_resolved_figure(mediator: Mediator, request: LocatedRequest[Fig]) -> Fig:
+def provide_generic_resolved_shape(mediator: Mediator, request: LocatedRequest[ShapeT]) -> ShapeT:
     if not request.loc_map.has(TypeHintLoc):
         return mediator.provide(request)
-    return FigureGenericResolver(mediator, request).provide()
+    return ShapeGenericResolver(mediator, request).provide()
+
+
+T = TypeVar('T')
+
+
+class SimilarShapeProvider(ProviderWithAttachableRC):
+    def __init__(self, target: TypeHint, prototype: TypeHint, for_input: bool = True, for_output: bool = True):
+        self._target = target
+        self._prototype = prototype
+        self._request_checker = create_request_checker(self._target)
+        self._for_input = for_input
+        self._for_output = for_output
+
+    @static_provision_action
+    def _provide_input_shape(self, mediator: Mediator, request: InputShapeRequest) -> InputShape:
+        if not self._for_input:
+            raise CannotProvide
+
+        self._request_checker.check_request(mediator, request)
+        shape = mediator.provide(
+            replace(
+                request,
+                loc_map=request.loc_map.add(TypeHintLoc(self._prototype))
+            )
+        )
+        return replace(shape, constructor=self._target)
+
+    @static_provision_action
+    def _provide_output_shape(self, mediator: Mediator, request: OutputShapeRequest) -> OutputShape:
+        if not self._for_output:
+            raise CannotProvide
+
+        self._request_checker.check_request(mediator, request)
+        shape = mediator.provide(
+            replace(
+                request,
+                loc_map=request.loc_map.add(TypeHintLoc(self._prototype))
+            )
+        )
+        return shape
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/input_creation_gen.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/model/input_creation_gen.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-from ...code_tools import CodeBuilder, ContextNamespace
-from ...model_tools import InputField, ParamKind
+from ...code_tools.compiler import CodeBuilder
+from ...code_tools.context_namespace import ContextNamespace
+from ...model_tools.definitions import InputField, ParamKind
 from .crown_definitions import ExtraKwargs, ExtraSaturate, ExtraTargets, InpExtraMove
-from .definitions import CodeGenerator, InputFigure, VarBinder
+from .definitions import CodeGenerator, InputShape, VarBinder
 
 
 class BuiltinInputCreationGen(CodeGenerator):
     """Generator producing creation of desired object.
 
     It takes fields, extra and opt_fields from local vars to
     """
 
-    def __init__(self, figure: InputFigure, extra_move: InpExtraMove):
-        self._figure = figure
+    def __init__(self, shape: InputShape, extra_move: InpExtraMove):
+        self._shape = shape
         self._extra_move = extra_move
 
     def _is_extra_target(self, field: InputField):
         return (
             isinstance(self._extra_move, ExtraTargets)
             and
-            field.name in self._extra_move.fields
+            field.id in self._extra_move.fields
         )
 
     def __call__(self, binder: VarBinder, ctx_namespace: ContextNamespace) -> CodeBuilder:
         has_opt_fields = any(
             fld.is_optional and not self._is_extra_target(fld)
-            for fld in self._figure.fields
+            for fld in self._shape.fields
         )
 
         builder = CodeBuilder()
-        ctx_namespace.add('constructor', self._figure.constructor)
+        ctx_namespace.add('constructor', self._shape.constructor)
 
         with builder("constructor("):
-            for field in self._figure.fields:
+            for field in self._shape.fields:
 
                 if field.is_required or self._is_extra_target(field):
                     value = binder.field(field)
                 else:
                     continue
 
                 if field.param_kind == ParamKind.KW_ONLY:
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/input_extraction_gen.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/model/input_extraction_gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import contextlib
 from copy import copy
 from typing import Dict, Mapping, Optional, Set
 
-from ...code_tools import CodeBuilder, ContextNamespace
+from adaptix._internal.provider.model.special_cases_optimization import as_is_stub
+
+from ...code_tools.code_builder import CodeBuilder
+from ...code_tools.context_namespace import ContextNamespace
 from ...common import Loader
 from ...load_error import (
     ExtraFieldsError,
     ExtraItemsError,
     LoadError,
     NoRequiredFieldsError,
     NoRequiredItemsError,
     TypeLoadError,
 )
-from ...model_tools import InputField, InputFigure
+from ...model_tools.definitions import InputField, InputShape
 from ...struct_path import append_path, extend_path
 from .crown_definitions import (
     CrownPath,
     CrownPathElem,
     ExtraCollect,
     ExtraForbid,
     ExtraSkip,
@@ -35,15 +38,15 @@
     KNOWN_FIELDS = 'known_fields'
 
     def __init__(self, binder: VarBinder, ctx_namespace: ContextNamespace, name_to_field: Dict[str, InputField]):
         self.binder = binder
         self.ctx_namespace = ctx_namespace
         self._name_to_field = name_to_field
 
-        self.field_name2path: Dict[str, CrownPath] = {}
+        self.field_id2path: Dict[str, CrownPath] = {}
         self.path2suffix: Dict[CrownPath, str] = {}
         self.path2known_fields: Dict[CrownPath, Set[str]] = {}
 
         self._last_path_idx = 0
         self._path: CrownPath = ()
         self._parent_path: Optional[CrownPath] = None
 
@@ -69,19 +72,19 @@
 
     def get_extra_var_name(self) -> str:
         if not self._path:
             return self.binder.extra
 
         return self.binder.extra + '_' + self._get_path_idx(self._path)
 
-    def field_loader(self, field_name: str) -> str:
-        return f"loader_{field_name}"
+    def field_loader(self, field_id: str) -> str:
+        return f"loader_{field_id}"
 
     def raw_field(self, field: InputField) -> str:
-        return f"r_{field.name}"
+        return f"r_{field.id}"
 
     @property
     def path(self):
         return self._path
 
     @contextlib.contextmanager
     def add_key(self, key: CrownPathElem):
@@ -91,16 +94,16 @@
         self._parent_path = self._path
         self._path += (key,)
         yield
         self._path = past
         self._parent_path = past_parent
 
     def get_field(self, crown: InpFieldCrown) -> InputField:
-        self.field_name2path[crown.name] = self._path
-        return self._name_to_field[crown.name]
+        self.field_id2path[crown.id] = self._path
+        return self._name_to_field[crown.id]
 
     def with_parent_path(self) -> "GenState":
         # pylint: disable=protected-access
         if self._parent_path is None:
             raise ValueError
 
         cp = copy(self)
@@ -112,36 +115,36 @@
 class BuiltinInputExtractionGen(CodeGenerator):
     """BuiltinInputExtractionGen generates code that extracts raw values from input data,
     calls loaders and stores results to variables.
     """
 
     def __init__(
         self,
-        figure: InputFigure,
+        shape: InputShape,
         name_layout: InputNameLayout,
         debug_path: bool,
         field_loaders: Mapping[str, Loader],
     ):
-        self._figure = figure
+        self._shape = shape
         self._name_layout = name_layout
         self._debug_path = debug_path
         self._name_to_field: Dict[str, InputField] = {
-            field.name: field for field in self._figure.fields
+            field.id: field for field in self._shape.fields
         }
         self._field_loaders = field_loaders
 
     @property
     def _can_collect_extra(self) -> bool:
         return self._name_layout.extra_move is not None
 
     def _is_extra_target(self, field: InputField):
         return (
             isinstance(self._name_layout.extra_move, ExtraTargets)
             and
-            field.name in self._name_layout.extra_move.fields
+            field.id in self._name_layout.extra_move.fields
         )
 
     def _create_state(self, binder: VarBinder, ctx_namespace: ContextNamespace) -> GenState:
         return GenState(binder, ctx_namespace, self._name_to_field)
 
     def __call__(self, binder: VarBinder, ctx_namespace: ContextNamespace) -> CodeBuilder:
         for exception in [
@@ -153,26 +156,26 @@
 
         ctx_namespace.add("append_path", append_path)
         ctx_namespace.add("extend_path", extend_path)
 
         crown_builder = CodeBuilder()
         state = self._create_state(binder, ctx_namespace)
 
-        for field_name, loader in self._field_loaders.items():
-            state.ctx_namespace.add(state.field_loader(field_name), loader)
+        for field_id, loader in self._field_loaders.items():
+            state.ctx_namespace.add(state.field_loader(field_id), loader)
 
         if not self._gen_root_crown_dispatch(crown_builder, state, self._name_layout.crown):
             raise TypeError
 
         builder = CodeBuilder()
         self._gen_header(builder, state)
 
         has_opt_fields = any(
             fld.is_optional and not self._is_extra_target(fld)
-            for fld in self._figure.fields
+            for fld in self._shape.fields
         )
 
         if has_opt_fields:
             builder += f"{binder.opt_fields} = {{}}"
 
         builder.extend(crown_builder)
 
@@ -184,17 +187,17 @@
         if state.path2suffix:
             builder += "# suffix to path"
             for path, suffix in state.path2suffix.items():
                 builder += f"# {suffix} -> {list(path)}"
 
             builder.empty_line()
 
-        if state.field_name2path:
+        if state.field_id2path:
             builder += "# field to path"
-            for f_name, path in state.field_name2path.items():
+            for f_name, path in state.field_id2path.items():
                 builder += f"# {f_name} -> {list(path)}"
 
             builder.empty_line()
 
     def _gen_root_crown_dispatch(self, builder: CodeBuilder, state: GenState, crown: InpCrown):
         """Returns True if code is generated"""
         if isinstance(crown, InpDictCrown):
@@ -352,71 +355,69 @@
             self._gen_crown_dispatch(builder, state, value, key)
 
         if self._can_collect_extra:
             self._add_self_extra_to_parent_extra(builder, state)
 
     def _gen_field_crown(self, builder: CodeBuilder, state: GenState, crown: InpFieldCrown):
         field = state.get_field(crown)
-
-        if field.is_required:
-            field_left_value = state.binder.field(field)
+        if field.is_optional:
+            last_path_el = state.path[-1]
+            data = state.with_parent_path().get_data_var_name()
+            with builder(f'if {last_path_el!r} in {data}:'):
+                self._gen_field_assigment(
+                    builder=builder,
+                    assign_to=f"{state.binder.opt_fields}[{field.id!r}]",
+                    field_id=field.id,
+                    data_for_loader=f"{data}[{last_path_el!r}]",
+                    state=state,
+                )
         else:
-            field_left_value = f"{state.binder.opt_fields}[{field.name!r}]"
-
-        self._gen_var_assigment_from_data(
-            builder,
-            state,
-            assign_to=state.raw_field(field),
-            ignore_lookup_error=field.is_optional,
-        )
-        data_for_loader = state.raw_field(field)
-
-        if field.is_required:
+            self._gen_var_assigment_from_data(
+                builder=builder,
+                state=state,
+                assign_to=state.raw_field(field),
+                ignore_lookup_error=field.is_optional,
+            )
             builder.empty_line()
             self._gen_field_assigment(
-                builder,
-                field_left_value,
-                field.name,
-                data_for_loader,
-                state,
+                builder=builder,
+                assign_to=state.binder.field(field),
+                field_id=field.id,
+                data_for_loader=state.raw_field(field),
+                state=state,
             )
-        else:
-            with builder("else:"):
-                self._gen_field_assigment(
-                    builder,
-                    field_left_value,
-                    field.name,
-                    data_for_loader,
-                    state,
-                )
-
         builder.empty_line()
 
     def _gen_field_assigment(
         self,
         builder: CodeBuilder,
-        field_left_value: str,
-        field_name: str,
+        assign_to: str,
+        field_id: str,
         data_for_loader: str,
         state: GenState,
     ):
-        field_loader = state.field_loader(field_name)
+        field_loader = state.field_loader(field_id)
+
+        if self._field_loaders[field_id] == as_is_stub:
+            processing_expr = data_for_loader
+        else:
+            processing_expr = f'{field_loader}({data_for_loader})'
 
         if self._debug_path and state.path:
             builder(
                 f"""
                 try:
-                    {field_left_value} = {field_loader}({data_for_loader})
+                    {assign_to} = {processing_expr}
                 except Exception as e:
                     raise {self._wrap_error('e', state.path)}
                 """
             )
         else:
             builder(
-                f"{field_left_value} = {field_loader}({data_for_loader})"
+                f"{assign_to} = {processing_expr}"
             )
 
     def _gen_extra_targets_assigment(self, builder: CodeBuilder, state: GenState):
         # Saturate extra targets with data.
         # If extra data is not collected, loader of required field will get empty dict
         extra_move = self._name_layout.extra_move
 
@@ -424,29 +425,28 @@
             return
 
         if self._name_layout.crown.extra_policy == ExtraCollect():
             for target in extra_move.fields:
                 field = self._name_to_field[target]
 
                 self._gen_field_assigment(
-                    builder,
-                    field_left_value=state.binder.field(field),
-                    field_name=target,
+                    builder=builder,
+                    assign_to=state.binder.field(field),
+                    field_id=target,
                     data_for_loader=state.get_extra_var_name(),
                     state=state,
                 )
         else:
             for target in extra_move.fields:
                 field = self._name_to_field[target]
-
                 if field.is_required:
                     self._gen_field_assigment(
-                        builder,
-                        field_left_value=state.binder.field(field),
-                        field_name=target,
+                        builder=builder,
+                        assign_to=state.binder.field(field),
+                        field_id=target,
                         data_for_loader="{}",
                         state=state,
                     )
 
         builder.empty_line()
 
     def _gen_none_crown(self, builder: CodeBuilder, state: GenState, crown: InpNoneCrown):
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/loader_provider.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/model/loader_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,187 +1,176 @@
 from typing import Mapping, Protocol, Tuple
 
-from ...code_tools import BasicClosureCompiler, BuiltinContextNamespace
+from ...code_tools.compiler import BasicClosureCompiler
+from ...code_tools.context_namespace import BuiltinContextNamespace
 from ...common import Loader
-from ..essential import CannotProvide, Mediator
-from ..model.definitions import CodeGenerator, InputFigure, InputFigureRequest, VarBinder
+from ...essential import CannotProvide, Mediator
+from ...model_tools.definitions import InputShape
+from ..model.definitions import CodeGenerator, InputShapeRequest, VarBinder
 from ..model.input_extraction_gen import BuiltinInputExtractionGen
 from ..provider_template import LoaderProvider
-from ..request_cls import DebugPathRequest, FieldLoc, InputFieldLoc, LoaderRequest, LocMap, TypeHintLoc
+from ..request_cls import DebugPathRequest, LoaderRequest, TypeHintLoc
 from .basic_gen import (
     CodeGenHookRequest,
     NameSanitizer,
     compile_closure_with_globals_capturing,
     get_extra_targets_at_crown,
     get_optional_fields_at_list_crown,
     get_skipped_fields,
     get_wild_extra_targets,
     has_collect_policy,
-    strip_figure_fields,
+    strip_shape_fields,
     stub_code_gen_hook,
 )
 from .crown_definitions import InpExtraMove, InputNameLayout, InputNameLayoutRequest
-from .figure_provider import provide_generic_resolved_figure
+from .fields import input_field_to_loc_map
 from .input_creation_gen import BuiltinInputCreationGen
+from .shape_provider import provide_generic_resolved_shape
 
 
 class InputExtractionMaker(Protocol):
     def __call__(
         self,
         mediator: Mediator,
         request: LoaderRequest,
-    ) -> Tuple[CodeGenerator, InputFigure, InpExtraMove]:
+    ) -> Tuple[CodeGenerator, InputShape, InpExtraMove]:
         ...
 
 
 class InputCreationMaker(Protocol):
     def __call__(
         self,
         mediator: Mediator,
         request: LoaderRequest,
-        figure: InputFigure,
+        shape: InputShape,
         extra_move: InpExtraMove,
     ) -> CodeGenerator:
         ...
 
 
 class BuiltinInputExtractionMaker(InputExtractionMaker):
-    def _fetch_figure(self, mediator: Mediator, request: LoaderRequest) -> InputFigure:
-        return provide_generic_resolved_figure(mediator, InputFigureRequest(loc_map=request.loc_map))
+    def _fetch_shape(self, mediator: Mediator, request: LoaderRequest) -> InputShape:
+        return provide_generic_resolved_shape(mediator, InputShapeRequest(loc_map=request.loc_map))
 
-    def __call__(self, mediator: Mediator, request: LoaderRequest) -> Tuple[CodeGenerator, InputFigure, InpExtraMove]:
-        figure = self._fetch_figure(mediator, request)
+    def __call__(self, mediator: Mediator, request: LoaderRequest) -> Tuple[CodeGenerator, InputShape, InpExtraMove]:
+        shape = self._fetch_shape(mediator, request)
 
         name_layout: InputNameLayout = mediator.provide(
             InputNameLayoutRequest(
                 loc_map=request.loc_map,
-                figure=figure,
+                shape=shape,
             )
         )
 
-        processed_figure = self._process_figure(figure, name_layout)
-        self._validate_params(processed_figure, name_layout)
+        processed_shape = self._process_shape(shape, name_layout)
+        self._validate_params(processed_shape, name_layout)
 
         field_loaders = {
-            field.name: mediator.provide(
+            field.id: mediator.provide(
                 LoaderRequest(
-                    loc_map=LocMap(
-                        TypeHintLoc(
-                            type=field.type,
-                        ),
-                        FieldLoc(
-                            name=field.name,
-                            default=field.default,
-                            metadata=field.metadata,
-                        ),
-                        InputFieldLoc(
-                            is_required=field.is_required,
-                            param_kind=field.param_kind,
-                            param_name=field.param_name,
-                        )
-                    ),
+                    loc_map=input_field_to_loc_map(field),
                 )
             )
-            for field in processed_figure.fields
+            for field in processed_shape.fields
         }
         debug_path = mediator.provide(DebugPathRequest(loc_map=request.loc_map))
-        extraction_gen = self._create_extraction_gen(debug_path, figure, name_layout, field_loaders)
+        extraction_gen = self._create_extraction_gen(debug_path, shape, name_layout, field_loaders)
 
-        return extraction_gen, figure, name_layout.extra_move
+        return extraction_gen, shape, name_layout.extra_move
 
-    def _process_figure(self, figure: InputFigure, name_layout: InputNameLayout) -> InputFigure:
-        wild_extra_targets = get_wild_extra_targets(figure, name_layout.extra_move)
+    def _process_shape(self, shape: InputShape, name_layout: InputNameLayout) -> InputShape:
+        wild_extra_targets = get_wild_extra_targets(shape, name_layout.extra_move)
         if wild_extra_targets:
             raise ValueError(
                 f"ExtraTargets {wild_extra_targets} are attached to non-existing fields"
             )
 
-        skipped_fields = get_skipped_fields(figure, name_layout)
+        skipped_fields = get_skipped_fields(shape, name_layout)
 
         skipped_required_fields = [
-            field.name
-            for field in figure.fields
-            if field.is_required and field.name in skipped_fields
+            field.id
+            for field in shape.fields
+            if field.is_required and field.id in skipped_fields
         ]
         if skipped_required_fields:
             raise ValueError(
                 f"Required fields {skipped_required_fields} are skipped"
             )
 
-        return strip_figure_fields(figure, skipped_fields)
+        return strip_shape_fields(shape, skipped_fields)
 
-    def _validate_params(self, processed_figure: InputFigure, name_layout: InputNameLayout) -> None:
+    def _validate_params(self, processed_shape: InputShape, name_layout: InputNameLayout) -> None:
         if name_layout.extra_move is None and has_collect_policy(name_layout.crown):
             raise ValueError(
                 "Cannot create loader that collect extra data"
-                " if InputFigure does not take extra data",
+                " if InputShape does not take extra data",
             )
 
         extra_targets_at_crown = get_extra_targets_at_crown(name_layout)
         if extra_targets_at_crown:
             raise ValueError(
                 f"Extra targets {extra_targets_at_crown} are found at crown"
             )
 
         optional_fields_at_list_crown = get_optional_fields_at_list_crown(
-            {field.name: field for field in processed_figure.fields},
+            {field.id: field for field in processed_shape.fields},
             name_layout.crown,
         )
         if optional_fields_at_list_crown:
             raise ValueError(
                 f"Optional fields {optional_fields_at_list_crown} are found at list crown"
             )
 
     def _create_extraction_gen(
         self,
         debug_path: bool,
-        figure: InputFigure,
+        shape: InputShape,
         name_layout: InputNameLayout,
         field_loaders: Mapping[str, Loader],
     ) -> CodeGenerator:
         return BuiltinInputExtractionGen(
-            figure=figure,
+            shape=shape,
             name_layout=name_layout,
             debug_path=debug_path,
             field_loaders=field_loaders,
         )
 
 
 class InlinedInputExtractionMaker(BuiltinInputExtractionMaker):
-    def __init__(self, figure: InputFigure):
-        self._figure = figure
+    def __init__(self, shape: InputShape):
+        self._shape = shape
         super().__init__()
 
-    def _fetch_figure(self, mediator: Mediator, request: LoaderRequest) -> InputFigure:
-        return self._figure
+    def _fetch_shape(self, mediator: Mediator, request: LoaderRequest) -> InputShape:
+        return self._shape
 
 
 def make_input_creation(
     mediator: Mediator,
     request: LoaderRequest,
-    figure: InputFigure,
+    shape: InputShape,
     extra_move: InpExtraMove,
 ) -> CodeGenerator:
-    return BuiltinInputCreationGen(figure=figure, extra_move=extra_move)
+    return BuiltinInputCreationGen(shape=shape, extra_move=extra_move)
 
 
 class ModelLoaderProvider(LoaderProvider):
     def __init__(
         self,
         name_sanitizer: NameSanitizer,
         extraction_maker: InputExtractionMaker,
         creation_maker: InputCreationMaker,
     ):
         self._name_sanitizer = name_sanitizer
         self._extraction_maker = extraction_maker
         self._creation_maker = creation_maker
 
     def _provide_loader(self, mediator: Mediator, request: LoaderRequest) -> Loader:
-        extraction_gen, figure, extra_move = self._extraction_maker(mediator, request)
-        creation_gen = self._creation_maker(mediator, request, figure, extra_move)
+        extraction_gen, shape, extra_move = self._extraction_maker(mediator, request)
+        creation_gen = self._creation_maker(mediator, request, shape, extra_move)
 
         try:
             code_gen_hook = mediator.provide(CodeGenHookRequest())
         except CannotProvide:
             code_gen_hook = stub_code_gen_hook
 
         binder = self._get_binder()
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/output_creation_gen.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/model/output_creation_gen.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import contextlib
 from string import Template
 from typing import Dict, NamedTuple, Optional
 
-from ...code_tools import CodeBuilder, ContextNamespace, get_literal_expr, get_literal_from_factory
-from ...model_tools import DefaultFactory, DefaultValue, OutputField
+from ...code_tools.code_builder import CodeBuilder
+from ...code_tools.context_namespace import ContextNamespace
+from ...code_tools.utils import get_literal_expr, get_literal_from_factory, is_singleton
+from ...model_tools.definitions import DefaultFactory, DefaultValue, OutputField
 from .crown_definitions import (
     CrownPathElem,
     OutCrown,
     OutDictCrown,
     OutFieldCrown,
     OutListCrown,
     OutNoneCrown,
     OutputNameLayout,
     Sieve,
 )
-from .definitions import CodeGenerator, OutputFigure, VarBinder
+from .definitions import CodeGenerator, OutputShape, VarBinder
 from .input_extraction_gen import CrownPath
+from .special_cases_optimization import get_default_clause
 
 
 class GenState:
     def __init__(self, binder: VarBinder, ctx_namespace: ContextNamespace, name_to_field: Dict[str, OutputField]):
         self.binder = binder
         self.ctx_namespace = ctx_namespace
         self._name_to_field = name_to_field
 
-        self.field_name2path: Dict[str, CrownPath] = {}
+        self.field_id2path: Dict[str, CrownPath] = {}
         self.path2suffix: Dict[CrownPath, str] = {}
 
         self._last_path_idx = 0
         self._path: CrownPath = ()
         self._parent_path: Optional[CrownPath] = None
 
     def _get_path_idx(self, path: CrownPath) -> str:
@@ -73,39 +76,46 @@
     def sieve(self, key: CrownPathElem) -> str:
         path = self._path + (key,)
         if not path:
             return "sieve"
 
         return 'sieve_' + self._get_path_idx(path)
 
+    def default_clause(self, key: CrownPathElem) -> str:
+        path = self._path + (key,)
+        if not path:
+            return "dfl"
+
+        return 'dfl_' + self._get_path_idx(path)
+
 
 class ElementExpr(NamedTuple):
     expr: str
     can_inline: bool
 
 
 class BuiltinOutputCreationGen(CodeGenerator):
-    def __init__(self, figure: OutputFigure, name_layout: OutputNameLayout, debug_path: bool):
-        self._figure = figure
+    def __init__(self, shape: OutputShape, name_layout: OutputNameLayout, debug_path: bool):
+        self._shape = shape
         self._name_layout = name_layout
         self._debug_path = debug_path
 
-        self._name_to_field: Dict[str, OutputField] = {field.name: field for field in self._figure.fields}
+        self._name_to_field: Dict[str, OutputField] = {field.id: field for field in self._shape.fields}
 
     def _gen_header(self, builder: CodeBuilder, state: GenState):
         if state.path2suffix:
             builder += "# suffix to path"
             for path, suffix in state.path2suffix.items():
                 builder += f"# {suffix} -> {list(path)}"
 
             builder.empty_line()
 
-        if state.field_name2path:
+        if state.field_id2path:
             builder += "# field to path"
-            for f_name, path in state.field_name2path.items():
+            for f_name, path in state.field_id2path.items():
                 builder += f"# {f_name} -> {list(path)}"
 
             builder.empty_line()
 
     def _create_state(self, binder: VarBinder, ctx_namespace: ContextNamespace) -> GenState:
         return GenState(binder, ctx_namespace, self._name_to_field)
 
@@ -175,15 +185,15 @@
 
     def _get_element_expr(self, state: GenState, key: CrownPathElem, crown: OutCrown) -> ElementExpr:
         with state.add_key(key):
             if isinstance(crown, OutNoneCrown):
                 return self._get_element_expr_for_none_crown(state, key, crown)
 
             if isinstance(crown, OutFieldCrown):
-                field = self._name_to_field[crown.name]
+                field = self._name_to_field[crown.id]
                 if field.is_required:
                     field_expr = state.binder.field(field)
                 else:
                     raise ValueError("Can not generate ElementExpr for optional field")
                 return ElementExpr(field_expr, can_inline=True)
 
             if isinstance(crown, (OutDictCrown, OutListCrown)):
@@ -191,15 +201,15 @@
 
             raise TypeError
 
     def _is_required_crown(self, crown: OutCrown) -> bool:
         if not isinstance(crown, OutFieldCrown):
             return True
 
-        return self._name_to_field[crown.name].is_required
+        return self._name_to_field[crown.id].is_required
 
     def _gen_dict_crown(self, builder: CodeBuilder, state: GenState, crown: OutDictCrown):
         for key, value in crown.map.items():
             self._gen_crown_dispatch(builder, state, value, key)
 
         required_keys = [
             key for key, sub_crown in crown.map.items()
@@ -230,18 +240,18 @@
         self,
         builder: CodeBuilder,
         state: GenState,
         crown: OutDictCrown,
         key: str,
         sub_crown: OutCrown
     ):
-        if isinstance(sub_crown, OutFieldCrown) and self._name_to_field[sub_crown.name].is_optional:
+        if isinstance(sub_crown, OutFieldCrown) and self._name_to_field[sub_crown.id].is_optional:
             builder += f"""
                 try:
-                    value = {state.binder.opt_fields}[{sub_crown.name!r}]
+                    value = {state.binder.opt_fields}[{sub_crown.id!r}]
                 except KeyError:
                     pass
                 else:
             """
             with builder:
                 if key in crown.sieves:
                     self._gen_dict_sieved_append(
@@ -262,39 +272,63 @@
         builder: CodeBuilder,
         state: GenState,
         sieve: Sieve,
         key: str,
         element_expr: ElementExpr,
     ):
         self_var = state.crown_var_self()
-        sieve_var = state.sieve(key)
-        state.ctx_namespace.add(sieve_var, sieve)
-
+        condition = self._gen_sieve_condition(state, sieve, key, element_expr.expr)
         if element_expr.can_inline:
             builder += f"""
-                if {sieve_var}({element_expr.expr}):
+                if {condition}:
                     {self_var}[{key!r}] = {element_expr.expr}
             """
         else:
             builder += f"""
                 value = {element_expr.expr}
-                if {sieve_var}(value):
+                if {condition}:
                     {self_var}[{key!r}] = value
             """
-
         builder.empty_line()
 
+    def _gen_sieve_condition(self, state: GenState, sieve: Sieve, key: str, input_expr: str) -> str:
+        default_clause = get_default_clause(sieve)
+        if default_clause is None:
+            sieve_var = state.sieve(key)
+            state.ctx_namespace.add(sieve_var, sieve)
+            return f'{sieve_var}({input_expr})'
+
+        if isinstance(default_clause, DefaultValue):
+            literal_expr = get_literal_expr(default_clause.value)
+            if literal_expr is not None:
+                if is_singleton(default_clause.value):
+                    return f"{input_expr} is not {literal_expr}"
+                return f"{input_expr} != {literal_expr}"
+            default_clause_var = state.default_clause(key)
+            state.ctx_namespace.add(default_clause_var, default_clause.value)
+            return f"{input_expr} != {default_clause_var}"
+
+        if isinstance(default_clause, DefaultFactory):
+            literal_expr = get_literal_from_factory(default_clause.factory)
+            if literal_expr is not None:
+                return f"{input_expr} != {literal_expr}"
+            default_clause_var = state.default_clause(key)
+            state.ctx_namespace.add(default_clause_var, default_clause.factory)
+            return f"{input_expr} != {default_clause_var}()"
+
+        raise TypeError
+
     def _gen_list_crown(self, builder: CodeBuilder, state: GenState, crown: OutListCrown):
         for i, sub_crown in enumerate(crown.map):
             self._gen_crown_dispatch(builder, state, sub_crown, i)
 
         with builder(f"{state.crown_var_self()} = ["):
             for i, sub_crown in enumerate(crown.map):
                 builder += self._get_element_expr(state, i, sub_crown).expr + ","
 
         builder += "]"
 
     def _gen_field_crown(self, builder: CodeBuilder, state: GenState, crown: OutFieldCrown):
-        state.field_name2path[crown.name] = state.path
+        state.field_id2path[crown.id] = state.path
 
     def _gen_none_crown(self, builder: CodeBuilder, state: GenState, crown: OutNoneCrown):
         pass
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/output_extraction_gen.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/model/output_extraction_gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 from string import Template
 from typing import Dict, Mapping
 
-from ...code_tools import CodeBuilder, ContextNamespace, get_literal_expr
+from ...code_tools.code_builder import CodeBuilder
+from ...code_tools.context_namespace import ContextNamespace
+from ...code_tools.utils import get_literal_expr
 from ...common import Dumper
-from ...model_tools import AttrAccessor, ItemAccessor, OutputField, OutputFigure
+from ...model_tools.definitions import AttrAccessor, ItemAccessor, OutputField, OutputShape
 from ...struct_path import append_path, extend_path
 from .crown_definitions import ExtraExtract, ExtraTargets, OutExtraMove
 from .definitions import CodeGenerator, VarBinder
+from .special_cases_optimization import as_is_stub
 
 
 class BuiltinOutputExtractionGen(CodeGenerator):
     def __init__(
         self,
-        figure: OutputFigure,
+        shape: OutputShape,
         extra_move: OutExtraMove,
         debug_path: bool,
         fields_dumpers: Mapping[str, Dumper],
     ):
-        self._figure = figure
+        self._shape = shape
         self._extra_move = extra_move
         self._debug_path = debug_path
         self._fields_dumpers = fields_dumpers
         self._extra_targets = (
             self._extra_move.fields
             if isinstance(self._extra_move, ExtraTargets)
             else ()
         )
 
     def __call__(self, binder: VarBinder, ctx_namespace: ContextNamespace) -> CodeBuilder:
         builder = CodeBuilder()
 
         ctx_namespace.add("append_path", append_path)
         ctx_namespace.add("extend_path", extend_path)
-        name_to_fields = {field.name: field for field in self._figure.fields}
+        name_to_fields = {field.id: field for field in self._shape.fields}
 
-        for field_name, dumper in self._fields_dumpers.items():
-            ctx_namespace.add(self._dumper(name_to_fields[field_name]), dumper)
+        for field_id, dumper in self._fields_dumpers.items():
+            ctx_namespace.add(self._dumper(name_to_fields[field_id]), dumper)
 
-        if any(field.is_optional for field in self._figure.fields):
+        if any(field.is_optional for field in self._shape.fields):
             builder(f"{binder.opt_fields} = {{}}")
             builder.empty_line()
 
-        for field in self._figure.fields:
+        for field in self._shape.fields:
             if not self._is_extra_target(field):
                 self._gen_field_extraction(
                     builder, binder, ctx_namespace, field,
                     on_access_error="pass",
                     on_access_ok_req=f"{binder.field(field)} = $expr",
-                    on_access_ok_opt=f"{binder.opt_fields}[{field.name!r}] = $expr",
+                    on_access_ok_opt=f"{binder.opt_fields}[{field.id!r}] = $expr",
                 )
 
         self._gen_extra_extraction(
             builder, binder, ctx_namespace, name_to_fields,
         )
         return builder
 
     def _is_extra_target(self, field: OutputField) -> bool:
-        return field.name in self._extra_targets
+        return field.id in self._extra_targets
 
     def _dumper(self, field: OutputField) -> str:
-        return f"dumper_{field.name}"
+        return f"dumper_{field.id}"
 
     def _raw_field(self, field: OutputField) -> str:
-        return f"r_{field.name}"
+        return f"r_{field.id}"
 
     def _accessor_getter(self, field: OutputField) -> str:
-        return f"accessor_getter_{field.name}"
+        return f"accessor_getter_{field.id}"
 
     def _gen_access_expr(self, binder: VarBinder, ctx_namespace: ContextNamespace, field: OutputField) -> str:
         accessor = field.accessor
         if isinstance(accessor, AttrAccessor):
             if accessor.attr_name.isidentifier():
                 return f"{binder.data}.{accessor.attr_name}"
             return f"getattr({binder.data}, {accessor.attr_name!r})"
@@ -77,15 +80,15 @@
             return f"{binder.data}[{accessor.item_name!r}]"
 
         accessor_getter = self._accessor_getter(field)
         ctx_namespace.add(accessor_getter, field.accessor.getter)
         return f"{accessor_getter}({binder.data})"
 
     def _get_path_element_var_name(self, field: OutputField) -> str:
-        return f"path_element_{field.name}"
+        return f"path_element_{field.id}"
 
     def _gen_path_element_expr(self, ctx_namespace: ContextNamespace, field: OutputField) -> str:
         path_element = field.accessor.path_element
         literal_expr = get_literal_expr(path_element)
         if literal_expr is not None:
             return literal_expr
 
@@ -101,16 +104,19 @@
         field: OutputField,
         *,
         on_access_ok: str,
     ):
         raw_access_expr = self._gen_access_expr(binder, ctx_namespace, field)
         path_element_expr = self._gen_path_element_expr(ctx_namespace, field)
 
-        dumper = self._dumper(field)
-        on_access_ok_stmt = Template(on_access_ok).substitute(expr=f"{dumper}({raw_access_expr})")
+        if self._fields_dumpers[field.id] == as_is_stub:
+            on_access_ok_stmt = Template(on_access_ok).substitute(expr=raw_access_expr)
+        else:
+            dumper = self._dumper(field)
+            on_access_ok_stmt = Template(on_access_ok).substitute(expr=f"{dumper}({raw_access_expr})")
 
         if self._debug_path:
             builder += f"""
                 try:
                     {on_access_ok_stmt}
                 except Exception as e:
                     append_path(e, {path_element_expr})
@@ -118,35 +124,40 @@
             """
         else:
             builder += on_access_ok_stmt
 
         builder.empty_line()
 
     def _get_access_error_var_name(self, field: OutputField) -> str:
-        return f"access_error_{field.name}"
+        return f"access_error_{field.id}"
 
     def _gen_optional_field_extraction(
         self,
         builder: CodeBuilder,
         binder: VarBinder,
         ctx_namespace: ContextNamespace,
         field: OutputField,
         *,
         on_access_error: str,
         on_access_ok: str,
     ):
         raw_access_expr = self._gen_access_expr(binder, ctx_namespace, field)
         path_element_expr = self._gen_path_element_expr(ctx_namespace, field)
 
-        dumper = self._dumper(field)
         raw_field = self._raw_field(field)
 
-        on_access_ok_stmt = Template(on_access_ok).substitute(
-            expr=f"{dumper}({raw_field})"
-        )
+        if self._fields_dumpers[field.id] == as_is_stub:
+            on_access_ok_stmt = Template(on_access_ok).substitute(
+                expr=raw_field,
+            )
+        else:
+            dumper = self._dumper(field)
+            on_access_ok_stmt = Template(on_access_ok).substitute(
+                expr=f"{dumper}({raw_field})",
+            )
 
         access_error = field.accessor.access_error
         access_error_var = get_literal_expr(access_error)
         if access_error_var is None:
             access_error_var = self._get_access_error_var_name(field)
             ctx_namespace.add(access_error_var, access_error)
 
@@ -229,35 +240,35 @@
                 builder, binder, ctx_namespace, field,
                 on_access_error=f"{binder.extra} = {{}}",
                 on_access_ok_req=f"{binder.extra} = $expr",
                 on_access_ok_opt=f"{binder.extra} = $expr",
             )
 
         elif all(field.is_required for field in name_to_fields.values()):
-            for field_name in self._extra_targets:
-                field = name_to_fields[field_name]
+            for field_id in self._extra_targets:
+                field = name_to_fields[field_id]
 
                 self._gen_required_field_extraction(
                     builder, binder, ctx_namespace, field,
                     on_access_ok=f"{binder.field(field)} = $expr",
                 )
 
             builder += f'{binder.extra} = {{'
             builder <<= ", ".join(
-                "**" + binder.field(name_to_fields[field_name])
-                for field_name in self._extra_targets
+                "**" + binder.field(name_to_fields[field_id])
+                for field_id in self._extra_targets
             )
             builder <<= '}'
         else:
             extra_stack = self._get_extra_stack_name()
 
             builder += f"{extra_stack} = []"
 
-            for field_name in self._extra_targets:
-                field = name_to_fields[field_name]
+            for field_id in self._extra_targets:
+                field = name_to_fields[field_id]
 
                 self._gen_field_extraction(
                     builder, binder, ctx_namespace, field,
                     on_access_ok_req=f"{extra_stack}.append($expr)",
                     on_access_ok_opt=f"{extra_stack}.append($expr)",
                     on_access_error="pass",
                 )
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/request_filtering.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/model/request_filtering.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from ..essential import CannotProvide, Request
+from ...essential import CannotProvide, Request
 from ..request_cls import LocatedRequest
 from ..request_filtering import DirectMediator, RequestChecker
-from .definitions import InputFigureRequest, OutputFigureRequest
+from .definitions import InputShapeRequest, OutputShapeRequest
 
 
 class AnyModelRC(RequestChecker):
     def check_request(self, mediator: DirectMediator, request: Request) -> None:
         if not isinstance(request, LocatedRequest):
             raise CannotProvide
 
         try:
-            mediator.provide(InputFigureRequest(loc_map=request.loc_map))
+            mediator.provide(InputShapeRequest(loc_map=request.loc_map))
         except CannotProvide:
-            mediator.provide(OutputFigureRequest(loc_map=request.loc_map))
+            mediator.provide(OutputShapeRequest(loc_map=request.loc_map))
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/base.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/name_layout/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from abc import ABC, abstractmethod
 from typing import Mapping, Sequence, TypeVar, Union
 
 from adaptix._internal.provider.model.crown_definitions import (
+    DictExtraPolicy,
     Extractor,
     ExtraForbid,
     ExtraKwargs,
+    ExtraSkip,
     InpExtraMove,
     InputNameLayoutRequest,
     LeafInpCrown,
     LeafOutCrown,
     OutExtraMove,
     OutputNameLayoutRequest,
     Saturator,
+    Sieve,
 )
 
 from ...common import VarTuple
-from ..essential import Mediator
-from ..model import DictExtraPolicy, ExtraSkip, Sieve
+from ...essential import Mediator
 
 T = TypeVar('T')
 
 
 ExtraIn = Union[ExtraSkip, str, Sequence[str], ExtraForbid, ExtraKwargs, Saturator]
 ExtraOut = Union[ExtraSkip, str, Sequence[str], Extractor]
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/component.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/name_layout/component.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 from collections import defaultdict
 from dataclasses import dataclass
-from typing import (
-    Callable,
-    DefaultDict,
-    Dict,
-    Iterable,
-    List,
-    Mapping,
-    MutableMapping,
-    Optional,
-    Pattern,
-    Sequence,
-    Set,
-    Tuple,
-    TypeVar,
-    Union,
-)
+from typing import Callable, DefaultDict, Dict, Iterable, List, Mapping, Optional, Sequence, Set, Tuple, TypeVar, Union
 
-from ...common import EllipsisType, VarTuple
-from ...model_tools import BaseField, DefaultFactory, DefaultValue, InputField, NoDefault, OutputField
+from ...common import VarTuple
+from ...essential import CannotProvide, Mediator, Provider
+from ...model_tools.definitions import BaseField, DefaultFactory, DefaultValue, InputField, NoDefault, OutputField
+from ...retort.operating_retort import OperatingRetort
 from ...utils import Omittable
-from ..essential import Mediator
-from ..model import Sieve
 from ..model.crown_definitions import (
+    BaseFieldCrown,
+    BaseNameLayoutRequest,
     DictExtraPolicy,
     ExtraCollect,
     ExtraExtract,
     ExtraForbid,
     ExtraKwargs,
     ExtraSaturate,
     ExtraSkip,
@@ -38,137 +25,148 @@
     LeafBaseCrown,
     LeafInpCrown,
     LeafOutCrown,
     OutExtraMove,
     OutFieldCrown,
     OutNoneCrown,
     OutputNameLayoutRequest,
+    Sieve,
 )
+from ..model.fields import field_to_loc_map
+from ..model.special_cases_optimization import with_default_clause
 from ..name_style import NameStyle, convert_snake_style
 from ..overlay_schema import Overlay, Schema, provide_schema
 from ..request_cls import FieldLoc, LocatedRequest, TypeHintLoc
+from ..request_filtering import ExtraStackMediator, RequestChecker
 from .base import ExtraIn, ExtraMoveMaker, ExtraOut, ExtraPoliciesMaker, Key, Path, PathsTo, SievesMaker, StructureMaker
-
-RawKey = Union[Key, EllipsisType]
-RawPath = VarTuple[RawKey]
-NameMapStack = VarTuple[Tuple[Pattern, RawPath]]
+from .name_mapping import NameMappingFilterRequest, NameMappingRequest
 
 
 @dataclass
 class StructureSchema(Schema):
-    skip: Iterable[str]
-    only_mapped: bool
-    only: Optional[Iterable[str]]
+    skip: RequestChecker
+    only: RequestChecker
 
-    map: NameMapStack
+    map: VarTuple[Provider]
     trim_trailing_underscore: bool
     name_style: Optional[NameStyle]
 
 
 @dataclass
 class StructureOverlay(Overlay[StructureSchema]):
-    skip: Omittable[Iterable[str]]
-    only_mapped: Omittable[bool]
-    only: Omittable[Optional[Iterable[str]]]
+    skip: Omittable[RequestChecker]
+    only: Omittable[RequestChecker]
 
-    map: Omittable[NameMapStack]
+    map: Omittable[VarTuple[Provider]]
     trim_trailing_underscore: Omittable[bool]
     name_style: Omittable[Optional[NameStyle]]
 
-    def _merge_map(self, old: NameMapStack, new: NameMapStack) -> NameMapStack:
+    def _merge_map(self, old: VarTuple[Provider], new: VarTuple[Provider]) -> VarTuple[Provider]:
         return new + old
 
 
-F = TypeVar('F', bound=BaseField)
 AnyField = Union[InputField, OutputField]
 LeafCr = TypeVar('LeafCr', bound=LeafBaseCrown)
+FieldCr = TypeVar('FieldCr', bound=BaseFieldCrown)
+F = TypeVar('F', bound=BaseField)
+FieldAndPath = Tuple[F, Optional[Path]]
 
 
 def location_to_string(request: LocatedRequest) -> str:
     loc_map = request.loc_map
     if loc_map.has(TypeHintLoc, FieldLoc):
         return f' at type {loc_map[TypeHintLoc].type} that situated at field {request.loc_map[FieldLoc].name!r}'
     if loc_map.has(TypeHintLoc):
         return f' at type {loc_map[TypeHintLoc].type}'
     if loc_map.has(FieldLoc):
         return f' situated at field {request.loc_map[FieldLoc].name!r}'
     return ''
 
 
-class BuiltinStructureMaker(StructureMaker):
-    def _ensure_field_path(self, schema: StructureSchema, field: BaseField) -> Tuple[Path, bool]:
-        name = field.name
-        for pattern, raw_path in schema.map:
-            if pattern.fullmatch(field.name):
-                return tuple(
-                    field.name if isinstance(el, EllipsisType) else el
-                    for el in raw_path
-                ), True
+def apply_rc(mediator: Mediator, request_checker: RequestChecker, field: BaseField) -> bool:
+    request = NameMappingFilterRequest(loc_map=field_to_loc_map(field))
+    try:
+        request_checker.check_request(
+            ExtraStackMediator(mediator, [request]),
+            request,
+        )
+    except CannotProvide:
+        return False
+    return True
+
 
+class BuiltinStructureMaker(StructureMaker):
+    def _make_non_mapped_path(self, schema: StructureSchema, field: BaseField) -> Optional[Path]:
+        name = field.id
         if schema.trim_trailing_underscore and name.endswith('_') and not name.endswith('__'):
             name = name.rstrip('_')
         if schema.name_style is not None:
             name = convert_snake_style(name, schema.name_style)
-        return (name, ), False
+        return (name, )
 
-    def _can_include_field(self, schema: StructureSchema, field: BaseField, is_mapped: bool) -> bool:
-        if schema.only is None and not schema.only_mapped:
-            return True
-        return (
-            (schema.only is not None and field.name in schema.only)
-            or (schema.only_mapped and is_mapped)
-        )
+    def _create_map_provider(self, schema: StructureSchema) -> Provider:
+        return OperatingRetort(recipe=schema.map)
 
-    def _fields_to_paths(
+    def _map_fields(
         self,
+        mediator: Mediator,
+        request: BaseNameLayoutRequest,
         schema: StructureSchema,
-        fields: Iterable[F],
         extra_move: Union[InpExtraMove, OutExtraMove],
-    ) -> Iterable[Tuple[F, Optional[Path]]]:
-        if isinstance(extra_move, ExtraTargets):
-            extra_targets = extra_move.fields
-        else:
-            extra_targets = ()
-
-        for field in fields:
-            if field.name in extra_targets:
+    ) -> Iterable[FieldAndPath]:
+        extra_targets = extra_move.fields if isinstance(extra_move, ExtraTargets) else ()
+        map_provider = self._create_map_provider(schema)
+        for field in request.shape.fields:
+            if field.id in extra_targets:
                 continue
 
-            if field.name in schema.skip:
-                yield field, None
-                continue
+            try:
+                path = map_provider.apply_provider(
+                    mediator,
+                    NameMappingRequest(
+                        shape=request.shape,
+                        field=field,
+                        loc_map=field_to_loc_map(field),
+                    )
+                )
+            except CannotProvide:
+                path = self._make_non_mapped_path(schema, field)
 
-            path, is_mapped = self._ensure_field_path(schema, field)
-            if self._can_include_field(schema, field, is_mapped):
+            if path is None:
+                yield field, None
+            elif (
+                not apply_rc(mediator, schema.skip, field)
+                and apply_rc(mediator, schema.only, field)
+            ):
                 yield field, path
             else:
                 yield field, None
 
     def _validate_structure(
         self,
         request: LocatedRequest,
-        fields_to_paths: Iterable[Tuple[AnyField, Optional[Path]]],
+        fields_to_paths: Iterable[FieldAndPath],
     ) -> None:
         paths_to_fields: DefaultDict[Path, List[AnyField]] = defaultdict(list)
         for field, path in fields_to_paths:
             if path is not None:
                 paths_to_fields[path].append(field)
 
         duplicates = {
-            path: [field.name for field in fields]
+            path: [field.id for field in fields]
             for path, fields in paths_to_fields.items()
             if len(fields) > 1
         }
         if duplicates:
             raise ValueError(
                 f"Paths {duplicates} pointed to several fields" + location_to_string(request)
             )
 
         optional_fields_at_list = [
-            field.name
+            field.id
             for field, path in fields_to_paths
             if path is not None and field.is_optional and isinstance(path[-1], int)
         ]
         if optional_fields_at_list:
             raise ValueError(
                 f"Optional fields {optional_fields_at_list} can not be mapped to list elements"
                 + location_to_string(request)
@@ -184,15 +182,14 @@
 
                 yielded.add(result)
                 yield result
 
     def _get_paths_to_list(self, request: LocatedRequest, paths: Iterable[Path]) -> Mapping[Path, Set[int]]:
         paths_to_lists: DefaultDict[Path, Set[int]] = defaultdict(set)
         paths_to_dicts: Set[Path] = set()
-
         for sub_path, key in self._iterate_sub_paths(paths):
             if isinstance(key, int):
                 if sub_path in paths_to_dicts:
                     raise ValueError(
                         f"Inconsistent path elements at {sub_path}" + location_to_string(request)
                     )
 
@@ -203,114 +200,112 @@
                         f"Inconsistent path elements at {sub_path}" + location_to_string(request)
                     )
 
                 paths_to_dicts.add(sub_path)
 
         return paths_to_lists
 
-    def _fill_gaps_at_list(
+    def _make_paths_to_leaves(
         self,
-        gaps_filler: Callable[[Path], LeafCr],
         request: LocatedRequest,
-        paths_to_leaves: MutableMapping[Path, LeafCr],
-    ) -> None:
+        fields_to_paths: Iterable[FieldAndPath],
+        field_crown: Callable[[str], FieldCr],
+        gaps_filler: Callable[[Path], LeafCr],
+    ) -> PathsTo[Union[FieldCr, LeafCr]]:
+        paths_to_leaves: Dict[Path, Union[FieldCr, LeafCr]] = {
+            path: field_crown(field.id)
+            for field, path in fields_to_paths
+            if path is not None
+        }
+
         paths_to_lists = self._get_paths_to_list(request, paths_to_leaves.keys())
         for path, indexes in paths_to_lists.items():
             for i in range(max(indexes)):
                 if i not in indexes:
                     complete_path = path + (i, )
                     paths_to_leaves[complete_path] = gaps_filler(complete_path)
 
+        return paths_to_leaves
+
     def _fill_input_gap(self, path: Path) -> LeafInpCrown:
         return InpNoneCrown()
 
     def _fill_output_gap(self, path: Path) -> LeafOutCrown:
         return OutNoneCrown(filler=DefaultValue(None))
 
     def make_inp_structure(
         self,
         mediator: Mediator,
         request: InputNameLayoutRequest,
         extra_move: InpExtraMove,
     ) -> PathsTo[LeafInpCrown]:
         schema = provide_schema(StructureOverlay, mediator, request.loc_map)
-        fields_to_paths = list(self._fields_to_paths(schema, request.figure.fields, extra_move))
+        fields_to_paths: List[FieldAndPath[InputField]] = list(
+            self._map_fields(mediator, request, schema, extra_move)
+        )
         skipped_required_fields = [
-            field.name
+            field.id
             for field, path in fields_to_paths
             if path is None and field.is_required
         ]
         if skipped_required_fields:
             raise ValueError(
                 f"Required fields {skipped_required_fields} are skipped" + location_to_string(request)
             )
         self._validate_structure(request, fields_to_paths)
-        paths_to_leaves: Dict[Path, LeafInpCrown] = {
-            path: InpFieldCrown(field.name)
-            for field, path in fields_to_paths
-            if path is not None
-        }
-        self._fill_gaps_at_list(self._fill_input_gap, request, paths_to_leaves)
-        return paths_to_leaves
+        return self._make_paths_to_leaves(request, fields_to_paths, InpFieldCrown, self._fill_input_gap)
 
     def make_out_structure(
         self,
         mediator: Mediator,
         request: OutputNameLayoutRequest,
         extra_move: OutExtraMove,
     ) -> PathsTo[LeafOutCrown]:
         schema = provide_schema(StructureOverlay, mediator, request.loc_map)
-        fields_to_paths = list(self._fields_to_paths(schema, request.figure.fields, extra_move))
+        fields_to_paths: List[FieldAndPath[OutputField]] = list(
+            self._map_fields(mediator, request, schema, extra_move)
+        )
         self._validate_structure(request, fields_to_paths)
-        paths_to_leaves: Dict[Path, LeafOutCrown] = {
-            path: OutFieldCrown(field.name)
-            for field, path in fields_to_paths
-            if path is not None
-        }
-        self._fill_gaps_at_list(self._fill_output_gap, request, paths_to_leaves)
-        return paths_to_leaves
+        return self._make_paths_to_leaves(request, fields_to_paths, OutFieldCrown, self._fill_output_gap)
 
 
 @dataclass
 class SievesSchema(Schema):
-    omit_default: bool
+    omit_default: RequestChecker
 
 
 @dataclass
 class SievesOverlay(Overlay[SievesSchema]):
-    omit_default: Omittable[bool]
+    omit_default: Omittable[RequestChecker]
 
 
 class BuiltinSievesMaker(SievesMaker):
     def _create_sieve(self, field: OutputField) -> Sieve:
         if isinstance(field.default, DefaultValue):
             default_value = field.default.value
-            return lambda x: x != default_value
+            return with_default_clause(lambda x: x != default_value, field.default)
 
         if isinstance(field.default, DefaultFactory):
             default_factory = field.default.factory
-            return lambda x: x != default_factory()
+            return with_default_clause(lambda x: x != default_factory(), field.default)
 
         raise ValueError
 
     def make_sieves(
         self,
         mediator: Mediator,
         request: OutputNameLayoutRequest,
         paths_to_leaves: PathsTo[LeafOutCrown],
     ) -> PathsTo[Sieve]:
         schema = provide_schema(SievesOverlay, mediator, request.loc_map)
-        if not schema.omit_default:
-            return {}
-
         result = {}
         for path, leaf in paths_to_leaves.items():
             if isinstance(leaf, OutFieldCrown):
-                field = request.figure.fields_dict[leaf.name]
-                if field.default != NoDefault():
+                field = request.shape.fields_dict[leaf.id]
+                if field.default != NoDefault() and apply_rc(mediator, schema.omit_default, field):
                     result[path] = self._create_sieve(field)
         return result
 
 
 def _paths_to_branches(paths_to_leaves: PathsTo[LeafBaseCrown]) -> Iterable[Tuple[Path, Key]]:
     yielded_branch_path: Set[Path] = set()
     for path in paths_to_leaves.keys():
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/crown_builder.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/name_layout/crown_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
     leaf: LeafCr
 
 
 PathedLeafs = Sequence[PathWithLeaf[LeafCr]]
 
 
 class BaseCrownBuilder(ABC, Generic[LeafCr, DictCr, ListCr]):
-    def build_crown(self, path_to_leaf: PathsTo[LeafCr]) -> Union[DictCr, ListCr]:
-        if not path_to_leaf:
+    def build_crown(self, paths_to_leaves: PathsTo[LeafCr]) -> Union[DictCr, ListCr]:
+        if not paths_to_leaves:
             return self._make_dict_crown(current_path=(), paths_with_leafs=[])
 
-        paths_with_leafs = [PathWithLeaf(path, leaf) for path, leaf in path_to_leaf.items()]
+        paths_with_leafs = [PathWithLeaf(path, leaf) for path, leaf in paths_to_leaves.items()]
         paths_with_leafs.sort(key=lambda x: x.path)
         return cast(Union[DictCr, ListCr], self._build_crown(paths_with_leafs, 0))
 
     def _build_crown(self, paths_with_leafs: PathedLeafs[LeafCr], path_offset: int) -> Union[LeafCr, DictCr, ListCr]:
         if not paths_with_leafs:
             raise ValueError
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/provider.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/name_layout/provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from typing import TypeVar
 
-from ...model_tools import InputFigure, OutputFigure
-from ..essential import Mediator
-from ..model import DictExtraPolicy, InputNameLayout, OutputNameLayout
+from adaptix._internal.essential import Mediator
+
+from ...model_tools.definitions import InputShape, OutputShape
 from ..model.crown_definitions import (
     BranchInpCrown,
     BranchOutCrown,
+    DictExtraPolicy,
+    InputNameLayout,
     InputNameLayoutRequest,
     LeafInpCrown,
     LeafOutCrown,
+    OutputNameLayout,
     OutputNameLayoutRequest,
     Sieve,
 )
 from ..static_provider import StaticProvider, static_provision_action
 from .base import ExtraMoveMaker, ExtraPoliciesMaker, PathsTo, SievesMaker, StructureMaker
 from .crown_builder import InpCrownBuilder, OutCrownBuilder
 
@@ -31,45 +34,43 @@
         self._sieves_maker = sieves_maker
         self._extra_policies_maker = extra_policies_maker
         self._extra_move_maker = extra_move_maker
 
     @static_provision_action
     def _provide_input_name_layout(self, mediator: Mediator, request: InputNameLayoutRequest) -> InputNameLayout:
         extra_move = self._extra_move_maker.make_inp_extra_move(mediator, request)
-        path_to_leaf = self._structure_maker.make_inp_structure(mediator, request, extra_move)
-        extra_policies = self._extra_policies_maker.make_extra_policies(mediator, request, path_to_leaf)
-
+        paths_to_leaves = self._structure_maker.make_inp_structure(mediator, request, extra_move)
+        extra_policies = self._extra_policies_maker.make_extra_policies(mediator, request, paths_to_leaves)
         return InputNameLayout(
-            crown=self._create_input_crown(mediator, request.figure, path_to_leaf, extra_policies),
+            crown=self._create_input_crown(mediator, request.shape, paths_to_leaves, extra_policies),
             extra_move=extra_move,
         )
 
     # noinspection PyUnusedLocal
     def _create_input_crown(
         self,
         mediator: Mediator,
-        figure: InputFigure,
-        path_to_leaf: PathsTo[LeafInpCrown],
+        shape: InputShape,
+        paths_to_leaves: PathsTo[LeafInpCrown],
         extra_policies: PathsTo[DictExtraPolicy],
     ) -> BranchInpCrown:
-        return InpCrownBuilder(extra_policies).build_crown(path_to_leaf)
+        return InpCrownBuilder(extra_policies).build_crown(paths_to_leaves)
 
     @static_provision_action
     def _provide_output_name_layout(self, mediator: Mediator, request: OutputNameLayoutRequest) -> OutputNameLayout:
         extra_move = self._extra_move_maker.make_out_extra_move(mediator, request)
-        path_to_leaf = self._structure_maker.make_out_structure(mediator, request, extra_move)
-        path_to_sieve = self._sieves_maker.make_sieves(mediator, request, path_to_leaf)
-
+        paths_to_leaves = self._structure_maker.make_out_structure(mediator, request, extra_move)
+        path_to_sieve = self._sieves_maker.make_sieves(mediator, request, paths_to_leaves)
         return OutputNameLayout(
-            crown=self._create_output_crown(mediator, request.figure, path_to_leaf, path_to_sieve),
+            crown=self._create_output_crown(mediator, request.shape, paths_to_leaves, path_to_sieve),
             extra_move=extra_move,
         )
 
     # noinspection PyUnusedLocal
     def _create_output_crown(
         self,
         mediator: Mediator,
-        figure: OutputFigure,
-        path_to_leaf: PathsTo[LeafOutCrown],
+        shape: OutputShape,
+        paths_to_leaves: PathsTo[LeafOutCrown],
         path_to_sieve: PathsTo[Sieve],
     ) -> BranchOutCrown:
-        return OutCrownBuilder(path_to_sieve).build_crown(path_to_leaf)
+        return OutCrownBuilder(path_to_sieve).build_crown(paths_to_leaves)
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/name_style.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/name_style.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from dataclasses import dataclass
 from enum import Enum
 from functools import partial
 from typing import Callable
 
 
 class NameStyle(Enum):
+    """An enumeration of different naming conventions"""
+
     LOWER_SNAKE = "snake_case"
     CAMEL_SNAKE = "camel_Snake"
     PASCAL_SNAKE = "Pascal_Snake"
     UPPER_SNAKE = "UPPER_SNAKE"
 
     LOWER_KEBAB = "lower-kebab"
     CAMEL_KEBAB = "camel-Kebab"
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/overlay_schema.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/overlay_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, fields
 from typing import Any, Callable, ClassVar, Generic, Iterable, Mapping, Optional, Type, TypeVar
 
+from ..essential import CannotProvide, Mediator
 from ..type_tools import strip_alias
 from ..utils import ClassMap, Omitted
-from .essential import CannotProvide, Mediator
-from .provider_basics import Chain
+from .provider_wrapper import Chain
 from .request_cls import LocatedRequest, LocMap, TypeHintLoc
 from .static_provider import StaticProvider, static_provision_action
 
 
 @dataclass
 class Schema:
     pass
@@ -48,28 +48,28 @@
                 field.name: getattr(cls, f'_merge_{field.name}', cls._default_merge)
                 for field in fields(cls)
             }
         return cls._mergers
 
     def merge(self: Ov, new: Ov) -> Ov:
         merged = {}
-        for field_name, merger in self._load_mergers().items():
-            old_field_value = getattr(self, field_name)
-            new_field_value = getattr(new, field_name)
+        for field_id, merger in self._load_mergers().items():
+            old_field_value = getattr(self, field_id)
+            new_field_value = getattr(new, field_id)
             if self._is_omitted(old_field_value):
-                merged[field_name] = new_field_value
+                merged[field_id] = new_field_value
             elif self._is_omitted(new_field_value):
-                merged[field_name] = old_field_value
+                merged[field_id] = old_field_value
             else:
-                merged[field_name] = merger(self, old_field_value, new_field_value)
+                merged[field_id] = merger(self, old_field_value, new_field_value)
         return self.__class__(**merged)
 
     def to_schema(self) -> Sc:
         omitted_fields = [
-            field_name for field_name, field_value in vars(self).items()
+            field_id for field_id, field_value in vars(self).items()
             if self._is_omitted(field_value)
         ]
         if omitted_fields:
             raise ValueError(
                 f"Can not create schema because overlay contains omitted values at {omitted_fields}"
             )
         # noinspection PyArgumentList
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/provider_basics.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/provider_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import Generic, Optional, Type, TypeVar
+from typing import Optional, Type, TypeVar
 
-from .essential import CannotProvide, Mediator, Provider, Request
+from ..essential import CannotProvide, Mediator, Provider, Request
 from .request_filtering import ProviderWithRC, RequestChecker
 
 T = TypeVar('T')
 
 
 class RequestClassDeterminedProvider(Provider, ABC):
     @abstractmethod
@@ -31,32 +31,14 @@
             return self._provider.maybe_can_process_request_cls(request_cls)
         return True
 
     def get_request_checker(self) -> Optional[RequestChecker]:
         return self._request_checker
 
 
-class ValueProvider(RequestClassDeterminedProvider, Generic[T]):
-    def __init__(self, request_cls: Type[Request[T]], value: T):
-        self._request_cls = request_cls
-        self._value = value
-
-    def apply_provider(self, mediator: Mediator, request: Request):
-        if not isinstance(request, self._request_cls):
-            raise CannotProvide
-
-        return self._value
-
-    def __repr__(self):
-        return f"{type(self).__name__}({self._request_cls}, {self._value})"
-
-    def maybe_can_process_request_cls(self, request_cls: Type[Request]) -> bool:
-        return issubclass(request_cls, self._request_cls)
-
-
 class ConcatProvider(RequestClassDeterminedProvider):
     def __init__(self, *providers: Provider):
         self._providers = providers
 
     def apply_provider(self, mediator: Mediator[T], request: Request[T]) -> T:
         errors = []
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/provider_template.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/provider_template.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import ABC, abstractmethod
-from typing import Optional, Type, TypeVar, final
+from typing import Generic, Optional, Type, TypeVar, final
 
 from ..common import Dumper, Loader, TypeHint
+from ..essential import CannotProvide, Mediator, Request
 from ..type_tools import normalize_type
-from .essential import Mediator
+from .provider_wrapper import RequestClassDeterminedProvider
 from .request_cls import DumperRequest, LoaderRequest, LocMap, TypeHintLoc
 from .request_filtering import (
     AnyRequestChecker,
     ExactOriginRC,
     Pred,
     ProviderWithRC,
     RequestChecker,
@@ -77,7 +78,25 @@
 
     def _provide_dumper(self, mediator: Mediator, request: DumperRequest) -> Dumper:
         return mediator.provide(
             DumperRequest(
                 loc_map=LocMap(TypeHintLoc(type=self._impl))
             )
         )
+
+
+class ValueProvider(RequestClassDeterminedProvider, Generic[T]):
+    def __init__(self, request_cls: Type[Request[T]], value: T):
+        self._request_cls = request_cls
+        self._value = value
+
+    def apply_provider(self, mediator: Mediator, request: Request):
+        if not isinstance(request, self._request_cls):
+            raise CannotProvide
+
+        return self._value
+
+    def __repr__(self):
+        return f"{type(self).__name__}({self._request_cls}, {self._value})"
+
+    def maybe_can_process_request_cls(self, request_cls: Type[Request]) -> bool:
+        return issubclass(request_cls, self._request_cls)
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/request_cls.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/request_cls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass, field
 from typing import Any, Mapping, TypeVar
 
+from adaptix._internal.essential import CannotProvide, Request
+
 from ..common import Dumper, Loader, TypeHint
-from ..model_tools import Accessor, Default, ParamKind
-from ..provider.essential import CannotProvide, Request
+from ..model_tools.definitions import Accessor, Default, ParamKind
 from ..utils import ClassMap
 
 T = TypeVar('T')
 
 
 @dataclass(frozen=True)
 class Location:
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/request_filtering.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/request_filtering.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,26 @@
 from abc import ABC, abstractmethod
 from copy import copy
 from dataclasses import dataclass
 from inspect import isabstract
 from typing import Any, ClassVar, Iterable, Optional, Pattern, Protocol, Sequence, Tuple, Type, TypeVar, Union
 
 from ..common import TypeHint, VarTuple
-from ..type_tools import BaseNormType, NormTV, is_parametrized, is_protocol, is_subclass_soft, normalize_type
+from ..essential import CannotProvide, Mediator, Provider, Request
+from ..type_tools import (
+    BaseNormType,
+    NormTV,
+    is_bare_generic,
+    is_generic,
+    is_parametrized,
+    is_protocol,
+    is_subclass_soft,
+    normalize_type,
+)
 from ..type_tools.normalize_type import NotSubscribedError
-from .essential import CannotProvide, Mediator, Provider, Request
 from .request_cls import FieldLoc, GenericParamLoc, LocatedRequest, Location, TypeHintLoc
 
 T = TypeVar('T')
 
 
 class DirectMediator(Protocol):
     """This is copy of Mediator protocol but without provide_from_next() method"""
@@ -26,22 +35,28 @@
 
 
 class RequestChecker(ABC):
     @abstractmethod
     def check_request(self, mediator: DirectMediator, request: Request) -> None:
         """Raise CannotProvide if the request does not meet the conditions"""
 
-    def __or__(self, other: 'RequestChecker') -> 'RequestChecker':
-        return OrRequestChecker([self, other])
-
-    def __and__(self, other: 'RequestChecker') -> 'RequestChecker':
-        return AndRequestChecker([self, other])
-
-    def __xor__(self, other: 'RequestChecker') -> 'RequestChecker':
-        return XorRequestChecker(self, other)
+    def __or__(self, other: Any) -> 'RequestChecker':
+        if isinstance(other, RequestChecker):
+            return OrRequestChecker([self, other])
+        return NotImplemented
+
+    def __and__(self, other: Any) -> 'RequestChecker':
+        if isinstance(other, RequestChecker):
+            return AndRequestChecker([self, other])
+        return NotImplemented
+
+    def __xor__(self, other: Any) -> 'RequestChecker':
+        if isinstance(other, RequestChecker):
+            return XorRequestChecker(self, other)
+        return NotImplemented
 
     def __invert__(self) -> 'RequestChecker':
         return NegRequestChecker(self)
 
 
 class ProviderWithRC(Provider, ABC):
     @abstractmethod
@@ -127,32 +142,32 @@
     def _check_location(self, mediator: DirectMediator, loc: Any) -> None:
         ...
 
 
 @dataclass
 class ExactFieldNameRC(LocatedRequestChecker):
     LOCATION = FieldLoc
-    field_name: str
+    field_id: str
 
     def _check_location(self, mediator: DirectMediator, loc: FieldLoc) -> None:
-        if self.field_name == loc.name:
+        if self.field_id == loc.name:
             return
-        raise CannotProvide(f'field_name must be a {self.field_name!r}')
+        raise CannotProvide(f'field_id must be a {self.field_id!r}')
 
 
 @dataclass
 class ReFieldNameRC(LocatedRequestChecker):
     LOCATION = FieldLoc
     pattern: Pattern[str]
 
     def _check_location(self, mediator: DirectMediator, loc: FieldLoc) -> None:
         if self.pattern.fullmatch(loc.name):
             return
 
-        raise CannotProvide(f'field_name must be matched by {self.pattern!r}')
+        raise CannotProvide(f'field_id must be matched by {self.pattern!r}')
 
 
 @dataclass
 class ExactTypeRC(LocatedRequestChecker):
     LOCATION = TypeHintLoc
     norm: BaseNormType
 
@@ -204,41 +219,54 @@
             provider = self.origin_to_provider[normalize_type(loc.type).origin]
         except KeyError:
             raise CannotProvide
 
         return provider.apply_provider(mediator, request)
 
 
-class RequestStackCutter(DirectMediator):
+class RequestStackCutterMediator(DirectMediator):
     def __init__(self, mediator: DirectMediator, end_offset: int):
         self._mediator = mediator
         self._end_offset = end_offset
 
     def provide(self, request: Request[T]) -> T:
         return self._mediator.provide(request)
 
     @property
     def request_stack(self) -> Sequence[Request[Any]]:
         return self._mediator.request_stack[:-self._end_offset or None]
 
 
+class ExtraStackMediator(DirectMediator):
+    def __init__(self, mediator: Mediator, extra_stack: Sequence[Request[Any]]):
+        self._mediator = mediator
+        self._extra_stack = extra_stack
+
+    def provide(self, request: Request[T]) -> T:
+        return self._mediator.provide(request, extra_stack=self._extra_stack)
+
+    @property
+    def request_stack(self) -> Sequence[Request[Any]]:
+        return [*self._mediator.request_stack, *self._extra_stack]
+
+
 @dataclass
 class StackEndRC(RequestChecker):
     request_checkers: Sequence[RequestChecker]
 
     def check_request(self, mediator: DirectMediator, request: Request[T]) -> None:
         stack = mediator.request_stack
         offset = len(stack) - len(self.request_checkers)
 
         if offset < 0:
             raise CannotProvide("Request stack is too small")
 
         for i, (checker, stack_request) in enumerate(zip(self.request_checkers, stack[offset:]), start=0):
             checker.check_request(
-                RequestStackCutter(mediator, i),
+                RequestStackCutterMediator(mediator, i),
                 stack_request,
             )
 
 
 @dataclass
 class GenericParamRC(LocatedRequestChecker):
     LOCATION = GenericParamLoc
@@ -272,14 +300,20 @@
 
     if isinstance(pred, RequestPattern):
         return pred.build_request_checker()
 
     return None
 
 
+def _create_request_checker_by_origin(origin):
+    if is_protocol(origin) or isabstract(origin):
+        return OriginSubclassRC(origin)
+    return ExactOriginRC(origin)
+
+
 def create_request_checker(pred: Pred) -> RequestChecker:
     result = _create_non_type_hint_request_checker(pred)
     if result is not None:
         return result
 
     try:
         norm = normalize_type(pred)
@@ -287,20 +321,25 @@
         return ExactOriginRC(pred)
     except ValueError:
         raise ValueError(f'Can not create RequestChecker from {pred}')
 
     if isinstance(norm, NormTV):
         raise ValueError(f'Can not create RequestChecker from {pred} type var')
 
-    if is_parametrized(pred):
-        return ExactTypeRC(norm)
+    if is_bare_generic(pred):
+        return _create_request_checker_by_origin(norm.origin)
 
-    if is_protocol(norm.origin) or isabstract(norm.origin):
-        return OriginSubclassRC(norm.origin)
-    return ExactOriginRC(norm.origin)
+    if is_generic(pred):
+        raise ValueError(
+            f'Can not create RequestChecker from {pred} generic alias (parametrized generic)'
+        )
+
+    if not is_generic(norm.origin) and not is_parametrized(pred):
+        return _create_request_checker_by_origin(norm.origin)   # this is only an optimization
+    return ExactTypeRC(norm)
 
 
 Pat = TypeVar('Pat', bound='RequestPattern')
 
 
 class RequestPattern:
     def __init__(self, stack: VarTuple[RequestChecker]):
@@ -319,53 +358,73 @@
         if item.startswith('__') and item.endswith('__'):
             raise AttributeError
         return self[item]
 
     def __getitem__(self: Pat, item: Union[Pred, VarTuple[Pred]]) -> Pat:
         if isinstance(item, tuple):
             return self._extend_stack(
-                [OrRequestChecker([self._ensure_request_checker(el) for el in item])]
+                [OrRequestChecker([self._ensure_request_checker_from_pred(el) for el in item])]
             )
-        return self._extend_stack([self._ensure_request_checker(item)])
+        return self._extend_stack([self._ensure_request_checker_from_pred(item)])
+
+    def _ensure_request_checker(self: Pat, other: Union[Pat, RequestChecker]) -> RequestChecker:
+        if isinstance(other, RequestChecker):
+            return other
+        return other.build_request_checker()
+
+    def __or__(self: Pat, other: Union[Pat, RequestChecker]) -> Pat:
+        return self._from_rc(
+            self.build_request_checker() | self._ensure_request_checker(other)
+        )
+
+    def __ror__(self: Pat, other: Union[Pat, RequestChecker]) -> Pat:
+        return self._from_rc(
+            self._ensure_request_checker(other) | self.build_request_checker()
+        )
+
+    def __and__(self: Pat, other: Union[Pat, RequestChecker]) -> Pat:
+        return self._from_rc(
+            self.build_request_checker() & self._ensure_request_checker(other)
+        )
 
-    def __or__(self: Pat, other: Pat) -> Pat:
+    def __rand__(self: Pat, other: Union[Pat, RequestChecker]) -> Pat:
         return self._from_rc(
-            self.build_request_checker() | other.build_request_checker()
+            self._ensure_request_checker(other) & self.build_request_checker()
         )
 
-    def __and__(self: Pat, other: Pat) -> Pat:
+    def __xor__(self: Pat, other: Union[Pat, RequestChecker]) -> Pat:
         return self._from_rc(
-            self.build_request_checker() & other.build_request_checker()
+            self.build_request_checker() ^ self._ensure_request_checker(other)
         )
 
-    def __xor__(self: Pat, other: Pat) -> Pat:
+    def __rxor__(self: Pat, other: Union[Pat, RequestChecker]) -> Pat:
         return self._from_rc(
-            self.build_request_checker() ^ other.build_request_checker()
+            self._ensure_request_checker(other) ^ self.build_request_checker()
         )
 
     def __invert__(self: Pat) -> Pat:
         return self._from_rc(
             ~self.build_request_checker()
         )
 
     def __add__(self: Pat, other: Pat) -> Pat:
         return self._extend_stack(other._stack)
 
-    def _ensure_request_checker(self, pred: Any) -> RequestChecker:
+    def _ensure_request_checker_from_pred(self, pred: Any) -> RequestChecker:
         if isinstance(pred, RequestPattern):
             raise TypeError(
                 "Can not use RequestPattern as predicate inside RequestPattern."
                 " If you want to combine several RequestPattern, you can use `+` operator"
             )
 
         return create_request_checker(pred)
 
     def generic_arg(self: Pat, pos: int, pred: Pred) -> Pat:
         return self._extend_stack(
-            [GenericParamRC(pos) & self._ensure_request_checker(pred)]
+            [GenericParamRC(pos) & self._ensure_request_checker_from_pred(pred)]
         )
 
     def build_request_checker(self) -> RequestChecker:
         if len(self._stack) == 1:
             return self._stack[0]
         return StackEndRC(self._stack)
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/provider/static_provider.py` & `adaptix-3.0.0a4/src/adaptix/_internal/provider/static_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 from inspect import isfunction
 from typing import Callable, ClassVar, Dict, Iterable, Type, TypeVar, final, overload
 
-from ..type_tools import is_subclass_soft, normalize_type, strip_tags
+from ..essential import CannotProvide, Mediator, Provider, Request
+from ..type_tools import get_all_type_hints, is_subclass_soft, normalize_type, strip_tags
 from ..utils import ClassDispatcher
-from .essential import CannotProvide, Mediator, Provider, Request
-from .provider_basics import RequestClassDeterminedProvider
+from .provider_wrapper import RequestClassDeterminedProvider
 
 __all__ = ('StaticProvider', 'static_provision_action', 'RequestDispatcher')
 
 RequestDispatcher = ClassDispatcher[Request, str]
 
 R = TypeVar('R', bound=Request)
 P = TypeVar('P', bound=Provider)
@@ -59,24 +59,25 @@
 
 
 def _infer_rc(func) -> Type[Request]:
     signature = inspect.signature(func)
 
     params = list(signature.parameters.values())
 
-    if len(params) != 3:
+    if len(params) < 3:
         raise ValueError("Can not infer request class from callable")
 
     if params[2].annotation == signature.empty:
         raise ValueError("Can not infer request class from callable")
 
-    request_tp = strip_tags(normalize_type(params[2].annotation))
+    type_hints = get_all_type_hints(func)
+    request_tp = strip_tags(normalize_type(type_hints[params[2].name]))
 
     if is_subclass_soft(request_tp.origin, Request):
-        return params[2].annotation
+        return request_tp.source
 
     raise TypeError("Request parameter must be subclass of Request")
 
 
 def _make_spa_decorator(request_cls: Type[R]):
     def spa_decorator(func: Callable[[P, Mediator, R], T]):
         if hasattr(func, _SPA_RC_STORAGE):
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/retort/base_retort.py` & `adaptix-3.0.0a4/src/adaptix/_internal/retort/base_retort.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, ABCMeta, abstractmethod
-from typing import ClassVar, Iterable, Optional, Sequence, TypeVar
+from typing import ClassVar, Iterable, Sequence, TypeVar
 
 from ..common import VarTuple
-from ..provider import Mediator, Provider, Request
+from ..essential import Mediator, Provider, Request
 from ..utils import Cloneable, ForbiddingDescriptor
 from .mediator import BuiltinMediator, IntrospectingRecipeSearcher, RecipeSearcher, RecursionResolving
 
 
 class RetortMeta(ABCMeta):  # inherits from ABCMeta to be compatible with ABC
     _own_class_recipe: VarTuple[Provider]
     recipe = ForbiddingDescriptor()
@@ -40,21 +40,20 @@
                 for parent in cls.mro()
                 if isinstance(parent, RetortMeta)
             ),
             start=(),
         )
         cls._full_class_recipe = recipe_sum
 
-    def __init__(self, recipe: Optional[Iterable[Provider]]):
-        self._inc_instance_recipe = () if recipe is None else tuple(recipe)
+    def __init__(self, recipe: Iterable[Provider] = ()):
+        self._inc_instance_recipe = tuple(recipe)
         self._calculate_derived()
 
-    @abstractmethod
     def _get_config_recipe(self) -> VarTuple[Provider]:
-        ...
+        return ()
 
     def _get_full_recipe(self) -> Sequence[Provider]:
         return self._full_recipe
 
     def _calculate_derived(self):
         super()._calculate_derived()
         self._full_recipe = (
@@ -63,25 +62,21 @@
             + self._full_class_recipe
         )
         self._searcher = self._create_searcher(self._full_recipe)
 
     def _create_searcher(self, full_recipe: Sequence[Provider]) -> RecipeSearcher:
         return IntrospectingRecipeSearcher(full_recipe)
 
-    def _get_searcher(self) -> RecipeSearcher:
-        return self._searcher
-
     @abstractmethod
     def _get_recursion_resolving(self) -> RecursionResolving:
         ...
 
     def _create_mediator(self, request_stack: Sequence[Request]) -> Mediator:
-        searcher = self._get_searcher()
         recursion_resolving = self._get_recursion_resolving()
-        return BuiltinMediator(searcher, recursion_resolving, request_stack)
+        return BuiltinMediator(self._searcher, recursion_resolving, request_stack)
 
     def _provide_from_recipe(self, request: Request[T], request_stack: Sequence[Request]) -> T:
         """Process request iterating over the result of _get_full_recipe()
         :param request:
         :return: request result
         :raise CannotProvide: request was not processed
         """
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/retort/mediator.py` & `adaptix-3.0.0a4/src/adaptix/_internal/retort/mediator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from itertools import islice
 from typing import Any, Callable, Dict, Generic, Iterable, List, Sequence, Set, Tuple, Type, TypeVar
 
 from ..common import TypeHint
-from ..provider import CannotProvide, Mediator, Provider, Request
-from ..provider.provider_basics import RequestClassDeterminedProvider
+from ..essential import CannotProvide, Mediator, Provider, Request
+from ..provider.provider_wrapper import RequestClassDeterminedProvider
 from ..provider.request_filtering import ExactOriginMergedProvider, ExactOriginRC, ProviderWithRC
 from ..utils import ClassDispatcher
 
 T = TypeVar('T')
 
 
 class StubsRecursionResolver(ABC, Generic[T]):
@@ -57,30 +57,33 @@
         self.searcher = searcher
         self.recursion_resolving = recursion_resolving
 
         self._request_stack = list(request_stack)
         self.next_offset = 0
         self.recursion_stubs: Dict[Request, Any] = {}
 
-    def provide(self, request: Request[T]) -> T:
+    def provide(self, request: Request[T], *, extra_stack: Sequence[Request[Any]] = ()) -> T:
         if request in self._request_stack:  # maybe we need to lookup in set for large request_stack
+            if request in self.recursion_stubs:
+                return self.recursion_stubs[request]
             try:
                 resolver = self._get_resolver(request)
             except KeyError:
                 raise RecursionError("Infinite recursion has been detected that can not be resolved") from None
 
             stub = resolver.get_stub(request)
             self.recursion_stubs[request] = stub
             return stub
 
+        self._request_stack.extend(extra_stack)
         self._request_stack.append(request)
         try:
             result = self._provide_non_recursive(request, 0)
         finally:
-            self._request_stack.pop(-1)
+            del self._request_stack[-1 - len(extra_stack):]
 
         if request in self.recursion_stubs:
             resolver = self._get_resolver(request)
             stub = self.recursion_stubs.pop(request)
             resolver.saturate_stub(result, stub)
 
         return result
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/retort/operating_retort.py` & `adaptix-3.0.0a4/src/adaptix/_internal/retort/operating_retort.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC
 from typing import TypeVar
 
-from ..provider import CannotProvide, DumperRequest, LoaderRequest, Mediator, Provider, Request
+from ..essential import CannotProvide, Mediator, Provider, Request
+from ..provider.request_cls import DumperRequest, LoaderRequest
 from .base_retort import BaseRetort
 from .mediator import RecursionResolving, StubsRecursionResolver
 
 
 class FuncWrapper:
     __slots__ = ('__call__',)
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/struct_path.py` & `adaptix-3.0.0a4/src/adaptix/_internal/struct_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
         exc_path = get_path(exc_val)
         raise PathedException(exc_val, exc_path)
 
 
 def default_path_processor(path):
     return [
-        element if isinstance(element, (int, str)) else str(element)
+        element if isinstance(element, (int, str)) else repr(element)
         for element in path
     ]
 
 
 class StructPathRendererFilter(logging.Filter):
     __slots__ = ('_attr_name', '_path_processor')
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/type_tools/basic_utils.py` & `adaptix-3.0.0a4/src/adaptix/_internal/type_tools/basic_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import types
+import typing
 from typing import (
     Any,
     Dict,
     ForwardRef,
     Generic,
     Iterable,
     Protocol,
@@ -12,14 +13,15 @@
     get_args,
     get_origin,
     get_type_hints,
 )
 
 from ..common import TypeHint, VarTuple
 from ..feature_requirement import HAS_ANNOTATED, HAS_PY_39, HAS_STD_CLASSES_GENERICS
+from .constants import BUILTIN_ORIGIN_TO_TYPEVARS
 
 TYPED_DICT_MCS = type(types.new_class("_TypedDictSample", (TypedDict,), {}))
 
 
 def strip_alias(type_hint: TypeHint) -> TypeHint:
     origin = get_origin(type_hint)
     return type_hint if origin is None else origin
@@ -57,26 +59,14 @@
     return (
         is_subclass_soft(tp, tuple)
         and
         has_attrs(tp, NAMED_TUPLE_METHODS)
     )
 
 
-def get_type_vars(tp: TypeHint) -> VarTuple[TypeVar]:
-    return getattr(tp, '__parameters__', ())
-
-
-def is_user_defined_generic(tp) -> bool:
-    return bool(get_type_vars(tp)) and is_subclass_soft(strip_alias(tp), Generic)
-
-
-def is_generic(tp) -> bool:
-    return bool(get_type_vars(tp))
-
-
 def is_protocol(tp):
     if not isinstance(tp, type):
         return False
 
     return Protocol in tp.__bases__
 
 
@@ -91,14 +81,50 @@
     get_all_type_hints = get_type_hints
 
 
 def is_parametrized(tp: TypeHint) -> bool:
     return bool(get_args(tp))
 
 
+def get_type_vars(tp: TypeHint) -> VarTuple[TypeVar]:
+    return getattr(tp, '__parameters__', ())
+
+
+def is_user_defined_generic(tp) -> bool:
+    return bool(get_type_vars(tp)) and is_subclass_soft(strip_alias(tp), Generic)
+
+
+def is_generic(tp) -> bool:
+    return (
+        bool(get_type_vars(tp))
+        or (
+            strip_alias(tp) in BUILTIN_ORIGIN_TO_TYPEVARS
+            and not is_parametrized(tp)
+            and (
+                bool(HAS_STD_CLASSES_GENERICS) or not isinstance(tp, type)
+            )
+        )
+        or (
+            bool(HAS_ANNOTATED)
+            and get_origin(tp) == typing.Annotated
+            and is_generic(tp.__origin__)
+        )
+    )
+
+
+def is_bare_generic(tp) -> bool:
+    return (
+        (
+            is_generic(strip_alias(tp))
+            or is_generic(tp)  # for 3.8 and List (list is not generic)
+        )
+        and not is_parametrized(tp)
+    )
+
+
 def get_type_vars_of_parametrized(tp: TypeHint) -> VarTuple[TypeVar]:
     try:
         params = tp.__parameters__
     except AttributeError:
         return ()
 
     if isinstance(tp, type):
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/type_tools/generic_resolver.py` & `adaptix-3.0.0a4/src/adaptix/_internal/type_tools/generic_resolver.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/type_tools/norm_utils.py` & `adaptix-3.0.0a4/src/adaptix/_internal/type_tools/norm_utils.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/type_tools/normalize_type.py` & `adaptix-3.0.0a4/src/adaptix/_internal/type_tools/normalize_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -688,15 +688,15 @@
 
         params = self.implicit_params_getter.get_implicit_params(origin)
         if not (
             params
             or isinstance(origin, type)
             or origin in self.ALLOWED_ZERO_PARAMS_ORIGINS
         ):
-            raise ValueError(f'Can not normalize {tp}')
+            raise ValueError(f'Can not normalize {tp!r}')
 
         return _NormType(
             origin,
             tuple(self._norm_implicit_param(param) for param in params),
             source=tp,
         )
```

### Comparing `adaptix-3.0.0a3/src/adaptix/_internal/utils.py` & `adaptix-3.0.0a4/src/adaptix/_internal/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+import itertools
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from copy import copy
 from typing import (
     AbstractSet,
     Any,
     Callable,
     Collection,
     Dict,
     Generator,
     Generic,
+    Hashable,
     Iterable,
     Iterator,
     KeysView,
     Mapping,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
     ValuesView,
     final,
 )
 
+from adaptix._internal.feature_requirement import HAS_PY_310
+
 C = TypeVar('C', bound='Cloneable')
 
 
 class Cloneable(ABC):
     @abstractmethod
     def _calculate_derived(self) -> None:
         ...
@@ -95,25 +99,27 @@
 
     def __call__(cls):
         return cls._instance
 
 
 T = TypeVar('T')
 
-
-def pairs(iterable: Iterable[T]) -> Iterable[Tuple[T, T]]:
-    it = iter(iterable)
-    try:
-        past = next(it)
-    except StopIteration:
-        return
-
-    for current in it:
-        yield past, current
-        past = current
+if HAS_PY_310:
+    pairs = itertools.pairwise  # pylint: disable=invalid-name
+else:
+    def pairs(iterable: Iterable[T]) -> Iterable[Tuple[T, T]]:  # type: ignore[no-redef]
+        it = iter(iterable)
+        try:
+            past = next(it)
+        except StopIteration:
+            return
+
+        for current in it:
+            yield past, current
+            past = current
 
 
 class Omitted(metaclass=SingletonMeta):
     def __bool__(self):
         raise TypeError('Omitted() can not be used in boolean context')
 
 
@@ -194,79 +200,85 @@
 
     def __repr__(self):
         return f'{type(self).__qualname__}({self._keys!r})'
 
 
 CM = TypeVar('CM', bound='ClassMap')
 D = TypeVar('D')
+H = TypeVar('H', bound=Hashable)
 
 
-class ClassMap(Generic[T]):
+class ClassMap(Generic[H]):
     __slots__ = ('_mapping', )
 
-    def __init__(self, *values: T):
-        self._mapping: Mapping[Type[T], T] = {type(value): value for value in values}
+    def __init__(self, *values: H):
+        # need stable order for hash calculation
+        self._mapping: Mapping[Type[H], H] = {
+            type(value): value
+            for value in sorted(values, key=lambda v: type(v).__qualname__)
+        }
 
     def __getitem__(self, item: Type[D]) -> D:
         return self._mapping[item]  # type: ignore[index,return-value]
 
-    def __iter__(self) -> Iterator[Type[T]]:
+    def __iter__(self) -> Iterator[Type[H]]:
         return iter(self._mapping)
 
     def __len__(self) -> int:
         return len(self._mapping)
 
     def __contains__(self, item):
         return item in self._mapping
 
-    def has(self, *classes: Type[T]) -> bool:
+    def has(self, *classes: Type[H]) -> bool:
         return all(key in self._mapping for key in classes)
 
     def get_or_raise(
         self,
         key: Type[D],
         exception_factory: Callable[[], Union[BaseException, Type[BaseException]]],
     ) -> D:
         try:
             return self._mapping[key]  # type: ignore[index,return-value]
         except KeyError:
             raise exception_factory() from None
 
-    def keys(self) -> KeysView[Type[T]]:
+    def keys(self) -> KeysView[Type[H]]:
         return self._mapping.keys()
 
-    def values(self) -> ValuesView[T]:
+    def values(self) -> ValuesView[H]:
         return self._mapping.values()
 
     def __eq__(self, other):
         if isinstance(other, ClassMap):
             return self._mapping == other._mapping
         return NotImplemented
 
     def __ne__(self, other):
         if isinstance(other, ClassMap):
             return self._mapping != other._mapping
         return NotImplemented
 
     def __hash__(self):
-        return hash((key, value) for key, value in self._mapping.items())
+        return hash(tuple(self._mapping.values()))
 
     def __repr__(self):
-        return f'{type(self).__qualname__}({self._mapping!r})'
+        args_str = ', '.join(repr(v) for v in self._mapping.values())
+        return f'{type(self).__qualname__}({args_str})'
 
-    def _with_new_mapping(self: CM, mapping: Mapping[Type[T], T]) -> CM:
+    def _with_new_mapping(self: CM, mapping: Mapping[Type[H], H]) -> CM:
         self_copy = copy(self)
         self_copy._mapping = mapping  # pylint: disable=protected-access
         return self_copy
 
-    def add(self: CM, *values: T) -> CM:
+    def add(self: CM, *values: H) -> CM:
         return self._with_new_mapping(
             {**self._mapping, **{type(value): value for value in values}}
         )
 
-    def discard(self: CM, *classes: Type[T]) -> CM:
+    def discard(self: CM, *classes: Type[H]) -> CM:
         return self._with_new_mapping(
             {
                 key: value for key, value in self._mapping.items()
                 if key not in classes
             }
         )
```

### Comparing `adaptix-3.0.0a3/src/adaptix/load_error.py` & `adaptix-3.0.0a4/src/adaptix/load_error.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a3/src/adaptix/provider/__init__.py` & `adaptix-3.0.0a4/src/adaptix/provider/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from adaptix._internal.provider.essential import CannotProvide, Mediator, Provider, Request
+from adaptix._internal.essential import CannotProvide, Mediator, Provider, Request
 from adaptix._internal.provider.model.crown_definitions import (
     ExtraCollect,
     Extractor,
     ExtraForbid,
     ExtraKwargs,
     ExtraSkip,
     Saturator,
 )
 from adaptix._internal.provider.model.request_filtering import AnyModelRC
 from adaptix._internal.provider.name_layout.base import ExtraIn, ExtraOut
-from adaptix._internal.provider.name_layout.component import NameMapStack, RawKey, RawPath
 from adaptix._internal.provider.name_style import NameStyle
-from adaptix._internal.provider.provider_basics import Chain
+from adaptix._internal.provider.provider_wrapper import Chain
 from adaptix._internal.provider.request_filtering import P, RequestPattern, create_request_checker
 
 __all__ = (
     'CannotProvide',
     'Mediator',
     'Provider',
     'Request',
@@ -23,17 +22,14 @@
     'Extractor',
     'ExtraForbid',
     'ExtraKwargs',
     'ExtraSkip',
     'Saturator',
     'ExtraIn',
     'ExtraOut',
-    'NameMapStack',
-    'RawKey',
-    'RawPath',
     'NameStyle',
     'Chain',
     'RequestPattern',
     'P',
     'create_request_checker',
     'AnyModelRC',
 )
```

### Comparing `adaptix-3.0.0a3/src/adaptix.egg-info/PKG-INFO` & `adaptix-3.0.0a4/src/adaptix.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptix
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: An utility class for creating instances of dataclasses
 Author-email: "A. Tikhonov" <17@itishka.org>
 Project-URL: Homepage, https://github.com/reagento/dataclass_factory
 Project-URL: Bug Tracker, https://github.com/reagento/dataclass_factory/issues
 Project-URL: Documentation, https://adaptix.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/reagento/dataclass_factory/
 Project-URL: Download, https://github.com/reagento/dataclass_factory/#files
@@ -25,15 +25,15 @@
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Adaptix
 
-[![PyPI version](https://badge.fury.io/py/adaptix.svg)](https://badge.fury.io/py/dataclass-factory)
+[![PyPI version](https://img.shields.io/pypi/v/adaptix.svg)](https://badge.fury.io/py/dataclass-factory)
 [![downloads](https://img.shields.io/pypi/dm/adaptix.svg)](https://pypistats.org/packages/adaptix)
 [![versions](https://img.shields.io/pypi/pyversions/adaptix.svg)](https://github.com/reagento/dataclass_factory)
 [![license](https://img.shields.io/github/license/reagento/dataclass_factory.svg)](https://github.com/reagento/dataclass_factory/blob/master/LICENSE)
 
 An extremely flexible and configurable data model conversion library.
 
 📑 [Documentation](https://adaptix.readthedocs.io/)
@@ -67,18 +67,14 @@
 retort = Retort()
 
 book = retort.load(data, Book)
 assert book == Book(title="Fahrenheit 451", price=100)
 assert retort.dump(book) == data
 ```
 
-## Requirements
-
-* Python 3.8
-
 ## Use cases
 
 * Validation and transformation of received data for your API.
 * Config loading/dumping via codec that produces/takes dict.
 * Storing JSON in a database and representing it as a model inside the application code.
 * Creating API clients that convert a model to JSON sending to the server.
 * Persisting entities at cache storage.
@@ -91,15 +87,15 @@
   that allow preserving [SRP](https://blog.cleancoder.com/uncle-bob/2014/05/08/SingleReponsibilityPrinciple.html)
   and have different representations for one model.
 * Speed. It is one of the fastest data parsing and serialization libraries.
 * There is no forced model representation, adaptix can adjust to your needs.
 * Support [dozens](https://adaptix.readthedocs.io/en/latest/specific_types_behavior.html) of types,
   including different model kinds:
   ``@dataclass``, ``TypedDict``, ``NamedTuple``, and [``attrs``](https://www.attrs.org/en/stable/)
-* Working with cyclic-referenced structures (such as linked lists or trees).
+* Working with self-referenced data types (such as linked lists or trees).
 * Saving [path](https://adaptix.readthedocs.io/en/latest/tutorial.html#struct-path)
   where an exception is raised (including unexpected errors).
 * Easy [integration](https://adaptix.readthedocs.io/en/latest/tutorial.html#struct-path)
   with Sentry, Datadog, and other monitoring systems.
 * Machine-readable [errors](https://adaptix.readthedocs.io/en/latest/tutorial.html#error-handling)
   that could be dumped.
 * Support for user-defined generic models.
```

### Comparing `adaptix-3.0.0a3/src/adaptix.egg-info/SOURCES.txt` & `adaptix-3.0.0a4/src/adaptix.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/adaptix/struct_path.py
 src/adaptix.egg-info/PKG-INFO
 src/adaptix.egg-info/SOURCES.txt
 src/adaptix.egg-info/dependency_links.txt
 src/adaptix.egg-info/top_level.txt
 src/adaptix/_internal/__init__.py
 src/adaptix/_internal/common.py
+src/adaptix/_internal/essential.py
 src/adaptix/_internal/feature_requirement.py
 src/adaptix/_internal/load_error.py
 src/adaptix/_internal/struct_path.py
 src/adaptix/_internal/utils.py
 src/adaptix/_internal/code_tools/__init__.py
 src/adaptix/_internal/code_tools/code_builder.py
 src/adaptix/_internal/code_tools/compiler.py
@@ -26,45 +27,49 @@
 src/adaptix/_internal/facade/provider.py
 src/adaptix/_internal/facade/retort.py
 src/adaptix/_internal/model_tools/__init__.py
 src/adaptix/_internal/model_tools/definitions.py
 src/adaptix/_internal/model_tools/introspection.py
 src/adaptix/_internal/provider/__init__.py
 src/adaptix/_internal/provider/concrete_provider.py
-src/adaptix/_internal/provider/essential.py
+src/adaptix/_internal/provider/enum_provider.py
 src/adaptix/_internal/provider/generic_provider.py
 src/adaptix/_internal/provider/name_style.py
 src/adaptix/_internal/provider/overlay_schema.py
-src/adaptix/_internal/provider/provider_basics.py
 src/adaptix/_internal/provider/provider_template.py
+src/adaptix/_internal/provider/provider_wrapper.py
 src/adaptix/_internal/provider/request_cls.py
 src/adaptix/_internal/provider/request_filtering.py
 src/adaptix/_internal/provider/static_provider.py
 src/adaptix/_internal/provider/model/__init__.py
 src/adaptix/_internal/provider/model/basic_gen.py
 src/adaptix/_internal/provider/model/crown_definitions.py
 src/adaptix/_internal/provider/model/definitions.py
 src/adaptix/_internal/provider/model/dumper_provider.py
-src/adaptix/_internal/provider/model/figure_provider.py
+src/adaptix/_internal/provider/model/fields.py
 src/adaptix/_internal/provider/model/input_creation_gen.py
 src/adaptix/_internal/provider/model/input_extraction_gen.py
 src/adaptix/_internal/provider/model/loader_provider.py
 src/adaptix/_internal/provider/model/output_creation_gen.py
 src/adaptix/_internal/provider/model/output_extraction_gen.py
 src/adaptix/_internal/provider/model/request_filtering.py
+src/adaptix/_internal/provider/model/shape_provider.py
+src/adaptix/_internal/provider/model/special_cases_optimization.py
 src/adaptix/_internal/provider/name_layout/__init__.py
 src/adaptix/_internal/provider/name_layout/base.py
 src/adaptix/_internal/provider/name_layout/component.py
 src/adaptix/_internal/provider/name_layout/crown_builder.py
+src/adaptix/_internal/provider/name_layout/name_mapping.py
 src/adaptix/_internal/provider/name_layout/provider.py
 src/adaptix/_internal/retort/__init__.py
 src/adaptix/_internal/retort/base_retort.py
 src/adaptix/_internal/retort/mediator.py
 src/adaptix/_internal/retort/operating_retort.py
 src/adaptix/_internal/type_tools/__init__.py
 src/adaptix/_internal/type_tools/basic_utils.py
+src/adaptix/_internal/type_tools/constants.py
 src/adaptix/_internal/type_tools/generic_resolver.py
 src/adaptix/_internal/type_tools/implicit_params.py
 src/adaptix/_internal/type_tools/norm_utils.py
 src/adaptix/_internal/type_tools/normalize_type.py
 src/adaptix/provider/__init__.py
 src/adaptix/provider/static_provider.py
```

