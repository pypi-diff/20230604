# Comparing `tmp/context_menu-1.3.0.tar.gz` & `tmp/context_menu-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "context_menu-1.3.0.tar", last modified: Fri Jun  2 19:52:45 2023, max compression
+gzip compressed data, was "context_menu-1.3.1.tar", last modified: Sun Jun  4 19:20:43 2023, max compression
```

## Comparing `context_menu-1.3.0.tar` & `context_menu-1.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 19:52:45.047681 context_menu-1.3.0/
--rw-rw-rw-   0        0        0     1086 2023-06-02 19:45:36.000000 context_menu-1.3.0/LICENSE
--rw-rw-rw-   0        0        0    14964 2023-06-02 19:52:45.047681 context_menu-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    14389 2023-06-02 19:46:16.000000 context_menu-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 19:52:45.015641 context_menu-1.3.0/context_menu/
--rw-rw-rw-   0        0        0       36 2023-06-02 19:45:36.000000 context_menu-1.3.0/context_menu/__init__.py
--rw-rw-rw-   0        0        0    11820 2023-06-02 19:45:36.000000 context_menu-1.3.0/context_menu/linux_menus.py
--rw-rw-rw-   0        0        0     5401 2023-06-02 19:45:36.000000 context_menu-1.3.0/context_menu/menus.py
--rw-rw-rw-   0        0        0    12508 2023-06-02 19:45:36.000000 context_menu-1.3.0/context_menu/windows_menus.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:52:45.039684 context_menu-1.3.0/context_menu.egg-info/
--rw-rw-rw-   0        0        0    14964 2023-06-02 19:52:44.000000 context_menu-1.3.0/context_menu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-06-02 19:52:44.000000 context_menu-1.3.0/context_menu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 19:52:44.000000 context_menu-1.3.0/context_menu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 19:52:44.000000 context_menu-1.3.0/context_menu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 19:52:45.047681 context_menu-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      943 2023-06-02 19:48:43.000000 context_menu-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:20:43.256331 context_menu-1.3.1/
+-rw-rw-rw-   0        0        0     1086 2023-06-02 19:45:36.000000 context_menu-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0    14964 2023-06-04 19:20:43.254822 context_menu-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14389 2023-06-02 19:46:16.000000 context_menu-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 19:20:43.237307 context_menu-1.3.1/context_menu/
+-rw-rw-rw-   0        0        0       36 2023-06-02 19:45:36.000000 context_menu-1.3.1/context_menu/__init__.py
+-rw-rw-rw-   0        0        0    11820 2023-06-02 19:45:36.000000 context_menu-1.3.1/context_menu/linux_menus.py
+-rw-rw-rw-   0        0        0     5401 2023-06-02 19:45:36.000000 context_menu-1.3.1/context_menu/menus.py
+-rw-rw-rw-   0        0        0    12508 2023-06-02 19:45:36.000000 context_menu-1.3.1/context_menu/windows_menus.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:20:43.254822 context_menu-1.3.1/context_menu.egg-info/
+-rw-rw-rw-   0        0        0    14964 2023-06-04 19:20:43.000000 context_menu-1.3.1/context_menu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-06-04 19:20:43.000000 context_menu-1.3.1/context_menu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 19:20:43.000000 context_menu-1.3.1/context_menu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-04 19:20:43.000000 context_menu-1.3.1/context_menu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 19:20:43.256331 context_menu-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      943 2023-06-04 19:20:37.000000 context_menu-1.3.1/setup.py
```

### Comparing `context_menu-1.3.0/LICENSE` & `context_menu-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `context_menu-1.3.0/PKG-INFO` & `context_menu-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: context_menu
-Version: 1.3.0
+Version: 1.3.1
 Summary: Library to create cross-platform native context menus.
 Home-page: https://github.com/saleguas/context_menu
 Author: Salvador Aleguas
 Author-email: salvador@aleguas.dev
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `context_menu-1.3.0/README.md` & `context_menu-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `context_menu-1.3.0/context_menu/linux_menus.py` & `context_menu-1.3.1/context_menu/linux_menus.py`

 * *Files identical despite different names*

### Comparing `context_menu-1.3.0/context_menu/menus.py` & `context_menu-1.3.1/context_menu/menus.py`

 * *Files identical despite different names*

### Comparing `context_menu-1.3.0/context_menu/windows_menus.py` & `context_menu-1.3.1/context_menu/windows_menus.py`

 * *Files identical despite different names*

### Comparing `context_menu-1.3.0/context_menu.egg-info/PKG-INFO` & `context_menu-1.3.1/context_menu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: context-menu
-Version: 1.3.0
+Version: 1.3.1
 Summary: Library to create cross-platform native context menus.
 Home-page: https://github.com/saleguas/context_menu
 Author: Salvador Aleguas
 Author-email: salvador@aleguas.dev
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `context_menu-1.3.0/setup.py` & `context_menu-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text(encoding='utf-8')
 
 # This call to setup() does all the work
 setuptools.setup(
     name="context_menu",
-    version="1.3.0",
+    version="1.3.1",
     description="Library to create cross-platform native context menus.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/saleguas/context_menu",
     author="Salvador Aleguas",
     author_email="salvador@aleguas.dev",
     license="MIT",
```

