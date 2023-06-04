# Comparing `tmp/textual-astview-0.7.0.tar.gz` & `tmp/textual-astview-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual-astview-0.7.0.tar", last modified: Sat Jun  3 07:40:23 2023, max compression
+gzip compressed data, was "textual-astview-0.7.1.tar", last modified: Sun Jun  4 08:07:39 2023, max compression
```

## Comparing `textual-astview-0.7.0.tar` & `textual-astview-0.7.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-03 07:40:23.476415 textual-astview-0.7.0/
--rw-r--r--   0 davep      (501) staff       (20)     1087 2023-04-27 21:09:18.000000 textual-astview-0.7.0/LICENCE
--rw-r--r--   0 davep      (501) staff       (20)     6342 2023-06-03 07:40:23.476487 textual-astview-0.7.0/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)     4963 2023-06-03 07:39:48.000000 textual-astview-0.7.0/README.md
--rw-r--r--   0 davep      (501) staff       (20)      124 2023-04-27 21:09:18.000000 textual-astview-0.7.0/pyproject.toml
--rw-r--r--   0 davep      (501) staff       (20)     1600 2023-06-03 07:40:23.476730 textual-astview-0.7.0/setup.cfg
--rw-r--r--   0 davep      (501) staff       (20)      345 2023-04-27 21:09:18.000000 textual-astview-0.7.0/setup.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-03 07:40:23.473872 textual-astview-0.7.0/textual_astview/
--rw-r--r--   0 davep      (501) staff       (20)      934 2023-06-03 07:39:48.000000 textual-astview-0.7.0/textual_astview/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)      352 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/__main__.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-03 07:40:23.475088 textual-astview-0.7.0/textual_astview/app/
--rw-r--r--   0 davep      (501) staff       (20)       88 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/app/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     3624 2023-06-03 07:39:48.000000 textual-astview-0.7.0/textual_astview/app/astare.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-03 07:40:23.475461 textual-astview-0.7.0/textual_astview/app/screens/
--rw-r--r--   0 davep      (501) staff       (20)      342 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/app/screens/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     7822 2023-06-03 07:39:48.000000 textual-astview-0.7.0/textual_astview/app/screens/main.py
--rw-r--r--   0 davep      (501) staff       (20)        0 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/py.typed
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-03 07:40:23.476198 textual-astview-0.7.0/textual_astview/widgets/
--rw-r--r--   0 davep      (501) staff       (20)       72 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/widgets/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     7774 2023-06-03 07:39:48.000000 textual-astview-0.7.0/textual_astview/widgets/astview.py
--rw-r--r--   0 davep      (501) staff       (20)     1770 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/widgets/node_info.py
--rw-r--r--   0 davep      (501) staff       (20)     7847 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/widgets/source.py
--rw-r--r--   0 davep      (501) staff       (20)     3790 2023-04-28 08:00:33.000000 textual-astview-0.7.0/textual_astview/widgets/source_info.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-03 07:40:23.474653 textual-astview-0.7.0/textual_astview.egg-info/
--rw-r--r--   0 davep      (501) staff       (20)     6342 2023-06-03 07:40:23.000000 textual-astview-0.7.0/textual_astview.egg-info/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      687 2023-06-03 07:40:23.000000 textual-astview-0.7.0/textual_astview.egg-info/SOURCES.txt
--rw-r--r--   0 davep      (501) staff       (20)        1 2023-06-03 07:40:23.000000 textual-astview-0.7.0/textual_astview.egg-info/dependency_links.txt
--rw-r--r--   0 davep      (501) staff       (20)       59 2023-06-03 07:40:23.000000 textual-astview-0.7.0/textual_astview.egg-info/entry_points.txt
--rw-r--r--   0 davep      (501) staff       (20)       33 2023-06-03 07:40:23.000000 textual-astview-0.7.0/textual_astview.egg-info/requires.txt
--rw-r--r--   0 davep      (501) staff       (20)       16 2023-06-03 07:40:23.000000 textual-astview-0.7.0/textual_astview.egg-info/top_level.txt
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-04 08:07:39.846535 textual-astview-0.7.1/
+-rw-r--r--   0 davep      (501) staff       (20)     1087 2023-04-27 21:09:18.000000 textual-astview-0.7.1/LICENCE
+-rw-r--r--   0 davep      (501) staff       (20)     6342 2023-06-04 08:07:39.846602 textual-astview-0.7.1/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)     4963 2023-06-03 07:39:48.000000 textual-astview-0.7.1/README.md
+-rw-r--r--   0 davep      (501) staff       (20)      124 2023-04-27 21:09:18.000000 textual-astview-0.7.1/pyproject.toml
+-rw-r--r--   0 davep      (501) staff       (20)     1607 2023-06-04 08:07:39.846844 textual-astview-0.7.1/setup.cfg
+-rw-r--r--   0 davep      (501) staff       (20)      345 2023-04-27 21:09:18.000000 textual-astview-0.7.1/setup.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-04 08:07:39.844706 textual-astview-0.7.1/textual_astview/
+-rw-r--r--   0 davep      (501) staff       (20)      934 2023-06-04 08:07:08.000000 textual-astview-0.7.1/textual_astview/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)      352 2023-04-27 21:09:18.000000 textual-astview-0.7.1/textual_astview/__main__.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-04 08:07:39.845607 textual-astview-0.7.1/textual_astview/app/
+-rw-r--r--   0 davep      (501) staff       (20)       88 2023-04-27 21:09:18.000000 textual-astview-0.7.1/textual_astview/app/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     3624 2023-06-03 07:39:48.000000 textual-astview-0.7.1/textual_astview/app/astare.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-04 08:07:39.845829 textual-astview-0.7.1/textual_astview/app/screens/
+-rw-r--r--   0 davep      (501) staff       (20)      342 2023-04-27 21:09:18.000000 textual-astview-0.7.1/textual_astview/app/screens/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     8019 2023-06-04 08:07:08.000000 textual-astview-0.7.1/textual_astview/app/screens/main.py
+-rw-r--r--   0 davep      (501) staff       (20)        0 2023-04-27 21:09:18.000000 textual-astview-0.7.1/textual_astview/py.typed
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-04 08:07:39.846417 textual-astview-0.7.1/textual_astview/widgets/
+-rw-r--r--   0 davep      (501) staff       (20)       72 2023-04-27 21:09:18.000000 textual-astview-0.7.1/textual_astview/widgets/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     7774 2023-06-03 07:39:48.000000 textual-astview-0.7.1/textual_astview/widgets/astview.py
+-rw-r--r--   0 davep      (501) staff       (20)     1770 2023-04-27 21:09:18.000000 textual-astview-0.7.1/textual_astview/widgets/node_info.py
+-rw-r--r--   0 davep      (501) staff       (20)     7847 2023-04-27 21:09:18.000000 textual-astview-0.7.1/textual_astview/widgets/source.py
+-rw-r--r--   0 davep      (501) staff       (20)     3790 2023-04-28 08:00:33.000000 textual-astview-0.7.1/textual_astview/widgets/source_info.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-04 08:07:39.845378 textual-astview-0.7.1/textual_astview.egg-info/
+-rw-r--r--   0 davep      (501) staff       (20)     6342 2023-06-04 08:07:39.000000 textual-astview-0.7.1/textual_astview.egg-info/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      687 2023-06-04 08:07:39.000000 textual-astview-0.7.1/textual_astview.egg-info/SOURCES.txt
+-rw-r--r--   0 davep      (501) staff       (20)        1 2023-06-04 08:07:39.000000 textual-astview-0.7.1/textual_astview.egg-info/dependency_links.txt
+-rw-r--r--   0 davep      (501) staff       (20)       59 2023-06-04 08:07:39.000000 textual-astview-0.7.1/textual_astview.egg-info/entry_points.txt
+-rw-r--r--   0 davep      (501) staff       (20)       40 2023-06-04 08:07:39.000000 textual-astview-0.7.1/textual_astview.egg-info/requires.txt
+-rw-r--r--   0 davep      (501) staff       (20)       16 2023-06-04 08:07:39.000000 textual-astview-0.7.1/textual_astview.egg-info/top_level.txt
```

### Comparing `textual-astview-0.7.0/LICENCE` & `textual-astview-0.7.1/LICENCE`

 * *Files identical despite different names*

### Comparing `textual-astview-0.7.0/PKG-INFO` & `textual-astview-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-astview
-Version: 0.7.0
+Version: 0.7.1
 Summary: An AST viewing widget library plus app, built for and with Textual.
 Home-page: https://github.com/davep/textual-astview
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
```

### Comparing `textual-astview-0.7.0/README.md` & `textual-astview-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `textual-astview-0.7.0/setup.cfg` & `textual-astview-0.7.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 [options]
 packages = find:
 platforms = any
 include_package_data = True
 install_requires = 
 	textual>=0.27.0
-	textual-fspicker
+	textual-fspicker>=0.0.9
 python_requires = >=3.8
 
 [options.package_data]
 textual_astview = py.typed
 
 [options.entry_points]
 console_scripts =
```

### Comparing `textual-astview-0.7.0/textual_astview/__init__.py` & `textual-astview-0.7.1/textual_astview/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ######################################################################
 # Main app information.
 __author__     = "Dave Pearson"
 __copyright__  = "Copyright 2022-2023, Dave Pearson"
 __credits__    = [ "Dave Pearson" ]
 __maintainer__ = "Dave Pearson"
 __email__      = "davep@davep.org"
-__version__    = "0.7.0"
+__version__    = "0.7.1"
 __licence__    = "MIT"
 
 ##############################################################################
 # Import the widgets to make them easier to get at.
 from .widgets.astview     import ASTView, ASTNode
 from .widgets.node_info   import NodeInfo
 from .widgets.source_info import SourceInfo
```

### Comparing `textual-astview-0.7.0/textual_astview/app/astare.py` & `textual-astview-0.7.1/textual_astview/app/astare.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.7.0/textual_astview/app/screens/main.py` & `textual-astview-0.7.1/textual_astview/app/screens/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 """Main screen for astare."""
 
 ##############################################################################
+# Backward compatibility.
+from __future__ import annotations
+
+##############################################################################
 # Python imports.
 from typing    import Final, Any, cast, Optional
 from argparse  import Namespace
 from functools import partial
 from pathlib   import Path
 
 ##############################################################################
@@ -183,24 +187,25 @@
         self.app.dark = not self.app.dark
         try:
             self.query_one( Source ).dark = self.app.dark
             self.highlight_node( cast( ASTNode, self.query_one( ASTView ).cursor_node ) )
         except NoMatches:
             pass
 
-    async def open_file( self, new_file: Path ) -> None:
+    async def open_file( self, new_file: Path | None ) -> None:
         """Open a new file for viewing.
 
         Args:
             new_file: The new file to view.
         """
-        self._args.file = new_file
-        self.query_one( ASTView ).reset( new_file )
-        self.query_one( Source ).show_file( self._args.file )
-        self._init_tree()
+        if new_file is not None:
+            self._args.file = new_file
+            self.query_one( ASTView ).reset( new_file )
+            self.query_one( Source ).show_file( self._args.file )
+            self._init_tree()
 
     def action_open_new( self ) -> None:
         """Open a new file for viewing."""
         self.app.push_screen( FileOpen( self._args.file.parent if self._args.file else ".", filters=Filters(
             ( "Python Source", lambda p: p.suffix.lower() == ".py" ),
             ( "Any",           lambda _: True )
         ), must_exist=True ), callback=self.open_file )
```

### Comparing `textual-astview-0.7.0/textual_astview/widgets/astview.py` & `textual-astview-0.7.1/textual_astview/widgets/astview.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.7.0/textual_astview/widgets/node_info.py` & `textual-astview-0.7.1/textual_astview/widgets/node_info.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.7.0/textual_astview/widgets/source.py` & `textual-astview-0.7.1/textual_astview/widgets/source.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.7.0/textual_astview/widgets/source_info.py` & `textual-astview-0.7.1/textual_astview/widgets/source_info.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.7.0/textual_astview.egg-info/PKG-INFO` & `textual-astview-0.7.1/textual_astview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-astview
-Version: 0.7.0
+Version: 0.7.1
 Summary: An AST viewing widget library plus app, built for and with Textual.
 Home-page: https://github.com/davep/textual-astview
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
```

### Comparing `textual-astview-0.7.0/textual_astview.egg-info/SOURCES.txt` & `textual-astview-0.7.1/textual_astview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

