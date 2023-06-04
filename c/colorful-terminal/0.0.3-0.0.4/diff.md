# Comparing `tmp/colorful_terminal-0.0.3.tar.gz` & `tmp/colorful_terminal-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorful_terminal-0.0.3.tar", last modified: Sat Jan  7 18:43:27 2023, max compression
+gzip compressed data, was "colorful_terminal-0.0.4.tar", last modified: Sun Jun  4 17:40:48 2023, max compression
```

## Comparing `colorful_terminal-0.0.3.tar` & `colorful_terminal-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-01-07 18:43:27.512565 colorful_terminal-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-01-07 18:23:21.000000 colorful_terminal-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     9720 2023-01-07 18:43:27.511565 colorful_terminal-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8702 2023-01-07 18:23:21.000000 colorful_terminal-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-01-07 18:43:27.502563 colorful_terminal-0.0.3/colorful_terminal/
--rw-rw-rw-   0        0        0      236 2023-01-07 18:42:17.000000 colorful_terminal-0.0.3/colorful_terminal/__init__.py
--rw-rw-rw-   0        0        0    30808 2023-01-07 18:38:53.000000 colorful_terminal-0.0.3/colorful_terminal/definitions.py
-drwxrwxrwx   0        0        0        0 2023-01-07 18:43:27.510565 colorful_terminal-0.0.3/colorful_terminal.egg-info/
--rw-rw-rw-   0        0        0     9720 2023-01-07 18:43:27.000000 colorful_terminal-0.0.3/colorful_terminal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-01-07 18:43:27.000000 colorful_terminal-0.0.3/colorful_terminal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-07 18:43:27.000000 colorful_terminal-0.0.3/colorful_terminal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-01-07 18:43:27.000000 colorful_terminal-0.0.3/colorful_terminal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-07 18:43:27.512565 colorful_terminal-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1976 2023-01-07 18:42:40.000000 colorful_terminal-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:40:48.503451 colorful_terminal-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-01-07 18:23:21.000000 colorful_terminal-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     9720 2023-06-04 17:40:48.503451 colorful_terminal-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8702 2023-01-07 18:23:21.000000 colorful_terminal-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 17:40:48.495771 colorful_terminal-0.0.4/colorful_terminal/
+-rw-rw-rw-   0        0        0      260 2023-06-04 17:39:34.000000 colorful_terminal-0.0.4/colorful_terminal/__init__.py
+-rw-rw-rw-   0        0        0    31061 2023-06-04 17:37:21.000000 colorful_terminal-0.0.4/colorful_terminal/definitions.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:40:48.500908 colorful_terminal-0.0.4/colorful_terminal.egg-info/
+-rw-rw-rw-   0        0        0     9720 2023-06-04 17:40:48.000000 colorful_terminal-0.0.4/colorful_terminal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-06-04 17:40:48.000000 colorful_terminal-0.0.4/colorful_terminal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 17:40:48.000000 colorful_terminal-0.0.4/colorful_terminal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-04 17:40:48.000000 colorful_terminal-0.0.4/colorful_terminal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 17:40:48.504454 colorful_terminal-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1976 2023-06-04 17:39:43.000000 colorful_terminal-0.0.4/setup.py
```

### Comparing `colorful_terminal-0.0.3/LICENSE` & `colorful_terminal-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `colorful_terminal-0.0.3/PKG-INFO` & `colorful_terminal-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorful_terminal
-Version: 0.0.3
+Version: 0.0.4
 Summary: Print with color, style your output and take full control of your terminal.
 Home-page: https://github.com/ICreedenI/colorful_terminal
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python,print,color,colour,colored,coloured,rainbow,terminal,console,colorama
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `colorful_terminal-0.0.3/README.md` & `colorful_terminal-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `colorful_terminal-0.0.3/colorful_terminal/definitions.py` & `colorful_terminal-0.0.4/colorful_terminal/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,16 +341,17 @@
 class Styling:
     RESET_ALL = Select_Graphic_Rendition(0)
     BOLD = Select_Graphic_Rendition(1)
     DIM = Select_Graphic_Rendition(2)
     ITALIC = Select_Graphic_Rendition(3)
     UNDERLINED = Select_Graphic_Rendition(4)
     CORSSED_OUT = Select_Graphic_Rendition(9)
-    NORMAL = Select_Graphic_Rendition(22)
-    DOUBLY_UNDERLINED = NOT_BOLD = Select_Graphic_Rendition(21)
+    NORMAL = NOT_BOLD = Select_Graphic_Rendition(22)
+    NOT_ITALIC = NOT_BLACKLETTER = Select_Graphic_Rendition(23)
+    DOUBLY_UNDERLINED = Select_Graphic_Rendition(21)
     NOT_UNDERLINED = Select_Graphic_Rendition(24)
     NOT_CORSSED_OUT = Select_Graphic_Rendition(29)
     OVERLINED = Select_Graphic_Rendition(53)
     NOT_OVERLINED = Select_Graphic_Rendition(55)
     SUPERSCRIPT = Select_Graphic_Rendition(73)
     SUBSCRIPT = Select_Graphic_Rendition(74)
     NEITHER_SUPERSCRIPT_NOR_SUBSCRIPT = Select_Graphic_Rendition(75)
@@ -783,10 +784,16 @@
     )
     colored_print(Fore.get_rainbow_string("This is a rainbow string!"))
     colored_print(Back.get_rainbow_string("This is also a rainbow string!"))
     print()
     termact_demo()
 
 
+def reprint_last_line(*args):
+    nargs = [str(a) for a in args]
+    sargs = " ".join(nargs)
+    colored_print(f"{TermAct.Cursor_Previous_Line}\r{TermAct.Erase_in_Line()}{sargs}")
+
+
 if __name__ == "__main__":
 
     demo_print()
```

### Comparing `colorful_terminal-0.0.3/colorful_terminal.egg-info/PKG-INFO` & `colorful_terminal-0.0.4/colorful_terminal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorful-terminal
-Version: 0.0.3
+Version: 0.0.4
 Summary: Print with color, style your output and take full control of your terminal.
 Home-page: https://github.com/ICreedenI/colorful_terminal
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python,print,color,colour,colored,coloured,rainbow,terminal,console,colorama
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `colorful_terminal-0.0.3/setup.py` & `colorful_terminal-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = (
     "Print with color, style your output and take full control of your terminal."
 )
 
 # Setting up
 setup(
     name="colorful_terminal",
```

