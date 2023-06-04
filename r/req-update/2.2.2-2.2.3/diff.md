# Comparing `tmp/req-update-2.2.2.tar.gz` & `tmp/req-update-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "req-update-2.2.2.tar", last modified: Mon Mar 13 07:30:54 2023, max compression
+gzip compressed data, was "req-update-2.2.3.tar", last modified: Sun Jun  4 04:45:48 2023, max compression
```

## Comparing `req-update-2.2.2.tar` & `req-update-2.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 07:30:54.220759 req-update-2.2.2/
--rw-r--r--   0 root         (0) root         (0)     4704 2023-03-13 07:30:29.000000 req-update-2.2.2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1068 2023-03-13 07:30:29.000000 req-update-2.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2023-03-13 07:30:29.000000 req-update-2.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3150 2023-03-13 07:30:54.220759 req-update-2.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2291 2023-03-13 07:30:29.000000 req-update-2.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 07:30:54.216759 req-update-2.2.2/req_update/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-13 07:30:29.000000 req-update-2.2.2/req_update/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5380 2023-03-13 07:30:29.000000 req-update-2.2.2/req_update/gitsubmodule.py
--rw-r--r--   0 root         (0) root         (0)     1306 2023-03-13 07:30:29.000000 req-update-2.2.2/req_update/go.py
--rw-r--r--   0 root         (0) root         (0)     5964 2023-03-13 07:30:29.000000 req-update-2.2.2/req_update/node.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-13 07:30:29.000000 req-update-2.2.2/req_update/py.typed
--rw-r--r--   0 root         (0) root         (0)     6181 2023-03-13 07:30:29.000000 req-update-2.2.2/req_update/python.py
--rwxr-xr-x   0 root         (0) root         (0)     3771 2023-03-13 07:30:29.000000 req-update-2.2.2/req_update/req_update.py
--rw-r--r--   0 root         (0) root         (0)     6213 2023-03-13 07:30:29.000000 req-update-2.2.2/req_update/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 07:30:54.220759 req-update-2.2.2/req_update.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-03-13 07:30:54.000000 req-update-2.2.2/req_update.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2023-03-13 07:30:54.000000 req-update-2.2.2/req_update.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 07:30:54.000000 req-update-2.2.2/req_update.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-03-13 07:30:54.000000 req-update-2.2.2/req_update.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-03-13 07:30:54.000000 req-update-2.2.2/req_update.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-13 07:30:54.000000 req-update-2.2.2/req_update.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-13 07:30:54.220759 req-update-2.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1774 2023-03-13 07:30:29.000000 req-update-2.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:45:48.837639 req-update-2.2.3/
+-rw-r--r--   0 root         (0) root         (0)     4811 2023-06-04 04:44:46.000000 req-update-2.2.3/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-06-04 04:44:46.000000 req-update-2.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-04 04:44:46.000000 req-update-2.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-06-04 04:45:48.837639 req-update-2.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-06-04 04:44:46.000000 req-update-2.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:45:48.837639 req-update-2.2.3/req_update/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 04:44:46.000000 req-update-2.2.3/req_update/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5380 2023-06-04 04:44:46.000000 req-update-2.2.3/req_update/gitsubmodule.py
+-rw-r--r--   0 root         (0) root         (0)     1306 2023-06-04 04:44:46.000000 req-update-2.2.3/req_update/go.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2023-06-04 04:44:46.000000 req-update-2.2.3/req_update/node.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 04:44:46.000000 req-update-2.2.3/req_update/py.typed
+-rw-r--r--   0 root         (0) root         (0)     6226 2023-06-04 04:44:46.000000 req-update-2.2.3/req_update/python.py
+-rwxr-xr-x   0 root         (0) root         (0)     3771 2023-06-04 04:44:46.000000 req-update-2.2.3/req_update/req_update.py
+-rw-r--r--   0 root         (0) root         (0)     6213 2023-06-04 04:44:46.000000 req-update-2.2.3/req_update/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:45:48.837639 req-update-2.2.3/req_update.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-06-04 04:45:48.000000 req-update-2.2.3/req_update.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-04 04:45:48.000000 req-update-2.2.3/req_update.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 04:45:48.000000 req-update-2.2.3/req_update.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-04 04:45:48.000000 req-update-2.2.3/req_update.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-04 04:45:48.000000 req-update-2.2.3/req_update.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-04 04:45:48.000000 req-update-2.2.3/req_update.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 04:45:48.837639 req-update-2.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-06-04 04:44:46.000000 req-update-2.2.3/setup.py
```

### Comparing `req-update-2.2.2/CHANGELOG.md` & `req-update-2.2.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGELOG
 =========
 
+2.2.3 (2023-06-03)
+------------------
+
+ - Fix python obeying dryrun configuration
+ - Update dependencies
+
+
 2.2.2 (2023-03-13)
 ------------------
 
  - Ensure spacing between version and comment when a version number increases in number of characters
  - Update dependencies
  - CI optimizations
```

### Comparing `req-update-2.2.2/LICENSE` & `req-update-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `req-update-2.2.2/PKG-INFO` & `req-update-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: req-update
-Version: 2.2.2
+Version: 2.2.3
 Summary: Req Update
 Home-page: https://github.com/albertyw/req-update
 Author: Albert Wang
 Author-email: git@albertyw.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `req-update-2.2.2/README.md` & `req-update-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `req-update-2.2.2/req_update/gitsubmodule.py` & `req-update-2.2.3/req_update/gitsubmodule.py`

 * *Files identical despite different names*

### Comparing `req-update-2.2.2/req_update/go.py` & `req-update-2.2.3/req_update/go.py`

 * *Files identical despite different names*

### Comparing `req-update-2.2.2/req_update/node.py` & `req-update-2.2.3/req_update/node.py`

 * *Files identical despite different names*

### Comparing `req-update-2.2.2/req_update/python.py` & `req-update-2.2.3/req_update/python.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,36 +94,36 @@
         result = self.util.execute_shell(command, True)
         outdated: list[dict[str, str]] = json.loads(result.stdout)
         outdated = sorted(outdated, key=lambda p: p["name"])
         return outdated
 
     @staticmethod
     @contextmanager
-    def edit_requirements(file_name: str) -> Iterator[list[str]]:
+    def edit_requirements(file_name: str, dry_run: bool) -> Iterator[list[str]]:
         """
         This yields lines from a file, which will be written back into
         the file after yielding
         """
         lines: list[str] = []
         try:
             with open(file_name, "r") as handle:
                 lines = handle.readlines()
         except FileNotFoundError:
             pass
         yield lines
-        if not lines:
+        if dry_run or not lines:
             return
         with open(file_name, "w") as handle:
             handle.write("".join(lines))
 
     def write_dependency_update(self, dependency: str, version: str) -> bool:
         """Given a dependency, update it to a given version"""
         updated = False
         for reqfile in REQUIREMENTS_FILES:
-            with Python.edit_requirements(reqfile) as lines:
+            with Python.edit_requirements(reqfile, self.util.dry_run) as lines:
                 updated_file = self.write_dependency_update_lines(
                     dependency, version, lines
                 )
                 if updated_file:
                     self.updated_files.add(reqfile)
                     updated = True
         return updated
```

### Comparing `req-update-2.2.2/req_update/req_update.py` & `req-update-2.2.3/req_update/req_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from req_update.gitsubmodule import GitSubmodule  # NOQA
 from req_update.go import Go  # NOQA
 from req_update.node import Node  # NOQA
 from req_update.python import Python  # NOQA
 from req_update.util import Updater, Util  # NOQA
 
 
-VERSION = (2, 2, 2)
+VERSION = (2, 2, 3)
 __version__ = ".".join(map(str, VERSION))
 
 
 DESCRIPTION = (
     "Update python, go, node, and git submodule dependencies for your "
     "project with git integration\n\n"
     "https://github.com/albertyw/req-update"
```

### Comparing `req-update-2.2.2/req_update/util.py` & `req-update-2.2.3/req_update/util.py`

 * *Files identical despite different names*

### Comparing `req-update-2.2.2/req_update.egg-info/PKG-INFO` & `req-update-2.2.3/req_update.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: req-update
-Version: 2.2.2
+Version: 2.2.3
 Summary: Req Update
 Home-page: https://github.com/albertyw/req-update
 Author: Albert Wang
 Author-email: git@albertyw.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `req-update-2.2.2/setup.py` & `req-update-2.2.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,16 +39,14 @@
     ],
     keywords="",
     package_data={"req_update": ["py.typed"]},
     packages=find_packages(exclude=["tests"]),
     py_modules=["req_update.req_update"],
     install_requires=[],
     test_suite="req_update.tests",
-    # testing requires flake8 and coverage but they're listed separately
-    # because they need to wrap setup.py
     extras_require={
         "dev": [],
         "test": [],
     },
     entry_points={
         "console_scripts": [
             "req_update=req_update.req_update:main",
```

