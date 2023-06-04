# Comparing `tmp/busy-5.0.2.tar.gz` & `tmp/busy-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busy-5.0.2.tar", last modified: Wed May 31 18:58:18 2023, max compression
+gzip compressed data, was "busy-5.0.3.tar", last modified: Sun Jun  4 04:59:36 2023, max compression
```

## Comparing `busy-5.0.2.tar` & `busy-5.0.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.203659 busy-5.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-31 18:57:57.000000 busy-5.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    22714 2023-05-31 18:58:18.203659 busy-5.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    22464 2023-05-31 18:57:57.000000 busy-5.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.193659 busy-5.0.2/busy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 18:57:57.000000 busy-5.0.2/busy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-31 18:57:57.000000 busy-5.0.2/busy/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.198659 busy-5.0.2/busy/command/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/activate_command.py
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/add_command.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/base_command.py
--rw-rw-rw-   0 root         (0) root         (0)     6843 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/command.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/curses_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1714 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/defer_command.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/delete_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/drop_and_pop_command.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/edit_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/finish_command.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/list_command.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/queues_command.py
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/resource_command.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/show_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/switch_command.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/tags_command.py
--rw-rw-rw-   0 root         (0) root         (0)     3551 2023-05-31 18:57:57.000000 busy-5.0.2/busy/handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.199659 busy-5.0.2/busy/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.200659 busy-5.0.2/busy/model/collection/
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/collection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/collection/done_collection.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/collection/plan_collection.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/collection/skip_collection.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/collection/todo_collection.py
--rw-rw-rw-   0 root         (0) root         (0)     3376 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.200659 busy-5.0.2/busy/storage/
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-31 18:57:57.000000 busy-5.0.2/busy/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-05-31 18:57:57.000000 busy-5.0.2/busy/storage/file_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.201659 busy-5.0.2/busy/ui/
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6423 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/curses_ui.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/shell_ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.202659 busy-5.0.2/busy/ui/tcl_ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/tcl_ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/tcl_ui/edit_task_widget.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/tcl_ui/get_item_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     5599 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.203659 busy-5.0.2/busy/util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 18:57:57.000000 busy-5.0.2/busy/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5935 2023-05-31 18:57:57.000000 busy-5.0.2/busy/util/class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2023-05-31 18:57:57.000000 busy-5.0.2/busy/util/date_util.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-05-31 18:57:57.000000 busy-5.0.2/busy/util/python_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-05-31 18:57:57.000000 busy-5.0.2/busy/util/selector.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-05-31 18:57:57.000000 busy-5.0.2/busy/util/super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.195659 busy-5.0.2/busy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22714 2023-05-31 18:58:18.000000 busy-5.0.2/busy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1383 2023-05-31 18:58:18.000000 busy-5.0.2/busy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:58:18.000000 busy-5.0.2/busy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-31 18:58:18.000000 busy-5.0.2/busy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-31 18:58:18.000000 busy-5.0.2/busy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-31 18:58:18.000000 busy-5.0.2/busy.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      601 2023-05-31 18:57:57.000000 busy-5.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 18:58:18.203659 busy-5.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-05-31 18:57:57.000000 busy-5.0.2/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:59:36.100295 busy-5.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-06-04 04:59:15.000000 busy-5.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22714 2023-06-04 04:59:36.100295 busy-5.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    22464 2023-06-04 04:59:15.000000 busy-5.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:59:36.092295 busy-5.0.3/busy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 04:59:16.000000 busy-5.0.3/busy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-04 04:59:15.000000 busy-5.0.3/busy/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:59:36.096295 busy-5.0.3/busy/command/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 04:59:16.000000 busy-5.0.3/busy/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/activate_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/add_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/base_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     6843 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/command.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/curses_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/defer_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/delete_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/drop_and_pop_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/edit_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/finish_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/list_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/queues_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/resource_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/show_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/switch_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-06-04 04:59:15.000000 busy-5.0.3/busy/command/tags_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     3551 2023-06-04 04:59:15.000000 busy-5.0.3/busy/handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:59:36.096295 busy-5.0.3/busy/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 04:59:16.000000 busy-5.0.3/busy/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:59:36.097295 busy-5.0.3/busy/model/collection/
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-06-04 04:59:15.000000 busy-5.0.3/busy/model/collection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-04 04:59:15.000000 busy-5.0.3/busy/model/collection/done_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-04 04:59:15.000000 busy-5.0.3/busy/model/collection/plan_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-06-04 04:59:15.000000 busy-5.0.3/busy/model/collection/skip_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-06-04 04:59:15.000000 busy-5.0.3/busy/model/collection/todo_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2023-06-04 04:59:15.000000 busy-5.0.3/busy/model/item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:59:36.097295 busy-5.0.3/busy/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-04 04:59:15.000000 busy-5.0.3/busy/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-06-04 04:59:15.000000 busy-5.0.3/busy/storage/file_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:59:36.098295 busy-5.0.3/busy/ui/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-04 04:59:15.000000 busy-5.0.3/busy/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6589 2023-06-04 04:59:15.000000 busy-5.0.3/busy/ui/curses_ui.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-06-04 04:59:15.000000 busy-5.0.3/busy/ui/shell_ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:59:36.098295 busy-5.0.3/busy/ui/tcl_ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 04:59:16.000000 busy-5.0.3/busy/ui/tcl_ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-04 04:59:15.000000 busy-5.0.3/busy/ui/tcl_ui/edit_task_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-06-04 04:59:15.000000 busy-5.0.3/busy/ui/tcl_ui/get_item_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     5599 2023-06-04 04:59:15.000000 busy-5.0.3/busy/ui/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:59:36.099295 busy-5.0.3/busy/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 04:59:16.000000 busy-5.0.3/busy/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5935 2023-06-04 04:59:16.000000 busy-5.0.3/busy/util/class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2023-06-04 04:59:16.000000 busy-5.0.3/busy/util/date_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-06-04 04:59:16.000000 busy-5.0.3/busy/util/python_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-06-04 04:59:16.000000 busy-5.0.3/busy/util/selector.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-06-04 04:59:16.000000 busy-5.0.3/busy/util/super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:59:36.093295 busy-5.0.3/busy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22714 2023-06-04 04:59:36.000000 busy-5.0.3/busy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-06-04 04:59:36.000000 busy-5.0.3/busy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 04:59:36.000000 busy-5.0.3/busy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-04 04:59:36.000000 busy-5.0.3/busy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-04 04:59:36.000000 busy-5.0.3/busy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-04 04:59:36.000000 busy-5.0.3/busy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      601 2023-06-04 04:59:16.000000 busy-5.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 04:59:36.100295 busy-5.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-06-04 04:59:16.000000 busy-5.0.3/version
```

### Comparing `busy-5.0.2/LICENSE` & `busy-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/PKG-INFO` & `busy-5.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 5.0.2
+Version: 5.0.3
 Summary: Personal time management for techies
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `busy-5.0.2/README.md` & `busy-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/command/activate_command.py` & `busy-5.0.3/busy/command/activate_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/command/add_command.py` & `busy-5.0.3/busy/command/add_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/command/command.py` & `busy-5.0.3/busy/command/command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/command/defer_command.py` & `busy-5.0.3/busy/command/defer_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/command/delete_command.py` & `busy-5.0.3/busy/command/delete_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/command/drop_and_pop_command.py` & `busy-5.0.3/busy/command/drop_and_pop_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/command/edit_command.py` & `busy-5.0.3/busy/command/edit_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/command/finish_command.py` & `busy-5.0.3/busy/command/finish_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/command/list_command.py` & `busy-5.0.3/busy/command/list_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/command/switch_command.py` & `busy-5.0.3/busy/command/switch_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/handler.py` & `busy-5.0.3/busy/handler.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/model/collection/__init__.py` & `busy-5.0.3/busy/model/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/model/item.py` & `busy-5.0.3/busy/model/item.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/storage/file_storage.py` & `busy-5.0.3/busy/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/ui/curses_ui.py` & `busy-5.0.3/busy/ui/curses_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 from argparse import Namespace
 from string import capwords
 from time import sleep
 
 from busy.ui.ui import Chooser, Prompt, TerminalUI, UserCancelError
 
 
+class CursesError(Exception):
+    pass
+
+
 class CursesUI(TerminalUI):  # pragma: nocover
 
     name = "curses"
 
     def start(self):
         self._mode = "WORK"
         chooser = Chooser()
@@ -107,14 +111,17 @@
         while True:
             self.output()
             self._update_status(self._command_prompt)
             try:
                 key = self._get_key()
             except UserCancelError:
                 break
+            except CursesError:
+                sleep(1)
+                continue
             if key == "q":
                 break
             command = self.handler.get_command(
                 'key', key, ui=self, storage=self.handler.storage,
                 queue=self.queue)
             if not command:
                 self._status = f"Invalid command {key}"
@@ -150,16 +157,18 @@
         self._statuswin.move(*cursor)
 
     # Convenience method to get one keystroke from the user.
     #
     def _get_key(self):
         try:
             key = self._statuswin.getkey()
-        except (KeyboardInterrupt, curses.error):
+        except KeyboardInterrupt:
             raise UserCancelError
+        except curses.error:
+            raise CursesError
         return key
 
     # def listmode(self):
     #     length = len(list.splitlines())
     #     if length:
     #         listpad = curses.newpad(length, curses.COLS)
     #         listpad.addstr(list)
```

### Comparing `busy-5.0.2/busy/ui/shell_ui.py` & `busy-5.0.3/busy/ui/shell_ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/ui/tcl_ui/edit_task_widget.py` & `busy-5.0.3/busy/ui/tcl_ui/edit_task_widget.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/ui/tcl_ui/get_item_widget.py` & `busy-5.0.3/busy/ui/tcl_ui/get_item_widget.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/ui/ui.py` & `busy-5.0.3/busy/ui/ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/util/class_family.py` & `busy-5.0.3/busy/util/class_family.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/util/date_util.py` & `busy-5.0.3/busy/util/date_util.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/util/selector.py` & `busy-5.0.3/busy/util/selector.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy/util/super_wrapper.py` & `busy-5.0.3/busy/util/super_wrapper.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/busy.egg-info/PKG-INFO` & `busy-5.0.3/busy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 5.0.2
+Version: 5.0.3
 Summary: Personal time management for techies
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `busy-5.0.2/busy.egg-info/SOURCES.txt` & `busy-5.0.3/busy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `busy-5.0.2/pyproject.toml` & `busy-5.0.3/pyproject.toml`

 * *Files identical despite different names*

