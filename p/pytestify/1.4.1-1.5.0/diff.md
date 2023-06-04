# Comparing `tmp/pytestify-1.4.1.tar.gz` & `tmp/pytestify-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestify-1.4.1.tar", last modified: Wed May 18 06:06:25 2022, max compression
+gzip compressed data, was "pytestify-1.5.0.tar", last modified: Sun Jun  4 02:02:53 2023, max compression
```

## Comparing `pytestify-1.4.1.tar` & `pytestify-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 danny      (501) staff       (20)        0 2022-05-18 06:06:25.637215 pytestify-1.4.1/
--rw-r--r--   0 danny      (501) staff       (20)     1056 2021-07-19 02:36:52.000000 pytestify-1.4.1/LICENSE
--rw-r--r--   0 danny      (501) staff       (20)     5590 2022-05-18 06:06:25.637500 pytestify-1.4.1/PKG-INFO
--rw-r--r--   0 danny      (501) staff       (20)     4848 2022-05-17 23:29:27.000000 pytestify-1.4.1/README.md
-drwxr-xr-x   0 danny      (501) staff       (20)        0 2022-05-18 06:06:25.622120 pytestify-1.4.1/pytestify/
--rw-r--r--   0 danny      (501) staff       (20)        0 2021-07-19 02:36:52.000000 pytestify-1.4.1/pytestify/__init__.py
--rw-r--r--   0 danny      (501) staff       (20)      114 2022-03-16 03:26:18.000000 pytestify-1.4.1/pytestify/__main__.py
--rw-r--r--   0 danny      (501) staff       (20)      967 2022-03-16 04:10:02.000000 pytestify-1.4.1/pytestify/_ast_helpers.py
--rw-r--r--   0 danny      (501) staff       (20)     3085 2022-05-17 23:29:27.000000 pytestify-1.4.1/pytestify/_main.py
--rw-r--r--   0 danny      (501) staff       (20)     1539 2022-05-18 05:19:12.000000 pytestify-1.4.1/pytestify/_token_helpers.py
-drwxr-xr-x   0 danny      (501) staff       (20)        0 2022-05-18 06:06:25.636428 pytestify-1.4.1/pytestify/fixes/
--rw-r--r--   0 danny      (501) staff       (20)        0 2021-07-19 02:36:52.000000 pytestify-1.4.1/pytestify/fixes/__init__.py
--rw-r--r--   0 danny      (501) staff       (20)    13327 2022-05-18 05:19:52.000000 pytestify-1.4.1/pytestify/fixes/asserts.py
--rw-r--r--   0 danny      (501) staff       (20)     2001 2022-05-17 23:29:25.000000 pytestify-1.4.1/pytestify/fixes/base_class.py
--rw-r--r--   0 danny      (501) staff       (20)     2353 2022-03-16 03:26:18.000000 pytestify-1.4.1/pytestify/fixes/funcs.py
--rw-r--r--   0 danny      (501) staff       (20)     1234 2022-03-16 03:26:18.000000 pytestify-1.4.1/pytestify/fixes/imports.py
--rw-r--r--   0 danny      (501) staff       (20)     1599 2022-03-16 03:26:18.000000 pytestify-1.4.1/pytestify/fixes/method_name.py
-drwxr-xr-x   0 danny      (501) staff       (20)        0 2022-05-18 06:06:25.626368 pytestify-1.4.1/pytestify.egg-info/
--rw-r--r--   0 danny      (501) staff       (20)     5590 2022-05-18 06:06:24.000000 pytestify-1.4.1/pytestify.egg-info/PKG-INFO
--rw-r--r--   0 danny      (501) staff       (20)      521 2022-05-18 06:06:25.000000 pytestify-1.4.1/pytestify.egg-info/SOURCES.txt
--rw-r--r--   0 danny      (501) staff       (20)        1 2022-05-18 06:06:24.000000 pytestify-1.4.1/pytestify.egg-info/dependency_links.txt
--rw-r--r--   0 danny      (501) staff       (20)       51 2022-05-18 06:06:25.000000 pytestify-1.4.1/pytestify.egg-info/entry_points.txt
--rw-r--r--   0 danny      (501) staff       (20)       19 2022-05-18 06:06:25.000000 pytestify-1.4.1/pytestify.egg-info/requires.txt
--rw-r--r--   0 danny      (501) staff       (20)       10 2022-05-18 06:06:25.000000 pytestify-1.4.1/pytestify.egg-info/top_level.txt
--rw-r--r--   0 danny      (501) staff       (20)     1155 2022-05-18 06:06:25.639035 pytestify-1.4.1/setup.cfg
--rw-r--r--   0 danny      (501) staff       (20)       74 2022-03-16 03:26:18.000000 pytestify-1.4.1/setup.py
+drwxr-xr-x   0 danny      (502) staff       (20)        0 2023-06-04 02:02:53.044812 pytestify-1.5.0/
+-rw-r--r--   0 danny      (502) staff       (20)     1056 2023-06-04 00:22:30.000000 pytestify-1.5.0/LICENSE
+-rw-r--r--   0 danny      (502) staff       (20)     5389 2023-06-04 02:02:53.044858 pytestify-1.5.0/PKG-INFO
+-rw-r--r--   0 danny      (502) staff       (20)     4848 2023-06-04 00:22:30.000000 pytestify-1.5.0/README.md
+drwxr-xr-x   0 danny      (502) staff       (20)        0 2023-06-04 02:02:53.043057 pytestify-1.5.0/pytestify/
+-rw-r--r--   0 danny      (502) staff       (20)        0 2023-06-04 00:22:30.000000 pytestify-1.5.0/pytestify/__init__.py
+-rw-r--r--   0 danny      (502) staff       (20)      114 2023-06-04 00:22:30.000000 pytestify-1.5.0/pytestify/__main__.py
+-rw-r--r--   0 danny      (502) staff       (20)      967 2023-06-04 00:22:30.000000 pytestify-1.5.0/pytestify/_ast_helpers.py
+-rw-r--r--   0 danny      (502) staff       (20)     3085 2023-06-04 00:22:30.000000 pytestify-1.5.0/pytestify/_main.py
+-rw-r--r--   0 danny      (502) staff       (20)     1539 2023-06-04 00:22:30.000000 pytestify-1.5.0/pytestify/_token_helpers.py
+drwxr-xr-x   0 danny      (502) staff       (20)        0 2023-06-04 02:02:53.044577 pytestify-1.5.0/pytestify/fixes/
+-rw-r--r--   0 danny      (502) staff       (20)        0 2023-06-04 00:22:30.000000 pytestify-1.5.0/pytestify/fixes/__init__.py
+-rw-r--r--   0 danny      (502) staff       (20)    13861 2023-06-04 02:00:19.000000 pytestify-1.5.0/pytestify/fixes/asserts.py
+-rw-r--r--   0 danny      (502) staff       (20)     2001 2023-06-04 00:22:30.000000 pytestify-1.5.0/pytestify/fixes/base_class.py
+-rw-r--r--   0 danny      (502) staff       (20)     2353 2023-06-04 00:22:30.000000 pytestify-1.5.0/pytestify/fixes/funcs.py
+-rw-r--r--   0 danny      (502) staff       (20)     1234 2023-06-04 00:22:30.000000 pytestify-1.5.0/pytestify/fixes/imports.py
+-rw-r--r--   0 danny      (502) staff       (20)     1599 2023-06-04 00:22:30.000000 pytestify-1.5.0/pytestify/fixes/method_name.py
+drwxr-xr-x   0 danny      (502) staff       (20)        0 2023-06-04 02:02:53.043789 pytestify-1.5.0/pytestify.egg-info/
+-rw-r--r--   0 danny      (502) staff       (20)     5389 2023-06-04 02:02:53.000000 pytestify-1.5.0/pytestify.egg-info/PKG-INFO
+-rw-r--r--   0 danny      (502) staff       (20)      540 2023-06-04 02:02:53.000000 pytestify-1.5.0/pytestify.egg-info/SOURCES.txt
+-rw-r--r--   0 danny      (502) staff       (20)        1 2023-06-04 02:02:53.000000 pytestify-1.5.0/pytestify.egg-info/dependency_links.txt
+-rw-r--r--   0 danny      (502) staff       (20)       51 2023-06-04 02:02:53.000000 pytestify-1.5.0/pytestify.egg-info/entry_points.txt
+-rw-r--r--   0 danny      (502) staff       (20)       19 2023-06-04 02:02:53.000000 pytestify-1.5.0/pytestify.egg-info/requires.txt
+-rw-r--r--   0 danny      (502) staff       (20)       10 2023-06-04 02:02:53.000000 pytestify-1.5.0/pytestify.egg-info/top_level.txt
+-rw-r--r--   0 danny      (502) staff       (20)      999 2023-06-04 02:02:53.045107 pytestify-1.5.0/setup.cfg
+-rw-r--r--   0 danny      (502) staff       (20)       74 2023-06-04 00:22:30.000000 pytestify-1.5.0/setup.py
+drwxr-xr-x   0 danny      (502) staff       (20)        0 2023-06-04 02:02:53.044709 pytestify-1.5.0/tests/
+-rw-r--r--   0 danny      (502) staff       (20)     1498 2023-06-04 00:22:30.000000 pytestify-1.5.0/tests/test_main.py
```

### Comparing `pytestify-1.4.1/LICENSE` & `pytestify-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestify-1.4.1/PKG-INFO` & `pytestify-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: pytestify
-Version: 1.4.1
+Version: 1.5.0
 Summary: Automatically convert unittests to pytest
 Home-page: https://github.com/dannysepler/pytestify
 Author: Danny Sepler
 Author-email: dannysepler@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dannysepler/pytestify/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pytestify
 =========
```

### Comparing `pytestify-1.4.1/README.md` & `pytestify-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pytestify-1.4.1/pytestify/_ast_helpers.py` & `pytestify-1.5.0/pytestify/_ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pytestify-1.4.1/pytestify/_main.py` & `pytestify-1.5.0/pytestify/_main.py`

 * *Files identical despite different names*

### Comparing `pytestify-1.4.1/pytestify/_token_helpers.py` & `pytestify-1.5.0/pytestify/_token_helpers.py`

 * *Files identical despite different names*

### Comparing `pytestify-1.4.1/pytestify/fixes/asserts.py` & `pytestify-1.5.0/pytestify/fixes/asserts.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 @dataclass
 class Call:
     name: str
     line: int
     token_idx: int
     end_line: int
     commas: list[Token]
+    comments: list[Token]
     keywords: list[ast.keyword]
     places: int | None = None
     delta: int | None = None
     offset: int = 0
     kwargs: dict[str, str] = field(default_factory=dict)
 
     @property
@@ -134,14 +135,18 @@
 
         line = call.lineno
         call_idx = next(
             tok_no for tok_no, tok in enumerate(self.tokens)
             if tok.src == method and tok.line == line
         )
 
+        comments = [
+            t for i, t in enumerate(self.tokens)
+            if i >= call_idx and t.name == 'COMMENT'
+        ]
         operators = [
             t for i, t in enumerate(self.tokens)
             if i >= call_idx and t.name == 'OP'
         ]
         open_paren = next(t for t in operators if t.src == '(')
         commas = [
             find_outer_comma(operators, comma_no=1),
@@ -173,30 +178,31 @@
         end_line = close_paren.line
         self.calls.append(
             Call(
                 name=method,
                 line=line - 1,
                 token_idx=call_idx,
                 end_line=end_line - 1,
+                comments=comments,
                 commas=commas,
                 keywords=call.keywords,
                 **kwargs
             ),
         )
 
 
 def rewrite_parens(
     operators: list[Token],
     call: Call,
     content_list: list[str],
     comma: Token | None,
 ) -> bool:
     '''
-    For single line asserts, remove parantheses
-    For multi-line asserts, convert parantheses to slashes
+    For single line asserts, remove parentheses
+    For multi-line asserts, convert parentheses to slashes
     '''
     open_paren = next(t for t in operators if t.src == '(')
     closing_paren = find_closing_paren(open_paren, operators)
 
     start_line = content_list[call.line]
     start_line = remove_token(start_line, open_paren, offset=call.offset)
     content_list[call.line] = start_line
@@ -226,14 +232,24 @@
         call.end_line -= 1
         return True
     else:
         return False
 
 
 def add_suffix(call: Call, content_list: list[str], suffix: str) -> None:
+    for comment in call.comments:
+        if (
+            call.end_line == comment.line - 1
+            and comment.src in content_list[call.end_line]
+        ):
+            content_list[call.end_line] = (
+                content_list[call.end_line].replace(comment.src, '').rstrip()
+            )
+            suffix += ' ' + comment.src
+
     second_comma = call.commas[1]
     if second_comma:
         # The suffix should be added BEFORE a second comma, such as...
         # self.assertCountEqual(a, b, 'my error')
         #
         # should be...
         # assert sorted(a) == sorted(b), 'my error'
```

### Comparing `pytestify-1.4.1/pytestify/fixes/base_class.py` & `pytestify-1.5.0/pytestify/fixes/base_class.py`

 * *Files identical despite different names*

### Comparing `pytestify-1.4.1/pytestify/fixes/funcs.py` & `pytestify-1.5.0/pytestify/fixes/funcs.py`

 * *Files identical despite different names*

### Comparing `pytestify-1.4.1/pytestify/fixes/imports.py` & `pytestify-1.5.0/pytestify/fixes/imports.py`

 * *Files identical despite different names*

### Comparing `pytestify-1.4.1/pytestify/fixes/method_name.py` & `pytestify-1.5.0/pytestify/fixes/method_name.py`

 * *Files identical despite different names*

### Comparing `pytestify-1.4.1/pytestify.egg-info/PKG-INFO` & `pytestify-1.5.0/pytestify.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: pytestify
-Version: 1.4.1
+Version: 1.5.0
 Summary: Automatically convert unittests to pytest
 Home-page: https://github.com/dannysepler/pytestify
 Author: Danny Sepler
 Author-email: dannysepler@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dannysepler/pytestify/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pytestify
 =========
```

### Comparing `pytestify-1.4.1/setup.cfg` & `pytestify-1.5.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 [metadata]
 name = pytestify
-version = 1.4.1
+version = 1.5.0
 description = Automatically convert unittests to pytest
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/dannysepler/pytestify
 author = Danny Sepler
 author_email = dannysepler@gmail.com
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 project_urls = 
 	Bug Tracker = https://github.com/dannysepler/pytestify/issues
 
 [options]
 packages = find:
 install_requires = 
 	tokenize-rt>=4.0.0
```

