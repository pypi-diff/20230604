# Comparing `tmp/joltedmod-0.1.0.tar.gz` & `tmp/joltedmod-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joltedmod-0.1.0.tar", max compression
+gzip compressed data, was "joltedmod-0.1.1.tar", max compression
```

## Comparing `joltedmod-0.1.0.tar` & `joltedmod-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1101 2023-06-01 12:22:59.095108 joltedmod-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-06-01 12:51:13.405416 joltedmod-0.1.0/README.md
--rw-r--r--   0        0        0      311 2023-06-01 13:03:57.935186 joltedmod-0.1.0/jolted_mod/__init__.py
--rw-r--r--   0        0        0     2915 2023-06-01 12:57:15.756973 joltedmod-0.1.0/jolted_mod/block.py
--rw-r--r--   0        0        0      569 2023-06-01 12:59:00.270039 joltedmod-0.1.0/jolted_mod/block_factory.py
--rw-r--r--   0        0        0       91 2023-06-01 12:22:59.233084 joltedmod-0.1.0/jolted_mod/cell_type.py
--rw-r--r--   0        0        0     7729 2023-06-01 12:57:37.984892 joltedmod-0.1.0/jolted_mod/content_generator.py
--rw-r--r--   0        0        0     3885 2023-06-01 13:18:22.149509 joltedmod-0.1.0/jolted_mod/main.py
--rw-r--r--   0        0        0     4116 2023-06-01 12:22:59.233432 joltedmod-0.1.0/jolted_mod/template_generator.py
--rw-r--r--   0        0        0      667 2023-06-01 13:02:58.259141 joltedmod-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 joltedmod-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-06-01 12:22:59.095108 joltedmod-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-01 12:51:13.405416 joltedmod-0.1.1/README.md
+-rw-r--r--   0        0        0      311 2023-06-01 13:03:57.935186 joltedmod-0.1.1/jolted_mod/__init__.py
+-rw-r--r--   0        0        0     2915 2023-06-01 12:57:15.756973 joltedmod-0.1.1/jolted_mod/block.py
+-rw-r--r--   0        0        0      569 2023-06-01 12:59:00.270039 joltedmod-0.1.1/jolted_mod/block_factory.py
+-rw-r--r--   0        0        0       91 2023-06-01 12:22:59.233084 joltedmod-0.1.1/jolted_mod/cell_type.py
+-rw-r--r--   0        0        0     7706 2023-06-04 20:11:48.747702 joltedmod-0.1.1/jolted_mod/content_generator.py
+-rw-r--r--   0        0        0     3885 2023-06-01 13:18:22.149509 joltedmod-0.1.1/jolted_mod/main.py
+-rw-r--r--   0        0        0     4116 2023-06-01 12:22:59.233432 joltedmod-0.1.1/jolted_mod/template_generator.py
+-rw-r--r--   0        0        0      649 2023-06-04 20:13:51.947283 joltedmod-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 joltedmod-0.1.1/PKG-INFO
```

### Comparing `joltedmod-0.1.0/LICENSE` & `joltedmod-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `joltedmod-0.1.0/jolted_mod/block.py` & `joltedmod-0.1.1/jolted_mod/block.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.1.0/jolted_mod/block_factory.py` & `joltedmod-0.1.1/jolted_mod/block_factory.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.1.0/jolted_mod/content_generator.py` & `joltedmod-0.1.1/jolted_mod/content_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         blocks = await self.create_content(config_file)
         return await self._create_markdown_text(blocks)
 
     async def _create_markdown_text(self, blocks):
         """Create a markdown file from the given blocks."""
         markdown_text = ""
         for block in blocks:
-            markdown_text += f"{markdown2.markdown(block.content)}"
+            markdown_text += (block.content)
         return markdown_text
 
     async def create_content(self, config_file):
         """Create content for blocks from the given config file asynchronously."""
         async with aiohttp.ClientSession() as self._session:
             blocks = await self._parse_config_file(config_file)
             await self._update_context(config_file, blocks)
```

### Comparing `joltedmod-0.1.0/jolted_mod/main.py` & `joltedmod-0.1.1/jolted_mod/main.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.1.0/jolted_mod/template_generator.py` & `joltedmod-0.1.1/jolted_mod/template_generator.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.1.0/pyproject.toml` & `joltedmod-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "JoltEdMod"
-version = "0.1.0"
+version = "0.1.1"
 description = "JoltEd self-documenting learning module"
 authors = ["Nathan Laundry"]
+license = "MIT" 
 readme = "README.md"
 packages = [{include = "jolted_mod"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^0.27.7"
 nbformat = "^5.8.0"
 markdown2 = "^2.4.8"
 markdownify = "^0.11.6"
 tqdm = "^4.65.0"
 aiofiles = "^23.1.0"
 alive-progress = "^3.1.3"
 colorama = "^0.4.6"
-click = "^8.1.3"
-pytest = "^7.3.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 
 [build-system]
```

### Comparing `joltedmod-0.1.0/PKG-INFO` & `joltedmod-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: joltedmod
-Version: 0.1.0
+Version: 0.1.1
 Summary: JoltEd self-documenting learning module
+License: MIT
 Author: Nathan Laundry
 Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: alive-progress (>=3.1.3,<4.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: markdown2 (>=2.4.8,<3.0.0)
 Requires-Dist: markdownify (>=0.11.6,<0.12.0)
 Requires-Dist: nbformat (>=5.8.0,<6.0.0)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
```

