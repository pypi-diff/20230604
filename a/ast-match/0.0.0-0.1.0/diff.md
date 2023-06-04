# Comparing `tmp/ast-match-0.0.0.tar.gz` & `tmp/ast-match-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ast-match-0.0.0.tar", last modified: Sun Jun  4 13:46:01 2023, max compression
+gzip compressed data, was "ast-match-0.1.0.tar", last modified: Sun Jun  4 15:26:41 2023, max compression
```

## Comparing `ast-match-0.0.0.tar` & `ast-match-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-04 13:46:01.017707 ast-match-0.0.0/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1821 2023-06-04 09:58:25.000000 ast-match-0.0.0/.gitignore
--rw-r--r--   0 user202729  (1000) user202729  (1000)    35149 2023-06-03 08:51:03.000000 ast-match-0.0.0/LICENSE
--rw-r--r--   0 user202729  (1000) user202729  (1000)     4909 2023-06-04 13:46:01.017707 ast-match-0.0.0/PKG-INFO
--rw-r--r--   0 user202729  (1000) user202729  (1000)     4385 2023-06-04 10:57:40.000000 ast-match-0.0.0/README.md
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-04 13:46:01.017707 ast-match-0.0.0/ast_match/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     6861 2023-06-04 10:33:43.000000 ast-match-0.0.0/ast_match/__init__.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)      326 2023-06-03 08:56:41.000000 ast-match-0.0.0/ast_match/parse.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     3601 2023-06-03 10:35:34.000000 ast-match-0.0.0/ast_match/pattern.py
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-04 13:46:01.017707 ast-match-0.0.0/ast_match.egg-info/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     4909 2023-06-04 13:46:00.000000 ast-match-0.0.0/ast_match.egg-info/PKG-INFO
--rw-r--r--   0 user202729  (1000) user202729  (1000)      280 2023-06-04 13:46:00.000000 ast-match-0.0.0/ast_match.egg-info/SOURCES.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2023-06-04 13:46:00.000000 ast-match-0.0.0/ast_match.egg-info/dependency_links.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)       10 2023-06-04 13:46:00.000000 ast-match-0.0.0/ast_match.egg-info/top_level.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2023-06-03 09:06:01.000000 ast-match-0.0.0/ast_match.egg-info/zip-safe
--rw-r--r--   0 user202729  (1000) user202729  (1000)       69 2023-06-04 10:08:42.000000 ast-match-0.0.0/pytest.ini
--rw-r--r--   0 user202729  (1000) user202729  (1000)      606 2023-06-04 13:46:01.017707 ast-match-0.0.0/setup.cfg
--rw-r--r--   0 user202729  (1000) user202729  (1000)       38 2023-06-03 09:05:26.000000 ast-match-0.0.0/setup.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-04 15:26:41.094521 ast-match-0.1.0/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1821 2023-06-04 09:58:25.000000 ast-match-0.1.0/.gitignore
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      339 2023-06-04 15:15:02.000000 ast-match-0.1.0/INTERNAL.md
+-rw-r--r--   0 user202729  (1000) user202729  (1000)    35149 2023-06-03 08:51:03.000000 ast-match-0.1.0/LICENSE
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     5467 2023-06-04 15:26:41.094521 ast-match-0.1.0/PKG-INFO
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     4943 2023-06-04 15:06:27.000000 ast-match-0.1.0/README.md
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-04 15:26:41.087854 ast-match-0.1.0/ast_match/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     9039 2023-06-04 15:25:34.000000 ast-match-0.1.0/ast_match/__init__.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     4856 2023-06-04 15:09:50.000000 ast-match-0.1.0/ast_match/_pattern.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-04 15:26:41.087854 ast-match-0.1.0/ast_match.egg-info/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     5467 2023-06-04 15:26:40.000000 ast-match-0.1.0/ast_match.egg-info/PKG-INFO
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      391 2023-06-04 15:26:40.000000 ast-match-0.1.0/ast_match.egg-info/SOURCES.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2023-06-04 15:26:40.000000 ast-match-0.1.0/ast_match.egg-info/dependency_links.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       10 2023-06-04 15:26:40.000000 ast-match-0.1.0/ast_match.egg-info/top_level.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2023-06-03 09:06:01.000000 ast-match-0.1.0/ast_match.egg-info/zip-safe
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-04 15:26:41.091188 ast-match-0.1.0/docs/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      638 2023-06-04 15:14:12.000000 ast-match-0.1.0/docs/Makefile
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      152 2023-06-04 15:19:18.000000 ast-match-0.1.0/docs/ast_match.rst
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1266 2023-06-04 15:16:25.000000 ast-match-0.1.0/docs/conf.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      456 2023-06-04 15:14:36.000000 ast-match-0.1.0/docs/index.rst
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      804 2023-06-04 15:14:12.000000 ast-match-0.1.0/docs/make.bat
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-04 15:26:41.094521 ast-match-0.1.0/docs/source/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      922 2023-06-04 15:14:12.000000 ast-match-0.1.0/docs/source/conf.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      443 2023-06-04 15:14:12.000000 ast-match-0.1.0/docs/source/index.rst
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       89 2023-06-04 15:17:45.000000 ast-match-0.1.0/pytest.ini
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      606 2023-06-04 15:26:41.094521 ast-match-0.1.0/setup.cfg
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       38 2023-06-03 09:05:26.000000 ast-match-0.1.0/setup.py
```

### Comparing `ast-match-0.0.0/.gitignore` & `ast-match-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ast-match-0.0.0/LICENSE` & `ast-match-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ast-match-0.0.0/PKG-INFO` & `ast-match-0.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-Metadata-Version: 2.1
-Name: ast-match
-Version: 0.0.0
-Summary: A library to facilitate easier manipulation of Python AST (abstract syntax tree) objects.
-Home-page: https://github.com/user202729/ast-match
-Author: user202729
-License: GNU General Public License v3 or later (GPLv3+)
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ast-match
 
 A library to facilitate easier manipulation of Python AST (abstract syntax tree) objects.
 
 This library allows you to write the syntax in an intuitive way, instead of having to write the names of the internal classes in `ast` module.
 
 For manipulating the internal structure, it's recommended to read through https://docs.python.org/3/library/ast.html to know what kind of nodes may appear in an AST.
 
+It's recommended to read through these at least once (as well as linked documentations at the bottom of the page) at least once,
+it will save you lots of time later on.
+
+### Limitations
+
+This module does not allow you to manipulate the tree in *all possible* ways. For that you still need to tinker with the AST itself.
+
+### Related packages
+
+https://greentreesnakes.readthedocs.io/en/latest/examples.html#real-projects
+
 ### Usage
 
 Import everything (apart from testing purpose it's recommended to avoid `import *`):
 
 ```python
 >>> from ast_match import *
 >>> from pprint import pprint
@@ -75,15 +73,15 @@
 <td> 
 
 ```python
 >>> from ast_match import *
 >>> pattern=compile(expr("_last-1"))
 >>> match=pattern.fullmatch(expr("7*8-1"))
 >>> match
-Matching{'last': <ast.AST: 7 * 8>}
+Match{'last': <ast.AST: 7 * 8>}
 
 ```
 
 </td>
 </tr>
 <tr>
 <td>
@@ -120,16 +118,16 @@
 
 </td>
 <td> 
 
 ```python
 >>> pattern=compile(expr("_a*_b"))
 >>> pprint([*pattern.finditer(expr("1*2+3*4"))])
-[Matching{'a': <ast.AST: 1>, 'b': <ast.AST: 2>},
- Matching{'a': <ast.AST: 3>, 'b': <ast.AST: 4>}]
+[Match{'a': <ast.AST: 1>, 'b': <ast.AST: 2>},
+ Match{'a': <ast.AST: 3>, 'b': <ast.AST: 4>}]
 
 ```
 
 </td>
 </tr>
 </table>
 
@@ -216,7 +214,9 @@
                 left=Name(id='i', ctx=Load()),
                 op=Add(),
                 right=Constant(value=1))],
             keywords=[]))],
       orelse=[])],
   type_ignores=[])
 ```
+
+It may also be desirable to put the code into `.ipython/profile_default/startup/` or similar so that it's run automatically when IPython starts.
```

#### html2text {}

```diff
@@ -1,43 +1,41 @@
-Metadata-Version: 2.1 Name: ast-match Version: 0.0.0 Summary: A library to
-facilitate easier manipulation of Python AST (abstract syntax tree) objects.
-Home-page: https://github.com/user202729/ast-match Author: user202729 License:
-GNU General Public License v3 or later (GPLv3+) Classifier: License :: OSI
-Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Description-Content-Type: text/markdown License-File: LICENSE # ast-match
-A library to facilitate easier manipulation of Python AST (abstract syntax
-tree) objects. This library allows you to write the syntax in an intuitive way,
-instead of having to write the names of the internal classes in `ast` module.
-For manipulating the internal structure, it's recommended to read through
-https://docs.python.org/3/library/ast.html to know what kind of nodes may
-appear in an AST. ### Usage Import everything (apart from testing purpose it's
-recommended to avoid `import *`): ```python >>> from ast_match import * >>>
-from pprint import pprint ``` First, note that Python distinguishes between
-statement and expression, so you need to specify the type explicitly: ```python
->>> expr("a=1") Traceback (most recent call last): ... AssertionError >>> pp
-(stmt("a=1"))
+# ast-match A library to facilitate easier manipulation of Python AST (abstract
+syntax tree) objects. This library allows you to write the syntax in an
+intuitive way, instead of having to write the names of the internal classes in
+`ast` module. For manipulating the internal structure, it's recommended to read
+through https://docs.python.org/3/library/ast.html to know what kind of nodes
+may appear in an AST. It's recommended to read through these at least once (as
+well as linked documentations at the bottom of the page) at least once, it will
+save you lots of time later on. ### Limitations This module does not allow you
+to manipulate the tree in *all possible* ways. For that you still need to
+tinker with the AST itself. ### Related packages https://
+greentreesnakes.readthedocs.io/en/latest/examples.html#real-projects ### Usage
+Import everything (apart from testing purpose it's recommended to avoid `import
+*`): ```python >>> from ast_match import * >>> from pprint import pprint ```
+First, note that Python distinguishes between statement and expression, so you
+need to specify the type explicitly: ```python >>> expr("a=1") Traceback (most
+recent call last): ... AssertionError >>> pp(stmt("a=1"))
 AST: a = 1> ``` Here the `pp` function used to "pretty-print" the resulting
 `ast.AST` object. If you use IPython you may want to refer to the section below
 for automatic pretty-printing. The API somewhat resemble `re` module API:
 `re` module                            `ast_match` module
 ```python >>> import re >>>            ```python >>> from ast_match import *
 pattern=re.compile("(?P.*)-1") >>>     >>> pattern=compile(expr("_last-1")) >>>
 match=pattern.fullmatch("7*8-1") >>>   match=pattern.fullmatch(expr("7*8-1"))
-match.groupdict() {'last': '7*8'} ```  >>> match Matching{'last':
+match.groupdict() {'last': '7*8'} ```  >>> match Match{'last':
                                        AST: 7 * 8>} ```
 ```python >>> pattern=re.compile(r"    ```python >>> pattern=compile(expr("_x *
 (?P\d+)\*(?P\d+)") >>> pattern.sub     _y")) >>> pp(pattern.sub(repl(expr
 (r"\g*\g", "1*2+3*4") '2*1+4*3' ```    ("_y*_x")), expr("1*2+3*4")))
                                        AST: 2 * 1 + 4 * 3> ```
 ```python >>> pattern=re.compile(r"    ```python >>> pattern=compile(expr
 (?P\d+)\*(?P\d+)") >>> pprint(         ("_a*_b")) >>> pprint([*pattern.finditer
-[*pattern.finditer("1*2+3*4")]) [Match (expr("1*2+3*4"))]) [Matching{'a':
+[*pattern.finditer("1*2+3*4")]) [Match (expr("1*2+3*4"))]) [Match{'a':
 object; span=(0, 3), match='1*2'>,     AST: 1>, 'b':
-Match object; span=(4, 7),             AST: 2>}, Matching{'a':
+Match object; span=(4, 7),             AST: 2>}, Match{'a':
 match='3*4'>] ```                      AST: 3>, 'b':
                                        AST: 4>}] ```
 ### Note for Vim users The code inside strings may not be syntax-highlighted as
 Python code. To fix, consider adding the following to `.vim/after/syntax/
 python.vim`: ```vim syn region pythonSpecialInclude1 \ start=+\(expr\|stmt\)
 (r\?\z(['"]\)+ end=+\z1)+ keepend \ contains=pythonSpecialIncludeInner1 syn
 region pythonSpecialIncludeInner1 \ start=+\z(['"]\)\zs+ end=+\ze\z1+ keepend \
@@ -57,8 +55,10 @@
 alternative, prettier but does not show the internal #formatter.pop(ast.AST) #
 revert ``` Then the display will be more readable: ```python In [21]: ast.parse
 ('for i in range(10): print(i, i+1)') Out[21]: Module( body=[ For( target=Name
 (id='i', ctx=Store()), iter=Call( func=Name(id='range', ctx=Load()), args=
 [ Constant(value=10)], keywords=[]), body=[ Expr( value=Call( func=Name
 (id='print', ctx=Load()), args=[ Name(id='i', ctx=Load()), BinOp( left=Name
 (id='i', ctx=Load()), op=Add(), right=Constant(value=1))], keywords=[]))],
-orelse=[])], type_ignores=[]) ```
+orelse=[])], type_ignores=[]) ``` It may also be desirable to put the code into
+`.ipython/profile_default/startup/` or similar so that it's run automatically
+when IPython starts.
```

### Comparing `ast-match-0.0.0/ast_match/__init__.py` & `ast-match-0.1.0/ast_match/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,45 @@
 """
 Main module.
+
+Pattern syntax
+--------------
+
+Refer to :func:`compile`.
 """
 
 from __future__ import annotations
 
 import ast
-from ast_match.parse import parse_statement, parse_expr
-from ast_match.pattern import *
+from ast_match._pattern import *
 from copy import deepcopy
 from typing import Union, Iterator, Callable, Optional
 
 def stmt(code: str)->ast.stmt:
 	r"""
 	Parse code as a statement::
 
 		>>> pp(stmt('a=1'))
 		<ast.AST: a = 1>
 		>>> pp(stmt('for i in range(5): print(i)'))
 		<ast.AST: for i in range(5):
 		    print(i)>
+
+	Note that the resulting code must be a single statement::
+
+		>>> pp(stmt('a=1; b=2'))
+		Traceback (most recent call last):
+			...
+		AssertionError
+
+	If you want to parse multiple statements, consider using ``ast.parse`` directly::
+
+		>>> pp(ast.parse('a=1; b=2'))
+		<ast.AST: a = 1
+		b = 2>
 	"""
 	body=ast.parse(code).body
 	assert len(body)==1
 	assert isinstance(body[0], ast.stmt)
 	return body[0]
 
 def expr(code: str)->ast.expr:
@@ -32,39 +49,48 @@
 		>>> pp(expr('a+b'))
 		<ast.AST: a + b>
 		>>> pp(expr('a=1'))
 		Traceback (most recent call last):
 			...
 		AssertionError
 	"""
-	statement=parse_statement(code)
+	statement=stmt(code)
 	assert isinstance(statement, ast.Expr)
 	return statement.value
 
-def prettyrepr(o: ast.AST)->str:
+def prettyrepr(o: ast.AST|list)->str:
 	"""
 	Pretty print an ``ast.AST`` object. Return a string.
+
+	This function is mainly for internal pytest doctesting only.
+
 	The output should not be considered stable.
 
 	Example::
 
 		>>> prettyrepr(stmt('a=1'))
 		'<ast.AST: a = 1>'
 	"""
-	try: return "<ast.AST: " + ast.unparse(o) + ">"
-	except: return "<ast.AST: " + ast.dump(o, indent=2) + ">"
+	if isinstance(o, list):
+		return "[" + ", ".join(prettyrepr(x) for x in o) + "]"
+	if isinstance(o, ast.AST):
+		try: return "<ast.AST: " + ast.unparse(o) + ">"
+		except: return "<ast.AST: " + ast.dump(o, indent=2) + ">"
+	else:
+		return repr(o)
 
 @dataclass
 class _Prettyprint:
 	repr: str
 	def __repr__(self)->str: return self.repr
 
 def pp(o: ast.AST)->_Prettyprint:
 	"""
 	Pretty print an ``ast.AST`` object (by returning an object whose repr is the specified string).
+
 	This function is mainly for internal pytest doctesting only.
 
 	The output should not be considered stable.
 
 	Example::
 
 		>>> pp(stmt('a=1'))
@@ -76,118 +102,147 @@
 
 _privateconstructonly=_Privateconstructonly()
 
 @dataclass
 class Repl:
 	"""
 	Second argument to :meth:`Pattern.sub` and similar methods.
+
+	Refer to :func:`repl` on how to construct this class.
 	"""
 	_pattern: Pattern0
 
 	def __init__(self, o: _Privateconstructonly, pattern: Pattern0)->None:
 		if o is not _privateconstructonly: raise TypeError("Repl is not constructible directly, use repl() instead")
 		self._pattern=pattern
 
 	def __repr__(self)->str:
 		return "<Repl: " + ast.dump(self._pattern, indent=2) + ">"
 
 
 def repl(node: ast.AST)->Repl:
 	"""
 	Construct a :class:`Repl` object.
+
+	Used as the first argument of :meth:`Pattern.sub` and similar methods.
+
+	The syntax is similar to, but not the same as, :func:`compile`.
+
+	For example::
+
+		>>> pp(compile(stmt('_a=1')).sub(repl(stmt('_a=2')), stmt('b=1')))
+		<ast.AST: b = 2>
+
+	Similar to :func:`compile`, you can also use ``BlankNullSequence``::
+
+		>>> pp(compile(stmt('f(__a)*g(__b)')).sub(repl(stmt('h(__a, 0, __b)')), stmt('f(1, 2)*g(3, 4)')))
+		<ast.AST: h(1, 2, 0, 3, 4)>
 	"""
 	node=deepcopy(node)
 	return Repl(_privateconstructonly, to_pattern_mutable(node))
 
 @dataclass
-class Matching:
+class Match:
 	"""
 	Return type of functions such as :meth:`Pattern.fullmatch`.
 	"""
-	matching: Matching0
+	_matching: Matching0
 
 	def __init__(self, *args, **kwargs):
 		"""
 		Constructor. Example::
 
-			>>> Matching({"a": expr("1")})
-			Matching{'a': <ast.AST: 1>}
-			>>> Matching(a=expr("1"))
-			Matching{'a': <ast.AST: 1>}
+			>>> Match({"a": expr("1")})
+			Match{'a': <ast.AST: 1>}
+			>>> Match(a=expr("1"))
+			Match{'a': <ast.AST: 1>}
 		"""
 		if len(args)==1 and not kwargs:
 			assert isinstance(args[0], dict)
-			self.matching=args[0]
+			self._matching=args[0]
 		else:
 			assert not args
-			self.matching=dict(**kwargs)
+			self._matching=dict(**kwargs)
 
 	def __repr__(self):
 		"""
-		>>> Matching({"a": expr("1")})
-		Matching{'a': <ast.AST: 1>}
+		>>> Match({"a": expr("1")})
+		Match{'a': <ast.AST: 1>}
 		"""
-		return "Matching{" + ", ".join(
-				f"{key!r}: {prettyrepr(value)}" for key, value in self.matching.items()
+		return "Match{" + ", ".join(
+				f"{key!r}: {prettyrepr(value)}" for key, value in self._matching.items()
 				) + "}"
 	
 	def expand(self, o: Repl)->ast.AST:
 		"""
 		Substitute the matched values into the pattern, and return the result.
 
 		Example::
 
-			>>> m=Matching(a=expr("b"))
+			>>> m=Match(a=expr("b"))
 			>>> m
-			Matching{'a': <ast.AST: b>}
+			Match{'a': <ast.AST: b>}
 			>>> pp(m.expand(repl(stmt('_a=1'))))
 			<ast.AST: b = 1>
 
 		As they're ``ast.AST`` objects, nestings etc. are properly handled::
 
-			>>> pp(Matching(a=expr("1*2"), b=expr("3*4")).expand(repl(expr("_a+_b"))))
+			>>> pp(Match(a=expr("1*2"), b=expr("3*4")).expand(repl(expr("_a+_b"))))
 			<ast.AST: 1 * 2 + 3 * 4>
-			>>> pp(Matching(a=expr("1+2"), b=expr("3+4")).expand(repl(expr("_a*_b"))))
+			>>> pp(Match(a=expr("1+2"), b=expr("3+4")).expand(repl(expr("_a*_b"))))
 			<ast.AST: (1 + 2) * (3 + 4)>
-			>>> pp(Matching(body=stmt("print(i)")).expand(repl(stmt("for i in range(n): _body"))))
+			>>> pp(Match(body=stmt("print(i)")).expand(repl(stmt("for i in range(n): _body"))))
 			<ast.AST: for i in range(n):
 			    print(i)>
 
 		"""
 		return pattern_replace_mutable(
-				deepcopy(o._pattern), self.matching)
+				deepcopy(o._pattern), self._matching)
+
+	def __getitem__(self, key: str)->ast.AST|list:
+		"""
+		>>> pp(Match(a=expr("1"))["a"])
+		<ast.AST: 1>
+		"""
+		return self._matching[key]
 
+	def group(self, key: str)->ast.AST|list:
+		"""
+		>>> pp(Match(a=expr("1")).group("a"))
+		<ast.AST: 1>
+		"""
+		return self._matching[key]
 
 @dataclass
 class Pattern:
 	pattern: Pattern0
 
 	def __init__(self, o: _Privateconstructonly, pattern: Pattern0)->None:
 		if o is not _privateconstructonly: raise TypeError("Pattern is not constructible directly, use compile() instead")
 		self._pattern=pattern
 
-	def fullmatch(self, text: ast.AST)->Optional[Matching]:
+	def fullmatch(self, text: ast.AST)->Optional[Match]:
 		r"""
 		Match this pattern against the provided text::
 
 			>>> compile(expr("_last-1")).fullmatch(expr("7*8-1"))
-			Matching{'last': <ast.AST: 7 * 8>}
+			Match{'last': <ast.AST: 7 * 8>}
 		"""
 		match=pattern_match(self._pattern, text)
 		if match is None: return None
-		return Matching(match)
+		return Match(match)
 
-	def finditer(self, text: ast.AST)->Iterator[Matching]:
+	def finditer(self, text: ast.AST)->Iterator[Match]:
 		"""
 		Find all matching occurrences.
 
 		Example::
 
 			>>> [*compile(expr("_a*_b")).finditer(expr("1*2+3*4"))]
-			[Matching{'a': <ast.AST: 1>, 'b': <ast.AST: 2>}, Matching{'a': <ast.AST: 3>, 'b': <ast.AST: 4>}]
+			[Match{'a': <ast.AST: 1>, 'b': <ast.AST: 2>}, Match{'a': <ast.AST: 3>, 'b': <ast.AST: 4>}]
 		"""
 		if isinstance(text, list):
 			for item in text:
 				yield from self.finditer(item)
 
 		elif isinstance(text, ast.AST):
 			# check top level match
@@ -199,27 +254,27 @@
 			for field_name, text0 in ast.iter_fields(text):
 				if isinstance(text0, ast.AST):  # TODO what if text0 is list?
 					yield from self.finditer(text0)
 
 		else:
 			assert False, (self, text)
 
-	def sub(self, replace: Union[ast.AST, Repl, Callable[[ast.AST, Matching], ast.AST]], text: ast.AST)->ast.AST:
+	def sub(self, replace: Union[ast.AST, Repl, Callable[[ast.AST, Match], ast.AST]], text: ast.AST)->ast.AST:
 		"""
 		Replace all occurrences.
 
 		Parameters like ``count`` or functionalities like ``re.subn`` is not supported.
 
-		The *replace* parameter can be an AST, a pattern, or a function that takes the whole match and a :class:`Matching` object and returns an AST.
+		The *replace* parameter can be an AST, a pattern, or a function that takes the whole match and a :class:`Match` object and returns an AST.
 
 		Example::
 
 			>>> pp(compile(expr("1")).sub(expr("2"), expr("1+5+7+1")))
 			<ast.AST: 2 + 5 + 7 + 2>
-			>>> pp(compile(expr("1")).sub(lambda whole, _matching: Matching(x=whole).expand(repl(expr("f(_x)"))), expr("1+5+7+1")))
+			>>> pp(compile(expr("1")).sub(lambda whole, _matching: Match(x=whole).expand(repl(expr("f(_x)"))), expr("1+5+7+1")))
 			<ast.AST: f(1) + 5 + 7 + f(1)>
 			>>> pp(compile(expr("_x*_y")).sub(repl(expr("_y*_x")), expr("2*3+4*5")))
 			<ast.AST: 3 * 2 + 5 * 4>
 		"""
 		#if isinstance(text, list):
 		#	return [self.sub(replace, item) for item in text]
 
@@ -258,11 +313,40 @@
 		>>> compile(stmt('_a=1'))
 		<Pattern: Assign(
 		  targets=[
 		    Blank(var='a')],
 		  value=Constant(value=1))>
 		>>> compile(expr('_a+_b'))
 		<Pattern: BinOp(left=Blank(var='a'), op=Add(), right=Blank(var='b'))>
+
+	A variable prefixed with ``_`` denotes a "blank" i.e. placeholder.
+	The concept of ``Blank`` comes from Mathematica.
+
+	Similarly there's a ``BlankNullSequence``.
+	While a ``Blank`` can only match one item::
+
+		>>> compile(expr("f(_a)")).fullmatch(expr("f(1)"))
+		Match{'a': <ast.AST: 1>}
+		>>> compile(expr("f(_a)")).fullmatch(expr("f(1, 2)")) is None
+		True
+
+	A ``BlankNullSequence`` can match zero or more items::
+
+		>>> compile(expr("f(__a)")).fullmatch(expr("f(1)"))
+		Match{'a': [<ast.AST: 1>]}
+		>>> compile(expr("f(__a)")).fullmatch(expr("f()"))
+		Match{'a': []}
+		>>> compile(expr("f(__a)")).fullmatch(expr("f(1, 2)"))
+		Match{'a': [<ast.AST: 1>, <ast.AST: 2>]}
+
+	Similarly:
+
+		>>> pattern=compile(stmt("for i in range(10): _a"))
+		>>> pattern.fullmatch(stmt("for i in range(10): 1; 2")) is None
+		True
+		>>> pattern=compile(stmt("for i in range(10): __a"))
+		>>> pattern.fullmatch(stmt("for i in range(10): 1; 2"))
+		Match{'a': [<ast.AST: 1>, <ast.AST: 2>]}
 	"""
 	node=deepcopy(node)
 	return Pattern(_privateconstructonly, to_pattern_mutable(node))
```

### Comparing `ast-match-0.0.0/ast_match.egg-info/PKG-INFO` & `ast-match-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ast-match
-Version: 0.0.0
+Version: 0.1.0
 Summary: A library to facilitate easier manipulation of Python AST (abstract syntax tree) objects.
 Home-page: https://github.com/user202729/ast-match
 Author: user202729
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,25 @@
 
 A library to facilitate easier manipulation of Python AST (abstract syntax tree) objects.
 
 This library allows you to write the syntax in an intuitive way, instead of having to write the names of the internal classes in `ast` module.
 
 For manipulating the internal structure, it's recommended to read through https://docs.python.org/3/library/ast.html to know what kind of nodes may appear in an AST.
 
+It's recommended to read through these at least once (as well as linked documentations at the bottom of the page) at least once,
+it will save you lots of time later on.
+
+### Limitations
+
+This module does not allow you to manipulate the tree in *all possible* ways. For that you still need to tinker with the AST itself.
+
+### Related packages
+
+https://greentreesnakes.readthedocs.io/en/latest/examples.html#real-projects
+
 ### Usage
 
 Import everything (apart from testing purpose it's recommended to avoid `import *`):
 
 ```python
 >>> from ast_match import *
 >>> from pprint import pprint
@@ -75,15 +86,15 @@
 <td> 
 
 ```python
 >>> from ast_match import *
 >>> pattern=compile(expr("_last-1"))
 >>> match=pattern.fullmatch(expr("7*8-1"))
 >>> match
-Matching{'last': <ast.AST: 7 * 8>}
+Match{'last': <ast.AST: 7 * 8>}
 
 ```
 
 </td>
 </tr>
 <tr>
 <td>
@@ -120,16 +131,16 @@
 
 </td>
 <td> 
 
 ```python
 >>> pattern=compile(expr("_a*_b"))
 >>> pprint([*pattern.finditer(expr("1*2+3*4"))])
-[Matching{'a': <ast.AST: 1>, 'b': <ast.AST: 2>},
- Matching{'a': <ast.AST: 3>, 'b': <ast.AST: 4>}]
+[Match{'a': <ast.AST: 1>, 'b': <ast.AST: 2>},
+ Match{'a': <ast.AST: 3>, 'b': <ast.AST: 4>}]
 
 ```
 
 </td>
 </tr>
 </table>
 
@@ -216,7 +227,9 @@
                 left=Name(id='i', ctx=Load()),
                 op=Add(),
                 right=Constant(value=1))],
             keywords=[]))],
       orelse=[])],
   type_ignores=[])
 ```
+
+It may also be desirable to put the code into `.ipython/profile_default/startup/` or similar so that it's run automatically when IPython starts.
```

#### html2text {}

```diff
@@ -1,43 +1,48 @@
-Metadata-Version: 2.1 Name: ast-match Version: 0.0.0 Summary: A library to
+Metadata-Version: 2.1 Name: ast-match Version: 0.1.0 Summary: A library to
 facilitate easier manipulation of Python AST (abstract syntax tree) objects.
 Home-page: https://github.com/user202729/ast-match Author: user202729 License:
 GNU General Public License v3 or later (GPLv3+) Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Description-Content-Type: text/markdown License-File: LICENSE # ast-match
 A library to facilitate easier manipulation of Python AST (abstract syntax
 tree) objects. This library allows you to write the syntax in an intuitive way,
 instead of having to write the names of the internal classes in `ast` module.
 For manipulating the internal structure, it's recommended to read through
 https://docs.python.org/3/library/ast.html to know what kind of nodes may
-appear in an AST. ### Usage Import everything (apart from testing purpose it's
-recommended to avoid `import *`): ```python >>> from ast_match import * >>>
-from pprint import pprint ``` First, note that Python distinguishes between
-statement and expression, so you need to specify the type explicitly: ```python
->>> expr("a=1") Traceback (most recent call last): ... AssertionError >>> pp
-(stmt("a=1"))
+appear in an AST. It's recommended to read through these at least once (as well
+as linked documentations at the bottom of the page) at least once, it will save
+you lots of time later on. ### Limitations This module does not allow you to
+manipulate the tree in *all possible* ways. For that you still need to tinker
+with the AST itself. ### Related packages https://
+greentreesnakes.readthedocs.io/en/latest/examples.html#real-projects ### Usage
+Import everything (apart from testing purpose it's recommended to avoid `import
+*`): ```python >>> from ast_match import * >>> from pprint import pprint ```
+First, note that Python distinguishes between statement and expression, so you
+need to specify the type explicitly: ```python >>> expr("a=1") Traceback (most
+recent call last): ... AssertionError >>> pp(stmt("a=1"))
 AST: a = 1> ``` Here the `pp` function used to "pretty-print" the resulting
 `ast.AST` object. If you use IPython you may want to refer to the section below
 for automatic pretty-printing. The API somewhat resemble `re` module API:
 `re` module                            `ast_match` module
 ```python >>> import re >>>            ```python >>> from ast_match import *
 pattern=re.compile("(?P.*)-1") >>>     >>> pattern=compile(expr("_last-1")) >>>
 match=pattern.fullmatch("7*8-1") >>>   match=pattern.fullmatch(expr("7*8-1"))
-match.groupdict() {'last': '7*8'} ```  >>> match Matching{'last':
+match.groupdict() {'last': '7*8'} ```  >>> match Match{'last':
                                        AST: 7 * 8>} ```
 ```python >>> pattern=re.compile(r"    ```python >>> pattern=compile(expr("_x *
 (?P\d+)\*(?P\d+)") >>> pattern.sub     _y")) >>> pp(pattern.sub(repl(expr
 (r"\g*\g", "1*2+3*4") '2*1+4*3' ```    ("_y*_x")), expr("1*2+3*4")))
                                        AST: 2 * 1 + 4 * 3> ```
 ```python >>> pattern=re.compile(r"    ```python >>> pattern=compile(expr
 (?P\d+)\*(?P\d+)") >>> pprint(         ("_a*_b")) >>> pprint([*pattern.finditer
-[*pattern.finditer("1*2+3*4")]) [Match (expr("1*2+3*4"))]) [Matching{'a':
+[*pattern.finditer("1*2+3*4")]) [Match (expr("1*2+3*4"))]) [Match{'a':
 object; span=(0, 3), match='1*2'>,     AST: 1>, 'b':
-Match object; span=(4, 7),             AST: 2>}, Matching{'a':
+Match object; span=(4, 7),             AST: 2>}, Match{'a':
 match='3*4'>] ```                      AST: 3>, 'b':
                                        AST: 4>}] ```
 ### Note for Vim users The code inside strings may not be syntax-highlighted as
 Python code. To fix, consider adding the following to `.vim/after/syntax/
 python.vim`: ```vim syn region pythonSpecialInclude1 \ start=+\(expr\|stmt\)
 (r\?\z(['"]\)+ end=+\z1)+ keepend \ contains=pythonSpecialIncludeInner1 syn
 region pythonSpecialIncludeInner1 \ start=+\z(['"]\)\zs+ end=+\ze\z1+ keepend \
@@ -57,8 +62,10 @@
 alternative, prettier but does not show the internal #formatter.pop(ast.AST) #
 revert ``` Then the display will be more readable: ```python In [21]: ast.parse
 ('for i in range(10): print(i, i+1)') Out[21]: Module( body=[ For( target=Name
 (id='i', ctx=Store()), iter=Call( func=Name(id='range', ctx=Load()), args=
 [ Constant(value=10)], keywords=[]), body=[ Expr( value=Call( func=Name
 (id='print', ctx=Load()), args=[ Name(id='i', ctx=Load()), BinOp( left=Name
 (id='i', ctx=Load()), op=Add(), right=Constant(value=1))], keywords=[]))],
-orelse=[])], type_ignores=[]) ```
+orelse=[])], type_ignores=[]) ``` It may also be desirable to put the code into
+`.ipython/profile_default/startup/` or similar so that it's run automatically
+when IPython starts.
```

### Comparing `ast-match-0.0.0/setup.cfg` & `ast-match-0.1.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ast-match
-version = 0.0.0
+version = 0.1.0
 author = user202729
 description = A library to facilitate easier manipulation of Python AST (abstract syntax tree) objects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU General Public License v3 or later (GPLv3+)
 url = https://github.com/user202729/ast-match
 classifiers =
```

