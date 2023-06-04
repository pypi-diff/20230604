# Comparing `tmp/plynx-1.9.8.tar.gz` & `tmp/plynx-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plynx-1.9.8.tar", last modified: Sat Dec 24 14:42:42 2022, max compression
+gzip compressed data, was "plynx-1.9.9.tar", last modified: Mon Dec 26 22:50:41 2022, max compression
```

## Comparing `plynx-1.9.8.tar` & `plynx-1.9.9.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.409081 plynx-1.9.8/
--rw-r--r--   0 khaxis     (501) staff       (20)    11344 2020-07-25 18:46:24.000000 plynx-1.9.8/LICENSE
--rw-r--r--   0 khaxis     (501) staff       (20)     1390 2022-12-24 14:42:42.409304 plynx-1.9.8/PKG-INFO
--rw-r--r--   0 khaxis     (501) staff       (20)     4271 2022-06-04 13:09:12.000000 plynx-1.9.8/README.md
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.332040 plynx-1.9.8/plynx/
--rw-r--r--   0 khaxis     (501) staff       (20)      126 2022-12-24 14:38:06.000000 plynx-1.9.8/plynx/__init__.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.336061 plynx-1.9.8/plynx/base/
--rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.8/plynx/base/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)     6265 2022-12-10 14:55:22.000000 plynx-1.9.8/plynx/base/executor.py
--rw-r--r--   0 khaxis     (501) staff       (20)      585 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/base/hub.py
--rw-r--r--   0 khaxis     (501) staff       (20)     1773 2022-10-26 13:41:54.000000 plynx-1.9.8/plynx/base/resource.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.337167 plynx-1.9.8/plynx/bin/
--rw-r--r--   0 khaxis     (501) staff       (20)      360 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/bin/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)     7904 2022-12-24 14:38:06.000000 plynx-1.9.8/plynx/bin/cli.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.341994 plynx-1.9.8/plynx/constants/
--rw-r--r--   0 khaxis     (501) staff       (20)      715 2022-11-26 01:30:08.000000 plynx-1.9.8/plynx/constants/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)      384 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/constants/collections.py
--rw-r--r--   0 khaxis     (501) staff       (20)     3274 2022-12-23 02:07:09.000000 plynx-1.9.8/plynx/constants/node_enums.py
--rw-r--r--   0 khaxis     (501) staff       (20)      335 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/constants/parameter_types.py
--rw-r--r--   0 khaxis     (501) staff       (20)      420 2022-11-26 01:30:08.000000 plynx-1.9.8/plynx/constants/resource_enums.py
--rw-r--r--   0 khaxis     (501) staff       (20)     1145 2022-10-19 21:40:14.000000 plynx-1.9.8/plynx/constants/users.py
--rw-r--r--   0 khaxis     (501) staff       (20)      557 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/constants/validation_enums.py
--rw-r--r--   0 khaxis     (501) staff       (20)      135 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/constants/web.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.352244 plynx-1.9.8/plynx/db/
--rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.8/plynx/db/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)     4496 2022-11-26 01:30:08.000000 plynx-1.9.8/plynx/db/db_object.py
--rw-r--r--   0 khaxis     (501) staff       (20)     1977 2022-12-23 02:07:09.000000 plynx-1.9.8/plynx/db/demo_user_manager.py
--rw-r--r--   0 khaxis     (501) staff       (20)    13104 2022-12-10 14:55:22.000000 plynx-1.9.8/plynx/db/node.py
--rw-r--r--   0 khaxis     (501) staff       (20)     2530 2022-10-18 00:17:35.000000 plynx-1.9.8/plynx/db/node_cache.py
--rw-r--r--   0 khaxis     (501) staff       (20)     3818 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/db/node_cache_manager.py
--rw-r--r--   0 khaxis     (501) staff       (20)    12075 2022-12-23 19:53:14.000000 plynx-1.9.8/plynx/db/node_collection_manager.py
--rw-r--r--   0 khaxis     (501) staff       (20)     1759 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/db/run_cancellation_manager.py
--rw-r--r--   0 khaxis     (501) staff       (20)     2113 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/db/test_db_object.py
--rw-r--r--   0 khaxis     (501) staff       (20)     4858 2022-12-23 02:07:09.000000 plynx-1.9.8/plynx/db/user.py
--rw-r--r--   0 khaxis     (501) staff       (20)      424 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/db/validation_error.py
--rw-r--r--   0 khaxis     (501) staff       (20)     1221 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/db/worker_state.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.365126 plynx-1.9.8/plynx/demo/
--rw-r--r--   0 khaxis     (501) staff       (20)      272 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/demo/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)     2876 2022-12-10 14:55:22.000000 plynx-1.9.8/plynx/demo/basic_functions.py
--rw-r--r--   0 khaxis     (501) staff       (20)      758 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/demo/hello_world.py
--rw-r--r--   0 khaxis     (501) staff       (20)     2458 2022-10-26 13:41:54.000000 plynx-1.9.8/plynx/demo/types.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.373579 plynx-1.9.8/plynx/node/
--rw-r--r--   0 khaxis     (501) staff       (20)     3996 2022-12-10 14:55:22.000000 plynx-1.9.8/plynx/node/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)      557 2022-10-26 13:41:54.000000 plynx-1.9.8/plynx/node/typing.py
--rw-r--r--   0 khaxis     (501) staff       (20)     2366 2022-12-10 14:55:22.000000 plynx-1.9.8/plynx/node/utils.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.374423 plynx-1.9.8/plynx/plugins/
--rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.8/plynx/plugins/__init__.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.378755 plynx-1.9.8/plynx/plugins/executors/
--rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.8/plynx/plugins/executors/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)     2263 2022-10-18 00:17:35.000000 plynx-1.9.8/plynx/plugins/executors/bases.py
--rw-r--r--   0 khaxis     (501) staff       (20)    13749 2022-10-26 13:41:54.000000 plynx-1.9.8/plynx/plugins/executors/dag.py
--rw-r--r--   0 khaxis     (501) staff       (20)    18518 2022-11-26 01:30:08.000000 plynx-1.9.8/plynx/plugins/executors/local.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.383007 plynx-1.9.8/plynx/plugins/executors/python/
--rw-r--r--   0 khaxis     (501) staff       (20)        0 2022-02-13 21:59:50.000000 plynx-1.9.8/plynx/plugins/executors/python/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)     7975 2022-12-10 14:55:22.000000 plynx-1.9.8/plynx/plugins/executors/python/dag.py
--rw-r--r--   0 khaxis     (501) staff       (20)     6743 2022-10-26 13:41:54.000000 plynx-1.9.8/plynx/plugins/executors/python/local.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.385125 plynx-1.9.8/plynx/plugins/hubs/
--rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.8/plynx/plugins/hubs/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)      699 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/plugins/hubs/collection.py
--rw-r--r--   0 khaxis     (501) staff       (20)     3073 2022-11-26 01:30:08.000000 plynx-1.9.8/plynx/plugins/hubs/static_list.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.387044 plynx-1.9.8/plynx/plugins/resources/
--rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.8/plynx/plugins/resources/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)     1833 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/plugins/resources/cloud_resources.py
--rw-r--r--   0 khaxis     (501) staff       (20)     5144 2022-10-26 13:41:54.000000 plynx-1.9.8/plynx/plugins/resources/common.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.388328 plynx-1.9.8/plynx/plugins/resources/python/
--rw-r--r--   0 khaxis     (501) staff       (20)        0 2022-10-26 13:41:54.000000 plynx-1.9.8/plynx/plugins/resources/python/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)     1446 2022-12-10 14:55:22.000000 plynx-1.9.8/plynx/plugins/resources/python/common.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.391584 plynx-1.9.8/plynx/service/
--rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.8/plynx/service/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)     3773 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/service/cache.py
--rw-r--r--   0 khaxis     (501) staff       (20)      352 2022-11-24 21:19:42.000000 plynx-1.9.8/plynx/service/execute.py
--rw-r--r--   0 khaxis     (501) staff       (20)     1895 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/service/users.py
--rw-r--r--   0 khaxis     (501) staff       (20)     9709 2022-12-24 14:38:06.000000 plynx-1.9.8/plynx/service/worker.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.401363 plynx-1.9.8/plynx/utils/
--rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.8/plynx/utils/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)     2842 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/utils/common.py
--rw-r--r--   0 khaxis     (501) staff       (20)     9346 2022-12-24 14:38:06.000000 plynx-1.9.8/plynx/utils/config.py
--rw-r--r--   0 khaxis     (501) staff       (20)     2497 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/utils/content.py
--rw-r--r--   0 khaxis     (501) staff       (20)     2089 2022-10-18 00:17:35.000000 plynx-1.9.8/plynx/utils/db_connector.py
--rw-r--r--   0 khaxis     (501) staff       (20)      340 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/utils/exceptions.py
--rw-r--r--   0 khaxis     (501) staff       (20)      859 2022-10-18 00:17:35.000000 plynx-1.9.8/plynx/utils/executor.py
--rw-r--r--   0 khaxis     (501) staff       (20)     1389 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/utils/file_handler.py
--rw-r--r--   0 khaxis     (501) staff       (20)     1175 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/utils/hub_node_registry.py
--rw-r--r--   0 khaxis     (501) staff       (20)      359 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/utils/logs.py
--rw-r--r--   0 khaxis     (501) staff       (20)    16003 2022-12-23 02:07:09.000000 plynx-1.9.8/plynx/utils/node_utils.py
--rw-r--r--   0 khaxis     (501) staff       (20)     5126 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/utils/plugin_manager.py
--rw-r--r--   0 khaxis     (501) staff       (20)     1159 2022-10-26 13:41:54.000000 plynx-1.9.8/plynx/utils/thumbnails.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.408529 plynx-1.9.8/plynx/web/
--rw-r--r--   0 khaxis     (501) staff       (20)      377 2022-12-23 02:07:09.000000 plynx-1.9.8/plynx/web/__init__.py
--rw-r--r--   0 khaxis     (501) staff       (20)     5880 2022-12-23 02:07:09.000000 plynx-1.9.8/plynx/web/common.py
--rw-r--r--   0 khaxis     (501) staff       (20)      181 2022-06-04 13:09:12.000000 plynx-1.9.8/plynx/web/health.py
--rw-r--r--   0 khaxis     (501) staff       (20)    16966 2022-12-11 22:15:18.000000 plynx-1.9.8/plynx/web/node.py
--rw-r--r--   0 khaxis     (501) staff       (20)     3094 2022-12-24 01:11:27.000000 plynx-1.9.8/plynx/web/resource.py
--rw-r--r--   0 khaxis     (501) staff       (20)     1060 2022-12-23 02:07:09.000000 plynx-1.9.8/plynx/web/run.py
--rw-r--r--   0 khaxis     (501) staff       (20)     1166 2022-12-23 02:07:09.000000 plynx-1.9.8/plynx/web/state.py
--rw-r--r--   0 khaxis     (501) staff       (20)     6332 2022-12-23 02:07:09.000000 plynx-1.9.8/plynx/web/user.py
-drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-24 14:42:42.334370 plynx-1.9.8/plynx.egg-info/
--rw-r--r--   0 khaxis     (501) staff       (20)     1390 2022-12-24 14:42:42.000000 plynx-1.9.8/plynx.egg-info/PKG-INFO
--rw-r--r--   0 khaxis     (501) staff       (20)     2288 2022-12-24 14:42:42.000000 plynx-1.9.8/plynx.egg-info/SOURCES.txt
--rw-r--r--   0 khaxis     (501) staff       (20)        1 2022-12-24 14:42:42.000000 plynx-1.9.8/plynx.egg-info/dependency_links.txt
--rw-r--r--   0 khaxis     (501) staff       (20)       42 2022-12-24 14:42:42.000000 plynx-1.9.8/plynx.egg-info/entry_points.txt
--rw-r--r--   0 khaxis     (501) staff       (20)        1 2020-09-03 15:39:48.000000 plynx-1.9.8/plynx.egg-info/not-zip-safe
--rw-r--r--   0 khaxis     (501) staff       (20)      755 2022-12-24 14:42:42.000000 plynx-1.9.8/plynx.egg-info/requires.txt
--rw-r--r--   0 khaxis     (501) staff       (20)        6 2022-12-24 14:42:42.000000 plynx-1.9.8/plynx.egg-info/top_level.txt
--rw-r--r--   0 khaxis     (501) staff       (20)      129 2022-12-24 14:42:42.409948 plynx-1.9.8/setup.cfg
--rwxr-xr-x   0 khaxis     (501) staff       (20)     2488 2022-10-18 00:17:35.000000 plynx-1.9.8/setup.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.511985 plynx-1.9.9/
+-rw-r--r--   0 khaxis     (501) staff       (20)    11344 2020-07-25 18:46:24.000000 plynx-1.9.9/LICENSE
+-rw-r--r--   0 khaxis     (501) staff       (20)     1390 2022-12-26 22:50:41.512137 plynx-1.9.9/PKG-INFO
+-rw-r--r--   0 khaxis     (501) staff       (20)     4271 2022-06-04 13:09:12.000000 plynx-1.9.9/README.md
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.469907 plynx-1.9.9/plynx/
+-rw-r--r--   0 khaxis     (501) staff       (20)      126 2022-12-26 22:44:13.000000 plynx-1.9.9/plynx/__init__.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.473845 plynx-1.9.9/plynx/base/
+-rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.9/plynx/base/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     6264 2022-12-26 22:44:13.000000 plynx-1.9.9/plynx/base/executor.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      585 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/base/hub.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     1773 2022-10-26 13:41:54.000000 plynx-1.9.9/plynx/base/resource.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.475162 plynx-1.9.9/plynx/bin/
+-rw-r--r--   0 khaxis     (501) staff       (20)      360 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/bin/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     7904 2022-12-24 14:38:06.000000 plynx-1.9.9/plynx/bin/cli.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.480115 plynx-1.9.9/plynx/constants/
+-rw-r--r--   0 khaxis     (501) staff       (20)      715 2022-11-26 01:30:08.000000 plynx-1.9.9/plynx/constants/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      384 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/constants/collections.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     3274 2022-12-23 02:07:09.000000 plynx-1.9.9/plynx/constants/node_enums.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      335 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/constants/parameter_types.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      420 2022-11-26 01:30:08.000000 plynx-1.9.9/plynx/constants/resource_enums.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     1145 2022-10-19 21:40:14.000000 plynx-1.9.9/plynx/constants/users.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      557 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/constants/validation_enums.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      135 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/constants/web.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.487182 plynx-1.9.9/plynx/db/
+-rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.9/plynx/db/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     4496 2022-11-26 01:30:08.000000 plynx-1.9.9/plynx/db/db_object.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     1977 2022-12-23 02:07:09.000000 plynx-1.9.9/plynx/db/demo_user_manager.py
+-rw-r--r--   0 khaxis     (501) staff       (20)    13104 2022-12-10 14:55:22.000000 plynx-1.9.9/plynx/db/node.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     2530 2022-10-18 00:17:35.000000 plynx-1.9.9/plynx/db/node_cache.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     3818 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/db/node_cache_manager.py
+-rw-r--r--   0 khaxis     (501) staff       (20)    12075 2022-12-23 19:53:14.000000 plynx-1.9.9/plynx/db/node_collection_manager.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     1759 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/db/run_cancellation_manager.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     2113 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/db/test_db_object.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     4858 2022-12-23 02:07:09.000000 plynx-1.9.9/plynx/db/user.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      424 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/db/validation_error.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     1221 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/db/worker_state.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.489012 plynx-1.9.9/plynx/demo/
+-rw-r--r--   0 khaxis     (501) staff       (20)      272 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/demo/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     2876 2022-12-10 14:55:22.000000 plynx-1.9.9/plynx/demo/basic_functions.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      758 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/demo/hello_world.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     2458 2022-10-26 13:41:54.000000 plynx-1.9.9/plynx/demo/types.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.490767 plynx-1.9.9/plynx/node/
+-rw-r--r--   0 khaxis     (501) staff       (20)     3996 2022-12-10 14:55:22.000000 plynx-1.9.9/plynx/node/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      557 2022-10-26 13:41:54.000000 plynx-1.9.9/plynx/node/typing.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     2366 2022-12-10 14:55:22.000000 plynx-1.9.9/plynx/node/utils.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.491329 plynx-1.9.9/plynx/plugins/
+-rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.9/plynx/plugins/__init__.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.493094 plynx-1.9.9/plynx/plugins/executors/
+-rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.9/plynx/plugins/executors/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     2263 2022-10-18 00:17:35.000000 plynx-1.9.9/plynx/plugins/executors/bases.py
+-rw-r--r--   0 khaxis     (501) staff       (20)    13749 2022-10-26 13:41:54.000000 plynx-1.9.9/plynx/plugins/executors/dag.py
+-rw-r--r--   0 khaxis     (501) staff       (20)    18518 2022-11-26 01:30:08.000000 plynx-1.9.9/plynx/plugins/executors/local.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.494955 plynx-1.9.9/plynx/plugins/executors/python/
+-rw-r--r--   0 khaxis     (501) staff       (20)        0 2022-02-13 21:59:50.000000 plynx-1.9.9/plynx/plugins/executors/python/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     7670 2022-12-26 22:44:13.000000 plynx-1.9.9/plynx/plugins/executors/python/dag.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     6743 2022-10-26 13:41:54.000000 plynx-1.9.9/plynx/plugins/executors/python/local.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.496478 plynx-1.9.9/plynx/plugins/hubs/
+-rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.9/plynx/plugins/hubs/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      699 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/plugins/hubs/collection.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     3073 2022-11-26 01:30:08.000000 plynx-1.9.9/plynx/plugins/hubs/static_list.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.497897 plynx-1.9.9/plynx/plugins/resources/
+-rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.9/plynx/plugins/resources/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     1833 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/plugins/resources/cloud_resources.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     5144 2022-10-26 13:41:54.000000 plynx-1.9.9/plynx/plugins/resources/common.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.498821 plynx-1.9.9/plynx/plugins/resources/python/
+-rw-r--r--   0 khaxis     (501) staff       (20)        0 2022-10-26 13:41:54.000000 plynx-1.9.9/plynx/plugins/resources/python/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     1446 2022-12-10 14:55:22.000000 plynx-1.9.9/plynx/plugins/resources/python/common.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.501221 plynx-1.9.9/plynx/service/
+-rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.9/plynx/service/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     3773 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/service/cache.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      352 2022-11-24 21:19:42.000000 plynx-1.9.9/plynx/service/execute.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     1895 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/service/users.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     9369 2022-12-26 22:44:13.000000 plynx-1.9.9/plynx/service/worker.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.507081 plynx-1.9.9/plynx/utils/
+-rw-r--r--   0 khaxis     (501) staff       (20)        0 2020-07-25 18:46:24.000000 plynx-1.9.9/plynx/utils/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     2842 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/utils/common.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     9346 2022-12-24 14:38:06.000000 plynx-1.9.9/plynx/utils/config.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     2497 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/utils/content.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     2089 2022-10-18 00:17:35.000000 plynx-1.9.9/plynx/utils/db_connector.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      340 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/utils/exceptions.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      859 2022-10-18 00:17:35.000000 plynx-1.9.9/plynx/utils/executor.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     1389 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/utils/file_handler.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     1175 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/utils/hub_node_registry.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      359 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/utils/logs.py
+-rw-r--r--   0 khaxis     (501) staff       (20)    16003 2022-12-23 02:07:09.000000 plynx-1.9.9/plynx/utils/node_utils.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     5126 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/utils/plugin_manager.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     1159 2022-10-26 13:41:54.000000 plynx-1.9.9/plynx/utils/thumbnails.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.511592 plynx-1.9.9/plynx/web/
+-rw-r--r--   0 khaxis     (501) staff       (20)      377 2022-12-23 02:07:09.000000 plynx-1.9.9/plynx/web/__init__.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     5880 2022-12-23 02:07:09.000000 plynx-1.9.9/plynx/web/common.py
+-rw-r--r--   0 khaxis     (501) staff       (20)      181 2022-06-04 13:09:12.000000 plynx-1.9.9/plynx/web/health.py
+-rw-r--r--   0 khaxis     (501) staff       (20)    16966 2022-12-26 22:28:25.000000 plynx-1.9.9/plynx/web/node.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     3094 2022-12-24 01:11:27.000000 plynx-1.9.9/plynx/web/resource.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     1658 2022-12-26 22:44:13.000000 plynx-1.9.9/plynx/web/run.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     1166 2022-12-23 02:07:09.000000 plynx-1.9.9/plynx/web/state.py
+-rw-r--r--   0 khaxis     (501) staff       (20)     6332 2022-12-23 02:07:09.000000 plynx-1.9.9/plynx/web/user.py
+drwxr-xr-x   0 khaxis     (501) staff       (20)        0 2022-12-26 22:50:41.472415 plynx-1.9.9/plynx.egg-info/
+-rw-r--r--   0 khaxis     (501) staff       (20)     1390 2022-12-26 22:50:41.000000 plynx-1.9.9/plynx.egg-info/PKG-INFO
+-rw-r--r--   0 khaxis     (501) staff       (20)     2288 2022-12-26 22:50:41.000000 plynx-1.9.9/plynx.egg-info/SOURCES.txt
+-rw-r--r--   0 khaxis     (501) staff       (20)        1 2022-12-26 22:50:41.000000 plynx-1.9.9/plynx.egg-info/dependency_links.txt
+-rw-r--r--   0 khaxis     (501) staff       (20)       42 2022-12-26 22:50:41.000000 plynx-1.9.9/plynx.egg-info/entry_points.txt
+-rw-r--r--   0 khaxis     (501) staff       (20)        1 2020-09-03 15:39:48.000000 plynx-1.9.9/plynx.egg-info/not-zip-safe
+-rw-r--r--   0 khaxis     (501) staff       (20)      755 2022-12-26 22:50:41.000000 plynx-1.9.9/plynx.egg-info/requires.txt
+-rw-r--r--   0 khaxis     (501) staff       (20)        6 2022-12-26 22:50:41.000000 plynx-1.9.9/plynx.egg-info/top_level.txt
+-rw-r--r--   0 khaxis     (501) staff       (20)      129 2022-12-26 22:50:41.512592 plynx-1.9.9/setup.cfg
+-rwxr-xr-x   0 khaxis     (501) staff       (20)     2488 2022-10-18 00:17:35.000000 plynx-1.9.9/setup.py
```

### Comparing `plynx-1.9.8/LICENSE` & `plynx-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/PKG-INFO` & `plynx-1.9.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plynx
-Version: 1.9.8
+Version: 1.9.9
 Summary: ML platform
 Home-page: https://plynx.com
 Author: Ivan Khomyakov
 Author-email: ivan@plynx.com
 License: UNKNOWN
 Project-URL: Demo, https://plynx.com
 Project-URL: Source, https://github.com/plynx-team/plynx
```

### Comparing `plynx-1.9.8/README.md` & `plynx-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/base/executor.py` & `plynx-1.9.9/plynx/base/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         """Function that is regularly called by a Worker.
 
         The function is running in a separate thread and does not block execution of `run()`.
 
         Returns:
             (bool):     True if worker needs to update DB else False
         """
-        return False
+        return True
 
     @classmethod
     def get_default_node(cls, is_workflow: bool) -> Node:
         """Generate a new default Node for this executor"""
         node = Node()
         if cls.IS_GRAPH:
             nodes_parameter = Parameter(
```

### Comparing `plynx-1.9.8/plynx/base/hub.py` & `plynx-1.9.9/plynx/base/hub.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/base/resource.py` & `plynx-1.9.9/plynx/base/resource.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/bin/cli.py` & `plynx-1.9.9/plynx/bin/cli.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/constants/__init__.py` & `plynx-1.9.9/plynx/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/constants/node_enums.py` & `plynx-1.9.9/plynx/constants/node_enums.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/constants/users.py` & `plynx-1.9.9/plynx/constants/users.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/constants/validation_enums.py` & `plynx-1.9.9/plynx/constants/validation_enums.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/db/db_object.py` & `plynx-1.9.9/plynx/db/db_object.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/db/demo_user_manager.py` & `plynx-1.9.9/plynx/db/demo_user_manager.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/db/node.py` & `plynx-1.9.9/plynx/db/node.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/db/node_cache.py` & `plynx-1.9.9/plynx/db/node_cache.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/db/node_cache_manager.py` & `plynx-1.9.9/plynx/db/node_cache_manager.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/db/node_collection_manager.py` & `plynx-1.9.9/plynx/db/node_collection_manager.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/db/run_cancellation_manager.py` & `plynx-1.9.9/plynx/db/run_cancellation_manager.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/db/test_db_object.py` & `plynx-1.9.9/plynx/db/test_db_object.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/db/user.py` & `plynx-1.9.9/plynx/db/user.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/db/worker_state.py` & `plynx-1.9.9/plynx/db/worker_state.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/demo/basic_functions.py` & `plynx-1.9.9/plynx/demo/basic_functions.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/demo/hello_world.py` & `plynx-1.9.9/plynx/demo/hello_world.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/demo/types.py` & `plynx-1.9.9/plynx/demo/types.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/node/__init__.py` & `plynx-1.9.9/plynx/node/__init__.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/node/typing.py` & `plynx-1.9.9/plynx/node/typing.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/node/utils.py` & `plynx-1.9.9/plynx/node/utils.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/plugins/executors/bases.py` & `plynx-1.9.9/plynx/plugins/executors/bases.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/plugins/executors/dag.py` & `plynx-1.9.9/plynx/plugins/executors/dag.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/plugins/executors/local.py` & `plynx-1.9.9/plynx/plugins/executors/local.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/plugins/executors/python/dag.py` & `plynx-1.9.9/plynx/plugins/executors/python/dag.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import queue
 import traceback
 import uuid
 from typing import List
 
 import plynx.plugins.executors.dag
 import plynx.utils.executor
-from plynx.constants import Collections, NodeRunningStatus
+from plynx.constants import NodeRunningStatus
 from plynx.db.node import Node
 from plynx.utils import node_utils
 from plynx.utils.common import to_object_id
 
 POOL_SIZE = 3
 
 
@@ -100,27 +100,23 @@
                         ).values
                     )
             node.node_running_status = NodeRunningStatus.IN_QUEUE
 
             res.append(node)
         del self.dependency_index_to_node_ids[0]
 
-        if num_completed_jobs > 0:
-            self.node.save(collection=Collections.RUNS, force=True)
-
         return res
 
     def _execute_node(self, node: Node):
         assert self.node, "Attribute `node` is undefined"
         if NodeRunningStatus.is_finished(node.node_running_status):     # NodeRunningStatus.SPECIAL
             return
 
         logging.info(f'Execute {node} {node.title}')
         node.node_running_status = NodeRunningStatus.RUNNING
-        self.node.save(collection=Collections.RUNS)
         # TODO somehow optimize `update_node`?
         # If not copy but original sent, the dependencies list won't be updated
         self.job_run_queue.put(node.copy())
 
     def kill(self):
         """Force to kill the process.
 
@@ -188,26 +184,24 @@
             raise Exception("`preview` is not supported for the DAG")
 
         for sub_node in node_utils.traverse_in_order(self.node):
             if NodeRunningStatus.is_finished(sub_node.node_running_status):
                 continue
             self._apply_inputs(sub_node)
             sub_node.node_running_status = NodeRunningStatus.RUNNING
-            self.node.save(collection=Collections.RUNS, force=True)
 
             # Run
             self.job_run_queue.put(sub_node.copy())
             new_node = self.job_complete_queue.get()
 
             # In case something else is on the queue (i.e. canceled)
             if isinstance(new_node, Node):
                 self.update_node(new_node)
 
             if NodeRunningStatus.is_finished(self._node_running_status):
                 prev_status = self._node_running_status
                 self._node_running_status = prev_status
                 break
-            self.node.save(collection=Collections.RUNS, force=True)
 
         if self._node_running_status == NodeRunningStatus.FAILED_WAITING:
             self._node_running_status = NodeRunningStatus.FAILED
         return self._node_running_status
```

### Comparing `plynx-1.9.8/plynx/plugins/executors/python/local.py` & `plynx-1.9.9/plynx/plugins/executors/python/local.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/plugins/hubs/collection.py` & `plynx-1.9.9/plynx/plugins/hubs/collection.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/plugins/hubs/static_list.py` & `plynx-1.9.9/plynx/plugins/hubs/static_list.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/plugins/resources/cloud_resources.py` & `plynx-1.9.9/plynx/plugins/resources/cloud_resources.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/plugins/resources/common.py` & `plynx-1.9.9/plynx/plugins/resources/common.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/plugins/resources/python/common.py` & `plynx-1.9.9/plynx/plugins/resources/python/common.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/service/cache.py` & `plynx-1.9.9/plynx/service/cache.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/service/users.py` & `plynx-1.9.9/plynx/service/users.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/service/worker.py` & `plynx-1.9.9/plynx/service/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,20 @@
 import traceback
 import uuid
 from typing import Dict, Optional, Set
 
 import requests
 import six
 
-import plynx.db.node_collection_manager
-import plynx.db.run_cancellation_manager
 import plynx.utils.executor
 from plynx.base.executor import BaseExecutor
-from plynx.constants import Collections, NodeRunningStatus
+from plynx.constants import NodeRunningStatus
 from plynx.db.worker_state import WorkerState
 from plynx.utils.common import JSONEncoder, ObjectId
 from plynx.utils.config import WorkerConfig, get_web_config, get_worker_config
-from plynx.utils.db_connector import check_connection
 from plynx.utils.file_handler import upload_file_stream
 
 CONNECT_POST_TIMEOUT = 1.0
 NUM_RETRIES = 3
 REQUESTS_TIMEOUT = 10
 
 
@@ -56,16 +53,16 @@
     It calls method `tick()` of the executor with a given interval
     """
 
     TICK_TIMEOUT: int = 1
 
     def __init__(self, executor: BaseExecutor):
         self.executor = executor
-        self._tick_thread = threading.Thread(target=self.call_executor_tick, args=())
         self._stop_event = threading.Event()
+        self._tick_thread = threading.Thread(target=self.call_executor_tick, args=())
 
     def __enter__(self):
         """
         Currently no meaning of returned class
         """
         self._tick_thread.start()
         return self
@@ -78,14 +75,15 @@
         while not self._stop_event.is_set():
             self._stop_event.wait(timeout=TickThread.TICK_TIMEOUT)
             if self.executor.is_updated():
                 # Save logs whe operation is running
                 with self.executor._lock:
                     if NodeRunningStatus.is_finished(self.executor.node.node_running_status):
                         continue
+
                     resp = post_request("update_run", data={"node": self.executor.node.to_dict()})
                     logging.info(f"Run update res: {resp}")
 
 
 class Worker:
     # TODO update docstring
     """Worker main class.
@@ -109,16 +107,14 @@
     SDB_STATUS_UPDATE_TIMEOUT: int = 1
 
     # Worker State update timeout
     WORKER_STATE_UPDATE_TIMEOUT: int = 1
 
     def __init__(self, worker_config: WorkerConfig, worker_id: Optional[str]):
         self.worker_id = worker_id if worker_id else str(uuid.uuid1())
-        self.node_collection_manager = plynx.db.node_collection_manager.NodeCollectionManager(collection=Collections.RUNS)
-        self.run_cancellation_manager = plynx.db.run_cancellation_manager.RunCancellationManager()
         self.kinds = worker_config.kinds
         self.host = socket.gethostname()
         self._stop_event = threading.Event()
 
         # Mapping keep track of Worker Status
         self._run_id_to_executor: Dict[ObjectId, BaseExecutor] = {}
         self._run_id_to_executor_lock = threading.Lock()
@@ -165,15 +161,15 @@
             if executor.node._id in self._killed_run_ids:
                 self._killed_run_ids.remove(executor.node._id)
         except Exception as e:  # pylint: disable=broad-except
             logging.warning(f"Execution failed: {e}")
             executor.node.node_running_status = NodeRunningStatus.FAILED
         finally:
             with executor._lock:    # type: ignore
-                resp = post_request("update_run", data={"node": executor.node.to_dict()})
+                resp = post_request("update_run", data={"node": executor.node.to_dict()}, num_retries=3)
                 logging.info(f"Run update res: {resp}")
             with self._run_id_to_executor_lock:
                 del self._run_id_to_executor[executor.node._id]
 
     def _run_db_status_update(self):
         """Syncing with the database."""
         try:
@@ -204,19 +200,21 @@
             logging.info(f"Exit {self._run_db_status_update.__name__}")
 
     def _run_worker_state_update(self):
         """Syncing with the database."""
         try:
             while not self._stop_event.is_set():
                 # TODO move CANCEL to a separate thread
-                run_cancellations = list(self.run_cancellation_manager.get_run_cancellations())
-                run_cancellation_ids = set(map(lambda rc: rc.run_id, run_cancellations)) & set(self._run_id_to_executor.keys())
-                for run_id in run_cancellation_ids:
-                    self._killed_run_ids.add(run_id)
-                    self._run_id_to_executor[run_id].kill()
+                run_ids = list(self._run_id_to_executor.keys())
+                if run_ids:
+                    response = post_request("get_run_cancelations", data={"run_ids": run_ids}, num_retries=1)
+                    runs_to_kill = [] if not response else response["run_ids_to_cancel"]
+                    for run_id in runs_to_kill:
+                        self._killed_run_ids.add(run_id)
+                        self._run_id_to_executor[run_id].kill()
 
                 runs = []
                 with self._run_id_to_executor_lock:
                     for executor in self._run_id_to_executor.values():
                         runs.append(executor.node.to_dict())
                 worker_state = WorkerState(
                     worker_id=self.worker_id,
@@ -235,17 +233,14 @@
     def stop(self):
         """Stop worker."""
         self._stop_event.set()
 
 
 def run_worker(worker_id: Optional[str] = None):
     """Run worker daemon. It will run in the same thread."""
-    # Check connection to the db
-    check_connection()
-
     logging.info('Init Worker')
     worker_config = get_worker_config()
     logging.info(worker_config)
     worker = Worker(worker_config, worker_id)
 
     # Activate the server; this will keep running until you
     # interrupt the program with Ctrl-C
```

### Comparing `plynx-1.9.8/plynx/utils/common.py` & `plynx-1.9.9/plynx/utils/common.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/utils/config.py` & `plynx-1.9.9/plynx/utils/config.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/utils/content.py` & `plynx-1.9.9/plynx/utils/content.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/utils/db_connector.py` & `plynx-1.9.9/plynx/utils/db_connector.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/utils/executor.py` & `plynx-1.9.9/plynx/utils/executor.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/utils/file_handler.py` & `plynx-1.9.9/plynx/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/utils/hub_node_registry.py` & `plynx-1.9.9/plynx/utils/hub_node_registry.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/utils/node_utils.py` & `plynx-1.9.9/plynx/utils/node_utils.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/utils/plugin_manager.py` & `plynx-1.9.9/plynx/utils/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/utils/thumbnails.py` & `plynx-1.9.9/plynx/utils/thumbnails.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/web/common.py` & `plynx-1.9.9/plynx/web/common.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/web/node.py` & `plynx-1.9.9/plynx/web/node.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/web/resource.py` & `plynx-1.9.9/plynx/web/resource.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/web/state.py` & `plynx-1.9.9/plynx/web/state.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx/web/user.py` & `plynx-1.9.9/plynx/web/user.py`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx.egg-info/PKG-INFO` & `plynx-1.9.9/plynx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plynx
-Version: 1.9.8
+Version: 1.9.9
 Summary: ML platform
 Home-page: https://plynx.com
 Author: Ivan Khomyakov
 Author-email: ivan@plynx.com
 License: UNKNOWN
 Project-URL: Demo, https://plynx.com
 Project-URL: Source, https://github.com/plynx-team/plynx
```

### Comparing `plynx-1.9.8/plynx.egg-info/SOURCES.txt` & `plynx-1.9.9/plynx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/plynx.egg-info/requires.txt` & `plynx-1.9.9/plynx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plynx-1.9.8/setup.py` & `plynx-1.9.9/setup.py`

 * *Files identical despite different names*

