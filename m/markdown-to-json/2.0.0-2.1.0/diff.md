# Comparing `tmp/markdown-to-json-2.0.0.tar.gz` & `tmp/markdown_to_json-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-to-json-2.0.0.tar", last modified: Fri Jun  2 15:46:29 2023, max compression
+gzip compressed data, was "markdown_to_json-2.1.0.tar", max compression
```

## Comparing `markdown-to-json-2.0.0.tar` & `markdown_to_json-2.1.0.tar`

### file list

```diff
@@ -1,40 +1,21 @@
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-06-02 15:46:29.726367 markdown-to-json-2.0.0/
--rw-r--r--   0 njvack     (501) staff       (20)     1118 2023-06-02 15:44:16.000000 markdown-to-json-2.0.0/LICENSE
--rw-r--r--   0 njvack     (501) staff       (20)     3898 2023-06-02 15:46:29.726262 markdown-to-json-2.0.0/PKG-INFO
--rw-r--r--   0 njvack     (501) staff       (20)     3657 2023-06-01 18:48:52.000000 markdown-to-json-2.0.0/README.md
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-06-02 15:46:29.723064 markdown-to-json-2.0.0/markdown_to_json/
--rw-r--r--   0 njvack     (501) staff       (20)      377 2023-06-01 18:36:08.000000 markdown-to-json-2.0.0/markdown_to_json/__init__.py
--rw-r--r--   0 njvack     (501) staff       (20)      486 2023-06-02 15:45:31.000000 markdown-to-json-2.0.0/markdown_to_json/_metadata.py
--rw-r--r--   0 njvack     (501) staff       (20)     6270 2023-06-02 15:44:09.000000 markdown-to-json-2.0.0/markdown_to_json/markdown_to_json.py
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-06-02 15:46:29.723788 markdown-to-json-2.0.0/markdown_to_json/scripts/
--rw-r--r--   0 njvack     (501) staff       (20)        0 2023-06-01 14:08:58.000000 markdown-to-json-2.0.0/markdown_to_json/scripts/__init__.py
--rwxr-xr-x   0 njvack     (501) staff       (20)     2767 2023-06-02 15:44:27.000000 markdown-to-json-2.0.0/markdown_to_json/scripts/md_to_json.py
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-06-02 15:46:29.723888 markdown-to-json-2.0.0/markdown_to_json/vendor/
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-06-02 15:46:29.724730 markdown-to-json-2.0.0/markdown_to_json/vendor/CommonMark/
--rwxr-xr-x   0 njvack     (501) staff       (20)    54960 2023-06-01 14:12:35.000000 markdown-to-json-2.0.0/markdown_to_json/vendor/CommonMark/CommonMark.py
--rw-r--r--   0 njvack     (501) staff       (20)      172 2023-06-01 14:08:58.000000 markdown-to-json-2.0.0/markdown_to_json/vendor/CommonMark/__init__.py
--rwxr-xr-x   0 njvack     (501) staff       (20)    62427 2023-06-01 14:08:58.000000 markdown-to-json-2.0.0/markdown_to_json/vendor/CommonMark/entitytrans.py
--rw-r--r--   0 njvack     (501) staff       (20)        0 2023-06-01 14:08:58.000000 markdown-to-json-2.0.0/markdown_to_json/vendor/__init__.py
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-06-02 15:46:29.724985 markdown-to-json-2.0.0/markdown_to_json/vendor/docopt/
--rw-r--r--   0 njvack     (501) staff       (20)       62 2023-06-01 14:08:58.000000 markdown-to-json-2.0.0/markdown_to_json/vendor/docopt/__init__.py
--rw-r--r--   0 njvack     (501) staff       (20)    19542 2023-06-01 14:08:58.000000 markdown-to-json-2.0.0/markdown_to_json/vendor/docopt/docopt.py
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-06-02 15:46:29.725216 markdown-to-json-2.0.0/markdown_to_json/vendor/ordereddict/
--rw-r--r--   0 njvack     (501) staff       (20)      134 2023-06-01 14:08:58.000000 markdown-to-json-2.0.0/markdown_to_json/vendor/ordereddict/__init__.py
--rw-r--r--   0 njvack     (501) staff       (20)     4198 2023-06-01 14:08:58.000000 markdown-to-json-2.0.0/markdown_to_json/vendor/ordereddict/ordereddict.py
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-06-02 15:46:29.723596 markdown-to-json-2.0.0/markdown_to_json.egg-info/
--rw-r--r--   0 njvack     (501) staff       (20)     3898 2023-06-02 15:46:29.000000 markdown-to-json-2.0.0/markdown_to_json.egg-info/PKG-INFO
--rw-r--r--   0 njvack     (501) staff       (20)      939 2023-06-02 15:46:29.000000 markdown-to-json-2.0.0/markdown_to_json.egg-info/SOURCES.txt
--rw-r--r--   0 njvack     (501) staff       (20)        1 2023-06-02 15:46:29.000000 markdown-to-json-2.0.0/markdown_to_json.egg-info/dependency_links.txt
--rw-r--r--   0 njvack     (501) staff       (20)       72 2023-06-02 15:46:29.000000 markdown-to-json-2.0.0/markdown_to_json.egg-info/entry_points.txt
--rw-r--r--   0 njvack     (501) staff       (20)       23 2023-06-02 15:46:29.000000 markdown-to-json-2.0.0/markdown_to_json.egg-info/top_level.txt
--rw-r--r--   0 njvack     (501) staff       (20)     3631 2023-06-01 18:22:32.000000 markdown-to-json-2.0.0/pyproject.toml
--rw-r--r--   0 njvack     (501) staff       (20)       38 2023-06-02 15:46:29.726398 markdown-to-json-2.0.0/setup.cfg
--rwxr-xr-x   0 njvack     (501) staff       (20)     1194 2023-06-01 18:22:32.000000 markdown-to-json-2.0.0/setup.py
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-06-02 15:46:29.726122 markdown-to-json-2.0.0/tests/
--rw-r--r--   0 njvack     (501) staff       (20)        0 2023-06-01 14:08:58.000000 markdown-to-json-2.0.0/tests/__init__.py
--rw-r--r--   0 njvack     (501) staff       (20)     1181 2023-06-01 18:22:32.000000 markdown-to-json-2.0.0/tests/test_example_files.py
--rw-r--r--   0 njvack     (501) staff       (20)      721 2023-06-02 15:44:14.000000 markdown-to-json-2.0.0/tests/test_lists.py
--rw-r--r--   0 njvack     (501) staff       (20)     1713 2023-06-01 18:22:32.000000 markdown-to-json-2.0.0/tests/test_mixed_content.py
--rw-r--r--   0 njvack     (501) staff       (20)      403 2023-06-01 18:44:42.000000 markdown-to-json-2.0.0/tests/test_sugar_methods.py
--rw-r--r--   0 njvack     (501) staff       (20)     1061 2023-06-01 18:22:32.000000 markdown-to-json-2.0.0/tests/test_unicode.py
--rw-r--r--   0 njvack     (501) staff       (20)      464 2023-06-01 14:08:58.000000 markdown-to-json-2.0.0/tests/util.py
+-rw-r--r--   0        0        0     1118 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3406 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/README.md
+-rw-r--r--   0        0        0      265 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/__main__.py
+-rw-r--r--   0        0        0      486 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/_metadata.py
+-rw-r--r--   0        0        0     6249 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/markdown_to_json.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/scripts/__init__.py
+-rwxr-xr-x   0        0        0     2767 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/scripts/md_to_json.py
+-rwxr-xr-x   0        0        0    54960 2023-06-04 16:55:29.960157 markdown_to_json-2.1.0/markdown_to_json/vendor/CommonMark/CommonMark.py
+-rwxr-xr-x   0        0        0     1645 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/vendor/CommonMark/LICENSE
+-rwxr-xr-x   0        0        0     3735 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/vendor/CommonMark/README.md
+-rw-r--r--   0        0        0      172 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/vendor/CommonMark/__init__.py
+-rwxr-xr-x   0        0        0    62427 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/vendor/CommonMark/entitytrans.py
+-rwxr-xr-x   0        0        0     6684 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/vendor/CommonMark/test/test-CommonMark.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/vendor/__init__.py
+-rw-r--r--   0        0        0     1086 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/vendor/docopt/LICENSE-MIT
+-rw-r--r--   0        0        0    33269 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/vendor/docopt/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/vendor/docopt/_version.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/markdown_to_json/vendor/docopt/py.typed
+-rw-r--r--   0        0        0     3501 2023-06-04 16:54:55.819467 markdown_to_json-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4627 1970-01-01 00:00:00.000000 markdown_to_json-2.1.0/PKG-INFO
```

### Comparing `markdown-to-json-2.0.0/LICENSE` & `markdown_to_json-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown-to-json-2.0.0/PKG-INFO` & `markdown_to_json-2.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,78 @@
 Metadata-Version: 2.1
 Name: markdown-to-json
-Version: 2.0.0
-Home-page: https://github.com/njvack/bids-json-writer
+Version: 2.1.0
+Summary: Markdown to dict and json deserializer
+Home-page: https://github.com/njvack/markdown_to_json
+License: MIT
+Keywords: serializer,deserializer,markdown
 Author: Nathan Vack
 Author-email: njvack@wisc.edu
-License: MIT
+Requires-Python: >=3.6.2
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Project-URL: Bug Tracker, https://github.com/njvack/markdown_to_json/issues
+Project-URL: Change Log, https://github.com/njvack/markdown_to_json/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://github.com/njvack/markdown_to_json
+Project-URL: Repository, https://github.com/njvack/markdown_to_json
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Markdown to JSON converter
 
 ## Description
 
-A simple tool to convert Markdown (technically CommonMark) data into JSON. It uses headings as JSON keys, and the stuff following headings as values. Lists are turned into arrays. Higher heading values yield nested JSON keys.
-
-## Why the hell would I want to do this?
+A simple tool to convert Markdown (CommonMark dialect) data into JSON. It uses headings as JSON keys, and the stuff following headings as values. Lists are turned into arrays. Higher heading values yield nested JSON keys.
 
-Sometimes, you need to write JSON. Writing it by hand is a pain. It's a fiddly format and there are strings to escape and commas and it looks bad and you'll have validation errors and yuck. You could build a custom tool to write your particular JSON, but that's a bunch of work. You could use some JSON-specific editor, but they tend to be pretty neckbeard. Sometimes, you maybe just want to open a text editor and pump out a little nested data structure in a human-readable way.
+## Why would you want to do this?
 
-This lets you do that. Markdown is easy.
+If you don't mind the loss of fidelity to the exact Markdown Document Object Model (DOM), you can get a simple python or json datastructure to extract data-like structures from a Markdown document.
 
-As a point of reference, this tool was built to allow easy(-ish) creation of dataset descriptions for the [Brain Imaging Data Structure](http://bids.neuroimaging.io/) data sharing specification.
+This tool was built to allow easy creation of dataset descriptions for the [Brain Imaging Data Structure](http://bids.neuroimaging.io/) data sharing specification.
 
 ## Installation
 
-Easy method:
-
-```
+Non isolated install from pypi
+```bash
 pip install markdown-to-json
+md_to_json --help
 ```
 
-Also easy method:
+Isolated install with pipx if you only want the CLI
+```bash
+pipx install markdown-to-json
+md_to_json --help
+```
+
+Install bleeding edge from github
+```bash
+pip install git+https://github.com/njvack/markdown-to-json/
+python -m markdown_to_json --help
+```
 
 ```bash
 git clone https://github.com/njvack/markdown-to-json.git
 cd markdown_to_json
 ./setup.py install
 ```
 
 The package has no external requirements and has been tested python 3.6+.
 
 Please use version 1 or 1.1 for python 2.x.
 
-You'll get one executable:
-
-## `md_to_json`
+## CLI Usage, `md_to_json`
 
 ```
 Translate markdown into JSON.
 
 Usage:
   md_to_json [options] <markdown_file>
   md_to_json -h | --help
@@ -57,40 +81,32 @@
   -h --help     Show this screen
   --version     Print version number
   -o <file>     Save output to a file instead of stdout
   -i <val>      Indent nested JSON by this amount. Use a negative number for
                 most compact possible JSON. the [default: 2]
 ```
 
-Programmatic usage
+## Programmatic usage
 ```python
 import markdown_to_json
 value = """
 # Nested List
 
 * Item 1
     * Item 1.1
 * Item 2
 """
 
 # The simple way:
-
 dictified = markdown_to_json.dictify(value)
 assert dictified == {'Nested List': ['Item 1', ['Item 1.1'], 'Item 2']}
 
 # Or, if you want a json string
 jsonified = markdown_to_json.jsonify(value)
-
-# The more involved way:
-
-ast = markdown_to_json.CommonMark.DocParser().parse(value)
-tmp = markdown_to_json.CMarkASTNester().nest(ast)  # This contains useless trash
-dictified = dict(markdown_to_json.Renderer().stringify_dict(dictionary))
-
-assert dictified == {'Nested List': ['Item 1', ['Item 1.1'], 'Item 2']}
+assert jsonified == """{"Nested List": ["Item 1", ["Item 1.1"], "Item 2"]}"""
 ```
 
 This translates a markdown document into JSON as described in the example below.
 
 ## Example
 
 The markdown:
@@ -131,14 +147,18 @@
 }
 ```
 
 ## Credits
 
 `markdown_to_json` was written by Nate Vack <njvack@freshforever.net> at the Center for Healthy Minds at the University of Wisconsin–Madison.
 
+Maintenance development by [Matthew Martin](https://github.com/matthewdeanmartin/) 
+
 This tool ships a few really excellent tools in its `vendor` directory:
 
 [docopt](https://github.com/docopt/docopt) is copyright (c) 2012 Vladimir Keleshev, <vladimir@keleshev.com>
 
-[CommonMark-py](https://github.com/rolandshoemaker/CommonMark-py) is copyright Copyright (c) 2014, Bibek Kafle and Roland Shoemaker
+Upgraded to docopt-ng.
+
+[CommonMark-py](https://github.com/rolandshoemaker/CommonMark-py) is copyright Copyright (c) 2014, Bibek Kafle and Roland Shoemaker. 
 
-The packaged ordereddict implementation is copyright (c) 2009 Raymond Hettinger
+Cannot upgrade to 0.6.0 because of breaking changes in AST.
```

### Comparing `markdown-to-json-2.0.0/README.md` & `markdown_to_json-2.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 # Markdown to JSON converter
 
 ## Description
 
-A simple tool to convert Markdown (technically CommonMark) data into JSON. It uses headings as JSON keys, and the stuff following headings as values. Lists are turned into arrays. Higher heading values yield nested JSON keys.
+A simple tool to convert Markdown (CommonMark dialect) data into JSON. It uses headings as JSON keys, and the stuff following headings as values. Lists are turned into arrays. Higher heading values yield nested JSON keys.
 
-## Why the hell would I want to do this?
+## Why would you want to do this?
 
-Sometimes, you need to write JSON. Writing it by hand is a pain. It's a fiddly format and there are strings to escape and commas and it looks bad and you'll have validation errors and yuck. You could build a custom tool to write your particular JSON, but that's a bunch of work. You could use some JSON-specific editor, but they tend to be pretty neckbeard. Sometimes, you maybe just want to open a text editor and pump out a little nested data structure in a human-readable way.
+If you don't mind the loss of fidelity to the exact Markdown Document Object Model (DOM), you can get a simple python or json datastructure to extract data-like structures from a Markdown document.
 
-This lets you do that. Markdown is easy.
-
-As a point of reference, this tool was built to allow easy(-ish) creation of dataset descriptions for the [Brain Imaging Data Structure](http://bids.neuroimaging.io/) data sharing specification.
+This tool was built to allow easy creation of dataset descriptions for the [Brain Imaging Data Structure](http://bids.neuroimaging.io/) data sharing specification.
 
 ## Installation
 
-Easy method:
-
-```
+Non isolated install from pypi
+```bash
 pip install markdown-to-json
+md_to_json --help
 ```
 
-Also easy method:
+Isolated install with pipx if you only want the CLI
+```bash
+pipx install markdown-to-json
+md_to_json --help
+```
+
+Install bleeding edge from github
+```bash
+pip install git+https://github.com/njvack/markdown-to-json/
+python -m markdown_to_json --help
+```
 
 ```bash
 git clone https://github.com/njvack/markdown-to-json.git
 cd markdown_to_json
 ./setup.py install
 ```
 
 The package has no external requirements and has been tested python 3.6+.
 
 Please use version 1 or 1.1 for python 2.x.
 
-You'll get one executable:
-
-## `md_to_json`
+## CLI Usage, `md_to_json`
 
 ```
 Translate markdown into JSON.
 
 Usage:
   md_to_json [options] <markdown_file>
   md_to_json -h | --help
@@ -47,40 +53,32 @@
   -h --help     Show this screen
   --version     Print version number
   -o <file>     Save output to a file instead of stdout
   -i <val>      Indent nested JSON by this amount. Use a negative number for
                 most compact possible JSON. the [default: 2]
 ```
 
-Programmatic usage
+## Programmatic usage
 ```python
 import markdown_to_json
 value = """
 # Nested List
 
 * Item 1
     * Item 1.1
 * Item 2
 """
 
 # The simple way:
-
 dictified = markdown_to_json.dictify(value)
 assert dictified == {'Nested List': ['Item 1', ['Item 1.1'], 'Item 2']}
 
 # Or, if you want a json string
 jsonified = markdown_to_json.jsonify(value)
-
-# The more involved way:
-
-ast = markdown_to_json.CommonMark.DocParser().parse(value)
-tmp = markdown_to_json.CMarkASTNester().nest(ast)  # This contains useless trash
-dictified = dict(markdown_to_json.Renderer().stringify_dict(dictionary))
-
-assert dictified == {'Nested List': ['Item 1', ['Item 1.1'], 'Item 2']}
+assert jsonified == """{"Nested List": ["Item 1", ["Item 1.1"], "Item 2"]}"""
 ```
 
 This translates a markdown document into JSON as described in the example below.
 
 ## Example
 
 The markdown:
@@ -121,14 +119,18 @@
 }
 ```
 
 ## Credits
 
 `markdown_to_json` was written by Nate Vack <njvack@freshforever.net> at the Center for Healthy Minds at the University of Wisconsin–Madison.
 
+Maintenance development by [Matthew Martin](https://github.com/matthewdeanmartin/) 
+
 This tool ships a few really excellent tools in its `vendor` directory:
 
 [docopt](https://github.com/docopt/docopt) is copyright (c) 2012 Vladimir Keleshev, <vladimir@keleshev.com>
 
-[CommonMark-py](https://github.com/rolandshoemaker/CommonMark-py) is copyright Copyright (c) 2014, Bibek Kafle and Roland Shoemaker
+Upgraded to docopt-ng.
+
+[CommonMark-py](https://github.com/rolandshoemaker/CommonMark-py) is copyright Copyright (c) 2014, Bibek Kafle and Roland Shoemaker. 
 
-The packaged ordereddict implementation is copyright (c) 2009 Raymond Hettinger
+Cannot upgrade to 0.6.0 because of breaking changes in AST.
```

### Comparing `markdown-to-json-2.0.0/markdown_to_json/markdown_to_json.py` & `markdown_to_json-2.1.0/markdown_to_json/markdown_to_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,20 +42,20 @@
 strings, lists, or OrderedDicts as values.
 """
 
 from __future__ import absolute_import, unicode_literals
 
 import json
 import operator
+from collections import OrderedDict
 from functools import reduce
 from typing import Any, Dict, List, Optional, Union
 
 from .vendor import CommonMark
 from .vendor.CommonMark.CommonMark import Block
-from .vendor.ordereddict import OrderedDict
 
 
 def dictify(markdown_str: str):
     """
     Turn a markdown string into a nested python dict
     Really, just a little semantic sugar
     """
@@ -100,15 +100,14 @@
         splitted = dictify_list_by(blocks, matches_heading)
         for heading, nests in splitted.items():
             splitted[heading] = self._dictify_blocks(nests, heading_level + 1)
         return splitted
 
     def _ensure_list_singleton(self, blocks):
         """Make sure lists don't mix content"""
-        pass
 
 
 class ContentError(ValueError):
     """Content Error"""
 
 
 def dictify_list_by(list_of_blocks: List[Any], filter_function) -> Dict[Any, Any]:
```

### Comparing `markdown-to-json-2.0.0/markdown_to_json/scripts/md_to_json.py` & `markdown_to_json-2.1.0/markdown_to_json/scripts/md_to_json.py`

 * *Files identical despite different names*

### Comparing `markdown-to-json-2.0.0/markdown_to_json/vendor/CommonMark/CommonMark.py` & `markdown_to_json-2.1.0/markdown_to_json/vendor/CommonMark/CommonMark.py`

 * *Files identical despite different names*

### Comparing `markdown-to-json-2.0.0/markdown_to_json/vendor/CommonMark/entitytrans.py` & `markdown_to_json-2.1.0/markdown_to_json/vendor/CommonMark/entitytrans.py`

 * *Files identical despite different names*

### Comparing `markdown-to-json-2.0.0/pyproject.toml` & `markdown_to_json-2.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "markdown_to_json"
-version = "2.0.0"
-description = "Lossy python to markdown serializer"
+version = "2.1.0"
+description = "Markdown to dict and json deserializer"
 
 authors = ["Nathan Vack <njvack@wisc.edu>"]
 keywords = ["serializer", "deserializer", "markdown",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -30,33 +30,36 @@
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/njvack/markdown_to_json"
 homepage = "https://github.com/njvack/markdown_to_json"
 documentation ="https://github.com/njvack/markdown_to_json"
 
 [tool.poetry.urls]
-"Bug Tracker" = "https://github.com/matthewdeanmartin/markdown_to_json/issues"
-"Change Log" = "https://github.com/matthewdeanmartin/markdown_to_json/blob/main/CHANGES.md"
+"Bug Tracker" = "https://github.com/njvack/markdown_to_json/issues"
+"Change Log" = "https://github.com/njvack/markdown_to_json/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = ">3"
+python = ">=3.6.2"
 
 [tool.poetry.dev-dependencies]
 pytest-cov = "*"
 pytest = "*"
 vermin = "*"
 tox = "*"
 isort = "*"
 bandit = "*"
 black = "*"
 pylint = "*"
 ruff = "*"
 mypy = "*"
 pre-commit = "*"
 
+[tool.poetry.scripts]
+md_to_json = 'markdown_to_json.scripts.md_to_json:main'
+
 [tool.black]
 line-length = 120
 target-version = ['py39']
 include = '\.pyi?$'
 exclude = '''
 
 (
@@ -83,19 +86,15 @@
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = [
     "tests",
 ]
 junit_family = "xunit1"
 norecursedirs = ["vendor", "scripts"]
-# don't know how to do this in toml
-#addopts = "--strict-markers"
-#markers =
-#	slow: marks tests as slow (deselect with '-m "not slow"')
-#	fast: marks tests as fast (deselect with '-m "not fast"')
+
 
 [tool.isort]
 default_section = "THIRDPARTY"
 force_grid_wrap = 0
 include_trailing_comma = true
 known_first_party = ["markdown_to_json"]
 line_length = 88
```

