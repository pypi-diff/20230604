# Comparing `tmp/liquidpy-0.8.0.tar.gz` & `tmp/liquidpy-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liquidpy-0.8.0.tar", max compression
+gzip compressed data, was "liquidpy-0.8.1.tar", max compression
```

## Comparing `liquidpy-0.8.0.tar` & `liquidpy-0.8.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-03-22 19:35:15.137846 liquidpy-0.8.0/LICENSE
--rw-r--r--   0        0        0     2860 2023-03-22 19:35:15.137846 liquidpy-0.8.0/README.md
--rw-r--r--   0        0        0      191 2023-03-22 19:35:15.137846 liquidpy-0.8.0/liquid/__init__.py
--rw-r--r--   0        0        0     1553 2023-03-22 19:35:15.137846 liquidpy-0.8.0/liquid/defaults.py
--rw-r--r--   0        0        0        0 2023-03-22 19:35:15.137846 liquidpy-0.8.0/liquid/exts/__init__.py
--rw-r--r--   0        0        0     2684 2023-03-22 19:35:15.137846 liquidpy-0.8.0/liquid/exts/ext.py
--rw-r--r--   0        0        0     1979 2023-03-22 19:35:15.137846 liquidpy-0.8.0/liquid/exts/filter_colon.py
--rw-r--r--   0        0        0     1176 2023-03-22 19:35:15.137846 liquidpy-0.8.0/liquid/exts/front_matter.py
--rw-r--r--   0        0        0      238 2023-03-22 19:35:15.137846 liquidpy-0.8.0/liquid/exts/jekyll.py
--rw-r--r--   0        0        0      243 2023-03-22 19:35:15.137846 liquidpy-0.8.0/liquid/exts/shopify.py
--rw-r--r--   0        0        0     3510 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/exts/standard.py
--rw-r--r--   0        0        0      216 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/exts/wild.py
--rw-r--r--   0        0        0        0 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/filters/__init__.py
--rw-r--r--   0        0        0     9144 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/filters/jekyll.py
--rw-r--r--   0        0        0     2236 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/filters/manager.py
--rw-r--r--   0        0        0      824 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/filters/shopify.py
--rw-r--r--   0        0        0    10555 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/filters/standard.py
--rw-r--r--   0        0        0     2550 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/filters/wild.py
--rw-r--r--   0        0        0     8870 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/liquid.py
--rw-r--r--   0        0        0     4040 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/patching.py
--rw-r--r--   0        0        0        0 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/tags/__init__.py
--rw-r--r--   0        0        0     1296 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/tags/jekyll.py
--rw-r--r--   0        0        0     4065 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/tags/manager.py
--rw-r--r--   0        0        0      680 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/tags/shopify.py
--rw-r--r--   0        0        0    11387 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/tags/standard.py
--rw-r--r--   0        0        0     5289 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/tags/wild.py
--rw-r--r--   0        0        0     1927 2023-03-22 19:35:15.141846 liquidpy-0.8.0/liquid/utils.py
--rw-r--r--   0        0        0     1483 2023-03-22 19:35:15.141846 liquidpy-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 liquidpy-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-04 07:25:13.810159 liquidpy-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2860 2023-06-04 07:25:13.810159 liquidpy-0.8.1/README.md
+-rw-r--r--   0        0        0      191 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/__init__.py
+-rw-r--r--   0        0        0     1553 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/defaults.py
+-rw-r--r--   0        0        0        0 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/exts/__init__.py
+-rw-r--r--   0        0        0     3321 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/exts/ext.py
+-rw-r--r--   0        0        0     1979 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/exts/filter_colon.py
+-rw-r--r--   0        0        0     1176 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/exts/front_matter.py
+-rw-r--r--   0        0        0      238 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/exts/jekyll.py
+-rw-r--r--   0        0        0      243 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/exts/shopify.py
+-rw-r--r--   0        0        0     3510 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/exts/standard.py
+-rw-r--r--   0        0        0      216 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/exts/wild.py
+-rw-r--r--   0        0        0        0 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/filters/__init__.py
+-rw-r--r--   0        0        0     9144 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/filters/jekyll.py
+-rw-r--r--   0        0        0     2236 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/filters/manager.py
+-rw-r--r--   0        0        0      824 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/filters/shopify.py
+-rw-r--r--   0        0        0    10555 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/filters/standard.py
+-rw-r--r--   0        0        0     2550 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/filters/wild.py
+-rw-r--r--   0        0        0     8870 2023-06-04 07:25:13.814159 liquidpy-0.8.1/liquid/liquid.py
+-rw-r--r--   0        0        0     4040 2023-06-04 07:25:13.818159 liquidpy-0.8.1/liquid/patching.py
+-rw-r--r--   0        0        0        0 2023-06-04 07:25:13.818159 liquidpy-0.8.1/liquid/tags/__init__.py
+-rw-r--r--   0        0        0     1296 2023-06-04 07:25:13.818159 liquidpy-0.8.1/liquid/tags/jekyll.py
+-rw-r--r--   0        0        0     4065 2023-06-04 07:25:13.818159 liquidpy-0.8.1/liquid/tags/manager.py
+-rw-r--r--   0        0        0      680 2023-06-04 07:25:13.818159 liquidpy-0.8.1/liquid/tags/shopify.py
+-rw-r--r--   0        0        0    11387 2023-06-04 07:25:13.818159 liquidpy-0.8.1/liquid/tags/standard.py
+-rw-r--r--   0        0        0     5289 2023-06-04 07:25:13.818159 liquidpy-0.8.1/liquid/tags/wild.py
+-rw-r--r--   0        0        0     1927 2023-06-04 07:25:13.818159 liquidpy-0.8.1/liquid/utils.py
+-rw-r--r--   0        0        0     1531 2023-06-04 07:25:13.818159 liquidpy-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3948 1970-01-01 00:00:00.000000 liquidpy-0.8.1/setup.py
+-rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 liquidpy-0.8.1/PKG-INFO
```

### Comparing `liquidpy-0.8.0/LICENSE` & `liquidpy-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/README.md` & `liquidpy-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/defaults.py` & `liquidpy-0.8.1/liquid/defaults.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/exts/ext.py` & `liquidpy-0.8.1/liquid/exts/ext.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from jinja2.ext import Extension
 
 if TYPE_CHECKING:
     from jinja2.parser import Parser
 
 
 re_e = re.escape
-re_c = lambda rex: re.compile(rex, re.M | re.S)
+re_c = lambda rex: re.compile(rex, re.DOTALL | re.MULTILINE)
 
 # A unique id to encode the start strings
 ENCODING_ID = id(Extension)
 
 
 class LiquidExtension(Extension):
     """A base extension class for extensions in this package to extend"""
@@ -31,20 +31,38 @@
         name: str,
         filename: str,
     ) -> str:
         """Try to keep the tag body raw by encode the variable/comment/block
         start strings ('{{', '{#', '{%') so that the body won't be tokenized
         by jinjia.
         """
+        # Turn
+        # "  {{* ... }}" to
+        # "  {{* ... | indent(2) }}"
+        # to keep the indent for multiline variables
+        variable_start_re = re_e(self.environment.variable_start_string)
+        variable_end_re = re_e(self.environment.variable_end_string)
+        indent_re = re_c(
+            fr"^([ \t]+){variable_start_re}\*"
+            "(.*?)"
+            fr"(\-{variable_end_re}|\+{variable_end_re}|{variable_end_re})"
+        )
+        source = indent_re.sub(
+            lambda m: (
+                f"{m.group(1)}{self.environment.variable_start_string}"
+                f"{m.group(2)} | indent({m.group(1)!r}){m.group(3)}"
+            ),
+            source,
+        )
+
         if not self.__class__.raw_tags:  # pragma: no cover
             return super().preprocess(source, name, filename=filename)
 
         block_start_re = re_e(self.environment.block_start_string)
         block_end_re = re_e(self.environment.block_end_string)
-        variable_start_re = re_e(self.environment.variable_start_string)
         comment_start_re = re_e(self.environment.comment_start_string)
         to_encode = re_c(
             f"({block_start_re}|{variable_start_re}|{comment_start_re})"
         )
 
         def encode_raw(matched):
             content = to_encode.sub(
```

### Comparing `liquidpy-0.8.0/liquid/exts/filter_colon.py` & `liquidpy-0.8.1/liquid/exts/filter_colon.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/exts/front_matter.py` & `liquidpy-0.8.1/liquid/exts/front_matter.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/exts/standard.py` & `liquidpy-0.8.1/liquid/exts/standard.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/filters/jekyll.py` & `liquidpy-0.8.1/liquid/filters/jekyll.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/filters/manager.py` & `liquidpy-0.8.1/liquid/filters/manager.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/filters/shopify.py` & `liquidpy-0.8.1/liquid/filters/shopify.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/filters/standard.py` & `liquidpy-0.8.1/liquid/filters/standard.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/filters/wild.py` & `liquidpy-0.8.1/liquid/filters/wild.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/liquid.py` & `liquidpy-0.8.1/liquid/liquid.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/patching.py` & `liquidpy-0.8.1/liquid/patching.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/tags/jekyll.py` & `liquidpy-0.8.1/liquid/tags/jekyll.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/tags/manager.py` & `liquidpy-0.8.1/liquid/tags/manager.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/tags/shopify.py` & `liquidpy-0.8.1/liquid/tags/shopify.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/tags/standard.py` & `liquidpy-0.8.1/liquid/tags/standard.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/tags/wild.py` & `liquidpy-0.8.1/liquid/tags/wild.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/liquid/utils.py` & `liquidpy-0.8.1/liquid/utils.py`

 * *Files identical despite different names*

### Comparing `liquidpy-0.8.0/pyproject.toml` & `liquidpy-0.8.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "liquidpy"
-version = "0.8.0"
+version = "0.8.1"
 description = "A port of liquid template engine for python"
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/liquidpy"
 repository = "https://github.com/pwwang/liquidpy"
 
+[tool.poetry.build]
+generate-setup-file = true
+
 [[tool.poetry.packages]]
 include = "liquid"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 jinja2 = "^3"
 python-frontmatter = {version = "^1.0", optional = true}
```

### Comparing `liquidpy-0.8.0/PKG-INFO` & `liquidpy-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquidpy
-Version: 0.8.0
+Version: 0.8.1
 Summary: A port of liquid template engine for python
 Home-page: https://github.com/pwwang/liquidpy
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

