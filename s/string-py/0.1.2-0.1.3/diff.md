# Comparing `tmp/string_py-0.1.2.tar.gz` & `tmp/string_py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_py-0.1.2.tar", last modified: Wed Apr 12 17:50:59 2023, max compression
+gzip compressed data, was "string_py-0.1.3.tar", last modified: Sat Jun  3 22:52:31 2023, max compression
```

## Comparing `string_py-0.1.2.tar` & `string_py-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 17:50:59.390922 string_py-0.1.2/
--rw-rw-rw-   0        0        0     1767 2023-04-12 17:50:59.388920 string_py-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1199 2023-04-12 16:46:39.000000 string_py-0.1.2/README.md
--rw-rw-rw-   0        0        0      683 2023-04-12 17:50:39.000000 string_py-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 17:50:59.390922 string_py-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-04-12 17:47:36.000000 string_py-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:50:59.371905 string_py-0.1.2/string_py/
--rw-rw-rw-   0        0        0      171 2023-04-12 17:45:17.000000 string_py-0.1.2/string_py/__init__.py
--rw-rw-rw-   0        0        0    12676 2023-04-12 16:29:23.000000 string_py-0.1.2/string_py/string_py.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:50:59.385918 string_py-0.1.2/string_py.egg-info/
--rw-rw-rw-   0        0        0     1767 2023-04-12 17:50:59.000000 string_py-0.1.2/string_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-04-12 17:50:59.000000 string_py-0.1.2/string_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 17:50:59.000000 string_py-0.1.2/string_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-12 17:50:59.000000 string_py-0.1.2/string_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 22:52:31.455397 string_py-0.1.3/
+-rw-rw-rw-   0        0        0     1767 2023-06-03 22:52:31.453396 string_py-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1199 2023-04-12 16:46:39.000000 string_py-0.1.3/README.md
+-rw-rw-rw-   0        0        0      683 2023-04-12 17:50:39.000000 string_py-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 22:52:31.455397 string_py-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-06-03 22:48:25.000000 string_py-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:52:31.440383 string_py-0.1.3/string_py/
+-rw-rw-rw-   0        0        0      171 2023-06-03 22:48:25.000000 string_py-0.1.3/string_py/__init__.py
+-rw-rw-rw-   0        0        0    16011 2023-06-03 22:48:25.000000 string_py-0.1.3/string_py/string_py.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:52:31.451397 string_py-0.1.3/string_py.egg-info/
+-rw-rw-rw-   0        0        0     1767 2023-06-03 22:52:31.000000 string_py-0.1.3/string_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-06-03 22:52:31.000000 string_py-0.1.3/string_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 22:52:31.000000 string_py-0.1.3/string_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-03 22:52:31.000000 string_py-0.1.3/string_py.egg-info/top_level.txt
```

### Comparing `string_py-0.1.2/PKG-INFO` & `string_py-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string_py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utils for strings in python
 Home-page: https://github.com/BabyEntchen/string_py
 Author: BabyEntchen
 Author-email: BabyEntchen <baby_entchen@web.de>
 License: MIT
 Project-URL: GitHub, https://github.com/BabyEntchen/string_py
 Project-URL: Documentation, https://string-py.readthedocs.io
```

### Comparing `string_py-0.1.2/README.md` & `string_py-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `string_py-0.1.2/pyproject.toml` & `string_py-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `string_py-0.1.2/setup.py` & `string_py-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 from pathlib import Path
 
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'Utils for strings in python'
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 URL = "https://github.com/BabyEntchen/string_py"
 PROJECT_URLS = {
     "Documentation": "https://string-py.readthedocs.io/en/latest/"
 },
```

### Comparing `string_py-0.1.2/string_py/string_py.py` & `string_py-0.1.3/string_py/string_py.py`

 * *Files 25% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         The value you want to work with
 
     """
 
     def __init__(self, values: str | int):
         self.values = str(values)
         self.chars = [*self.values]
-        self.ascii = {
+        self._ascii = {
             "ascii_lowercase": string.ascii_lowercase,
             "ascii_uppercase": string.ascii_uppercase,
             "digits": string.digits,
             "punctuation": string.punctuation
         }
 
     def generate(self, length: int = None, min_: int = None, max_: int = None) -> str:
@@ -187,15 +187,15 @@
             return self.values[:-length]
         else:
             return self.values[-length:]
 
     def __get(self, type_: str, index: bool) -> list[str] | dict[int, str]:
         gets = [] if index is False else {}
         for num, char in enumerate(self.values):
-            if char in self.ascii[type_]:
+            if char in self._ascii[type_]:
                 if index is False:
                     gets.append(char)
                 else:
                     gets[num] = char
         return gets
 
     def get_upper(self, chars: bool = True, index: bool = False) -> int | list[str] | dict[int, str]:
@@ -260,26 +260,82 @@
         return punctuation if chars else len(punctuation)
 
 
 class Format:
     """Format texts"""
 
     @staticmethod
-    def surround(values: str, char: str = "*") -> str:
+    def surround(values: str | list[str],
+                 all_: str = None,
+                 left: str = "\u2502",
+                 top: str = "\u2500",
+                 bottom: str = "\u2500",
+                 top_left: str = "\u250c",
+                 top_right: str = "\u2510",
+                 bottom_left: str = "\u2514",
+                 bottom_right: str = "\u2518"
+                 ) -> str:
         """Surround a text with chars
 
-        :param values: `str`
+        :param bottom:
+            Char to surround the bottom with
+        :param top:
+            Char to surround the top with
+        :param values:`str`
             Text to surround
-        :param char: `*`
-            Char to surround with
+        :param all_:
+            Char to surround everything with (Overrides all other chars)
+        :param bottom_right:
+            Char to surround the bottom right corner with
+        :param bottom_left:
+            Char to surround the bottom left corner with
+        :param top_right:
+            Char to surround the top right corner with
+        :param top_left:
+            Char to surround the top left corner with
+        :param left:
+            Char to surround the left side with
         :return:
             Returns a string with the text surrounded with certain chars
 
         """
-        return f"{char * (len(values) + 4)}\n{char} {values} {char}\n{char * (len(values) + 4)}"
+        if all_:
+            top = all_
+            bottom = all_
+            left = all_
+            top_left = all_
+            top_right = all_
+            bottom_left = all_
+            bottom_right = all_
+
+        text = ""
+        length_values = []
+
+        for part_values in values if isinstance(values, list) else [values]:
+
+            length_values += part_values.split("\n")
+
+        length = max([len(x) for x in length_values])
+        row_values = []
+
+        for num1, part_values in enumerate(values if isinstance(values, list) else [values]):
+            row_values += (part_values + ("\n" + bottom * length if num1 != len(
+                values if isinstance(values, list) else [values]) - 1 else "")).split("\n")
+
+
+        length = max([len(x) for x in row_values])
+        for num2, value in enumerate(row_values):
+            if num2 == 0:
+                text += top_left + top * length + top_right + "\n"
+            text += left + value + " " * (length - len(value)) + left + "\n"
+            if num2 == len(row_values) - 1:
+                text += bottom_left + bottom * length + bottom_right
+
+
+        return text
 
     @staticmethod
     def align(values: dict[str, str]):
         """Align a text
 
         :param values: `dict[str, str]`
             Texts to align {"Left side": "Right side"}
@@ -311,15 +367,14 @@
             The values to create the table with
         :param border: `True`
             Set to `False` to remove the border
         :return:
             Returns the table as string
 
         """
-
         length = [max([len(str(x)) for x in column]) for column in zip(*values)]
         if border:
             table = "\u250C" + "\u2500" * (sum(length) + (3 * len(values) - 1)) + "\u2510\n"
             for index, row in enumerate(values):
                 table += "\u2502"
                 for i, column in enumerate(row):
                     table += " " + column + " " * (length[i] - len(column)) + " \u2502"
@@ -334,7 +389,56 @@
             table = ""
             for index, row in enumerate(values):
                 for i, column in enumerate(row):
                     table += " " + column + " " * (length[i] - len(column)) + " "
                 if index != len(values) - 1:
                     table += "\n"
         return table
+
+
+    @staticmethod
+    def embed(
+            title: str,
+            description: str = None,
+            url: str = None,
+            fields: list[dict[str, str]] = None,
+            footer: str = None,
+            author: str = None,
+            image: str = None
+    ):
+        """Create an embed
+
+        :param title: `str`
+            Title of the embed
+        :param description: `str`
+            Description of the embed
+        :param url: `str`
+            Url of the embed
+        :param fields: `list[dict[str, str]]`
+            Fields of the embed
+        :param footer: `str`
+            Footer of the embed
+        :param author: `str`
+            Author of the embed
+        :param image: `str`
+            Image of the embed
+        :return: `str`
+
+        """
+        embed = []
+        if author:
+            embed.append(author)
+        if title:
+            embed.append(title)
+        if description:
+            embed.append(description)
+        if url:
+            embed.append(url)
+        if fields:
+            for field in fields:
+                embed.append(field["name"] + ": " + field["value"])
+        if footer:
+            embed.append(footer)
+
+        if image:
+            embed.append(image)
+        return Format.surround(embed)
```

### Comparing `string_py-0.1.2/string_py.egg-info/PKG-INFO` & `string_py-0.1.3/string_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utils for strings in python
 Home-page: https://github.com/BabyEntchen/string_py
 Author: BabyEntchen
 Author-email: BabyEntchen <baby_entchen@web.de>
 License: MIT
 Project-URL: GitHub, https://github.com/BabyEntchen/string_py
 Project-URL: Documentation, https://string-py.readthedocs.io
```

